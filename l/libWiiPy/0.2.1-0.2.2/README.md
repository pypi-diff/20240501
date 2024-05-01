# Comparing `tmp/libWiiPy-0.2.1.tar.gz` & `tmp/libwiipy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libWiiPy-0.2.1.tar", last modified: Fri Apr  5 05:07:12 2024, max compression
+gzip compressed data, was "libwiipy-0.2.2.tar", last modified: Wed May  1 03:09:12 2024, max compression
```

## Comparing `libWiiPy-0.2.1.tar` & `libwiipy-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libWiiPy-0.2.1/LICENSE
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4599 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)     3942 2024-04-04 03:07:12.000000 libWiiPy-0.2.1/README.md
--rw-r--r--   0 campbell  (1000) campbell  (1000)      752 2024-04-03 23:07:45.000000 libWiiPy-0.2.1/pyproject.toml
--rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/setup.cfg
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/src/
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/src/libWiiPy/
--rw-r--r--   0 campbell  (1000) campbell  (1000)      350 2024-04-04 01:06:05.000000 libWiiPy-0.2.1/src/libWiiPy/__init__.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/commonkeys.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    16468 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/content.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4301 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/crypto.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     7776 2024-04-05 04:04:30.000000 libWiiPy-0.2.1/src/libWiiPy/nus.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1181 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/shared.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    11921 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/ticket.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     9062 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/title.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    13738 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/tmd.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/types.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    12515 2024-04-05 05:06:09.000000 libWiiPy-0.2.1/src/libWiiPy/wad.py
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/src/libWiiPy.egg-info/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4599 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)      460 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/SOURCES.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/dependency_links.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)       21 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/requires.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/top_level.txt
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.989026 libwiipy-0.2.2/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libwiipy-0.2.2/LICENSE
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4600 2024-05-01 03:09:12.989026 libwiipy-0.2.2/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     3942 2024-04-04 03:07:12.000000 libwiipy-0.2.2/README.md
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      753 2024-05-01 03:08:41.000000 libwiipy-0.2.2/pyproject.toml
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-05-01 03:09:12.989026 libwiipy-0.2.2/setup.cfg
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.982360 libwiipy-0.2.2/src/
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.985693 libwiipy-0.2.2/src/libWiiPy/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      350 2024-04-04 01:06:05.000000 libwiipy-0.2.2/src/libWiiPy/__init__.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-14 16:45:16.000000 libwiipy-0.2.2/src/libWiiPy/commonkeys.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    16468 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/content.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4264 2024-04-07 00:18:51.000000 libwiipy-0.2.2/src/libWiiPy/crypto.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     7824 2024-05-01 03:08:41.000000 libwiipy-0.2.2/src/libWiiPy/nus.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1181 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/shared.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    11921 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/ticket.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     9216 2024-04-14 16:53:37.000000 libwiipy-0.2.2/src/libWiiPy/title.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    13730 2024-04-27 01:34:39.000000 libwiipy-0.2.2/src/libWiiPy/tmd.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/types.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    12515 2024-04-05 05:06:09.000000 libwiipy-0.2.2/src/libWiiPy/wad.py
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.989026 libwiipy-0.2.2/src/libWiiPy.egg-info/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4600 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      460 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       22 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/requires.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/top_level.txt
```

### Comparing `libWiiPy-0.2.1/LICENSE` & `libwiipy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/PKG-INFO` & `libwiipy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: libWiiPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A modern Python library for handling files used by the Wii
 Author-email: NinjaCheetah <ninjacheetah@ncxprogramming.com>, Lillian Skinner <lillian@randommeaninglesscharacters.com>
 Project-URL: Homepage, https://github.com/NinjaCheetah/libWiiPy
 Project-URL: Issues, https://github.com/NinjaCheetah/libWiipy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome
-Requires-Dist: urllib3
+Requires-Dist: requests
 
 ![libWiiPy](https://github.com/NinjaCheetah/libWiiPy/assets/58050615/80093c68-b86e-4b96-87b7-db3855382ca8)
 # libWiiPy
 libWiiPy is a modern Python 3 library for interacting with and editing files from the Wii. It aims to be simple to use, well maintained, and offer as many features as reasonably possible in one library, so that a newly-written Python program could reasonably do 100% of its Wii-related work with just one library. It also aims to be fully cross-platform, so that any tools written with it can also be cross-platform.
 
 libWiiPy is inspired by [libWiiSharp](https://github.com/TheShadowEevee/libWiiSharp), originally created by `Leathl`, now maintained by [@TheShadowEevee](https://github.com/TheShadowEevee). libWiiSharp is absolutely the way to go if you need a C# library for Wii files.
```

### Comparing `libWiiPy-0.2.1/README.md` & `libwiipy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/pyproject.toml` & `libwiipy-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "libWiiPy"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name="NinjaCheetah", email="ninjacheetah@ncxprogramming.com" },
     { name="Lillian Skinner", email="lillian@randommeaninglesscharacters.com" }
 ]
 description = "A modern Python library for handling files used by the Wii"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pycryptodome",
-    "urllib3"
+    "requests"
 ]
 
 [project.urls]
 Homepage = "https://github.com/NinjaCheetah/libWiiPy"
 Issues = "https://github.com/NinjaCheetah/libWiipy/issues"
 
 [build-system]
```

### Comparing `libWiiPy-0.2.1/src/libWiiPy/commonkeys.py` & `libwiipy-0.2.2/src/libWiiPy/commonkeys.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/src/libWiiPy/content.py` & `libwiipy-0.2.2/src/libWiiPy/content.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/src/libWiiPy/crypto.py` & `libwiipy-0.2.2/src/libWiiPy/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,15 @@
     if (len(content_enc) % 16) != 0:
         content_enc = content_enc + (b'\x00' * (16 - (len(content_enc) % 16)))
     # Create a new AES object with the values provided, with the content's unique ID as the IV.
     aes = AES.new(title_key, AES.MODE_CBC, content_index_bin)
     # Decrypt the content using the AES object.
     content_dec = aes.decrypt(content_enc)
     # Trim additional bytes that may have been added so the content is the correct size.
-    while len(content_dec) > content_length:
-        content_dec = content_dec[:-1]
+    content_dec = content_dec[:content_length]
     return content_dec
 
 
 def encrypt_content(content_dec, title_key, content_index) -> bytes:
     """
     Gets the encrypted version of the decrypted content.
```

### Comparing `libWiiPy-0.2.1/src/libWiiPy/nus.py` & `libwiipy-0.2.2/src/libWiiPy/nus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # "nus.py" from libWiiPy by NinjaCheetah & Contributors
 # https://github.com/NinjaCheetah/libWiiPy
 #
 # See https://wiibrew.org/wiki/NUS for details about the NUS
 
 import io
-import urllib3
+import requests
 import hashlib
 from typing import List
 from .title import Title
 from .tmd import TMD
 from .ticket import Ticket
 
 
@@ -58,26 +58,26 @@
     Returns
     -------
     bytes
         The TMD file from the NUS.
     """
     # Build the download URL. The structure is download/<TID>/tmd for latest and download/<TID>/tmd.<version> for
     # when a specific version is requested.
-    tmd_url = "http://ccs.shop.wii.com/ccs/download/" + title_id + "/tmd"
+    tmd_url = "http://nus.cdn.shop.wii.com/ccs/download/" + title_id + "/tmd"
     # Add the version to the URL if one was specified.
     if title_version is not None:
         tmd_url += "." + str(title_version)
     # Make the request.
-    tmd_response = urllib3.request(method='GET', url=tmd_url, headers={'User-Agent': 'wii libnup/1.0'})
+    tmd_request = requests.get(url=tmd_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True)
     # Handle a 404 if the TID/version doesn't exist.
-    if tmd_response.status != 200:
+    if tmd_request.status_code != 200:
         raise ValueError("The requested Title ID or TMD version does not exist. Please check the Title ID and Title"
                          " version and then try again.")
     # Save the raw TMD.
-    raw_tmd = tmd_response.data
+    raw_tmd = tmd_request.content
     # Use a TMD object to load the data and then return only the actual TMD.
     tmd_temp = TMD()
     tmd_temp.load(raw_tmd)
     tmd = tmd_temp.dump()
     return tmd
 
 
@@ -94,22 +94,22 @@
     Returns
     -------
     bytes
         The Ticket file from the NUS.
     """
     # Build the download URL. The structure is download/<TID>/cetk, and cetk will only exist if this is a free
     # title.
-    ticket_url = "http://ccs.shop.wii.com/ccs/download/" + title_id + "/cetk"
+    ticket_url = "http://nus.cdn.shop.wii.com/ccs/download/" + title_id + "/cetk"
     # Make the request.
-    ticket_response = urllib3.request(method='GET', url=ticket_url, headers={'User-Agent': 'wii libnup/1.0'})
-    if ticket_response.status != 200:
+    ticket_request = requests.get(url=ticket_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True)
+    if ticket_request.status_code != 200:
         raise ValueError("The requested Title ID does not exist, or refers to a non-free title. Tickets can only"
                          " be downloaded for titles that are free on the NUS.")
     # Save the raw cetk file.
-    cetk = ticket_response.data
+    cetk = ticket_request.content
     # Use a Ticket object to load only the Ticket data from cetk and return it.
     ticket_temp = Ticket()
     ticket_temp.load(cetk)
     ticket = ticket_temp.dump()
     return ticket
 
 
@@ -119,18 +119,18 @@
 
     Returns
     -------
     bytes
         The cert file.
     """
     # Download the TMD and cetk for the System Menu 4.3U.
-    tmd = urllib3.request(method='GET', url='http://ccs.shop.wii.com/ccs/download/0000000100000002/tmd.513',
-                          headers={'User-Agent': 'wii libnup/1.0'}).data
-    cetk = urllib3.request(method='GET', url='http://ccs.shop.wii.com/ccs/download/0000000100000002/cetk',
-                           headers={'User-Agent': 'wii libnup/1.0'}).data
+    tmd = requests.get(url='http://nus.cdn.shop.wii.com/ccs/download/0000000100000002/tmd.513',
+                       headers={'User-Agent': 'wii libnup/1.0'}, stream=True).content
+    cetk = requests.get(url='http://nus.cdn.shop.wii.com/ccs/download/0000000100000002/cetk',
+                        headers={'User-Agent': 'wii libnup/1.0'}, stream=True).content
     # Assemble the certificate.
     with io.BytesIO() as cert_data:
         # Certificate Authority data.
         cert_data.write(cetk[0x2A4 + 768:])
         # Certificate Policy data.
         cert_data.write(tmd[0x328:0x328 + 768])
         # XS data.
@@ -159,22 +159,23 @@
     bytes
         The downloaded content.
     """
     # Build the download URL. The structure is download/<TID>/<Content ID>.
     content_id_hex = hex(content_id)[2:]
     if len(content_id_hex) < 2:
         content_id_hex = "0" + content_id_hex
-    content_url = "http://ccs.shop.wii.com/ccs/download/" + title_id + "/000000" + content_id_hex
+    content_url = "http://nus.cdn.shop.wii.com/ccs/download/" + title_id + "/000000" + content_id_hex
     # Make the request.
-    content_response = urllib3.request(method='GET', url=content_url, headers={'User-Agent': 'wii libnup/1.0'})
-    if content_response.status != 200:
+    content_request = requests.get(url=content_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True)
+    if content_request.status_code != 200:
         raise ValueError("The requested Title ID does not exist, or an invalid Content ID is present in the"
                          " content records provided.\n Failed while downloading Content ID: 000000" +
                          content_id_hex)
-    return content_response.data
+    content_data = content_request.content
+    return content_data
 
 
 def download_contents(title_id: str, tmd: TMD) -> List[bytes]:
     """
     Downloads all the contents for the title specified in the object. This requires a TMD to already be available
     so that the content records can be accessed.
```

### Comparing `libWiiPy-0.2.1/src/libWiiPy/shared.py` & `libwiipy-0.2.2/src/libWiiPy/shared.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/src/libWiiPy/ticket.py` & `libwiipy-0.2.2/src/libWiiPy/ticket.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/src/libWiiPy/title.py` & `libwiipy-0.2.2/src/libWiiPy/title.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         into raw data and returns it.
 
         Returns
         -------
         wad_data : bytes
             The raw data of the WAD.
         """
+        # Set WAD type to ib if the title being packed is boot2.
+        if self.tmd.title_id == "0000000100000001":
+            self.wad.wad_type = "ib"
         # Dump the TMD and set it in the WAD.
         self.wad.set_tmd_data(self.tmd.dump())
         # Dump the Ticket and set it in the WAD.
         self.wad.set_ticket_data(self.ticket.dump())
         # Dump the ContentRegion and set it in the WAD.
         self.wad.set_content_data(self.content.dump())
         # Dump the WAD with the new regions back into raw data and return it.
```

### Comparing `libWiiPy-0.2.1/src/libWiiPy/tmd.py` & `libwiipy-0.2.2/src/libWiiPy/tmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             return False
 
     def get_title_type(self) -> str:
         """
         Gets the type of the TMD's associated title.
 
         Can be one of several possible values:
-        'System', 'Game', 'Channel', 'SystemChannel', 'GameWithChannel', or 'HiddenChannel'
+        'System', 'Game', 'Channel', 'SystemChannel', 'GameChannel', or 'HiddenChannel'
 
         Returns
         -------
         str
             The type of the title.
         """
         title_id_high = self.title_id[:8]
@@ -271,15 +271,15 @@
             case '00010000':
                 return "Game"
             case '00010001':
                 return "Channel"
             case '00010002':
                 return "SystemChannel"
             case '00010004':
-                return "GameWithChannel"
+                return "GameChannel"
             case '00010005':
                 return "DLC"
             case '00010008':
                 return "HiddenChannel"
             case _:
                 return "Unknown"
```

### Comparing `libWiiPy-0.2.1/src/libWiiPy/types.py` & `libwiipy-0.2.2/src/libWiiPy/types.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/src/libWiiPy/wad.py` & `libwiipy-0.2.2/src/libWiiPy/wad.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.1/src/libWiiPy.egg-info/PKG-INFO` & `libwiipy-0.2.2/src/libWiiPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: libWiiPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A modern Python library for handling files used by the Wii
 Author-email: NinjaCheetah <ninjacheetah@ncxprogramming.com>, Lillian Skinner <lillian@randommeaninglesscharacters.com>
 Project-URL: Homepage, https://github.com/NinjaCheetah/libWiiPy
 Project-URL: Issues, https://github.com/NinjaCheetah/libWiipy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome
-Requires-Dist: urllib3
+Requires-Dist: requests
 
 ![libWiiPy](https://github.com/NinjaCheetah/libWiiPy/assets/58050615/80093c68-b86e-4b96-87b7-db3855382ca8)
 # libWiiPy
 libWiiPy is a modern Python 3 library for interacting with and editing files from the Wii. It aims to be simple to use, well maintained, and offer as many features as reasonably possible in one library, so that a newly-written Python program could reasonably do 100% of its Wii-related work with just one library. It also aims to be fully cross-platform, so that any tools written with it can also be cross-platform.
 
 libWiiPy is inspired by [libWiiSharp](https://github.com/TheShadowEevee/libWiiSharp), originally created by `Leathl`, now maintained by [@TheShadowEevee](https://github.com/TheShadowEevee). libWiiSharp is absolutely the way to go if you need a C# library for Wii files.
```

