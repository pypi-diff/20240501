# Comparing `tmp/seam-0.5.0.tar.gz` & `tmp/seam-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.5.0.tar", max compression
+gzip compressed data, was "seam-0.6.0.tar", max compression
```

## Comparing `seam-0.5.0.tar` & `seam-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1087 2024-04-18 19:00:30.379406 seam-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     4228 2024-04-18 19:00:30.379406 seam-0.5.0/README.rst
--rw-r--r--   0        0        0      726 2024-04-18 19:00:30.379406 seam-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       97 2024-04-18 19:00:30.379406 seam-0.5.0/seam/__init__.py
--rw-r--r--   0        0        0    11938 2024-04-18 19:00:30.379406 seam-0.5.0/seam/access_codes.py
--rw-r--r--   0        0        0      903 2024-04-18 19:00:30.379406 seam-0.5.0/seam/access_codes_simulate.py
--rw-r--r--   0        0        0     3979 2024-04-18 19:00:30.379406 seam-0.5.0/seam/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1746 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs.py
--rw-r--r--   0        0        0     2505 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_access_groups.py
--rw-r--r--   0        0        0      718 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_credential_pools.py
--rw-r--r--   0        0        0     1782 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4763 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_credentials.py
--rw-r--r--   0        0        0     2172 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_entrances.py
--rw-r--r--   0        0        0      955 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_systems.py
--rw-r--r--   0        0        0     6476 2024-04-18 19:00:30.379406 seam-0.5.0/seam/acs_users.py
--rw-r--r--   0        0        0     3169 2024-04-18 19:00:30.379406 seam-0.5.0/seam/action_attempts.py
--rw-r--r--   0        0        0     5751 2024-04-18 19:00:30.379406 seam-0.5.0/seam/client_sessions.py
--rw-r--r--   0        0        0     3292 2024-04-18 19:00:30.379406 seam-0.5.0/seam/connect_webviews.py
--rw-r--r--   0        0        0     2520 2024-04-18 19:00:30.379406 seam-0.5.0/seam/connected_accounts.py
--rw-r--r--   0        0        0     4761 2024-04-18 19:00:30.379406 seam-0.5.0/seam/devices.py
--rw-r--r--   0        0        0      517 2024-04-18 19:00:30.379406 seam-0.5.0/seam/devices_simulate.py
--rw-r--r--   0        0        0     3323 2024-04-18 19:00:30.379406 seam-0.5.0/seam/devices_unmanaged.py
--rw-r--r--   0        0        0     2385 2024-04-18 19:00:30.379406 seam-0.5.0/seam/events.py
--rw-r--r--   0        0        0     4181 2024-04-18 19:00:30.379406 seam-0.5.0/seam/locks.py
--rw-r--r--   0        0        0      765 2024-04-18 19:00:30.379406 seam-0.5.0/seam/networks.py
--rw-r--r--   0        0        0      714 2024-04-18 19:00:30.379406 seam-0.5.0/seam/noise_sensors.py
--rw-r--r--   0        0        0     4350 2024-04-18 19:00:30.379406 seam-0.5.0/seam/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      594 2024-04-18 19:00:30.379406 seam-0.5.0/seam/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1063 2024-04-18 19:00:30.379406 seam-0.5.0/seam/phones.py
--rw-r--r--   0        0        0     1185 2024-04-18 19:00:30.379406 seam-0.5.0/seam/phones_simulate.py
--rw-r--r--   0        0        0     1535 2024-04-18 19:00:30.379406 seam-0.5.0/seam/routes.py
--rw-r--r--   0        0        0     3175 2024-04-18 19:00:30.379406 seam-0.5.0/seam/seam.py
--rw-r--r--   0        0        0     8926 2024-04-18 19:00:30.379406 seam-0.5.0/seam/thermostats.py
--rw-r--r--   0        0        0     6930 2024-04-18 19:00:30.379406 seam-0.5.0/seam/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    65327 2024-04-18 19:00:30.383406 seam-0.5.0/seam/types.py
--rw-r--r--   0        0        0     6700 2024-04-18 19:00:30.383406 seam-0.5.0/seam/user_identities.py
--rw-r--r--   0        0        0     2903 2024-04-18 19:00:30.383406 seam-0.5.0/seam/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      864 2024-04-18 19:00:30.383406 seam-0.5.0/seam/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1815 2024-04-18 19:00:30.383406 seam-0.5.0/seam/webhooks.py
--rw-r--r--   0        0        0     2174 2024-04-18 19:00:30.383406 seam-0.5.0/seam/workspaces.py
--rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 seam-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-01 10:54:55.246269 seam-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     4765 2024-05-01 10:54:55.246269 seam-0.6.0/README.rst
+-rw-r--r--   0        0        0      726 2024-05-01 10:54:55.250269 seam-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-01 10:54:55.250269 seam-0.6.0/seam/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-01 10:54:55.250269 seam-0.6.0/seam/access_codes.py
+-rw-r--r--   0        0        0      903 2024-05-01 10:54:55.250269 seam-0.6.0/seam/access_codes_simulate.py
+-rw-r--r--   0        0        0     3979 2024-05-01 10:54:55.250269 seam-0.6.0/seam/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1746 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs.py
+-rw-r--r--   0        0        0     2505 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_access_groups.py
+-rw-r--r--   0        0        0      718 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_credential_pools.py
+-rw-r--r--   0        0        0     1782 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4763 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_credentials.py
+-rw-r--r--   0        0        0     2172 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_entrances.py
+-rw-r--r--   0        0        0      955 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_systems.py
+-rw-r--r--   0        0        0     6476 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_users.py
+-rw-r--r--   0        0        0     3255 2024-05-01 10:54:55.250269 seam-0.6.0/seam/action_attempts.py
+-rw-r--r--   0        0        0     5751 2024-05-01 10:54:55.250269 seam-0.6.0/seam/client_sessions.py
+-rw-r--r--   0        0        0     3292 2024-05-01 10:54:55.250269 seam-0.6.0/seam/connect_webviews.py
+-rw-r--r--   0        0        0     2520 2024-05-01 10:54:55.250269 seam-0.6.0/seam/connected_accounts.py
+-rw-r--r--   0        0        0     4761 2024-05-01 10:54:55.250269 seam-0.6.0/seam/devices.py
+-rw-r--r--   0        0        0      517 2024-05-01 10:54:55.250269 seam-0.6.0/seam/devices_simulate.py
+-rw-r--r--   0        0        0     3323 2024-05-01 10:54:55.250269 seam-0.6.0/seam/devices_unmanaged.py
+-rw-r--r--   0        0        0     2385 2024-05-01 10:54:55.250269 seam-0.6.0/seam/events.py
+-rw-r--r--   0        0        0     4181 2024-05-01 10:54:55.250269 seam-0.6.0/seam/locks.py
+-rw-r--r--   0        0        0      765 2024-05-01 10:54:55.250269 seam-0.6.0/seam/networks.py
+-rw-r--r--   0        0        0      714 2024-05-01 10:54:55.250269 seam-0.6.0/seam/noise_sensors.py
+-rw-r--r--   0        0        0     4350 2024-05-01 10:54:55.250269 seam-0.6.0/seam/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      594 2024-05-01 10:54:55.250269 seam-0.6.0/seam/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1063 2024-05-01 10:54:55.250269 seam-0.6.0/seam/phones.py
+-rw-r--r--   0        0        0     1185 2024-05-01 10:54:55.250269 seam-0.6.0/seam/phones_simulate.py
+-rw-r--r--   0        0        0     1535 2024-05-01 10:54:55.250269 seam-0.6.0/seam/routes.py
+-rw-r--r--   0        0        0     3175 2024-05-01 10:54:55.250269 seam-0.6.0/seam/seam.py
+-rw-r--r--   0        0        0     8926 2024-05-01 10:54:55.250269 seam-0.6.0/seam/thermostats.py
+-rw-r--r--   0        0        0     6930 2024-05-01 10:54:55.250269 seam-0.6.0/seam/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    65327 2024-05-01 10:54:55.250269 seam-0.6.0/seam/types.py
+-rw-r--r--   0        0        0     6700 2024-05-01 10:54:55.250269 seam-0.6.0/seam/user_identities.py
+-rw-r--r--   0        0        0     2903 2024-05-01 10:54:55.250269 seam-0.6.0/seam/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      851 2024-05-01 10:54:55.250269 seam-0.6.0/seam/utils/action_attempt_errors.py
+-rw-r--r--   0        0        0      864 2024-05-01 10:54:55.250269 seam-0.6.0/seam/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1815 2024-05-01 10:54:55.250269 seam-0.6.0/seam/webhooks.py
+-rw-r--r--   0        0        0     2174 2024-05-01 10:54:55.250269 seam-0.6.0/seam/workspaces.py
+-rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 seam-0.6.0/PKG-INFO
```

### Comparing `seam-0.5.0/LICENSE.txt` & `seam-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/README.rst` & `seam-0.6.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -102,22 +102,40 @@
 ::
 
     $ make watch
 
 Publishing
 ~~~~~~~~~~
 
-Use the `poetry version`_ command to release a new version.
-Then run `make version` to commit and push a new git tag
-which will trigger a GitHub action.
+New versions are created with `poetry version`_.
 
-Publishing may be triggered using a `workflow_dispatch on GitHub Actions`_.
+Automatic
+^^^^^^^^^
+
+New versions are released automatically with semantic-release_
+as long as commits follow the `Angular Commit Message Conventions`_.
+
+.. _Angular Commit Message Conventions: https://semantic-release.gitbook.io/semantic-release/#commit-message-format
+.. _semantic-release: https://semantic-release.gitbook.io/
+
+Manual
+^^^^^^
+
+Publish a new version by triggering a `version workflow_dispatch on GitHub Actions`_.
+The `version` input will be passed as the first argument to `poetry version`_.
+
+This may be done on the web or using the `GitHub CLI`_ with
+
+::
+
+    $ gh workflow run version.yml --raw-field version=<version>
 
 .. _Poetry version: https://python-poetry.org/docs/cli/#version
-.. _workflow_dispatch on GitHub Actions: https://github.com/seamapi/python-next/actions?query=workflow%3Aversion
+.. _GitHub CLI: https://cli.github.com/
+.. _version workflow_dispatch on GitHub Actions: https://github.com/seamapi/python-next/actions?query=workflow%3Aversion
 
 GitHub Actions
 --------------
 
 *GitHub Actions should already be configured: this section is for reference only.*
 
 The following repository secrets must be set on GitHub Actions.
@@ -125,15 +143,15 @@
 - ``PYPI_API_TOKEN``: API token for publishing on PyPI.
 
 These must be set manually.
 
 Secrets for Optional GitHub Actions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The version and format GitHub actions
+The version, format, generate, and semantic-release GitHub actions
 require a user with write access to the repository
 including access to read and write packages.
 Set these additional secrets to enable the action:
 
 - ``GH_TOKEN``: A personal access token for the user.
 - ``GIT_USER_NAME``: The name to set for Git commits.
 - ``GIT_USER_EMAIL``: The email to set for Git commits.
```

### Comparing `seam-0.5.0/pyproject.toml` & `seam-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seam"
-version = "0.5.0"
+version = "0.6.0"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
```

### Comparing `seam-0.5.0/seam/access_codes.py` & `seam-0.6.0/seam/access_codes.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/access_codes_simulate.py` & `seam-0.6.0/seam/access_codes_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/access_codes_unmanaged.py` & `seam-0.6.0/seam/access_codes_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs.py` & `seam-0.6.0/seam/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_access_groups.py` & `seam-0.6.0/seam/acs_access_groups.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_credential_pools.py` & `seam-0.6.0/seam/acs_credential_pools.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_credential_provisioning_automations.py` & `seam-0.6.0/seam/acs_credential_provisioning_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_credentials.py` & `seam-0.6.0/seam/acs_credentials.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_entrances.py` & `seam-0.6.0/seam/acs_entrances.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_systems.py` & `seam-0.6.0/seam/acs_systems.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/acs_users.py` & `seam-0.6.0/seam/acs_users.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/action_attempts.py` & `seam-0.6.0/seam/action_attempts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from seam.types import AbstractActionAttempts, AbstractSeam as Seam, ActionAttempt
 from typing import Optional, Any, List, Dict, Union
 
 import time
 
+from seam.utils.action_attempt_errors import (
+    SeamActionAttemptFailedError,
+    SeamActionAttemptTimeoutError,
+)
+
 
 class ActionAttempts(AbstractActionAttempts):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def get(
         self,
         *,
         action_attempt_id: str,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         json_payload = {}
 
         if action_attempt_id is not None:
             json_payload["action_attempt_id"] = action_attempt_id
 
         res = self.seam.make_request("POST", "/action_attempts/get", json=json_payload)
@@ -39,45 +44,45 @@
         return [ActionAttempt.from_dict(item) for item in res["action_attempts"]]
 
     def poll_until_ready(
         self,
         *,
         action_attempt_id: str,
         timeout: Optional[float] = 5.0,
-        polling_interval: Optional[float] = 0.5,
+        polling_interval: Optional[float] = 0.5
     ) -> ActionAttempt:
         seam = self.seam
         time_waiting = 0.0
 
         action_attempt = seam.action_attempts.get(
             action_attempt_id=action_attempt_id, wait_for_action_attempt=False
         )
 
         while action_attempt.status == "pending":
             time.sleep(polling_interval)
             time_waiting += polling_interval
 
             if time_waiting > timeout:
-                raise Exception("Timed out waiting for action attempt to be ready")
+                raise SeamActionAttemptTimeoutError(action_attempt, timeout)
 
             action_attempt = seam.action_attempts.get(
                 action_attempt_id=action_attempt.action_attempt_id,
                 wait_for_action_attempt=False,
             )
 
         if action_attempt.status == "failed":
-            raise Exception(f"Action Attempt failed: {action_attempt.error.message}")
+            raise SeamActionAttemptFailedError(action_attempt)
 
         return action_attempt
 
     def decide_and_wait(
         self,
         *,
         action_attempt: ActionAttempt,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         wait_decision = (
             self.seam.wait_for_action_attempt
             if wait_for_action_attempt is None
             else wait_for_action_attempt
         )
```

### Comparing `seam-0.5.0/seam/client_sessions.py` & `seam-0.6.0/seam/client_sessions.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/connect_webviews.py` & `seam-0.6.0/seam/connect_webviews.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/connected_accounts.py` & `seam-0.6.0/seam/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/devices.py` & `seam-0.6.0/seam/devices.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/devices_simulate.py` & `seam-0.6.0/seam/devices_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/devices_unmanaged.py` & `seam-0.6.0/seam/devices_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/events.py` & `seam-0.6.0/seam/events.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/locks.py` & `seam-0.6.0/seam/locks.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/networks.py` & `seam-0.6.0/seam/networks.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/noise_sensors.py` & `seam-0.6.0/seam/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/noise_sensors_noise_thresholds.py` & `seam-0.6.0/seam/noise_sensors_noise_thresholds.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/noise_sensors_simulate.py` & `seam-0.6.0/seam/noise_sensors_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/phones.py` & `seam-0.6.0/seam/phones.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/phones_simulate.py` & `seam-0.6.0/seam/phones_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/routes.py` & `seam-0.6.0/seam/routes.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/seam.py` & `seam-0.6.0/seam/seam.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/thermostats.py` & `seam-0.6.0/seam/thermostats.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/thermostats_climate_setting_schedules.py` & `seam-0.6.0/seam/thermostats_climate_setting_schedules.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/types.py` & `seam-0.6.0/seam/types.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/user_identities.py` & `seam-0.6.0/seam/user_identities.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/user_identities_enrollment_automations.py` & `seam-0.6.0/seam/user_identities_enrollment_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/utils/deep_attr_dict.py` & `seam-0.6.0/seam/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/webhooks.py` & `seam-0.6.0/seam/webhooks.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/seam/workspaces.py` & `seam-0.6.0/seam/workspaces.py`

 * *Files identical despite different names*

### Comparing `seam-0.5.0/PKG-INFO` & `seam-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.5.0
+Version: 0.6.0
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -122,22 +122,40 @@
 ::
 
     $ make watch
 
 Publishing
 ~~~~~~~~~~
 
-Use the `poetry version`_ command to release a new version.
-Then run `make version` to commit and push a new git tag
-which will trigger a GitHub action.
+New versions are created with `poetry version`_.
 
-Publishing may be triggered using a `workflow_dispatch on GitHub Actions`_.
+Automatic
+^^^^^^^^^
+
+New versions are released automatically with semantic-release_
+as long as commits follow the `Angular Commit Message Conventions`_.
+
+.. _Angular Commit Message Conventions: https://semantic-release.gitbook.io/semantic-release/#commit-message-format
+.. _semantic-release: https://semantic-release.gitbook.io/
+
+Manual
+^^^^^^
+
+Publish a new version by triggering a `version workflow_dispatch on GitHub Actions`_.
+The `version` input will be passed as the first argument to `poetry version`_.
+
+This may be done on the web or using the `GitHub CLI`_ with
+
+::
+
+    $ gh workflow run version.yml --raw-field version=<version>
 
 .. _Poetry version: https://python-poetry.org/docs/cli/#version
-.. _workflow_dispatch on GitHub Actions: https://github.com/seamapi/python-next/actions?query=workflow%3Aversion
+.. _GitHub CLI: https://cli.github.com/
+.. _version workflow_dispatch on GitHub Actions: https://github.com/seamapi/python-next/actions?query=workflow%3Aversion
 
 GitHub Actions
 --------------
 
 *GitHub Actions should already be configured: this section is for reference only.*
 
 The following repository secrets must be set on GitHub Actions.
@@ -145,15 +163,15 @@
 - ``PYPI_API_TOKEN``: API token for publishing on PyPI.
 
 These must be set manually.
 
 Secrets for Optional GitHub Actions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The version and format GitHub actions
+The version, format, generate, and semantic-release GitHub actions
 require a user with write access to the repository
 including access to read and write packages.
 Set these additional secrets to enable the action:
 
 - ``GH_TOKEN``: A personal access token for the user.
 - ``GIT_USER_NAME``: The name to set for Git commits.
 - ``GIT_USER_EMAIL``: The email to set for Git commits.
```

