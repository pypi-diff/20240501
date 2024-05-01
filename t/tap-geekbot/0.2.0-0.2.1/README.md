# Comparing `tmp/tap_geekbot-0.2.0.tar.gz` & `tmp/tap_geekbot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_geekbot-0.2.0.tar", max compression
+gzip compressed data, was "tap_geekbot-0.2.1.tar", max compression
```

## Comparing `tap_geekbot-0.2.0.tar` & `tap_geekbot-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2024-03-01 17:25:18.425346 tap_geekbot-0.2.0/LICENSE
--rw-r--r--   0        0        0     3116 2024-03-01 17:25:18.425346 tap_geekbot-0.2.0/README.md
--rw-r--r--   0        0        0     2433 2024-03-01 17:25:36.609333 tap_geekbot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       82 2024-03-01 17:25:18.429345 tap_geekbot-0.2.0/tap_geekbot/__init__.py
--rw-r--r--   0        0        0      116 2024-03-01 17:25:18.429345 tap_geekbot-0.2.0/tap_geekbot/__main__.py
--rw-r--r--   0        0        0     1464 2024-03-01 17:25:18.429345 tap_geekbot-0.2.0/tap_geekbot/client.py
--rw-r--r--   0        0        0     4005 2024-03-01 17:25:18.429345 tap_geekbot-0.2.0/tap_geekbot/streams.py
--rw-r--r--   0        0        0      926 2024-03-01 17:25:18.429345 tap_geekbot-0.2.0/tap_geekbot/tap.py
--rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 tap_geekbot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3116 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/README.md
+-rw-r--r--   0        0        0     2433 2024-05-01 20:57:12.864814 tap_geekbot-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/tap_geekbot/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/tap_geekbot/__main__.py
+-rw-r--r--   0        0        0     1464 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/tap_geekbot/client.py
+-rw-r--r--   0        0        0     4005 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/tap_geekbot/streams.py
+-rw-r--r--   0        0        0      926 2024-05-01 20:57:07.184795 tap_geekbot-0.2.1/tap_geekbot/tap.py
+-rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 tap_geekbot-0.2.1/PKG-INFO
```

### Comparing `tap_geekbot-0.2.0/LICENSE` & `tap_geekbot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_geekbot-0.2.0/README.md` & `tap_geekbot-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tap_geekbot-0.2.0/pyproject.toml` & `tap_geekbot-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core<2,>=1.8",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-geekbot"
-version = "0.2.0"
+version = "0.2.1"
 description = "`tap-geekbot` is a Singer tap for Geekbot, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Geekbot",
 ]
@@ -19,20 +19,20 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-geekbot"
 repository = "https://github.com/edgarrmondragon/tap-geekbot"
 documentation = "https://github.com/edgarrmondragon/tap-geekbot#readme"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-singer-sdk = "~=0.36.0"
+singer-sdk = "~=0.37.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = ">=1.8.0"
 pytest = "~=8.0"
-singer-sdk = {version = "~=0.36.0", extras = ["testing"]}
+singer-sdk = {version = "~=0.37.0", extras = ["testing"]}
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-geekbot" = "tap_geekbot.tap:TapGeekbot.cli"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `tap_geekbot-0.2.0/tap_geekbot/client.py` & `tap_geekbot-0.2.1/tap_geekbot/client.py`

 * *Files identical despite different names*

### Comparing `tap_geekbot-0.2.0/tap_geekbot/streams.py` & `tap_geekbot-0.2.1/tap_geekbot/streams.py`

 * *Files identical despite different names*

### Comparing `tap_geekbot-0.2.0/tap_geekbot/tap.py` & `tap_geekbot-0.2.1/tap_geekbot/tap.py`

 * *Files identical despite different names*

### Comparing `tap_geekbot-0.2.0/PKG-INFO` & `tap_geekbot-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tap-geekbot
-Version: 0.2.0
+Version: 0.2.1
 Summary: `tap-geekbot` is a Singer tap for Geekbot, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-geekbot
 License: Apache-2.0
 Keywords: ELT,singer.io,Geekbot
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: singer-sdk (>=0.36.0,<0.37.0)
+Requires-Dist: singer-sdk (>=0.37.0,<0.38.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-geekbot#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-geekbot
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # `tap-geekbot`
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: tap-geekbot Version: 0.2.0 Summary: `tap-geekbot`
+Metadata-Version: 2.1 Name: tap-geekbot Version: 0.2.1 Summary: `tap-geekbot`
 is a Singer tap for Geekbot, built with the Meltano SDK for Singer Taps. Home-
 page: https://github.com/edgarrmondragon/tap-geekbot License: Apache-2.0
 Keywords: ELT,singer.io,Geekbot Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Requires-Python: >=3.8 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: singer-sdk (>=0.36.0,<0.37.0)
+Language :: Python :: 3.12 Requires-Dist: singer-sdk (>=0.37.0,<0.38.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-
 geekbot#readme Project-URL: Repository, https://github.com/edgarrmondragon/tap-
 geekbot Description-Content-Type: text/markdown
                                 # `tap-geekbot`
             _[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
   Singer tap for [Geekbot](https://geekbot.com/). Built with the [Meltano Tap
                 SDK](https://sdk.meltano.com) for Singer Taps.
```

