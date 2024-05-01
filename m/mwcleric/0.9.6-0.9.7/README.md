# Comparing `tmp/mwcleric-0.9.6.tar.gz` & `tmp/mwcleric-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwcleric-0.9.6.tar", last modified: Wed May  1 03:45:27 2024, max compression
+gzip compressed data, was "mwcleric-0.9.7.tar", last modified: Wed May  1 09:47:17 2024, max compression
```

## Comparing `mwcleric-0.9.6.tar` & `mwcleric-0.9.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.064736 mwcleric-0.9.6/
--rw-rw-rw-   0        0        0     1099 2021-03-18 12:29:46.000000 mwcleric-0.9.6/LICENSE
--rw-rw-rw-   0        0        0     7715 2024-05-01 03:45:27.064736 mwcleric-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     7330 2024-04-29 09:37:18.000000 mwcleric-0.9.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.010733 mwcleric-0.9.6/mwcleric/
--rw-rw-rw-   0        0        0      305 2024-02-27 20:51:00.000000 mwcleric-0.9.6/mwcleric/__init__.py
--rw-rw-rw-   0        0        0     6243 2024-04-29 12:24:58.000000 mwcleric-0.9.6/mwcleric/auth_credentials.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.043734 mwcleric-0.9.6/mwcleric/clients/
--rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/clients/__init__.py
--rw-rw-rw-   0        0        0     3774 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/clients/cargo_client.py
--rw-rw-rw-   0        0        0      990 2022-03-03 08:58:57.000000 mwcleric-0.9.6/mwcleric/clients/session_manager.py
--rw-rw-rw-   0        0        0      162 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/clients/site.py
--rw-rw-rw-   0        0        0      738 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/errors.py
--rw-rw-rw-   0        0        0     3269 2024-02-10 10:12:09.000000 mwcleric-0.9.6/mwcleric/fandom_client.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.053733 mwcleric-0.9.6/mwcleric/models/
--rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.062731 mwcleric-0.9.6/mwcleric/models/logs/
--rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/logs/__init__.py
--rw-rw-rw-   0        0        0      378 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/logs/log_entry.py
--rw-rw-rw-   0        0        0      321 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/logs/move_log_entry.py
--rw-rw-rw-   0        0        0      281 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/namespace.py
--rw-rw-rw-   0        0        0      264 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/simple_page.py
--rw-rw-rw-   0        0        0     5150 2021-11-23 13:12:06.000000 mwcleric-0.9.6/mwcleric/page_modifier.py
--rw-rw-rw-   0        0        0     4156 2022-06-08 23:33:03.000000 mwcleric-0.9.6/mwcleric/template_modifier.py
--rw-rw-rw-   0        0        0    23375 2024-02-10 10:12:09.000000 mwcleric-0.9.6/mwcleric/wiki_client.py
--rw-rw-rw-   0        0        0     1339 2024-04-29 09:39:53.000000 mwcleric-0.9.6/mwcleric/wikigg_client.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.063735 mwcleric-0.9.6/mwcleric.egg-info/
--rw-rw-rw-   0        0        0     7715 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2021-03-18 13:18:35.000000 mwcleric-0.9.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 03:45:27.064736 mwcleric-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      578 2024-04-29 09:32:45.000000 mwcleric-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:47:17.137312 mwcleric-0.9.7/
+-rw-rw-rw-   0        0        0     1099 2021-03-18 12:29:46.000000 mwcleric-0.9.7/LICENSE
+-rw-rw-rw-   0        0        0     7715 2024-05-01 09:47:17.137312 mwcleric-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7330 2024-04-29 09:37:18.000000 mwcleric-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 09:47:17.110312 mwcleric-0.9.7/mwcleric/
+-rw-rw-rw-   0        0        0      305 2024-02-27 20:51:00.000000 mwcleric-0.9.7/mwcleric/__init__.py
+-rw-rw-rw-   0        0        0     6243 2024-04-29 12:24:58.000000 mwcleric-0.9.7/mwcleric/auth_credentials.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:47:17.133312 mwcleric-0.9.7/mwcleric/clients/
+-rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/clients/__init__.py
+-rw-rw-rw-   0        0        0     3774 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/clients/cargo_client.py
+-rw-rw-rw-   0        0        0      990 2022-03-03 08:58:57.000000 mwcleric-0.9.7/mwcleric/clients/session_manager.py
+-rw-rw-rw-   0        0        0      162 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/clients/site.py
+-rw-rw-rw-   0        0        0      738 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/errors.py
+-rw-rw-rw-   0        0        0     3269 2024-02-10 10:12:09.000000 mwcleric-0.9.7/mwcleric/fandom_client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:47:17.134312 mwcleric-0.9.7/mwcleric/models/
+-rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:47:17.136312 mwcleric-0.9.7/mwcleric/models/logs/
+-rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/models/logs/__init__.py
+-rw-rw-rw-   0        0        0      378 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/models/logs/log_entry.py
+-rw-rw-rw-   0        0        0      321 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/models/logs/move_log_entry.py
+-rw-rw-rw-   0        0        0      281 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/models/namespace.py
+-rw-rw-rw-   0        0        0      264 2021-09-08 08:49:52.000000 mwcleric-0.9.7/mwcleric/models/simple_page.py
+-rw-rw-rw-   0        0        0     5150 2021-11-23 13:12:06.000000 mwcleric-0.9.7/mwcleric/page_modifier.py
+-rw-rw-rw-   0        0        0     4156 2022-06-08 23:33:03.000000 mwcleric-0.9.7/mwcleric/template_modifier.py
+-rw-rw-rw-   0        0        0    24131 2024-05-01 09:46:19.000000 mwcleric-0.9.7/mwcleric/wiki_client.py
+-rw-rw-rw-   0        0        0     1339 2024-04-29 09:39:53.000000 mwcleric-0.9.7/mwcleric/wikigg_client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:47:17.136312 mwcleric-0.9.7/mwcleric.egg-info/
+-rw-rw-rw-   0        0        0     7715 2024-05-01 09:47:17.000000 mwcleric-0.9.7/mwcleric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-05-01 09:47:17.000000 mwcleric-0.9.7/mwcleric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 09:47:17.000000 mwcleric-0.9.7/mwcleric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-01 09:47:17.000000 mwcleric-0.9.7/mwcleric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 09:47:17.000000 mwcleric-0.9.7/mwcleric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2021-03-18 13:18:35.000000 mwcleric-0.9.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 09:47:17.137312 mwcleric-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      578 2024-05-01 09:38:43.000000 mwcleric-0.9.7/setup.py
```

### Comparing `mwcleric-0.9.6/LICENSE` & `mwcleric-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/PKG-INFO` & `mwcleric-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwcleric
-Version: 0.9.6
+Version: 0.9.7
 Summary: River's mwclient wrapper
 Home-page: https://github.com/RheingoldRiver/mwcleric
 Author: RheingoldRiver
 Author-email: river.esports@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mwcleric-0.9.6/README.md` & `mwcleric-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/auth_credentials.py` & `mwcleric-0.9.7/mwcleric/auth_credentials.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/clients/cargo_client.py` & `mwcleric-0.9.7/mwcleric/clients/cargo_client.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/clients/session_manager.py` & `mwcleric-0.9.7/mwcleric/clients/session_manager.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/errors.py` & `mwcleric-0.9.7/mwcleric/errors.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/fandom_client.py` & `mwcleric-0.9.7/mwcleric/fandom_client.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/page_modifier.py` & `mwcleric-0.9.7/mwcleric/page_modifier.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/template_modifier.py` & `mwcleric-0.9.7/mwcleric/template_modifier.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric/wiki_client.py` & `mwcleric-0.9.7/mwcleric/wiki_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,34 @@
                 raise e
 
     def _retry_move(self, **kwargs):
         # token is mandatory
         token = kwargs.pop('token')
         self.client.api('move', token=token, **kwargs)
 
+    def protect(self, page: Page, protections="edit=sysop|move=sysop", expiry="infinite", reason=None, **data):
+        data.update({
+            'title': page.name,
+            'protections': protections,
+            'expiry': expiry,
+            'reason': reason,
+        })
+        protect_token = self.client.get_token('csrf')
+        try:
+            self.client.api('protect', **data, token=protect_token)
+        except APIError as e:
+            if e.code == 'badtoken':
+                self._retry_login_action(self._retry_protect, 'move', **data, token=protect_token)
+            else:
+                raise e
+
+    def _retry_protect(self, **kwargs):
+        token = kwargs.pop('token')
+        self.client.api('protect', token=token, **kwargs)
+
     def delete(self, page: Page, reason='', watch=False, unwatch=False, oldimage=False):
         try:
             page.site = self.client
             page.delete(reason=reason, watch=watch, unwatch=unwatch, oldimage=oldimage)
         except APIError as e:
             if e.code == 'badtoken':
                 self._retry_login_action(self._retry_delete, 'delete', page=page, reason=reason,
```

### Comparing `mwcleric-0.9.6/mwcleric/wikigg_client.py` & `mwcleric-0.9.7/mwcleric/wikigg_client.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/mwcleric.egg-info/PKG-INFO` & `mwcleric-0.9.7/mwcleric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwcleric
-Version: 0.9.6
+Version: 0.9.7
 Summary: River's mwclient wrapper
 Home-page: https://github.com/RheingoldRiver/mwcleric
 Author: RheingoldRiver
 Author-email: river.esports@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mwcleric-0.9.6/mwcleric.egg-info/SOURCES.txt` & `mwcleric-0.9.7/mwcleric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.6/setup.py` & `mwcleric-0.9.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "0.9.6"
+__version__ = "0.9.7"
 
 setuptools.setup(
     name="mwcleric",
     version=__version__,
     author="RheingoldRiver",
     author_email="river.esports@gmail.com",
     description="River's mwclient wrapper",
```

