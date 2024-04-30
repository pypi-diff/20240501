# Comparing `tmp/pipefunc-0.4.0.tar.gz` & `tmp/pipefunc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefunc-0.4.0.tar", last modified: Tue Mar 12 00:01:47 2024, max compression
+gzip compressed data, was "pipefunc-0.5.0.tar", last modified: Tue Apr 30 22:04:13 2024, max compression
```

## Comparing `pipefunc-0.4.0.tar` & `pipefunc-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:01:47.425711 pipefunc-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-12 00:01:40.000000 pipefunc-0.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-12 00:01:40.000000 pipefunc-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-12 00:01:40.000000 pipefunc-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10660 2024-03-12 00:01:47.425711 pipefunc-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-03-12 00:01:40.000000 pipefunc-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:01:47.425711 pipefunc-0.4.0/pipefunc/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pipefunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pipefunc/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pipefunc/_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    58438 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pipefunc/_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pipefunc/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    24591 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pipefunc/_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 00:01:47.425711 pipefunc-0.4.0/pipefunc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:01:47.421711 pipefunc-0.4.0/pipefunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10660 2024-03-12 00:01:47.000000 pipefunc-0.4.0/pipefunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-12 00:01:47.000000 pipefunc-0.4.0/pipefunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 00:01:47.000000 pipefunc-0.4.0/pipefunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-12 00:01:47.000000 pipefunc-0.4.0/pipefunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 00:01:47.000000 pipefunc-0.4.0/pipefunc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-12 00:01:40.000000 pipefunc-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-12 00:01:47.425711 pipefunc-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:01:47.421711 pipefunc-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-12 00:01:40.000000 pipefunc-0.4.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-12 00:01:40.000000 pipefunc-0.4.0/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-03-12 00:01:40.000000 pipefunc-0.4.0/tests/test_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-03-12 00:01:40.000000 pipefunc-0.4.0/tests/test_sweep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.094823 pipefunc-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 22:04:07.000000 pipefunc-0.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 22:04:07.000000 pipefunc-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 22:04:07.000000 pipefunc-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-30 22:04:13.094823 pipefunc-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-30 22:04:07.000000 pipefunc-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.098823 pipefunc-0.5.0/pipefunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45131 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24844 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 22:04:13.098823 pipefunc-0.5.0/pipefunc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.094823 pipefunc-0.5.0/pipefunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 22:04:13.098823 pipefunc-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.094823 pipefunc-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_sweep.py
```

### Comparing `pipefunc-0.4.0/LICENSE` & `pipefunc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipefunc-0.4.0/PKG-INFO` & `pipefunc-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
@@ -86,38 +86,31 @@
 - [:hammer_and_wrench: Development](#hammer_and_wrench-development)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 <!-- toc-end -->
 
 ## :thinking: What is this?
 
-`pipefunc` is a Python library designed to create and manage complex networks of interdependent functions, often known as function pipelines.
+`pipefunc` is a Python library that simplifies the creation and management of complex function pipelines. It allows you to declare the dependencies between functions and automatically organizes the execution order to satisfy these dependencies.
 
-In a function pipeline, each function can have dependencies on the results of other functions. Managing these dependencies, ensuring each function has the inputs it needs, and determining the order of execution can become an annoying bookkeeping task in complex cases.
+`pipefunc` provides a range of features to streamline your workflow, including pipeline visualization, flexible function arguments, support for multiple outputs, pipeline simplification, resource usage profiling, parallel execution, caching, and parameter sweep utilities.
 
-`pipefunc` simplifies this process by allowing you to declare the dependencies of each function and automatically organizing the execution order to satisfy these dependencies. Additionally, the library provides features for visualizing the function pipeline, simplifying the pipeline graph, caching function results for efficiency, and profiling resource usage for optimization.
-
-For example, imagine you have a set of functions where `function B` needs the output from `function A`, and `function C` needs the outputs from both `function A` and `function B`. `pipefunc` allows you to specify these dependencies when you create the functions and then automatically manages their execution. It also provides tools for visualizing this function network, simplifying it if possible, and understanding the resource usage of each function.
-
-The library is designed to be an efficient and flexible tool for managing complex function dependencies in an intuitive and clear way. Whether you're dealing with data processing tasks, scientific computations, machine learning (AI) workflows, or other scenarios where functions depend on one another, `pipefunc` can help streamline your code and improve your productivity.
+Whether you're working with data processing, scientific computations, machine learning (AI) workflows, or any other scenario involving interdependent functions, `pipefunc` helps you focus on the logic of your code while it handles the intricacies of function dependencies and execution order.
 
 ## :rocket: Key Features
 
-Some of the key features of `pipefunc` include:
-
-1. 🚀 **Function Composition and Pipelining:** The core functionality of `pipefunc` is to create a pipeline of functions, allowing you to feed the output of one function into another, and execute them in the right order.
-1. 📊 **Visualizing Pipelines:** `pipefunc` can generate a visual graph of the function pipeline, making it easier to understand the flow of data.
-1. 💡 **Flexible Function Arguments:** `pipefunc` lets you call a function with different combinations of arguments, automatically determining which other functions to call based on the arguments you provide.
-1. 👥 **Multiple Outputs:** `pipefunc` supports functions that return multiple results, allowing each result to be used as input to other functions.
-1. ➡️ **Reducing Pipelines:** `pipefunc` can simplify a complex pipeline by merging nodes, improving computational efficiency at the cost of losing visibility into some intermediate steps.
-1. 🎛️ **Resources Report:** `pipefunc` provides a report on the performance of your pipeline, including CPU usage, memory usage, and execution time, helping you identify bottlenecks and optimize your code.
-1. 🔄 **Parallel Execution and Caching:** `pipefunc` supports parallel execution of functions, and caching of results to avoid redundant computation.
-1. 🔍 **Parameter Sweeps:** `pipefunc` provides a utility for generating combinations of parameters to use in a parameter sweep, along with the ability to cache results to optimize the sweep.
-1. 🛠️ **Flexibility and Ease of Use:** `pipefunc` is a lightweight, flexible, and powerful tool for managing complex function dependencies in a clear and intuitive way, designed to improve your productivity in any scenario where functions depend on one another.
-
+1. 🚀 **Function Composition and Pipelining**: Create pipelines where the output of one function feeds into another, with `pipefunc` handling the execution order.
+2. 📊 **Pipeline Visualization**: Generate visual graphs of your pipelines to better understand the flow of data.
+3. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
+4. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
+5. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
+6. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
+7. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
+8. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
+9. 🛠️ **Flexibility and Ease of Use**: Manage complex function dependencies in a clear, intuitive way with this lightweight yet powerful tool.
 
 ## :test_tube: How does it work?
 
 pipefunc provides a Pipeline class that you use to define your function pipeline.
 You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify a function's output name and dependencies.
 Once your pipeline is defined, you can execute it for specific output values, simplify it by combining functions with the same root arguments, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
 For more detailed usage instructions and examples, please check the usage example provided in the package.
```

### Comparing `pipefunc-0.4.0/README.md` & `pipefunc-0.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -28,38 +28,31 @@
 - [:hammer_and_wrench: Development](#hammer_and_wrench-development)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 <!-- toc-end -->
 
 ## :thinking: What is this?
 
-`pipefunc` is a Python library designed to create and manage complex networks of interdependent functions, often known as function pipelines.
+`pipefunc` is a Python library that simplifies the creation and management of complex function pipelines. It allows you to declare the dependencies between functions and automatically organizes the execution order to satisfy these dependencies.
 
-In a function pipeline, each function can have dependencies on the results of other functions. Managing these dependencies, ensuring each function has the inputs it needs, and determining the order of execution can become an annoying bookkeeping task in complex cases.
+`pipefunc` provides a range of features to streamline your workflow, including pipeline visualization, flexible function arguments, support for multiple outputs, pipeline simplification, resource usage profiling, parallel execution, caching, and parameter sweep utilities.
 
-`pipefunc` simplifies this process by allowing you to declare the dependencies of each function and automatically organizing the execution order to satisfy these dependencies. Additionally, the library provides features for visualizing the function pipeline, simplifying the pipeline graph, caching function results for efficiency, and profiling resource usage for optimization.
-
-For example, imagine you have a set of functions where `function B` needs the output from `function A`, and `function C` needs the outputs from both `function A` and `function B`. `pipefunc` allows you to specify these dependencies when you create the functions and then automatically manages their execution. It also provides tools for visualizing this function network, simplifying it if possible, and understanding the resource usage of each function.
-
-The library is designed to be an efficient and flexible tool for managing complex function dependencies in an intuitive and clear way. Whether you're dealing with data processing tasks, scientific computations, machine learning (AI) workflows, or other scenarios where functions depend on one another, `pipefunc` can help streamline your code and improve your productivity.
+Whether you're working with data processing, scientific computations, machine learning (AI) workflows, or any other scenario involving interdependent functions, `pipefunc` helps you focus on the logic of your code while it handles the intricacies of function dependencies and execution order.
 
 ## :rocket: Key Features
 
-Some of the key features of `pipefunc` include:
-
-1. 🚀 **Function Composition and Pipelining:** The core functionality of `pipefunc` is to create a pipeline of functions, allowing you to feed the output of one function into another, and execute them in the right order.
-1. 📊 **Visualizing Pipelines:** `pipefunc` can generate a visual graph of the function pipeline, making it easier to understand the flow of data.
-1. 💡 **Flexible Function Arguments:** `pipefunc` lets you call a function with different combinations of arguments, automatically determining which other functions to call based on the arguments you provide.
-1. 👥 **Multiple Outputs:** `pipefunc` supports functions that return multiple results, allowing each result to be used as input to other functions.
-1. ➡️ **Reducing Pipelines:** `pipefunc` can simplify a complex pipeline by merging nodes, improving computational efficiency at the cost of losing visibility into some intermediate steps.
-1. 🎛️ **Resources Report:** `pipefunc` provides a report on the performance of your pipeline, including CPU usage, memory usage, and execution time, helping you identify bottlenecks and optimize your code.
-1. 🔄 **Parallel Execution and Caching:** `pipefunc` supports parallel execution of functions, and caching of results to avoid redundant computation.
-1. 🔍 **Parameter Sweeps:** `pipefunc` provides a utility for generating combinations of parameters to use in a parameter sweep, along with the ability to cache results to optimize the sweep.
-1. 🛠️ **Flexibility and Ease of Use:** `pipefunc` is a lightweight, flexible, and powerful tool for managing complex function dependencies in a clear and intuitive way, designed to improve your productivity in any scenario where functions depend on one another.
-
+1. 🚀 **Function Composition and Pipelining**: Create pipelines where the output of one function feeds into another, with `pipefunc` handling the execution order.
+2. 📊 **Pipeline Visualization**: Generate visual graphs of your pipelines to better understand the flow of data.
+3. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
+4. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
+5. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
+6. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
+7. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
+8. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
+9. 🛠️ **Flexibility and Ease of Use**: Manage complex function dependencies in a clear, intuitive way with this lightweight yet powerful tool.
 
 ## :test_tube: How does it work?
 
 pipefunc provides a Pipeline class that you use to define your function pipeline.
 You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify a function's output name and dependencies.
 Once your pipeline is defined, you can execute it for specific output values, simplify it by combining functions with the same root arguments, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
 For more detailed usage instructions and examples, please check the usage example provided in the package.
```

### Comparing `pipefunc-0.4.0/pipefunc/__init__.py` & `pipefunc-0.5.0/pipefunc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """PipeFunc: A Python library for defining, managing, and executing function pipelines."""
 
-from pipefunc._pipefunc import Pipeline, PipelineFunction, pipefunc
+from pipefunc._lazy import construct_dag, evaluate_lazy
+from pipefunc._pipefunc import (
+    PipelineFunction,
+    pipefunc,
+)
+from pipefunc._pipeline import Pipeline
 from pipefunc._sweep import (
     MultiSweep,
     Sweep,
     count_sweep,
     generate_sweep,
     get_precalculation_order,
     set_cache_for_sweep,
 )
 from pipefunc._version import __version__
 
 __all__ = [
+    "construct_dag",
     "__version__",
     "count_sweep",
+    "evaluate_lazy",
     "generate_sweep",
     "get_precalculation_order",
+    "MultiSweep",
     "pipefunc",
     "Pipeline",
     "PipelineFunction",
     "set_cache_for_sweep",
     "Sweep",
-    "MultiSweep",
 ]
```

### Comparing `pipefunc-0.4.0/pipefunc/_perf.py` & `pipefunc-0.5.0/pipefunc/_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.4.0/pipefunc/_pipefunc.py` & `pipefunc-0.5.0/pipefunc/_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,367 +10,59 @@
 the resource usage of the pipeline functions.
 """
 
 from __future__ import annotations
 
 import contextlib
 import functools
-import hashlib
 import inspect
-import json
-import os
 import sys
 import time
 import warnings
-from collections import OrderedDict, defaultdict
-from pathlib import Path
+from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     Any,
     Generator,
-    Generic,
     Iterable,
     Literal,
     Tuple,
-    TypeVar,
     Union,
+    cast,
 )
 
-import cloudpickle
 import networkx as nx
 
-from pipefunc._cache import HybridCache, LRUCache
-from pipefunc._perf import ProfilingStats, ResourceProfiler
+from pipefunc._cache import DiskCache, HybridCache, LRUCache
+from pipefunc._lazy import _LazyFunction
+from pipefunc._pipefunc import PipelineFunction
 from pipefunc._plotting import visualize, visualize_holoviews
-
-if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Callable
-else:
-    from collections.abc import Callable
+from pipefunc._simplify import _combine_nodes, _get_signature, _wrap_dict_to_tuple
+from pipefunc._utils import at_least_tuple, generate_filename_from_dict
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 
 if TYPE_CHECKING:
-    import holoviews as hv
-
-T = TypeVar("T", bound=Callable[..., Any])
-_OUTPUT_TYPE = Union[str, Tuple[str, ...]]
-_CACHE_KEY_TYPE: TypeAlias = Tuple[
-    _OUTPUT_TYPE,
-    Tuple[Tuple[str, Any], ...],
-]
-
-
-def _at_least_tuple(x: Any) -> tuple[Any, ...]:
-    """Convert x to a tuple if it is not already a tuple."""
-    return x if isinstance(x, tuple) else (x,)
-
-
-def _default_output_picker(
-    output: Any,
-    name: str,
-    output_name: _OUTPUT_TYPE,
-) -> Any:
-    """Default output picker function for tuples."""
-    return output[output_name.index(name)]
-
-
-def _update_wrapper(wrapper, wrapped) -> None:  # noqa: ANN001
-    functools.update_wrapper(wrapper, wrapped)
-    # Need to manually update __wrapped__ to keep functions picklable
-    del wrapper.__dict__["__wrapped__"]
-
-
-class PipelineFunction(Generic[T]):
-    """Function wrapper class for pipeline functions with additional attributes.
-
-    Parameters
-    ----------
-    func
-        The original function to be wrapped.
-    output_name
-        The identifier for the output of the wrapped function.
-    output_picker
-        A function that takes the output of the wrapped function as first argument
-        and the output_name (str) as second argument, and returns the desired output.
-        If None, the output of the wrapped function is returned as is.
-    renames
-        A dictionary mapping from original argument names to new argument names.
-    profile
-        Flag indicating whether the wrapped function should be profiled.
-    debug
-        Flag indicating whether debug information should be printed.
-    cache
-        Flag indicating whether the wrapped function should be cached.
-    save
-        Flag indicating whether the output of the wrapped function should be saved.
-    save_function
-        A function that takes the filename and a dict containing the inputs and output.
-
-    Returns
-    -------
-        The identifier for the output of the wrapped function.
-
-    Examples
-    --------
-    >>> def add_one(a, b):
-    ...     return a + 1, b + 1
-    >>> add_one_func = PipelineFunction(
-    ...     add_one,
-    ...     output_name="a_plus_one",
-    ...     renames={"a": "x", "b": "y"},
-    ... )
-    >>> add_one_func(x=1, y=2)
-    (2, 3)
-
-    """
-
-    def __init__(
-        self,
-        func: T,
-        output_name: _OUTPUT_TYPE,
-        *,
-        output_picker: Callable[[str, Any], Any] | None = None,
-        renames: dict[str, str] | None = None,
-        profile: bool = False,
-        debug: bool = False,
-        cache: bool = False,
-        save: bool | None = None,
-        save_function: Callable[[str | Path, dict[str, Any]], None] | None = None,
-    ) -> None:
-        """Function wrapper class for pipeline functions with additional attributes."""
-        _update_wrapper(self, func)
-        self.func: Callable[..., Any] = func
-        self.output_name: _OUTPUT_TYPE = output_name
-        self.debug = debug
-        self.cache = cache
-        self.save_function = save_function
-        self.save = save if save is not None else save_function is not None
-        self.output_picker: Callable[[Any, str], Any] | None = output_picker
-        if output_picker is None and isinstance(output_name, tuple):
-            self.output_picker = functools.partial(
-                _default_output_picker,
-                output_name=self.output_name,
-            )
-
-        self._profile = profile
-        self.renames: dict[str, str] = renames or {}
-        self._inverse_renames: dict[str, str] = {v: k for k, v in self.renames.items()}
-        parameters = inspect.signature(func).parameters
-        self.parameters: list[str] = [self.renames.get(k, k) for k in parameters]
-        self.defaults: dict[str, Any] = {
-            self.renames.get(k, k): v.default
-            for k, v in parameters.items()
-            if v.default is not inspect.Parameter.empty
-        }
-        self.profiling_stats: ProfilingStats | None
-        self.set_profiling(enable=profile)
-
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        """Call the wrapped function with the given arguments.
-
-        Returns
-        -------
-        Any
-            The return value of the wrapped function.
-
-        """
-        kwargs = {self._inverse_renames.get(k, k): v for k, v in kwargs.items()}
-        with self._maybe_profiler():
-            result = self.func(*args, **kwargs)
-
-        if self.debug and self.profiling_stats is not None:
-            dt = self.profiling_stats.time.average
-            print(
-                f"Function {self.func.__name__} called with args={args},"
-                f" kwargs={kwargs}, took {dt:.2e} seconds to execute.",
-            )
-        return result
-
-    @property
-    def profile(self) -> bool:
-        """Return whether profiling is enabled for the wrapped function."""
-        return self._profile
-
-    @profile.setter
-    def profile(self, enable: bool) -> None:
-        """Enable or disable profiling for the wrapped function."""
-        self.set_profiling(enable=enable)
-
-    def set_profiling(self, *, enable: bool = True) -> None:
-        """Enable or disable profiling for the wrapped function."""
-        self._profile = enable
-        if enable:
-            self.profiling_stats = ProfilingStats()
-        else:
-            self.profiling_stats = None
+    if sys.version_info < (3, 9):  # pragma: no cover
+        from typing import Callable
+    else:
+        from collections.abc import Callable
 
-    def _maybe_profiler(self) -> contextlib.AbstractContextManager:
-        """Maybe get profiler.
-
-        Get a profiler instance if profiling is enabled, otherwise
-        return a dummy context manager.
-
-        Returns
-        -------
-        AbstractContextManager
-            A ResourceProfiler instance if profiling is enabled, or a
-            nullcontext if disabled.
-
-        """
-        if self.profiling_stats is not None:
-            return ResourceProfiler(os.getpid(), self.profiling_stats)
-        return contextlib.nullcontext()
-
-    def __getattr__(self, name: str) -> Any:
-        """Get attributes of the wrapped function.
-
-        Parameters
-        ----------
-        name
-            The name of the attribute to get.
-
-        Returns
-        -------
-        Any
-            The value of the attribute.
-
-        """
-        return getattr(self.func, name)
-
-    def __str__(self) -> str:
-        """Return a string representation of the PipelineFunction instance.
-
-        Returns
-        -------
-        str
-            A string representation of the PipelineFunction instance.
-
-        """
-        params = ", ".join(self.parameters)
-        outputs = ", ".join(_at_least_tuple(self.output_name))
-        return f"{self.func.__name__}({params}) → {outputs}"
-
-    def __repr__(self) -> str:
-        """Return a string representation of the PipelineFunction instance.
-
-        Returns
-        -------
-        str
-            A string representation of the PipelineFunction instance.
-
-        """
-        return f"PipelineFunction({self.func.__name__})"
-
-    def __getstate__(self) -> dict:
-        """Prepare the state of the current object for pickling.
-
-        The state includes all picklable instance variables.
-        For non-picklable instance variable,  they are transformed
-        into a picklable form or ignored.
-
-        Returns
-        -------
-        state : dict
-            A dictionary containing the picklable state of the object.
-
-        """
-        state = self.__dict__.copy()
-        state["func"] = cloudpickle.dumps(state.pop("func"))
-        return state
-
-    def __setstate__(self, state: dict) -> None:
-        """Restore the state of the current object from the provided state.
-
-        It also handles restoring non-picklable instance variable
-        into their original form.
-
-        Parameters
-        ----------
-        state : dict
-            A dictionary containing the picklable state of the object.
-
-        """
-        self.__dict__.update(state)
-        self.func = cloudpickle.loads(self.func)
-
-
-def pipefunc(
-    output_name: _OUTPUT_TYPE,
-    *,
-    output_picker: Callable[[Any, str], Any] | None = None,
-    renames: dict[str, str] | None = None,
-    profile: bool = False,
-    debug: bool = False,
-    cache: bool = False,
-    save: bool | None = None,
-    save_function: Callable[[str | Path, dict[str, Any]], None] | None = None,
-) -> Callable[[Callable[..., Any]], PipelineFunction]:
-    """A decorator for tagging pipeline functions with a return identifier.
+    from pathlib import Path
 
-    Parameters
-    ----------
-    output_name
-        The identifier for the output of the decorated function.
-    output_picker
-        A function that takes the output of the wrapped function as first argument
-        and the output_name (str) as second argument, and returns the desired output.
-        If None, the output of the wrapped function is returned as is.
-    renames
-        A dictionary mapping from original argument names to new argument names.
-    profile
-        Flag indicating whether the decorated function should be profiled.
-    debug
-        Flag indicating whether debug information should be printed.
-    cache
-        Flag indicating whether the decorated function should be cached.
-    save
-        Flag indicating whether the output of the wrapped function should be saved.
-    save_function
-        A function that takes the filename and a dict containing the inputs and output.
-
-    Returns
-    -------
-    Callable[[Callable[..., Any]], PipelineFunction]
-        A decorator function that takes the original function and output_name a
-        PipelineFunction instance with the specified return identifier.
-
-    """
-
-    def decorator(f: Callable[..., Any]) -> PipelineFunction:
-        """Wraps the original function in a PipelineFunction instance.
-
-        Parameters
-        ----------
-        f
-            The original function to be wrapped.
-
-        Returns
-        -------
-        PipelineFunction
-            The wrapped function with the specified return identifier.
+    import holoviews as hv
 
-        """
-        return PipelineFunction(
-            f,
-            output_name,
-            output_picker=output_picker,
-            renames=renames,
-            profile=profile,
-            debug=debug,
-            cache=cache,
-            save=save,
-            save_function=save_function,
-        )
+    from pipefunc._perf import ProfilingStats
 
-    return decorator
+_OUTPUT_TYPE = Union[str, Tuple[str, ...]]
+_CACHE_KEY_TYPE: TypeAlias = Tuple[_OUTPUT_TYPE, Tuple[Tuple[str, Any], ...]]
 
 
 class _Function:
     """Wrapper class for a pipeline function.
 
     Parameters
     ----------
@@ -379,25 +71,33 @@
     output_name
         The identifier for the return value of the pipeline function.
     root_args
         The names of the pipeline function's root inputs.
 
     """
 
+    __slots__ = ["pipeline", "output_name", "root_args", "_call_with_root_args"]
+
     def __init__(
         self,
         pipeline: Pipeline,
         output_name: _OUTPUT_TYPE,
         root_args: tuple[str, ...],
     ) -> None:
         """Initialize the function wrapper."""
         self.pipeline = pipeline
         self.output_name = output_name
         self.root_args = root_args
-        self.call_with_root_args = self._create_call_with_root_args_method()
+        self._call_with_root_args: Callable[..., Any] | None = None
+
+    @property
+    def call_with_root_args(self) -> Callable[..., Any]:
+        if self._call_with_root_args is None:
+            self._call_with_root_args = self._create_call_with_root_args_method()
+        return self._call_with_root_args
 
     def __call__(self, **kwargs: Any) -> Any:
         """Call the pipeline function with the given arguments.
 
         Parameters
         ----------
         kwargs
@@ -445,22 +145,24 @@
             The return value of the pipeline function.
 
         """
         return self(**kwargs)
 
     def __getstate__(self) -> dict:
         """Prepare the state of the current object for pickling."""
-        state = self.__dict__.copy()
-        state.pop("call_with_root_args", None)  # don't pickle the execute method
+        state = {slot: getattr(self, slot) for slot in self.__slots__}
+        state["_call_with_root_args"] = None  # don't pickle the execute method
         return state
 
     def __setstate__(self, state: dict) -> None:
         """Restore the state of the current object from the provided state."""
-        self.__dict__.update(state)
-        self.call_with_root_args = self._create_call_with_root_args_method()
+        for slot in self.__slots__:
+            setattr(self, slot, state[slot])
+        # Initialize _call_with_root_args if necessary
+        self._call_with_root_args = None
 
     def _create_call_with_parameters_method(
         self,
         parameters: tuple[str, ...],
         output_name: _OUTPUT_TYPE | None = None,
     ) -> Callable[..., Any]:
         sig = inspect.signature(self.__call__)
@@ -488,77 +190,99 @@
         call.__signature__ = new_sig  # type: ignore[attr-defined]
         return call
 
     def _create_call_with_root_args_method(self) -> Callable[..., Any]:
         return self._create_call_with_parameters_method(self.root_args)
 
 
-def _next_root_args(
-    pipeline: Pipeline,
-    arg_set: set[tuple[str, ...]],
-) -> tuple[str, ...]:
-    """Find the tuple of root arguments."""
-    return next(
-        args
-        for args in arg_set
-        if all(isinstance(pipeline.node_mapping[n], str) for n in args)
-    )
-
-
 class Pipeline:
     """Pipeline class for managing and executing a sequence of functions.
 
     Parameters
     ----------
     functions
         A list of functions that form the pipeline.
+    lazy
+        Flag indicating whether the pipeline should be lazy.
     debug
         Flag indicating whether debug information should be printed.
         If None, the value of each PipelineFunction's debug attribute is used.
     profile
         Flag indicating whether profiling information should be collected.
         If None, the value of each PipelineFunction's profile attribute is used.
-    cache
+    cache_type
         The type of cache to use.
+    cache_kwargs
+        Keyword arguments passed to
 
     """
 
     def __init__(
         self,
         functions: list[PipelineFunction],
         *,
+        lazy: bool = False,
         debug: bool | None = None,
         profile: bool | None = None,
-        cache: Literal["shared", "hybrid", "disk"] | None = "hybrid",
+        cache_type: Literal["lru", "hybrid", "disk"] | None = "lru",
+        cache_kwargs: dict[str, Any] | None = None,
     ) -> None:
         """Pipeline class for managing and executing a sequence of functions."""
-        # TODO: add support for disk cache
-        # TODO: check https://joblib.readthedocs.io/en/latest/memory.html
-        # TODO: add caching kwargs
-
         self.functions: list[PipelineFunction] = []
+        self.lazy = lazy
         self._debug = debug
         self._profile = profile
         self.output_to_func: dict[_OUTPUT_TYPE, PipelineFunction] = {}
         for f in functions:
             self.add(f)
-        self._graph = None
+        self._init_internal_cache()
+        self._set_cache(cache_type, lazy, cache_kwargs)
+
+    def _init_internal_cache(self) -> None:
+        # Internal Pipeline cache
         self._arg_combinations: dict[_OUTPUT_TYPE, set[tuple[str, ...]]] = {}
-        self.cache: LRUCache | HybridCache
+        self._root_args: dict[_OUTPUT_TYPE, tuple[str, ...]] = {}
+        self._func: dict[_OUTPUT_TYPE, _Function] = {}
+        with contextlib.suppress(AttributeError):
+            del self.graph
+        with contextlib.suppress(AttributeError):
+            del self.root_nodes
+        with contextlib.suppress(AttributeError):
+            del self.leaf_nodes
+        with contextlib.suppress(AttributeError):
+            del self.unique_leaf_node
 
-        if cache == "shared":
-            self.cache = LRUCache()
-        elif cache == "hybrid":
-            self.cache = HybridCache()
-        elif cache == "disk":
-            msg = "Disk cache not yet implemented"
-            raise NotImplementedError(msg)
-        else:
-            msg = f"Unknown cache type {cache}"
-            raise ValueError(msg)
+    def _set_cache(
+        self,
+        cache_type: Literal["lru", "hybrid", "disk"] | None,
+        lazy: bool,  # noqa: FBT001
+        cache_kwargs: dict[str, Any] | None,
+    ) -> None:
+        # Function result cache
+        self.cache: LRUCache | HybridCache | DiskCache | None = None
+        if cache_type is None:
+            return
+        if cache_kwargs is None:
+            cache_kwargs = {}
+        if cache_type == "lru":
+            cache_kwargs.setdefault("shared", not lazy)
+            self.cache = LRUCache(**cache_kwargs)
+        elif cache_type == "hybrid":
+            if lazy:
+                warnings.warn(
+                    "Hybrid cache uses function evaluation duration which"
+                    " is not measured correctly when using `lazy=True`.",
+                    UserWarning,
+                    stacklevel=2,
+                )
+            cache_kwargs.setdefault("shared", not lazy)
+            self.cache = HybridCache(**cache_kwargs)
+        elif cache_type == "disk":
+            cache_kwargs.setdefault("lru_shared", not lazy)
+            self.cache = DiskCache(**cache_kwargs)
 
     @property
     def profile(self) -> bool | None:
         """Flag indicating whether profiling information should be collected."""
         return self._profile
 
     @profile.setter
@@ -585,16 +309,14 @@
     def add(self, f: PipelineFunction) -> None:
         """Add a function to the pipeline.
 
         Parameters
         ----------
         f
             The function to add to the pipeline.
-        profile
-            Flag indicating whether profiling information should be collected.
 
         """
         if not isinstance(f, PipelineFunction):
             f = PipelineFunction(f, output_name=f.__name__)
         self.functions.append(f)
 
         self.output_to_func[f.output_name] = f
@@ -602,16 +324,16 @@
             for name in f.output_name:
                 self.output_to_func[name] = f
 
         if self.profile is not None:
             f.set_profiling(enable=self.profile)
         if self.debug is not None:
             f.debug = self.debug
-        self._graph = None
-        self._arg_combinations = {}
+
+        self._init_internal_cache()  # reset cache
 
     def _check_consistent_defaults(self) -> None:
         """Check that the default values for shared arguments are consistent."""
         arg_defaults = defaultdict(set)
         for f in self.functions:
             for arg, default_value in f.defaults.items():
                 arg_defaults[arg].add(default_value)
@@ -619,22 +341,16 @@
                     msg = (
                         f"Inconsistent default values for argument '{arg}' in"
                         " functions. Please make sure the shared input arguments have"
                         " the same default value or are set only for one function.",
                     )
                     raise ValueError(msg)
 
-    @property
+    @functools.cached_property
     def graph(self) -> nx.DiGraph:
-        """The directed graph representing the pipeline."""
-        if self._graph is None:
-            self._graph = self._make_graph()
-        return self._graph
-
-    def _make_graph(self) -> nx.DiGraph:
         """Create a directed graph representing the pipeline.
 
         Returns
         -------
         nx.DiGraph
             A directed graph with nodes representing functions and edges
             representing dependencies between functions.
@@ -650,15 +366,15 @@
                     edge = (self.output_to_func[arg], f)
                     if edge not in g.edges:
                         g.add_edge(*edge, arg=arg)
                     else:
                         # tuple output of function, and the edge already exists
                         assert isinstance(edge[0].output_name, tuple)
                         current = g.edges[edge]["arg"]
-                        g.edges[edge]["arg"] = (*_at_least_tuple(current), arg)
+                        g.edges[edge]["arg"] = (*at_least_tuple(current), arg)
 
                 else:
                     if arg not in g:  # Add the node only if it doesn't exist
                         default_value = f.defaults.get(arg, inspect.Parameter.empty)
                         g.add_node(arg, default_value=default_value)
                     g.add_edge(arg, f, arg=arg)
         return g
@@ -673,35 +389,50 @@
 
         Returns
         -------
         Callable[..., Any]
             The composed function that can be called with keyword arguments.
 
         """
-        root_args = self.arg_combinations(output_name, root_args_only=True)
+        if f := self._func.get(output_name):
+            return f
+        root_args = self.root_args(output_name)
         assert isinstance(root_args, tuple)
-        return _Function(self, output_name, root_args=root_args)
+        f = _Function(self, output_name, root_args=root_args)
+        self._func[output_name] = f
+        return f
 
-    def __call__(self, output_name: _OUTPUT_TYPE, **kwargs: Any) -> Any:
+    def __call__(
+        self,
+        __output_name__: _OUTPUT_TYPE | None = None,
+        /,
+        **kwargs: Any,
+    ) -> Any:
         """Call the pipeline for a specific return value.
 
         Parameters
         ----------
-        output_name
+        __output_name__
             The identifier for the return value of the pipeline.
+            Is None by default, in which case the unique leaf node is used.
+            This parameter is positional-only and the strange name is used
+            to avoid conflicts with the `output_name` argument that might be
+            passed via `kwargs`.
         kwargs
             Keyword arguments to be passed to the pipeline functions.
 
         Returns
         -------
         Any
             The return value of the pipeline.
 
         """
-        return self.func(output_name)(**kwargs)
+        if __output_name__ is None:
+            __output_name__ = self.unique_leaf_node.output_name
+        return self.func(__output_name__)(**kwargs)
 
     def _compute_cache_key(
         self,
         output_name: _OUTPUT_TYPE,
         kwargs: dict[str, Any],
     ) -> _CACHE_KEY_TYPE | None:
         """Compute the cache key for a specific output name.
@@ -727,27 +458,93 @@
         -------
         _CACHE_KEY_TYPE | None
             A tuple containing the output name and a tuple of root input keys
             and their corresponding values, or None if the cache key computation
             is skipped.
 
         """
-        root_args = self.arg_combinations(output_name, root_args_only=True)
+        root_args = self.root_args(output_name)
         assert isinstance(root_args, tuple)
         cache_key_items = []
         for k in sorted(root_args):
             if k not in kwargs:
                 # This means the computation was run with non-root inputs
                 # i.e., the output of a function was directly provided as an input to
                 # another function. In this case, we don't want to cache the result.
                 return None
             cache_key_items.append((k, kwargs[k]))
 
         return output_name, tuple(cache_key_items)
 
+    def _execute_pipeline(  # noqa: PLR0912
+        self,
+        *,
+        output_name: _OUTPUT_TYPE,
+        kwargs: Any,
+        all_results: dict[_OUTPUT_TYPE, Any],
+        full_output: bool,
+    ) -> Any:
+        if output_name in all_results:
+            return all_results[output_name]
+
+        func = self.output_to_func[output_name]
+        assert func.parameters is not None
+        result_from_cache = False
+        if func.cache and self.cache is not None:
+            cache_key = self._compute_cache_key(func.output_name, kwargs)
+            if cache_key is not None and cache_key in self.cache:
+                r = self.cache.get(cache_key)
+                _update_all_results(func, r, output_name, all_results, self.lazy)
+                result_from_cache = True
+                if not full_output:
+                    return all_results[output_name]
+
+        func_args = {}
+        for arg in func.parameters:
+            if arg in kwargs:
+                func_args[arg] = kwargs[arg]
+            elif arg in func.defaults:
+                func_args[arg] = func.defaults[arg]
+            else:
+                func_args[arg] = self._execute_pipeline(
+                    output_name=arg,
+                    kwargs=kwargs,
+                    all_results=all_results,
+                    full_output=full_output,
+                )
+
+        if result_from_cache:
+            # Can only happen if full_output is True
+            return all_results[output_name]
+        start_time = time.perf_counter()
+
+        r = _LazyFunction(func, kwargs=func_args) if self.lazy else func(**func_args)
+
+        if func.cache and cache_key is not None and self.cache is not None:
+            if isinstance(self.cache, HybridCache):
+                duration = time.perf_counter() - start_time
+                self.cache.put(cache_key, r, duration)
+            else:
+                self.cache.put(cache_key, r)
+
+        _update_all_results(func, r, output_name, all_results, self.lazy)
+        if func.save and not result_from_cache:
+            to_save = {k: all_results[k] for k in self.root_args(output_name)}
+            filename = generate_filename_from_dict(to_save)  # type: ignore[arg-type]
+            filename = func.__name__ / filename
+            to_save[output_name] = all_results[output_name]  # type: ignore[index]
+            assert func.save_function is not None
+            if self.lazy:
+                lazy_save = _LazyFunction(func.save_function, args=(filename, to_save))
+                r.add_delayed_callback(lazy_save)
+            else:
+                func.save_function(filename, to_save)  # type: ignore[arg-type]
+
+        return all_results[output_name]
+
     def _run_pipeline(
         self,
         output_name: _OUTPUT_TYPE,
         *,
         full_output: bool = False,
         **kwargs: Any,
     ) -> Any:
@@ -766,92 +563,21 @@
         Returns
         -------
         Any
             The return value of the pipeline or a dictionary mapping function
             names to their return values if full_output is True.
 
         """
-
-        def _update_all_results(
-            func: PipelineFunction,
-            r: Any,
-            output_name: _OUTPUT_TYPE,
-            all_results: dict[_OUTPUT_TYPE, Any],
-        ) -> None:
-            if isinstance(func.output_name, tuple) and not isinstance(
-                output_name,
-                tuple,
-            ):
-                for name in func.output_name:
-                    assert func.output_picker is not None
-                    all_results[name] = func.output_picker(r, name)
-            else:
-                all_results[func.output_name] = r
-
-        def _execute_pipeline(  # noqa: PLR0912
-            output_name: _OUTPUT_TYPE,
-            **kwargs: Any,
-        ) -> Any:
-            if output_name in all_results:
-                return all_results[output_name]
-
-            func = self.output_to_func[output_name]
-
-            if func is None:
-                msg = (
-                    f"Argument {output_name} is not in kwargs and has no default value."
-                )
-                raise ValueError(msg)
-
-            assert func.parameters is not None
-            result_from_cache = False
-            if func.cache:
-                cache_key = self._compute_cache_key(func.output_name, kwargs)
-                if cache_key is not None and cache_key in self.cache:
-                    r = self.cache.get(cache_key)
-                    assert r is not None
-                    _update_all_results(func, r, output_name, all_results)
-                    result_from_cache = True
-                    if not full_output:
-                        return all_results[output_name]
-
-            func_args = {}
-            for arg in func.parameters:
-                if arg not in kwargs and arg not in func.defaults:
-                    func_args[arg] = _execute_pipeline(arg, **kwargs)
-                elif arg in kwargs:
-                    func_args[arg] = kwargs[arg]
-                else:  # arg in func.defaults
-                    func_args[arg] = func.defaults[arg]
-            if result_from_cache:
-                # Can only happen if full_output is True
-                return all_results[output_name]
-            start_time = time.perf_counter()
-            r = func(**func_args)
-
-            if func.cache and cache_key is not None:
-                if isinstance(self.cache, HybridCache):
-                    duration = time.perf_counter() - start_time
-                    self.cache.put(cache_key, r, duration)
-                else:
-                    self.cache.put(cache_key, r)
-
-            _update_all_results(func, r, output_name, all_results)
-            if func.save and not result_from_cache:
-                root_args = self.arg_combinations(output_name, root_args_only=True)
-                to_save = {k: all_results[k] for k in root_args if k in all_results}
-                filename = generate_filename_from_dict(to_save)  # type: ignore[arg-type]
-                filename = func.__name__ / filename
-                to_save[output_name] = all_results[output_name]
-                assert func.save_function is not None
-                func.save_function(filename, to_save)  # type: ignore[arg-type]
-            return all_results[output_name]
-
         all_results: dict[_OUTPUT_TYPE, Any] = kwargs.copy()  # type: ignore[assignment]
-        _execute_pipeline(output_name, **kwargs)
+        self._execute_pipeline(
+            output_name=output_name,
+            kwargs=kwargs,
+            all_results=all_results,
+            full_output=full_output,
+        )
         return all_results if full_output else all_results[output_name]
 
     @property
     def node_mapping(self) -> dict[_OUTPUT_TYPE, PipelineFunction | str]:
         """Return a mapping from node names to nodes.
 
         Returns
@@ -868,14 +594,25 @@
                         mapping[name] = node
                 mapping[node.output_name] = node
             else:
                 assert isinstance(node, str)
                 mapping[node] = node
         return mapping
 
+    def _next_root_args(
+        self,
+        arg_set: set[tuple[str, ...]],
+    ) -> tuple[str, ...]:
+        """Find the tuple of root arguments."""
+        return next(
+            args
+            for args in arg_set
+            if all(isinstance(self.node_mapping[n], str) for n in args)
+        )
+
     def arg_combinations(
         self,
         output_name: _OUTPUT_TYPE,
         *,
         root_args_only: bool = False,
     ) -> set[tuple[str, ...]] | tuple[str, ...]:
         """Return the arguments required to compute a specific output.
@@ -893,22 +630,22 @@
         -------
         Set[Tuple[str, ...]]
             A set of tuples containing possible argument combinations.
 
         """
         if r := self._arg_combinations.get(output_name):
             if root_args_only:
-                return _next_root_args(self, r)
+                return self._next_root_args(r)
             return r
 
         def names(nodes: Iterable[PipelineFunction | str]) -> tuple[str, ...]:
             names: list[str] = []
             for n in nodes:
                 if isinstance(n, PipelineFunction):
-                    names.extend(_at_least_tuple(n.output_name))
+                    names.extend(at_least_tuple(n.output_name))
                 else:
                     assert isinstance(n, str)
                     names.append(n)
             return tuple(names)
 
         def sort_key(node: PipelineFunction | str) -> str:
             if isinstance(node, PipelineFunction):
@@ -945,32 +682,41 @@
                 compute_arg_mapping(func, head, new_args, [*replaced, node])
 
         head = self.node_mapping[output_name]
         arg_set: set[tuple[str, ...]] = set()
         compute_arg_mapping(head, head, [], [])  # type: ignore[arg-type]
         self._arg_combinations[output_name] = arg_set
         if root_args_only:
-            return _next_root_args(self, arg_set)
+            return self._next_root_args(arg_set)
         return arg_set
 
+    def root_args(self, output_name: _OUTPUT_TYPE) -> tuple[str, ...]:
+        """Return the root arguments required to compute a specific output."""
+        if r := self._root_args.get(output_name):
+            return r
+        root_args = self.arg_combinations(output_name, root_args_only=True)
+        root_args = cast(Tuple[str, ...], root_args)
+        self._root_args[output_name] = root_args
+        return root_args
+
     def func_dependencies(self, output_name: _OUTPUT_TYPE) -> list[_OUTPUT_TYPE]:
         """Return the functions required to compute a specific output."""
 
         def _predecessors(x: _OUTPUT_TYPE | PipelineFunction) -> list[_OUTPUT_TYPE]:
             preds = set()
             if isinstance(x, (str, tuple)):
                 x = self.node_mapping[x]
             for pred in self.graph.predecessors(x):
                 if isinstance(pred, PipelineFunction):
                     preds.add(pred.output_name)
                     for p in _predecessors(pred):
                         preds.add(p)
             return preds  # type: ignore[return-value]
 
-        return sorted(_predecessors(output_name), key=_at_least_tuple)
+        return sorted(_predecessors(output_name), key=at_least_tuple)
 
     def all_arg_combinations(
         self,
         *,
         root_args_only: bool = False,
     ) -> dict[_OUTPUT_TYPE, set[tuple[str, ...]]]:
         """Compute all possible argument mappings for the pipeline.
@@ -1001,15 +747,16 @@
                     root_args_only=root_args_only,
                 )
                 if not isinstance(arg_combinations, set):  # root_args_only=True
                     arg_combinations = {arg_combinations}
                 mapping[node.output_name] = arg_combinations
         return mapping
 
-    def _unique_leaf_node(self) -> PipelineFunction:
+    @functools.cached_property
+    def unique_leaf_node(self) -> PipelineFunction:
         """Return the unique leaf node of the pipeline graph."""
         leaf_nodes = self.leaf_nodes
         if len(leaf_nodes) != 1:  # pragma: no cover
             msg = (
                 "The pipeline has multiple leaf nodes. Please specify the output_name"
                 " argument to disambiguate.",
             )
@@ -1019,15 +766,15 @@
     def _func_node_colors(
         self,
         *,
         conservatively_combine: bool = False,
         output_name: _OUTPUT_TYPE | None = None,
     ) -> list[str]:
         if output_name is None:
-            output_name = self._unique_leaf_node().output_name
+            output_name = self.unique_leaf_node.output_name
 
         func_node_colors = []
         combinable_nodes = self._identify_combinable_nodes(
             output_name=output_name,
             conservatively_combine=conservatively_combine,
         )
         combinable_nodes = _combine_nodes(combinable_nodes)
@@ -1157,23 +904,23 @@
         current function being checked in the execution graph.
 
         """
         # Nested function _recurse performs the depth-first search and updates the
         # `combinable_nodes` dictionary.
 
         def _recurse(head: PipelineFunction) -> None:
-            head_args = self.arg_combinations(head.output_name, root_args_only=True)
+            head_args = self.root_args(head.output_name)
             funcs = set()
             i = 0
             for node in self.graph.predecessors(head):
                 if isinstance(node, (tuple, str)):  # node is root_arg
                     continue
                 i += 1
                 _recurse(node)
-                node_args = self.arg_combinations(node.output_name, root_args_only=True)
+                node_args = self.root_args(node.output_name)
                 if node_args == head_args:
                     funcs.add(node)
             if funcs and (not conservatively_combine or i == len(funcs)):
                 combinable_nodes[head] = funcs
 
         combinable_nodes: dict[PipelineFunction, set[PipelineFunction]] = {}
         func = self.node_mapping[output_name]
@@ -1235,15 +982,15 @@
 
         This process can significantly simplify complex pipelines, making them
         easier to understand and potentially improving performance by simplifying
         function calls.
 
         """
         if output_name is None:
-            output_name = self._unique_leaf_node().output_name
+            output_name = self.unique_leaf_node.output_name
         combinable_nodes = self._identify_combinable_nodes(
             output_name,
             conservatively_combine=conservatively_combine,
         )
         if not combinable_nodes:
             warnings.warn(
                 "No combinable nodes found, the pipeline cannot be simplified.",
@@ -1342,20 +1089,20 @@
             output_name,
             root_args_only=True,
         )
         for arg in root_args:
             func_only_graph.remove_node(arg)
         return nx.all_topological_sorts(func_only_graph)
 
-    @property
+    @functools.cached_property
     def leaf_nodes(self) -> list[PipelineFunction]:
         """Return the leaf nodes in the pipeline's execution graph."""
         return [node for node in self.graph.nodes() if self.graph.out_degree(node) == 0]
 
-    @property
+    @functools.cached_property
     def root_nodes(self) -> list[PipelineFunction]:
         """Return the root nodes in the pipeline's execution graph."""
         return [node for node in self.graph.nodes() if self.graph.in_degree(node) == 0]
 
     def all_transitive_paths(
         self,
         output_name: str,
@@ -1386,22 +1133,22 @@
             can produce the output. Each list of `PipelineFunction` represents a
             possible ordering of functions in that chain.
 
         """
         pipeline = self.simplified_pipeline(output_name) if simplify else self
 
         func_only_graph = pipeline.graph.copy()
-        root_args = pipeline.arg_combinations(output_name, root_args_only=True)
+        root_args = pipeline.root_args(output_name)
         for arg in root_args:
             func_only_graph.remove_node(arg)
 
         leaf = next(
             n
             for n in func_only_graph.nodes
-            if output_name in _at_least_tuple(n.output_name)
+            if output_name in at_least_tuple(n.output_name)
         )
         roots = [n for n, d in func_only_graph.in_degree() if d == 0]
         graph = nx.transitive_reduction(func_only_graph)
         return [list(nx.all_simple_paths(graph, root, leaf)) for root in roots]
 
     @property
     def profiling_stats(self) -> dict[str, ProfilingStats]:
@@ -1420,154 +1167,25 @@
                 pipeline_str += (
                     f"  {fn.output_name} = {fn.__name__}({', '.join(fn.parameters)})\n"
                 )
                 pipeline_str += f"    Possible input arguments: {input_args}\n"
         return pipeline_str
 
 
-def _wrap_dict_to_tuple(
-    func: Callable[..., Any],
-    inputs: tuple[str, ...],
-    output_name: str | tuple[str, ...],
-) -> Callable[..., Any]:
-    sig = inspect.signature(func)
-    new_params = [
-        inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
-        for name in inputs
-    ]
-    new_sig = sig.replace(parameters=new_params)
-
-    def call(*args: Any, **kwargs: Any) -> Any:
-        """Call the pipeline function with the root arguments."""
-        bound = new_sig.bind(*args, **kwargs)
-        bound.apply_defaults()
-        r = func(**bound.arguments)
-        if isinstance(output_name, tuple):
-            return tuple(r[k] for k in output_name)
-        return r[output_name]
-
-    call.__signature__ = new_sig  # type: ignore[attr-defined]
-
-    return call
-
-
-def _combine_nodes(
-    combinable_nodes: dict[PipelineFunction, set[PipelineFunction]],
-) -> dict[PipelineFunction, set[PipelineFunction]]:
-    """Reduce the dictionary of combinable nodes to a minimal set.
-
-    The input dictionary `combinable_nodes` indicates which nodes
-    (functions in the pipeline) can be combined together. The dictionary
-    keys are PipelineFunction objects, and the values are sets of
-    PipelineFunction objects that the key depends on and can be
-    combined with. For example,
-    if `combinable_nodes = {f6: {f5}, f5: {f1, f4}}`, it means that `f6`
-    can be combined with `f5`, and `f5` can be combined with `f1` and `f4`.
-
-    This method simplifies the input dictionary by iteratively checking each
-    node in the dictionary to see if it is a dependency of any other nodes.
-    If it is, the method replaces that dependency with the node's own
-    dependencies and removes the node from the dictionary. For example, if
-    `f5` is found to be a dependency of `f6`, then `f5` is replaced by its
-    own dependencies `{f1, f4}` in the `f6` entry,  and the `f5` entry is
-    removed from the dictionary. This results in a new
-    dictionary, `{f6: {f1, f4}}`.
-
-    The aim is to get a dictionary where each node only depends on nodes
-    that cannot be further combined. This simplified dictionary is useful for
-    constructing a simplified graph of the computation.
-
-    Parameters
-    ----------
-    combinable_nodes
-        A dictionary where the keys are PipelineFunction objects, and the
-        values are sets of PipelineFunction objects that can be combined
-        with the key.
-
-    Returns
-    -------
-    Dict[PipelineFunction, Set[PipelineFunction]]
-        A simplified dictionary where each node only depends on nodes
-        that cannot be further combined.
-
-    """
-    combinable_nodes = OrderedDict(combinable_nodes)
-    for _ in range(len(combinable_nodes)):
-        node, deps = combinable_nodes.popitem(last=False)
-        added_nodes = []
-        for _node, _deps in list(combinable_nodes.items()):
-            if node in _deps:
-                combinable_nodes[_node] |= deps
-                added_nodes.append(_node)
-        if not added_nodes:
-            combinable_nodes[node] = deps
-    return dict(combinable_nodes)
-
-
-def _get_signature(
-    combinable_nodes: dict[PipelineFunction, set[PipelineFunction]],
-    graph: nx.DiGraph,
-) -> tuple[dict[PipelineFunction, set[str]], dict[PipelineFunction, set[str]]]:
-    """Retrieve the inputs and outputs for the signature of the combinable nodes.
-
-    This function generates a mapping of the inputs and outputs required for
-    each node in the combinable_nodes dictionary. For each node, it collects
-    the outputs of all nodes it depends on and the parameters it and its
-    dependent nodes require. In addition, it considers additional outputs
-    based on the dependencies in the graph. It then filters these lists to
-    ensure that no parameter is considered an output and no output is
-    considered a parameter.
-
-    Parameters
-    ----------
-    combinable_nodes
-        Dictionary containing the nodes that can be combined together.
-        The keys of the dictionary are the nodes that can be combined,
-        and the values are sets of nodes that they depend on.
-    graph
-        The directed graph of the pipeline functions. Each node represents a
-        function, and each edge represents a dependency relationship between
-        functions.
-
-    Returns
-    -------
-    all_inputs : dict[PipelineFunction, set[str]]
-        Dictionary where keys are nodes and values are sets of parameter
-        names that the node and its dependent nodes require.
-    all_outputs : dict[PipelineFunction, set[str]]
-        Dictionary where keys are nodes and values are sets of output names
-        that the node and its dependent nodes produce, plus additional output
-        names based on the dependency relationships in the graph.
-
-    """
-    all_inputs = {}
-    all_outputs = {}
-    for node, to_replace in combinable_nodes.items():
-        outputs = set(_at_least_tuple(node.output_name))
-        parameters = set(node.parameters)
-        additional_outputs = set()  # parameters that are outputs to other functions
-        for f in to_replace:
-            outputs |= set(_at_least_tuple(f.output_name))
-            parameters |= set(f.parameters)
-            for successor in graph.successors(f):
-                if successor not in to_replace and successor != node:
-                    edge = graph.edges[f, successor]
-                    additional_outputs |= set(_at_least_tuple(edge["arg"]))
-        all_outputs[node] = (outputs - parameters) | additional_outputs
-        all_inputs[node] = parameters - outputs
-    return all_inputs, all_outputs
-
-
-def generate_filename_from_dict(obj: dict[str, Any], suffix: str = ".pickle") -> Path:
-    """Generate a filename from a dictionary."""
-    keys = "_".join(obj.keys())
-    obj_string = json.dumps(
-        obj,
-        sort_keys=True,
-    )  # Convert the dictionary to a sorted string
-    obj_bytes = obj_string.encode()  # Convert the string to bytes
-
-    sha256_hash = hashlib.sha256()
-    sha256_hash.update(obj_bytes)
-    # Convert the hash to a hexadecimal string for the filename
-    str_hash = sha256_hash.hexdigest()
-    return Path(f"{keys}__{str_hash}{suffix}")
+def _update_all_results(
+    func: PipelineFunction,
+    r: Any,
+    output_name: _OUTPUT_TYPE,
+    all_results: dict[_OUTPUT_TYPE, Any],
+    lazy: bool,  # noqa: FBT001
+) -> None:
+    if isinstance(func.output_name, tuple) and not isinstance(output_name, tuple):
+        # Function produces multiple outputs, but only one is requested
+        assert func.output_picker is not None
+        for name in func.output_name:
+            all_results[name] = (
+                _LazyFunction(func.output_picker, args=(r, name))
+                if lazy
+                else func.output_picker(r, name)
+            )
+    else:
+        all_results[func.output_name] = r
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pipefunc-0.4.0/pipefunc/_plotting.py` & `pipefunc-0.5.0/pipefunc/_plotting.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.4.0/pipefunc/_sweep.py` & `pipefunc-0.5.0/pipefunc/_sweep.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 from collections import defaultdict
 from collections.abc import Iterable, Mapping
 from itertools import product
 from typing import TYPE_CHECKING, Any, Callable, Generator, Hashable, Sequence
 
 import networkx as nx
 
-if TYPE_CHECKING:
-    from pipefunc._pipefunc import _OUTPUT_TYPE, Pipeline, PipelineFunction
-
+from pipefunc._utils import at_least_tuple
 
-def _at_least_tuple(x: Any) -> tuple[Any, ...]:
-    """Convert x to a tuple if it is not already a tuple."""
-    return x if isinstance(x, tuple) else (x,)
+if TYPE_CHECKING:
+    from pipefunc._pipeline import _OUTPUT_TYPE, Pipeline, PipelineFunction
 
 
 def _combined_exclude(
     *func: Callable[[Mapping[str, Any]], bool] | None,
 ) -> Callable[[Mapping[str, Any]], bool] | None:
     """Combine multiple exclude functions into one."""
     funcs = [f for f in func if f is not None]
@@ -124,16 +121,17 @@
                         combination[key] = func(combination)
                 if self.exclude is None or not self.exclude(combination):
                     yield combination
         else:
             # Otherwise, create a product considering the provided dimensions.
             product_parts = []
             for dim_group in self.dims:
-                dims = _at_least_tuple(dim_group)
+                dims = at_least_tuple(dim_group)
                 dim_seqs = [self.items[dim] for dim in dims]
+                _check_dim_lengths(dim_seqs, dims)
                 product_parts.append([dict(zip(dims, res)) for res in zip(*dim_seqs)])
             for combo in product(*product_parts):
                 combination = {k: v for item in combo for k, v in item.items()}
                 if self.constants is not None:
                     for key, value in self.constants.items():
                         combination.setdefault(key, value)
                 if self.derivers is not None:
@@ -199,15 +197,15 @@
             total_length = 1
             for value in self.items.values():
                 total_length *= len(value)
             return total_length
         # Otherwise, calculate lengths considering the provided dimensions.
         total_length = 1
         for dim_group in self.dims:
-            dims = _at_least_tuple(dim_group)
+            dims = at_least_tuple(dim_group)
             group_length = len(self.items[dims[0]])
             total_length *= group_length
         return total_length
 
     def __add__(self, other: Sweep) -> MultiSweep:
         """Combine this Sweep with another one, creating a MultiSweep."""
         if not isinstance(other, Sweep):
@@ -356,14 +354,23 @@
         if isinstance(other, MultiSweep):
             self.sweeps.extend(other.sweeps)
         else:
             self.sweeps.append(other)
         return self
 
 
+def _check_dim_lengths(seqs: Sequence[Sequence[Any]], dims: tuple[str, ...]) -> None:
+    """Check that all sequences in a list have the same length."""
+    seq_len = len(seqs[0])
+    for seq, dim in zip(seqs, dims):
+        if len(seq) != seq_len:
+            msg = f"Dimension '{dim}' has a different length than the other dimensions."
+            raise ValueError(msg)
+
+
 def generate_sweep(
     items: dict[str, Sequence[Any]],
     dims: list[str | tuple[str, ...]] | None = None,
     exclude: Callable[[Mapping[str, Any]], bool] | None = None,
     constants: Mapping[str, Any] | None = None,
     derivers: dict[str, Callable[[dict[str, Any]], Any]] | None = None,
 ) -> list[dict[str, Any]]:
@@ -646,22 +653,22 @@
     -------
     Tuple[List[Any], dict]
         A tuple where the first element is a list of the minimal set of argument
         combinations for each function in the execution order and the second
         element is a nested dictionary that represents the sweep combinations.
 
     """
-    root_args = pipeline.arg_combinations(output_name, root_args_only=True)
+    root_args = pipeline.root_args(output_name)
     assert isinstance(root_args, tuple)
     root_args_set = set(root_args)
     left_over = root_args_set.copy()
 
     left_overs: list[tuple[str, ...]] = []
     for f in execution_order:
-        f_root_args = pipeline.arg_combinations(f.output_name, root_args_only=True)
+        f_root_args = pipeline.root_args(f.output_name)
         assert isinstance(f_root_args, tuple)
         left_over = left_over - set(f_root_args)
         if not left_over:
             break
         args = tuple(sorted(root_args_set - left_over))
         if args not in left_overs:
             left_overs.append(args)
```

### Comparing `pipefunc-0.4.0/pipefunc.egg-info/PKG-INFO` & `pipefunc-0.5.0/pipefunc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
@@ -86,38 +86,31 @@
 - [:hammer_and_wrench: Development](#hammer_and_wrench-development)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 <!-- toc-end -->
 
 ## :thinking: What is this?
 
-`pipefunc` is a Python library designed to create and manage complex networks of interdependent functions, often known as function pipelines.
+`pipefunc` is a Python library that simplifies the creation and management of complex function pipelines. It allows you to declare the dependencies between functions and automatically organizes the execution order to satisfy these dependencies.
 
-In a function pipeline, each function can have dependencies on the results of other functions. Managing these dependencies, ensuring each function has the inputs it needs, and determining the order of execution can become an annoying bookkeeping task in complex cases.
+`pipefunc` provides a range of features to streamline your workflow, including pipeline visualization, flexible function arguments, support for multiple outputs, pipeline simplification, resource usage profiling, parallel execution, caching, and parameter sweep utilities.
 
-`pipefunc` simplifies this process by allowing you to declare the dependencies of each function and automatically organizing the execution order to satisfy these dependencies. Additionally, the library provides features for visualizing the function pipeline, simplifying the pipeline graph, caching function results for efficiency, and profiling resource usage for optimization.
-
-For example, imagine you have a set of functions where `function B` needs the output from `function A`, and `function C` needs the outputs from both `function A` and `function B`. `pipefunc` allows you to specify these dependencies when you create the functions and then automatically manages their execution. It also provides tools for visualizing this function network, simplifying it if possible, and understanding the resource usage of each function.
-
-The library is designed to be an efficient and flexible tool for managing complex function dependencies in an intuitive and clear way. Whether you're dealing with data processing tasks, scientific computations, machine learning (AI) workflows, or other scenarios where functions depend on one another, `pipefunc` can help streamline your code and improve your productivity.
+Whether you're working with data processing, scientific computations, machine learning (AI) workflows, or any other scenario involving interdependent functions, `pipefunc` helps you focus on the logic of your code while it handles the intricacies of function dependencies and execution order.
 
 ## :rocket: Key Features
 
-Some of the key features of `pipefunc` include:
-
-1. 🚀 **Function Composition and Pipelining:** The core functionality of `pipefunc` is to create a pipeline of functions, allowing you to feed the output of one function into another, and execute them in the right order.
-1. 📊 **Visualizing Pipelines:** `pipefunc` can generate a visual graph of the function pipeline, making it easier to understand the flow of data.
-1. 💡 **Flexible Function Arguments:** `pipefunc` lets you call a function with different combinations of arguments, automatically determining which other functions to call based on the arguments you provide.
-1. 👥 **Multiple Outputs:** `pipefunc` supports functions that return multiple results, allowing each result to be used as input to other functions.
-1. ➡️ **Reducing Pipelines:** `pipefunc` can simplify a complex pipeline by merging nodes, improving computational efficiency at the cost of losing visibility into some intermediate steps.
-1. 🎛️ **Resources Report:** `pipefunc` provides a report on the performance of your pipeline, including CPU usage, memory usage, and execution time, helping you identify bottlenecks and optimize your code.
-1. 🔄 **Parallel Execution and Caching:** `pipefunc` supports parallel execution of functions, and caching of results to avoid redundant computation.
-1. 🔍 **Parameter Sweeps:** `pipefunc` provides a utility for generating combinations of parameters to use in a parameter sweep, along with the ability to cache results to optimize the sweep.
-1. 🛠️ **Flexibility and Ease of Use:** `pipefunc` is a lightweight, flexible, and powerful tool for managing complex function dependencies in a clear and intuitive way, designed to improve your productivity in any scenario where functions depend on one another.
-
+1. 🚀 **Function Composition and Pipelining**: Create pipelines where the output of one function feeds into another, with `pipefunc` handling the execution order.
+2. 📊 **Pipeline Visualization**: Generate visual graphs of your pipelines to better understand the flow of data.
+3. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
+4. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
+5. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
+6. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
+7. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
+8. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
+9. 🛠️ **Flexibility and Ease of Use**: Manage complex function dependencies in a clear, intuitive way with this lightweight yet powerful tool.
 
 ## :test_tube: How does it work?
 
 pipefunc provides a Pipeline class that you use to define your function pipeline.
 You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify a function's output name and dependencies.
 Once your pipeline is defined, you can execute it for specific output values, simplify it by combining functions with the same root arguments, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
 For more detailed usage instructions and examples, please check the usage example provided in the package.
```

### Comparing `pipefunc-0.4.0/pyproject.toml` & `pipefunc-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipefunc-0.4.0/tests/test_perf.py` & `pipefunc-0.5.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.4.0/tests/test_pipefunc.py` & `pipefunc-0.5.0/tests/test_pipefunc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """Tests for pipefunc.py."""
 
+from __future__ import annotations
+
 import inspect
+import pickle
+from typing import TYPE_CHECKING
 
 import pytest
 
 from pipefunc import (
     Pipeline,
     PipelineFunction,
     Sweep,
     count_sweep,
     get_precalculation_order,
     pipefunc,
 )
-from pipefunc._pipefunc import _combine_nodes, _get_signature
+
+if TYPE_CHECKING:
+    from pathlib import Path
 
 
 def test_pipeline_and_all_arg_combinations() -> None:
     @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
 
@@ -56,14 +62,54 @@
     kw["d"] = f2(b=kw["b"], c=kw["c"])
     kw["e"] = f3(c=kw["c"], d=kw["d"], x=kw["x"])
     for params in all_args["e"]:
         _kw = {k: kw[k] for k in params}
         assert fe(**_kw) == kw["e"]
 
 
+def test_pipeline_and_all_arg_combinations_lazy() -> None:
+    @pipefunc(output_name="c")
+    def f1(a, b):
+        return a + b
+
+    @pipefunc(output_name="d")
+    def f2(b, c, x=1):
+        return b * c * x
+
+    @pipefunc(output_name="e")
+    def f3(c, d, x=1):
+        return c * d * x
+
+    pipeline = Pipeline([f1, f2, f3], debug=True, profile=True, lazy=True)
+
+    fc = pipeline.func("c")
+    fd = pipeline.func("d")
+    c = f1(a=2, b=3)
+    assert fc(a=2, b=3).evaluate() == c == fc(b=3, a=2).evaluate() == 5
+    assert fd(a=2, b=3).evaluate() == f2(b=3, c=c) == fd(b=3, c=c).evaluate() == 15
+
+    fe = pipeline.func("e")
+    assert (
+        fe(a=2, b=3, x=1).evaluate()
+        == fe(a=2, b=3, d=15, x=1).evaluate()
+        == f3(c=c, d=15, x=1)
+        == 75
+    )
+
+    all_args = pipeline.all_arg_combinations()
+
+    kw = {"a": 2, "b": 3, "x": 1}
+    kw["c"] = f1(a=kw["a"], b=kw["b"])
+    kw["d"] = f2(b=kw["b"], c=kw["c"])
+    kw["e"] = f3(c=kw["c"], d=kw["d"], x=kw["x"])
+    for params in all_args["e"]:
+        _kw = {k: kw[k] for k in params}
+        assert fe(**_kw).evaluate() == kw["e"]
+
+
 @pytest.mark.parametrize(
     "f2",
     [
         PipelineFunction(
             lambda b, c, x: b * c * x,
             output_name="d",
             renames={"x": "xx"},
@@ -279,73 +325,97 @@
 
     def f6(b, f5):
         return b + f5
 
     def f7(a, f2, f6):
         return a + f2 + f6
 
-    pipeline = Pipeline([f1, f2, f3, f4, f5, f6, f7])
+    pipeline = Pipeline([f1, f2, f3, f4, f5, f6, f7], lazy=True)
 
-    pipeline("f7", a=1, b=2, c=3, d=4, e=5)
+    r = pipeline("f7", a=1, b=2, c=3, d=4, e=5)
+    assert r.evaluate() == 52
 
 
-def test_tuple_outputs():
+def test_tuple_outputs(tmp_path: Path):
     cache = True
 
     @pipefunc(
         output_name=("c", "_throw"),
         profile=True,
         debug=True,
         cache=cache,
         output_picker=dict.__getitem__,
     )
     def f_c(a, b):
         return {"c": a + b, "_throw": 1}
 
-    @pipefunc(output_name=("d", "e"), cache=cache)
+    def save_function(fname, result):
+        p = tmp_path / fname
+        p.parent.mkdir(parents=True, exist_ok=True)
+        with p.open("wb") as f:
+            pickle.dump(result, f)
+
+    @pipefunc(
+        output_name=("d", "e"),
+        cache=cache,
+        save=True,
+        save_function=save_function,
+    )
     def f_d(b, c, x=1):  # noqa: ARG001
         return b * c, 1
 
     @pipefunc(
         output_name=("g", "h"),
         output_picker=getattr,
         cache=cache,
+        save=True,
+        save_function=save_function,
     )
     def f_e(c, e, x=1):  # noqa: ARG001
         from types import SimpleNamespace
 
         print(f"Called f_e with c={c} and e={e}")
         return SimpleNamespace(g=c + e, h=c - e)
 
     @pipefunc(output_name="i", cache=cache)
     def f_i(h, g):
         return h + g
 
-    pipeline = Pipeline([f_c, f_d, f_e, f_i], debug=True, profile=True, cache="shared")
+    pipeline = Pipeline(
+        [f_c, f_d, f_e, f_i],
+        debug=True,
+        profile=True,
+        cache_type="lru",
+        lazy=True,
+        cache_kwargs={"shared": False},
+    )
     f = pipeline.func("i")
-    assert f.call_full_output(a=1, b=2, x=3)["i"] == f(a=1, b=2, x=3)
+    r = f.call_full_output(a=1, b=2, x=3)["i"].evaluate()
+    assert r == f(a=1, b=2, x=3).evaluate()
     assert (
         pipeline.arg_combinations("g", root_args_only=True)
         == pipeline.arg_combinations("h", root_args_only=True)
         == pipeline.arg_combinations(("g", "h"), root_args_only=True)
         == ("a", "b", "x")
     )
-    assert pipeline.cache.cache[(("d", "e"), (("a", 1), ("b", 2), ("x", 3)))] == (6, 1)
-    assert pipeline.func(("g", "h"))(a=1, b=2, x=3).g == 4
+    key = (("d", "e"), (("a", 1), ("b", 2), ("x", 3)))
+    assert pipeline.cache is not None
+    assert pipeline.cache.cache[key].evaluate() == (6, 1)
+    assert pipeline.func(("g", "h"))(a=1, b=2, x=3).evaluate().g == 4
     assert pipeline.func_dependencies("i") == [("c", "_throw"), ("d", "e"), ("g", "h")]
 
     assert (
         pipeline.func_dependencies("g")
         == pipeline.func_dependencies("h")
         == pipeline.func_dependencies(("g", "h"))
         == [("c", "_throw"), ("d", "e")]
     )
 
     f = pipeline.func(("g", "h"))
-    r = f(a=1, b=2, x=3)
+    r = f(a=1, b=2, x=3).evaluate()
     assert r.g == 4
     assert r.h == 2
 
     edges = {
         (f_c, f_d): {"arg": "c"},
         (f_c, f_e): {"arg": "c"},
         ("a", f_c): {"arg": "a"},
@@ -389,204 +459,106 @@
     pipeline = Pipeline([f_d, f_e, f_i, f_gg])
     sweep = Sweep({"a": [1, 2], "b": [3, 4], "x": [5, 6]})
     cnt = count_sweep("i", sweep, pipeline)
     # f_d is skipped because max(cnt) is 1
     assert get_precalculation_order(pipeline, cnt) == [f_e, f_gg]
 
 
-def test_identify_combinable_nodes():
-    @pipefunc(output_name=("d", "e"))
-    def f_d(b, g, x=1):  # noqa: ARG001
-        pass
-
-    @pipefunc(output_name=("g", "h"))
-    def f_e(a, x=1):  # noqa: ARG001
-        pass
-
-    @pipefunc(output_name="gg")
-    def f_gg(g):  # noqa: ARG001
-        pass
-
-    @pipefunc(output_name="i")
-    def f_i(gg, b, e):  # noqa: ARG001
-        pass
-
-    pipeline = Pipeline([f_d, f_e, f_i, f_gg])
-    combinable_nodes = pipeline._identify_combinable_nodes(
-        "i",
-        conservatively_combine=True,
-    )
-    assert combinable_nodes == {f_gg: {f_e}}
-    sig_in, sig_out = _get_signature(combinable_nodes, pipeline.graph)
-    assert sig_in == {f_gg: {"a", "x"}}
-    assert sig_out == {f_gg: {"gg", "h", "g"}}
-    combinable_nodes = pipeline._identify_combinable_nodes(
-        "i",
-        conservatively_combine=False,
-    )
-    assert combinable_nodes == {f_gg: {f_e}, f_i: {f_d}}
-    sig_in, sig_out = _get_signature(combinable_nodes, pipeline.graph)
-    assert sig_in == {f_gg: {"a", "x"}, f_i: {"g", "b", "gg", "x"}}
-    assert sig_out == {f_gg: {"gg", "h", "g"}, f_i: {"d", "i"}}
-
-
-def test_conservatively_combine():
-    @pipefunc(output_name="x")
-    def f1(a):
-        return a
-
-    @pipefunc(output_name="y")
-    def f2(b, x):
-        return x * b
-
-    @pipefunc(output_name="z")
-    def f3(b, x, y):
-        return x * y * b
-
-    pipeline = Pipeline([f1, f2, f3], debug=True, profile=True)
-
-    root_args = pipeline.all_arg_combinations(root_args_only=True)
-    assert root_args == {"x": {("a",)}, "y": {("a", "b")}, "z": {("a", "b")}}
-
-    # Test with conservatively_combine=True
-    combinable_nodes_true = pipeline._identify_combinable_nodes(
-        "z",
-        conservatively_combine=True,
-    )
-    assert combinable_nodes_true == {}
-
-    # Test simplified_pipeline with conservatively_combine=True
-    simplified_pipeline_true = pipeline.simplified_pipeline(
-        "z",
-        conservatively_combine=True,
-    )
-    simplified_functions_true = simplified_pipeline_true.functions
-    assert len(simplified_functions_true) == 3
-    function_names_true = [f.__name__ for f in simplified_functions_true]
-    assert "f1" in function_names_true
-    assert "f2" in function_names_true
-    assert "f3" in function_names_true
-
-    # Test with conservatively_combine=False
-    combinable_nodes_false = pipeline._identify_combinable_nodes(
-        "z",
-        conservatively_combine=False,
-    )
-    assert combinable_nodes_false == {f3: {f2}}
+@pytest.mark.parametrize("cache", [True, False])
+def test_full_output(cache, tmp_path: Path):
+    from pipefunc import Pipeline
 
-    # Test simplified_pipeline with conservatively_combine=False
-    simplified_pipeline_false = pipeline.simplified_pipeline(
-        "z",
-        conservatively_combine=False,
-    )
-    simplified_functions_false = simplified_pipeline_false.functions
-    assert len(simplified_functions_false) == 2
-    function_names_false = [f.__name__ for f in simplified_functions_false]
-    assert "f1" in function_names_false
-    assert "combined_f3" in function_names_false
-
-    # Check that the combined function has the expected input and output arguments
-    combined_f3 = next(
-        f for f in simplified_functions_false if f.__name__ == "combined_f3"
-    )
-    assert combined_f3.parameters == ["b", "x"]
-    assert combined_f3.output_name == "z"
+    def save_function(fname, result):
+        p = tmp_path / fname
+        p.parent.mkdir(parents=True, exist_ok=True)
+        with p.open("wb") as f:
+            pickle.dump(result, f)
 
-    # Check that the simplified pipeline produces the same output as the original pipeline
-    input_data = {"a": 2, "b": 3}
-    original_output = pipeline("z", **input_data)
-    simplified_output_true = simplified_pipeline_true("z", **input_data)
-    simplified_output_false = simplified_pipeline_false("z", **input_data)
-    assert original_output == simplified_output_true == simplified_output_false
+    @pipefunc(output_name="f1", save=True, save_function=save_function)
+    def f1(a, b):
+        return a + b
 
-    assert pipeline._func_node_colors() == ["C1", "C0", "C0"]
+    @pipefunc(output_name=("f2i", "f2j"), save=True, save_function=save_function)
+    def f2(f1):
+        return 2 * f1, 1
 
+    @pipefunc(output_name="f3", save=True, save_function=save_function)
+    def f3(a, f2i):
+        return a + f2i
+
+    if cache:
+        cache_dir = tmp_path / "cache"
+        cache_dir.mkdir(exist_ok=True)
+        cache_kwargs = {"cache_type": "disk", "cache_kwargs": {"cache_dir": cache_dir}}
+    else:
+        cache_kwargs = {}
+    pipeline = Pipeline([f1, f2, f3], **cache_kwargs)  # type: ignore[arg-type]
+    for f in pipeline.functions:
+        f.cache = cache
+    pipeline("f3", a=1, b=2)
+    func = pipeline.func("f3")
+    assert func.call_full_output(a=1, b=2) == {
+        "a": 1,
+        "b": 2,
+        "f1": 3,
+        "f2i": 6,
+        "f2j": 1,
+        "f3": 7,
+    }
+    if cache:
+        assert len(list(cache_dir.glob("*.pkl"))) == 3
 
-def test_identify_combinable_nodes2():
-    def f1(a, b, c, d):
-        return a + b + c + d
 
-    def f2(a, b, e):
-        return a + b + e
+def test_lazy_pipeline():
+    @pipefunc(output_name="c", cache=True)
+    def f1(a, b):
+        return a + b
 
-    def f3(a, b, f1):
-        return a + b + f1
+    @pipefunc(output_name="d", cache=True)
+    def f2(b, c, x=1):
+        return b * c * x
 
-    def f4(f1, f3):
-        return f1 + f3
+    @pipefunc(output_name="e", cache=True)
+    def f3(c, d, x=1):
+        return c * d * x
 
-    def f5(f1, f4):
-        return f1 + f4
+    pipeline = Pipeline([f1, f2, f3], lazy=True)
 
-    def f6(b, f5):
-        return b + f5
+    f = pipeline.func("e")
+    r = f(a=1, b=2, x=3).evaluate()
+    assert r == 162
+    r = f.call_full_output(a=1, b=2, x=3)["e"].evaluate()
+    assert r == 162
 
-    def f7(a, f2, f6):
-        return a + f2 + f6
 
-    pipeline = Pipeline([f1, f2, f3, f4, f5, f6, f7])
-    m = pipeline.node_mapping
+@pipefunc(output_name="test_function")
+def test_function(arg1: str, arg2: str) -> str:
+    return f"{arg1} {arg2}"
 
-    expected = {m["f6"]: {m["f1"], m["f3"], m["f4"], m["f5"]}}
-    combinable_nodes = pipeline._identify_combinable_nodes("f7")
-    simplified_combinable_nodes = _combine_nodes(combinable_nodes)
-    assert simplified_combinable_nodes == expected
-
-    sig_in, sig_out = _get_signature(simplified_combinable_nodes, pipeline.graph)
-    assert sig_in == {m["f6"]: {"a", "b", "c", "d"}}
-    assert sig_out == {m["f6"]: {"f6"}}
 
-    # Test simplified_pipeline
-    simplified_pipeline = pipeline.simplified_pipeline()
-    assert (
-        pipeline._unique_leaf_node().output_name
-        == simplified_pipeline._unique_leaf_node().output_name
-        == "f7"
-    )
-    simplified_functions = simplified_pipeline.functions
+pipeline = Pipeline([test_function])
 
-    # Check that the simplified pipeline has the expected number of functions
-    assert len(simplified_functions) == 3
 
-    # Check that the simplified pipeline has the expected function names
-    function_names = [f.__name__ for f in simplified_functions]
-    assert "f2" in function_names
-    assert "combined_f6" in function_names
-    assert "f7" in function_names
-
-    # Check that the combined function has the expected input and output arguments
-    combined_f6 = next(f for f in simplified_functions if f.__name__ == "combined_f6")
-    assert combined_f6.parameters == ["a", "b", "c", "d"]
-    assert combined_f6.output_name == "f6"
-
-    # Check that the simplified pipeline produces the same output as the original pipeline
-    input_data = {"a": 1, "b": 2, "c": 3, "d": 4, "e": 5}
-    original_output = pipeline("f7", **input_data)
-    simplified_output = simplified_pipeline("f7", **input_data)
-    assert original_output == simplified_output
+def test_function_pickling():
+    # Get the _Function instance from the pipeline
+    func = pipeline.func("test_function")
 
+    # Pickle the _Function instance
+    pickled_func = pickle.dumps(func)
 
-@pytest.mark.parametrize("cache", [True, False])
-def test_full_output(cache):
-    from pipefunc import Pipeline
-
-    def f1(a, b):
-        return a + b
+    # Unpickle the _Function instance
+    unpickled_func = pickle.loads(pickled_func)  # noqa: S301
 
-    def f2(f1):
-        return 2 * f1
+    # Assert that the unpickled instance has the same attributes
+    assert unpickled_func.output_name == "test_function"
+    assert unpickled_func.root_args == ("arg1", "arg2")
 
-    def f3(a, f2):
-        return a + f2
+    # Assert that the unpickled instance behaves the same as the original
+    result = unpickled_func(arg1="hello", arg2="world")
+    assert result == "hello world"
 
-    pipeline = Pipeline([f1, f2, f3])
-    for f in pipeline.functions:
-        f.cache = cache
-    pipeline("f3", a=1, b=2)
-    func = pipeline.func("f3")
-    assert func.call_full_output(a=1, b=2) == {
-        "a": 1,
-        "b": 2,
-        "f1": 3,
-        "f2": 6,
-        "f3": 7,
+    # Assert that the call_with_root_args method is recreated after unpickling
+    assert unpickled_func.call_with_root_args is not None
+    assert unpickled_func.call_with_root_args.__signature__.parameters.keys() == {
+        "arg1",
+        "arg2",
     }
```

### Comparing `pipefunc-0.4.0/tests/test_sweep.py` & `pipefunc-0.5.0/tests/test_sweep.py`

 * *Files identical despite different names*

