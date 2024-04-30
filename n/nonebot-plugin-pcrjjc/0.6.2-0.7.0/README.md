# Comparing `tmp/nonebot-plugin-pcrjjc-0.6.2.tar.gz` & `tmp/nonebot_plugin_pcrjjc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-pcrjjc-0.6.2.tar", last modified: Fri Jan  5 03:15:27 2024, max compression
+gzip compressed data, was "nonebot_plugin_pcrjjc-0.7.0.tar", last modified: Tue Apr 30 23:50:06 2024, max compression
```

## Comparing `nonebot-plugin-pcrjjc-0.6.2.tar` & `nonebot_plugin_pcrjjc-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 03:15:27.992185 nonebot-plugin-pcrjjc-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-05 03:15:27.992185 nonebot-plugin-pcrjjc-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 03:15:27.992185 nonebot-plugin-pcrjjc-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 03:15:27.988185 nonebot-plugin-pcrjjc-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 03:15:27.988185 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/
--rw-r--r--   0 runner    (1001) docker     (127)    40093 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-01-05 03:15:14.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/text2img.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 03:15:27.988185 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-05 03:15:27.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-05 03:15:27.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 03:15:27.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-05 03:15:27.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-05 03:15:27.000000 nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/
+-rw-r--r--   0 runner    (1001) docker     (127)    40026 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-30 23:49:53.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/text2img.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:50:06.215087 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 23:50:06.000000 nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/LICENSE` & `nonebot_plugin_pcrjjc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.6.2/PKG-INFO` & `nonebot_plugin_pcrjjc-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.6.2
+Version: 0.7.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -15,15 +15,15 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack>=1.0.5
 Requires-Dist: requests>=2.30.0
 Requires-Dist: Pillow>=9.5.0
-Requires-Dist: pydantic>=1.10.9
+Requires-Dist: pydantic>=2
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pycryptodome>=3.18.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.3
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
 
 # nonebot-plugin-pcrjjc
@@ -81,20 +81,16 @@
 
 登录账号（即PCR_ACCOUNTS）模板
 
 ```python
 PCRJJC_ACCOUNTS='[
     {
      "account": "account1",
-     "password": "password",
-     "platform": 2,
-     "channel": 1
+     "password": "password"
     },
     {
      "account": "account2",
-     "password": "password",
-     "platform": 2,
-     "channel": 1
+     "password": "password"
     }
 ]'
 ```
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/README.md` & `nonebot_plugin_pcrjjc-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,20 +53,16 @@
 
 登录账号（即PCR_ACCOUNTS）模板
 
 ```python
 PCRJJC_ACCOUNTS='[
     {
      "account": "account1",
-     "password": "password",
-     "platform": 2,
-     "channel": 1
+     "password": "password"
     },
     {
      "account": "account2",
-     "password": "password",
-     "platform": 2,
-     "channel": 1
+     "password": "password"
     }
 ]'
 ```
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/pyproject.toml` & `nonebot_plugin_pcrjjc-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.6.2"
+version = "0.7.0"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
 dependencies = [
     "msgpack>=1.0.5",
     "requests>=2.30.0",
     "Pillow>=9.5.0",
-    "pydantic>=1.10.9",
+    "pydantic>=2",
     "python-dateutil>=2.8.2",
     "pycryptodome>=3.18.0",
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-plugin-apscheduler>=0.3.0"
 ]
 classifiers = [
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/__init__.py` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,35 +25,33 @@
     GroupDecreaseNoticeEvent
 )
 from nonebot.internal.matcher import Matcher
 from nonebot.params import RegexGroup
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
 
-from .config import Config
-from .pcrclient import ApiException
+from .config import config, Config
 from .query import queue, path
 from .text2img import image_draw
 
 require("nonebot_plugin_apscheduler")
 
-from nonebot_plugin_apscheduler import scheduler
+from nonebot_plugin_apscheduler import scheduler  
 
 __plugin_meta__ = PluginMetadata(
     name="pcrjjc",
     config=Config,
     description="公主连结（国服）排名监测工具",
     usage="发送 竞技场帮助 获取详细使用说明",
     type="application",
     homepage="https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc",
     supported_adapters={"~onebot.v11"}
 )
 
 driver = get_driver()
-config = Config.parse_obj(driver.config)
 
 MAX_PRI = config.max_pri
 MAX_PCRID = config.max_pcrid
 MAX_HISTORY = config.max_history
 NOTICE_CD_MIN = config.notice_cd_min
 REFRESH_SECOND = config.refresh_second
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,100 @@
 from asyncio import sleep
 from base64 import b64encode, b64decode
 from datetime import datetime
 from hashlib import md5
 from json import loads
-from os.path import join, exists
+from os.path import join
 from pathlib import Path
 from random import randint
 from re import search
 
 from Crypto.Cipher import AES
 from dateutil.parser import parse
 from msgpack import packb, unpackb
 from nonebot import logger, get_driver
 
 from .aiorequests import post
 from .bsgamesdk import login
-from .config import Config
+from .config import config
 
 driver = get_driver()
-config = Config.parse_obj(driver.config)
 
-api_root = 'https://le1-prod-all-gs-gzlj.bilibiligame.net'
+api_root = "https://le1-prod-all-gs-gzlj.bilibiligame.net"
 debugging = 1
 
 data_path = config.data_path
 path = join(str(Path()), data_path)
-version_txt = join(path, 'version.txt')
-version = config.version
+# version_txt = join(path, 'version.txt')
+version = "0.0.0"
 
-if exists(version_txt):
-    with open(version_txt, encoding='utf-8') as fp:
-        version = fp.read().strip()
+# if exists(version_txt):
+#     with open(version_txt, encoding='utf-8') as fp:
+#         version = fp.read().strip()
 
 defaultHeaders = {
-    'Accept-Encoding': 'gzip',
-    'User-Agent': 'Dalvik/2.1.0 (Linux, U, Android 5.1.1, PCRT00 Build/LMY48Z)',
-    'X-Unity-Version': '2018.4.30f1',
-    'APP-VER': version,
-    'BATTLE-LOGIC-VERSION': '4',
-    'BUNDLE-VER': '',
-    'DEVICE': '2',
-    'DEVICE-ID': '7b1703a5d9b394e24051d7a5d4818f17',
-    'DEVICE-NAME': 'OPPO PCRT00',
-    'EXCEL-VER': '1.0.0',
-    'GRAPHICS-DEVICE-NAME': 'Adreno (TM) 640',
-    'IP-ADDRESS': '10.0.2.15',
-    'KEYCHAIN': '',
-    'LOCALE': 'CN',
-    'PLATFORM-OS-VERSION': 'Android OS 5.1.1 / API-22 (LMY48Z/rel.se.infra.20200612.100533)',
-    'REGION-CODE': '',
-    'RES-KEY': 'ab00a0a6dd915a052a2ef7fd649083e5',
-    'RES-VER': '10002200',
-    'SHORT-UDID': '0'
+    "Accept-Encoding": "gzip",
+    "User-Agent": "Dalvik/2.1.0 (Linux, U, Android 5.1.1, PCRT00 Build/LMY48Z)",
+    "X-Unity-Version": "2018.4.30f1",
+    "APP-VER": version,
+    "BATTLE-LOGIC-VERSION": "4",
+    "BUNDLE-VER": "",
+    "DEVICE": "2",
+    "DEVICE-ID": "7b1703a5d9b394e24051d7a5d4818f17",
+    "DEVICE-NAME": "OPPO PCRT00",
+    "EXCEL-VER": "1.0.0",
+    "GRAPHICS-DEVICE-NAME": "Adreno (TM) 640",
+    "IP-ADDRESS": "10.0.2.15",
+    "KEYCHAIN": "",
+    "LOCALE": "CN",
+    "PLATFORM-OS-VERSION": "Android OS 5.1.1 / API-22 (LMY48Z/rel.se.infra.20200612.100533)",
+    "REGION-CODE": "",
+    "RES-KEY": "ab00a0a6dd915a052a2ef7fd649083e5",
+    "RES-VER": "10002200",
+    "SHORT-UDID": "0",
 }
 
 
 class ApiException(Exception):
-
     def __init__(self, message, code):
         super().__init__(message)
         self.code = code
 
 
 class BSdkClient:
-    '''
-        acccountinfo = {
-            'account': '',
-            'password': '',
-            'platform': 2, # indicates android platform
-            'channel': 1, # indicates bilibili channel
-        }
-    '''
+    """
+    acccountinfo = {
+        'account': '',
+        'password': '',
+        'platform': 2, # indicates android platform
+        'channel': 1, # indicates bilibili channel
+    }
+    """
 
     def __init__(self, account_info, captcha_verifier):
         self.account = account_info.account
         self.pwd = account_info.password
-        self.platform = account_info.platform
-        self.channel = account_info.channel
+        self.platform = 2
+        self.channel = 1
         self.captcha_verifier = captcha_verifier
 
     async def login(self):
         while True:
             resp = await login(self.account, self.pwd, self.captcha_verifier)
-            if resp['code'] == 0:
+            if resp["code"] == 0:
                 logger.info("geetest or captcha succeed")
                 break
-            logger.info(resp['message'])
-            if str(resp['message']) == "用户名或密码错误":
+            logger.info(resp["message"])
+            if str(resp["message"]) == "用户名或密码错误":
                 raise Exception("用户名或密码错误")
 
-        return resp['uid'], resp['access_key']
+        return resp["uid"], resp["access_key"]
 
 
 class PcrClient:
-
     def __init__(self, bs_client: BSdkClient):
         self.viewer_id = 0
         self.b_sdk = bs_client
 
         self.headers = {}
         for key in defaultHeaders.keys():
             self.headers[key] = defaultHeaders[key]
@@ -105,147 +102,173 @@
         self.shouldLogin = True
         self.shouldLoginB = True
 
     async def bili_login(self):
         self.uid, self.access_key = await self.b_sdk.login()
         self.platform = self.b_sdk.platform
         self.channel = self.b_sdk.channel
-        self.headers['PLATFORM'] = str(self.platform)
-        self.headers['PLATFORM-ID'] = str(self.platform)
-        self.headers['CHANNEL-ID'] = str(self.channel)
+        self.headers["PLATFORM"] = str(self.platform)
+        self.headers["PLATFORM-ID"] = str(self.platform)
+        self.headers["CHANNEL-ID"] = str(self.channel)
         self.shouldLoginB = False
 
     @staticmethod
     def create_key() -> bytes:
-        return bytes([ord('0123456789abcdef'[randint(0, 15)]) for _ in range(32)])
+        return bytes([ord("0123456789abcdef"[randint(0, 15)]) for _ in range(32)])
 
     @staticmethod
     def add_to_16(b: bytes) -> bytes:
         n = len(b) % 16
         n = n // 16 * 16 - n + 16
         return b + (n * bytes([n]))
 
     @staticmethod
     def pack(data: object, key: bytes) -> bytes:
-        aes = AES.new(key, AES.MODE_CBC, b'ha4nBYA2APUD6Uv1')
+        aes = AES.new(key, AES.MODE_CBC, b"ha4nBYA2APUD6Uv1")
         return aes.encrypt(PcrClient.add_to_16(packb(data, use_bin_type=False))) + key
 
     @staticmethod
     def encrypt(data: str, key: bytes) -> bytes:
-        aes = AES.new(key, AES.MODE_CBC, b'ha4nBYA2APUD6Uv1')
-        return aes.encrypt(PcrClient.add_to_16(data.encode('utf8'))) + key
+        aes = AES.new(key, AES.MODE_CBC, b"ha4nBYA2APUD6Uv1")
+        return aes.encrypt(PcrClient.add_to_16(data.encode("utf8"))) + key
 
     @staticmethod
     def decrypt(data: bytes):
-        data = b64decode(data.decode('utf8'))
-        aes = AES.new(data[-32:], AES.MODE_CBC, b'ha4nBYA2APUD6Uv1')
+        data = b64decode(data.decode("utf8"))
+        aes = AES.new(data[-32:], AES.MODE_CBC, b"ha4nBYA2APUD6Uv1")
         return aes.decrypt(data[:-32]), data[-32:]
 
     @staticmethod
     def unpack(data: bytes):
-        data = b64decode(data.decode('utf8'))
-        aes = AES.new(data[-32:], AES.MODE_CBC, b'ha4nBYA2APUD6Uv1')
+        data = b64decode(data.decode("utf8"))
+        aes = AES.new(data[-32:], AES.MODE_CBC, b"ha4nBYA2APUD6Uv1")
         dec = aes.decrypt(data[:-32])
-        return unpackb(dec[:-dec[-1]], strict_map_key=False), data[-32:]
+        return unpackb(dec[: -dec[-1]], strict_map_key=False), data[-32:]
 
-    async def callapi(self, api_url: str, request: dict, crypte: bool = True, noerr: bool = True):
+    async def callapi(
+        self, api_url: str, request: dict, crypte: bool = True, noerr: bool = True
+    ):
         # 按api_url创建json文件 保存api_url request data_headers data
         key = PcrClient.create_key()
 
         try:
             if self.viewer_id is not None:
-                request['viewer_id'] = b64encode(PcrClient.encrypt(
-                    str(self.viewer_id), key)) if crypte else str(self.viewer_id)
-
-            response = await (await post(api_root + api_url,
-                                         data=PcrClient.pack(request, key) if crypte else str(request).encode('utf8'),
-                                         headers=self.headers, timeout=10)).content
+                request["viewer_id"] = (
+                    b64encode(PcrClient.encrypt(str(self.viewer_id), key))
+                    if crypte
+                    else str(self.viewer_id)
+                )
+
+            response = await (
+                await post(
+                    api_root + api_url,
+                    data=PcrClient.pack(request, key)
+                    if crypte
+                    else str(request).encode("utf8"),
+                    headers=self.headers,
+                    timeout=10,
+                )
+            ).content
 
-            response = PcrClient.unpack(
-                response)[0] if crypte else loads(response)
+            response = PcrClient.unpack(response)[0] if crypte else loads(response)
 
-            data_headers = response['data_headers']
+            data_headers = response["data_headers"]
             if "/check/game_start" == api_url and "store_url" in data_headers:
                 global version
                 import re
+
                 pattern = re.compile(r"\d\.\d\.\d")
                 version = pattern.findall(data_headers["store_url"])[0]
 
-                defaultHeaders['APP-VER'] = version
-                self.headers['APP-VER'] = version
-                with open(version_txt, "w", encoding='utf-8') as fp:
-                    print(version, file=fp)
+                defaultHeaders["APP-VER"] = version
+                self.headers["APP-VER"] = version
+                # 写入新版本号
+                # with open(version_txt, "w", encoding='utf-8') as fp:
+                #     print(version, file=fp)
 
             # logger.debug("data_headers\ntype={}\n{}", type(data_headers), data_headers)
 
-            if 'sid' in data_headers and data_headers["sid"] != '':
+            if "sid" in data_headers and data_headers["sid"] != "":
                 t = md5()
-                t.update((data_headers['sid'] + 'c!SID!n').encode('utf8'))
-                self.headers['SID'] = t.hexdigest()
+                t.update((data_headers["sid"] + "c!SID!n").encode("utf8"))
+                self.headers["SID"] = t.hexdigest()
 
-            if 'request_id' in data_headers:
-                self.headers['REQUEST-ID'] = data_headers['request_id']
+            if "request_id" in data_headers:
+                self.headers["REQUEST-ID"] = data_headers["request_id"]
 
-            if 'viewer_id' in data_headers:
-                self.viewer_id = data_headers['viewer_id']
+            if "viewer_id" in data_headers:
+                self.viewer_id = data_headers["viewer_id"]
 
-            data = response['data']
+            data = response["data"]
 
-            if not noerr and 'server_error' in data:
-                data = data['server_error']
-                logger.info('pcrclient: {} api failed {}', api_url, data)
-                raise ApiException(data['message'], data['status'])
+            if not noerr and "server_error" in data:
+                data = data["server_error"]
+                logger.info("pcrclient: {} api failed {}", api_url, data)
+                raise ApiException(data["message"], data["status"])
 
             # logger.debug('pcrclient: {} api called', api_url)
             return data
         except:
             self.shouldLogin = True
             raise
 
     async def login(self):
         if self.shouldLoginB:
             await self.bili_login()
 
-        if 'REQUEST-ID' in self.headers:
-            self.headers.pop('REQUEST-ID')
+        if "REQUEST-ID" in self.headers:
+            self.headers.pop("REQUEST-ID")
 
         while True:
-            manifest = await self.callapi('/source_ini/get_maintenance_status?format=json', {}, False, noerr=True)
-            if 'maintenance_message' not in manifest:
+            manifest = await self.callapi(
+                "/source_ini/get_maintenance_status?format=json", {}, False, noerr=True
+            )
+            if "maintenance_message" not in manifest:
                 break
 
             try:
-                match = search('\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d',
-                               manifest['maintenance_message']).group()
+                match = search(
+                    "\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d", manifest["maintenance_message"]
+                ).group()
                 end = parse(match)
-                logger.info('server is in maintenance until {}', match)
+                logger.info("server is in maintenance until {}", match)
                 while datetime.now() < end:
                     await sleep(1)
             except:
-                logger.info('server is in maintenance. waiting for 60 secs')
+                logger.info("server is in maintenance. waiting for 60 secs")
                 await sleep(60)
 
-        ver = manifest['required_manifest_ver']
-        logger.info('using manifest ver = {}', ver)
-        self.headers['MANIFEST-VER'] = str(ver)
-        l_res = await self.callapi('/tool/sdk_login',
-                                   {'uid': str(self.uid), 'access_key': self.access_key, 'channel': str(self.channel),
-                                    'platform': str(self.platform)})
-        if 'is_risk' in l_res and l_res['is_risk'] == 1:
+        ver = manifest["required_manifest_ver"]
+        logger.info("using manifest ver = {}", ver)
+        self.headers["MANIFEST-VER"] = str(ver)
+        l_res = await self.callapi(
+            "/tool/sdk_login",
+            {
+                "uid": str(self.uid),
+                "access_key": self.access_key,
+                "channel": str(self.channel),
+                "platform": str(self.platform),
+            },
+        )
+        if "is_risk" in l_res and l_res["is_risk"] == 1:
             self.shouldLoginB = True
             return
 
-        gamestart = await self.callapi('/check/game_start',
-                                       {'apptype': 0, 'campaign_data': '', 'campaign_user': randint(0, 99999)})
+        gamestart = await self.callapi(
+            "/check/game_start",
+            {"apptype": 0, "campaign_data": "", "campaign_user": randint(0, 99999)},
+        )
 
         try:
-            if not gamestart['now_tutorial']:
+            if not gamestart["now_tutorial"]:
                 raise Exception("该账号没过完教程!")
-        except:
+        except: 
             pass
 
-        load_index = await self.callapi('/load/index', {'carrier': 'OPPO'})
-        home_index = await self.callapi('/home/index',
-                                        {'message_id': 1, 'tips_id_list': [], 'is_first': 1, 'gold_history': 0})
+        load_index = await self.callapi("/load/index", {"carrier": "OPPO"})
+        home_index = await self.callapi(
+            "/home/index",
+            {"message_id": 1, "tips_id_list": [], "is_first": 1, "gold_history": 0},
+        )
 
         self.shouldLogin = False
         return load_index, home_index
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/query.py` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 
 from nonebot import get_driver, logger, on_regex
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot.params import RegexGroup
 from nonebot.permission import SUPERUSER
 
 from .aiorequests import get
-from .config import Config, AccountInfo
+from .config import config, AccountInfo
 from .pcrclient import PcrClient, ApiException, BSdkClient
 
 driver = get_driver()
-config = Config.parse_obj(driver.config)
 
 bot: Bot | None = None
 captcha_lck = Lock()
 queue = asyncio.PriorityQueue()
 otto = config.otto
 pcrjjc_group = config.pcrjjc_group
 ordd = 'x'
@@ -30,17 +29,15 @@
 ac_first = False
 client = None
 captcha_cnt = 0
 admin = int(config.superusers[0]) if len(config.superusers) > 0 else 0
 data_path = config.data_path
 path = join(str(Path()), data_path)
 font_path = join(path, 'SourceHanSansCN-Medium.otf')
-ac_info: list[AccountInfo] = []
-if config.pcrjjc_accounts:
-    ac_info = config.pcrjjc_accounts
+ac_info: list[AccountInfo] = config.pcrjjc_accounts
 binds_info = {}
 
 font_download_url = config.font_download_url
 
 
 @driver.on_startup
 async def _():
@@ -89,22 +86,15 @@
     while pcr_client.shouldLogin:
         await pcr_client.login()
 
 
 async def load_config():
     global ac_info, binds_info, path
     if not ac_info:
-        account_json_name = "account.json"
-        try:
-            with open(join(path, account_json_name)) as fp:
-                ac_info_arr = load(fp)
-                ac_info = [AccountInfo(acc['account'], acc['password'], acc['platform'], acc['channel']) for acc in
-                           ac_info_arr]
-        except FileNotFoundError:
-            logger.error("请在配置文件中配置PCRJJC_ACCOUNTS字段，具体格式见自述文件")
+        logger.error("请在配置文件中配置PCRJJC_ACCOUNTS字段，具体格式见自述文件")
     binds_json_name = "binds.json"
     try:
         with open(join(path, binds_json_name)) as fp:
             binds_info = load(fp)
     except FileNotFoundError:
         pass
 
@@ -144,15 +134,15 @@
         await captcha_lck.acquire()
         ac_first = True
 
     validating = True
 
     # 非自动过码
     if not otto:
-        online_url_head = f"https://help.tencentbot.top/geetest_/?"
+        online_url_head = "https://help.tencentbot.top/geetest_/?"
         url = f"captcha_type=1&challenge={challenge}&gt={gt}&userid={userid}&gs=1"
         message = f'''pcr账号登录需要验证码，请完成以下链接中的验证内容后将第1个方框的内容点击复制，并加上"validate{ordd} "前缀发送给机器人完成验证
         示例：validate{ordd} 123456789\n您也可以发送 validate{ordd} auto 命令bot自动过验证码
         验证链接头：{online_url_head}
         链接：{url}
         为避免tx网页安全验证使验证码过期，请手动拼接链接头和链接'''
         await bot.send_admin_msg_of_pcrjjc(user_id=admin, group_id=pcrjjc_group, message=message)
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.6.2
+Version: 0.7.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -15,15 +15,15 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack>=1.0.5
 Requires-Dist: requests>=2.30.0
 Requires-Dist: Pillow>=9.5.0
-Requires-Dist: pydantic>=1.10.9
+Requires-Dist: pydantic>=2
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pycryptodome>=3.18.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.3
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
 
 # nonebot-plugin-pcrjjc
@@ -81,20 +81,16 @@
 
 登录账号（即PCR_ACCOUNTS）模板
 
 ```python
 PCRJJC_ACCOUNTS='[
     {
      "account": "account1",
-     "password": "password",
-     "platform": 2,
-     "channel": 1
+     "password": "password"
     },
     {
      "account": "account2",
-     "password": "password",
-     "platform": 2,
-     "channel": 1
+     "password": "password"
     }
 ]'
 ```
```

### Comparing `nonebot-plugin-pcrjjc-0.6.2/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot_plugin_pcrjjc-0.7.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

