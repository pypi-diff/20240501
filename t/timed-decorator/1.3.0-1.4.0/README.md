# Comparing `tmp/timed_decorator-1.3.0.tar.gz` & `tmp/timed_decorator-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timed_decorator-1.3.0.tar", last modified: Mon Apr 29 10:43:09 2024, max compression
+gzip compressed data, was "timed_decorator-1.4.0.tar", last modified: Wed May  1 09:05:04 2024, max compression
```

## Comparing `timed_decorator-1.3.0.tar` & `timed_decorator-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.250914 timed_decorator-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/tests/test_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.250914 timed_decorator-1.3.0/timed_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/nested_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/simple_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/timed_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/tests/test_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/timed_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/nested_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/simple_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/timed_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/top_level.txt
```

### Comparing `timed_decorator-1.3.0/LICENSE` & `timed_decorator-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.3.0/PKG-INFO` & `timed_decorator-1.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,43 @@
-Metadata-Version: 2.1
-Name: timed-decorator
-Version: 1.3.0
-Summary: A timing decorator for python functions.
-Author-email: George Stoica <george.stoica@senticlab.com>
-Maintainer-email: George Stoica <george.stoica@senticlab.com>
-License: Copyright (c) 2024 George Stoica
-        
-        Permission is hereby granted, free of charge, to any person obtaining
-        a copy of this software and associated documentation files (the
-        "Software"), to deal in the Software without restriction, including
-        without limitation the rights to use, copy, modify, merge, publish,
-        distribute, sublicense, and/or sell copies of the Software, and to
-        permit persons to whom the Software is furnished to do so, subject to
-        the following conditions:
-        
-        The above copyright notice and this permission notice shall be
-        included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-        NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-        LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-        WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: repository, https://github.com/ancestor-mithril/timed-decorator
-Keywords: timing
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-
 # timed-decorator
 
+Simple and configurable timing decorator with little overhead that can be easily attached to python functions to measure their execution time.
+Can easily display parameter types and lengths if available and is compatible with NumPy ndarrays, Pandas DataFrames and PyTorch tensors.
+
+
 ## Installation
 
 ```
 pip install --upgrade timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
-```py
-import torch
-from torch import Tensor
 
+```py
 from timed_decorator.simple_timed import timed
 
 
-@timed(show_args=True)
-def batched_euclidean_distance(x: Tensor, y: Tensor) -> Tensor:
-    diff = x @ y.T
-    x_squared = (x ** 2).sum(dim=1)
-    y_squared = (b ** 2).sum(dim=1)
-    return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
-
+@timed()
+def fibonacci(n: int) -> int:
+    assert n > 0
+    a, b = 0, 1
+    for _ in range(n):
+        a, b = b, a + b
+    return a
 
-a = torch.rand((10000, 800))
-b = torch.rand((12000, 800))
-batched_euclidean_distance(a, b)
 
-if torch.cuda.is_available():
-    a = a.cuda()
-    b = b.cuda()
-    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
-```
-Prints:
-```
-batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
-batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
+fibonacci(10000)
+# fibonacci() -> total time: 1114100ns
 ```
 
+For more advanced usage, consider registering a timed decorator and using it afterward through your codebase. See [Registering a timed decorator](#registering-a-timed-decorator).
+
 ### Documentation
 
 1. `timed`
     * `collect_gc` (`bool`): If `True`, runs a full garbage collection before timing the wrapped function. Default: `True`.
     * `disable_gc` (`bool`): If `True`, disabled garbage collection during function execution. Default: `False`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
@@ -92,18 +45,28 @@
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
     * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
     * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key.  If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
+3. `create_timed_decorator` registers a timed decorator with a given name.
+   * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
+   * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
+   * Also receives all the other arguments accepted by `timed` and `nested_timed`.
+
+4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call.
+   * `name` (`str`): The name of the timed decorator registered using `timed_decorator.builder.create_timed_decorator`.
+
+
 ### Examples
 
 Simple usage.
 ```py
 from timed_decorator.simple_timed import timed
 
 
@@ -319,14 +282,27 @@
     np.random.rand(1, 3),
     weights=[i / 10 for i in range(1)],
     inplace=True
 )
 # numpy_operation([array([[0.74500602, 0.70666224, 0.83888559]])], [[0.74579988 0.51878032 0.06419635]], ('weights', '[0.0]'), ('inplace', 'True')) -> total time: 185300ns
 ```
 
+Using the fully qualified name for timing. 
+
+```py
+from time import sleep
+from timed_decorator.simple_timed import timed
+class ClassA:
+    @timed(use_qualname=True)
+    def wait(self, x):
+        sleep(x)
+ClassA().wait(0.1)
+# ClassA.wait() -> total time: 100943000ns
+```
+
 ### Nested timing decorator
 
 ```py
 from time import sleep
 
 from timed_decorator.nested_timed import nested_timed
 
@@ -433,7 +409,131 @@
 print(ns)
 ```
 Prints
 ```
 {'fn': 1000767300}
 {'fn': 2001006100}
 ```
+
+### Compatible with PyTorch tensors
+
+Synchronizes cuda device when cuda tensors are passed as function parameters.
+
+```py
+import torch
+from torch import Tensor
+
+from timed_decorator.simple_timed import timed
+
+
+@timed(show_args=True)
+def batched_euclidean_distance(x: Tensor, y: Tensor) -> Tensor:
+    diff = x @ y.T
+    x_squared = (x ** 2).sum(dim=1)
+    y_squared = (b ** 2).sum(dim=1)
+    return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
+
+
+a = torch.rand((10000, 800))
+b = torch.rand((12000, 800))
+batched_euclidean_distance(a, b)
+
+if torch.cuda.is_available():
+    a = a.cuda()
+    b = b.cuda()
+    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
+```
+Prints:
+```
+batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
+batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
+```
+
+
+### Registering a timed decorator
+
+```py
+from time import sleep
+
+from timed_decorator.builder import create_timed_decorator, get_timed_decorator
+
+
+@get_timed_decorator("MyCustomTimer")
+def main():
+    @get_timed_decorator("MyCustomTimer")
+    def function_1():
+        sleep(0.1)
+
+    @get_timed_decorator("MyCustomTimer")
+    def nested_function():
+        @get_timed_decorator("MyCustomTimer")
+        def function_2():
+            sleep(0.2)
+
+        @get_timed_decorator("MyCustomTimer")
+        def function_3():
+            sleep(0.3)
+
+        function_2()
+        function_2()
+        function_3()
+
+    nested_function()
+    function_1()
+    nested_function()
+    function_1()
+
+
+if __name__ == '__main__':
+    my_measurements = {}
+    create_timed_decorator("MyCustomTimer",
+                           collect_gc=False,  # I don't want to explicitly collect garbage
+                           disable_gc=True,  # I don't want to wait for garbage collection during measuring
+                           stdout=False,  # I don't wat to print stuff to console
+                           out=my_measurements  # My measurements dict
+                           )
+    main()
+    for key, value in my_measurements.items():
+        print(f'Function {key} took {value / 1e+9}s')
+    print()
+    print()
+
+    # Now I can do stuff with my measurements.
+    functions = sorted(my_measurements.keys(), reverse=True)
+
+    for i in range(len(functions)):
+        fn_1 = functions[i]
+        print(f'Function {fn_1}:')
+        for j in range(i + 1, len(functions)):
+            fn_2 = functions[j]
+            if fn_1.startswith(fn_2):
+                ratio = my_measurements[fn_1] / my_measurements[fn_2] * 100
+                print(f'* took {ratio:.2f}% from {fn_2}')
+        print()
+```
+
+Prints:
+```
+Function main.<locals>.nested_function.<locals>.function_2 took 0.8016428s
+Function main.<locals>.nested_function.<locals>.function_3 took 0.6014647s
+Function main.<locals>.nested_function took 1.403586s
+Function main.<locals>.function_1 took 0.2006981s
+Function main took 1.6045189s
+
+
+Function main.<locals>.nested_function.<locals>.function_3:
+* took 42.85% from main.<locals>.nested_function
+* took 37.49% from main
+
+Function main.<locals>.nested_function.<locals>.function_2:
+* took 57.11% from main.<locals>.nested_function
+* took 49.96% from main
+
+Function main.<locals>.nested_function:
+* took 87.48% from main
+
+Function main.<locals>.function_1:
+* took 12.51% from main
+
+Function main:
+
+```
```

### Comparing `timed_decorator-1.3.0/pyproject.toml` & `timed_decorator-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timed-decorator"
-version = "1.3.0"
+version = "1.4.0"
 #requires-python = ">=3.10"
 requires-python = ">=3.7"
 description = "A timing decorator for python functions."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "George Stoica", email = "george.stoica@senticlab.com" },
```

### Comparing `timed_decorator-1.3.0/tests/test_usage.py` & `timed_decorator-1.4.0/tests/test_usage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import unittest
 from io import StringIO
 from time import sleep
 
 from tests.functions import fibonacci, recursive_fibonacci
+from timed_decorator.builder import create_timed_decorator, get_timed_decorator
 from timed_decorator.nested_timed import nested_timed
 from timed_decorator.simple_timed import timed
 from timed_decorator.utils import build_decorated_fn
 
 
 class UsageTest(unittest.TestCase):
     @staticmethod
@@ -61,15 +62,15 @@
         nested_fn()
 
     def test_file_usage(self):
         filename = 'file.txt'
 
         @timed(file_path=filename, stdout=False)
         def fn():
-            sleep(0.5)
+            sleep(0.1)
 
         try:
             fn()
             fn()
             with open(filename, 'r') as f:
                 lines = f.readlines()
                 self.assertEqual(len(lines), 2)
@@ -83,43 +84,79 @@
         logger_name = 'TEST_LOGGER'
         log_stream = StringIO()
         log_handler = logging.StreamHandler(log_stream)
         logging.root.setLevel(logging.NOTSET)
         logging.getLogger(logger_name).addHandler(log_handler)
 
         @timed(logger_name=logger_name, stdout=False)
-        def fn():
-            sleep(0.5)
+        def fn_1():
+            sleep(0.1)
 
-        fn()
-        fn()
+        fn_1()
+
+        @timed(logger_name=logger_name, stdout=False, use_qualname=True)
+        def fn_2():
+            sleep(0.1)
+
+        fn_2()
 
         logged = log_stream.getvalue().split('\n')[:-1]
         self.assertEqual(len(logged), 2)
-        self.assertIn(fn.__name__, logged[0])
-        self.assertIn(fn.__name__, logged[1])
+        self.assertIn(fn_1.__name__, logged[0])
+        self.assertNotIn(fn_1.__qualname__, logged[0])
+        self.assertIn(fn_2.__name__, logged[1])
+        self.assertIn(fn_2.__qualname__, logged[1])
 
     def test_ns_output(self):
-        ns = {}
+        out = {}
 
-        @timed(out=ns, stdout=False)
+        @timed(out=out, stdout=False)
         def fn():
-            sleep(0.5)
+            sleep(0.1)
 
         fn()
 
-        self.assertIsInstance(ns[fn.__name__], int)
-        self.assertGreater(ns[fn.__name__], 1**9 / 2)
+        self.assertIsInstance(out[fn.__qualname__], int)
+        self.assertGreater(out[fn.__qualname__], 1e+8)
+
+    def test_qualname(self):
+        out = {}
+
+        class ClassA:
+            @timed(out=out)
+            def wait(self, x):
+                sleep(x)
+
+        ClassA().wait(0.1)
+        key = next(iter(out.keys()))
+        self.assertIn(ClassA.__name__, key)
 
     def test_return_time(self):
+        seconds = 0.1
+
         @timed(return_time=True, stdout=False)
-        def fn():
-            sleep(0.5)
+        def fn(x):
+            sleep(x)
 
-        _, elapsed = fn()
+        _, elapsed = fn(seconds)
 
         self.assertIsInstance(elapsed, int)
-        self.assertGreater(elapsed, 1**9 / 2)
+        self.assertGreater(elapsed / 1e+9, seconds)
+
+    def test_create_timed_decorator(self):
+        create_timed_decorator('same name')
+        self.assertRaises(KeyError, create_timed_decorator, 'same name')
+        create_timed_decorator('other name')
+
+        get_timed_decorator('same name')(fibonacci)(10000)
+        get_timed_decorator('other name')(fibonacci)(10000)
+        fn = get_timed_decorator('no name')(fibonacci)  # Does not raise error if not called
+        self.assertRaises(KeyError, fn, 10000)
+
+        # Defer instantiation
+        fn = get_timed_decorator('lazy name')(fibonacci)
+        create_timed_decorator('lazy name')
+        fn(10000)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timed_decorator-1.3.0/timed_decorator/nested_timed.py` & `timed_decorator-1.4.0/timed_decorator/simple_timed.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,34 +2,31 @@
 from functools import wraps
 from gc import collect
 from time import perf_counter_ns
 from typing import Union
 
 from .utils import nop, TimeFormatter, InputFormatter, synchronize_cuda, Logger, write_mutable
 
-nested_level = 0
-nested_times = dict()
 
-
-def nested_timed(collect_gc: bool = True,
-                 disable_gc: bool = False,
-                 use_seconds: bool = False,
-                 precision: int = 9,
-                 show_args: bool = False,
-                 show_kwargs: bool = False,
-                 display_level: int = 1,
-                 sep: str = ', ',
-                 stdout: bool = True,
-                 file_path: Union[str, None] = None,
-                 logger_name: Union[str, None] = None,
-                 return_time: bool = False,
-                 out: dict = None):
+def timed(collect_gc: bool = True,
+          disable_gc: bool = False,
+          use_seconds: bool = False,
+          precision: int = 9,
+          show_args: bool = False,
+          show_kwargs: bool = False,
+          display_level: int = 1,
+          sep: str = ', ',
+          stdout: bool = True,
+          file_path: Union[str, None] = None,
+          logger_name: Union[str, None] = None,
+          return_time: bool = False,
+          out: dict = None,
+          use_qualname: bool = False):
     """
-    A nested timing decorator that measures the time elapsed during the function call and accounts for other decorators
-    further in the call stack.
+    A simple timing decorator that measures the time elapsed during the function call and prints it.
     It uses perf_counter_ns for measuring which includes time elapsed during sleep and is system-wide.
 
     Args:
         collect_gc (bool): If `True`, runs a full garbage collection before timing the wrapped function. Default:
             `True`.
         disable_gc (bool): If `True`, disabled garbage collection during function execution. Default: `False`.
         use_seconds (bool): If `True`, displays the elapsed time in seconds. Default: `False`.
@@ -45,64 +42,45 @@
         stdout (bool): If `True`, writes the elapsed time to stdout. Default: `True`.
         file_path (str): If not `None`, writes the measurement at the end of the given file path. For thread safe
             file writing configure use `logger_name` instead. Default: `None`.
         logger_name (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction
             with `file_path`. Default: `None`.
         return_time (bool): If `True`, returns the elapsed time in addition to the wrapped function's return value.
             Default: `False`.
-        out (dict): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as
-            key. If the key already exists, adds the time to the existing value. Default: `None`.
+        out (dict): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified
+            function name as key. If the key already exists, adds the time to the existing value. Default: `None`.
+        use_qualname (bool): If `True`, uses the qualified name of the function when logging the elapsed time. Default:
+            `False`.
     """
     gc_collect = collect if collect_gc else nop
     time_formatter = TimeFormatter(use_seconds, precision)
     input_formatter = InputFormatter(show_args, show_kwargs, display_level, sep)
     logger = Logger(stdout, file_path, logger_name)
     ns_out = write_mutable if out is not None else nop
 
     def decorator(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
-            global nested_level, nested_times
-            nested_level += 1
-
             gc_collect()
             if disable_gc:
                 gc.disable()
 
             try:
                 start = perf_counter_ns()
                 ret = fn(*args, **kwargs)
                 synchronize_cuda(*args, **kwargs)
                 end = perf_counter_ns()
-            except Exception as e:
-                nested_level -= 1
-                raise e
             finally:
                 if disable_gc:
                     gc.enable()
 
             elapsed = end - start
-
-            children_time = 0
-            if nested_level in nested_times:
-                children_time = sum(nested_times[nested_level])
-                del nested_times[nested_level]
-
-            own_time = elapsed - children_time
-            nested_level -= 1
-
-            if nested_level != 0:
-                if nested_level not in nested_times:
-                    nested_times[nested_level] = []
-                nested_times[nested_level].append(elapsed)
-
-            ns_out(out, fn.__name__, elapsed)
-            logger('\t' * nested_level + f'{input_formatter(fn.__name__, *args, **kwargs)} '
-                                         f'-> total time: {time_formatter(elapsed)}, '
-                                         f'own time: {time_formatter(own_time)}')
+            fn_name = fn.__qualname__ if use_qualname else fn.__name__
+            ns_out(out, fn.__qualname__, elapsed)
+            logger(f'{input_formatter(fn_name, *args, **kwargs)} -> total time: {time_formatter(elapsed)}')
             if return_time:
                 return ret, elapsed
             return ret
 
         return wrap
 
     return decorator
```

### Comparing `timed_decorator-1.3.0/timed_decorator/utils.py` & `timed_decorator-1.4.0/timed_decorator/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             with open(self.file_path, 'a') as f:
                 f.write(string + '\n')
 
         if self.logger_name is not None:
             logging.getLogger(self.logger_name).info(string)
 
 
-
 class InputFormatter:
     def __init__(self, show_args: bool = False, show_kwargs: bool = False, display_level: int = 1, sep: str = ', '):
         self.show_args = show_args
         self.show_kwargs = show_kwargs
         self.display_level = display_level
         self.sep = sep
```

### Comparing `timed_decorator-1.3.0/timed_decorator.egg-info/PKG-INFO` & `timed_decorator-1.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.3.0
+Version: 1.4.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -37,54 +37,48 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 
 # timed-decorator
 
+Simple and configurable timing decorator with little overhead that can be easily attached to python functions to measure their execution time.
+Can easily display parameter types and lengths if available and is compatible with NumPy ndarrays, Pandas DataFrames and PyTorch tensors.
+
+
 ## Installation
 
 ```
 pip install --upgrade timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
-```py
-import torch
-from torch import Tensor
 
+```py
 from timed_decorator.simple_timed import timed
 
 
-@timed(show_args=True)
-def batched_euclidean_distance(x: Tensor, y: Tensor) -> Tensor:
-    diff = x @ y.T
-    x_squared = (x ** 2).sum(dim=1)
-    y_squared = (b ** 2).sum(dim=1)
-    return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
-
+@timed()
+def fibonacci(n: int) -> int:
+    assert n > 0
+    a, b = 0, 1
+    for _ in range(n):
+        a, b = b, a + b
+    return a
 
-a = torch.rand((10000, 800))
-b = torch.rand((12000, 800))
-batched_euclidean_distance(a, b)
 
-if torch.cuda.is_available():
-    a = a.cuda()
-    b = b.cuda()
-    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
-```
-Prints:
-```
-batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
-batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
+fibonacci(10000)
+# fibonacci() -> total time: 1114100ns
 ```
 
+For more advanced usage, consider registering a timed decorator and using it afterward through your codebase. See [Registering a timed decorator](#registering-a-timed-decorator).
+
 ### Documentation
 
 1. `timed`
     * `collect_gc` (`bool`): If `True`, runs a full garbage collection before timing the wrapped function. Default: `True`.
     * `disable_gc` (`bool`): If `True`, disabled garbage collection during function execution. Default: `False`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
@@ -92,18 +86,28 @@
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
     * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
     * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key.  If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
+3. `create_timed_decorator` registers a timed decorator with a given name.
+   * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
+   * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
+   * Also receives all the other arguments accepted by `timed` and `nested_timed`.
+
+4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call.
+   * `name` (`str`): The name of the timed decorator registered using `timed_decorator.builder.create_timed_decorator`.
+
+
 ### Examples
 
 Simple usage.
 ```py
 from timed_decorator.simple_timed import timed
 
 
@@ -319,14 +323,27 @@
     np.random.rand(1, 3),
     weights=[i / 10 for i in range(1)],
     inplace=True
 )
 # numpy_operation([array([[0.74500602, 0.70666224, 0.83888559]])], [[0.74579988 0.51878032 0.06419635]], ('weights', '[0.0]'), ('inplace', 'True')) -> total time: 185300ns
 ```
 
+Using the fully qualified name for timing. 
+
+```py
+from time import sleep
+from timed_decorator.simple_timed import timed
+class ClassA:
+    @timed(use_qualname=True)
+    def wait(self, x):
+        sleep(x)
+ClassA().wait(0.1)
+# ClassA.wait() -> total time: 100943000ns
+```
+
 ### Nested timing decorator
 
 ```py
 from time import sleep
 
 from timed_decorator.nested_timed import nested_timed
 
@@ -433,7 +450,131 @@
 print(ns)
 ```
 Prints
 ```
 {'fn': 1000767300}
 {'fn': 2001006100}
 ```
+
+### Compatible with PyTorch tensors
+
+Synchronizes cuda device when cuda tensors are passed as function parameters.
+
+```py
+import torch
+from torch import Tensor
+
+from timed_decorator.simple_timed import timed
+
+
+@timed(show_args=True)
+def batched_euclidean_distance(x: Tensor, y: Tensor) -> Tensor:
+    diff = x @ y.T
+    x_squared = (x ** 2).sum(dim=1)
+    y_squared = (b ** 2).sum(dim=1)
+    return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
+
+
+a = torch.rand((10000, 800))
+b = torch.rand((12000, 800))
+batched_euclidean_distance(a, b)
+
+if torch.cuda.is_available():
+    a = a.cuda()
+    b = b.cuda()
+    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
+```
+Prints:
+```
+batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
+batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
+```
+
+
+### Registering a timed decorator
+
+```py
+from time import sleep
+
+from timed_decorator.builder import create_timed_decorator, get_timed_decorator
+
+
+@get_timed_decorator("MyCustomTimer")
+def main():
+    @get_timed_decorator("MyCustomTimer")
+    def function_1():
+        sleep(0.1)
+
+    @get_timed_decorator("MyCustomTimer")
+    def nested_function():
+        @get_timed_decorator("MyCustomTimer")
+        def function_2():
+            sleep(0.2)
+
+        @get_timed_decorator("MyCustomTimer")
+        def function_3():
+            sleep(0.3)
+
+        function_2()
+        function_2()
+        function_3()
+
+    nested_function()
+    function_1()
+    nested_function()
+    function_1()
+
+
+if __name__ == '__main__':
+    my_measurements = {}
+    create_timed_decorator("MyCustomTimer",
+                           collect_gc=False,  # I don't want to explicitly collect garbage
+                           disable_gc=True,  # I don't want to wait for garbage collection during measuring
+                           stdout=False,  # I don't wat to print stuff to console
+                           out=my_measurements  # My measurements dict
+                           )
+    main()
+    for key, value in my_measurements.items():
+        print(f'Function {key} took {value / 1e+9}s')
+    print()
+    print()
+
+    # Now I can do stuff with my measurements.
+    functions = sorted(my_measurements.keys(), reverse=True)
+
+    for i in range(len(functions)):
+        fn_1 = functions[i]
+        print(f'Function {fn_1}:')
+        for j in range(i + 1, len(functions)):
+            fn_2 = functions[j]
+            if fn_1.startswith(fn_2):
+                ratio = my_measurements[fn_1] / my_measurements[fn_2] * 100
+                print(f'* took {ratio:.2f}% from {fn_2}')
+        print()
+```
+
+Prints:
+```
+Function main.<locals>.nested_function.<locals>.function_2 took 0.8016428s
+Function main.<locals>.nested_function.<locals>.function_3 took 0.6014647s
+Function main.<locals>.nested_function took 1.403586s
+Function main.<locals>.function_1 took 0.2006981s
+Function main took 1.6045189s
+
+
+Function main.<locals>.nested_function.<locals>.function_3:
+* took 42.85% from main.<locals>.nested_function
+* took 37.49% from main
+
+Function main.<locals>.nested_function.<locals>.function_2:
+* took 57.11% from main.<locals>.nested_function
+* took 49.96% from main
+
+Function main.<locals>.nested_function:
+* took 87.48% from main
+
+Function main.<locals>.function_1:
+* took 12.51% from main
+
+Function main:
+
+```
```

