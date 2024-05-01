# Comparing `tmp/aptly_ctl-1.0.0rc0.tar.gz` & `tmp/aptly_ctl-1.0.0rc1.tar.gz`

## Comparing `aptly_ctl-1.0.0rc0.tar` & `aptly_ctl-1.0.0rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/__main__.py
--rw-r--r--   0        0        0    37562 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/aptly.py
--rw-r--r--   0        0        0    58087 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/cmd.py
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/config.py
--rw-r--r--   0        0        0     9337 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/debian.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/exceptions.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/aptly_ctl/util.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/README.md
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/__main__.py
+-rw-r--r--   0        0        0    37562 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/aptly.py
+-rw-r--r--   0        0        0    58087 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/cmd.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/config.py
+-rw-r--r--   0        0        0     9337 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/debian.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/exceptions.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/aptly_ctl/util.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 aptly_ctl-1.0.0rc1/PKG-INFO
```

### Comparing `aptly_ctl-1.0.0rc0/aptly_ctl/aptly.py` & `aptly_ctl-1.0.0rc1/aptly_ctl/aptly.py`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/aptly_ctl/cmd.py` & `aptly_ctl-1.0.0rc1/aptly_ctl/cmd.py`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/aptly_ctl/config.py` & `aptly_ctl-1.0.0rc1/aptly_ctl/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 )
 
 
 class Config:
     url: str = "http://localhost:8090/"
     default_signing_config: SigningConfig = DefaultSigningConfig
     signing_config_map: Optional[Dict[str, SigningConfig]] = None
-    connect_timeout: Optional[float] = 15.0
-    read_timeout: Optional[float] = None
+    connect_timeout: Optional[float] = 60.0 * 60
+    read_timeout: Optional[float] = 60.0 * 30
 
     def __init__(
         self, path: str = None, section: str = "", override: Dict[str, Any] = None
     ) -> None:
         config = {}
         if path:
             with open(path, "r") as file:
```

### Comparing `aptly_ctl-1.0.0rc0/aptly_ctl/debian.py` & `aptly_ctl-1.0.0rc1/aptly_ctl/debian.py`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/aptly_ctl/exceptions.py` & `aptly_ctl-1.0.0rc1/aptly_ctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/aptly_ctl/util.py` & `aptly_ctl-1.0.0rc1/aptly_ctl/util.py`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/LICENSE` & `aptly_ctl-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/README.md` & `aptly_ctl-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/pyproject.toml` & `aptly_ctl-1.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aptly_ctl-1.0.0rc0/PKG-INFO` & `aptly_ctl-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aptly-ctl
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: Convenient command line Aptly API client
 Project-URL: Homepage, https://github.com/cyril-s/aptly-ctl
 Project-URL: Repository, https://github.com/cyril-s/aptly-ctl.git
 Project-URL: Issues, https://github.com/cyril-s/aptly-ctl/issues
 Author-email: Kyrylo Shestakov <freyr.sh@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

