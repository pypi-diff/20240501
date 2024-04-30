# Comparing `tmp/fire_opal-7.2.0.tar.gz` & `tmp/fire_opal-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-7.2.0.tar", max compression
+gzip compressed data, was "fire_opal-7.3.0.tar", max compression
```

## Comparing `fire_opal-7.2.0.tar` & `fire_opal-7.3.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0    36587 2024-04-18 23:43:46.772082 fire_opal-7.2.0/LICENSE
--rw-r--r--   0        0        0      532 2024-04-18 23:43:46.772082 fire_opal-7.2.0/README.md
--rw-r--r--   0        0        0     1335 2024-04-18 23:44:11.760151 fire_opal-7.2.0/fireopal/__init__.py
--rw-r--r--   0        0        0    11489 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/_event_tracker.py
--rw-r--r--   0        0        0     2129 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/_utils.py
--rw-r--r--   0        0        0      624 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/admin.py
--rw-r--r--   0        0        0     4718 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/config.py
--rw-r--r--   0        0        0     1198 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/constants.py
--rw-r--r--   0        0        0      909 2024-04-18 23:44:11.760151 fire_opal-7.2.0/fireopal/credentials/__init__.py
--rw-r--r--   0        0        0     3840 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/credentials/_credentials.py
--rw-r--r--   0        0        0      907 2024-04-18 23:44:11.756151 fire_opal-7.2.0/fireopal/functions/__init__.py
--rw-r--r--   0        0        0     6800 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/activity_monitor.py
--rw-r--r--   0        0        0     2686 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/authenticate.py
--rw-r--r--   0        0        0     1058 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/base.py
--rw-r--r--   0        0        0     7004 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/execute.py
--rw-r--r--   0        0        0     2252 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/get_result.py
--rw-r--r--   0        0        0     1106 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/read_data.py
--rw-r--r--   0        0        0     1163 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     3414 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1754 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2966 2024-04-18 23:44:11.752151 fire_opal-7.2.0/pyproject.toml
--rw-r--r--   0        0        0     2612 1970-01-01 00:00:00.000000 fire_opal-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-04-30 23:31:50.692692 fire_opal-7.3.0/LICENSE
+-rw-r--r--   0        0        0      532 2024-04-30 23:31:50.692692 fire_opal-7.3.0/README.md
+-rw-r--r--   0        0        0     1401 2024-04-30 23:32:15.192692 fire_opal-7.3.0/fireopal/__init__.py
+-rw-r--r--   0        0        0    11489 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/_event_tracker.py
+-rw-r--r--   0        0        0     2129 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/_utils.py
+-rw-r--r--   0        0        0      624 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/admin.py
+-rw-r--r--   0        0        0     4718 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/config.py
+-rw-r--r--   0        0        0     1198 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/constants.py
+-rw-r--r--   0        0        0      909 2024-04-30 23:32:15.188692 fire_opal-7.3.0/fireopal/credentials/__init__.py
+-rw-r--r--   0        0        0     3840 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/credentials/_credentials.py
+-rw-r--r--   0        0        0      975 2024-04-30 23:32:15.188692 fire_opal-7.3.0/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0     8414 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/_utils.py
+-rw-r--r--   0        0        0     6800 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/activity_monitor.py
+-rw-r--r--   0        0        0     2686 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/authenticate.py
+-rw-r--r--   0        0        0     1058 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/base.py
+-rw-r--r--   0        0        0     2897 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     2252 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/get_result.py
+-rw-r--r--   0        0        0     3021 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/iterate.py
+-rw-r--r--   0        0        0     1106 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1163 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     3414 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1412 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/stop_iterate.py
+-rw-r--r--   0        0        0     1754 2024-04-30 23:31:50.692692 fire_opal-7.3.0/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2966 2024-04-30 23:32:15.180692 fire_opal-7.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2612 1970-01-01 00:00:00.000000 fire_opal-7.3.0/PKG-INFO
```

### Comparing `fire_opal-7.2.0/LICENSE` & `fire_opal-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/README.md` & `fire_opal-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/__init__.py` & `fire_opal-7.3.0/fireopal/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,42 +7,46 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "7.2.0"
+__version__ = "7.3.0"
 
 from qctrlworkflowclient.utils import check_package_version as _check_package_version
 
 from . import credentials
 from ._utils import print_package_versions
 from .config import configure_organization
 from .constants import PACKAGE_INFO as _package_info
 from .functions import (
     activity_monitor,
     authenticate_qctrl_account,
     execute,
     get_action_metadata,
     get_result,
+    iterate,
     show_supported_devices,
     solve_qaoa,
+    stop_iterate,
     validate,
 )
 
 _check_package_version(_package_info)
 
 
 __all__ = [
     "activity_monitor",
     "authenticate_qctrl_account",
     "credentials",
     "configure_organization",
     "execute",
     "get_action_metadata",
     "get_result",
+    "iterate",
     "show_supported_devices",
     "solve_qaoa",
+    "stop_iterate",
     "validate",
     "print_package_versions",
 ]
```

### Comparing `fire_opal-7.2.0/fireopal/_event_tracker.py` & `fire_opal-7.3.0/fireopal/_event_tracker.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/_utils.py` & `fire_opal-7.3.0/fireopal/_utils.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/admin.py` & `fire_opal-7.3.0/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/config.py` & `fire_opal-7.3.0/fireopal/config.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/constants.py` & `fire_opal-7.3.0/fireopal/constants.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/credentials/__init__.py` & `fire_opal-7.3.0/fireopal/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/credentials/_credentials.py` & `fire_opal-7.3.0/fireopal/credentials/_credentials.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/__init__.py` & `fire_opal-7.3.0/fireopal/functions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,11 +14,13 @@
 from .activity_monitor import (
     activity_monitor,
     get_action_metadata,
 )
 from .authenticate import authenticate_qctrl_account
 from .execute import execute
 from .get_result import get_result
+from .iterate import iterate
 from .read_data import read_data
 from .show_supported_devices import show_supported_devices
 from .solve_qaoa import solve_qaoa
+from .stop_iterate import stop_iterate
 from .validate import validate
```

### Comparing `fire_opal-7.2.0/fireopal/functions/activity_monitor.py` & `fire_opal-7.3.0/fireopal/functions/activity_monitor.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/authenticate.py` & `fire_opal-7.3.0/fireopal/functions/authenticate.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/base.py` & `fire_opal-7.3.0/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/execute.py` & `fire_opal-7.3.0/fireopal/functions/_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,108 +10,54 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 from __future__ import annotations
 
 import logging
-from typing import Optional
+from typing import (
+    Any,
+    Optional,
+)
 
 from qctrlcommons.exceptions import QctrlArgumentsValueError
 
-from fireopal._utils import log_activity
-from fireopal.config import get_config
 from fireopal.credentials import Credentials
 
-from .base import fire_opal_workflow
 
-
-@fire_opal_workflow("compile_and_run_workflow")
-def execute(
-    circuits: str | list[str],
-    shot_count: int,
-    credentials: Credentials,
-    backend_name: str,
-) -> dict:
-    """
-    Execute a batch of `circuits` where `shot_count` measurements are taken per circuit.
-
-    Parameters
-    ----------
-    circuits : str or list[str]
-        Quantum circuit(s) in the form of a QASM strings. You may use Qiskit to
-        generate these strings.
-    shot_count : int
-        Number of bitstrings that are sampled from the final quantum state.
-    credentials : Credentials
-        The credentials for running circuits. See the `credentials` module for functions
-        to generate credentials for your desired provider.
-    backend_name : str
-        The backend device name that should be used to run circuits.
-
-    Returns
-    -------
-    dict
-        A dictionary containing probability mass functions and warnings.
-    """
-    log_activity(
-        function_called="execute",
-        circuits=circuits,
-        shot_count=shot_count,
-        backend_name=backend_name,
-    )
-
-    _check_execute_validity(
-        circuits=circuits,
-        shot_count=shot_count,
-        credentials=credentials,
-        backend_name=backend_name,
-    )
-    circuits = _handle_single_circuit(circuits)
-
-    settings = get_config()
-    credentials_with_org = credentials.copy()
-    credentials_with_org.update({"organization": settings.organization})
-    return {
-        "circuits": circuits,
-        "shot_count": shot_count,
-        "credentials": credentials_with_org,
-        "backend_name": backend_name,
-    }
-
-
-def _handle_single_circuit(strings: str | list[str]) -> list[str]:
+def handle_single_item(item: Any) -> list[Any]:
     """
-    Convert a single string to a list holding containing it, if applicable.
+    Convert a single item to a list holding containing it, if applicable.
 
     Parameters
     ----------
-    strings : str or list[str]
-        One or more strings.
+    item : Any
+        One or more items.
 
     Returns
     -------
-    list[str]
-        The input if originally provided as a list. Otherwise, the input string in
+    list[Any]
+        The input if originally provided as a list. Otherwise, the input in
         a list.
     """
-    if isinstance(strings, str):
-        return [strings]
-    return strings
+    if not isinstance(item, list):
+        return [item]
+    return item
 
 
-def _check_single_circuit_validity(
+def check_single_circuit_validity(
     circuit: str, circuit_index: Optional[int] = None
 ) -> None:
     """
     Validate that circuits are of type string as well as nonempty.
+
     Parameters
     ----------
     circuit : str
-        The input circuit
+        The input circuit.
     circuit_index : int, optional
         The index of the circuit if the input is a list. Defaults to None.
     """
 
     extras = {"circuit_index": circuit_index} if circuit_index is not None else None
     if not isinstance(circuit, str):
         logging.error(
@@ -127,35 +73,96 @@
         raise QctrlArgumentsValueError(
             "The circuit string provided must be non-empty.",
             arguments={"circuits": circuit},
             extras=extras,
         )
 
 
-def _check_execute_validity(
+def check_single_parameter_dict_validity(
+    parameters: dict[str, float], parameter_dict_index: Optional[int] = None
+) -> None:
+    """
+    Validate that the parameter dictionary and its entries have valid
+    types.
+
+    Parameters
+    ----------
+    parameters : dict[str, float]
+        The parameter dictionary.
+    parameter_dict_index : int, optional
+        The index of the parameter dictionary if the parameters input
+        is a list. Defaults to None.
+    """
+
+    extras = (
+        {"parameter_dict_index": parameter_dict_index}
+        if parameter_dict_index is not None
+        else None
+    )
+    if not isinstance(parameters, dict):
+        logging.error(
+            "QCTRL - Invalid type received for parameters input. "
+            "The parameters must consist of dictionaries."
+        )
+        raise QctrlArgumentsValueError(
+            "Invalid type received for parameters input. "
+            "The parameters must consist of dictionaries.",
+            arguments={"parameters": parameters},
+            extras=extras,
+        )
+    for key, value in parameters.items():
+        if not isinstance(key, str):
+            logging.error(
+                "QCTRL - Invalid type received for parameters' key. "
+                "The keys in parameters must be strings."
+            )
+            raise QctrlArgumentsValueError(
+                "Invalid type received for parameters' key. "
+                "The keys in parameters must be strings.",
+                arguments={"parameters": parameters},
+                extras=extras,
+            )
+        if not isinstance(value, float):
+            logging.error(
+                "QCTRL - Invalid type received for parameters' values. "
+                "The values in parameters must be floats."
+            )
+            raise QctrlArgumentsValueError(
+                "Invalid type received for parameters' values. "
+                "The values in parameters must be floats.",
+                arguments={"parameters": parameters},
+                extras=extras,
+            )
+
+
+def check_circuit_submission_validity(
     circuits: str | list[str],
     shot_count: int,
     credentials: Credentials,
     backend_name: str,
+    parameters: Optional[dict[str, float] | list[dict[str, float]]] = None,
 ) -> None:
     """
-    Check if the inputs are valid for execute function.
+    Check if the inputs are valid for submission of circuits to a hardware provider.
 
     Parameters
     ----------
     circuits : str or list[str]
-        Quantum circuit(s) in the form of a QASM strings. You may use Qiskit to
+        Quantum circuit(s) in the form of QASM strings. You may use Qiskit to
         generate these strings. This list or string must be non-empty.
     shot_count : int
         Number of bitstrings that are sampled from the final quantum state.
     credentials : Credentials
         The credentials for running circuits. See the `credentials` module for functions
         to generate credentials for your desired provider.
     backend_name : str
         The backend device name that should be used to run circuits.
+    parameters : dict[str, float] or list[dict[str, float]] or None, optional
+        The list of parameters for the circuit(s), if they're parametric.
+        Defaults to None.
     """
 
     if isinstance(circuits, list):
         if not all(isinstance(circuit, str) for circuit in circuits):
             logging.error(
                 "QCTRL - Invalid type received for circuits input. All circuits must be strings."
             )
@@ -166,17 +173,17 @@
         if len(circuits) == 0:
             logging.error("QCTRL - The list of circuits must be non-empty.")
             raise QctrlArgumentsValueError(
                 "The list of circuits must be non-empty.",
                 arguments={"circuits": circuits},
             )
         for index, circuit in enumerate(circuits):
-            _check_single_circuit_validity(circuit=circuit, circuit_index=index)
+            check_single_circuit_validity(circuit=circuit, circuit_index=index)
     else:
-        _check_single_circuit_validity(circuit=circuits)
+        check_single_circuit_validity(circuit=circuits)
     if not isinstance(shot_count, int):
         logging.error(
             "QCTRL - Invalid type received for shot_count input. The shot_count must be an integer."
         )
         raise QctrlArgumentsValueError(
             "Invalid type received for shot_count input. The shot_count must be an integer.",
             arguments={"shot_count": shot_count},
@@ -198,7 +205,26 @@
             "QCTRL - Invalid type received for backend_name input. "
             "The backend_name must be a string."
         )
         raise QctrlArgumentsValueError(
             "Invalid type received for backend_name input. The backend_name must be a string.",
             arguments={"backend_name": backend_name},
         )
+    if parameters is not None:
+        if not isinstance(parameters, (list, dict)):
+            logging.error(
+                "QCTRL - Invalid type received for parameters input. "
+                "The parameters must be a list or dict."
+            )
+            raise QctrlArgumentsValueError(
+                "Invalid type received for parameters input. "
+                "The parameters must be a list or dict.",
+                arguments={"parameters": parameters},
+            )
+
+        if isinstance(parameters, list):
+            for index, parameter_dict in enumerate(parameters):
+                check_single_parameter_dict_validity(
+                    parameters=parameter_dict, parameter_dict_index=index
+                )
+        else:
+            check_single_parameter_dict_validity(parameters=parameters)
```

### Comparing `fire_opal-7.2.0/fireopal/functions/get_result.py` & `fire_opal-7.3.0/fireopal/functions/get_result.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/read_data.py` & `fire_opal-7.3.0/fireopal/functions/read_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/show_supported_devices.py` & `fire_opal-7.3.0/fireopal/functions/show_supported_devices.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/solve_qaoa.py` & `fire_opal-7.3.0/fireopal/functions/solve_qaoa.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/fireopal/functions/validate.py` & `fire_opal-7.3.0/fireopal/functions/validate.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.2.0/pyproject.toml` & `fire_opal-7.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "7.2.0"
+version = "7.3.0"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com/fire-opal"
```

### Comparing `fire_opal-7.2.0/PKG-INFO` & `fire_opal-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 7.2.0
+Version: 7.3.0
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

