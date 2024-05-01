# Comparing `tmp/mentabotix-0.1.0.tar.gz` & `tmp/mentabotix-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.0.tar", last modified: Tue Apr 23 16:28:59 2024, max compression
+gzip compressed data, was "mentabotix-0.1.1a0.tar", last modified: Wed May  1 16:22:14 2024, max compression
```

## Comparing `mentabotix-0.1.0.tar` & `mentabotix-0.1.1a0.tar`

### file list

```diff
@@ -1,10 +1,17 @@
--rw-r--r--   0        0        0     1768 2024-04-23 16:28:34.491044 mentabotix-0.1.0/README.md
--rw-r--r--   0        0        0      602 2024-04-23 16:28:59.066994 mentabotix-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      646 2024-04-23 16:28:34.491044 mentabotix-0.1.0/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    12899 2024-04-23 16:28:34.491044 mentabotix-0.1.0/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      137 2024-04-23 16:28:34.491044 mentabotix-0.1.0/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-04-23 16:28:34.491044 mentabotix-0.1.0/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    19645 2024-04-23 16:28:34.491044 mentabotix-0.1.0/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0        0 2024-04-23 16:28:34.491044 mentabotix-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     6334 2024-04-23 16:28:34.491044 mentabotix-0.1.0/tests/test_menta.py
--rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 mentabotix-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    14350 2024-05-01 16:21:51.481188 mentabotix-0.1.1a0/README.md
+-rw-r--r--   0        0        0      701 2024-05-01 16:22:14.453434 mentabotix-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      847 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    56590 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    19645 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     3363 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/tools/algrithm_tools.py
+-rw-r--r--   0        0        0      229 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     5457 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/vision/camra.py
+-rw-r--r--   0        0        0     8336 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/__init__.py
+-rw-r--r--   0        0        0    12243 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_botix.py
+-rw-r--r--   0        0        0     8042 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5578 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    14877 1970-01-01 00:00:00.000000 mentabotix-0.1.1a0/PKG-INFO
```

### Comparing `mentabotix-0.1.0/pyproject.toml` & `mentabotix-0.1.1a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [project]
 name = "mentabotix"
-version = "0.1.0"
+version = "0.1.1a0"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pydantic>=2.7.0",
     "coloredlogs>=15.0.1",
-    "bdmc >=0.1.2",
+    "bdmc>=0.1.3",
     "pyyaml>=6.0.1",
     "numpy>=1.26.4",
     "pyuptech>=0.1.4a0",
+    "opencv-python-headless>=4.9.0.80",
+    "pyapriltags>=3.3.0.3",
+    "terminaltables>=3.1.10",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `mentabotix-0.1.0/src/mentabotix/__init__.py` & `mentabotix-0.1.1a0/src/mentabotix/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-from .modules.botix import MovingState, MovingTransform, Botix
-from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError
+from .modules.botix import MovingState, MovingTransition, Botix
+from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
 from .modules.logger import set_log_level
 from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
+from .vision.camra import Camera
+from .vision.tagdetector import TagDetector
 
 __all__ = [
     "set_log_level",
     # botix
     "MovingState",
-    "MovingTransform",
+    "MovingTransition",
     "Botix",
     # menta
     "Menta",
     "SequenceSampler",
     "IndexedSampler",
     "DirectSampler",
     "SamplerUsage",
     "SamplerType",
     "Sampler",
+    # vision
+    "Camera",
+    "TagDetector",
     # exceptions
     "BadSignatureError",
     "RequirementError",
     "SamplerTypeError",
+    "TokenizeError",
+    "StructuralError",
 ]
```

### Comparing `mentabotix-0.1.0/src/mentabotix/modules/logger.py` & `mentabotix-0.1.1a0/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.0/src/mentabotix/modules/menta.py` & `mentabotix-0.1.1a0/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.0/tests/test_menta.py` & `mentabotix-0.1.1a0/tests/test_menta.py`

 * *Files 18% similar despite different names*

```diff
@@ -167,14 +167,58 @@
     def test_indexer_idx(self):
         varname = "hel"
         req = [0, 1, 2]
         data_1 = self.menta._index_for_idx_sampler_data(varname, req)
         print(data_1)
         self.assertEqual(["hel(0)", "hel(1)", "hel(2)"], data_1)
 
+    def test_constructed_judge_function_performance(self):
+        sages = [
+            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
+            SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
+        ]
+        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
+
+        def _manual_seq_func():
+            seq_temp = mock_sequence_sampler()
+
+            return seq_temp[0], seq_temp[2]
+
+        def _manual_drc_func():
+            drc_temp = mock_direct_sampler()
+            return tuple((drc_temp >> ri) & 1 for ri in [0, 1, 2])
+
+        def _manual_asm_func():
+            return *_manual_seq_func(), mock_indexed_sampler(5), *_manual_drc_func()
+
+        def _manual_judge_func():
+            return sum(_manual_asm_func())
+
+        self.assertEqual(func(), _manual_judge_func())
+
+        import timeit
+
+        # 假设这两个函数已经在你的代码中定义好了
+
+        # 设置测试次数（例如：1000次）
+        number_of_runs = 1000
+
+        # 对func()进行计时测试
+        func_time = timeit.timeit(lambda: func(), number=number_of_runs)
+
+        print(f"func() execution time for {number_of_runs} runs: {func_time:.6f} seconds")
+
+        # 对_manual_judge_func()进行计时测试
+        manual_judge_func_time = timeit.timeit(lambda: _manual_judge_func(), number=number_of_runs)
+
+        print(f"_manual_judge_func() execution time for {number_of_runs} runs: {manual_judge_func_time:.6f} seconds")
+
+        print(f"func() is {manual_judge_func_time / func_time:.2f} times faster than _manual_judge_func()")
+
     def tearDown(self):
         # 清理可能的副作用
         pass
 
 
 if __name__ == "__main__":
     unittest.main()
```

