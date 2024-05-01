# Comparing `tmp/tap_betterstack-0.1.1a1.tar.gz` & `tmp/tap_betterstack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_betterstack-0.1.1a1.tar", max compression
+gzip compressed data, was "tap_betterstack-0.1.2.tar", max compression
```

## Comparing `tap_betterstack-0.1.1a1.tar` & `tap_betterstack-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11355 2024-01-03 03:20:01.323055 tap_betterstack-0.1.1a1/LICENSE
--rw-r--r--   0        0        0     5312 2024-01-03 03:20:01.323055 tap_betterstack-0.1.1a1/README.md
--rw-r--r--   0        0        0     2386 2024-01-03 03:20:21.067098 tap_betterstack-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0       86 2024-01-03 03:20:01.327055 tap_betterstack-0.1.1a1/tap_betterstack/__init__.py
--rw-r--r--   0        0        0      128 2024-01-03 03:20:01.327055 tap_betterstack-0.1.1a1/tap_betterstack/__main__.py
--rw-r--r--   0        0        0     2807 2024-01-03 03:20:01.327055 tap_betterstack-0.1.1a1/tap_betterstack/client.py
--rw-r--r--   0        0        0       28 2024-01-03 03:20:01.327055 tap_betterstack-0.1.1a1/tap_betterstack/streams/__init__.py
--rw-r--r--   0        0        0    17940 2024-01-03 03:20:01.327055 tap_betterstack-0.1.1a1/tap_betterstack/streams/uptime.py
--rw-r--r--   0        0        0     1372 2024-01-03 03:20:01.327055 tap_betterstack-0.1.1a1/tap_betterstack/tap.py
--rw-r--r--   0        0        0     6302 1970-01-01 00:00:00.000000 tap_betterstack-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-01 19:19:15.396065 tap_betterstack-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5312 2024-05-01 19:19:15.396065 tap_betterstack-0.1.2/README.md
+-rw-r--r--   0        0        0     2384 2024-05-01 19:19:18.756058 tap_betterstack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-05-01 19:19:15.400065 tap_betterstack-0.1.2/tap_betterstack/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-01 19:19:15.400065 tap_betterstack-0.1.2/tap_betterstack/__main__.py
+-rw-r--r--   0        0        0     2807 2024-05-01 19:19:15.400065 tap_betterstack-0.1.2/tap_betterstack/client.py
+-rw-r--r--   0        0        0       28 2024-05-01 19:19:15.400065 tap_betterstack-0.1.2/tap_betterstack/streams/__init__.py
+-rw-r--r--   0        0        0    17940 2024-05-01 19:19:15.400065 tap_betterstack-0.1.2/tap_betterstack/streams/uptime.py
+-rw-r--r--   0        0        0     1372 2024-05-01 19:19:15.400065 tap_betterstack-0.1.2/tap_betterstack/tap.py
+-rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 tap_betterstack-0.1.2/PKG-INFO
```

### Comparing `tap_betterstack-0.1.1a1/LICENSE` & `tap_betterstack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.1.1a1/README.md` & `tap_betterstack-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.1.1a1/pyproject.toml` & `tap_betterstack-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core==1.8",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-betterstack"
-version = "0.1.1a1"
+version = "0.1.2"
 description = "`tap-betterstack` is a Singer tap for Better Stack, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Better Stack",
 ]
@@ -19,15 +19,15 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-betterstack"
 repository = "https://github.com/edgarrmondragon/tap-betterstack"
 documentation = "https://github.com/edgarrmondragon/tap-betterstack#readme"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-singer-sdk = "~=0.34.0"
+singer-sdk = "~=0.36.0"
 
 [tool.poetry.group.dev.dependencies]
 singer-sdk = {version = "*", extras = ["testing"]}
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-betterstack" = "tap_betterstack.tap:TapBetterStack.cli"
```

### Comparing `tap_betterstack-0.1.1a1/tap_betterstack/client.py` & `tap_betterstack-0.1.2/tap_betterstack/client.py`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.1.1a1/tap_betterstack/streams/uptime.py` & `tap_betterstack-0.1.2/tap_betterstack/streams/uptime.py`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.1.1a1/tap_betterstack/tap.py` & `tap_betterstack-0.1.2/tap_betterstack/tap.py`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.1.1a1/PKG-INFO` & `tap_betterstack-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tap-betterstack
-Version: 0.1.1a1
+Version: 0.1.2
 Summary: `tap-betterstack` is a Singer tap for Better Stack, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-betterstack
 License: Apache-2.0
 Keywords: ELT,singer.io,Better Stack
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
-Requires-Dist: singer-sdk (>=0.34.0,<0.35.0)
+Requires-Dist: singer-sdk (>=0.36.0,<0.37.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-betterstack#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-betterstack
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # tap-betterstack
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: tap-betterstack Version: 0.1.1a1 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-betterstack Version: 0.1.2 Summary: `tap-
 betterstack` is a Singer tap for Better Stack, built with the Meltano SDK for
 Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-betterstack
 License: Apache-2.0 Keywords: ELT,singer.io,Better Stack Author: Edgar
 RamÃ­rez-MondragÃ³n Author-email: edgarrm358@gmail.com Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: singer-sdk (>=0.34.0,<0.35.0) Project-URL: Documentation, https://
+Dist: singer-sdk (>=0.36.0,<0.37.0) Project-URL: Documentation, https://
 github.com/edgarrmondragon/tap-betterstack#readme Project-URL: Repository,
 https://github.com/edgarrmondragon/tap-betterstack Description-Content-Type:
 text/markdown
                                # tap-betterstack
             _[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 Singer tap for [Better Stack](https://betterstack.com). Built with the [Meltano
                     Singer SDK](https://sdk.meltano.com).
```

