# Comparing `tmp/kframe-0.4.2.tar.gz` & `tmp/kframe-0.4.2rc1.tar.gz`

## Comparing `kframe-0.4.2.tar` & `kframe-0.4.2rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.2/.tool-versions
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 kframe-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kframe-0.4.2/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.4.2/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.4.2/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kframe-0.4.2/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.2/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.2/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.2/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.2/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.2/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.2/.gitignore
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.4.2/README.md
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 kframe-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 kframe-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.tool-versions
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/LICENSE.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/README.md
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/PKG-INFO
```

### Comparing `kframe-0.4.2/CHANGELOG.md` & `kframe-0.4.2rc1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-## v0.4.2rc1 (2024-05-01)
-
 ## v0.4.2a1 (2024-05-01)
 
 ### Fix
 
 - Update README.md: Remove empty lines
 
 ## v0.4.1 (2024-05-01)
```

### Comparing `kframe-0.4.2/.github/workflows/main_ci.yml` & `kframe-0.4.2rc1/.github/workflows/main_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/.github/workflows/main_pre_release.yml` & `kframe-0.4.2rc1/.github/workflows/main_pre_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/.github/workflows/main_release.yml` & `kframe-0.4.2rc1/.github/workflows/main_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/src/kframe/config/configattr.py` & `kframe-0.4.2rc1/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/src/kframe/config/configentity.py` & `kframe-0.4.2rc1/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/tests/test_secretattr.py` & `kframe-0.4.2rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/LICENSE.txt` & `kframe-0.4.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/README.md` & `kframe-0.4.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2/pyproject.toml` & `kframe-0.4.2rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.4.2"
+version = "0.4.2rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
```

### Comparing `kframe-0.4.2/PKG-INFO` & `kframe-0.4.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.4.2
+Version: 0.4.2rc1
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
```
