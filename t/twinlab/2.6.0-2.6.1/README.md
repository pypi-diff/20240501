# Comparing `tmp/twinlab-2.6.0.tar.gz` & `tmp/twinlab-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-2.6.0.tar", max compression
+gzip compressed data, was "twinlab-2.6.1.tar", max compression
```

## Comparing `twinlab-2.6.0.tar` & `twinlab-2.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1031 2023-09-19 13:29:40.794269 twinlab-2.6.0/LICENSE
--rw-r--r--   0        0        0     2657 2024-04-29 09:55:28.721775 twinlab-2.6.0/README.md
--rw-r--r--   0        0        0     1759 2024-04-29 09:55:28.722058 twinlab-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     1486 2024-04-25 10:08:03.722392 twinlab-2.6.0/twinlab/__init__.py
--rw-r--r--   0        0        0      171 2023-09-19 13:29:40.807103 twinlab-2.6.0/twinlab/_version.py
--rw-r--r--   0        0        0    14702 2024-04-29 09:55:28.777944 twinlab-2.6.0/twinlab/api.py
--rw-r--r--   0        0        0    40736 2024-04-29 09:55:28.778517 twinlab-2.6.0/twinlab/client.py
--rw-r--r--   0        0        0     9608 2024-04-29 09:55:28.778655 twinlab-2.6.0/twinlab/core.py
--rw-r--r--   0        0        0     9256 2024-04-29 09:55:28.778932 twinlab-2.6.0/twinlab/dataset.py
--rw-r--r--   0        0        0      843 2024-04-29 09:55:28.779188 twinlab-2.6.0/twinlab/distributions.py
--rw-r--r--   0        0        0    66335 2024-04-29 09:55:28.779451 twinlab-2.6.0/twinlab/emulator.py
--rw-r--r--   0        0        0     4876 2024-04-15 15:01:48.559474 twinlab-2.6.0/twinlab/helper.py
--rw-r--r--   0        0        0    29378 2024-04-29 09:55:28.779621 twinlab-2.6.0/twinlab/params.py
--rw-r--r--   0        0        0     1862 2024-03-13 15:41:11.184579 twinlab-2.6.0/twinlab/plotting.py
--rw-r--r--   0        0        0      659 2024-04-29 09:55:28.779734 twinlab-2.6.0/twinlab/prior.py
--rw-r--r--   0        0        0     1926 2024-04-15 15:01:48.560048 twinlab-2.6.0/twinlab/sampling.py
--rw-r--r--   0        0        0     1637 2024-01-11 11:15:46.668160 twinlab-2.6.0/twinlab/settings.py
--rw-r--r--   0        0        0     5669 2024-04-29 09:55:28.779852 twinlab-2.6.0/twinlab/utils.py
--rw-r--r--   0        0        0     4081 1970-01-01 00:00:00.000000 twinlab-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-09-19 13:29:40.794269 twinlab-2.6.1/LICENSE
+-rw-r--r--   0        0        0     2657 2024-04-29 12:58:08.159852 twinlab-2.6.1/README.md
+-rw-r--r--   0        0        0     1759 2024-05-01 08:08:37.375772 twinlab-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1486 2024-04-30 15:00:41.994100 twinlab-2.6.1/twinlab/__init__.py
+-rw-r--r--   0        0        0      171 2023-09-19 13:29:40.807103 twinlab-2.6.1/twinlab/_version.py
+-rw-r--r--   0        0        0    14702 2024-04-29 12:58:08.199408 twinlab-2.6.1/twinlab/api.py
+-rw-r--r--   0        0        0    40736 2024-04-29 12:58:08.199897 twinlab-2.6.1/twinlab/client.py
+-rw-r--r--   0        0        0     9549 2024-05-01 08:08:27.641140 twinlab-2.6.1/twinlab/core.py
+-rw-r--r--   0        0        0     9256 2024-04-29 12:58:08.200160 twinlab-2.6.1/twinlab/dataset.py
+-rw-r--r--   0        0        0      843 2024-04-29 12:58:08.200663 twinlab-2.6.1/twinlab/distributions.py
+-rw-r--r--   0        0        0    66186 2024-05-01 08:08:27.641673 twinlab-2.6.1/twinlab/emulator.py
+-rw-r--r--   0        0        0     4876 2024-04-15 15:01:48.559474 twinlab-2.6.1/twinlab/helper.py
+-rw-r--r--   0        0        0    29618 2024-05-01 08:08:27.642016 twinlab-2.6.1/twinlab/params.py
+-rw-r--r--   0        0        0     1862 2024-03-13 15:41:11.184579 twinlab-2.6.1/twinlab/plotting.py
+-rw-r--r--   0        0        0      659 2024-04-29 12:58:08.201372 twinlab-2.6.1/twinlab/prior.py
+-rw-r--r--   0        0        0     1926 2024-04-15 15:01:48.560048 twinlab-2.6.1/twinlab/sampling.py
+-rw-r--r--   0        0        0     1637 2024-01-11 11:15:46.668160 twinlab-2.6.1/twinlab/settings.py
+-rw-r--r--   0        0        0     5674 2024-05-01 08:08:27.642300 twinlab-2.6.1/twinlab/utils.py
+-rw-r--r--   0        0        0     4081 1970-01-01 00:00:00.000000 twinlab-2.6.1/PKG-INFO
```

### Comparing `twinlab-2.6.0/LICENSE` & `twinlab-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/README.md` & `twinlab-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/pyproject.toml` & `twinlab-2.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "2.6.0"
+version = "2.6.1"
 description = "twinLab - Probabilistic Machine Learning for Engineers"
 license = "MIT"
 homepage = "https://twinlab.ai"
 documentation = "https://twinlab.ai"
 authors = ["digiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
     "Alexander Mead <alexander@digilab.co.uk>",
```

### Comparing `twinlab-2.6.0/twinlab/__init__.py` & `twinlab-2.6.1/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/api.py` & `twinlab-2.6.1/twinlab/api.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/client.py` & `twinlab-2.6.1/twinlab/client.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/core.py` & `twinlab-2.6.1/twinlab/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         pprint(datasets, compact=True, sort_dicts=False)
     return datasets
 
 
 @typechecked
 def list_emulators(
     verbose: bool = False,
-) -> Optional[List[str]]:  # TODO: Is this really an Optional return type?
+) -> List[str]:
     """List trained emulators that exist in the user's twinLab cloud account.
 
     These trained emulators can be used for a variety of inference operations (see methods of the Emulator class).
     Setting ``verbose=True`` will also show the state of currently training emulators, as well as those that have failed to train.
     Information about start time and current/final run time will also be shown if ``verbose=True``.
 
     Args:
```

### Comparing `twinlab-2.6.0/twinlab/dataset.py` & `twinlab-2.6.1/twinlab/dataset.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/distributions.py` & `twinlab-2.6.1/twinlab/distributions.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/emulator.py` & `twinlab-2.6.1/twinlab/emulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Standard imports
 import io
 import json
 import sys
 import time
 import uuid
-
+import warnings
 from pprint import pprint
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 # Third-party imports
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -150,24 +150,26 @@
         )
         if verbose:
             message = _get_response_message(body)
             print(f"Job status for {PROCESS_MAP[method]}: {message}")
     return status, body
 
 
-# TODO: This is awful!
+# TODO: This function needs streamlining, what about dict.get(key, default)?
 # TODO: All responses should return a "message", then this would not be necessary
 @typechecked
 def _get_response_message(body: dict) -> str:
-    if "message" in body:  # TODO: Yuck!
+    if "message" in body:  # TODO: if/else structure needs to be streamlined
         message = body["message"]
     elif "process_status" in body:
-        message = body["process_status"]  # TODO: This is a foul hack
-    elif "process_status:" in body:
-        message = body["process_status:"]  # TODO: This is an even fouler hack
+        message = body["process_status"]
+    elif (
+        "process_status:" in body
+    ):  # TODO: Note the colon; this needs to be made more robust
+        message = body["process_status:"]
     else:
         message = "No response message in body"
     return message
 
 
 @typechecked
 def _process_csv(
@@ -351,27 +353,27 @@
         # Send training request
         _, response = api.train_request_model(
             self.id, params_str, processor=PROCESSOR, verbose=DEBUG
         )
         if verbose:
             message = utils.get_message(response)
             print(message)
-        # TODO: Should process_id be appended to the emulator object?
-        self.process_id = utils.get_value_from_body("process_id", response)
+
+        # Get the process ID from the response
+        process_id = utils.get_value_from_body("process_id", response)
         if verbose:
-            print(f"Emulator {self.id} with process ID {self.process_id} is training.")
+            print(f"Emulator {self.id} with process ID {process_id} is training.")
         if not wait:
-            return self.process_id
-        _wait_for_training_completion(self.id, self.process_id, verbose=verbose)
+            return process_id
+        _wait_for_training_completion(self.id, process_id, verbose=verbose)
         if verbose:
             print(
-                f"Training of emulator {self.id} with process ID {self.process_id} is complete!"
+                f"Training of emulator {self.id} with process ID {process_id} is complete!"
             )
 
-    # TODO: This seems to be completely broken!! There is no self.process_id!!
     @typechecked
     def status(self, process_id: str, verbose: bool = False) -> dict:
         """Check the status of a training process on the twinLab cloud.
 
         Args:
             process_id (str): The process ID of the training process to check the status of.
             verbose (bool, optional): Display information about the operation while running.
@@ -730,16 +732,15 @@
     ) -> Optional[Union[pd.DataFrame, float]]:
         """Score the performance of a trained emulator.
 
         Returns a score for a trained emulator that quantifies its performance on the test dataset.
         Note that a test dataset must have been defined in order for this to produce a result.
         This means that ``train_test_ratio`` in TrainParams must be less than ``1`` when training the emulator.
         If there is no test dataset then this will return ``None``.
-        The score can be calculated using two metrics: the mean-squared error (MSE) or mean-standarised log loss (MSLL).
-        See the ``ScoreParams`` class for a full list and description of available metrics.
+        The score can be calculated using different metrics, see the ``ScoreParams`` class for a full list and description of available metrics.
 
         Args:
             params (ScoreParams, optional): A parameters object that contains optional scoring parameters.
             verbose (bool, optional): Display detailed information about the operation while running.
 
         Returns:
             Either a ``pandas.DataFrame`` containing the emulator per output dimension (if ``combined_score = False``),
@@ -784,16 +785,15 @@
             if not params.combined_score:  # DataFrame
                 score = pd.read_csv(score, sep=",")
             if verbose:
                 print("Emulator Score:")
                 print(score)  # Could be pd.DataFrame or float
             return score
         else:
-            # TODO: Convert to warning!
-            print(
+            warnings.warn(
                 "No test data was available for this emulator, so it cannot be scored."
             )
 
     @typechecked
     def benchmark(
         self,
         params: BenchmarkParams = BenchmarkParams(),
@@ -849,17 +849,16 @@
         if csv is not None:
             df = pd.read_csv(csv, sep=",")
             if verbose:
                 print("Calibration curve:")
                 pprint(df)
             return df
         else:
-            # TODO: Convert to warning!
-            print(
-                "No test data was available for this emulator, so it cannot be benchmarked."
+            warnings.warn(
+                "No test data was available for this emulator, so it cannot be scored."
             )
 
     @typechecked
     def predict(
         self,
         df: pd.DataFrame,
         params: PredictParams = PredictParams(),
```

### Comparing `twinlab-2.6.0/twinlab/helper.py` & `twinlab-2.6.1/twinlab/helper.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/params.py` & `twinlab-2.6.1/twinlab/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,24 +91,24 @@
             - ``"RQF"``: Rational Quadratic Function.
 
             Kernels can also be composed by using combinations of the ``"+"`` (addative) and ``"*"`` (multiplicative) operators.
             For example, ``covar_module = "(M52*PER)+RQF"`` is valid.
         estimator_type (str, optional): Specifies the type of Gaussian process to use for the emulator.
             The default is ``"single_task_gp"``, but the value can be chosen from the following list:
 
-            • ``"single_task_gp"``: The standard Gaussian Process, which learns a mean, covariance, and noise level.
-            • ``"fixed_noise_gp"``: A Gaussian Process with fixed noise, which is specified by the user.
+            - ``"single_task_gp"``: The standard Gaussian Process, which learns a mean, covariance, and noise level.
+            - ``"fixed_noise_gp"``: A Gaussian Process with fixed noise, which is specified by the user.
               Particularly useful for modelling noise-free simulated data where the noise can be set to zero manually.
-            • ``"heteroskedastic_gp"``: A Gaussian Process with fixed noise that is allowed to vary with the input.
+            - ``"heteroskedastic_gp"``: A Gaussian Process with fixed noise that is allowed to vary with the input.
               The noise is specified by the user, and is also learned by the Process.
-            • ``"variational_gp"``: An approximate Gaussian Process that is more efficient to train with large datasets.
-            • ``"mixed_single_task_gp"``: A Gaussian Process that works with a mix of continuous and categorical or discrete input data.
-            • ``"multi_fidelity_gp"``:  A Gaussian Process that works with input data that has multiple levels of fidelity.
+            - ``"variational_gp"``: An approximate Gaussian Process that is more efficient to train with large datasets.
+            - ``"mixed_single_task_gp"``: A Gaussian Process that works with a mix of continuous and categorical or discrete input data.
+            - ``"multi_fidelity_gp"``:  A Gaussian Process that works with input data that has multiple levels of fidelity.
               For example, combined data from both a high- and low-resolution simulation.
-            • ``"fixed_noise_multi_fidelity_gp"``: A Gaussian Process that works with input data that has multiple levels of fidelity and fixed noise.
+            - ``"fixed_noise_multi_fidelity_gp"``: A Gaussian Process that works with input data that has multiple levels of fidelity and fixed noise.
     """
 
     def __init__(
         self,
         detrend: bool = False,
         covar_module: Optional[str] = None,
         estimator_type: str = "single_task_gp",
@@ -324,17 +324,21 @@
 
 @typechecked
 class ScoreParams(Params):
     """Parameter configuration for scoring a trained emulator.
 
     Attributes:
         metric (str, optional): Metric used for scoring the performance of an emulator.
-            Can be either:
-            • ``"MSE"``: Mean Squared Error, which only compared the mean emulator prediction to the test data.
-            • ``"MSLL"``: Mean Squared Log Loss, which compares the distribution of the emulator prediction to the test data.
+            Can be one of:
+
+            - ``"MSLL"``: Mean Squared Log Loss, which compares the distribution of the emulator prediction to that of the test data.
+              A score of zero is that of the most naive data-generating model, which predicts the mean and standard deviation of the training data.
+              Lower (more negative) scores are better, while positive scores indicate serious problems.
+            - ``"MSE"``: Mean Squared Error, which only compares the mean emulator prediction to the test data.
+
             The default is ``"MSLL"``.
         combined_score (bool, optional): Determining whether to combined (average) the emulator score across output dimensions.
             If ``False`` a dataframe of scores will be returned, with the score for each output dimension, even if there is only a single emulator output dimension.
             If ``True`` a single number will be returned, which is the average score across all output dimensions.
             The default is ``False``.
 
     """
@@ -358,16 +362,16 @@
 class BenchmarkParams(Params):
     """Parameter configuration for benchmarking a trained emulator.
 
     Attributes:
         type (str, optional): Specifies the type of emulator benchmark to be performed.
             Can be either:
 
-            • ``"quantile"``: The calibration curve is calculated over Gaussian quantiles.
-            • ``"interval"``: The calibration curve is calculated over Gaussian confidence intervals.
+            - ``"quantile"``: The calibration curve is calculated over Gaussian quantiles.
+            - ``"interval"``: The calibration curve is calculated over Gaussian confidence intervals.
 
             The default is ``"quantile"``.
 
     """
 
     # TODO: This docstring needs to be massively improved.
```

### Comparing `twinlab-2.6.0/twinlab/plotting.py` & `twinlab-2.6.1/twinlab/plotting.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/prior.py` & `twinlab-2.6.1/twinlab/prior.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/sampling.py` & `twinlab-2.6.1/twinlab/sampling.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/settings.py` & `twinlab-2.6.1/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.0/twinlab/utils.py` & `twinlab-2.6.1/twinlab/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 def check_dataset(string: str) -> None:
     """
 
     Check that a sensible dataframe can be created from a .csv file string.
 
     """
 
-    # check for duplicate columns # TODO this assumes label is row 0
+    # Check for duplicate columns
+    # TODO: This assumes label is row 0
     header = pd.read_csv(io.StringIO(string), header=None, nrows=1).iloc[0].to_list()
     if len(set(header)) != len(header):
         raise TypeError("Dataset must contain no duplicate column names.")
 
     string_io = io.StringIO(string)
     try:
         df = pd.read_csv(string_io)
```

### Comparing `twinlab-2.6.0/PKG-INFO` & `twinlab-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 2.6.0
+Version: 2.6.1
 Summary: twinLab - Probabilistic Machine Learning for Engineers
 Home-page: https://twinlab.ai
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: digiLab Solutions Ltd.
 Author-email: info@digilab.co.uk
 Maintainer: Alexander Mead
```

