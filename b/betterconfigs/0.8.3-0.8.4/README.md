# Comparing `tmp/betterconfigs-0.8.3.tar.gz` & `tmp/betterconfigs-0.8.4.tar.gz`

## Comparing `betterconfigs-0.8.3.tar` & `betterconfigs-0.8.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/buildscript.sh
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/test_conf.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/src/betterconfigs/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/src/betterconfigs/utilities.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/LICENSE
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/PKG-INFO
+-rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/buildscript.sh
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/test_conf.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/src/betterconfigs/__init__.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/src/betterconfigs/utilities.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 betterconfigs-0.8.4/PKG-INFO
```

### Comparing `betterconfigs-0.8.3/test_conf.py` & `betterconfigs-0.8.4/test_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,19 +72,23 @@
     assert(h.checkEncryptionValidity()==0)
     os.remove('test.config')
 def test_encdec():
     h = config('test.config')
     h['hello']='world'
     assert(h.encryptFile()==0)
     h['hello2']='world2'
+    h['1']=3
+    h['2']=True
     encryptionKey = h.encKey
     t = config('test.config')
     t.encKey = encryptionKey
     assert(t['hello']=='world')
     assert(t['hello2']=='world2')
+    assert(t['1']==3)
+    assert(t['2']==True)
     assert(t.decryptFile()==0)
     os.remove('test.config')
 def test_encdec_int():
     h = config('test.config')
     h['hello']='world'
     assert(h.encryptFile()==0)
     h['hello2']=3
```

### Comparing `betterconfigs-0.8.3/.github/workflows/python-publish.yml` & `betterconfigs-0.8.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8.3/src/betterconfigs/__init__.py` & `betterconfigs-0.8.4/src/betterconfigs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import os
 import warnings
 from cryptography.fernet import Fernet
-executableVersion = "0.8.3"
+executableVersion = "0.8.4"
 supportedTypes=[int, str, list, bool]
 class config:
     def __init__(self, path) -> None:
         self.path = path
         self.encKey = None
         if os.path.exists(path)==False:
             try:
@@ -82,15 +82,15 @@
             return 0
         else:
             return 1
     def encryptValue(self, value):
         self.checkReady()
         fernet = Fernet(self.encKey)
         if type(value) not in supportedTypes:
-            raise Exception("type "+ type(value)+ " is not supported for encryption")
+            raise Exception("type "+ str(type(value))+ " is not supported for encryption")
         if 'bool.e' in str(value) or 'int.e' in str(value):
             raise Exception("value contains encoding information before encoding occurred")
         if type(value) is int:
             return fernet.encrypt(("int.e"+str(value)).encode())
         elif type(value) is bool:
             return fernet.encrypt(("bool.e"+str(value)).encode())
         elif type(value) is list:
```

### Comparing `betterconfigs-0.8.3/LICENSE` & `betterconfigs-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8.3/README.md` & `betterconfigs-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8.3/pyproject.toml` & `betterconfigs-0.8.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "betterconfigs"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="Iain Rosen", email="hello@iainrosen.me" },
 ]
 description = "A small package to simplify configuration storing and retrieving"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `betterconfigs-0.8.3/PKG-INFO` & `betterconfigs-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: betterconfigs
-Version: 0.8.3
+Version: 0.8.4
 Summary: A small package to simplify configuration storing and retrieving
 Project-URL: Homepage, https://github.com/iainrosen/betterconfigs
 Project-URL: Bug Tracker, https://github.com/iainrosen/betterconfigs/issues
 Author-email: Iain Rosen <hello@iainrosen.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

