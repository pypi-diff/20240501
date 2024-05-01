# Comparing `tmp/mwcleric-0.9.5.tar.gz` & `tmp/mwcleric-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwcleric-0.9.5.tar", last modified: Tue Feb 27 21:15:17 2024, max compression
+gzip compressed data, was "mwcleric-0.9.6.tar", last modified: Wed May  1 03:45:27 2024, max compression
```

## Comparing `mwcleric-0.9.5.tar` & `mwcleric-0.9.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 21:15:17.766112 mwcleric-0.9.5/
--rw-rw-rw-   0        0        0     1099 2021-03-18 12:29:46.000000 mwcleric-0.9.5/LICENSE
--rw-rw-rw-   0        0        0     7713 2024-02-27 21:15:17.766112 mwcleric-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     7328 2021-11-23 18:11:06.000000 mwcleric-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 21:15:17.738112 mwcleric-0.9.5/mwcleric/
--rw-rw-rw-   0        0        0      305 2024-02-27 20:51:00.000000 mwcleric-0.9.5/mwcleric/__init__.py
--rw-rw-rw-   0        0        0     5096 2024-02-27 20:55:38.000000 mwcleric-0.9.5/mwcleric/auth_credentials.py
-drwxrwxrwx   0        0        0        0 2024-02-27 21:15:17.762112 mwcleric-0.9.5/mwcleric/clients/
--rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/clients/__init__.py
--rw-rw-rw-   0        0        0     3774 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/clients/cargo_client.py
--rw-rw-rw-   0        0        0      990 2022-03-03 08:58:57.000000 mwcleric-0.9.5/mwcleric/clients/session_manager.py
--rw-rw-rw-   0        0        0      162 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/clients/site.py
--rw-rw-rw-   0        0        0      738 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/errors.py
--rw-rw-rw-   0        0        0     3269 2024-02-10 10:12:09.000000 mwcleric-0.9.5/mwcleric/fandom_client.py
-drwxrwxrwx   0        0        0        0 2024-02-27 21:15:17.764113 mwcleric-0.9.5/mwcleric/models/
--rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-27 21:15:17.765112 mwcleric-0.9.5/mwcleric/models/logs/
--rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/models/logs/__init__.py
--rw-rw-rw-   0        0        0      378 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/models/logs/log_entry.py
--rw-rw-rw-   0        0        0      321 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/models/logs/move_log_entry.py
--rw-rw-rw-   0        0        0      281 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/models/namespace.py
--rw-rw-rw-   0        0        0      264 2021-09-08 08:49:52.000000 mwcleric-0.9.5/mwcleric/models/simple_page.py
--rw-rw-rw-   0        0        0     5150 2021-11-23 13:12:06.000000 mwcleric-0.9.5/mwcleric/page_modifier.py
--rw-rw-rw-   0        0        0     4156 2022-06-08 23:33:03.000000 mwcleric-0.9.5/mwcleric/template_modifier.py
--rw-rw-rw-   0        0        0    23375 2024-02-10 10:12:09.000000 mwcleric-0.9.5/mwcleric/wiki_client.py
--rw-rw-rw-   0        0        0     1493 2024-02-27 21:14:54.000000 mwcleric-0.9.5/mwcleric/wikigg_client.py
-drwxrwxrwx   0        0        0        0 2024-02-27 21:15:17.765112 mwcleric-0.9.5/mwcleric.egg-info/
--rw-rw-rw-   0        0        0     7713 2024-02-27 21:15:17.000000 mwcleric-0.9.5/mwcleric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2024-02-27 21:15:17.000000 mwcleric-0.9.5/mwcleric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 21:15:17.000000 mwcleric-0.9.5/mwcleric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-02-27 21:15:17.000000 mwcleric-0.9.5/mwcleric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-27 21:15:17.000000 mwcleric-0.9.5/mwcleric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2021-03-18 13:18:35.000000 mwcleric-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-27 21:15:17.767112 mwcleric-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0      578 2024-02-27 21:15:03.000000 mwcleric-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.064736 mwcleric-0.9.6/
+-rw-rw-rw-   0        0        0     1099 2021-03-18 12:29:46.000000 mwcleric-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0     7715 2024-05-01 03:45:27.064736 mwcleric-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7330 2024-04-29 09:37:18.000000 mwcleric-0.9.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.010733 mwcleric-0.9.6/mwcleric/
+-rw-rw-rw-   0        0        0      305 2024-02-27 20:51:00.000000 mwcleric-0.9.6/mwcleric/__init__.py
+-rw-rw-rw-   0        0        0     6243 2024-04-29 12:24:58.000000 mwcleric-0.9.6/mwcleric/auth_credentials.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.043734 mwcleric-0.9.6/mwcleric/clients/
+-rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/clients/__init__.py
+-rw-rw-rw-   0        0        0     3774 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/clients/cargo_client.py
+-rw-rw-rw-   0        0        0      990 2022-03-03 08:58:57.000000 mwcleric-0.9.6/mwcleric/clients/session_manager.py
+-rw-rw-rw-   0        0        0      162 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/clients/site.py
+-rw-rw-rw-   0        0        0      738 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/errors.py
+-rw-rw-rw-   0        0        0     3269 2024-02-10 10:12:09.000000 mwcleric-0.9.6/mwcleric/fandom_client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.053733 mwcleric-0.9.6/mwcleric/models/
+-rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.062731 mwcleric-0.9.6/mwcleric/models/logs/
+-rw-rw-rw-   0        0        0        0 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/logs/__init__.py
+-rw-rw-rw-   0        0        0      378 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/logs/log_entry.py
+-rw-rw-rw-   0        0        0      321 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/logs/move_log_entry.py
+-rw-rw-rw-   0        0        0      281 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/namespace.py
+-rw-rw-rw-   0        0        0      264 2021-09-08 08:49:52.000000 mwcleric-0.9.6/mwcleric/models/simple_page.py
+-rw-rw-rw-   0        0        0     5150 2021-11-23 13:12:06.000000 mwcleric-0.9.6/mwcleric/page_modifier.py
+-rw-rw-rw-   0        0        0     4156 2022-06-08 23:33:03.000000 mwcleric-0.9.6/mwcleric/template_modifier.py
+-rw-rw-rw-   0        0        0    23375 2024-02-10 10:12:09.000000 mwcleric-0.9.6/mwcleric/wiki_client.py
+-rw-rw-rw-   0        0        0     1339 2024-04-29 09:39:53.000000 mwcleric-0.9.6/mwcleric/wikigg_client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:45:27.063735 mwcleric-0.9.6/mwcleric.egg-info/
+-rw-rw-rw-   0        0        0     7715 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 03:45:26.000000 mwcleric-0.9.6/mwcleric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2021-03-18 13:18:35.000000 mwcleric-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:45:27.064736 mwcleric-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      578 2024-04-29 09:32:45.000000 mwcleric-0.9.6/setup.py
```

### Comparing `mwcleric-0.9.5/LICENSE` & `mwcleric-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/PKG-INFO` & `mwcleric-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwcleric
-Version: 0.9.5
+Version: 0.9.6
 Summary: River's mwclient wrapper
 Home-page: https://github.com/RheingoldRiver/mwcleric
 Author: RheingoldRiver
 Author-email: river.esports@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 This library can be installed from PyPI:
 ```
 pip install mwcleric
 ```
 
 However, for the most up-to-date version including minor changes you may want to pull directly from the repo if I haven't updated PyPI:
 ```
-pip install -U git+git://github.com/RheingoldRiver/mwcleric
+pip install -U git+https://github.com/RheingoldRiver/mwcleric
 ```
 
 If you're using PyCharm, press Alt+F12 to open the console and you can install directly to your venv or whatever it's using that way.
 
 ## Logging in
 
 Currently, bot passwords are supported; legacy login without bot passwords should also work. If you want to add support for another type of login, I'm happy to merge a PR for it.
```

### Comparing `mwcleric-0.9.5/README.md` & `mwcleric-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This library can be installed from PyPI:
 ```
 pip install mwcleric
 ```
 
 However, for the most up-to-date version including minor changes you may want to pull directly from the repo if I haven't updated PyPI:
 ```
-pip install -U git+git://github.com/RheingoldRiver/mwcleric
+pip install -U git+https://github.com/RheingoldRiver/mwcleric
 ```
 
 If you're using PyCharm, press Alt+F12 to open the console and you can install directly to your venv or whatever it's using that way.
 
 ## Logging in
 
 Currently, bot passwords are supported; legacy login without bot passwords should also work. If you want to add support for another type of login, I'm happy to merge a PR for it.
```

### Comparing `mwcleric-0.9.5/mwcleric/clients/cargo_client.py` & `mwcleric-0.9.6/mwcleric/clients/cargo_client.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/clients/session_manager.py` & `mwcleric-0.9.6/mwcleric/clients/session_manager.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/errors.py` & `mwcleric-0.9.6/mwcleric/errors.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/fandom_client.py` & `mwcleric-0.9.6/mwcleric/fandom_client.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/page_modifier.py` & `mwcleric-0.9.6/mwcleric/page_modifier.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/template_modifier.py` & `mwcleric-0.9.6/mwcleric/template_modifier.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/wiki_client.py` & `mwcleric-0.9.6/mwcleric/wiki_client.py`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/mwcleric/wikigg_client.py` & `mwcleric-0.9.6/mwcleric/wikigg_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,19 +21,16 @@
 
         :param wiki: Name of a wiki
         :param lang: Optional. If the wiki has a language path in the URL, provide it here.
         :param client: Otpional. If this is provided, SessionManager will not be used.
         :param credentials: Optional. Provide if you want a logged-in session.
         """
 
-        url = '{}{}{}{}{}.wiki.gg{}'.format(
-            credentials.site_user if use_site_pw else '',
-            ':' if use_site_pw else '',
-            credentials.site_pw if use_site_pw else '',
-            '@' if use_site_pw else '',
+        url = '{}{}.wiki.gg{}'.format(
+            credentials.site_password_prefix,
             wiki, f"/{lang}" if lang is not None else '')
         path = '/'
         super().__init__(url=url, path=path, credentials=credentials, client=client, **kwargs)
 
         self.cargo_client = CargoClient(self.client)
 
     def relog(self):
```

### Comparing `mwcleric-0.9.5/mwcleric.egg-info/PKG-INFO` & `mwcleric-0.9.6/mwcleric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwcleric
-Version: 0.9.5
+Version: 0.9.6
 Summary: River's mwclient wrapper
 Home-page: https://github.com/RheingoldRiver/mwcleric
 Author: RheingoldRiver
 Author-email: river.esports@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 This library can be installed from PyPI:
 ```
 pip install mwcleric
 ```
 
 However, for the most up-to-date version including minor changes you may want to pull directly from the repo if I haven't updated PyPI:
 ```
-pip install -U git+git://github.com/RheingoldRiver/mwcleric
+pip install -U git+https://github.com/RheingoldRiver/mwcleric
 ```
 
 If you're using PyCharm, press Alt+F12 to open the console and you can install directly to your venv or whatever it's using that way.
 
 ## Logging in
 
 Currently, bot passwords are supported; legacy login without bot passwords should also work. If you want to add support for another type of login, I'm happy to merge a PR for it.
```

### Comparing `mwcleric-0.9.5/mwcleric.egg-info/SOURCES.txt` & `mwcleric-0.9.6/mwcleric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwcleric-0.9.5/setup.py` & `mwcleric-0.9.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 setuptools.setup(
     name="mwcleric",
     version=__version__,
     author="RheingoldRiver",
     author_email="river.esports@gmail.com",
     description="River's mwclient wrapper",
```

