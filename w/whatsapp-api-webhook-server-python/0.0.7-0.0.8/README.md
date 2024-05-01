# Comparing `tmp/whatsapp-api-webhook-server-python-0.0.7.tar.gz` & `tmp/whatsapp_api_webhook_server_python-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-webhook-server-python-0.0.7.tar", last modified: Mon Jun 12 14:57:23 2023, max compression
+gzip compressed data, was "whatsapp_api_webhook_server_python-0.0.8.tar", last modified: Wed May  1 08:25:16 2024, max compression
```

## Comparing `whatsapp-api-webhook-server-python-0.0.7.tar` & `whatsapp_api_webhook_server_python-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.663206 whatsapp-api-webhook-server-python-0.0.7/
--rw-rw-rw-   0        0        0    18829 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     7921 2023-06-12 14:57:23.663206 whatsapp-api-webhook-server-python-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6847 2023-06-12 14:52:42.000000 whatsapp-api-webhook-server-python-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 14:57:23.663206 whatsapp-api-webhook-server-python-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-06-12 14:52:42.000000 whatsapp-api-webhook-server-python-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.656187 whatsapp-api-webhook-server-python-0.0.7/tests/
--rw-rw-rw-   0        0        0      518 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/tests/test_main.py
--rw-rw-rw-   0        0        0      204 2023-06-04 08:13:40.000000 whatsapp-api-webhook-server-python-0.0.7/tests/test_methods.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.658193 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/
--rw-rw-rw-   0        0        0        0 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/__init__.py
--rw-rw-rw-   0        0        0      255 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/webhooks.py
--rw-rw-rw-   0        0        0     1643 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/webhooksHandler.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.662203 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/
--rw-rw-rw-   0        0        0     7921 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 08:25:16.159289 whatsapp_api_webhook_server_python-0.0.8/
+-rw-rw-rw-   0        0        0    18829 2024-05-01 07:39:10.000000 whatsapp_api_webhook_server_python-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9344 2024-05-01 08:25:16.158290 whatsapp_api_webhook_server_python-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7776 2024-05-01 07:39:10.000000 whatsapp_api_webhook_server_python-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 08:25:16.159289 whatsapp_api_webhook_server_python-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1899 2024-05-01 08:00:50.000000 whatsapp_api_webhook_server_python-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:25:16.151288 whatsapp_api_webhook_server_python-0.0.8/tests/
+-rw-rw-rw-   0        0        0      294 2024-05-01 07:39:10.000000 whatsapp_api_webhook_server_python-0.0.8/tests/test_server.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:25:16.153288 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python/
+-rw-rw-rw-   0        0        0        0 2024-05-01 07:39:10.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python/__init__.py
+-rw-rw-rw-   0        0        0      411 2024-05-01 07:39:10.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python/webhooks.py
+-rw-rw-rw-   0        0        0     1328 2024-05-01 07:39:10.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python/webhooksHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:25:16.158290 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python.egg-info/
+-rw-rw-rw-   0        0        0     9344 2024-05-01 08:25:16.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-05-01 08:25:16.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 08:25:16.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 08:25:16.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-05-01 08:25:16.000000 whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-webhook-server-python-0.0.7/LICENSE` & `whatsapp_api_webhook_server_python-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-api-webhook-server-python-0.0.7/PKG-INFO` & `whatsapp_api_webhook_server_python-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-Metadata-Version: 2.1
-Name: whatsapp-api-webhook-server-python
-Version: 0.0.7
-Summary: This library helps you easily create a Python server endpoint to receive WhatsApp message webhooks.
-Home-page: https://github.com/green-api/whatsapp-api-webhook-server-python
-Author: GREEN API
-Author-email: support@green-api.com
-License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # whatsapp-api-webhook-server-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-api-webhook-server-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-api-webhook-server-python)
-![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-webhook-server-python/python-app.yml)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-webhook-server-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-api-webhook-server-python)
 
+## Support links
+
+[![Support](https://img.shields.io/badge/support@green--api.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:support@greenapi.com)
+[![Support](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/greenapi_support_eng_bot)
+[![Support](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/77273122366)
+
+## Guides & News
+
+[![Guides](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/@greenapi-en)
+[![News](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/green_api)
+[![News](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://whatsapp.com/channel/0029VaLj6J4LNSa2B5Jx6s3h)
+
 - [Документация на русском языке](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/docs/README_RU.md).
 
 whatsapp-api-webhook-server-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
```

### Comparing `whatsapp-api-webhook-server-python-0.0.7/setup.py` & `whatsapp_api_webhook_server_python-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,49 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-api-webhook-server-python",
-    version="0.0.7",
+    version="0.0.8",
     description=(
         "This library helps you easily create"
-        " a Python server endpoint to receive WhatsApp message webhooks."
+        " a Python server endpoint to receive"
+        " WhatsApp message webhooks."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
     author_email="support@green-api.com",
     url="https://github.com/green-api/whatsapp-api-webhook-server-python",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
+        "Natural Language :: English",
+        "Natural Language :: Russian",
         "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Topic :: Communications",
+        "Topic :: Communications :: Chat",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["tornado==6.3.2"],
+    install_requires=["tornado>=6.2"],
     python_requires=">=3.7"
 )
```

### Comparing `whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/webhooksHandler.py` & `whatsapp_api_webhook_server_python-0.0.8/whatsapp_api_webhook_server_python/webhooksHandler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 import tornado.ioloop
 import tornado.web
 
-from whatsapp_api_webhook_server_python.webhooks import Webhooks
+from .webhooks import handle_notification
 
 
 class WebhooksHandler(tornado.web.RequestHandler):
-
     def get(self):
         length = self.request.headers.get('Content-Length')
-        if length != None:
-            dataBytes = self.request.body
-            dataText = dataBytes.decode("utf-8", 'ignore')
-            Webhooks.webhookProccessing(dataText, self.onEvent)
+        if length is not None:
+            handle_notification(self.request.body, self.onEvent)
         else:
             self.set_status(200)
             self.set_header('Content-type', 'text/html')
 
     def post(self):
         length = self.request.headers.get('Content-Length')
-        if length != None:
-            dataBytes = self.request.body
-            dataText = dataBytes.decode("utf-8", 'ignore')
-            Webhooks.webhookProccessing(dataText, self.onEvent)
+        if length is not None:
+            handle_notification(self.request.body, self.onEvent)
 
     def delete(self):
         length = self.request.headers.get('Content-Length')
-        if length != None:
-            dataBytes = self.request.body
-            dataText = dataBytes.decode("utf-8", 'ignore')
-            Webhooks.webhookProccessing(dataText, self.onEvent)
-  
+        if length is not None:
+            handle_notification(self.request.body, self.onEvent)
+
+
 class Application(tornado.web.Application):
     def __init__(self, handler):
         handlers = [
             (r"/", handler),
         ]
         tornado.web.Application.__init__(self, handlers)
 
+
 def startServer(host: str, port: int, onEvent, startLoop: bool = True):
     handler = WebhooksHandler
     handler.onEvent = onEvent
     http_server = tornado.httpserver.HTTPServer(Application(handler))
     http_server.listen(port=port, address=host)
     if startLoop:
-        tornado.ioloop.IOLoop.instance().start()
+        tornado.ioloop.IOLoop.instance().start()
```

### Comparing `whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/PKG-INFO` & `whatsapp_api_webhook_server_python-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,61 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-webhook-server-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: This library helps you easily create a Python server endpoint to receive WhatsApp message webhooks.
 Home-page: https://github.com/green-api/whatsapp-api-webhook-server-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tornado>=6.2
 
 # whatsapp-api-webhook-server-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-api-webhook-server-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-api-webhook-server-python)
-![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-webhook-server-python/python-app.yml)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-webhook-server-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-api-webhook-server-python)
 
+## Support links
+
+[![Support](https://img.shields.io/badge/support@green--api.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:support@greenapi.com)
+[![Support](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/greenapi_support_eng_bot)
+[![Support](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/77273122366)
+
+## Guides & News
+
+[![Guides](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/@greenapi-en)
+[![News](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/green_api)
+[![News](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://whatsapp.com/channel/0029VaLj6J4LNSa2B5Jx6s3h)
+
 - [Документация на русском языке](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/docs/README_RU.md).
 
 whatsapp-api-webhook-server-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
```

