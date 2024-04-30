# Comparing `tmp/gep3-0.4.tar.gz` & `tmp/gep3-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gep3-0.4.tar", last modified: Mon Apr 29 23:53:47 2024, max compression
+gzip compressed data, was "gep3-0.4.1.tar", last modified: Tue Apr 30 03:16:18 2024, max compression
```

## Comparing `gep3-0.4.tar` & `gep3-0.4.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 23:53:38.000000 gep3-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-29 23:53:47.480560 gep3-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 23:53:38.000000 gep3-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 23:53:38.000000 gep3-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-29 23:53:47.480560 gep3-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.472560 gep3-0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/ccid/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/bulk_in_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/bulk_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/bulk_out_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-29 23:53:38.000000 gep3-0.4/src/common/ber.py
--rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-29 23:53:38.000000 gep3-0.4/src/common/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 23:53:38.000000 gep3-0.4/src/common/bitstr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-29 23:53:38.000000 gep3-0.4/src/common/hstr.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-29 23:53:38.000000 gep3-0.4/src/common/intlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-29 23:53:38.000000 gep3-0.4/src/common/parserc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-29 23:53:38.000000 gep3-0.4/src/common/str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29456 2024-04-29 23:53:38.000000 gep3-0.4/src/crypto/des.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-29 23:53:38.000000 gep3-0.4/src/crypto/modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/emv/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/dsc.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/key_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/emv_key_derivation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/evc_cvc3.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/evc_dcvv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/gep3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/globalplatform/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-29 23:53:38.000000 gep3-0.4/src/globalplatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-29 23:53:38.000000 gep3-0.4/src/globalplatform/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-29 23:53:38.000000 gep3-0.4/src/globalplatform/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/iso7816/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16507 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/apdu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/multos/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 23:53:38.000000 gep3-0.4/src/multos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 23:53:38.000000 gep3-0.4/src/multos/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-29 23:53:38.000000 gep3-0.4/src/multos/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-29 23:53:38.000000 gep3-0.4/src/tests/test_common_ber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-29 23:53:38.000000 gep3-0.4/src/tests/test_crypto_des.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.247423 gep3-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 03:16:10.000000 gep3-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-30 03:16:18.247423 gep3-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-30 03:16:10.000000 gep3-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 03:16:10.000000 gep3-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-30 03:16:18.247423 gep3-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.239422 gep3-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.239422 gep3-0.4.1/src/ccid/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 03:16:10.000000 gep3-0.4.1/src/ccid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-30 03:16:10.000000 gep3-0.4.1/src/ccid/bulk_in_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-30 03:16:10.000000 gep3-0.4.1/src/ccid/bulk_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-30 03:16:10.000000 gep3-0.4.1/src/ccid/bulk_out_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-30 03:16:10.000000 gep3-0.4.1/src/ccid/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.239422 gep3-0.4.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/bitstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/hstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/intlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/parserc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 03:16:10.000000 gep3-0.4.1/src/common/str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.243422 gep3-0.4.1/src/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:10.000000 gep3-0.4.1/src/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29456 2024-04-30 03:16:10.000000 gep3-0.4.1/src/crypto/des.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-30 03:16:10.000000 gep3-0.4.1/src/crypto/modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.243422 gep3-0.4.1/src/emv/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 03:16:10.000000 gep3-0.4.1/src/emv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-30 03:16:10.000000 gep3-0.4.1/src/emv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-30 03:16:10.000000 gep3-0.4.1/src/emv/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-30 03:16:10.000000 gep3-0.4.1/src/emv/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-30 03:16:10.000000 gep3-0.4.1/src/emv/key_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 03:16:10.000000 gep3-0.4.1/src/emv/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.243422 gep3-0.4.1/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:10.000000 gep3-0.4.1/src/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-30 03:16:10.000000 gep3-0.4.1/src/examples/emv_key_derivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-30 03:16:10.000000 gep3-0.4.1/src/examples/evc_cvc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-30 03:16:10.000000 gep3-0.4.1/src/examples/evc_dcvv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.247423 gep3-0.4.1/src/gep3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-30 03:16:18.000000 gep3-0.4.1/src/gep3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-30 03:16:18.000000 gep3-0.4.1/src/gep3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:16:18.000000 gep3-0.4.1/src/gep3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 03:16:18.000000 gep3-0.4.1/src/gep3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 03:16:18.000000 gep3-0.4.1/src/gep3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.243422 gep3-0.4.1/src/globalplatform/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 03:16:10.000000 gep3-0.4.1/src/globalplatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-30 03:16:10.000000 gep3-0.4.1/src/globalplatform/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-30 03:16:10.000000 gep3-0.4.1/src/globalplatform/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.243422 gep3-0.4.1/src/iso7816/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 03:16:10.000000 gep3-0.4.1/src/iso7816/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-30 03:16:10.000000 gep3-0.4.1/src/iso7816/apdu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-30 03:16:10.000000 gep3-0.4.1/src/iso7816/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-30 03:16:10.000000 gep3-0.4.1/src/iso7816/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.247423 gep3-0.4.1/src/multos/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 03:16:10.000000 gep3-0.4.1/src/multos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-30 03:16:10.000000 gep3-0.4.1/src/multos/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-30 03:16:10.000000 gep3-0.4.1/src/multos/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:18.247423 gep3-0.4.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:16:10.000000 gep3-0.4.1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-30 03:16:10.000000 gep3-0.4.1/src/tests/test_common_ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-30 03:16:10.000000 gep3-0.4.1/src/tests/test_crypto_des.py
```

### Comparing `gep3-0.4/LICENSE` & `gep3-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gep3-0.4/PKG-INFO` & `gep3-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.4
+Version: 0.4.1
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gep3-0.4/setup.cfg` & `gep3-0.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gep3
-version = 0.4
+version = 0.4.1
 author = Sebastien Pochic
 author_email = spochic@gmail.com
 description = Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spochic/gep3
 project_urls =
```

### Comparing `gep3-0.4/src/ccid/__init__.py` & `gep3-0.4.1/src/ccid/__init__.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/ccid/bulk_in_messages.py` & `gep3-0.4.1/src/ccid/bulk_in_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/ccid/bulk_message.py` & `gep3-0.4.1/src/ccid/bulk_message.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/ccid/bulk_out_messages.py` & `gep3-0.4.1/src/ccid/bulk_out_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/ccid/descriptors.py` & `gep3-0.4.1/src/ccid/descriptors.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/ber.py` & `gep3-0.4.1/src/common/ber.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/binary.py` & `gep3-0.4.1/src/common/binary.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/bitstr.py` & `gep3-0.4.1/src/common/bitstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/hstr.py` & `gep3-0.4.1/src/common/hstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/intlist.py` & `gep3-0.4.1/src/common/intlist.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/parserc.py` & `gep3-0.4.1/src/common/parserc.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/common/str.py` & `gep3-0.4.1/src/common/str.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/crypto/des.py` & `gep3-0.4.1/src/crypto/des.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/crypto/modes.py` & `gep3-0.4.1/src/crypto/modes.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/emv/commands.py` & `gep3-0.4.1/src/emv/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/emv/data.py` & `gep3-0.4.1/src/emv/data.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/emv/dsc.py` & `gep3-0.4.1/src/emv/dsc.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/emv/key_management.py` & `gep3-0.4.1/src/emv/key_management.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/emv/records.py` & `gep3-0.4.1/src/emv/records.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/examples/emv_key_derivation.py` & `gep3-0.4.1/src/examples/emv_key_derivation.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/examples/evc_cvc3.py` & `gep3-0.4.1/src/examples/evc_cvc3.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/examples/evc_dcvv.py` & `gep3-0.4.1/src/examples/evc_dcvv.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/gep3.egg-info/PKG-INFO` & `gep3-0.4.1/src/gep3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.4
+Version: 0.4.1
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gep3-0.4/src/gep3.egg-info/SOURCES.txt` & `gep3-0.4.1/src/gep3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/globalplatform/commands.py` & `gep3-0.4.1/src/globalplatform/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/globalplatform/encodings.py` & `gep3-0.4.1/src/globalplatform/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/iso7816/apdu.py` & `gep3-0.4.1/src/iso7816/apdu.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,14 +163,27 @@
 
             case CommandCase.Case2S | CommandCase.Case4S:
                 return self[-1]
 
             case CommandCase.Case2E | CommandCase.Case4E:
                 return self[-2:]
 
+    @property
+    def Ne(self) -> int:
+        match self.case:
+            case CommandCase.Case1 | CommandCase.Case3S | CommandCase.Case3E:
+                raise ValueError(
+                    F'Command APDU has no Le field ({self.case.value})')
+
+            case CommandCase.Case2S | CommandCase.Case4S:
+                return 256 if self[-1] == '00' else int(self[-1])
+
+            case CommandCase.Case2E | CommandCase.Case4E:
+                return 65536 if self[-2:] == '0000' else int(self[-2:])
+
     def updated_Ne(self, Ne: int) -> CommandApdu:
         match self.case:
             case CommandCase.Case1 | CommandCase.Case3S | CommandCase.Case3E:
                 raise ValueError(
                     F'Command APDU has no Le field ({self.case.value})')
 
             case CommandCase.Case2S:
@@ -180,29 +193,31 @@
                 return CommandApdu(self.CLA, self.INS, self.P1, self.P2, data_field=self.data_field, Ne=Ne)
 
             case CommandCase.Case2E | CommandCase.Case4E:
                 raise ValueError(
                     F"Cannot update Le with APDU {self.case.value}")
 
 
-def APDU(apdu: str | ByteString) -> CommandApdu:
+def CAPDU(apdu: str | ByteString) -> CommandApdu:
+    """CAPDU(): creates a CommandApdu object
+    """
     match apdu:
         case str():
             _apdu = ByteString(apdu)
         case ByteString():
             _apdu = apdu
         case _:
             raise TypeError(
-                F"APDU(): type {type(apdu)} not supported for argument apdu")
+                F"CAPDU(): type {type(apdu)} not supported for argument apdu")
 
     header = _apdu[0:4].blocks(1)
     match len(_apdu):
         case l if l < 4:
             raise ValueError(
-                F'APDU(): wrong Command APDU length, expected 4 or more bytes but received {_apdu}')
+                F'CAPDU(): wrong Command APDU length, expected 4 or more bytes but received {_apdu}')
 
         case 4:
             # Case 1
             return CommandApdu(*header, data_field=None, Ne=None)
 
         case 5:
             # Case 2S
@@ -238,15 +253,15 @@
                 elif len(_apdu) == 7 + int(_apdu[5:7]) + 2:
                     # Case 4E
                     Ne = 65536 if _apdu[-2:] == '0000' else int(_apdu[-2:])
                     return CommandApdu(*header, data_field=_apdu[7:], Ne=None)
 
                 else:
                     raise ValueError(
-                        F'APDU(): wrong Command APDU length: expected {7 + int(_apdu[5:7])} bytes for Case 3e or {7 + int(_apdu[5:7]) + 2} bytes for Case 4e but received {len(_apdu)} bytes instead')
+                        F'RAPDU(): wrong Command APDU length: expected {7 + int(_apdu[5:7])} bytes for Case 3e or {7 + int(_apdu[5:7]) + 2} bytes for Case 4e but received {len(_apdu)} bytes instead')
 
 
 class StatusBytes(ByteString):
     def __init__(self, sw12: ByteString):
         if len(sw12) != 2:
             raise ValueError(F"Expected 2 bytes, received: {sw12}")
 
@@ -454,7 +469,20 @@
     @property
     def SW2(self) -> ByteString:
         return self.SW12[1]
 
     @property
     def StatusBytes(self) -> StatusBytes:
         return self.SW12
+
+
+def RAPDU(apdu: str | ByteString) -> ResponseApdu:
+    """RAPDU(): creates a CommandApdu object
+    """
+    match apdu:
+        case str():
+            return ResponseApdu(ByteString(apdu))
+        case ByteString():
+            return ResponseApdu(apdu)
+        case _:
+            raise TypeError(
+                F"RAPDU(): type {type(apdu)} not supported for argument apdu")
```

### Comparing `gep3-0.4/src/iso7816/commands.py` & `gep3-0.4.1/src/iso7816/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/iso7816/encodings.py` & `gep3-0.4.1/src/iso7816/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/multos/commands.py` & `gep3-0.4.1/src/multos/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/multos/encodings.py` & `gep3-0.4.1/src/multos/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/tests/test_common_ber.py` & `gep3-0.4.1/src/tests/test_common_ber.py`

 * *Files identical despite different names*

### Comparing `gep3-0.4/src/tests/test_crypto_des.py` & `gep3-0.4.1/src/tests/test_crypto_des.py`

 * *Files identical despite different names*

