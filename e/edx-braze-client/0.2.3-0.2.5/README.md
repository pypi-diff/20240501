# Comparing `tmp/edx-braze-client-0.2.3.tar.gz` & `tmp/edx-braze-client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-braze-client-0.2.3.tar", last modified: Mon Apr  8 14:18:36 2024, max compression
+gzip compressed data, was "edx-braze-client-0.2.5.tar", last modified: Wed May  1 20:24:38 2024, max compression
```

## Comparing `edx-braze-client-0.2.3.tar` & `edx-braze-client-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/braze/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/braze/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/edx_braze_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 14:18:36.000000 edx-braze-client-0.2.3/edx_braze_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 14:18:36.720431 edx-braze-client-0.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5176 2024-04-08 14:18:16.000000 edx-braze-client-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:24:38.192884 edx-braze-client-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-01 20:24:38.192884 edx-braze-client-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:24:38.192884 edx-braze-client-0.2.5/braze/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/braze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24222 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/braze/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/braze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/braze/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:24:38.192884 edx-braze-client-0.2.5/edx_braze_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-01 20:24:38.000000 edx-braze-client-0.2.5/edx_braze_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-01 20:24:38.000000 edx-braze-client-0.2.5/edx_braze_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:24:38.000000 edx-braze-client-0.2.5/edx_braze_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:24:38.000000 edx-braze-client-0.2.5/edx_braze_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 20:24:38.000000 edx-braze-client-0.2.5/edx_braze_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:24:38.192884 edx-braze-client-0.2.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 20:24:38.192884 edx-braze-client-0.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5176 2024-05-01 20:24:19.000000 edx-braze-client-0.2.5/setup.py
```

### Comparing `edx-braze-client-0.2.3/CHANGELOG.rst` & `edx-braze-client-0.2.5/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.2.5]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+chore: Updates version
+
+[0.2.4]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: adds 'create_recipients' function to the braze client
+
 [0.2.3]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: pass error response content into raised exceptions
 
 [0.2.2]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling both ``email`` and ``external_id`` from braze export.
```

### Comparing `edx-braze-client-0.2.3/LICENSE` & `edx-braze-client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.3/LICENSE.txt` & `edx-braze-client-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.3/PKG-INFO` & `edx-braze-client-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-braze-client
-Version: 0.2.3
+Version: 0.2.5
 Summary: Python client for interacting with Braze APIs
 Home-page: https://github.com/edx/braze-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Platform: UNKNOWN
@@ -157,14 +157,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.2.5]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+chore: Updates version
+
+[0.2.4]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: adds 'create_recipients' function to the braze client
+
 [0.2.3]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: pass error response content into raised exceptions
 
 [0.2.2]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling both ``email`` and ``external_id`` from braze export.
```

### Comparing `edx-braze-client-0.2.3/README.rst` & `edx-braze-client-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.3/braze/client.py` & `edx-braze-client-0.2.5/braze/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections import deque
 from urllib.parse import urljoin
 
 import requests
 
 from braze.constants import (
     GET_EXTERNAL_IDS_CHUNK_SIZE,
+    MAX_NUM_IDENTIFY_USERS_ALIASES,
     REQUEST_TYPE_GET,
     REQUEST_TYPE_POST,
     TRACK_USER_COMPONENT_CHUNK_SIZE,
     UNSUBSCRIBED_EMAILS_API_LIMIT,
     UNSUBSCRIBED_EMAILS_API_SORT_DIRECTION,
     UNSUBSCRIBED_STATE,
     USER_ALIAS_CHUNK_SIZE,
@@ -205,14 +206,104 @@
 
         payload = {
             'aliases_to_identify': aliases_to_identify
         }
 
         return self._make_request(payload, BrazeAPIEndpoints.IDENTIFY_USERS, REQUEST_TYPE_POST)
 
+    def create_recipients(self, alias_label, user_id_by_email, trigger_properties_by_email=None):
+        """
+        Create a recipient object using the dictionary, `user_id_by_email`
+        containing the user_email key and `lms_user_id` value.
+        Identifies a list of given email addresess with any existing Braze alias records
+        via the provided ``lms_user_id``.
+
+        https://www.braze.com/docs/api/objects_filters/user_alias_object
+        The user_alias objects requires a passed in alias_label.
+
+        https://www.braze.com/docs/api/endpoints/user_data/post_user_identify/
+        The maximum email/user_id dictionary limit is 50, any length beyond 50 will raise an error.
+
+        The trigger properties default to None and return as an empty dictionary if no individualized
+        trigger property is set based on the email.
+
+        Arguments:
+        - `alias_label` (str): The alias label of the user
+        - `user_id_by_email` (dict):  A dictionary where the key is the user's email (str)
+                                    and the value is the `lms_user_id` (int).
+        - `trigger_properties_by_email` (dict) : A dictionary where the key is the user's email (str)
+                                                and the value are the `trigger_properties` (dict)
+                                                Default is None
+
+        Raises:
+        - `BrazeClientError`: if the number of entries in `user_id_by_email` exceeds 50.
+
+        Returns:
+        - Dict: A dictionary where the key is the `user_email` (str) and the value is the metadata
+                relating to the braze recipient.
+
+        Example: create_recipients(
+                    'alias_label'='Enterprise',
+                    'user_id_by_email'= {
+                        'hamzah@example.com': 123,
+                        'alex@example.com': 231,
+                    },
+                    'trigger_properties_by_email'= {
+                        'hamzah@example.com': {
+                            'foo':'bar'
+                        },
+                        'alex@example.com': {}
+                    },
+                )
+        """
+        if len(user_id_by_email) > MAX_NUM_IDENTIFY_USERS_ALIASES:
+            msg = "Max recipient limit reached."
+            raise BrazeClientError(msg)
+
+        if trigger_properties_by_email is None:
+            trigger_properties_by_email = {}
+
+        user_aliases_by_email = {
+                email: {
+                    "alias_label": alias_label,
+                    "alias_name": email,
+                }
+                for email in user_id_by_email
+        }
+        # Identify the user alias in case it already exists. This is necessary so
+        # we don't accidently create a duplicate Braze profile.
+        self.identify_users([
+            {
+                'external_id': lms_user_id,
+                'user_alias': user_aliases_by_email.get(email)
+            }
+            for email, lms_user_id in user_id_by_email.items()
+        ])
+
+        attributes_by_email = {
+            email: {
+                "user_alias": user_aliases_by_email.get(email),
+                "email": email,
+                "is_enterprise_learner": True,
+                "_update_existing_only": False,
+            }
+            for email in user_id_by_email
+        }
+
+        return {
+            email: {
+                'external_user_id': lms_user_id,
+                'attributes': attributes_by_email.get(email),
+                # If a profile does not already exist, Braze will create a new profile before sending a message.
+                'send_to_existing_only': False,
+                'trigger_properties': trigger_properties_by_email.get(email, {}),
+            }
+            for email, lms_user_id in user_id_by_email.items()
+        }
+
     def track_user(
         self,
         attributes=None,
         events=None,
         purchases=None
     ):
         """
```

### Comparing `edx-braze-client-0.2.3/braze/constants.py` & `edx-braze-client-0.2.5/braze/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,10 +24,13 @@
 REQUEST_TYPE_POST = 'post'
 TRACK_USER_COMPONENT_CHUNK_SIZE = 75
 USER_ALIAS_CHUNK_SIZE = 50
 
 # https://www.braze.com/docs/api/endpoints/export/user_data/post_users_identifier/?tab=all%20fields
 GET_EXTERNAL_IDS_CHUNK_SIZE = 50
 
+# https://www.braze.com/docs/api/endpoints/user_data/post_user_identify/
+MAX_NUM_IDENTIFY_USERS_ALIASES = 50
+
 UNSUBSCRIBED_STATE = 'unsubscribed'
 UNSUBSCRIBED_EMAILS_API_LIMIT = 500
 UNSUBSCRIBED_EMAILS_API_SORT_DIRECTION = 'desc'
```

### Comparing `edx-braze-client-0.2.3/braze/exceptions.py` & `edx-braze-client-0.2.5/braze/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.3/edx_braze_client.egg-info/PKG-INFO` & `edx-braze-client-0.2.5/edx_braze_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-braze-client
-Version: 0.2.3
+Version: 0.2.5
 Summary: Python client for interacting with Braze APIs
 Home-page: https://github.com/edx/braze-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Platform: UNKNOWN
@@ -157,14 +157,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[0.2.5]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+chore: Updates version
+
+[0.2.4]
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+feat: adds 'create_recipients' function to the braze client
+
 [0.2.3]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 feat: pass error response content into raised exceptions
 
 [0.2.2]
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 fix: be defensive about pulling both ``email`` and ``external_id`` from braze export.
```

### Comparing `edx-braze-client-0.2.3/requirements/constraints.txt` & `edx-braze-client-0.2.5/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-braze-client-0.2.3/setup.py` & `edx-braze-client-0.2.5/setup.py`

 * *Files identical despite different names*

