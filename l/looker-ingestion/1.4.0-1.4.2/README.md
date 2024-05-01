# Comparing `tmp/looker_ingestion-1.4.0.tar.gz` & `tmp/looker_ingestion-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looker_ingestion-1.4.0.tar", last modified: Thu Nov 16 16:09:59 2023, max compression
+gzip compressed data, was "looker_ingestion-1.4.2.tar", last modified: Wed May  1 17:48:30 2024, max compression
```

## Comparing `looker_ingestion-1.4.0.tar` & `looker_ingestion-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-16 16:09:59.465635 looker_ingestion-1.4.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10162 2023-11-16 16:09:59.461635 looker_ingestion-1.4.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-16 16:09:59.461635 looker_ingestion-1.4.0/looker_ingestion/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/looker_ingestion/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/looker_ingestion/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2915 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/looker_ingestion/load_s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10713 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/looker_ingestion/sync_data.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-16 16:09:59.461635 looker_ingestion-1.4.0/looker_ingestion.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10162 2023-11-16 16:09:59.000000 looker_ingestion-1.4.0/looker_ingestion.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2023-11-16 16:09:59.000000 looker_ingestion-1.4.0/looker_ingestion.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-11-16 16:09:59.000000 looker_ingestion-1.4.0/looker_ingestion.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-11-16 16:09:59.000000 looker_ingestion-1.4.0/looker_ingestion.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-11-16 16:09:59.000000 looker_ingestion-1.4.0/looker_ingestion.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-11-16 16:09:59.000000 looker_ingestion-1.4.0/looker_ingestion.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-11-16 16:09:59.465635 looker_ingestion-1.4.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-16 16:09:59.461635 looker_ingestion-1.4.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3573 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/tests/test_load_s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2023-11-16 16:09:46.000000 looker_ingestion-1.4.0/tests/test_sync_data.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 17:48:30.657428 looker_ingestion-1.4.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10235 2024-05-01 17:48:30.653427 looker_ingestion-1.4.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 17:48:30.653427 looker_ingestion-1.4.2/looker_ingestion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/looker_ingestion/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/looker_ingestion/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/looker_ingestion/load_s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10769 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/looker_ingestion/sync_data.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 17:48:30.653427 looker_ingestion-1.4.2/looker_ingestion.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10235 2024-05-01 17:48:30.000000 looker_ingestion-1.4.2/looker_ingestion.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2024-05-01 17:48:30.000000 looker_ingestion-1.4.2/looker_ingestion.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-01 17:48:30.000000 looker_ingestion-1.4.2/looker_ingestion.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-05-01 17:48:30.000000 looker_ingestion-1.4.2/looker_ingestion.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-01 17:48:30.000000 looker_ingestion-1.4.2/looker_ingestion.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2024-05-01 17:48:30.000000 looker_ingestion-1.4.2/looker_ingestion.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-01 17:48:30.657428 looker_ingestion-1.4.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 17:48:30.653427 looker_ingestion-1.4.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3573 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/tests/test_load_s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2024-05-01 17:48:19.000000 looker_ingestion-1.4.2/tests/test_sync_data.py
```

### Comparing `looker_ingestion-1.4.0/LICENSE` & `looker_ingestion-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `looker_ingestion-1.4.0/PKG-INFO` & `looker_ingestion-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: looker_ingestion
-Version: 1.4.0
-Summary: Extracts adhoc queries from the Looker API to S3
-Home-page: https://github.com/open-toast/extract-looker-metadata
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Looker Metadata Extractor
 
 [![PyPi](https://img.shields.io/pypi/v/looker_ingestion.svg)](https://pypi.org/project/looker_ingestion/)
 [![Downloads](https://pepy.tech/badge/looker_ingestion)](https://pepy.tech/project/looker_ingestion)
 
 This is a data infrastructure tool that extracts the results of any valid query against [Looker](https://looker.com/), a popular data visualization tool, and stores the results in [Amazon Simple Storage Service (Amazon S3)](https://aws.amazon.com/s3/). In the tool itself, metadata can be queried and manually extracted. However, not all objects that are available in the front end are exposed via the API. Instead, the data can be accessed by writing a custom query against the relevant Looker object. For instance, query history is not an API object that one can access directly, but the data can be extracted with a custom query.
 For definitions of terms used in this readme, please see the Terminology section.
@@ -217,8 +207,8 @@
 ## License
 
 This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details
 
 ## Acknowledgments
 
 The idea to use a custom query to get Looker metadata came from [Singer Looker Tap](https://github.com/singer-io/tap-looker)
-Made possible by the [Looker SDK](https://github.com/looker-open-source/sdk-codegen)
+Made possible by the [Looker SDK](https://github.com/looker-open-source/sdk-codegen)
```

### Comparing `looker_ingestion-1.4.0/README.md` & `looker_ingestion-1.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: looker_ingestion
+Version: 1.4.2
+Summary: Extracts adhoc queries from the Looker API to S3
+Home-page: https://github.com/open-toast/extract-looker-metadata
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3
+Requires-Dist: looker_sdk
+Requires-Dist: smart_open
+
 # Looker Metadata Extractor
 
 [![PyPi](https://img.shields.io/pypi/v/looker_ingestion.svg)](https://pypi.org/project/looker_ingestion/)
 [![Downloads](https://pepy.tech/badge/looker_ingestion)](https://pepy.tech/project/looker_ingestion)
 
 This is a data infrastructure tool that extracts the results of any valid query against [Looker](https://looker.com/), a popular data visualization tool, and stores the results in [Amazon Simple Storage Service (Amazon S3)](https://aws.amazon.com/s3/). In the tool itself, metadata can be queried and manually extracted. However, not all objects that are available in the front end are exposed via the API. Instead, the data can be accessed by writing a custom query against the relevant Looker object. For instance, query history is not an API object that one can access directly, but the data can be extracted with a custom query.
 For definitions of terms used in this readme, please see the Terminology section.
@@ -207,8 +220,8 @@
 ## License
 
 This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details
 
 ## Acknowledgments
 
 The idea to use a custom query to get Looker metadata came from [Singer Looker Tap](https://github.com/singer-io/tap-looker)
-Made possible by the [Looker SDK](https://github.com/looker-open-source/sdk-codegen)
+Made possible by the [Looker SDK](https://github.com/looker-open-source/sdk-codegen)
```

### Comparing `looker_ingestion-1.4.0/looker_ingestion/load_s3.py` & `looker_ingestion-1.4.2/looker_ingestion/load_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         files.extend(contents)
 
     ### if this is the first goaround, return an empty []
     if len(files) == 0:
         return json_row_objects
 
     most_recent_file = max(files, key=lambda x: x["LastModified"])
+    logging.info(f"Most recent file: {most_recent_file['Key']}")
 
     content_object = s3_storage.Object(s3_bucket, most_recent_file["Key"])
     file_content = content_object.get()["Body"].read().decode("utf-8")
     if content_object.key.endswith(".json"):
         for line in file_content.splitlines():
             for json_line in json.loads(line):
                 json_row_objects.append(json_line)
```

### Comparing `looker_ingestion-1.4.0/looker_ingestion/sync_data.py` & `looker_ingestion-1.4.2/looker_ingestion/sync_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,22 +203,23 @@
                 aws_storage_bucket_name,
                 aws_server_public_key,
                 aws_server_secret_key,
             )
             filters[datetime_index] = f"{date_filter}"
 
         ## hit the Looker API
-        write_query = looker_sdk.models.WriteQuery(
+        write_query = looker_sdk.models40.WriteQuery(
             model=query_body["model"],
             view=query_body["explore"],
             fields=fields,
             filters=filters,
             sorts=sorts,
             limit=row_limit,
         )
+        logging.info(f"Running query: {write_query}")
         sdk = looker_sdk.init40()
         query_run = sdk.run_inline_query(result_format, write_query)
         if result_format == "json":
             query_run = json.loads(query_run)
             if query_run != []:
                 if query_run[0].get("looker_error") is not None:
                     logging.error(
```

### Comparing `looker_ingestion-1.4.0/looker_ingestion.egg-info/PKG-INFO` & `looker_ingestion-1.4.2/looker_ingestion.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
-Name: looker-ingestion
-Version: 1.4.0
+Name: looker_ingestion
+Version: 1.4.2
 Summary: Extracts adhoc queries from the Looker API to S3
 Home-page: https://github.com/open-toast/extract-looker-metadata
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3
+Requires-Dist: looker_sdk
+Requires-Dist: smart_open
 
 # Looker Metadata Extractor
 
 [![PyPi](https://img.shields.io/pypi/v/looker_ingestion.svg)](https://pypi.org/project/looker_ingestion/)
 [![Downloads](https://pepy.tech/badge/looker_ingestion)](https://pepy.tech/project/looker_ingestion)
 
 This is a data infrastructure tool that extracts the results of any valid query against [Looker](https://looker.com/), a popular data visualization tool, and stores the results in [Amazon Simple Storage Service (Amazon S3)](https://aws.amazon.com/s3/). In the tool itself, metadata can be queried and manually extracted. However, not all objects that are available in the front end are exposed via the API. Instead, the data can be accessed by writing a custom query against the relevant Looker object. For instance, query history is not an API object that one can access directly, but the data can be extracted with a custom query.
```

### Comparing `looker_ingestion-1.4.0/setup.py` & `looker_ingestion-1.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="looker_ingestion",
-    version="1.4.0",
+    version="1.4.2",
     description="Extracts adhoc queries from the Looker API to S3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/open-toast/extract-looker-metadata",
     packages=find_packages(),
-    entry_points={
-        "console_scripts": ["extract_looker_metadata = looker_ingestion.sync_data:main"]
-    },
+    entry_points={"console_scripts": ["extract_looker_metadata = looker_ingestion.sync_data:main"]},
     install_requires=["boto3", "looker_sdk", "smart_open"],
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "moto"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `looker_ingestion-1.4.0/tests/test_load_s3.py` & `looker_ingestion-1.4.2/tests/test_load_s3.py`

 * *Files identical despite different names*

### Comparing `looker_ingestion-1.4.0/tests/test_sync_data.py` & `looker_ingestion-1.4.2/tests/test_sync_data.py`

 * *Files identical despite different names*

