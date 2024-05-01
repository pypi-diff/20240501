# Comparing `tmp/audiostack-1.2.4.tar.gz` & `tmp/audiostack-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-1.2.4.tar", last modified: Mon Apr 22 11:20:29 2024, max compression
+gzip compressed data, was "audiostack-1.2.5.tar", last modified: Wed May  1 09:11:43 2024, max compression
```

## Comparing `audiostack-1.2.4.tar` & `audiostack-1.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.334190 audiostack-1.2.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-04-22 11:20:01.000000 audiostack-1.2.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-04-22 11:20:29.334190 audiostack-1.2.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-04-22 11:20:01.000000 audiostack-1.2.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.330190 audiostack-1.2.4/audiostack/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-04-22 11:20:22.000000 audiostack-1.2.4/audiostack/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.330190 audiostack-1.2.4/audiostack/content/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/content/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/content/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/content/media.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/content/recommend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/content/root_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/content/script.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.330190 audiostack-1.2.4/audiostack/delivery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/delivery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3460 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/delivery/encoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/delivery/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.330190 audiostack-1.2.4/audiostack/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/docs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/docs/docs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.334190 audiostack-1.2.4/audiostack/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/api_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/api_list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/request_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/request_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/helpers/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.334190 audiostack-1.2.4/audiostack/orchestrator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.334190 audiostack-1.2.4/audiostack/production/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/production/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4703 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/production/mix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/production/sound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/production/suite.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.334190 audiostack-1.2.4/audiostack/speech/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/speech/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/speech/diction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/speech/predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/speech/tts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-04-22 11:20:01.000000 audiostack-1.2.4/audiostack/speech/voice.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 11:20:29.334190 audiostack-1.2.4/audiostack.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-04-22 11:20:29.000000 audiostack-1.2.4/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-04-22 11:20:29.000000 audiostack-1.2.4/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-22 11:20:29.000000 audiostack-1.2.4/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-04-22 11:20:29.000000 audiostack-1.2.4/audiostack.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-04-22 11:20:29.000000 audiostack-1.2.4/audiostack.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-22 11:20:29.334190 audiostack-1.2.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-04-22 11:20:01.000000 audiostack-1.2.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.667961 audiostack-1.2.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-05-01 09:11:22.000000 audiostack-1.2.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-01 09:11:43.667961 audiostack-1.2.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-05-01 09:11:22.000000 audiostack-1.2.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.659961 audiostack-1.2.5/audiostack/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-05-01 09:11:38.000000 audiostack-1.2.5/audiostack/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/content/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/media.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/recommend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/root_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/script.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/delivery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/delivery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3460 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/delivery/encoder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/delivery/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/docs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/docs/docs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/helpers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/api_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/api_list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/request_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/request_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/orchestrator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/production/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4703 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/mix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/sound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/suite.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/speech/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/diction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/predict.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/tts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/voice.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-01 09:11:43.667961 audiostack-1.2.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-05-01 09:11:22.000000 audiostack-1.2.5/setup.py
```

### Comparing `audiostack-1.2.4/LICENSE` & `audiostack-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/PKG-INFO` & `audiostack-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.2.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.2.5 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
```

### Comparing `audiostack-1.2.4/README.md` & `audiostack-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/content/__init__.py` & `audiostack-1.2.5/audiostack/content/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/content/file.py` & `audiostack-1.2.5/audiostack/content/file.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/content/media.py` & `audiostack-1.2.5/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/content/recommend.py` & `audiostack-1.2.5/audiostack/content/recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/content/root_functions.py` & `audiostack-1.2.5/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/content/script.py` & `audiostack-1.2.5/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/delivery/encoder.py` & `audiostack-1.2.5/audiostack/delivery/encoder.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/delivery/video.py` & `audiostack-1.2.5/audiostack/delivery/video.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/docs/docs.py` & `audiostack-1.2.5/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/helpers/api_item.py` & `audiostack-1.2.5/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/helpers/api_list.py` & `audiostack-1.2.5/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/helpers/request_interface.py` & `audiostack-1.2.5/audiostack/helpers/request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/production/mix.py` & `audiostack-1.2.5/audiostack/production/mix.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/production/sound.py` & `audiostack-1.2.5/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/production/suite.py` & `audiostack-1.2.5/audiostack/production/suite.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/speech/diction.py` & `audiostack-1.2.5/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/speech/predict.py` & `audiostack-1.2.5/audiostack/speech/predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/speech/tts.py` & `audiostack-1.2.5/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack/speech/voice.py` & `audiostack-1.2.5/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/audiostack.egg-info/PKG-INFO` & `audiostack-1.2.5/audiostack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.2.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.2.5 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
```

### Comparing `audiostack-1.2.4/audiostack.egg-info/SOURCES.txt` & `audiostack-1.2.5/audiostack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.4/setup.py` & `audiostack-1.2.5/setup.py`

 * *Files identical despite different names*

