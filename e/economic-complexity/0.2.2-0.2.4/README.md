# Comparing `tmp/economic_complexity-0.2.2.tar.gz` & `tmp/economic_complexity-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "economic_complexity-0.2.2.tar", max compression
+gzip compressed data, was "economic_complexity-0.2.4.tar", max compression
```

## Comparing `economic_complexity-0.2.2.tar` & `economic_complexity-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      729 2024-02-19 20:48:16.918396 economic_complexity-0.2.2/economic_complexity/__init__.py
--rw-r--r--   0        0        0     2347 2024-02-12 18:55:17.497358 economic_complexity-0.2.2/economic_complexity/complexity.py
--rw-r--r--   0        0        0     4234 2024-02-12 18:58:16.649172 economic_complexity-0.2.2/economic_complexity/cross_space.py
--rw-r--r--   0        0        0      333 2023-10-10 19:49:15.175456 economic_complexity-0.2.2/economic_complexity/polars/__init__.py
--rw-r--r--   0        0        0     1931 2023-10-10 19:43:59.681950 economic_complexity-0.2.2/economic_complexity/polars/complexity.py
--rw-r--r--   0        0        0     4072 2023-10-10 19:54:12.279666 economic_complexity-0.2.2/economic_complexity/polars/product_space.py
--rw-r--r--   0        0        0     3502 2024-02-12 19:14:10.679688 economic_complexity-0.2.2/economic_complexity/polars/rca.py
--rw-r--r--   0        0        0     1460 2024-02-12 19:12:48.819813 economic_complexity-0.2.2/economic_complexity/polars/run.py
--rw-r--r--   0        0        0    13712 2024-02-19 19:56:06.621539 economic_complexity-0.2.2/economic_complexity/product_space.py
--rw-r--r--   0        0        0     1431 2022-11-15 21:12:43.234320 economic_complexity-0.2.2/economic_complexity/rca.py
--rw-r--r--   0        0        0     2592 2024-02-19 18:38:03.638357 economic_complexity-0.2.2/economic_complexity/subnational.py
--rw-r--r--   0        0        0     1071 2022-05-06 03:32:39.758645 economic_complexity-0.2.2/LICENSE
--rw-r--r--   0        0        0     3293 2024-02-12 19:27:28.239850 economic_complexity-0.2.2/PACKAGE.md
--rw-r--r--   0        0        0      913 2024-02-19 20:40:06.714952 economic_complexity-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4282 1970-01-01 00:00:00.000000 economic_complexity-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-05-05 23:32:40.000000 economic_complexity-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3293 2024-05-01 04:10:31.568897 economic_complexity-0.2.4/PACKAGE.md
+-rw-r--r--   0        0        0      783 2024-05-01 05:03:05.956516 economic_complexity-0.2.4/economic_complexity/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-01 04:10:31.569897 economic_complexity-0.2.4/economic_complexity/complexity.py
+-rw-r--r--   0        0        0     4234 2024-05-01 04:10:31.569897 economic_complexity-0.2.4/economic_complexity/cross_space.py
+-rw-r--r--   0        0        0      333 2024-05-01 04:10:31.569897 economic_complexity-0.2.4/economic_complexity/polars/__init__.py
+-rw-r--r--   0        0        0     1931 2023-10-10 15:44:00.000000 economic_complexity-0.2.4/economic_complexity/polars/complexity.py
+-rw-r--r--   0        0        0     4072 2023-10-10 15:54:14.000000 economic_complexity-0.2.4/economic_complexity/polars/product_space.py
+-rw-r--r--   0        0        0     3253 2024-05-01 04:56:15.680891 economic_complexity-0.2.4/economic_complexity/polars/rca.py
+-rw-r--r--   0        0        0     1460 2024-02-12 15:12:50.000000 economic_complexity-0.2.4/economic_complexity/polars/run.py
+-rw-r--r--   0        0        0    14984 2024-05-01 04:19:49.408111 economic_complexity-0.2.4/economic_complexity/product_space.py
+-rw-r--r--   0        0        0     1431 2024-05-01 04:10:31.569897 economic_complexity-0.2.4/economic_complexity/rca.py
+-rw-r--r--   0        0        0     2592 2024-05-01 04:10:31.569897 economic_complexity-0.2.4/economic_complexity/subnational.py
+-rw-r--r--   0        0        0      912 2024-05-01 05:02:59.723477 economic_complexity-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 economic_complexity-0.2.4/PKG-INFO
```

### Comparing `economic_complexity-0.2.2/economic_complexity/__init__.py` & `economic_complexity-0.2.4/economic_complexity/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from .product_space import (
     distance,
     opportunity_gain,
     peii,
     pgi,
     proximity,
     relatedness,
+    relative_relatedness,
     similarity,
 )
 from .rca import rca
 from .subnational import complexity_subnational
 
-__version_info__ = ("0", "2", "2")
+__version_info__ = ("0", "2", "4")
 __version__ = ".".join(__version_info__)
 
 __all__ = (
     "rca",
     "complexity",
     "distance",
     "opportunity_gain",
@@ -29,8 +30,9 @@
     "relatedness",
     "cross_proximity",
     "cross_relatedness",
     "similarity",
     "pgi",
     "peii",
     "complexity_subnational",
+    "relative_relatedness",
 )
```

### Comparing `economic_complexity-0.2.2/economic_complexity/complexity.py` & `economic_complexity-0.2.4/economic_complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/economic_complexity/cross_space.py` & `economic_complexity-0.2.4/economic_complexity/cross_space.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/economic_complexity/polars/complexity.py` & `economic_complexity-0.2.4/economic_complexity/polars/complexity.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/economic_complexity/polars/product_space.py` & `economic_complexity-0.2.4/economic_complexity/polars/product_space.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/economic_complexity/polars/rca.py` & `economic_complexity-0.2.4/economic_complexity/polars/rca.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,45 +58,38 @@
 
     # Get LazyFrame
     lf = df if isinstance(df, pl.LazyFrame) else df.lazy()
 
     lf = lf.fill_nan(0).fill_null(0)
 
     # Calculate sum of measure per activity
-    total_activity = lf.groupby(by=activity).agg(
+    total_activity = lf.group_by(activity).agg(
         pl.sum(measure).alias("_sum_by_activity")
     )
 
     # Calculate sum of measure per location
-    total_location = lf.groupby(by=location).agg(
+    total_location = lf.group_by(location).agg(
         pl.sum(measure).alias("_sum_by_location")
     )
 
     # Merge sums of measure per activity and per location
     merged = lf.join(total_activity, on=activity).join(total_location, on=location)
 
-    # Calculate the total sum of the measure
-    total_measure = total_activity.select(
-        pl.col("_sum_by_activity").alias("_total_measure_sum")
-    ).sum()
-
     # Build the expression for the column division that calculates the RCA
-    rca_expr = (
-        (pl.col(measure) / pl.col("_sum_by_location"))
-        / (pl.col("_sum_by_activity") / pl.first("_total_measure_sum"))
+    rca_expr = (pl.col(measure) / pl.col("_sum_by_location")) / (
+        pl.col("_sum_by_activity") / pl.sum(measure)
     )
     # Do the calculation
-    rca = merged\
-        .with_context(total_measure)\
-        .with_columns(rca_expr.alias(measure + " RCA"))\
-        .drop(["_sum_by_activity", "_sum_by_location"])
+    rca = merged.with_columns(rca_expr.alias(measure + " RCA")).drop(
+        ["_sum_by_activity", "_sum_by_location"]
+    )
 
     # Apply binarization of matrix
     if binary:
         rca = rca.with_columns(
             pl.when(pl.col(measure + " RCA") >= cutoff)
-                .then(1.0)
-                .otherwise(0.0)
-                .alias(measure + " RCA")
+            .then(1.0)
+            .otherwise(0.0)
+            .alias(measure + " RCA")
         )
 
     return rca
```

### Comparing `economic_complexity-0.2.2/economic_complexity/polars/run.py` & `economic_complexity-0.2.4/economic_complexity/polars/run.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/economic_complexity/product_space.py` & `economic_complexity-0.2.4/economic_complexity/product_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""Product Space module
-"""
+"""Product Space module"""
 
-from typing import Optional
+from typing import Literal, Optional
 
 import numpy as np
 import pandas as pd
-from typing_extensions import Literal
 
 
 def proximity(
     df_rca: pd.DataFrame,
     *,
     cutoff: float = 1,
     procedure: Literal["max", "sqrt"] = "max",
@@ -374,7 +372,49 @@
     ### Returns:
     (pandas.DataFrame) -- PEII matrix with categories evaluated as an index.
     """
 
     peii = _pmi(tbl=tbl, rcas=rcas, measure=emissions, cutoff=cutoff)
     peii.rename(columns={peii.columns[0]: name}, inplace=True)
     return peii
+
+
+def relative_relatedness(
+    rcas: pd.DataFrame,
+    *,
+    cutoff: float = 1,
+    proximities: Optional[pd.DataFrame] = None,
+) -> pd.DataFrame:
+    """Calculates the Relative Relatedness, given a matrix of RCAs for the economic
+    activities of a location, and a matrix of Proximities.
+
+    ### Args:
+    * rcas (pd.DataFrame) -- Matrix of RCAs for a certain location.
+
+    ### Keyword Args:
+    * cutoff (float, optional) -- Set the cutoff threshold value.
+        Internally, RCA values under it will be set to zero, one otherwise.
+        Default value: `1`.
+    * proximities (pd.DataFrame, optional) -- Matrix with the proximity between the elements.
+        If not provided, will be calculated using the "max" procedure, and
+        the same cutoff value for this call.
+
+    ### Returns:
+    (pd.DataFrame) -- A matrix with the probability that a location generates
+        comparative advantages in a economic activity.
+    """
+
+    opp = rcas.copy()
+
+    if cutoff == 0:
+        opp = 1
+    else:
+        opp[opp >= cutoff] = pd.NA
+        opp[opp < cutoff] = 1
+
+    wcp = relatedness(rcas, cutoff=cutoff, proximities=proximities)
+
+    wcp_opp = opp * wcp
+    wcp_mean = wcp_opp.mean(axis=1)
+    wcp_std = wcp_opp.std(axis=1)
+
+    return wcp.transform(lambda x: (x - wcp_mean) / wcp_std)
```

### Comparing `economic_complexity-0.2.2/economic_complexity/rca.py` & `economic_complexity-0.2.4/economic_complexity/rca.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/economic_complexity/subnational.py` & `economic_complexity-0.2.4/economic_complexity/subnational.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/LICENSE` & `economic_complexity-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/PACKAGE.md` & `economic_complexity-0.2.4/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.2.2/pyproject.toml` & `economic_complexity-0.2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "economic-complexity"
-version = "0.2.2"
+version = "0.2.4"
 description = "Functions to calculate Economic Complexity indicators."
 authors = [
   "Jelmy Hermosilla <jelmy@datawheel.us>",
   "Nicolas Netz <nicolas.netz@datawheel.us>",
   "Samuel Osorio <samuel@datawheel.us>",
   "Marcos Perez <marcos@datawheel.us>",
 ]
@@ -14,23 +14,23 @@
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/py-economic-complexity"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = {version = "^1.5.0", optional = true}
-polars = {version = ">=0.18.0", optional = true}
+polars = {version = "^0.20.0", optional = true}
 
 [tool.poetry.extras]
 pandas = ["pandas"]
 polars = ["polars"]
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.2"
 pandas = "^1.5.3"
 polars = ">=0.18.0"
 pytest = "^7.4.2"
-ruff = "^0.1.8"
+ruff = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `economic_complexity-0.2.2/PKG-INFO` & `economic_complexity-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: economic-complexity
-Version: 0.2.2
+Version: 0.2.4
 Summary: Functions to calculate Economic Complexity indicators.
 Home-page: https://github.com/Datawheel/py-economic-complexity
 License: MIT
 Author: Jelmy Hermosilla
 Author-email: jelmy@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pandas
 Provides-Extra: polars
 Requires-Dist: pandas (>=1.5.0,<2.0.0) ; extra == "pandas"
-Requires-Dist: polars (>=0.18.0) ; extra == "polars"
+Requires-Dist: polars (>=0.20.0,<0.21.0) ; extra == "polars"
 Project-URL: Repository, https://github.com/Datawheel/py-economic-complexity
 Description-Content-Type: text/markdown
 
 This package contains functions to calculate Economic Complexity indicators.  
 The functions handle the data through `pandas.DataFrame` objects.
 
 <p>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: economic-complexity Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: economic-complexity Version: 0.2.4 Summary:
 Functions to calculate Economic Complexity indicators. Home-page: https://
 github.com/Datawheel/py-economic-complexity License: MIT Author: Jelmy
 Hermosilla Author-email: jelmy@datawheel.us Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: pandas
 Provides-Extra: polars Requires-Dist: pandas (>=1.5.0,<2.0.0) ; extra ==
-"pandas" Requires-Dist: polars (>=0.18.0) ; extra == "polars" Project-URL:
-Repository, https://github.com/Datawheel/py-economic-complexity Description-
-Content-Type: text/markdown This package contains functions to calculate
-Economic Complexity indicators. The functions handle the data through
+"pandas" Requires-Dist: polars (>=0.20.0,<0.21.0) ; extra == "polars" Project-
+URL: Repository, https://github.com/Datawheel/py-economic-complexity
+Description-Content-Type: text/markdown This package contains functions to
+calculate Economic Complexity indicators. The functions handle the data through
 `pandas.DataFrame` objects.
 _[_h_t_t_p_s_:_/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_D_a_t_a_w_h_e_e_l_/_p_y_-_e_c_o_n_o_m_i_c_-_c_o_m_p_l_e_x_i_t_y_]
 _[_h_t_t_p_s_:_/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_D_a_t_a_w_h_e_e_l_/_p_y_-_e_c_o_n_o_m_i_c_-_c_o_m_p_l_e_x_i_t_y_]
 _[_h_t_t_p_s_:_/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_c_h_e_c_k_s_/_D_a_t_a_w_h_e_e_l_/_p_y_-_e_c_o_n_o_m_i_c_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:
 _/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_D_a_t_a_w_h_e_e_l_/_p_y_-_e_c_o_n_o_m_i_c_-_c_o_m_p_l_e_x_i_t_y_]
 ## Installation We recommend the use of `poetry`, to resolve the best version
 of the dependencies that works with your current project. ```bash $ poetry add
```

