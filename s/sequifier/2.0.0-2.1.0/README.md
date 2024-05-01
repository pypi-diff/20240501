# Comparing `tmp/sequifier-2.0.0.tar.gz` & `tmp/sequifier-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequifier-2.0.0.tar", max compression
+gzip compressed data, was "sequifier-2.1.0.tar", max compression
```

## Comparing `sequifier-2.0.0.tar` & `sequifier-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.0.0/LICENSE
--rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.0.0/README.md
--rw-r--r--   0        0        0      919 2024-04-20 13:01:12.276139 sequifier-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4392 2024-04-20 13:01:12.276497 sequifier-2.0.0/src/sequifier/config/infer_config.py
--rw-r--r--   0        0        0     2154 2024-04-20 13:01:12.276844 sequifier-2.0.0/src/sequifier/config/preprocess_config.py
--rw-r--r--   0        0        0     7002 2024-04-20 13:01:12.277183 sequifier-2.0.0/src/sequifier/config/train_config.py
--rw-r--r--   0        0        0     2321 2024-04-20 13:01:12.277557 sequifier-2.0.0/src/sequifier/helpers.py
--rw-r--r--   0        0        0    17469 2024-04-20 13:01:12.278025 sequifier-2.0.0/src/sequifier/infer.py
--rw-r--r--   0        0        0    12294 2024-04-20 13:01:12.278244 sequifier-2.0.0/src/sequifier/preprocess.py
--rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.0.0/src/sequifier/sequifier.py
--rw-r--r--   0        0        0    22884 2024-04-20 13:01:12.278993 sequifier-2.0.0/src/sequifier/train.py
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.1.0/README.md
+-rw-r--r--   0        0        0      919 2024-05-01 11:32:11.870741 sequifier-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4707 2024-05-01 11:32:11.871058 sequifier-2.1.0/src/sequifier/config/infer_config.py
+-rw-r--r--   0        0        0     1760 2024-05-01 11:32:11.871370 sequifier-2.1.0/src/sequifier/config/preprocess_config.py
+-rw-r--r--   0        0        0     7430 2024-05-01 11:32:11.871712 sequifier-2.1.0/src/sequifier/config/train_config.py
+-rw-r--r--   0        0        0     2322 2024-05-01 11:32:11.872088 sequifier-2.1.0/src/sequifier/helpers.py
+-rw-r--r--   0        0        0    21156 2024-05-01 11:32:11.872493 sequifier-2.1.0/src/sequifier/infer.py
+-rw-r--r--   0        0        0    12716 2024-05-01 11:32:11.872842 sequifier-2.1.0/src/sequifier/preprocess.py
+-rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.1.0/src/sequifier/sequifier.py
+-rw-r--r--   0        0        0    22866 2024-05-01 11:32:11.873256 sequifier-2.1.0/src/sequifier/train.py
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.1.0/PKG-INFO
```

### Comparing `sequifier-2.0.0/LICENSE` & `sequifier-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequifier-2.0.0/README.md` & `sequifier-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sequifier-2.0.0/pyproject.toml` & `sequifier-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequifier"
-version = "2.0.0"
+version = "2.1.0"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "Train a transformer model with the command line"
 keywords = ["transformer", "sequence classification", "machine learning", "sequence", "sequence modelling", "nlp", "language", "language modelling", "torch", "pytorch"]
 readme = "README.md"
 license = "BSD 3-Clause"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `sequifier-2.0.0/src/sequifier/config/infer_config.py` & `sequifier-2.1.0/src/sequifier/config/infer_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,32 @@
         dd_config_path = config_values.get("ddconfig_path")
 
         with open(
             normalize_path(dd_config_path, config_values["project_path"]), "r"
         ) as f:
             dd_config = json.loads(f.read())
 
-        config_values["column_types"] = dd_config["column_types"]
+        config_values["column_types"] = config_values.get(
+            "column_types", dd_config["column_types"]
+        )
         config_values["categorical_columns"] = [
             col for col, type_ in dd_config["column_types"].items() if type_ == "int64"
         ]
         config_values["real_columns"] = [
             col
             for col, type_ in dd_config["column_types"].items()
             if type_ == "float64"
         ]
-        config_values["data_path"] = dd_config["split_paths"][2]
+        config_values["data_path"] = normalize_path(
+            config_values.get(
+                "data_path",
+                dd_config["split_paths"][min(2, len(dd_config["split_paths"]) - 1)],
+            ),
+            config_values["project_path"],
+        )
 
     return InfererModel(**config_values)
 
 
 class InfererModel(BaseModel):
     project_path: str
     ddconfig_path: Optional[str] = None
@@ -57,15 +65,16 @@
     seed: int
     device: str
     seq_length: int
     inference_batch_size: int
 
     sample_from_distribution: bool = False
     infer_with_dropout: bool = False
-    auto_regression: bool = True
+    autoregression: bool = True
+    autoregression_additional_steps: Optional[int] = None
 
     @validator("training_config_path", always=True)
     def validate_training_config_path(cls, v):
         if not (v is None or os.path.exists(v)):
             raise ValueError(f"{v} does not exist")
 
         return v
```

### Comparing `sequifier-2.0.0/src/sequifier/config/preprocess_config.py` & `sequifier-2.1.0/src/sequifier/config/preprocess_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,24 +31,14 @@
 
     @validator("data_path", always=True)
     def validate_data_path(cls, v):
         if not os.path.exists(v):
             raise ValueError(f"{v} does not exist")
         return v
 
-    @validator("group_proportions", always=True)
-    def validate_group_proportions(cls, v):
-        if abs(sum(v) - 1) > 1e-10:
-            raise ValueError(f"does not sum to 1: {v} - {sum(v)}")
-        if len(v) < 3:
-            raise ValueError(
-                f"You need at least 3 splits of data, which correspond to training, validation and testing data"
-            )
-        return v
-
     @validator("read_format", always=True)
     def validate_read_format(cls, v):
         assert v in [
             "csv",
             "parquet",
         ], "Currently only 'csv' and 'parquet' are supported"
         return v
```

### Comparing `sequifier-2.0.0/src/sequifier/config/train_config.py` & `sequifier-2.1.0/src/sequifier/config/train_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,42 +9,55 @@
 from pydantic import BaseModel, validator
 
 from sequifier.helpers import normalize_path
 
 ANYTYPE = Union[str, int, float]
 
 
-def load_transformer_config(config_path, args_config, on_unprocessed):
+def load_train_config(config_path, args_config, on_unprocessed):
     with open(config_path, "r") as f:
         config_values = yaml.safe_load(f)
 
     config_values.update(args_config)
 
     if not on_unprocessed:
         dd_config_path = config_values.pop("ddconfig_path")
 
         with open(
             normalize_path(dd_config_path, config_values["project_path"]), "r"
         ) as f:
             dd_config = json.loads(f.read())
 
-        config_values["column_types"] = dd_config["column_types"]
+        config_values["column_types"] = config_values.get(
+            "column_types", dd_config["column_types"]
+        )
         config_values["categorical_columns"] = [
             col for col, type_ in dd_config["column_types"].items() if type_ == "int64"
         ]
         config_values["real_columns"] = [
             col
             for col, type_ in dd_config["column_types"].items()
             if type_ == "float64"
         ]
-        config_values["n_classes"] = dd_config["n_classes"]
-        config_values["training_data_path"] = dd_config["split_paths"][0]
-        config_values["validation_data_path"] = dd_config["split_paths"][1]
+        config_values["n_classes"] = config_values.get(
+            "n_classes", dd_config["n_classes"]
+        )
+        config_values["training_data_path"] = normalize_path(
+            config_values.get("training_data_path", dd_config["split_paths"][0]),
+            config_values["project_path"],
+        )
+        config_values["validation_data_path"] = normalize_path(
+            config_values.get(
+                "validation_data_path",
+                dd_config["split_paths"][min(1, len(dd_config["split_paths"]) - 1)],
+            ),
+            config_values["project_path"],
+        )
 
-    return TransformerModel(**config_values)
+    return TrainModel(**config_values)
 
 
 VALID_LOSS_FUNCTIONS = [
     "L1Loss",
     "MSELoss",
     "CrossEntropyLoss",
     "CTCLoss",
@@ -174,15 +187,15 @@
 class ModelSpecModel(BaseModel):
     d_model: int
     nhead: int
     d_hid: int
     nlayers: int
 
 
-class TransformerModel(BaseModel):
+class TrainModel(BaseModel):
     project_path: str
     model_name: Optional[str]
     training_data_path: str
     validation_data_path: str
     read_format: str = "parquet"
 
     selected_columns: Optional[list[str]]
```

### Comparing `sequifier-2.0.0/src/sequifier/helpers.py` & `sequifier-2.1.0/src/sequifier/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     else:
         targets = None
 
     sequence = {}
     for col in column_types.keys():
         f = data["inputCol"].values == col
         data_subset = data.loc[f, [str(c) for c in range(seq_length, 0, -1)]].values
+
         tens = tensor(data_subset).to(column_types[col])
 
         if to_device:
             tens = tens.to(device)
 
         sequence[col] = tens
```

### Comparing `sequifier-2.0.0/src/sequifier/infer.py` & `sequifier-2.1.0/src/sequifier/infer.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 def infer(args, args_config):
     config_path = (
         args.config_path if args.config_path is not None else "configs/infer.yaml"
     )
 
     config = load_inferer_config(config_path, args_config, args.on_unprocessed)
 
-    if config.map_to_id:
-        assert (
-            config.ddconfig_path is not None
-        ), "If you want to map to id, you need to provide a file path to a json that contains: {{'id_map':{...}}} to ddconfig_path"
+    if config.map_to_id or (len(config.real_columns) > 0):
+        assert config.ddconfig_path is not None, (
+            "If you want to map to id, you need to provide a file path to a json that contains: {{'id_map':{...}}} to ddconfig_path"
+            "\nIf you have real columns in the data, you need to provide a json that contains: {{'min_max_values':{COL_NAME:{'min':..., 'max':...}}}}"
+        )
         with open(normalize_path(config.ddconfig_path, config.project_path), "r") as f:
-            id_maps = json.loads(f.read())["id_maps"]
+            dd_config = json.loads(f.read())
+            id_maps = dd_config["id_maps"]
+            min_max_values = dd_config["min_max_values"]
     else:
         id_maps = None
 
     inferer = Inferer(
         config.model_path,
         config.project_path,
         id_maps,
+        min_max_values,
         config.map_to_id,
         config.categorical_columns,
         config.real_columns,
         config.target_columns,
         config.target_column_types,
         config.sample_from_distribution,
         config.infer_with_dropout,
@@ -57,19 +61,23 @@
     )
 
     print(f"Inferring for {model_id}")
     data = read_data(config.data_path, config.read_format)
     if config.selected_columns is not None:
         data = subset_to_selected_columns(data, config.selected_columns)
 
-    if not config.auto_regression:
+    if not config.autoregression:
         probs, preds = get_probs_preds(config, inferer, data, column_types)
     else:
-        probs, preds = get_probs_preds_auto_regression(
-            config, inferer, data, column_types
+        if config.autoregression_additional_steps is not None:
+            data = expand_data_by_autoregression(
+                data, config.autoregression_additional_steps, config.seq_length
+            )
+        probs, preds = get_probs_preds_autoregression(
+            config, inferer, data, column_types, config.seq_length
         )
 
     if inferer.map_to_id:
         for target_column, predictions in preds.items():
             if target_column in inferer.index_map:
                 preds[target_column] = np.array(
                     [inferer.index_map[target_column][i] for i in predictions]
@@ -94,56 +102,104 @@
                 )
                 print(f"Writing probabilities to {probabilities_path}")
                 write_data(
                     pd.DataFrame(probs[target_column]),
                     probabilities_path,
                     config.write_format,
                 )
-
-    for target_column in inferer.target_columns:
-        predictions_path = os.path.join(
-            config.project_path,
-            "outputs",
-            "predictions",
-            f"{model_id}-{target_column}-predictions.{config.write_format}",
-        )
-        print(f"Writing predictions to {predictions_path}")
-        write_data(
-            pd.DataFrame(preds[target_column], columns=["model_output"]),
-            predictions_path,
-            config.write_format,
-        )
+    n_input_cols = len(np.unique(data["inputCol"]))
+    predictions = pd.DataFrame(
+        {
+            **{"sequenceId": list(data["sequenceId"].values)[::n_input_cols]},
+            **{
+                target_column: preds[target_column].flatten()
+                for target_column in inferer.target_columns
+            },
+        }
+    )
+    predictions_path = os.path.join(
+        config.project_path,
+        "outputs",
+        "predictions",
+        f"{model_id}-predictions.{config.write_format}",
+    )
+    print(f"Writing predictions to {predictions_path}")
+    write_data(
+        predictions,
+        predictions_path,
+        config.write_format,
+    )
     print("Inference complete")
 
 
+def expand_data_by_autoregression(data, autoregression_additional_steps, seq_length):
+    autoregression_additional_observations = []
+    for sequence_id, sequence_data in data.groupby("sequenceId"):
+        max_subsequence_id = sequence_data["subsequenceId"].values.max()
+        last_observation = sequence_data.query(f"subsequenceId=={max_subsequence_id}")
+
+        for offset in range(1, autoregression_additional_steps + 1):
+            sequence_id_fields = np.repeat(sequence_id, last_observation.shape[0])
+            subsequence_id_fields = np.repeat(
+                max_subsequence_id + offset, last_observation.shape[0]
+            )
+            input_col_fields = last_observation["inputCol"].values
+            empty_data_fields = (
+                np.ones((last_observation.shape[0], min(seq_length, offset))) * np.inf
+            )
+            data_cols = [str(c) for c in range(seq_length, 0, -1)]
+            offset_data_fields = last_observation[data_cols].values[
+                :, min(offset, last_observation.shape[1]) :
+            ]
+            data_fields = np.concatenate(
+                [offset_data_fields, empty_data_fields], axis=1
+            )
+            metadata = pd.DataFrame(
+                {
+                    "sequenceId": sequence_id_fields,
+                    "subsequenceId": subsequence_id_fields,
+                    "inputCol": input_col_fields,
+                }
+            )
+            data_df = pd.DataFrame(data_fields, columns=data_cols)
+            observation = pd.concat([metadata, data_df], axis=1)
+            autoregression_additional_observations.append(observation)
+
+    data = pd.concat(
+        [data] + autoregression_additional_observations, axis=0
+    ).sort_values(["sequenceId", "subsequenceId"])
+
+    return data
+
+
 def get_probs_preds(config, inferer, data, column_types):
+
     X, _ = numpy_to_pytorch(
         data,
         column_types,
         config.target_columns,
         config.seq_length,
         config.device,
         to_device=True,
     )
     X = {col: X_col.numpy() for col, X_col in X.items()}
 
     del data
 
     if config.output_probabilities:
         probs = inferer.infer(X, return_probs=True)
-
         preds = inferer.infer(None, probs)
     else:
         probs = None
         preds = inferer.infer(X)
 
     return (probs, preds)
 
 
-def get_probs_preds_auto_regression(config, inferer, data, column_types):
+def get_probs_preds_autoregression(config, inferer, data, column_types, seq_length):
     sequence_ids = data["sequenceId"].values
     subsequence_ids = data["subsequenceId"].values
     assert (
         np.all(sequence_ids[1:] - sequence_ids[:-1]) >= 0
     ), "sequenceId must be in ascending order for autoregression"
     assert (
         np.all(subsequence_ids[1:] - subsequence_ids[:-1]) >= 0
@@ -156,22 +212,23 @@
             sequence_data["subsequenceId"].values[1:]
             >= sequence_data["subsequenceId"].values[:-1]
         )
 
     n_input_col_values = len(np.unique(data["inputCol"]))
     preds_list, probs_list, indices = [], [], []
     subsequence_ids = sorted(list(np.unique(data["subsequenceId"])))
+    max_subsequence_id = np.max(subsequence_ids)
     for subsequence_id in subsequence_ids:
         data_subset = data.loc[data["subsequenceId"] == subsequence_id, :]
         probs, preds = get_probs_preds(config, inferer, data_subset, column_types)
         preds_list.append(preds)
         if probs is not None:
             probs_list.append(probs)
 
-        for offset in range(1, int(list(data.columns)[3])):
+        for offset in range(1, seq_length + 1):
             target_subsequence_filter = data["subsequenceId"].values == (
                 subsequence_id + offset
             )  # filter all data on target subsequence id
             data_subset_sequence_ids = sorted(
                 list(np.unique(data_subset["sequenceId"]))
             )
             sequence_filter = np.array(
@@ -240,14 +297,22 @@
                         == f_data_subset["sequenceId"].values
                     )
                 assert np.all(
                     (f_data_subset["subsequenceId"].values + 1) == (subsequence_id + 1)
                 ), f"{f_data_subset['subsequenceId'].values + 1} != {(subsequence_id + 1)}"
                 for target_column, f in fs.items():
                     data.loc[f, str(offset)] = f_preds[target_column]
+        data_subset = data.loc[data["subsequenceId"] == subsequence_id, :]
+        assert (
+            np.any(
+                np.abs(data_subset[[str(c) for c in range(seq_length, 0, -1)]])
+                == np.inf
+            )
+            == False
+        ), data_subset
 
     preds = {
         target_column: np.concatenate([p[target_column] for p in preds_list], axis=0)
         for target_column in inferer.target_columns
     }
     if len(probs_list):
         probs = {
@@ -263,27 +328,29 @@
 
 class Inferer(object):
     def __init__(
         self,
         model_path,
         project_path,
         id_map,
+        min_max_values,
         map_to_id,
         categorical_columns,
         real_columns,
         target_columns,
         target_column_types,
         sample_from_distribution,
         infer_with_dropout,
         inference_batch_size,
         device,
         args_config,
         training_config_path,
     ):
         self.map_to_id = map_to_id
+        self.min_max_values = min_max_values
         if self.map_to_id:
             self.index_map = {}
             for target_column in target_columns:
                 if target_column_types[target_column] == "categorical":
                     map_ = (
                         {v: k for k, v in id_map[target_column].items()}
                         if map_to_id
@@ -329,14 +396,21 @@
                 normalize_path(model_path, project_path),
                 self.training_config_path,
                 self.args_config,
                 self.device,
                 self.infer_with_dropout,
             )
 
+    def invert_normalization(self, values, target_column):
+        min_ = self.min_max_values[target_column]["min"]
+        max_ = self.min_max_values[target_column]["max"]
+        return np.array(
+            [(((v + 1.0) / 2.0) * (max_ - min_)) + min_ for v in values.flatten()]
+        ).reshape(*values.shape)
+
     def infer(
         self, x, probs=None, return_probs=False
     ):  # probs are of type Optional[dict[str, np.ndarray]]
         if probs is None or (
             x is not None and len(set(x.keys()).difference(set(probs.keys()))) > 0
         ):
             size = x[self.target_columns[0]].shape[0]
@@ -356,23 +430,26 @@
 
                 outs = {
                     target_column: np.concatenate(
                         [out_sub[target_column] for out_sub in out_subs], axis=0
                     )[:size, :]
                     for target_column in self.target_columns
                 }
+
             if self.inference_model_type == "pt":
                 x_adjusted = self.prepare_inference_batches(x, pad_to_batch_size=False)
                 outs = infer_with_model(
                     self.inference_model,
                     x_adjusted,
                     self.device,
                     size,
                     self.target_columns,
                 )
+            for target_column, target_outs in outs.items():
+                assert np.any(target_outs == np.inf) == False, target_outs
 
             if return_probs:
                 preds = {
                     target_column: outputs
                     for target_column, outputs in outs.items()
                     if self.target_column_types[target_column] != "categorical"
                 }
@@ -385,16 +462,24 @@
         else:
             outs = dict(probs)
         for target_column in self.target_columns:
             if self.target_column_types[target_column] == "categorical":
                 if self.sample_from_distribution is False:
                     outs[target_column] = outs[target_column].argmax(1)
                 else:
-                    outs[target_column] = sample_with_cumsum(outs[target_column])
-
+                    try:
+                        outs[target_column] = sample_with_cumsum(outs[target_column])
+                    except:
+                        import code
+
+                        code.interact(local=locals())
+
+        for target_column, output in outs.items():
+            if self.target_column_types[target_column] == "real":
+                outs[target_column] = self.invert_normalization(output, target_column)
         return outs
 
     def prepare_inference_batches(self, x, pad_to_batch_size):
         size = x[self.target_columns[0]].shape[0]
         if size == self.inference_batch_size:
             return [x]
         elif size < self.inference_batch_size:
```

### Comparing `sequifier-2.0.0/src/sequifier/preprocess.py` & `sequifier-2.1.0/src/sequifier/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,36 @@
         ]
 
         data_columns = [
             col for col in data.columns if col not in ["sequenceId", "itemPosition"]
         ]
 
         n_classes, id_maps = {}, {}
+        min_max_values = {}
         float_data_columns = []
         for data_col in data_columns:
             dtype = str(data[data_col].dtype)
             if dtype in ["object", "int64"]:
                 data, sup_id_map = replace_ids(data, column=data_col)
                 id_maps[data_col] = dict(sup_id_map)
                 n_classes[data_col] = len(np.unique(data[data_col])) + 1
             elif dtype in ["float64"]:
+                min_ = np.min(data[data_col].values)
+                max_ = np.max(data[data_col].values)
+                data[data_col] = [
+                    (((v - min_) / (max_ - min_)) * 2.0) - 1.0 for v in data[data_col]
+                ]
+                min_max_values[data_col] = {"min": min_, "max": max_}
                 float_data_columns.append(data_col)
             else:
                 raise Exception(
                     f"Column {data_col} is of dtype {dtype}, which is not supported"
                 )
         col_types = {col: str(data[col].dtype) for col in data_columns}
-        self.export_metadata(id_maps, n_classes, col_types)
+        self.export_metadata(id_maps, n_classes, col_types, min_max_values)
 
         data = data.sort_values(["sequenceId", "itemPosition"])
 
         n_cores = n_cores if n_cores is not None else multiprocessing.cpu_count()
 
         batch_limits = get_batch_limits(data, n_cores)
         batches = [
@@ -126,21 +133,22 @@
         )
 
         delete_path = os.path.join(project_path, "data", "temp")
         assert len(delete_path) > 9
         delete_command = f"rm -rf {delete_path}*"
         os.system(delete_command)
 
-    def export_metadata(self, id_maps, n_classes, col_types):
+    def export_metadata(self, id_maps, n_classes, col_types, min_max_values):
 
         data_driven_config = {
             "n_classes": n_classes,
             "id_maps": id_maps,
             "split_paths": self.split_paths,
             "column_types": col_types,
+            "min_max_values": min_max_values,
         }
         os.makedirs(
             os.path.join(self.project_path, "configs", "ddconfigs"), exist_ok=True
         )
 
         with open(
             os.path.join(
```

### Comparing `sequifier-2.0.0/src/sequifier/sequifier.py` & `sequifier-2.1.0/src/sequifier/sequifier.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.0.0/src/sequifier/train.py` & `sequifier-2.1.0/src/sequifier/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 import numpy as np
 import pandas as pd
 import torch
 from torch import Tensor, nn
 from torch.nn import ModuleDict, TransformerEncoder, TransformerEncoderLayer
 
-from sequifier.config.train_config import load_transformer_config
+from sequifier.config.train_config import load_train_config
 from sequifier.helpers import (PANDAS_TO_TORCH_TYPES, LogFile, normalize_path,
                                numpy_to_pytorch, read_data,
                                subset_to_selected_columns)
 
 
 def train(args, args_config):
     config_path = (
         args.config_path if args.config_path is not None else "configs/train.yaml"
     )
 
-    config = load_transformer_config(config_path, args_config, args.on_unprocessed)
+    config = load_train_config(config_path, args_config, args.on_unprocessed)
 
     column_types = {
         col: PANDAS_TO_TORCH_TYPES[config.column_types[col]]
         for col in config.column_types
     }
 
     data_train = read_data(
@@ -582,15 +582,15 @@
         else:
             return None
 
 
 def load_inference_model(
     model_path, training_config_path, args_config, device, infer_with_dropout
 ):
-    training_config = load_transformer_config(
+    training_config = load_train_config(
         training_config_path, args_config, args_config["on_unprocessed"]
     )
 
     with torch.no_grad():
 
         model = TransformerModel(training_config)
         model.log_file.write(f"Loading model weights from {model_path}")
```

### Comparing `sequifier-2.0.0/PKG-INFO` & `sequifier-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequifier
-Version: 2.0.0
+Version: 2.1.0
 Summary: Train a transformer model with the command line
 Home-page: https://github.com/0xideas/sequifier
 License: BSD 3-Clause
 Keywords: transformer,sequence classification,machine learning,sequence,sequence modelling,nlp,language,language modelling,torch,pytorch
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.9,<4.0
```

