# Comparing `tmp/yaconfiglib-0.3.2.tar.gz` & `tmp/yaconfiglib-0.3.5.tar.gz`

## Comparing `yaconfiglib-0.3.2.tar` & `yaconfiglib-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/examples/config.toml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/examples/hiera.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/examples/includeme.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/examples/jinja.yaml.j2
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/example.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/__init__.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/loader.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/backends/__init__.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/backends/base.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/backends/jinja2.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/backends/toml.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/backends/yaml.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/utils/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/utils/enum.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/utils/jinja2.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/utils/log.py
--rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/utils/merge.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/src/yaconfiglib/utils/source.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/LICENSE
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/README.md
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 yaconfiglib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/examples/config.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/examples/hiera.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/examples/includeme.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/examples/jinja.yaml.j2
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/examples/settings.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/examples/test.ini
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/example.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/__init__.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/loader.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/base.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/ini.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/jinja2.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/json.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/toml.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/backends/yaml.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/utils/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/utils/enum.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/utils/jinja2.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/utils/log.py
+-rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/utils/merge.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/src/yaconfiglib/utils/source.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/README.md
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 yaconfiglib-0.3.5/PKG-INFO
```

### Comparing `yaconfiglib-0.3.2/src/example.py` & `yaconfiglib-0.3.5/src/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 configloader = ConfigLoader()
 yaml.SafeLoader.add_constructor("!load", configloader)
 
 hieraconf = configloader.load(
     """#!test.yaml
 pathname:
   stem: root
+vscode_settings: !load examples/settings.json
+iniconfig: !load examples/test.ini
 """,
     "examples/hiera.yaml",
     interpolate=True,
     merge=MergeMethod.Deep,
 )
 print(yaml.dump(hieraconf, indent=2))
```

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/loader.py` & `yaconfiglib-0.3.5/src/yaconfiglib/loader.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/backends/base.py` & `yaconfiglib-0.3.5/src/yaconfiglib/backends/base.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/backends/jinja2.py` & `yaconfiglib-0.3.5/src/yaconfiglib/backends/jinja2.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/backends/yaml.py` & `yaconfiglib-0.3.5/src/yaconfiglib/backends/yaml.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/utils/enum.py` & `yaconfiglib-0.3.5/src/yaconfiglib/utils/enum.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/utils/jinja2.py` & `yaconfiglib-0.3.5/src/yaconfiglib/utils/jinja2.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/utils/log.py` & `yaconfiglib-0.3.5/src/yaconfiglib/utils/log.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/utils/merge.py` & `yaconfiglib-0.3.5/src/yaconfiglib/utils/merge.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/src/yaconfiglib/utils/source.py` & `yaconfiglib-0.3.5/src/yaconfiglib/utils/source.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/LICENSE` & `yaconfiglib-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/README.md` & `yaconfiglib-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.2/pyproject.toml` & `yaconfiglib-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yaconfiglib"
-version = "0.3.2"
+version = "0.3.5"
 authors = [{ name = "Jose A" }]
 description = "Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yaconfiglib-0.3.2/PKG-INFO` & `yaconfiglib-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yaconfiglib
-Version: 0.3.2
+Version: 0.3.5
 Summary: Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating.
 Project-URL: Homepage, https://github.com/jose-pr/yaconfiglib/
 Project-URL: Issues, https://github.com/jose-pr/yaconfiglib/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

