# Comparing `tmp/open_parser-0.0.6.tar.gz` & `tmp/open_parser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_parser-0.0.6.tar", max compression
+gzip compressed data, was "open_parser-0.0.7.tar", max compression
```

## Comparing `open_parser-0.0.6.tar` & `open_parser-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1886 2024-04-19 08:19:17.616734 open_parser-0.0.6/README.md
--rw-r--r--   0        0        0       89 2024-04-19 08:21:13.633818 open_parser-0.0.6/open_parser/__init__.py
--rw-r--r--   0        0        0     3494 2024-04-19 08:19:17.625678 open_parser-0.0.6/open_parser/base.py
--rw-r--r--   0        0        0      394 2024-04-19 08:21:13.634455 open_parser-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2548 1970-01-01 00:00:00.000000 open_parser-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1886 2024-04-19 08:19:17.616734 open_parser-0.0.7/README.md
+-rw-r--r--   0        0        0       89 2024-05-01 06:36:34.471916 open_parser-0.0.7/open_parser/__init__.py
+-rw-r--r--   0        0        0     3482 2024-05-01 06:31:12.459921 open_parser-0.0.7/open_parser/base.py
+-rw-r--r--   0        0        0      394 2024-05-01 06:36:34.472225 open_parser-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2548 1970-01-01 00:00:00.000000 open_parser-0.0.7/PKG-INFO
```

### Comparing `open_parser-0.0.6/README.md` & `open_parser-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `open_parser-0.0.6/open_parser/base.py` & `open_parser-0.0.7/open_parser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def setAPIKey(self, apiKey):
         self._request_header = {"x-api-key": apiKey}
 
     def extract(self, file_path):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_file_extraction(user_id, job_id, s3_key)
-        return json.loads(result)["result"]["file_content"]
+        return json.loads(result)["result"]
 
     def parse(self, file_path, prompt, mode="advanced"):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_info_extraction(user_id, job_id, s3_key, mode, prompt)
         return json.loads(result)["result"]
 
     def _error_handler(self, response):
@@ -81,15 +81,15 @@
         if mode not in ["advanced", "basic"]:
             raise ValueError("Invalid mode. Choose either 'advanced' or 'basic'.")
         payload = {
             "userId": user_id,
             "jobId": job_id,
             "fileKey": s3_key,
             "user_prompt": prompt,
-            "use_textract": True if mode == "advanced" else False,
+            "use_textract": "True" if mode == "advanced" else "False",
         }
         response = requests.post(
             self._parseurl, headers=self._request_header, json=payload
         )
 
         if response.status_code == 200:
             print("Extraction success.")
```

### Comparing `open_parser-0.0.6/PKG-INFO` & `open_parser-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: Open parser for all.
 Author: CambioML
 Author-email: wanwanaiai45@gmail.com
 Maintainer: Rachel Hu
 Maintainer-email: goldpiggy@berkeley.edu
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
```

