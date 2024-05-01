# Comparing `tmp/tf_ctc-0.1.5.tar.gz` & `tmp/tf_ctc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_ctc-0.1.5.tar", last modified: Thu Apr 25 07:41:21 2024, max compression
+gzip compressed data, was "tf_ctc-0.1.6.tar", last modified: Wed May  1 20:13:50 2024, max compression
```

## Comparing `tf_ctc-0.1.5.tar` & `tf_ctc-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3776 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3388 2024-03-14 10:50:47.000000 tf_ctc-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-04-25 07:41:19.000000 tf_ctc-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.354241 tf_ctc-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.354241 tf_ctc-0.1.5/src/tf_ctc/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      187 2024-04-22 05:26:08.000000 tf_ctc-0.1.5/src/tf_ctc/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3824 2024-04-22 05:28:09.000000 tf_ctc-0.1.5/src/tf_ctc/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2780 2024-04-22 05:25:31.000000 tf_ctc-0.1.5/src/tf_ctc/logits.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      594 2024-04-24 17:12:39.000000 tf_ctc-0.1.5/src/tf_ctc/loss_.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1647 2024-04-22 05:39:27.000000 tf_ctc-0.1.5/src/tf_ctc/metrics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-04-22 05:25:42.000000 tf_ctc-0.1.5/src/tf_ctc/test.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/src/tf_ctc/tests/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      935 2024-03-14 06:02:21.000000 tf_ctc-0.1.5/src/tf_ctc/tests/test_decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-03-14 05:40:16.000000 tf_ctc-0.1.5/src/tf_ctc/tests/test_loss.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      897 2024-03-14 09:49:15.000000 tf_ctc-0.1.5/src/tf_ctc/tests/test_metrics.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:41:21.364241 tf_ctc-0.1.5/src/tf_ctc.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3776 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      418 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       56 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-04-25 07:41:21.000000 tf_ctc-0.1.5/src/tf_ctc.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:13:50.053579 tf_ctc-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3897 2024-05-01 20:13:50.053579 tf_ctc-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3417 2024-05-01 20:06:33.000000 tf_ctc-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      561 2024-05-01 20:13:47.000000 tf_ctc-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-01 20:13:50.053579 tf_ctc-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:13:50.043579 tf_ctc-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:13:50.043579 tf_ctc-0.1.6/src/tf/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:13:50.053579 tf_ctc-0.1.6/src/tf/ctc/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-01 20:12:34.000000 tf_ctc-0.1.6/src/tf/ctc/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      333 2024-05-01 20:13:10.000000 tf_ctc-0.1.6/src/tf/ctc/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3824 2024-05-01 20:07:20.000000 tf_ctc-0.1.6/src/tf/ctc/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2780 2024-05-01 20:07:19.000000 tf_ctc-0.1.6/src/tf/ctc/logits.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      594 2024-05-01 20:07:37.000000 tf_ctc-0.1.6/src/tf/ctc/loss_.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1647 2024-05-01 20:07:19.000000 tf_ctc-0.1.6/src/tf/ctc/metrics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      230 2024-05-01 20:08:37.000000 tf_ctc-0.1.6/src/tf/ctc/test.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:13:50.053579 tf_ctc-0.1.6/src/tf/ctc/tests/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-05-01 20:13:18.000000 tf_ctc-0.1.6/src/tf/ctc/tests/test_decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      520 2024-05-01 20:11:32.000000 tf_ctc-0.1.6/src/tf/ctc/tests/test_loss.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      876 2024-05-01 20:11:34.000000 tf_ctc-0.1.6/src/tf/ctc/tests/test_metrics.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 20:13:50.053579 tf_ctc-0.1.6/src/tf_ctc.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3897 2024-05-01 20:13:50.000000 tf_ctc-0.1.6/src/tf_ctc.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      442 2024-05-01 20:13:50.000000 tf_ctc-0.1.6/src/tf_ctc.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-01 20:13:50.000000 tf_ctc-0.1.6/src/tf_ctc.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       68 2024-05-01 20:13:50.000000 tf_ctc-0.1.6/src/tf_ctc.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-01 20:13:50.000000 tf_ctc-0.1.6/src/tf_ctc.egg-info/top_level.txt
```

### Comparing `tf_ctc-0.1.5/PKG-INFO` & `tf_ctc-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: tf-ctc
-Version: 0.1.5
+Version: 0.1.6
 Summary: CTC with tensorflow, simplified
 Author-email: Marcel Claramunt <marcel@moveread.com>
+Project-URL: repo, https://github.com/marciclabas/tensorflow-ocr
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-tools
 Requires-Dist: tensorflow
+Requires-Dist: lazy-loader
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 
 # Tensorflow CTC
 
 > Tools to simplify CTC in `tensorflow`
 
 ## Mocked Logits
 
 'Perfect' logits to match any given labels. Basically, a large negative value ($10^{-9}$ by default) everywhere except $0$ at the appropriate index. Plus, blank characters (by default at index 0) interspersed to prevent collapse of equal, consecutive labels
 
 ```python
 import tensorflow as tf
-import tf_ctc as ctc
+import tf.ctc as ctc
 
 labs = tf.sparse.from_dense([[1, 2, 3, 0, 0],
                              [4, 3, 1, 2, 0],
                              [3, 1, 0, 0, 0]])
 
 logits = ctc.onehot_logits(labs) # 'perfect' logits
 
@@ -52,15 +54,15 @@
 #         [ 0.e+00, -1.e+09, -1.e+09, -1.e+09, -1.e+09]]], dtype=float32)>
 
 ctc.loss(labs, logits) # something very close to [0, 0, 0]
 ```
 
 ## Loss
 
-Wrapper around `tf.nn.loss` but labels must be a `SparseTensor` and the API is trivial (just labels and logits)
+Wrapper around `tf.nn.loss` but labels must be a `SparseTensor` (as they should probably be) and the API is trivial (just labels and logits)
 
 (See example above)
 
 ## Decoding
 
 Wrappers around `tf.nn.ctc_greedy_decoder` and `tf.nn.ctc_beam_search_decoder`, except:
 - Beam Search supports setting the blank index to 0 (and does so by default)
@@ -110,11 +112,11 @@
 
 ## Testing
 
 Very simple randomized tests using `ctc.onehot_logits`
 
 ```bash
 pip install tf-ctc[test]
-python -m tf_ctc.test
+python -m tf.ctc.test
 ```
 
 (Note: tests may spit out a warning about `jaxtyping`. That's just fine)
```

### Comparing `tf_ctc-0.1.5/README.md` & `tf_ctc-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Mocked Logits
 
 'Perfect' logits to match any given labels. Basically, a large negative value ($10^{-9}$ by default) everywhere except $0$ at the appropriate index. Plus, blank characters (by default at index 0) interspersed to prevent collapse of equal, consecutive labels
 
 ```python
 import tensorflow as tf
-import tf_ctc as ctc
+import tf.ctc as ctc
 
 labs = tf.sparse.from_dense([[1, 2, 3, 0, 0],
                              [4, 3, 1, 2, 0],
                              [3, 1, 0, 0, 0]])
 
 logits = ctc.onehot_logits(labs) # 'perfect' logits
 
@@ -38,15 +38,15 @@
 #         [ 0.e+00, -1.e+09, -1.e+09, -1.e+09, -1.e+09]]], dtype=float32)>
 
 ctc.loss(labs, logits) # something very close to [0, 0, 0]
 ```
 
 ## Loss
 
-Wrapper around `tf.nn.loss` but labels must be a `SparseTensor` and the API is trivial (just labels and logits)
+Wrapper around `tf.nn.loss` but labels must be a `SparseTensor` (as they should probably be) and the API is trivial (just labels and logits)
 
 (See example above)
 
 ## Decoding
 
 Wrappers around `tf.nn.ctc_greedy_decoder` and `tf.nn.ctc_beam_search_decoder`, except:
 - Beam Search supports setting the blank index to 0 (and does so by default)
@@ -96,11 +96,11 @@
 
 ## Testing
 
 Very simple randomized tests using `ctc.onehot_logits`
 
 ```bash
 pip install tf-ctc[test]
-python -m tf_ctc.test
+python -m tf.ctc.test
 ```
 
 (Note: tests may spit out a warning about `jaxtyping`. That's just fine)
```

### Comparing `tf_ctc-0.1.5/pyproject.toml` & `tf_ctc-0.1.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-ctc"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name="Marcel Claramunt", email="marcel@moveread.com" }
 ]
 description = "CTC with tensorflow, simplified"
 dependencies = [
-    "jaxtyping", "tf-tools", "tensorflow"
+    "jaxtyping", "tf-tools", "tensorflow", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.optional-dependencies]
 test = [
     "pytest", "hypothesis"
 ]
 
-# [project.urls]
-# repo = "<GIT_REPO_URL>"
+[project.urls]
+repo = "https://github.com/marciclabas/tensorflow-ocr"
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/decoding.py` & `tf_ctc-0.1.6/src/tf/ctc/decoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from jaxtyping import Float, Int
-from tf_tools import tf_function
+from tf.tools import tf_function
 
 @tf_function
 def beam_decode_tf(
 	logits: Float[tf.Tensor, "batch maxlen vocabsize"],
 	beam_width: int = 100, top_paths: int = 1
 ) -> tuple[list[Int[tf.SparseTensor, "batch maxlen"]], Float[tf.Tensor, "batch 1"]]:
 	"""CTC beam search decoding
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/logits.py` & `tf_ctc-0.1.6/src/tf/ctc/logits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from jaxtyping import Int, Float
-from tf_tools import tf_function, pad_dim_to
+from tf.tools import tf_function, pad_dim_to
 
 @tf_function
 def onehot_logits_sample(label: Int[tf.Tensor, "maxlen"], value: float = 1e9, blank_index: int = 0, vocabsize: int | None = None, num: int | None = None) -> Float[tf.Tensor, "2*maxlen vocabsize"]:
   """Logits that approach a CTC loss of 0 as `value` grows"""
   depth = tf.cast(vocabsize, tf.int32) # you'll have to ask tensorflow why the heck int64 indices are not valid for tf.one_hot...
   return value*tf.concat([
     [tf.one_hot(x, depth), tf.one_hot(blank_index, depth)]
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/loss_.py` & `tf_ctc-0.1.6/src/tf/ctc/loss_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from jaxtyping import Float, Int
-from tf_tools import tf_function
+from tf.tools import tf_function
 
 @tf_function
 def loss(
   labels: Int[tf.SparseTensor, "batch maxlen"],
   logits: Float[tf.Tensor, "batch maxlen vocab"],
   blank_index: int = 0
 ) -> Float[tf.Tensor, "batch"]:
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/metrics.py` & `tf_ctc-0.1.6/src/tf/ctc/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 from jaxtyping import Int, Float
 from .decoding import beam_decode
-import tf_tools as tft
+import tf.tools as tft
 
 def accuracy(
   labs: Int[tf.SparseTensor, "batch maxlen1"],
   logits: Float[tf.Tensor, "batch maxlen2 vocabsize"],
   beam_width: int = 100, k: int = 1, blank_zero: bool = True
 ) -> float:
   """Top `k`-accuracy of the batch
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/tests/test_decoding.py` & `tf_ctc-0.1.6/src/tf/ctc/tests/test_decoding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from hypothesis import given, strategies as st, settings
 import tensorflow as tf
-import numpy as np
-from .decoding import beam_decode, greedy_decode
-from ..utils import onehot_logits
+from tf.ctc import beam_decode, greedy_decode, onehot_logits
 
 def _test_exact(lab: list[int], decode):
   """Logits generated with `onehot_logits` should trivially decode to `lab`"""
   vlab = tf.sparse.from_dense([lab])
   logits = onehot_logits(vlab)
   paths, _ = decode(logits)
   dense_lab = tf.cast(tf.sparse.to_dense(vlab), tf.int32)
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/tests/test_loss.py` & `tf_ctc-0.1.6/src/tf/ctc/tests/test_loss.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from hypothesis import given, strategies as st, settings
 import tensorflow as tf
 import numpy as np
-from .loss_ import loss
-from ..utils import onehot_logits
+from tf.ctc import loss, onehot_logits
 
 @settings(deadline=None)
 @given(st.lists(st.integers(min_value=1, max_value=64), min_size=1, max_size=64), st.integers(min_value=0, max_value=12))
 def test_zero(lab: list[int], delta: int):
   min_depth = tf.reduce_max(lab)+1
   depth = min_depth + delta
   vlab = tf.sparse.from_dense([lab])
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc/tests/test_metrics.py` & `tf_ctc-0.1.6/src/tf/ctc/tests/test_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from hypothesis import given, strategies as st, settings
 import tensorflow as tf
 import keras
 import numpy as np
-from .metrics import edit_distance, accuracy
-from ..utils import onehot_logits
+from tf.ctc import edit_distance, accuracy, onehot_logits
 
 @settings(deadline=None)
 @given(st.lists(st.lists(st.integers(min_value=1, max_value=64), min_size=1, max_size=64), min_size=1, max_size=8))
 def test_perfect_ed(labs: list[list[int]]):
   batch = tf.sparse.from_dense(keras.utils.pad_sequences(labs))
   logits = onehot_logits(batch)
   assert tf.reduce_all(edit_distance(batch, logits) == 0)
```

### Comparing `tf_ctc-0.1.5/src/tf_ctc.egg-info/PKG-INFO` & `tf_ctc-0.1.6/src/tf_ctc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: tf-ctc
-Version: 0.1.5
+Version: 0.1.6
 Summary: CTC with tensorflow, simplified
 Author-email: Marcel Claramunt <marcel@moveread.com>
+Project-URL: repo, https://github.com/marciclabas/tensorflow-ocr
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jaxtyping
 Requires-Dist: tf-tools
 Requires-Dist: tensorflow
+Requires-Dist: lazy-loader
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 
 # Tensorflow CTC
 
 > Tools to simplify CTC in `tensorflow`
 
 ## Mocked Logits
 
 'Perfect' logits to match any given labels. Basically, a large negative value ($10^{-9}$ by default) everywhere except $0$ at the appropriate index. Plus, blank characters (by default at index 0) interspersed to prevent collapse of equal, consecutive labels
 
 ```python
 import tensorflow as tf
-import tf_ctc as ctc
+import tf.ctc as ctc
 
 labs = tf.sparse.from_dense([[1, 2, 3, 0, 0],
                              [4, 3, 1, 2, 0],
                              [3, 1, 0, 0, 0]])
 
 logits = ctc.onehot_logits(labs) # 'perfect' logits
 
@@ -52,15 +54,15 @@
 #         [ 0.e+00, -1.e+09, -1.e+09, -1.e+09, -1.e+09]]], dtype=float32)>
 
 ctc.loss(labs, logits) # something very close to [0, 0, 0]
 ```
 
 ## Loss
 
-Wrapper around `tf.nn.loss` but labels must be a `SparseTensor` and the API is trivial (just labels and logits)
+Wrapper around `tf.nn.loss` but labels must be a `SparseTensor` (as they should probably be) and the API is trivial (just labels and logits)
 
 (See example above)
 
 ## Decoding
 
 Wrappers around `tf.nn.ctc_greedy_decoder` and `tf.nn.ctc_beam_search_decoder`, except:
 - Beam Search supports setting the blank index to 0 (and does so by default)
@@ -110,11 +112,11 @@
 
 ## Testing
 
 Very simple randomized tests using `ctc.onehot_logits`
 
 ```bash
 pip install tf-ctc[test]
-python -m tf_ctc.test
+python -m tf.ctc.test
 ```
 
 (Note: tests may spit out a warning about `jaxtyping`. That's just fine)
```

