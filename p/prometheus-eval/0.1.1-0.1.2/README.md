# Comparing `tmp/prometheus_eval-0.1.1.tar.gz` & `tmp/prometheus_eval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_eval-0.1.1.tar", max compression
+gzip compressed data, was "prometheus_eval-0.1.2.tar", max compression
```

## Comparing `prometheus_eval-0.1.1.tar` & `prometheus_eval-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.1/README.md
--rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.1/prometheus_eval/__init__.py
--rw-r--r--   0        0        0     9285 2024-05-01 13:51:32.226312 prometheus_eval-0.1.1/prometheus_eval/judge.py
--rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.1/prometheus_eval/prompts.py
--rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.1/prometheus_eval/utils.py
--rw-r--r--   0        0        0     2464 2024-05-01 13:42:57.411514 prometheus_eval-0.1.1/prometheus_eval/vllm.py
--rw-r--r--   0        0        0      595 2024-05-01 14:07:06.350350 prometheus_eval-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 prometheus_eval-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.2/README.md
+-rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.2/prometheus_eval/__init__.py
+-rw-r--r--   0        0        0     9285 2024-05-01 13:51:32.226312 prometheus_eval-0.1.2/prometheus_eval/judge.py
+-rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.2/prometheus_eval/prompts.py
+-rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.2/prometheus_eval/utils.py
+-rw-r--r--   0        0        0     2464 2024-05-01 13:42:57.411514 prometheus_eval-0.1.2/prometheus_eval/vllm.py
+-rw-r--r--   0        0        0      595 2024-05-01 14:14:55.391261 prometheus_eval-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.2/PKG-INFO
```

### Comparing `prometheus_eval-0.1.1/prometheus_eval/judge.py` & `prometheus_eval-0.1.2/prometheus_eval/judge.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.1/prometheus_eval/prompts.py` & `prometheus_eval-0.1.2/prometheus_eval/prompts.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.1/prometheus_eval/utils.py` & `prometheus_eval-0.1.2/prometheus_eval/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.1/prometheus_eval/vllm.py` & `prometheus_eval-0.1.2/prometheus_eval/vllm.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.1/pyproject.toml` & `prometheus_eval-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "prometheus-eval"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package for evaluating the performance of language models with Prometheus"
 authors = ["Juyoung Suk <juyoung@kaist.ac.kr>", "Seungone Kim <seungone@cmu.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-vllm = "^0.4.1"
+vllm = "<0.4.0"
 fastchat = "^0.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 isort = "^5.13.2"
 autoflake = "^2.3.1"
```

### Comparing `prometheus_eval-0.1.1/PKG-INFO` & `prometheus_eval-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prometheus-eval
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for evaluating the performance of language models with Prometheus
 Author: Juyoung Suk
 Author-email: juyoung@kaist.ac.kr
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastchat (>=0.1.0,<0.2.0)
-Requires-Dist: vllm (>=0.4.1,<0.5.0)
+Requires-Dist: vllm (<0.4.0)
 Description-Content-Type: text/markdown
```

