# Comparing `tmp/sora_sdk-2024.2.0.dev2.tar.gz` & `tmp/sora_sdk-2024.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sora_sdk-2024.2.0.dev2.tar", last modified: Mon Apr  1 11:17:56 2024, max compression
+gzip compressed data, was "sora_sdk-2024.3.0.dev0.tar", last modified: Wed May  1 06:30:54 2024, max compression
```

## Comparing `sora_sdk-2024.2.0.dev2.tar` & `sora_sdk-2024.3.0.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-01 11:17:56.732118 sora_sdk-2024.2.0.dev2/
--rw-r--r--   0 runner     (501) staff       (20)    10174 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       33 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    31624 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/NOTICE.md
--rw-r--r--   0 runner     (501) staff       (20)    17809 2024-04-01 11:17:56.731205 sora_sdk-2024.2.0.dev2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     5334 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/README.md
--rw-r--r--   0 runner     (501) staff       (20)    10395 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/pypath.py
--rw-r--r--   0 runner     (501) staff       (20)     3762 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)    29155 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/run.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-01 11:17:56.732239 sora_sdk-2024.2.0.dev2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1893 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-01 11:17:56.695693 sora_sdk-2024.2.0.dev2/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-01 11:17:56.701019 sora_sdk-2024.2.0.dev2/src/sora_sdk/
--rw-r--r--   0 runner     (501) staff       (20)     1180 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/src/sora_sdk/__init__.py
--rw-r--r--   0 runner     (501) staff       (20) 14367024 2024-04-01 11:17:47.000000 sora_sdk-2024.2.0.dev2/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-01 11:17:56.730226 sora_sdk-2024.2.0.dev2/src/sora_sdk.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    17809 2024-04-01 11:17:56.000000 sora_sdk-2024.2.0.dev2/src/sora_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      319 2024-04-01 11:17:56.000000 sora_sdk-2024.2.0.dev2/src/sora_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-01 11:17:56.000000 sora_sdk-2024.2.0.dev2/src/sora_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-01 11:17:56.000000 sora_sdk-2024.2.0.dev2/src/sora_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-01 11:17:56.728274 sora_sdk-2024.2.0.dev2/tests/
--rw-r--r--   0 runner     (501) staff       (20)      596 2024-04-01 11:12:51.000000 sora_sdk-2024.2.0.dev2/tests/test_recvonly.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.630010 sora_sdk-2024.3.0.dev0/
+-rw-r--r--   0 runner     (501) staff       (20)    10174 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       33 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    31624 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/NOTICE.md
+-rw-r--r--   0 runner     (501) staff       (20)    17906 2024-05-01 06:30:54.629547 sora_sdk-2024.3.0.dev0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     5431 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    10395 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/pypath.py
+-rw-r--r--   0 runner     (501) staff       (20)     3741 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)    29155 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/run.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-01 06:30:54.630094 sora_sdk-2024.3.0.dev0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1893 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.606643 sora_sdk-2024.3.0.dev0/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.610005 sora_sdk-2024.3.0.dev0/src/sora_sdk/
+-rw-r--r--   0 runner     (501) staff       (20)     1180 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20) 14367024 2024-05-01 06:30:47.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.628927 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    17906 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      319 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.628526 sora_sdk-2024.3.0.dev0/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      596 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/tests/test_recvonly.py
```

### Comparing `sora_sdk-2024.2.0.dev2/LICENSE` & `sora_sdk-2024.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.2.0.dev2/NOTICE.md` & `sora_sdk-2024.3.0.dev0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.2.0.dev2/PKG-INFO` & `sora_sdk-2024.3.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sora_sdk
-Version: 2024.2.0.dev2
+Version: 2024.3.0.dev0
 Summary: WebRTC SFU Sora Python SDK
 Home-page: https://github.com/shiguredo/sora-python-sdk
 Author-email: "Shiguredo Inc." <contact+pypi@shiguredo.jp>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -289,14 +289,16 @@
 
 優先実装とは Sora のライセンスを契約頂いているお客様向けに Sora Python SDK の実装予定機能を有償にて前倒しで実装することです。
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
 - DataChannel 対応
   - [アダワープジャパン株式会社](https://adawarp.com/) 様
+- Intel VPL H.265 対応
+  - [アダワープジャパン株式会社](https://adawarp.com/) 様
 
 ### 優先実装が可能な機能一覧
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
 - Ubuntu 22.04 arm64
   - Python 3.10
```

### Comparing `sora_sdk-2024.2.0.dev2/README.md` & `sora_sdk-2024.3.0.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,16 @@
 
 優先実装とは Sora のライセンスを契約頂いているお客様向けに Sora Python SDK の実装予定機能を有償にて前倒しで実装することです。
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
 - DataChannel 対応
   - [アダワープジャパン株式会社](https://adawarp.com/) 様
+- Intel VPL H.265 対応
+  - [アダワープジャパン株式会社](https://adawarp.com/) 様
 
 ### 優先実装が可能な機能一覧
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
 - Ubuntu 22.04 arm64
   - Python 3.10
```

### Comparing `sora_sdk-2024.2.0.dev2/pypath.py` & `sora_sdk-2024.3.0.dev0/pypath.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.2.0.dev2/pyproject.toml` & `sora_sdk-2024.3.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "sora_sdk"
 authors = [{ name = "Shiguredo Inc.", email = "contact+pypi@shiguredo.jp" }]
-version = "2024.2.0.dev2"
+version = "2024.3.0.dev0"
 description = "WebRTC SFU Sora Python SDK"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
@@ -58,14 +58,13 @@
 [tool.rye]
 dev-dependencies = [
     "nanobind~=1.9.2",
     "setuptools>=69.2",
     "build~=1.1.1",
     "wheel~=0.43.0",
     "auditwheel~=6.0.0",
-    "pytest>=8.0.0",
-    "ruff>=0.3.0",
+    "pytest>=8.2",
+    "ruff>=0.4",
 ]
 
 [tool.ruff]
 line-length = 100
-indent-width = 4
```

### Comparing `sora_sdk-2024.2.0.dev2/run.py` & `sora_sdk-2024.3.0.dev0/run.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.2.0.dev2/setup.py` & `sora_sdk-2024.3.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.2.0.dev2/src/sora_sdk/__init__.py` & `sora_sdk-2024.3.0.dev0/src/sora_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.2.0.dev2/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so` & `sora_sdk-2024.3.0.dev0/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### strings -a -n 8 {}

```diff
@@ -3686,15 +3686,15 @@
 nLRbwHOoq7hHwg==
 -----END CERTIFICATE-----
 default cert file: 
 X509_STORE_CTX_new failed
 X509_STORE_CTX_init failed
 X509_verify_cert failed: r=
  message=
-Sora C++ SDK 2024.6.0 (49fdb4ac)
+Sora C++ SDK 2024.6.1 (61c89e2c)
 Shiguredo-Build M122.6261@{#1} (122.6261.1.0 6b419a05)
 Unknown Environment
 unknown arch
 Unknown OS
 /Users/runner/work/sora-cpp-sdk/sora-cpp-sdk/src/websocket.cpp
 Websocket::~Websocket this=
  resolved=
```

#### aarch64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit arm64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|WEAK_DEFINES|BINDS_TO_WEAK|HAS_TLV_DESCRIPTORS>*

```diff
@@ -193,15 +193,15 @@
 00000c00: 0200 0000 1800 0000 9821 d500 da0e 0000  .........!......
 00000c10: d024 d600 b060 0300 0b00 0000 5000 0000  .$...`......P...
 00000c20: 0000 0000 0000 0000 0000 0000 e10b 0000  ................
 00000c30: e10b 0000 f902 0000 0000 0000 0000 0000  ................
 00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c50: 380f d600 6505 0000 0000 0000 0000 0000  8...e...........
 00000c60: 0000 0000 0000 0000 1b00 0000 1800 0000  ................
-00000c70: 1c6d c7a8 542e 3e7a a73d 0128 b68f 1d88  .m..T.>z.=.(....
+00000c70: 8342 63ee eeb9 3a65 baac 3fc1 dbcf 6a0c  .Bc...:e..?...j.
 00000c80: 3200 0000 2000 0000 0100 0000 0006 0d00  2... ...........
 00000c90: 0000 0e00 0100 0000 0300 0000 0007 f703  ................
 00000ca0: 2a00 0000 1000 0000 0000 0000 0000 0000  *...............
 00000cb0: 0c00 0000 6800 0000 1800 0000 0200 0000  ....h...........
 00000cc0: 0000 0200 0000 0100 2f53 7973 7465 6d2f  ......../System/
 00000cd0: 4c69 6272 6172 792f 4672 616d 6577 6f72  Library/Framewor
 00000ce0: 6b73 2f41 5646 6f75 6e64 6174 696f 6e2e  ks/AVFoundation.
@@ -727504,16 +727504,16 @@
 00b19cf0: 6c65 3a20 0058 3530 395f 5354 4f52 455f  le: .X509_STORE_
 00b19d00: 4354 585f 6e65 7720 6661 696c 6564 0058  CTX_new failed.X
 00b19d10: 3530 395f 5354 4f52 455f 4354 585f 696e  509_STORE_CTX_in
 00b19d20: 6974 2066 6169 6c65 6400 5835 3039 5f76  it failed.X509_v
 00b19d30: 6572 6966 795f 6365 7274 2066 6169 6c65  erify_cert faile
 00b19d40: 643a 2072 3d00 206d 6573 7361 6765 3d00  d: r=. message=.
 00b19d50: 6874 7470 7300 536f 7261 2043 2b2b 2053  https.Sora C++ S
-00b19d60: 444b 2032 3032 342e 362e 3020 2834 3966  DK 2024.6.0 (49f
-00b19d70: 6462 3461 6329 0053 6869 6775 7265 646f  db4ac).Shiguredo
+00b19d60: 444b 2032 3032 342e 362e 3120 2836 3163  DK 2024.6.1 (61c
+00b19d70: 3839 6532 6329 0053 6869 6775 7265 646f  89e2c).Shiguredo
 00b19d80: 2d42 7569 6c64 204d 3132 322e 3632 3631  -Build M122.6261
 00b19d90: 407b 2331 7d20 2831 3232 2e36 3236 312e  @{#1} (122.6261.
 00b19da0: 312e 3020 3662 3431 3961 3035 2900 556e  1.0 6b419a05).Un
 00b19db0: 6b6e 6f77 6e20 456e 7669 726f 6e6d 656e  known Environmen
 00b19dc0: 7400 756e 6b6e 6f77 6e20 6172 6368 0055  t.unknown arch.U
 00b19dd0: 6e6b 6e6f 776e 204f 5300 5d20 002f 5573  nknown OS.] ./Us
 00b19de0: 6572 732f 7275 6e6e 6572 2f77 6f72 6b2f  ers/runner/work/
@@ -890970,17 +890970,17 @@
 00d98590: 0000 0014 fade 0c02 0001 b39a 0002 0400  ................
 00d985a0: 0002 0002 0000 007a 0000 0058 0000 0000  .......z...X....
 00d985b0: 0000 0d99 00d9 8580 2002 000c 0000 0000  ........ .......
 00d985c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00d985d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00d985e0: 00ad f950 0000 0000 0000 0000 736f 7261  ...P........sora
 00d985f0: 5f73 646b 5f65 7874 2e63 7079 7468 6f6e  _sdk_ext.cpython
-00d98600: 2d33 382d 6461 7277 696e 2e73 6f00 6c56  -38-darwin.so.lV
-00d98610: d18e 6bd5 99a6 a4fc ba1d 65f4 a105 a763  ..k.......e....c
-00d98620: 30a1 b0f6 7a28 2047 5d95 8db7 f87c 9eb8  0...z( G]....|..
+00d98600: 2d33 382d 6461 7277 696e 2e73 6f00 a1f7  -38-darwin.so...
+00d98610: 7743 ff5d 4a26 3d37 0015 5cfb b526 0ddd  wC.]J&=7..\..&..
+00d98620: 0c08 bc60 ccc6 8956 8904 885b 130d 9eb8  ...`...V...[....
 00d98630: 98f9 3981 cbff cabb eb57 563b c325 9e97  ..9......WV;.%..
 00d98640: 7d8e c084 3a43 afb3 0f48 5779 60d9 ad7f  }...:C...HWy`...
 00d98650: acb2 586f c6e9 66c0 04d7 d1d1 6b02 4f58  ..Xo..f.....k.OX
 00d98660: 05ff 7cb4 7c7a 85da bd8b 4889 2ca7 ad7f  ..|.|z....H.,...
 00d98670: acb2 586f c6e9 66c0 04d7 d1d1 6b02 4f58  ..Xo..f.....k.OX
 00d98680: 05ff 7cb4 7c7a 85da bd8b 4889 2ca7 ad7f  ..|.|z....H.,...
 00d98690: acb2 586f c6e9 66c0 04d7 d1d1 6b02 4f58  ..Xo..f.....k.OX
@@ -896652,17 +896652,17 @@
 00dae8b0: cb49 da8b 23eb ae28 d1e1 6fa2 0664 b37c  .I..#..(..o..d.|
 00dae8c0: b301 dcd0 c5d9 7031 e6b1 65d8 dad4 af67  ......p1..e....g
 00dae8d0: b22d 572e 8cb5 a725 2c79 6346 22f6 3a21  .-W....%,ycF".:!
 00dae8e0: 84d1 8a99 bbd5 dbf8 f715 94c2 eb6e 2f46  .............n/F
 00dae8f0: fcde 9188 97c9 b7ac 32c2 f403 298f 8605  ........2...)...
 00dae900: a459 2aab f08a a0e2 0ba7 d2dd 3a27 e7b6  .Y*.........:'..
 00dae910: 0aa3 a0a6 1fb9 b0a8 9b2c f013 ef2f cefd  .........,.../..
-00dae920: f11d b7fa bcd9 6c1c 7fb8 ce34 6394 48b7  ......l....4c.H.
-00dae930: 632c 5c84 e926 c055 ad4c ad24 77bd bcb7  c,\..&.U.L.$w...
-00dae940: e7ea e84f 3ec6 07a6 43d7 3d4e b89b c4d1  ...O>...C.=N....
+00dae920: f11d b7fa bcd9 6c1c 7fb8 ce34 6394 869e  ......l....4c...
+00dae930: 4df7 20af f850 7c7d ec59 c6fe b778 566c  M. ..P|}.Y...xVl
+00dae940: fbf3 a62d 8eef 6385 a77f 2e13 210e c4d1  ...-..c.....!...
 00dae950: d244 f4fa 8f1a c934 7bdf 8ced e7b3 5daf  .D.....4{.....].
 00dae960: 5ffe 550a cdb3 9133 68ec ad8d 493b 800c  _.U....3h...I;..
 00dae970: cde1 3766 5ce6 23ca e938 bbf3 c357 fcf1  ..7f\.#..8...W..
 00dae980: f1ce 13b0 7389 e48a c1a1 774d 9842 c733  ....s.....wM.B.3
 00dae990: f425 1ec8 0353 5e44 8a68 bb2e bcfe f754  .%...S^D.h.....T
 00dae9a0: b3d3 436c c7dd efd2 791d 7874 cb80 9ddc  ..Cl....y.xt....
 00dae9b0: 3562 cc54 ab7b 1759 9528 283f 8d7c 5fdb  5b.T.{.Y.((?.|_.
```

### Comparing `sora_sdk-2024.2.0.dev2/src/sora_sdk.egg-info/PKG-INFO` & `sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sora_sdk
-Version: 2024.2.0.dev2
+Version: 2024.3.0.dev0
 Summary: WebRTC SFU Sora Python SDK
 Home-page: https://github.com/shiguredo/sora-python-sdk
 Author-email: "Shiguredo Inc." <contact+pypi@shiguredo.jp>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -289,14 +289,16 @@
 
 優先実装とは Sora のライセンスを契約頂いているお客様向けに Sora Python SDK の実装予定機能を有償にて前倒しで実装することです。
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
 - DataChannel 対応
   - [アダワープジャパン株式会社](https://adawarp.com/) 様
+- Intel VPL H.265 対応
+  - [アダワープジャパン株式会社](https://adawarp.com/) 様
 
 ### 優先実装が可能な機能一覧
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
 - Ubuntu 22.04 arm64
   - Python 3.10
```

### Comparing `sora_sdk-2024.2.0.dev2/tests/test_recvonly.py` & `sora_sdk-2024.3.0.dev0/tests/test_recvonly.py`

 * *Files identical despite different names*

