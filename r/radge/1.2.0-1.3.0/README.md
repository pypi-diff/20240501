# Comparing `tmp/radge-1.2.0.tar.gz` & `tmp/radge-1.3.0.tar.gz`

## Comparing `radge-1.2.0.tar` & `radge-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.2.0/requirements.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 radge-1.2.0/radge/__init__.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 radge-1.2.0/radge/graph.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 radge-1.2.0/radge/numbers.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 radge-1.2.0/radge/polygon.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 radge-1.2.0/radge/sequences.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 radge-1.2.0/radge/string.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 radge-1.2.0/radge/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_graph.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_numbers.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_polygon.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_seed.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_sequences.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_string.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 radge-1.2.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 radge-1.2.0/LICENSE
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 radge-1.2.0/README.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 radge-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 radge-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.3.0/requirements.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 radge-1.3.0/radge/__init__.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 radge-1.3.0/radge/graph.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 radge-1.3.0/radge/numbers.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 radge-1.3.0/radge/polygon.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 radge-1.3.0/radge/sequences.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 radge-1.3.0/radge/string.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 radge-1.3.0/radge/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 radge-1.3.0/tests/test_graph.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 radge-1.3.0/tests/test_numbers.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 radge-1.3.0/tests/test_polygon.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 radge-1.3.0/tests/test_seed.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 radge-1.3.0/tests/test_sequences.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 radge-1.3.0/tests/test_string.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 radge-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 radge-1.3.0/LICENSE
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 radge-1.3.0/README.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 radge-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 radge-1.3.0/PKG-INFO
```

### Comparing `radge-1.2.0/radge/graph.py` & `radge-1.3.0/radge/graph.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/radge/numbers.py` & `radge-1.3.0/radge/numbers.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/radge/sequences.py` & `radge-1.3.0/radge/sequences.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/radge/string.py` & `radge-1.3.0/radge/string.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/tests/test_graph.py` & `radge-1.3.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/tests/test_seed.py` & `radge-1.3.0/tests/test_seed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import unittest
 
 import radge.utils as utils
 import radge.sequences as seq
 
+
 class TestSeed(unittest.TestCase):
     def test_is_same(self):
         """Test if a random sequence is the same if it's generated using the same seed twice."""
         TESTS = 100
         MAX_N = 10**4
         for _ in range(TESTS):
             start_seed = utils.SEED
             seq1 = seq.seq(MAX_N, range(1, MAX_N))
             utils.seed(2137)
             utils.seed(start_seed)
             seq2 = seq.seq(MAX_N, range(1, MAX_N))
 
             self.assertTrue(seq1 == seq2)
 
+
+if __name__ == "__main__":
+    unittest.main(failfast=True)
```

### Comparing `radge-1.2.0/tests/test_sequences.py` & `radge-1.3.0/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/tests/test_string.py` & `radge-1.3.0/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/.gitignore` & `radge-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/LICENSE` & `radge-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/README.md` & `radge-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `radge-1.2.0/PKG-INFO` & `radge-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: radge
-Version: 1.2.0
+Version: 1.3.0
 Summary: A random algorithmic data generator
 Author-email: Antoni Zasada <zsd.antoni@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Radge - Random algorithmic data generator
```

