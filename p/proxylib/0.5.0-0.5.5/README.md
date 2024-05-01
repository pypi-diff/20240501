# Comparing `tmp/proxylib-0.5.0.tar.gz` & `tmp/proxylib-0.5.5.tar.gz`

## Comparing `proxylib-0.5.0.tar` & `proxylib-0.5.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/example.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/__init__.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/env.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/netutils.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/proxy.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/utils.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/os/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/os/nt.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/pac/__init__.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/pac/javascript.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 proxylib-0.5.0/tests/test_pac.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 proxylib-0.5.0/tests/test_proxy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 proxylib-0.5.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proxylib-0.5.0/LICENSE
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 proxylib-0.5.0/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 proxylib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 proxylib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/example.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/__init__.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/env.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/netutils.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/proxy.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/requests.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/utils.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/os/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/os/nt.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/pac/__init__.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 proxylib-0.5.5/src/proxylib/pac/javascript.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 proxylib-0.5.5/tests/test_pac.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 proxylib-0.5.5/tests/test_proxy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 proxylib-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proxylib-0.5.5/LICENSE
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 proxylib-0.5.5/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 proxylib-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 proxylib-0.5.5/PKG-INFO
```

### Comparing `proxylib-0.5.0/src/proxylib/env.py` & `proxylib-0.5.5/src/proxylib/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
     def __getitem__(self, url: str) -> _Iter[Proxy]:
         uri = URL.from_str(url)
         url = f"{uri.scheme}://{uri.netloc}"
         ip = get_ip(uri.host)
         for _no in self.no_proxy:
             if _no is None:
+                if ip.is_loopback():
+                    return [None]
                 for _if in get_local_interfaces():
                     if ip in _if.network:
                         return [None]
             else:
                 if _no.match(url):
                     return [None]
         return self.https_proxy[url] if uri.scheme == "https" else self.http_proxy[url]
```

### Comparing `proxylib-0.5.0/src/proxylib/proxy.py` & `proxylib-0.5.5/src/proxylib/proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,29 @@
                 self.scheme,
                 self.username,
                 self.password,
                 self.host,
                 getservbyname(self.scheme),
             )
 
+    def as_uri(self):
+        authority = self.netloc
+        userinfo = ""
+        if self.username:
+            userinfo = self.username
+            if self.password:
+                userinfo = userinfo + ":" + self.password
+
+        if userinfo:
+            authority = userinfo + "@" + self.netloc
+        if self.scheme:
+            return self.scheme + "://" + authority
+        else:
+            return "//" + authority
+
     @classmethod
     def from_str(
         cls,
         uri: str,
         format: UriSplit = UriSplit.Default,
     ):
         return cls(*format.match(uri).groups()) if uri else None
```

### Comparing `proxylib-0.5.0/src/proxylib/utils.py` & `proxylib-0.5.5/src/proxylib/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, proxy: "Proxy|Sequence[Proxy]|str" = None) -> None:
         if isinstance(proxy, str):
             proxy = Proxy.find_all(proxy, UriSplit.PAC)
         self.proxies: Sequence[Proxy] = (
             proxy if isinstance(proxy, Sequence) else (proxy,)
         )
 
-    def __getitem__(self):
+    def __getitem__(self, uri: str):
         return self.proxies
 
 
 def get_proxymap_for(src: "str|Proxy|None") -> ProxyMap:
     if isinstance(src, str):
         try:
             _proxy = Proxy.find_all(src)
```

### Comparing `proxylib-0.5.0/src/proxylib/os/nt.py` & `proxylib-0.5.5/src/proxylib/os/nt.py`

 * *Files identical despite different names*

### Comparing `proxylib-0.5.0/src/proxylib/pac/__init__.py` & `proxylib-0.5.5/src/proxylib/pac/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 from typing import Literal as _Literal
 from typing import cast as _cast
 from typing import get_args as _args
 from typing import overload as _overload
 from urllib.request import urlopen as _urlopen
 from warnings import warn as _warn
 
-from ..proxy import Proxy, ProxyMap, UriSplit
+from ..netutils import get_ip
+from ..proxy import Proxy, UriSplit
 
 _WEEKDAY = _Literal["SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT"]
 _WEEKDAYS = ("SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT")
 
 __all__ = ("PAC", "load")
 
 
 class PAC(object):
 
     #### UTILITY FUNCTIONS ####
     @staticmethod
     def dnsResolve(host: str, /):
-        try:
-            return _socket.gethostbyname(host)
-        except:
-            return
+        ip = get_ip(host)
+        if ip:
+            return ip.exploded
 
     @staticmethod
     def myIpAddress():
         return _socket.gethostbyname(_socket.gethostname())
 
     @staticmethod
     def dnsDomainLevels(host: str, /):
```

### Comparing `proxylib-0.5.0/src/proxylib/pac/javascript.py` & `proxylib-0.5.5/src/proxylib/pac/javascript.py`

 * *Files identical despite different names*

### Comparing `proxylib-0.5.0/tests/test_proxy.py` & `proxylib-0.5.5/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `proxylib-0.5.0/LICENSE` & `proxylib-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proxylib-0.5.0/pyproject.toml` & `proxylib-0.5.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proxylib"
-version = "0.5.0"
+version = "0.5.5"
 authors = [{ name = "Jose A" }]
 description = "Proxy models and functions to build proxy configurations or get the systems proxy information and parse their result"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = []
 [project.optional-dependencies]
-dev = ['build', 'twine', 'hatchling', 'pytest']
-pac = ['dukpy']
+dev = ['build', 'twine', 'hatchling', 'pytest', 'requests']
+jspac = ['dukpy']
 ifaddr = ['ifaddr']
 
 [project.urls]
 Homepage = "https://github.com/jose-pr/proxylib/"
 Issues = "https://github.com/jose-pr/proxylib/issues"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `proxylib-0.5.0/PKG-INFO` & `proxylib-0.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.3
 Name: proxylib
-Version: 0.5.0
+Version: 0.5.5
 Summary: Proxy models and functions to build proxy configurations or get the systems proxy information and parse their result
 Project-URL: Homepage, https://github.com/jose-pr/proxylib/
 Project-URL: Issues, https://github.com/jose-pr/proxylib/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: hatchling; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: requests; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Provides-Extra: ifaddr
 Requires-Dist: ifaddr; extra == 'ifaddr'
-Provides-Extra: pac
-Requires-Dist: dukpy; extra == 'pac'
+Provides-Extra: jspac
+Requires-Dist: dukpy; extra == 'jspac'
 Description-Content-Type: text/markdown
 
 Proxy models and functions to build proxy configurations or get the systems proxy information and parse their result.
 
 Ability to handle PAC files.
```

