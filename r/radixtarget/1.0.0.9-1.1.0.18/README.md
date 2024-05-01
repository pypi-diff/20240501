# Comparing `tmp/radixtarget-1.0.0.9.tar.gz` & `tmp/radixtarget-1.1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radixtarget-1.0.0.9.tar", max compression
+gzip compressed data, was "radixtarget-1.1.0.18.tar", max compression
```

## Comparing `radixtarget-1.0.0.9.tar` & `radixtarget-1.1.0.18.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1152 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/README.md
--rw-r--r--   0        0        0      818 2024-04-22 18:39:53.703949 radixtarget-1.0.0.9/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/__init__.py
--rw-r--r--   0        0        0      882 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/radixtarget.py
--rw-r--r--   0        0        0        0 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/test/__init__.py
--rw-r--r--   0        0        0   454463 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/test/cidrs.txt
--rw-r--r--   0        0        0     3091 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/test/test_pyradix.py
--rw-r--r--   0        0        0      205 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/tree/base.py
--rw-r--r--   0        0        0      974 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/tree/dns.py
--rw-r--r--   0        0        0     1398 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/tree/ip.py
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 radixtarget-1.0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    34809 2024-05-01 20:50:12.519379 radixtarget-1.1.0.18/LICENSE
+-rw-r--r--   0        0        0     1918 2024-05-01 20:50:12.519379 radixtarget-1.1.0.18/README.md
+-rw-r--r--   0        0        0      819 2024-05-01 20:50:26.171262 radixtarget-1.1.0.18/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-05-01 20:50:12.519379 radixtarget-1.1.0.18/radixtarget/__init__.py
+-rw-r--r--   0        0        0     1092 2024-05-01 20:50:12.519379 radixtarget-1.1.0.18/radixtarget/radixtarget.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:50:12.519379 radixtarget-1.1.0.18/radixtarget/test/__init__.py
+-rw-r--r--   0        0        0   454463 2024-05-01 20:50:12.523379 radixtarget-1.1.0.18/radixtarget/test/cidrs.txt
+-rw-r--r--   0        0        0     3442 2024-05-01 20:50:12.523379 radixtarget-1.1.0.18/radixtarget/test/test_pyradix.py
+-rw-r--r--   0        0        0      251 2024-05-01 20:50:12.523379 radixtarget-1.1.0.18/radixtarget/tree/base.py
+-rw-r--r--   0        0        0      974 2024-05-01 20:50:12.523379 radixtarget-1.1.0.18/radixtarget/tree/dns.py
+-rw-r--r--   0        0        0     1398 2024-05-01 20:50:12.523379 radixtarget-1.1.0.18/radixtarget/tree/ip.py
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 radixtarget-1.1.0.18/PKG-INFO
```

### Comparing `radixtarget-1.0.0.9/README.md` & `radixtarget-1.1.0.18/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # RadixTarget
 
+[![Python Version](https://img.shields.io/badge/python-3.9+-blue)](https://www.python.org) [![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://github.com/blacklanternsecurity/radixtarget/blob/master/LICENSE) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![tests](https://github.com/blacklanternsecurity/radixtarget/actions/workflows/tests.yml/badge.svg)](https://github.com/blacklanternsecurity/radixtarget/actions/workflows/tests.yml) [![Codecov](https://codecov.io/gh/blacklanternsecurity/radixtarget/graph/badge.svg?token=7IPWMYMTGZ)](https://codecov.io/gh/blacklanternsecurity/radixtarget)
+
 RadixTarget is a performant radix implementation designed for quick lookups of IP addresses/networks and DNS hostnames. Written in pure python and capable of roughly 100,000 lookups per second regardless of the size of the database.
 
 Used by:
 - [BBOT (Bighuge BLS OSINT Tool)](https://github.com/blacklanternsecurity/bbot)
 - [cloudcheck](https://github.com/blacklanternsecurity/cloudcheck)
 
 ### Installation ([PyPi](https://pypi.org/project/radixtarget/))
@@ -17,26 +19,29 @@
 ```python
 from radixtarget import RadixTarget
 
 rt = RadixTarget()
 
 # IPv4
 rt.insert("192.168.1.0/24")
-rt.search("192.168.1.10") # ipaddress.ip_network("192.168.1.0/24")
+rt.search("192.168.1.10") # IPv4Network("192.168.1.0/24")
 rt.search("192.168.2.10") # None
 
 # ipv6
 rt.insert("dead::/64")
-rt.search("dead::beef") # ipaddress.ip_network("dead::/64")
+rt.search("dead::beef") # IPv6Network("dead::/64")
 rt.search("dead:cafe::beef") # None
 
 # DNS
 rt.insert("net")
 rt.insert("www.example.com")
 rt.insert("test.www.example.com")
-
 rt.search("net") # "net"
 rt.search("evilcorp.net") # "net"
 rt.search("www.example.com") # "www.example.com"
 rt.search("asdf.test.www.example.com") # "test.www.example.com"
 rt.search("example.com") # None
+
+# Custom data nodes
+rt.insert("evilcorp.co.uk", "custom_data")
+rt.search("www.evilcorp.co.uk") # "custom_data"
 ```
```

### Comparing `radixtarget-1.0.0.9/pyproject.toml` & `radixtarget-1.1.0.18/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radixtarget"
-version = "v1.0.0.9"
+version = "v1.1.0.18"
 description = "Check whether an IP address belongs to a cloud provider"
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/radixtarget"
 homepage = "https://github.com/blacklanternsecurity/radixtarget"
 
@@ -19,12 +19,12 @@
 flake8 = ">=6.1,<8.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata = false
-format-jinja = 'v1.0.0.{{ distance }}'
+format-jinja = 'v1.1.0.{{ distance }}'
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `radixtarget-1.0.0.9/radixtarget/test/cidrs.txt` & `radixtarget-1.1.0.18/radixtarget/test/cidrs.txt`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.9/radixtarget/test/test_pyradix.py` & `radixtarget-1.1.0.18/radixtarget/test/test_pyradix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import pytest
 import random
 import logging
 import ipaddress
 from pathlib import Path
 
 log = logging.getLogger("radixtarget.test")
 
@@ -62,14 +63,23 @@
         assert rt.search("evilcorp.net") == "net"
         assert rt.search("www.example.com") == "www.example.com"
         assert rt.search("asdf.test.www.example.com") == "test.www.example.com"
         assert rt.search("example.com") is None
         rt.insert("evilcorp.co.uk", "custom_data")
         assert rt.search("www.evilcorp.co.uk") == "custom_data"
 
+        with pytest.raises(ValueError, match=".*must be of str or ipaddress type.*"):
+            rt.insert(b"asdf")
+
+        with pytest.raises(ValueError, match=".*must be of str or ipaddress type.*"):
+            rt.search(b"asdf")
+
+        assert "net" in rt.dns_tree.root.children
+        assert "com" in rt.dns_tree.root.children
+
         # speed benchmark
         cidrs = open(cidr_list_path).read().splitlines()
         log.critical(len(cidrs))
         for c in cidrs:
             rt.insert(c)
 
         iterations = 10000
```

### Comparing `radixtarget-1.0.0.9/radixtarget/tree/dns.py` & `radixtarget-1.1.0.18/radixtarget/tree/dns.py`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.9/radixtarget/tree/ip.py` & `radixtarget-1.1.0.18/radixtarget/tree/ip.py`

 * *Files identical despite different names*

