# Comparing `tmp/wipac-rest-tools-1.7.2.tar.gz` & `tmp/wipac-rest-tools-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.7.2.tar", last modified: Mon Apr 22 18:29:51 2024, max compression
+gzip compressed data, was "wipac-rest-tools-1.7.3.tar", last modified: Wed May  1 17:53:10 2024, max compression
```

## Comparing `wipac-rest-tools-1.7.2.tar` & `wipac-rest-tools-1.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:29:51.520728 wipac-rest-tools-1.7.2/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6052 2024-04-22 18:29:51.520728 wipac-rest-tools-1.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4958 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:29:51.516728 wipac-rest-tools-1.7.2/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2024-04-22 18:29:49.000000 wipac-rest-tools-1.7.2/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:29:51.516728 wipac-rest-tools-1.7.2/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15182 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1960 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     7380 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     3048 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2523 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)     2545 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/client/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:29:51.516728 wipac-rest-tools-1.7.2/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      843 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8514 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    17104 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    18655 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2251 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:29:51.520728 wipac-rest-tools-1.7.2/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4832 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2311 2024-04-22 18:29:51.520728 wipac-rest-tools-1.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-22 18:29:48.000000 wipac-rest-tools-1.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:29:51.520728 wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6052 2024-04-22 18:29:51.000000 wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-22 18:29:51.000000 wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 18:29:51.000000 wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      583 2024-04-22 18:29:51.000000 wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-22 18:29:51.000000 wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4958 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.438392 wipac-rest-tools-1.7.3/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.438392 wipac-rest-tools-1.7.3/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15182 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.438392 wipac-rest-tools-1.7.3/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      843 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    17104 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    18655 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.7.2/LICENSE` & `wipac-rest-tools-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/PKG-INFO` & `wipac-rest-tools-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.7.2
+Version: 1.7.3
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.7.2/README.md` & `wipac-rest-tools-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/__init__.py` & `wipac-rest-tools-1.7.3/rest_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/__init__.py` & `wipac-rest-tools-1.7.3/rest_tools/client/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/client.py` & `wipac-rest-tools-1.7.3/rest_tools/client/client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.7.3/rest_tools/client/client_credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# fmt:off
 import logging
 from typing import Any
 
 import requests
 
 from .client import RestClient
 from ..utils.auth import OpenIDAuth
@@ -16,27 +15,32 @@
         address (str): base address of REST API
         token_url (str): base address of token service
         client_id (str): client id
         client_secret (str): client secret
         timeout (int): request timeout (optional)
         retries (int): number of retries to attempt (optional)
     """
+
     def __init__(
         self,
         address: str,
         token_url: str,
         client_id: str,
         client_secret: str,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         self.auth = OpenIDAuth(token_url)
         self.client_id = client_id
         self.client_secret = client_secret
-        super().__init__(address=address, token=self.make_access_token, logger=logging.getLogger('ClientCredentialsAuth'),
-                         **kwargs)
+        super().__init__(
+            address=address,
+            token=self.make_access_token,
+            logger=kwargs.pop('logger', logging.getLogger('ClientCredentialsAuth')),
+            **kwargs,
+        )
 
     def make_access_token(self) -> str:
         if not self.auth.token_url:
             self.auth._refresh_keys()
 
         # try making a new token
         args = {
```

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/device_client.py` & `wipac-rest-tools-1.7.3/rest_tools/client/device_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# fmt:off
 import io
-from itertools import zip_longest
 import logging
-from pathlib import Path
 import time
+from itertools import zip_longest
+from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import qrcode  # type: ignore[import]
 import requests
 
-from ..utils.auth import OpenIDAuth
 from .openid_client import OpenIDRestClient
+from ..utils.auth import OpenIDAuth
 
 
+# fmt:off
+
 def _print_qrcode(req: Dict[str, str]) -> None:
     if 'verification_uri_complete' not in req:
         req['verification_uri_complete'] = req['verification_uri']+'?user_code='+req['user_code']
 
     qr = qrcode.QRCode(border=2)
     qr.add_data(req['verification_uri_complete'])
     f = io.StringIO()
@@ -48,14 +49,16 @@
         print('+', '-' * box_width, '+', sep='')
         for text in qrtext:
             print('|  ', f'{text:<{box_width-4}}', '  |', sep='')
         for qrdata in code:
             print('|', f'{qrdata:<{box_width}}', '|', sep='')
         print('+', '-' * box_width, '+', sep='')
 
+# fmt:on
+
 
 def _perform_device_grant(
     logger: logging.Logger,
     device_url: str,
     token_url: str,
     client_id: str,
     client_secret: Optional[str] = None,
@@ -119,15 +122,17 @@
             raise RuntimeError('Device authorization failed') from exc
         break
 
     return req['refresh_token']
 
 
 def DeviceGrantAuth(
-    address: str, token_url: str, client_id: str,
+    address: str,
+    token_url: str,
+    client_id: str,
     client_secret: Optional[str] = None,
     scopes: Optional[List[str]] = None,
     **kwargs: Any,
 ) -> OpenIDRestClient:
     """A REST client that can handle OpenID and the OAuth2 Device Client flow.
 
     Args:
@@ -135,39 +140,49 @@
         token_url (str): base address of token service
         client_id (str): client id
         client_secret (str): client secret (optional - required for confidential clients)
         scopes (list): token scope list (optional)
         timeout (int): request timeout (optional)
         retries (int): number of retries to attempt (optional)
     """
-    logger = logging.getLogger('DeviceGrantAuth')
+    logger = kwargs.pop('logger', logging.getLogger('DeviceGrantAuth'))
 
     auth = OpenIDAuth(token_url)
     if 'device_authorization_endpoint' not in auth.provider_info:
         raise RuntimeError('Device grant not supported by server')
     endpoint = auth.provider_info['device_authorization_endpoint']
 
-    refresh_token = _perform_device_grant(logger, endpoint, auth.token_url, client_id, client_secret, scopes)
-
-    return OpenIDRestClient(address=address, token_url=token_url, client_id=client_id,
-                            client_secret=client_secret, refresh_token=refresh_token, **kwargs)
+    refresh_token = _perform_device_grant(
+        logger, endpoint, auth.token_url, client_id, client_secret, scopes
+    )
+
+    return OpenIDRestClient(
+        address=address,
+        token_url=token_url,
+        client_id=client_id,
+        client_secret=client_secret,
+        refresh_token=refresh_token,
+        logger=logger,
+        **kwargs,
+    )
 
 
 def _load_token_from_file(filepath: Path) -> Optional[str]:
     if filepath.exists():
         return filepath.read_text()
     return None
 
 
 def _save_token_to_file(filepath: Path, token: str) -> None:
     filepath.write_text(token)
 
 
 def SavedDeviceGrantAuth(
-    address: str, token_url: str,
+    address: str,
+    token_url: str,
     filename: str,
     client_id: str,
     client_secret: Optional[str] = None,
     scopes: Optional[List[str]] = None,
     **kwargs: Any,
 ) -> OpenIDRestClient:
     """
@@ -180,35 +195,51 @@
         filename (str): name of file to save/load refresh token
         client_id (str): client id
         client_secret (str): client secret (optional - required for confidential clients)
         scopes (list): token scope list (optional)
         timeout (int): request timeout (optional)
         retries (int): number of retries to attempt (optional)
     """
-    logger = logging.getLogger('SavedDeviceGrantAuth')
+    logger = kwargs.pop('logger', logging.getLogger('SavedDeviceGrantAuth'))
     filepath = Path(filename)
 
     def update_func(access, refresh):
         _save_token_to_file(filepath, refresh)
 
     refresh_token = _load_token_from_file(filepath)
     if refresh_token:
         try:
             # this will try to refresh, and raise if it fails
-            return OpenIDRestClient(address=address, token_url=token_url, client_id=client_id,
-                                    client_secret=client_secret, refresh_token=refresh_token,
-                                    update_func=update_func, **kwargs)
+            return OpenIDRestClient(
+                address=address,
+                token_url=token_url,
+                client_id=client_id,
+                client_secret=client_secret,
+                refresh_token=refresh_token,
+                update_func=update_func,
+                logger=logger,
+                **kwargs,
+            )
         except Exception:
             pass
 
     auth = OpenIDAuth(token_url)
     if not auth.provider_info:
         raise RuntimeError('Token service does not support .well-known discovery')
     if 'device_authorization_endpoint' not in auth.provider_info:
         raise RuntimeError('Device grant not supported by server')
     endpoint = auth.provider_info['device_authorization_endpoint']
 
-    refresh_token = _perform_device_grant(logger, endpoint, auth.token_url, client_id, client_secret, scopes)
-
-    return OpenIDRestClient(address=address, token_url=token_url, client_id=client_id,
-                            client_secret=client_secret, refresh_token=refresh_token,
-                            update_func=update_func, **kwargs)
+    refresh_token = _perform_device_grant(
+        logger, endpoint, auth.token_url, client_id, client_secret, scopes
+    )
+
+    return OpenIDRestClient(
+        address=address,
+        token_url=token_url,
+        client_id=client_id,
+        client_secret=client_secret,
+        refresh_token=refresh_token,
+        update_func=update_func,
+        logger=logger,
+        **kwargs,
+    )
```

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.7.3/rest_tools/client/openid_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 .. _requests: http://docs.python-requests.org
 
 The REST protocol is built on http(s), with the body containing
 a json-encoded dictionary as necessary.
 """
 
-# fmt:off
 import logging
 from typing import Any, Callable, Optional, Union
 
 import requests
 
-from ..utils.auth import OpenIDAuth
 from .client import RestClient
+from ..utils.auth import OpenIDAuth
 
 
 class OpenIDRestClient(RestClient):
     """A REST client that can handle token refresh using OpenID .well-known
     auto-discovery.
 
     Args:
@@ -26,32 +25,39 @@
         client_id (str): client id
         client_secret (str): client secret (optional - required to generate new refresh token)
         refresh_token (str): initial refresh token (optional)
         update_func (callable): a function that gets called when the access and refresh tokens are updated (optional)
         timeout (int): request timeout (optional)
         retries (int): number of retries to attempt (optional)
     """
+
     def __init__(
         self,
         address: str,
         token_url: str,
         refresh_token: Union[str, bytes],
         client_id: str,
         client_secret: Optional[str] = None,
-        update_func: Optional[Callable[[Union[str, bytes], Optional[Union[str, bytes]]], None]] = None,
-        **kwargs: Any
+        update_func: Optional[
+            Callable[[Union[str, bytes], Optional[Union[str, bytes]]], None]
+        ] = None,
+        **kwargs: Any,
     ) -> None:
         self.auth = OpenIDAuth(token_url)
         self.refresh_token = refresh_token
         self.client_id = client_id
         self.client_secret = client_secret
         self.update_func = update_func
 
-        super().__init__(address, logger=logging.getLogger('OpenIDRestClient'),
-                         token=self._openid_token, **kwargs)
+        super().__init__(
+            address,
+            logger=kwargs.pop('logger', logging.getLogger('OpenIDRestClient')),
+            token=self._openid_token,
+            **kwargs,
+        )
 
         # initial call to verify things work
         self._openid_token()
 
     def _openid_token(self) -> str:
         if not self.auth.token_url:
             self.auth._refresh_keys()
```

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/session.py` & `wipac-rest-tools-1.7.3/rest_tools/client/session.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/client/utils.py` & `wipac-rest-tools-1.7.3/rest_tools/client/utils.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/server/__init__.py` & `wipac-rest-tools-1.7.3/rest_tools/server/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.7.3/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/server/decorators.py` & `wipac-rest-tools-1.7.3/rest_tools/server/decorators.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/server/handler.py` & `wipac-rest-tools-1.7.3/rest_tools/server/handler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/server/server.py` & `wipac-rest-tools-1.7.3/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/server/stats.py` & `wipac-rest-tools-1.7.3/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/telemetry.py` & `wipac-rest-tools-1.7.3/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/utils/auth.py` & `wipac-rest-tools-1.7.3/rest_tools/utils/auth.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.7.3/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.7.3/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/setup.cfg` & `wipac-rest-tools-1.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.7.2
+Version: 1.7.3
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.2/wipac_rest_tools.egg-info/requires.txt` & `wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/requires.txt`

 * *Files identical despite different names*

