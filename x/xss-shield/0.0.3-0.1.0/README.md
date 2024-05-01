# Comparing `tmp/xss_shield-0.0.3.tar.gz` & `tmp/xss_shield-0.1.0.tar.gz`

## Comparing `xss_shield-0.0.3.tar` & `xss_shield-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 xss_shield-0.0.3/src/xss_shield/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 xss_shield-0.0.3/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 xss_shield-0.0.3/LICENSE
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 xss_shield-0.0.3/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 xss_shield-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 xss_shield-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 xss_shield-0.1.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 xss_shield-0.1.0/examples/example.ipynb
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 xss_shield-0.1.0/src/xss_shield/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 xss_shield-0.1.0/test/test_escape.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 xss_shield-0.1.0/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 xss_shield-0.1.0/LICENSE
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 xss_shield-0.1.0/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 xss_shield-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 xss_shield-0.1.0/PKG-INFO
```

### Comparing `xss_shield-0.0.3/.gitignore` & `xss_shield-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xss_shield-0.0.3/LICENSE` & `xss_shield-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xss_shield-0.0.3/pyproject.toml` & `xss_shield-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xss-shield"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Gordon Zhang", email="jp20171211@163.com" },
 ]
 description = "A library used to stop your website from being attacked."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xss_shield-0.0.3/PKG-INFO` & `xss_shield-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.3
 Name: xss-shield
-Version: 0.0.3
+Version: 0.1.0
 Summary: A library used to stop your website from being attacked.
 Project-URL: Homepage, https://github.com/GordonZhang2024/xss-shield/
 Project-URL: Issues, https://github.com/GordonZhang2024/xss-shield/issues
 Author-email: Gordon Zhang <jp20171211@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # xss-shield
-**xss-shield** is a python library which is used to stop your website from being attacked.
+A Python library to prevent your website from being attacked
 
 ## Installing
 Type command:
 ```bash
 $ pip install xss-shield
 ```
 
 ## Usage
 example:
 ```python
 import xss_shield
 unsafe_str = '<script>alert("Bad.");</script>'
 safe_str = xss_shield.escape(unsafe_str)
-```
+```
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.3 Name: xss-shield Version: 0.0.3 Summary: A library used
+Metadata-Version: 2.3 Name: xss-shield Version: 0.1.0 Summary: A library used
 to stop your website from being attacked. Project-URL: Homepage, https://
 github.com/GordonZhang2024/xss-shield/ Project-URL: Issues, https://github.com/
 GordonZhang2024/xss-shield/issues Author-email: Gordon Zhang
 163.com> License-File: LICENSE Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v2 or later (LGPLv2+) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8 Description-Content-Type: text/markdown # xss-shield
-**xss-shield** is a python library which is used to stop your website from
-being attacked. ## Installing Type command: ```bash $ pip install xss-shield
-``` ## Usage example: ```python import xss_shield unsafe_str = '
+Requires-Python: >=3.8 Description-Content-Type: text/markdown # xss-shield A
+Python library to prevent your website from being attacked ## Installing Type
+command: ```bash $ pip install xss-shield ``` ## Usage example: ```python
+import xss_shield unsafe_str = '
 ' safe_str = xss_shield.escape(unsafe_str) ```
```

