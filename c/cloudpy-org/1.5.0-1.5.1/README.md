# Comparing `tmp/cloudpy_org-1.5.0.tar.gz` & `tmp/cloudpy_org-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.5.0.tar", last modified: Fri Apr 26 20:39:48 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.5.1.tar", last modified: Wed May  1 08:59:29 2024, max compression
```

## Comparing `cloudpy_org-1.5.0.tar` & `cloudpy_org-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.583645 cloudpy_org-1.5.0/
--rw-rw-rw-   0        0        0      935 2024-04-26 20:39:48.582644 cloudpy_org-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.438570 cloudpy_org-1.5.0/cloudpy_org/
--rw-rw-rw-   0        0        0     1864 2024-04-26 20:38:32.000000 cloudpy_org-1.5.0/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    31386 2024-04-26 04:25:00.000000 cloudpy_org-1.5.0/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0     4309 2024-04-26 20:34:35.000000 cloudpy_org-1.5.0/cloudpy_org/client_usage.py
--rw-rw-rw-   0        0        0    12311 2024-04-20 07:40:33.000000 cloudpy_org-1.5.0/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     2618 2024-04-20 07:40:27.000000 cloudpy_org-1.5.0/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    49186 2024-04-20 07:40:22.000000 cloudpy_org-1.5.0/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     3696 2024-04-20 07:40:17.000000 cloudpy_org-1.5.0/cloudpy_org/web.py
-drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.559633 cloudpy_org-1.5.0/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-26 20:39:47.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-26 20:39:46.000000 cloudpy_org-1.5.0/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 20:39:48.583645 cloudpy_org-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-04-26 20:35:53.000000 cloudpy_org-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:59:29.608911 cloudpy_org-1.5.1/
+-rw-rw-rw-   0        0        0      935 2024-05-01 08:59:29.608262 cloudpy_org-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 08:59:29.474939 cloudpy_org-1.5.1/cloudpy_org/
+-rw-rw-rw-   0        0        0     3169 2024-05-01 08:55:23.000000 cloudpy_org-1.5.1/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    32752 2024-05-01 08:48:41.000000 cloudpy_org-1.5.1/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0    23305 2024-05-01 08:48:51.000000 cloudpy_org-1.5.1/cloudpy_org/client_usage.py
+-rw-rw-rw-   0        0        0    13614 2024-05-01 08:49:05.000000 cloudpy_org-1.5.1/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     3924 2024-05-01 08:43:26.000000 cloudpy_org-1.5.1/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    49731 2024-05-01 08:49:21.000000 cloudpy_org-1.5.1/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     4998 2024-05-01 08:49:29.000000 cloudpy_org-1.5.1/cloudpy_org/web.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:59:29.585321 cloudpy_org-1.5.1/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-05-01 08:59:28.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 08:59:29.608911 cloudpy_org-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-05-01 08:58:57.000000 cloudpy_org-1.5.1/setup.py
```

### Comparing `cloudpy_org-1.5.0/PKG-INFO` & `cloudpy_org-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.5.0
+Version: 1.5.1
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.0/cloudpy_org/aws.py` & `cloudpy_org-1.5.1/cloudpy_org/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+███████████████████████████aws of cloudpy_org███████████████████████████
+Copyright © 2023-2024 Cloudpy.org
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Find documentation at https://www.cloudpy.org
+"""
 from cloudpy_org import cloudpy_org_version,gsep,processing_tools,aws_regions,subscription_url,msh
 import requests
 import inspect
 import json
 import os
 import random
 import time
@@ -570,15 +581,16 @@
         url_base = "http://localhost/"
     url_1 = url_base + endpoint
     this_response = requests.post(url=url_1,json=json_data,verify=False)
     if expects_json:
         try:
             return this_response.json()
         except Exception as e:
-            return {"error":"this returned: " + this_response.text, "json_data":json_data}
+            return {"error":"Wrong post request-"}
+            #return {"error":"this returned: " + this_response.text, "json_data":json_data}
     else:
         return this_response.text
 def configure_aws(service_token:str,aws_namespace:str,access_key_id:str,secret_access_key:str,local:bool=False):
     enc1 = post_it(json_data={"val":access_key_id,"case":1},endpoint='special_enc',local=local)
     enc2 = post_it(json_data={"val":secret_access_key,"case":2},endpoint='special_enc',local=local)
     this_json_data = {"service_token":service_token,"enc1":enc1,"enc2":enc2,"aws_account_tagname":aws_namespace,"active":True}
     return post_it(json_data=this_json_data,endpoint='update_aws_auth_token',local=local)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cloudpy_org-1.5.0/cloudpy_org/docs.py` & `cloudpy_org-1.5.1/cloudpy_org/docs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+███████████████████████████docs of cloudpy_org███████████████████████████
+Copyright © 2023-2024 Cloudpy.org
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Find documentation at https://www.cloudpy.org
+"""
 from cloudpy_org import cloudpy_org_version,processing_tools
 from typing import Union
 import inspect
 import os
 pt = processing_tools()
 class auto_document:
     def __init__(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cloudpy_org-1.5.0/cloudpy_org/tools.py` & `cloudpy_org-1.5.1/cloudpy_org/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from cryptography.fernet import Fernet
 import numpy as np
 import inspect
 from os import walk
 import s3fs
 import random
 import time
+import re
 unique_id = lambda: int(round(time.time() * 100000))
 class processing_tools:
     def __init__(self,data:dict={},bucket_name:str='',region_name:str="us-east-2",local:bool=False,third_part:str=None):
         self.current_path = os.getcwd() + "/"
         self.aws_auth_token_expired = True
         self.aws_authenticated = False
         self.aws_auth_error_message = ""
@@ -73,14 +74,27 @@
         except:
             self.fs = None
         try:
             self.load_metadata()
         except:
             ...
     #__________________________________________________________________________
+    def camel_to_snake(self,input_str):
+        rslt = input_str.replace(' ','_')\
+        .replace('__','_')\
+        .replace('__','_')\
+        .replace('__','')
+        rslt = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', rslt)
+        rslt = re.sub('([a-z0-9])([A-Z])', r'\1_\2', rslt).lower()
+        rslt = rslt.lower().replace('__','_')\
+        .replace('__','_')\
+        .replace('__','')
+        return rslt
+    
+    #__________________________________________________________________________
     
     def dictstr_to_dict(self,dictstr:str):
         n = random.randint(1,1000)
         m = random.randint(1,1000)
         j = random.randint(1,1000)
         k = random.randint(1,1000)
         date_id,time_id = self.date_time_id(local=True)
@@ -282,14 +296,15 @@
                 #self.aws_auth_error_message = "Invalid AWS authentication token."
                 self.xsession = None
                 self.xs3_client = None
 
         self.__session = self.xsession
         self.__s3_client = self.xs3_client
         self.s3_client = self.__s3_client
+        self.b3session = self.xsession
         if self.__session != None:
             self.__resource = self.__session.resource('s3')
         else:
             self.__resource=boto3.resource('s3')
             
         del self.xtdata
         del self.xsession
```

### Comparing `cloudpy_org-1.5.0/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.5.1/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.5.0
+Version: 1.5.1
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.0/setup.py` & `cloudpy_org-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.5.0",
+    version="1.5.1",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

