# Comparing `tmp/prometheus_eval-0.1.4.tar.gz` & `tmp/prometheus_eval-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_eval-0.1.4.tar", max compression
+gzip compressed data, was "prometheus_eval-0.1.5.tar", max compression
```

## Comparing `prometheus_eval-0.1.4.tar` & `prometheus_eval-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.4/README.md
--rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.4/prometheus_eval/__init__.py
--rw-r--r--   0        0        0     9342 2024-05-01 14:40:46.049034 prometheus_eval-0.1.4/prometheus_eval/judge.py
--rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.4/prometheus_eval/prompts.py
--rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.4/prometheus_eval/utils.py
--rw-r--r--   0        0        0     2137 2024-05-01 14:38:14.384400 prometheus_eval-0.1.4/prometheus_eval/vllm.py
--rw-r--r--   0        0        0      595 2024-05-01 14:40:53.441064 prometheus_eval-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.5/README.md
+-rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.5/prometheus_eval/__init__.py
+-rw-r--r--   0        0        0     9355 2024-05-01 14:42:02.809346 prometheus_eval-0.1.5/prometheus_eval/judge.py
+-rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.5/prometheus_eval/prompts.py
+-rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.5/prometheus_eval/utils.py
+-rw-r--r--   0        0        0     2137 2024-05-01 14:38:14.384400 prometheus_eval-0.1.5/prometheus_eval/vllm.py
+-rw-r--r--   0        0        0      595 2024-05-01 14:42:43.885510 prometheus_eval-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.5/PKG-INFO
```

### Comparing `prometheus_eval-0.1.4/prometheus_eval/judge.py` & `prometheus_eval-0.1.5/prometheus_eval/judge.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             warnings.warn(
                 "Reference answer was not given in Relative Grading mode. This might lead to nonoptimal performances."
             )
 
         self.absolute_grade_template = absolute_grade_template
         self.relative_grade_template = relative_grade_template
         self.model = (
-            VLLM(model_id, num_gpus=num_gpus, download_dir=download_dir, **kwargs)
+            VLLM(model_id, num_gpus=num_gpus, download_dir=download_dir, dtype=dtype, **kwargs)
             if not is_test
             else MockVLLM()
         )
 
     def _get_conversation_prompt(self, messages: List[Dict[str, str]]):
         """
         From filled prompt, convert it into llama-2 conversation prompt
```

### Comparing `prometheus_eval-0.1.4/prometheus_eval/prompts.py` & `prometheus_eval-0.1.5/prometheus_eval/prompts.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.4/prometheus_eval/utils.py` & `prometheus_eval-0.1.5/prometheus_eval/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.4/prometheus_eval/vllm.py` & `prometheus_eval-0.1.5/prometheus_eval/vllm.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.4/pyproject.toml` & `prometheus_eval-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-eval"
-version = "0.1.4"
+version = "0.1.5"
 description = "A package for evaluating the performance of language models with Prometheus"
 authors = ["Juyoung Suk <juyoung@kaist.ac.kr>", "Seungone Kim <seungone@cmu.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 vllm = "<0.4.0"
```

### Comparing `prometheus_eval-0.1.4/PKG-INFO` & `prometheus_eval-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-eval
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for evaluating the performance of language models with Prometheus
 Author: Juyoung Suk
 Author-email: juyoung@kaist.ac.kr
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
