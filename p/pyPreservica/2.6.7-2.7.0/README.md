# Comparing `tmp/pyPreservica-2.6.7.tar.gz` & `tmp/pyPreservica-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-2.6.7.tar", last modified: Mon Mar 11 09:18:15 2024, max compression
+gzip compressed data, was "pyPreservica-2.7.0.tar", last modified: Wed May  1 18:37:34 2024, max compression
```

## Comparing `pyPreservica-2.6.7.tar` & `pyPreservica-2.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 09:18:15.260880 pyPreservica-2.6.7/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.6.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2559 2024-03-11 09:18:15.255896 pyPreservica-2.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.6.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 09:18:15.187077 pyPreservica-2.6.7/pyPreservica/
--rw-rw-rw-   0        0        0     1085 2024-03-11 09:17:50.000000 pyPreservica-2.6.7/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37781 2024-02-29 10:55:23.000000 pyPreservica-2.6.7/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0     9172 2023-09-11 08:14:21.000000 pyPreservica-2.6.7/pyPreservica/authorityAPI.py
--rw-rw-rw-   0        0        0    36463 2024-02-29 10:15:57.000000 pyPreservica-2.6.7/pyPreservica/common.py
--rw-rw-rw-   0        0        0    17245 2024-02-02 12:43:39.000000 pyPreservica-2.6.7/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   114526 2024-03-11 09:09:33.000000 pyPreservica-2.6.7/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6269 2024-02-29 10:52:08.000000 pyPreservica-2.6.7/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.6.7/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10771 2023-08-08 08:52:10.000000 pyPreservica-2.6.7/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23612 2024-02-19 11:08:10.000000 pyPreservica-2.6.7/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    93553 2024-01-22 11:56:37.000000 pyPreservica-2.6.7/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     6790 2024-01-11 09:43:25.000000 pyPreservica-2.6.7/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17323 2024-02-29 10:45:43.000000 pyPreservica-2.6.7/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2024-03-11 09:18:15.246919 pyPreservica-2.6.7/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2559 2024-03-11 09:18:14.000000 pyPreservica-2.6.7/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2024-03-11 09:18:14.000000 pyPreservica-2.6.7/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 09:18:14.000000 pyPreservica-2.6.7/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-03-11 09:18:14.000000 pyPreservica-2.6.7/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-11 09:18:14.000000 pyPreservica-2.6.7/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-11 09:18:15.262875 pyPreservica-2.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1666 2024-03-11 09:17:50.000000 pyPreservica-2.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:37:34.663979 pyPreservica-2.7.0/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2559 2024-05-01 18:37:34.661985 pyPreservica-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 18:37:34.590177 pyPreservica-2.7.0/pyPreservica/
+-rw-rw-rw-   0        0        0     1085 2024-05-01 18:37:09.000000 pyPreservica-2.7.0/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37781 2024-02-29 10:55:23.000000 pyPreservica-2.7.0/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0     9172 2023-09-11 08:14:21.000000 pyPreservica-2.7.0/pyPreservica/authorityAPI.py
+-rw-rw-rw-   0        0        0    36518 2024-03-22 11:25:44.000000 pyPreservica-2.7.0/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    17245 2024-02-02 12:43:39.000000 pyPreservica-2.7.0/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   114636 2024-05-01 18:34:48.000000 pyPreservica-2.7.0/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6269 2024-02-29 10:52:08.000000 pyPreservica-2.7.0/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.7.0/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10771 2023-08-08 08:52:10.000000 pyPreservica-2.7.0/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2024-02-19 11:08:10.000000 pyPreservica-2.7.0/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    93553 2024-01-22 11:56:37.000000 pyPreservica-2.7.0/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     6790 2024-01-11 09:43:25.000000 pyPreservica-2.7.0/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17323 2024-02-29 10:45:43.000000 pyPreservica-2.7.0/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:37:34.650016 pyPreservica-2.7.0/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2559 2024-05-01 18:37:33.000000 pyPreservica-2.7.0/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2024-05-01 18:37:33.000000 pyPreservica-2.7.0/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 18:37:33.000000 pyPreservica-2.7.0/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-01 18:37:33.000000 pyPreservica-2.7.0/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 18:37:33.000000 pyPreservica-2.7.0/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 18:37:34.664976 pyPreservica-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1666 2024-05-01 18:37:09.000000 pyPreservica-2.7.0/setup.py
```

### Comparing `pyPreservica-2.6.7/LICENSE.txt` & `pyPreservica-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/PKG-INFO` & `pyPreservica-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.6.7
+Version: 2.7.0
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.6.7/README.md` & `pyPreservica-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/__init__.py` & `pyPreservica-2.7.0/pyPreservica/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 from .authorityAPI import AuthorityAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "2.6.7"
+__version__ = "2.7.0"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-2.6.7/pyPreservica/adminAPI.py` & `pyPreservica-2.7.0/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/authorityAPI.py` & `pyPreservica-2.7.0/pyPreservica/authorityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/common.py` & `pyPreservica-2.7.0/pyPreservica/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import threading
 import time
 import unicodedata
 import xml.etree.ElementTree
 from enum import Enum
 from pathlib import Path
 import pyotp
+from requests import Response, Session
 from urllib3.util import Retry
 import requests
 from requests.adapters import HTTPAdapter
 
 import pyPreservica
 
 logger = logging.getLogger(__name__)
@@ -856,24 +857,24 @@
                 raise RuntimeError(response.status_code, msg)
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
                  use_shared_secret: bool = False, two_fa_secret_key: str = None, protocol: str = "https"):
 
         config = configparser.ConfigParser(interpolation=configparser.Interpolation())
         config.read('credentials.properties', encoding='utf-8')
-        self.session = requests.Session()
+        self.session: Session = requests.Session()
 
         retries = Retry(
             total=3,
             backoff_factor=0.1,
             status_forcelist=[502, 503, 504],
             allowed_methods=Retry.DEFAULT_ALLOWED_METHODS
         )
 
-        self.shared_secret = bool(use_shared_secret)
+        self.shared_secret: bool = bool(use_shared_secret)
         self.protocol = protocol
         self.two_fa_secret_key = two_fa_secret_key
 
         self.session.mount(f'{self.protocol}://', HTTPAdapter(max_retries=retries))
 
         self.session.request = functools.partial(self.session.request, timeout=TIME_OUT)
```

### Comparing `pyPreservica-2.6.7/pyPreservica/contentAPI.py` & `pyPreservica-2.7.0/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/entityAPI.py` & `pyPreservica-2.7.0/pyPreservica/entityAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1876,15 +1876,19 @@
             paged_set = self.children(folder, maximum=maximum, next_page=paged_set.next_page)
             for entity in paged_set.results:
                 yield entity
 
     def children(self, folder: Union[str, Folder] = None, maximum: int = 100, next_page: str = None) -> PagedSet:
         headers = {HEADER_TOKEN: self.token}
         data = {'start': str(0), 'max': str(maximum)}
-        folder_reference = folder
+
+        if isinstance(folder, Folder):
+            folder_reference = folder.reference
+        else:
+            folder_reference = folder
         if next_page is None:
             if folder_reference is None:
                 request = self.session.get(f'{self.protocol}://{self.server}/api/entity/root/children', params=data,
                                            headers=headers)
             else:
                 if hasattr(folder, "reference"):
                     folder_reference = folder.reference
```

### Comparing `pyPreservica-2.6.7/pyPreservica/monitorAPI.py` & `pyPreservica-2.7.0/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/opex.py` & `pyPreservica-2.7.0/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/parAPI.py` & `pyPreservica-2.7.0/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/retentionAPI.py` & `pyPreservica-2.7.0/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/uploadAPI.py` & `pyPreservica-2.7.0/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/webHooksAPI.py` & `pyPreservica-2.7.0/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica/workflowAPI.py` & `pyPreservica-2.7.0/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.7.0/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.6.7
+Version: 2.7.0
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.6.7/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.7.0/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.6.7/setup.py` & `pyPreservica-2.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="2.6.7",
+    version="2.7.0",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

