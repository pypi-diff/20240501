# Comparing `tmp/workos-4.4.0.tar.gz` & `tmp/workos-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.4.0.tar", last modified: Mon Apr 29 17:14:22 2024, max compression
+gzip compressed data, was "workos-4.5.0.tar", last modified: Wed May  1 20:54:18 2024, max compression
```

## Comparing `workos-4.4.0.tar` & `workos-4.5.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.314670 workos-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 17:14:15.000000 workos-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-29 17:14:22.314670 workos-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-29 17:14:15.000000 workos-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:14:22.314670 workos-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-29 17:14:15.000000 workos-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.310670 workos-4.4.0/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 17:14:15.000000 workos-4.4.0/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-29 17:14:15.000000 workos-4.4.0/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-29 17:14:15.000000 workos-4.4.0/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-29 17:14:15.000000 workos-4.4.0/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-29 17:14:15.000000 workos-4.4.0/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 17:14:15.000000 workos-4.4.0/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-29 17:14:15.000000 workos-4.4.0/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-29 17:14:15.000000 workos-4.4.0/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-29 17:14:15.000000 workos-4.4.0/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-29 17:14:15.000000 workos-4.4.0/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-29 17:14:15.000000 workos-4.4.0/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.314670 workos-4.4.0/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-29 17:14:15.000000 workos-4.4.0/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-29 17:14:15.000000 workos-4.4.0/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.314670 workos-4.4.0/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-29 17:14:15.000000 workos-4.4.0/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.310670 workos-4.4.0/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:14:20.000000 workos-4.4.0/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.715914 workos-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 20:54:11.000000 workos-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-01 20:54:18.715914 workos-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-01 20:54:11.000000 workos-4.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:54:18.715914 workos-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-01 20:54:11.000000 workos-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.711914 workos-4.5.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 20:54:11.000000 workos-4.5.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 20:54:11.000000 workos-4.5.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-01 20:54:11.000000 workos-4.5.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-01 20:54:11.000000 workos-4.5.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-01 20:54:11.000000 workos-4.5.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 20:54:11.000000 workos-4.5.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-01 20:54:11.000000 workos-4.5.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-01 20:54:11.000000 workos-4.5.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-01 20:54:11.000000 workos-4.5.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-01 20:54:11.000000 workos-4.5.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-01 20:54:11.000000 workos-4.5.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.715914 workos-4.5.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-01 20:54:11.000000 workos-4.5.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-05-01 20:54:11.000000 workos-4.5.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.715914 workos-4.5.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-01 20:54:11.000000 workos-4.5.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.711914 workos-4.5.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:54:17.000000 workos-4.5.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.4.0/LICENSE` & `workos-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/PKG-INFO` & `workos-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.4.0
+Version: 4.5.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.4.0/README.md` & `workos-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/setup.py` & `workos-4.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/audit_logs.py` & `workos-4.5.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/client.py` & `workos-4.5.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/directory_sync.py` & `workos-4.5.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/events.py` & `workos-4.5.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/exceptions.py` & `workos-4.5.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/mfa.py` & `workos-4.5.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/organizations.py` & `workos-4.5.0/workos/organizations.py`

 * *Files 23% similar despite different names*

```diff
@@ -174,53 +174,76 @@
 
         Args:
             organization (dict) - An organization object
                 organization[name] (str) - A unique, descriptive name for the organization
                 organization[allow_profiles_outside_organization] (boolean) - Whether Connections
                     within the Organization allow profiles that are outside of the Organization's
                     configured User Email Domains. (Optional)
-                organization[domains] (list) - List of domains that belong to the organization
+                organization[domain_data] (list[dict]) - List of domains that belong to the organization.
+                    organization[domain_data][][domain] - The domain of the organization.
+                    organization[domain_data][][state] - The state of the domain: either 'verified' or 'pending'.
             idempotency_key (str) - Idempotency key for creating an organization. (Optional)
 
         Returns:
             dict: Created Organization response from WorkOS.
         """
         headers = {}
         if idempotency_key:
             headers["idempotency-key"] = idempotency_key
 
+        if "domains" in organization:
+            warn(
+                "The 'domains' parameter for 'create_organization' is deprecated. Please use 'domain_data' instead.",
+                DeprecationWarning,
+            )
+
         response = self.request_helper.request(
             ORGANIZATIONS_PATH,
             method=REQUEST_METHOD_POST,
             params=organization,
             headers=headers,
             token=workos.api_key,
         )
 
         return WorkOSOrganization.construct_from_response(response).to_dict()
 
     def update_organization(
-        self, organization, name, allow_profiles_outside_organization=None, domains=None
+        self,
+        organization,
+        name,
+        allow_profiles_outside_organization=None,
+        domains=None,
+        domain_data=None,
     ):
         """Update an organization
 
         Args:
             organization(str) - Organization's unique identifier.
             name (str) - A unique, descriptive name for the organization.
             allow_profiles_outside_organization (boolean) - Whether Connections
                 within the Organization allow profiles that are outside of the Organization's
                 configured User Email Domains. (Optional)
-            domains (list) - List of domains that belong to the organization. (Optional)
+            domains (list) - [Deprecated] Use domain_data instead. List of domains that belong to the organization. (Optional)
+            domain_data (list[dict]) - List of domains that belong to the organization. (Optional)
+                domain_data[][domain] - The domain of the organization.
+                domain_data[][state] - The state of the domain: either 'verified' or 'pending'.
 
         Returns:
             dict: Updated Organization response from WorkOS.
         """
+        if domains:
+            warn(
+                "The 'domains' parameter for 'update_organization' is deprecated. Please use 'domain_data' instead.",
+                DeprecationWarning,
+            )
+
         params = {
             "name": name,
             "domains": domains,
+            "domain_data": domain_data,
             "allow_profiles_outside_organization": allow_profiles_outside_organization,
         }
         response = self.request_helper.request(
             "organizations/{organization}".format(organization=organization),
             method=REQUEST_METHOD_PUT,
             params=params,
             token=workos.api_key,
```

### Comparing `workos-4.4.0/workos/passwordless.py` & `workos-4.5.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/portal.py` & `workos-4.5.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/audit_logs_export.py` & `workos-4.5.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/base.py` & `workos-4.5.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/directory_sync.py` & `workos-4.5.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/event.py` & `workos-4.5.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/list.py` & `workos-4.5.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/mfa.py` & `workos-4.5.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/organizations.py` & `workos-4.5.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/passwordless.py` & `workos-4.5.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/sso.py` & `workos-4.5.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/resources/user_management.py` & `workos-4.5.0/workos/resources/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/sso.py` & `workos-4.5.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/user_management.py` & `workos-4.5.0/workos/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/utils/connection_types.py` & `workos-4.5.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/utils/request.py` & `workos-4.5.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/utils/validation.py` & `workos-4.5.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos/webhooks.py` & `workos-4.5.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.4.0/workos.egg-info/PKG-INFO` & `workos-4.5.0/workos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.4.0
+Version: 4.5.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.4.0/workos.egg-info/SOURCES.txt` & `workos-4.5.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

