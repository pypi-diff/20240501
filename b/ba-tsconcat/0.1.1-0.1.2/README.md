# Comparing `tmp/ba_tsconcat-0.1.1.tar.gz` & `tmp/ba_tsconcat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ba_tsconcat-0.1.1.tar", max compression
+gzip compressed data, was "ba_tsconcat-0.1.2.tar", max compression
```

## Comparing `ba_tsconcat-0.1.1.tar` & `ba_tsconcat-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    26190 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/LICENSE
--rw-r--r--   0        0        0     2779 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/README.md
--rw-r--r--   0        0        0     1695 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      262 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/__init__.py
--rw-r--r--   0        0        0     5911 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/cli.py
--rw-r--r--   0        0        0     1139 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/concat.py
--rw-r--r--   0        0        0     2623 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/pretreeprint.py
--rw-r--r--   0        0        0     2793 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/utils.py
--rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26190 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2779 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/README.md
+-rw-r--r--   0        0        0     1778 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/__init__.py
+-rw-r--r--   0        0        0     6511 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/cli.py
+-rw-r--r--   0        0        0     1565 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/concat.py
+-rw-r--r--   0        0        0     2623 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/pretreeprint.py
+-rw-r--r--   0        0        0     2829 2024-05-01 16:03:10.204197 ba_tsconcat-0.1.2/src/tsconcat/utils.py
+-rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.2/PKG-INFO
```

### Comparing `ba_tsconcat-0.1.1/LICENSE` & `ba_tsconcat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.1/README.md` & `ba_tsconcat-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.1/pyproject.toml` & `ba_tsconcat-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ba-tsconcat"
-version = "0.1.1"
+version = "0.1.2"
 description = "BIDS App and Python library for concatenating MRI time series."
 authors = ["CMI DAIR Center <florian.rupprecht@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "tsconcat", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -62,18 +62,19 @@
 ]
 line-length = 120
 indent-width = 4
 src = ["src"]
 target-version = "py311"
 
 [tool.ruff.lint]
-select = ["ANN", "D", "E", "F", "I"]
+select = ["ANN", "D", "E", "F", "I", "PD", "NPY"]
 ignore = [
   "ANN101",  # self should not be annotated.
-  "ANN102"  # cls should not be annotated.
+  "ANN102",  # cls should not be annotated.
+  "PD901"  # Avoid using the generic variable name df for DataFrames
 ]
 fixable = ["ALL"]
 unfixable = []
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.format]
 quote-style = "double"
```

### Comparing `ba_tsconcat-0.1.1/src/tsconcat/cli.py` & `ba_tsconcat-0.1.2/src/tsconcat/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """CLI for tsconcat."""
 
+import argparse
 import json
 import pathlib as pl
 from collections.abc import Callable
-from typing import List, Optional
+from dataclasses import dataclass
+from typing import Any, List, Optional
 
 import bids2table.table
 import elbow.dtypes  # noqa  makes pandas load json types as dicts from parquet
 import elbow.utils
 import pandas as pd
 
 from .concat import concat_nifti1_4d
@@ -46,15 +48,15 @@
     group_by_set = set(REDUCE_COLUMNS_ALIAS.get(g, g) for g in group_by)
 
     unknown_cols = list(group_by_set - REDUCE_COLUMNS_SET)
     if len(unknown_cols) > 0:
         raise Exception(f"Unknown columns: {unknown_cols}")
     del unknown_cols
 
-    df.sort_values(by=REDUCE_COLUMNS, inplace=True)
+    df = df.sort_values(by=REDUCE_COLUMNS)
 
     grouped = df.groupby(by=list(REDUCE_COLUMNS_SET - group_by_set), dropna=False)
 
     def _func_reduce(df_group: pd.DataFrame) -> Optional[pd.Series]:
         if df_group.shape[0] == 0:
             print("empty group")
             return None
@@ -77,16 +79,16 @@
 def _read_if_parquet(p: pl.Path, *args, **kwargs) -> Optional[pd.DataFrame]:  # noqa
     try:
         return pd.read_parquet(p, *args, **kwargs)
     except:  # noqa
         return None
 
 
-def main() -> None:
-    """Concatenate MRI timeseries."""
+def build_parser_tsconcat_bids_app() -> argparse.ArgumentParser:
+    """Build parser for tsconcat BIDS app."""
     parser = build_bidsapp_group_parser(prog="ba-tsconcat", description="Concatenate MRI timeseries.")
 
     parser.add_argument(
         "-c",
         "--concat",
         type=str,
         help=f"Concat across. Can be any combination of {', '.join(REDUCE_COLUMNS_ALIAS.keys())} separated by spaces. "
@@ -116,89 +118,103 @@
         "-w",
         "--workers",
         type=int,
         help="Number of workers for bids2table. Default is 1.",
         default=1,
     )
 
-    args = parser.parse_args()
+    return parser
+
+
+@dataclass
+class TSConcatSettings:
+    """Settings for tsconcat."""
+
+    input_dir: pl.Path
+    output_dir: pl.Path
+    concat_labels: List[str]
+    dry_run: bool
+    fake: bool
+    workers: int
+
+    @classmethod
+    def from_args(cls, args: Any) -> "TSConcatSettings":  # noqa
+        return cls(
+            input_dir=args.bids_dir,
+            output_dir=args.output_dir,
+            concat_labels=args.concat.split(" "),
+            dry_run=args.dry_run or args.fake,
+            fake=args.fake,
+            workers=args.workers,
+        )
 
-    input_dir: pl.Path = args.bids_dir
-    output_dir: pl.Path = args.output_dir
-    concat_labels: List[str] = args.concat.split(" ")
-    dry_run: bool = args.dry_run
-    fake: bool = args.fake
-    dry_run = dry_run or fake
-    workers: int = args.workers
 
-    if not input_dir.exists():
+def main() -> None:
+    """Concatenate MRI timeseries."""
+    settings = TSConcatSettings.from_args(build_parser_tsconcat_bids_app().parse_args())
+
+    if not settings.input_dir.exists():
         raise Exception("Input directory does not exist.")
 
-    if dry_run and (df := _read_if_parquet(input_dir)) is not None:
+    if settings.dry_run and (df := _read_if_parquet(settings.input_dir)) is not None:
         df = bids2table.table.flat_to_multi_columns(df)
     else:
-        df = bids2table.bids2table(input_dir, workers=workers)
+        df = bids2table.bids2table(settings.input_dir, workers=settings.workers)
 
         if df.shape[0] == 0:
             raise Exception("Empty BIDS dataset")
 
-    if not dry_run:
-        output_dir.mkdir(parents=True, exist_ok=True)
-
-    # print dataframe columns
-    print(df.columns)
+    if not settings.dry_run:
+        settings.output_dir.mkdir(parents=True, exist_ok=True)
 
     df_bold = df.query(
         "ent__datatype == 'func' and "
         "ent__ext == '.nii.gz' and "
-        "ent__suffix == 'bold'"# and "
-        #"ent__desc == 'preproc' and "
-        #"ent__space == 'MNI152NLin6ASym'"
-    )
-
-    print(df)
-    print(df_bold)
+        "ent__suffix == 'bold'"  # and "
+        # "ent__desc == 'preproc' and "
+        # "ent__space == 'MNI152NLin6ASym'"
+    )  # fmt: skip
 
     if df_bold.shape[0] == 0:
         raise Exception("No BOLD files found")
 
     def _process_group(df_group: pd.DataFrame) -> None:
-        group_identifiers = df_group.iloc[0][list(REDUCE_COLUMNS_SET - set(concat_labels))].to_dict()
+        group_identifiers = df_group.iloc[0][list(REDUCE_COLUMNS_SET - set(settings.concat_labels))].to_dict()
         print(f"Process group: {group_identifiers}")
 
         first_row: pd.Series = df_group.iloc[0]
 
-        for group_label in concat_labels:
+        for group_label in settings.concat_labels:
             first_row[group_label] = None  # todo does vectorized work here?
 
         # Generate file
 
-        file_path = output_dir / file_path_from_b2table_row(first_row)
+        file_path = settings.output_dir / file_path_from_b2table_row(first_row)
 
         file_path.parent.mkdir(parents=True, exist_ok=True)
         concat_nifti1_4d(paths=df_group.finfo__file_path.values, out_path=file_path)
 
         # Generate sidecar
 
-        sidecar_path = output_dir / sidecar_path_from_b2table_row(first_row)
+        sidecar_path = settings.output_dir / sidecar_path_from_b2table_row(first_row)
         sidecar_contents = first_row["meta__json"]  # TODO: Maybe add list of files that were concatenated?
         with open(sidecar_path, "w", encoding="utf-8") as fp:
             json.dump(sidecar_contents, fp)
 
     df_reduced_bold = _reduce_op(
         df_bold,
-        group_by=concat_labels,
-        group_callback=None if dry_run else _process_group,
+        group_by=settings.concat_labels,
+        group_callback=None if settings.dry_run else _process_group,
     )
 
-    if fake:
+    if settings.fake:
         df_reduced_bold = df_reduced_bold.astype(
-            {"sidecar": "json", "dataset_description": "json", "extra_entities": "json"}
+            {"meta__json": "json", "ds__dataset_description": "json", "ent__extra_entities": "json"}
         )
-        df_reduced_bold.to_parquet(output_dir)
+        df_reduced_bold.to_parquet(settings.output_dir)
 
     filepaths = file_paths_from_b2table(df_reduced_bold, include_sidecars=True)
     pretreeprint(filepaths)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ba_tsconcat-0.1.1/src/tsconcat/concat.py` & `ba_tsconcat-0.1.2/src/tsconcat/concat.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,19 +22,30 @@
     paths = [pl.Path(p) for p in paths]
 
     if len(paths) == 0:
         raise Exception("Empty path list.")
 
     img_handles: List[nib.nifti1.Nifti1Image] = [nib.nifti1.Nifti1Image.load(p) for p in paths]  # type: ignore
 
+    img_shapes: List[tuple] = [img.shape for img in img_handles]
+
+    # All 4D
+    if not np.all([len(shape) == 4 for shape in img_shapes]):
+        raise Exception("Images must be 4D.")
+
+    # First 3 dimensions must be equal
+    if not np.all([img_shapes[0][:-1] == shape[:-1] for shape in img_shapes]):
+        raise Exception("Spatial shapes must be equal.")
+
     img_affines: List[np.ndarray] = [img.affine for img in img_handles]
 
     affs = np.asarray(img_affines)
     if not np.all(affs == affs[0, :, :]):
         raise Exception("Affines must be equal.")
 
+    # Should this use the _dataobj to preserve integer types?
     img_arrays = [img.get_fdata() for img in img_handles]
 
     concat = np.concatenate(img_arrays, axis=3)
 
     concat_n1 = nib.nifti1.Nifti1Image(concat, img_affines[0])
     nib.nifti1.save(concat_n1, out_path)
```

### Comparing `ba_tsconcat-0.1.1/src/tsconcat/pretreeprint.py` & `ba_tsconcat-0.1.2/src/tsconcat/pretreeprint.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.1/src/tsconcat/utils.py` & `ba_tsconcat-0.1.2/src/tsconcat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     print(f"Start: {title}")
     start = time.perf_counter()
     yield
     duration = time.perf_counter() - start
     print(f"Done: {title} - {datetime.timedelta(seconds=duration)}")
 
 
-def build_bidsapp_group_parser(*args, **kwargs):  # noqa
+def build_bidsapp_group_parser(*args, **kwargs) -> argparse.ArgumentParser:  # noqa
     """Build a parser skeleton for the BIDS App group level.
 
     Args:
         args: Positional arguments to be passed to ArgumentParser costructor.
         kwargs: Keyword arguments to be passed to ArgumentParser costructor.
     """
     parser = argparse.ArgumentParser(*args, **kwargs)
@@ -50,15 +50,15 @@
 
 
 def file_paths_from_b2table(df: pd.DataFrame, include_sidecars: bool = False, inplace: bool = False) -> List[pl.Path]:
     """Generate list of filepaths from bids2table dataframe."""
     # b2t crashes if sidecar is not None
     if not inplace:
         df = df.copy()
-    df["sidecar"] = None
+    df["meta__json"] = None
 
     paths = list(df.apply(func=lambda row: bids2table.table.join_bids_path(row), axis=1).values)
 
     if include_sidecars:
         sidecar_paths = list(
             df.apply(
                 func=lambda row: bids2table.table.join_bids_path({**row, "ext": ".json"}),
@@ -71,23 +71,23 @@
 
 
 def file_path_from_b2table_row(row: pd.Series, inplace: bool = False, sidecar: bool = False) -> pl.Path:
     """Generate list of filepaths from bids2table dataframe."""
     # b2t crashes if sidecar is not None
     if not inplace:
         row = row.copy()
-    row["sidecar"] = None
+    row["meta__json"] = None
 
     if sidecar:
         row = {**row, "ext": ".json"}
 
     return bids2table.table.join_bids_path(row)
 
 
 def sidecar_path_from_b2table_row(row: pd.Series, inplace: bool = False) -> pl.Path:
     """Generate list of filepaths from bids2table dataframe."""
     # b2t crashes if sidecar is not None
     if not inplace:
         row = row.copy()
-    row["sidecar"] = None
+    row["meta__json"] = None
 
     return bids2table.table.join_bids_path({**row, "ext": ".json"})
```

### Comparing `ba_tsconcat-0.1.1/PKG-INFO` & `ba_tsconcat-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ba-tsconcat
-Version: 0.1.1
+Version: 0.1.2
 Summary: BIDS App and Python library for concatenating MRI time series.
 License: LGPL-2.1
 Author: CMI DAIR Center
 Author-email: florian.rupprecht@childmind.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

