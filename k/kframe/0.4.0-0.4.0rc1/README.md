# Comparing `tmp/kframe-0.4.0.tar.gz` & `tmp/kframe-0.4.0rc1.tar.gz`

## Comparing `kframe-0.4.0.tar` & `kframe-0.4.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.0/.tool-versions
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 kframe-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 kframe-0.4.0/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 kframe-0.4.0/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 kframe-0.4.0/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kframe-0.4.0/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.0/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.0/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.0/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.0/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.0/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.0/.gitignore
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.4.0/README.md
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 kframe-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 kframe-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.tool-versions
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/PKG-INFO
```

### Comparing `kframe-0.4.0/CHANGELOG.md` & `kframe-0.4.0rc1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-## v0.4.0rc1 (2024-05-01)
-
 ## v0.4.0a1 (2024-05-01)
 
 ### Fix
 
 - Update license format
 
 ## v0.3.0 (2024-05-01)
```

### Comparing `kframe-0.4.0/.github/workflows/main_ci.yml` & `kframe-0.4.0rc1/.github/workflows/main_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/.github/workflows/main_pre_release.yml` & `kframe-0.4.0rc1/.github/workflows/main_pre_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/.github/workflows/main_release.yml` & `kframe-0.4.0rc1/.github/workflows/main_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/src/kframe/config/configattr.py` & `kframe-0.4.0rc1/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/src/kframe/config/configentity.py` & `kframe-0.4.0rc1/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/tests/test_secretattr.py` & `kframe-0.4.0rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/LICENSE.txt` & `kframe-0.4.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/README.md` & `kframe-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0/pyproject.toml` & `kframe-0.4.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.4.0"
+version = "0.4.0rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
```

### Comparing `kframe-0.4.0/PKG-INFO` & `kframe-0.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.4.0
+Version: 0.4.0rc1
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
```

