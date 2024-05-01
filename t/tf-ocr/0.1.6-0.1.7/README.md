# Comparing `tmp/tf_ocr-0.1.6.tar.gz` & `tmp/tf_ocr-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_ocr-0.1.6.tar", last modified: Thu Apr 25 15:40:17 2024, max compression
+gzip compressed data, was "tf_ocr-0.1.7.tar", last modified: Wed May  1 20:15:15 2024, max compression
```

## Comparing `tf_ocr-0.1.6.tar` & `tf_ocr-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.742989 tf_ocr-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 15:40:17.742989 tf_ocr-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-04-25 15:40:13.000000 tf_ocr-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 15:40:17.742989 tf_ocr-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.712988 tf_ocr-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.722988 tf_ocr-0.1.6/src/tf_ocr/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.6/src/tf_ocr/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.6/src/tf_ocr/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.722988 tf_ocr-0.1.6/src/tf_ocr/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.6/src/tf_ocr/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.6/src/tf_ocr/images/images.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.722988 tf_ocr-0.1.6/src/tf_ocr/labels/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.6/src/tf_ocr/labels/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.6/src/tf_ocr/labels/labels.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.732988 tf_ocr-0.1.6/src/tf_ocr/serving/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.6/src/tf_ocr/serving/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.6/src/tf_ocr/serving/pipeline.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.732988 tf_ocr-0.1.6/src/tf_ocr/tfrecords/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 10:21:09.000000 tf_ocr-0.1.6/src/tf_ocr/tfrecords/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-25 10:21:03.000000 tf_ocr-0.1.6/src/tf_ocr/tfrecords/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4408 2024-04-25 15:07:42.000000 tf_ocr-0.1.6/src/tf_ocr/tfrecords/datasets.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-04-25 10:17:45.000000 tf_ocr-0.1.6/src/tf_ocr/tfrecords/examples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      601 2024-04-25 10:15:00.000000 tf_ocr-0.1.6/src/tf_ocr/tfrecords/params.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      636 2024-04-25 10:15:18.000000 tf_ocr-0.1.6/src/tf_ocr/tfrecords/params.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.732988 tf_ocr-0.1.6/src/tf_ocr/utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.6/src/tf_ocr/utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.6/src/tf_ocr/utils/logits.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.6/src/tf_ocr/utils/postprocess.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.742989 tf_ocr-0.1.6/src/tf_ocr/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.6/src/tf_ocr/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.6/src/tf_ocr/vocab/test_vocab.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2169 2024-04-25 15:38:30.000000 tf_ocr-0.1.6/src/tf_ocr/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 15:40:17.742989 tf_ocr-0.1.6/src/tf_ocr.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-04-25 15:40:17.000000 tf_ocr-0.1.6/src/tf_ocr.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      788 2024-04-25 15:40:17.000000 tf_ocr-0.1.6/src/tf_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 15:40:17.000000 tf_ocr-0.1.6/src/tf_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-04-25 15:40:17.000000 tf_ocr-0.1.6/src/tf_ocr.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 15:40:17.000000 tf_ocr-0.1.6/src/tf_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.673931 tf_ocr-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-05-01 20:15:15.673931 tf_ocr-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3304 2024-03-15 09:08:54.000000 tf_ocr-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-05-01 20:15:13.000000 tf_ocr-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-01 20:15:15.673931 tf_ocr-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 16:58:23.000000 tf_ocr-0.1.7/src/tf/ocr/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 06:34:35.000000 tf_ocr-0.1.7/src/tf/ocr/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-04-22 09:02:59.000000 tf_ocr-0.1.7/src/tf/ocr/images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3002 2024-04-22 09:02:46.000000 tf_ocr-0.1.7/src/tf/ocr/images/images.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/labels/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-14 04:50:41.000000 tf_ocr-0.1.7/src/tf/ocr/labels/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-04-24 17:29:16.000000 tf_ocr-0.1.7/src/tf/ocr/labels/labels.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/serving/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-03-15 07:32:33.000000 tf_ocr-0.1.7/src/tf/ocr/serving/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1977 2024-03-15 09:44:36.000000 tf_ocr-0.1.7/src/tf/ocr/serving/pipeline.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/tfrecords/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-25 10:21:09.000000 tf_ocr-0.1.7/src/tf/ocr/tfrecords/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-25 10:21:03.000000 tf_ocr-0.1.7/src/tf/ocr/tfrecords/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4408 2024-04-25 15:07:42.000000 tf_ocr-0.1.7/src/tf/ocr/tfrecords/datasets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-04-25 10:17:45.000000 tf_ocr-0.1.7/src/tf/ocr/tfrecords/examples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      601 2024-04-25 10:15:00.000000 tf_ocr-0.1.7/src/tf/ocr/tfrecords/params.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      636 2024-04-25 10:15:18.000000 tf_ocr-0.1.7/src/tf/ocr/tfrecords/params.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       72 2024-03-15 08:59:17.000000 tf_ocr-0.1.7/src/tf/ocr/utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      729 2024-04-25 06:57:33.000000 tf_ocr-0.1.7/src/tf/ocr/utils/logits.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      802 2024-04-25 06:57:39.000000 tf_ocr-0.1.7/src/tf/ocr/utils/postprocess.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf/ocr/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-03-13 13:27:25.000000 tf_ocr-0.1.7/src/tf/ocr/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-03-13 13:56:11.000000 tf_ocr-0.1.7/src/tf/ocr/vocab/test_vocab.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2166 2024-04-25 15:41:54.000000 tf_ocr-0.1.7/src/tf/ocr/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:15:15.663931 tf_ocr-0.1.7/src/tf_ocr.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3688 2024-05-01 20:15:15.000000 tf_ocr-0.1.7/src/tf_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      788 2024-05-01 20:15:15.000000 tf_ocr-0.1.7/src/tf_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-01 20:15:15.000000 tf_ocr-0.1.7/src/tf_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-05-01 20:15:15.000000 tf_ocr-0.1.7/src/tf_ocr.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-01 20:15:15.000000 tf_ocr-0.1.7/src/tf_ocr.egg-info/top_level.txt
```

### Comparing `tf_ocr-0.1.6/PKG-INFO` & `tf_ocr-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
```

### Comparing `tf_ocr-0.1.6/README.md` & `tf_ocr-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/pyproject.toml` & `tf_ocr-0.1.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-ocr"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     { name="Marcel Claramunt", email="marcel@moveread.com" }
 ]
 description = "Tools for OCR in tensorflow. Typed with `jaxtyping`"
 dependencies = [
     "jaxtyping", "tf-ctc", "tf-tools",
     "tensorflow", "tf-keras", "typing-extensions"
```

### Comparing `tf_ocr-0.1.6/src/tf_ocr/__init__.pyi` & `tf_ocr-0.1.7/src/tf/ocr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/images/images.py` & `tf_ocr-0.1.7/src/tf/ocr/images/images.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/labels/labels.py` & `tf_ocr-0.1.7/src/tf/ocr/labels/labels.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/serving/pipeline.py` & `tf_ocr-0.1.7/src/tf/ocr/serving/pipeline.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/tfrecords/datasets.py` & `tf_ocr-0.1.7/src/tf/ocr/tfrecords/datasets.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/tfrecords/examples.py` & `tf_ocr-0.1.7/src/tf/ocr/tfrecords/examples.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/tfrecords/params.py` & `tf_ocr-0.1.7/src/tf/ocr/tfrecords/params.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/tfrecords/params.pyi` & `tf_ocr-0.1.7/src/tf/ocr/tfrecords/params.pyi`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/utils/logits.py` & `tf_ocr-0.1.7/src/tf/ocr/utils/logits.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/utils/postprocess.py` & `tf_ocr-0.1.7/src/tf/ocr/utils/postprocess.py`

 * *Files identical despite different names*

### Comparing `tf_ocr-0.1.6/src/tf_ocr/vocab/vocab.py` & `tf_ocr-0.1.7/src/tf/ocr/vocab/vocab.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 StringLookup = keras.layers.StringLookup
 import tensorflow as tf
 from jaxtyping import Shaped, Int, Int32
 from haskellian import Thunk
 import string
 
 # VOCABULARY = list("#+-12345678=ABCDFKLNOPQRSTUabcdefghpx")
-VOCABULARY = list("-12345678=ABCDFKLNOPQRSTUabcdefghpxGHW")
+VOCABULARY = list("-12345678=ABCDFKLNOPQRSTUabcdefghpx")
 """Vocabulary used in the original Moveread OCR model: `-12345678=ABCDFKLNOPQRSTUabcdefghpx`"""
 
 NEW_VOCABULARY = list(string.ascii_letters + '12345678' + '-=')
 
 def char2num(vocabulary: list[str] = VOCABULARY) -> Callable[[Shaped[tf.Tensor, "*n"]], Int32[tf.Tensor, "*n"]]:
   """Mapper from characters to indices. Out-of-vocabulary (OOV) characters map to 0"""
   # `mask_token` defaults to ''. If we didn't specify `None`, it would map to 1, and then the vocabulary's chars start at 2
```

### Comparing `tf_ocr-0.1.6/src/tf_ocr.egg-info/PKG-INFO` & `tf_ocr-0.1.7/src/tf_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-ocr
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for OCR in tensorflow. Typed with `jaxtyping`
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-ctc
 Requires-Dist: tf-tools
```

### Comparing `tf_ocr-0.1.6/src/tf_ocr.egg-info/SOURCES.txt` & `tf_ocr-0.1.7/src/tf_ocr.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 README.md
 pyproject.toml
-src/tf_ocr/__init__.py
-src/tf_ocr/__init__.pyi
+src/tf/ocr/__init__.py
+src/tf/ocr/__init__.pyi
+src/tf/ocr/images/__init__.py
+src/tf/ocr/images/images.py
+src/tf/ocr/labels/__init__.py
+src/tf/ocr/labels/labels.py
+src/tf/ocr/serving/__init__.py
+src/tf/ocr/serving/pipeline.py
+src/tf/ocr/tfrecords/__init__.py
+src/tf/ocr/tfrecords/__init__.pyi
+src/tf/ocr/tfrecords/datasets.py
+src/tf/ocr/tfrecords/examples.py
+src/tf/ocr/tfrecords/params.py
+src/tf/ocr/tfrecords/params.pyi
+src/tf/ocr/utils/__init__.py
+src/tf/ocr/utils/logits.py
+src/tf/ocr/utils/postprocess.py
+src/tf/ocr/vocab/__init__.py
+src/tf/ocr/vocab/test_vocab.py
+src/tf/ocr/vocab/vocab.py
 src/tf_ocr.egg-info/PKG-INFO
 src/tf_ocr.egg-info/SOURCES.txt
 src/tf_ocr.egg-info/dependency_links.txt
 src/tf_ocr.egg-info/requires.txt
-src/tf_ocr.egg-info/top_level.txt
-src/tf_ocr/images/__init__.py
-src/tf_ocr/images/images.py
-src/tf_ocr/labels/__init__.py
-src/tf_ocr/labels/labels.py
-src/tf_ocr/serving/__init__.py
-src/tf_ocr/serving/pipeline.py
-src/tf_ocr/tfrecords/__init__.py
-src/tf_ocr/tfrecords/__init__.pyi
-src/tf_ocr/tfrecords/datasets.py
-src/tf_ocr/tfrecords/examples.py
-src/tf_ocr/tfrecords/params.py
-src/tf_ocr/tfrecords/params.pyi
-src/tf_ocr/utils/__init__.py
-src/tf_ocr/utils/logits.py
-src/tf_ocr/utils/postprocess.py
-src/tf_ocr/vocab/__init__.py
-src/tf_ocr/vocab/test_vocab.py
-src/tf_ocr/vocab/vocab.py
+src/tf_ocr.egg-info/top_level.txt
```

