# Comparing `tmp/wawona-1.1.1.tar.gz` & `tmp/wawona-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wawona-1.1.1.tar", last modified: Mon Apr 15 12:38:44 2024, max compression
+gzip compressed data, was "wawona-1.1.2.tar", last modified: Wed May  1 12:32:18 2024, max compression
```

## Comparing `wawona-1.1.1.tar` & `wawona-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.340938 wawona-1.1.1/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.1.1/LICENSE
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-15 12:38:44.339630 wawona-1.1.1/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     4048 2024-04-03 23:20:59.000000 wawona-1.1.1/README.md
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-04-15 12:38:02.000000 wawona-1.1.1/pyproject.toml
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-04-15 12:38:44.341123 wawona-1.1.1/setup.cfg
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.329340 wawona-1.1.1/src/
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.333655 wawona-1.1.1/src/wawona/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.1.1/src/wawona/__init__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.1.1/src/wawona/__main__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)    19567 2024-04-12 12:10:20.000000 wawona-1.1.1/src/wawona/wawona.py
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.338262 wawona-1.1.1/src/wawona.egg-info/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/SOURCES.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/dependency_links.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/entry_points.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/requires.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/top_level.txt
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.289623 wawona-1.1.2/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.1.2/LICENSE
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5112 2024-05-01 12:32:18.288014 wawona-1.1.2/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     4073 2024-04-25 12:25:34.000000 wawona-1.1.2/README.md
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-05-01 12:31:27.000000 wawona-1.1.2/pyproject.toml
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-05-01 12:32:18.298871 wawona-1.1.2/setup.cfg
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.246239 wawona-1.1.2/src/
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.264372 wawona-1.1.2/src/wawona/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.1.2/src/wawona/__init__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.1.2/src/wawona/__main__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)    19794 2024-04-25 12:22:33.000000 wawona-1.1.2/src/wawona/wawona.py
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.286066 wawona-1.1.2/src/wawona.egg-info/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5112 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/SOURCES.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/dependency_links.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/entry_points.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/requires.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/top_level.txt
```

### Comparing `wawona-1.1.1/LICENSE` & `wawona-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wawona-1.1.1/PKG-INFO` & `wawona-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.1.1
+Version: 1.1.2
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
@@ -144,12 +144,14 @@
 ```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
+- Does not support SSO
 - Uses public endpoints discovered from the web UI
 - No warranty or stability guarantees, could break one day if something changes on their end
 - Password/token is stored in system keychain
-- Add/remove followers using the app. basically if it is not here or it breaks here, use the real app/site.
+- Add/remove followers using the app.
+- Basically if it is not here or it breaks here, use the real app/site.
 - Named for the [drive-thru sequoia](https://en.wikipedia.org/wiki/Wawona_Tree)
```

### Comparing `wawona-1.1.1/README.md` & `wawona-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,12 +119,14 @@
 ```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
+- Does not support SSO
 - Uses public endpoints discovered from the web UI
 - No warranty or stability guarantees, could break one day if something changes on their end
 - Password/token is stored in system keychain
-- Add/remove followers using the app. basically if it is not here or it breaks here, use the real app/site.
+- Add/remove followers using the app.
+- Basically if it is not here or it breaks here, use the real app/site.
 - Named for the [drive-thru sequoia](https://en.wikipedia.org/wiki/Wawona_Tree)
```

### Comparing `wawona-1.1.1/pyproject.toml` & `wawona-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wawona"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="yuzawa-san", email="jtyuzawa@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Easily make office reservations in sequoia from the command line."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `wawona-1.1.1/src/wawona/wawona.py` & `wawona-1.1.2/src/wawona/wawona.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,38 +47,43 @@
     pass
 
 
 def api_call(method, url, **kwargs):
     if VERBOSE:
         print("API REQUEST: %s %s %s %s" % (method, url, kwargs.get("headers"), kwargs.get("json")))
     response = requests.request(method, url, **kwargs)
-    response_json = response.json()
-    if response.status_code == 400 and not response_json.get("success"):
-        raise ApiException(response_json.get("message"))
-    if response.status_code != 200:
-        raise ApiException("%s %s %s %s %s" % (method, url, kwargs.get("headers"), response, response.json()))
+    status_code = response.status_code
+    response_headers = response.headers
+    content_type = response_headers.get('Content-Type') or ''
+    response_json = {}
+    if content_type.startswith('application/json'):
+        response_json = response.json()
     if VERBOSE:
-        print("API RESPONSE: %s %s" % (response, response.json()))
-    return response
+        print("API RESPONSE: %s %s %s" % (status_code, response_headers, response_json))
+    if status_code != 200:
+        if status_code == 400 and not response_json.get("success"):
+            raise ApiException(response_json.get("message"))
+        raise ApiException("%s %s %s %s %s %s" %
+                           (method, url, kwargs.get("headers"), status_code, response_headers, response_json))
+    return response_json
 
 
 def get_token(config, refresh=False):
     email = config["email"]
     token = keyring.get_password(KEYRING_TOKEN, email)
     if token and not refresh:
         return token
     api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/v1/contacts/verify-email", headers=HEADERS,
              json={"email": email})
     password = keyring.get_password(KEYRING_EMAIL, email)
     if not password:
         password = inquirer.password(message='Password')
-    response = api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login", headers=HEADERS,
-                        json={"email": email, "password": password, "browserHash": BROWSER_HASH,
-                              "userType": "employee"})
-    login_json = response.json()
+    login_json = api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login", headers=HEADERS,
+                          json={"email": email, "password": password, "browserHash": BROWSER_HASH,
+                                "userType": "employee"})
     login_data = login_json["data"]
     user_details = login_data["userDetails"]
     token = user_details["apiToken"]
     okta_status = user_details["oktaStatus"]
     if okta_status == "MFA_CHALLENGE":
         factors = login_data.get("factors")
         if factors:
@@ -163,15 +168,15 @@
     headers.update(HEADERS)
     return headers
 
 
 def get_locations(token):
     response = api_call(
         method='GET', url="https://hrx-backend.sequoia.com/rtw/resv/client/locations", headers=token_headers(token))
-    return [(x["locationName"], x) for x in response.json()["data"]["locations"]]
+    return [(x["locationName"], x) for x in response["data"]["locations"]]
 
 
 def format_date(dt):
     return "%02d-%02d-%d" % (dt.day, dt.month, dt.year)
 
 
 def parse_date(dt):
@@ -180,25 +185,25 @@
 
 
 def get_summary(token, start, end):
     response = api_call(method='GET',
                         url="https://hrx-backend.sequoia.com/rtw/client/dashboard/summary?statStart=%s&statEnd=%s" % (
                             format_date(start), format_date(end)), headers=token_headers(token))
     out = set()
-    for stat in response.json()["data"]["weeklyStats"]:
+    for stat in response["data"]["weeklyStats"]:
         out.add(parse_date(stat["date"]))
     return out
 
 
 def get_followings(token, start, end):
     response = api_call(method='GET',
                         url="https://hrx-backend.sequoia.com/rtw/client/followings?startDate=%s&endDate=%s" % (
                             format_date(start), format_date(end)), headers=token_headers(token))
     out = []
-    followings = response.json()["data"]["followings"]
+    followings = response["data"]["followings"]
     if not followings:
         print("You are not following any coworkers.\n"
               "Add them in https://px.sequoia.com/workplace or the app, and they will appear calendar below.")
     for user in followings:
         name = user["fullName"]
         reservations = user.get("reservationsMetadata", [])
         days = set()
@@ -267,51 +272,52 @@
         raise Exception("No choice")
     return answers['choice']
 
 
 def get_pending_tasks(token):
     response = api_call(method='GET', url="https://hrx-backend.sequoia.com/rtw/client/pending-task",
                         headers=token_headers(token))
-    return [x["taskId"] for x in response.json()["data"]["tasks"]]
+    return [x["taskId"] for x in response["data"]["tasks"]]
 
 
 def get_task(token, task_id):
-    response = api_call(method='GET', url="https://hrx-backend.sequoia.com/rtw/client/task/info?taskId=%s" % task_id,
+    response = api_call(method='GET',
+                        url="https://hrx-backend.sequoia.com/rtw/client/task/info?taskId=%s" % task_id,
                         headers=token_headers(token))
-    return response.json()["data"]
+    return response["data"]
 
 
 def respond_to_task(token, task_id, answers):
     api_call(method='POST', url="https://hrx-backend.sequoia.com/rtw/client/task-response",
              headers=token_headers(token),
              json={"taskId": task_id, "response": answers})
 
 
 def get_floors(token, task_id):
     response = api_call(
         method='GET', url="https://hrx-backend.sequoia.com/rtw/client/space-bookings/floors?taskId=%s" % task_id,
         headers=token_headers(token))
-    return [(x["floorName"], x["floorId"]) for x in response.json()["data"]["floors"] if x["status"] == "active"]
+    return [(x["floorName"], x["floorId"]) for x in response["data"]["floors"] if x["status"] == "active"]
 
 
 def get_spaces(token, adjective, task_id, floor_id, start_time, end_time):
     url = ("https://hrx-backend.sequoia.com/rtw/client/space-bookings/%s/spaces?taskId=%s&floorId=%s&startTime=%s"
            "&endTime=%s") % (
               adjective, task_id, floor_id, start_time, end_time)
     response = api_call(method='GET', url=url, headers=token_headers(token))
-    return response.json()["data"]["spaces"]
+    return response["data"]["spaces"]
 
 
 def reserve_space(token, task_id, start_time, end_time, space_id, user_id, reservation_id):
     response = api_call(method='POST', url="https://hrx-backend.sequoia.com/rtw/client/space-bookings/space",
                         headers=token_headers(token),
                         json={"taskId": task_id, "startTime": start_time, "endTime": end_time, "spaceId": space_id,
                               "userId": user_id, "reservationId": reservation_id}
                         )
-    return response.json()["data"]["label"]
+    return response["data"]["label"]
 
 
 def get_space(token, task, floor_id, config):
     task_id = task["taskId"]
     start_time = task["reservationStartTime"]
     end_time = task["reservationEndTime"]
     available_spaces = get_spaces(token, "available", task_id, floor_id, start_time, end_time)
```

### Comparing `wawona-1.1.1/src/wawona.egg-info/PKG-INFO` & `wawona-1.1.2/src/wawona.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.1.1
+Version: 1.1.2
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
@@ -144,12 +144,14 @@
 ```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
+- Does not support SSO
 - Uses public endpoints discovered from the web UI
 - No warranty or stability guarantees, could break one day if something changes on their end
 - Password/token is stored in system keychain
-- Add/remove followers using the app. basically if it is not here or it breaks here, use the real app/site.
+- Add/remove followers using the app.
+- Basically if it is not here or it breaks here, use the real app/site.
 - Named for the [drive-thru sequoia](https://en.wikipedia.org/wiki/Wawona_Tree)
```

