# Comparing `tmp/GSG-0.5.4.tar.gz` & `tmp/GSG-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GSG-0.5.4.tar", last modified: Tue Apr 30 02:45:01 2024, max compression
+gzip compressed data, was "dist/GSG-0.5.5.tar", last modified: Wed May  1 01:59:47 2024, max compression
```

## Comparing `GSG-0.5.4.tar` & `GSG-0.5.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:45:01.000000 GSG-0.5.4/
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:45:01.000000 GSG-0.5.4/GSG.egg-info/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2749 2024-04-30 02:45:00.000000 GSG-0.5.4/GSG.egg-info/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-04-30 02:45:00.000000 GSG-0.5.4/GSG.egg-info/SOURCES.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-04-30 02:45:00.000000 GSG-0.5.4/GSG.egg-info/dependency_links.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-04-30 02:45:00.000000 GSG-0.5.4/GSG.egg-info/requires.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-04-30 02:45:00.000000 GSG-0.5.4/GSG.egg-info/top_level.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    40597 2024-04-18 05:21:38.000000 GSG-0.5.4/GSG.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2749 2024-04-30 02:45:01.000000 GSG-0.5.4/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2572 2024-04-30 02:44:51.000000 GSG-0.5.4/README.md
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:45:01.000000 GSG-0.5.4/datasets/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.4/datasets/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.4/datasets/data_util.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:45:01.000000 GSG-0.5.4/models/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.4/models/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.4/models/dot_gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.4/models/edcoder.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.4/models/gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.4/models/gcn.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.4/models/gin.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.4/models/loss_func.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-04-30 02:45:01.000000 GSG-0.5.4/setup.cfg
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      809 2024-04-30 02:44:58.000000 GSG-0.5.4/setup.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-04-30 02:45:01.000000 GSG-0.5.4/tools/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.4/tools/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.4/tools/batch_remove.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.4/tools/evaluation.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.4/tools/parameters_dict.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.4/tools/test.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.4/tools/utils.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/SOURCES.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/dependency_links.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/requires.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/top_level.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    40597 2024-04-18 05:21:38.000000 GSG-0.5.5/GSG.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-01 01:59:47.000000 GSG-0.5.5/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2764 2024-05-01 01:59:10.000000 GSG-0.5.5/README.md
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/datasets/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.5/datasets/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.5/datasets/data_util.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/models/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.5/models/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.5/models/dot_gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.5/models/edcoder.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.5/models/gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.5/models/gcn.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.5/models/gin.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.5/models/loss_func.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-05-01 01:59:47.000000 GSG-0.5.5/setup.cfg
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      809 2024-05-01 01:59:39.000000 GSG-0.5.5/setup.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/tools/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.5/tools/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.5/tools/batch_remove.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.5/tools/evaluation.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.5/tools/parameters_dict.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.5/tools/test.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.5/tools/utils.py
```

### Comparing `GSG-0.5.4/GSG.egg-info/PKG-INFO` & `GSG-0.5.5/GSG.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GSG
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/keaml-Guan/GSG
 License: MIT Licence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GSG: A generative self-supervised graph learning framework for spatial transcriptomics
 ![GitHub Repo stars](https://img.shields.io/github/stars/keaml-Guan/GSG?style=social) ![GitHub forks](https://img.shields.io/github/forks/keaml-Guan/GSG?style=social) ![GitHub watchers](https://img.shields.io/github/watchers/keaml-Guan/GSG?style=social)
@@ -33,11 +33,10 @@
 * pyyaml==6.0.1
 * ploty==5.21.0
 * kaleido==0.2.1
 * igraph==0.11.4
 
 ## Citation
 
-
-<!--
-## Citation
--->
+<mark>
+Guan, R., Sun, H., Zhang, T., Wu, Z., Du, M., Liang, Y., ... & Xu, D. (2024). Generative Self-Supervised Graphs Enhance Integration, Imputation and Domains Identification of Spatial Transcriptomics.
+</mark>
```

### Comparing `GSG-0.5.4/GSG.py` & `GSG-0.5.5/GSG.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/PKG-INFO` & `GSG-0.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GSG
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/keaml-Guan/GSG
 License: MIT Licence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GSG: A generative self-supervised graph learning framework for spatial transcriptomics
 ![GitHub Repo stars](https://img.shields.io/github/stars/keaml-Guan/GSG?style=social) ![GitHub forks](https://img.shields.io/github/forks/keaml-Guan/GSG?style=social) ![GitHub watchers](https://img.shields.io/github/watchers/keaml-Guan/GSG?style=social)
@@ -33,11 +33,10 @@
 * pyyaml==6.0.1
 * ploty==5.21.0
 * kaleido==0.2.1
 * igraph==0.11.4
 
 ## Citation
 
-
-<!--
-## Citation
--->
+<mark>
+Guan, R., Sun, H., Zhang, T., Wu, Z., Du, M., Liang, Y., ... & Xu, D. (2024). Generative Self-Supervised Graphs Enhance Integration, Imputation and Domains Identification of Spatial Transcriptomics.
+</mark>
```

### Comparing `GSG-0.5.4/README.md` & `GSG-0.5.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,10 @@
 * pyyaml==6.0.1
 * ploty==5.21.0
 * kaleido==0.2.1
 * igraph==0.11.4
 
 ## Citation
 
-
-<!--
-## Citation
--->
+<mark>
+Guan, R., Sun, H., Zhang, T., Wu, Z., Du, M., Liang, Y., ... & Xu, D. (2024). Generative Self-Supervised Graphs Enhance Integration, Imputation and Domains Identification of Spatial Transcriptomics.
+</mark>
```

### Comparing `GSG-0.5.4/datasets/data_util.py` & `GSG-0.5.5/datasets/data_util.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/__init__.py` & `GSG-0.5.5/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/dot_gat.py` & `GSG-0.5.5/models/dot_gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/edcoder.py` & `GSG-0.5.5/models/edcoder.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/gat.py` & `GSG-0.5.5/models/gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/gcn.py` & `GSG-0.5.5/models/gcn.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/gin.py` & `GSG-0.5.5/models/gin.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/models/loss_func.py` & `GSG-0.5.5/models/loss_func.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/setup.py` & `GSG-0.5.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name = 'GSG',
-    version='0.5.4',
+    version='0.5.5',
     packages=find_packages(),
     python_requires='>=3.8',
     py_modules=['GSG'],
     long_description=open(os.path.join("./","README.md"), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license="MIT Licence",
     url="https://github.com/keaml-Guan/GSG",
```

### Comparing `GSG-0.5.4/tools/batch_remove.py` & `GSG-0.5.5/tools/batch_remove.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/tools/evaluation.py` & `GSG-0.5.5/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/tools/parameters_dict.py` & `GSG-0.5.5/tools/parameters_dict.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/tools/test.py` & `GSG-0.5.5/tools/test.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.4/tools/utils.py` & `GSG-0.5.5/tools/utils.py`

 * *Files identical despite different names*

