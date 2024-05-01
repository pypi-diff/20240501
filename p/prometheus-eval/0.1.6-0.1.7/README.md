# Comparing `tmp/prometheus_eval-0.1.6.tar.gz` & `tmp/prometheus_eval-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_eval-0.1.6.tar", max compression
+gzip compressed data, was "prometheus_eval-0.1.7.tar", max compression
```

## Comparing `prometheus_eval-0.1.6.tar` & `prometheus_eval-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.6/README.md
--rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.6/prometheus_eval/__init__.py
--rw-r--r--   0        0        0     9355 2024-05-01 14:42:02.809346 prometheus_eval-0.1.6/prometheus_eval/judge.py
--rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.6/prometheus_eval/prompts.py
--rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.6/prometheus_eval/utils.py
--rw-r--r--   0        0        0     2130 2024-05-01 14:46:35.318415 prometheus_eval-0.1.6/prometheus_eval/vllm.py
--rw-r--r--   0        0        0      595 2024-05-01 14:46:42.814443 prometheus_eval-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.7/README.md
+-rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.7/prometheus_eval/__init__.py
+-rw-r--r--   0        0        0     9355 2024-05-01 14:42:02.809346 prometheus_eval-0.1.7/prometheus_eval/judge.py
+-rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.7/prometheus_eval/prompts.py
+-rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.7/prometheus_eval/utils.py
+-rw-r--r--   0        0        0     2142 2024-05-01 14:51:19.783489 prometheus_eval-0.1.7/prometheus_eval/vllm.py
+-rw-r--r--   0        0        0      595 2024-05-01 14:51:28.075520 prometheus_eval-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.7/PKG-INFO
```

### Comparing `prometheus_eval-0.1.6/prometheus_eval/judge.py` & `prometheus_eval-0.1.7/prometheus_eval/judge.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.6/prometheus_eval/prompts.py` & `prometheus_eval-0.1.7/prometheus_eval/prompts.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.6/prometheus_eval/utils.py` & `prometheus_eval-0.1.7/prometheus_eval/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.6/prometheus_eval/vllm.py` & `prometheus_eval-0.1.7/prometheus_eval/vllm.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ) -> None:
         dtype: str = "auto"
         self.name: str = name
 
 
         self.model: LLM = LLM(
             model=self.name,
-            num_gpus=num_gpus,
+            tensor_parallel_size=num_gpus,
             dtype=dtype,
             gpu_memory_utilization=gpu_memory_utilization,
             download_dir=download_dir,
             **kwargs
         )
 
     def completions(
```

### Comparing `prometheus_eval-0.1.6/pyproject.toml` & `prometheus_eval-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-eval"
-version = "0.1.6"
+version = "0.1.7"
 description = "A package for evaluating the performance of language models with Prometheus"
 authors = ["Juyoung Suk <juyoung@kaist.ac.kr>", "Seungone Kim <seungone@cmu.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 vllm = "<0.4.0"
```

### Comparing `prometheus_eval-0.1.6/PKG-INFO` & `prometheus_eval-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-eval
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for evaluating the performance of language models with Prometheus
 Author: Juyoung Suk
 Author-email: juyoung@kaist.ac.kr
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

