# Comparing `tmp/unmand-1.0.1.tar.gz` & `tmp/unmand-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unmand-1.0.1.tar", last modified: Thu Oct  7 11:01:44 2021, max compression
+gzip compressed data, was "unmand-2.0.0.tar", last modified: Wed May  1 00:56:15 2024, max compression
```

## Comparing `unmand-1.0.1.tar` & `unmand-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jkhor      (501) staff       (20)        0 2021-10-07 11:01:44.712298 unmand-1.0.1/
--rw-r--r--   0 jkhor      (501) staff       (20)    35149 2021-09-14 12:09:00.000000 unmand-1.0.1/LICENSE
--rw-r--r--   0 jkhor      (501) staff       (20)     3067 2021-10-07 11:01:44.712043 unmand-1.0.1/PKG-INFO
--rw-r--r--   0 jkhor      (501) staff       (20)     2430 2021-09-15 09:26:54.000000 unmand-1.0.1/README.md
--rw-r--r--   0 jkhor      (501) staff       (20)      103 2021-09-14 12:37:33.000000 unmand-1.0.1/pyproject.toml
--rw-r--r--   0 jkhor      (501) staff       (20)       38 2021-10-07 11:01:44.712391 unmand-1.0.1/setup.cfg
--rw-r--r--   0 jkhor      (501) staff       (20)     1042 2021-10-07 11:01:35.000000 unmand-1.0.1/setup.py
-drwxr-xr-x   0 jkhor      (501) staff       (20)        0 2021-10-07 11:01:44.707188 unmand-1.0.1/src/
-drwxr-xr-x   0 jkhor      (501) staff       (20)        0 2021-10-07 11:01:44.709556 unmand-1.0.1/src/unmand/
--rw-r--r--   0 jkhor      (501) staff       (20)     8225 2021-10-07 11:01:09.000000 unmand-1.0.1/src/unmand/__init__.py
-drwxr-xr-x   0 jkhor      (501) staff       (20)        0 2021-10-07 11:01:44.711644 unmand-1.0.1/src/unmand.egg-info/
--rw-r--r--   0 jkhor      (501) staff       (20)     3067 2021-10-07 11:01:44.000000 unmand-1.0.1/src/unmand.egg-info/PKG-INFO
--rw-r--r--   0 jkhor      (501) staff       (20)      266 2021-10-07 11:01:44.000000 unmand-1.0.1/src/unmand.egg-info/SOURCES.txt
--rw-r--r--   0 jkhor      (501) staff       (20)        1 2021-10-07 11:01:44.000000 unmand-1.0.1/src/unmand.egg-info/dependency_links.txt
--rw-r--r--   0 jkhor      (501) staff       (20)        1 2021-09-14 12:50:53.000000 unmand-1.0.1/src/unmand.egg-info/not-zip-safe
--rw-r--r--   0 jkhor      (501) staff       (20)        9 2021-10-07 11:01:44.000000 unmand-1.0.1/src/unmand.egg-info/requires.txt
--rw-r--r--   0 jkhor      (501) staff       (20)        7 2021-10-07 11:01:44.000000 unmand-1.0.1/src/unmand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.073983 unmand-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 00:56:08.000000 unmand-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-01 00:56:15.073983 unmand-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-01 00:56:08.000000 unmand-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 00:56:08.000000 unmand-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:56:15.073983 unmand-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-01 00:56:08.000000 unmand-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.069983 unmand-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.069983 unmand-2.0.0/src/unmand/
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-01 00:56:08.000000 unmand-2.0.0/src/unmand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.073983 unmand-2.0.0/src/unmand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:56:14.000000 unmand-2.0.0/src/unmand.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/top_level.txt
```

### Comparing `unmand-1.0.1/LICENSE` & `unmand-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unmand-1.0.1/setup.py` & `unmand-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Core module for making requests to Unmand APIs"""
 import setuptools
 
+
 def readme():
     """Pull README file for long documentation string"""
     with open("README.md", "r") as f:
         return f.read()
 
 setuptools.setup(name='unmand',
-    version='1.0.1',
+    version='2.0.0',
     description='Helper library for consuming the Unmand API',
     url='https://github.com/unmand-systems/unmand-python',
     author='Josiah Khor',
     author_email='josiah.khor@unmand.com',
     long_description=readme(),
     long_description_content_type="text/markdown",
     project_urls={
```

### Comparing `unmand-1.0.1/src/unmand/__init__.py` & `unmand-2.0.0/src/unmand/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Upload a Swarm task"""
+import os
 import time
 import logging
 from datetime import datetime
 
 import requests
 from requests.auth import AuthBase
 
@@ -14,35 +15,36 @@
         self.token = token
 
     def __call__(self, r):
         """Attach an API token to a custom auth header."""
         r.headers['Authorization'] = self.token
         return r
 
-class Job:
-    """Represents a job running on the Exfil API"""
 
-    def __init__(self, job_id, status):
-        self.job_id = job_id
+class Extraction:
+    """Represents an extraction running on Exfil API"""
+
+    def __init__(self, extraction_guid, status):
+        self.guid = extraction_guid
         self.status = status
         self.time_queued = time.time()
         self.time_finished = None
         self.result = None
 
     def update_status(self, status):
-        """Change status of the job"""
+        """Change status of the extraction"""
         self.status = status
 
     def save_result(self, result):
-        """Save job result"""
+        """Save extraction result"""
         self.time_finished = time.time()
         self.result = result
 
     def __repr__(self):
-        return '<{}: Id={} Status={}>'.format(self.__class__.__name__, self.job_id, self.status)
+        return f'<{self.__class__.__name__}: Id={self.guid} Status={self.status}>'
 
 
 class Task: # pylint: disable=too-few-public-methods, too-many-instance-attributes
     """Represents a Swarm task outcome"""
 
     def __init__(self, task_id, start, finish, status, environment, response, details, custom_column1, custom_column2, custom_column3): # pylint: disable=too-many-arguments, too-many-branches, unused-argument
         self.guid: str = task_id #pylint: disable=invalid-name
@@ -64,146 +66,158 @@
         if self.created is not None:
             self.created = self.created.isoformat()
         if self.updated is not None and not isinstance(self.updated, datetime):
             raise Exception('End value must be a datetime object if provided')
         if self.updated is not None:
             self.updated = self.updated.isoformat()
 
-        if isinstance(self.status, str):
-            if self.status not in ['FAILURE', 'SUCCESS']:
-                raise Exception('Status must be one of "FAILURE" or "SUCCESS"')
-        else:
+        if not isinstance(self.status, str):
             raise Exception('Status must be a string and one of "FAILURE" or "SUCCESS"')
 
-        if isinstance(self.environment, str):
-            if self.environment not in ['TEST', 'UAT', 'PROD']:
-                raise Exception("""Status must be one of "TEST", "UAT", or "PROD" """)
-            if self.environment == 'UAT':
-                self.environment = 'TEST'
-        else:
+        if self.status not in ['FAILURE', 'SUCCESS']:
+            raise Exception('Status must be one of "FAILURE" or "SUCCESS"')
+        if not isinstance(self.environment, str):
             raise Exception("""Status must be a string and one of "TEST", "UAT", or "PROD" """)
 
+        if self.environment not in ['TEST', 'UAT', 'PROD']:
+            raise Exception("""Status must be one of "TEST", "UAT", or "PROD" """)
+        if self.environment == 'UAT':
+            self.environment = 'TEST'
         if not isinstance(self.outcome, str):
             raise Exception('Response must be a string')
         if not self.outcome[0].isupper():
             raise Exception('First letter of response must be upper case')
 
         if not isinstance(self.data, (dict, list)) and self.data is not None:
             raise Exception('Details must be JSON compatible: list or dictionary')
 
     def __repr__(self):
-        return '<{}: Id={} Status={}>'.format(self.__class__.__name__, self.guid, self.status)
+        return f'<{self.__class__.__name__}: Id={self.guid} Status={self.status}>'
+
 
 class ExfilAPI:
     """Implements a connection to the Exfil API"""
 
     def __init__(self, token, test=False):
         self.token = token
         if test:
-            self.url = 'https://exfil-uat.unmand.app/'
+            self.url = os.getenv('EXFIL_API_URL', 'https://exfil-uat.unmand.app/')
         else:
-            self.url = 'https://exfil.unmand.app/'
+            self.url = os.getenv('EXFIL_API_URL', 'https://exfil.unmand.app/')
 
-    def queue(self, file_data, uuid=None):
+    def queue(self, file_data, guid=None):
         """Submit a document for prediction"""
-        files = {
-            "file": file_data
-        }
-
-        data = {
-            "model": uuid
-        }
+        files = {"file": file_data}
 
-        if uuid:
-            r = requests.post(self.url + 'predictions/', files=files, data=data, auth=TokenAuth(self.token))
-        else:
-            r = requests.post(self.url + 'predictions/', files=files, auth=TokenAuth(self.token))
+        if guid:
+            logging.error('Model version selection not supported. Defaulting to the ACTIVE model version.')
+
+        result = requests.post(
+            f'{self.url}projects/extractions',
+            files=files,
+            auth=TokenAuth(self.token)
+        )
 
-        if r.status_code == requests.codes.created: # pylint: disable=no-member
-            response = r.json()
-            return Job(response.get('jobId'), response.get('status'))
-        return Job(None, 'FAILED')
+        if result.status_code == requests.codes.created:  # pylint: disable=no-member
+            response = result.json()
+            return Extraction(response.get('extractionGuid'), response.get('status'))
 
-    def poll(self, job, max_tries=100, interval=10.0, suppress_output=False): # pylint: disable=too-many-branches
+        return Extraction(None, 'FAILED')
+
+    def poll(self, extraction, max_tries=100, interval=10.0, suppress_output=False):  # pylint: disable=too-many-branches
         """Check if prediction is done"""
 
         # Helper function
-        def estimate_job_time(bounding_box_count):
+        def estimate_extraction_time(bounding_box_count):
+            """Estimate extraction time based on number of bounding boxes"""
             return 0.000014 * (bounding_box_count ** 2) + (0.02255 * bounding_box_count) + 1.08
 
         try_count = 0
 
-        params = {
-            "jobId": job.job_id,
-        }
+        extraction_guid = extraction.guid
 
-        while job.status not in ['FAILED', 'FINISHED']:
+        while extraction.status not in ['FAILED', 'FINISHED']:
             time.sleep(interval)
 
-            r = requests.post(self.url + 'predictions/result', params, auth=TokenAuth(self.token))
+            result = requests.get(
+                f'{self.url}extractions/{extraction_guid}/data', auth=TokenAuth(self.token)
+            )
 
-            if r.status_code == requests.codes.ok: # pylint: disable=no-member
-                response = r.json()
+            if result.status_code == requests.codes.ok:  # pylint: disable=no-member
+                response = result.json()
 
-                job.update_status(response.get('status'))
+                extraction.update_status(response.get('status'))
 
-                if job.status == 'QUEUED':
+                if extraction.status == 'QUEUED':
                     try_count += 1
                     if try_count > max_tries:
                         if not suppress_output:
                             logging.error('API not responding')
-                        job.update_status('FAILED')
-                        return job
-                elif job.status == 'STARTED':
-                    wait_period = estimate_job_time(response.get('numberOfBboxes'))
+                        extraction.update_status('FAILED')
+                        return extraction
+
+                elif extraction.status == 'STARTED':
+                    wait_period = estimate_extraction_time(
+                        len(response.get('bboxes', [])))
                     if not suppress_output:
-                        logging.info('Job running: Estimated job length {:.1f}s'.format(wait_period))
+                        logging.info('Extraction running: Estimated extraction length {:.1f}s'.format(wait_period))
                     time.sleep(wait_period)
-                elif job.status == 'FAILED':
+
+                elif extraction.status == 'FAILED':
                     if not suppress_output:
-                        logging.error('Job failed')
-                    return job
-                elif job.status == 'FINISHED':
+                        logging.error('Extraction failed')
+                    return extraction
+
+                elif extraction.status == 'FINISHED':
                     result = {
                         'total_time': response.get('timeTaken'),
                         'feature_extraction_time': response.get('timeTakenFeatureExtraction'),
                         'time_in_queue': response.get('timeInQueue'),
                         'data': response.get('data'),
                         'bboxes': response.get('bboxes')
                     }
-                    job.save_result(result)
+
+                    extraction.save_result(result)
+
                     if not suppress_output:
-                        logging.info('Job completed')
-                    return job
+                        logging.info('Extraction completed')
+
+                    return extraction
+
             else:
-                job.update_status('FAILED')
+                extraction.update_status('FAILED')
                 if not suppress_output:
                     logging.error('API not responding or responding with error state')
-                return job
+                return extraction
+
 
 class SwarmAPI:
     """Implements a connection to the Exfil API"""
 
     def __init__(self, token, test=False):
         self.token = token
         if test:
             self.url = 'https://swarm-uat.unmand.app/'
         else:
             self.url = 'https://swarm.unmand.app/'
 
     def upload_swarm_task(self, task):
         """Upload a Swarm task"""
-        params = {k: v for k, v in task.__dict__.items()} # pylint: disable=unnecessary-comprehension
-        r = requests.post(self.url + 'tasks/create', json=params, auth=TokenAuth(self.token))
+        params = dict(task.__dict__.items())
+        r = requests.post(
+            f'{self.url}tasks/create', json=params, auth=TokenAuth(self.token)
+        )
         if r.status_code == requests.codes.created:  # pylint: disable=no-member
             return r.json()
         logging.error(f'API returned {r.status_code}') # pylint: disable=logging-fstring-interpolation
         return False
 
     def update_swarm_task(self, task):
         """Update a Swarm task"""
-        params = {k: v for k, v in task.__dict__.items()} # pylint: disable=unnecessary-comprehension
-        r = requests.put(self.url + f'tasks/{task.id}', json=params, auth=TokenAuth(self.token))
+        params = dict(task.__dict__.items())
+        r = requests.put(
+            f'{self.url}tasks/{task.id}', json=params, auth=TokenAuth(self.token)
+        )
         if r.status_code == requests.codes.ok:  # pylint: disable=no-member
             return r.json()
         logging.error(f'API returned {r.status_code}') # pylint: disable=logging-fstring-interpolation
         return False
```

