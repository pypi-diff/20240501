# Comparing `tmp/cupcake-1.0.0.tar.gz` & `tmp/cupcake-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-1.0.0.tar", max compression
+gzip compressed data, was "cupcake-1.0.1.tar", max compression
```

## Comparing `cupcake-1.0.0.tar` & `cupcake-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.0/LICENSE
--rw-r--r--   0        0        0      576 2024-04-26 23:12:40.394996 cupcake-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.0/src/cupcake/__init__.py
--rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.0/src/cupcake/cascade.py
--rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-1.0.0/src/cupcake/confee.py
--rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.0/src/cupcake/data/cmake_names.py
--rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.0/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0     1031 2024-04-26 22:06:39.942764 cupcake-1.0.0/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     2409 2024-04-26 22:06:34.282479 cupcake-1.0.0/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.0/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.0/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.0/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.0/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.0/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.0/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.0/src/cupcake/expression.py
--rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.0/src/cupcake/functional.py
--rw-r--r--   0        0        0    52971 2024-04-26 22:32:20.677109 cupcake-1.0.0/src/cupcake/main.py
--rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.0/src/cupcake/transformations.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 cupcake-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.1/LICENSE
+-rw-r--r--   0        0        0      576 2024-05-01 00:22:02.738062 cupcake-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.1/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.1/src/cupcake/cascade.py
+-rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-1.0.1/src/cupcake/confee.py
+-rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.1/src/cupcake/data/cmake_names.py
+-rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.1/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0     1031 2024-04-30 21:17:59.470632 cupcake-1.0.1/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     2477 2024-04-29 20:21:28.383431 cupcake-1.0.1/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.1/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.1/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.1/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.1/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.1/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.1/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.1/src/cupcake/expression.py
+-rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.1/src/cupcake/functional.py
+-rw-r--r--   0        0        0    53272 2024-05-01 00:10:40.111456 cupcake-1.0.1/src/cupcake/main.py
+-rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.1/src/cupcake/transformations.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 cupcake-1.0.1/PKG-INFO
```

### Comparing `cupcake-1.0.0/LICENSE` & `cupcake-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.0/pyproject.toml` & `cupcake-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupcake"
-version = "1.0.0"
+version = "1.0.1"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
```

### Comparing `cupcake-1.0.0/src/cupcake/cascade.py` & `cupcake-1.0.1/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.0/src/cupcake/confee.py` & `cupcake-1.0.1/src/cupcake/confee.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.0/src/cupcake/data/cmake_names.py` & `cupcake-1.0.1/src/cupcake/data/cmake_names.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.0/src/cupcake/data/new/CMakeLists.txt` & `cupcake-1.0.1/src/cupcake/data/new/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.16)
+cmake_minimum_required(VERSION 3.21)
 
 project({{ name }}
   VERSION 0.1.0
   {% if github %}
   HOMEPAGE_URL https://github.com/{{ github }}/{{ name }}
   {% endif %}
   LANGUAGES CXX
```

### Comparing `cupcake-1.0.0/src/cupcake/data/new/conanfile.py` & `cupcake-1.0.1/src/cupcake/data/new/conanfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import conan
+from conan import ConanFile, conan_version
 from conan.tools.cmake import CMake, cmake_layout
 
-class {{ name | pascal }}(conan.ConanFile):
+class {{ name | pascal }}(ConanFile):
     name = '{{ name }}'
     version = '0.1.0'
     {% if github %}
     user = 'github'
     channel = '{{ github }}'
     {% endif %}
 
@@ -18,14 +18,15 @@
     {% endif %}
 
     settings = 'os', 'compiler', 'build_type', 'arch'
     options = {'shared': [True, False], 'fPIC': [True, False]}
     default_options = {'shared': False, 'fPIC': True}
 
     requires = [
+        # Available at https://conan.jfreeman.dev
         'cupcake.cmake/{{ version }}@github/thejohnfreeman',
         {% if with_tests and not special %}
         'doctest/2.4.8',
         {% endif %}
     ]
     generators = ['CMakeDeps', 'CMakeToolchain']
 
@@ -53,15 +54,15 @@
         import pathlib
         path = pathlib.Path(self.recipe_folder) / 'cupcake.json'
         with path.open('r') as file:
             metadata = json.load(file)
         methods = {
             'tool': 'tool_requires',
             'test': 'test_requires',
-        } if conan.conan_version.major.value == 2 else {}
+        } if conan_version.major.value == 2 else {}
         for requirement in metadata.get('imports', []):
             groups = requirement.get('groups', [])
             group = groups[0] if len(groups) == 1 else 'main'
             method = methods.get(group, 'requires')
             getattr(self, method)(requirement['reference'])
 
     {% endif %}
```

### Comparing `cupcake-1.0.0/src/cupcake/expression.py` & `cupcake-1.0.1/src/cupcake/expression.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.0/src/cupcake/main.py` & `cupcake-1.0.1/src/cupcake/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import functools
 import hashlib
 from importlib import resources
 import io
 import itertools
 import jinja2
 import json
+import locale
 import operator
 import os
 import pathlib
 import re
 import shlex
 import shutil
 import subprocess
@@ -110,14 +111,17 @@
             value = f(*args, **kwargs)
             print(value)
             return value
         return decorated
     return decorate
 
 def compare_version(a, b):
+    """
+    Returns <0, 0, or >0.
+    """
     # Not all Conan packages use Semantic Versioning.
     # To be as flexible as possible,
     # we treat version strings as non-digit-separated sequences of numbers.
     # Sequences are compared item-by-item, in order.
     # Numbers are compared numerically,
     # non-numbers are compared lexicographically.
     # Numbers are considered higher/later/younger versions than non-numbers.
@@ -206,25 +210,30 @@
     if reference.startswith('test.'):
         return ('tests', reference[len('test.'):])
     return ('executables', reference)
 
 class SearchResult:
     """Representation for a Conan package search result."""
 
-    key = functools.cmp_to_key(
-        lambda a, b: compare_version(a.version, b.version)
-    )
+    key = functools.cmp_to_key(lambda a, b: a.__cmp__(b))
 
     def __init__(self, remote, reference):
         self.remote = remote
         match = re.match(f'^([^/]+)/([^@]+)(?:@(.*))?$', reference)
         self.package = match[1]
         self.version = match[2]
         self.remainder = match[3]
 
+    def __cmp__(self, rhs):
+        # Note reversed order for package name.
+        diff = locale.strcoll(rhs.package, self.package)
+        if diff != 0:
+            return diff
+        return compare_version(self.version, rhs.version)
+
     def __str__(self):
         s = f'{self.package}/{self.version}@'
         if self.remainder:
             s += self.remainder
         return s
 
 class Conan:
@@ -417,15 +426,15 @@
             If relative, must be relative to build_dir.
         """
         variables = dict(variables)
         args = [f'-D{name}={value}' for name, value in variables.items()]
         if generator is not None:
             args = ['-G', generator, *args]
         args = [*args, source_dir]
-        env = { **os.environ, **env }
+        env = os.environ | env
         run([self.CMAKE, *args], cwd=build_dir, env=env)
 
 TEST_TEMPLATE_ = """
 '{{ ctest }}' --test-dir '{{ cmakeDir }}'
 {% if multiConfig %} --build-config {{ flavor }} {% endif %}
 {% if regex %} --tests-regex {{ regex }} {% endif %}
 """
@@ -790,15 +799,15 @@
         else:
             cmake_args['CMAKE_BUILD_TYPE'] = FLAVORS[flavor_]
         # Add these last to let callers override anything.
         for name, value in cvars.items():
             cmake_args[name] = value
         CMake(CMAKE).configure(
             cmake_dir, source_dir_, generator, cmake_args,
-            env={'CMAKE_OUTPUT_DIR': build_dir_ / 'output'},
+            env={'CMAKE_OUTPUT_DIR': str(build_dir_ / 'output')},
         )
 
         state_.cmake.id = id
         state_.cmake.generator = generator
         state_.cmake.multiConfig = multiConfig
         state_.cmake.flavors = sflavors
         confee.write(config_)
@@ -837,20 +846,21 @@
     @cascade.argument('executable', required=False)
     # TODO: No way to pass arguments to default executable.
     @cascade.argument('arguments', nargs=-1)
     def exe(self, CMAKE, cmake_dir_, flavor_, cmake, executable, arguments):
         """Execute an executable target."""
         target = 'execute'
         if executable is not None:
-            target += '-' + executable
+            target += '.' + executable
         command = [CMAKE, '--build', cmake_dir_, '--target', target]
         if cmake.multiConfig():
             command.extend(['--config', FLAVORS[flavor_]])
         env = os.environ.copy()
-        env['CUPCAKE_EXE_ARGUMENTS'] = ' '.join(map(shlex.quote, arguments))
+        escape = lambda arg: arg.replace(';', '\\;')
+        env['CUPCAKE_EXE_ARGUMENTS'] = ';'.join(map(escape, arguments))
         run(command, env=env)
 
     @cascade.command()
     def install(self, CMAKE, cmake_dir_, flavor_, build, prefix_):
         """Install the selected flavor."""
         run([
             CMAKE,
```

### Comparing `cupcake-1.0.0/src/cupcake/transformations.py` & `cupcake-1.0.1/src/cupcake/transformations.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.0/PKG-INFO` & `cupcake-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

