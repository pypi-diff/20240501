# Comparing `tmp/cf2tf-0.7.2a6.tar.gz` & `tmp/cf2tf-0.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.7.2a6.tar", max compression
+gzip compressed data, was "cf2tf-0.8.0a0.tar", max compression
```

## Comparing `cf2tf-0.7.2a6.tar` & `cf2tf-0.8.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/LICENSE.txt
--rw-r--r--   0        0        0     7485 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/README.md
--rw-r--r--   0        0        0     1089 2024-05-01 01:45:23.288109 cf2tf-0.7.2a6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1451 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2621 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    32457 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     2026 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    21718 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2673 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2199 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     3995 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     4674 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2673 2024-05-01 01:45:10.324005 cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.7.2a6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/LICENSE.txt
+-rw-r--r--   0        0        0     7485 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/README.md
+-rw-r--r--   0        0        0     1089 2024-05-01 03:26:08.302907 cf2tf-0.8.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    32457 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2026 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    21718 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2673 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2199 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     4099 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     4691 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2673 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.8.0a0/PKG-INFO
```

### Comparing `cf2tf-0.7.2a6/LICENSE.txt` & `cf2tf-0.8.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/README.md` & `cf2tf-0.8.0a0/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/pyproject.toml` & `cf2tf-0.8.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.7.2a6"
+version = "0.8.0a0"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
```

### Comparing `cf2tf-0.7.2a6/src/cf2tf/app.py` & `cf2tf-0.8.0a0/src/cf2tf/app.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.8.0a0/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/conversion/expressions.py` & `cf2tf-0.8.0a0/src/cf2tf/conversion/expressions.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/conversion/overrides.py` & `cf2tf-0.8.0a0/src/cf2tf/conversion/overrides.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/convert.py` & `cf2tf-0.8.0a0/src/cf2tf/convert.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/save.py` & `cf2tf-0.8.0a0/src/cf2tf/save.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/blocks.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/blocks.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/code.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/code.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import re
 from pathlib import Path
+from shutil import rmtree
 from tempfile import gettempdir
 from typing import Optional
-from shutil import rmtree
 
 import click
 from click._termui_impl import ProgressBar
 from git import RemoteProgress
-from git.repo.base import Repo, InvalidGitRepositoryError
+from git.repo.base import InvalidGitRepositoryError, Repo
 from thefuzz import fuzz, process  # type: ignore
 
-import cf2tf.convert
+# import cf2tf.convert
 
 log = logging.getLogger("cf2tf")
 
 
 class SearchManager:
     def __init__(self, docs_path: Path) -> None:
         self.docs_path = docs_path
@@ -31,15 +31,15 @@
             doc_file: transform_file_name(doc_file.name) for doc_file in self.resources
         }
 
         resource_name: str
         ranking: int
         doc_path: Path
         resource_name, ranking, doc_path = process.extractOne(
-            name.lower(), files, scorer=fuzz.token_sort_ratio
+            name.lower(), files, scorer=fuzz.ratio
         )
 
         log.debug(
             f"Best match was {resource_name} at {doc_path} with score of {ranking}."
         )
 
         return doc_path
@@ -105,17 +105,19 @@
 
     Returns:
         str: A search term that can be used to match resources in the TF docs.
     """
 
     search_tokens = resource_type.replace("::", " ").replace("AWS", " ").split(" ")
 
-    for i, token in enumerate(search_tokens):
-        if len(token) >= 4:
-            search_tokens[i] = cf2tf.convert.camel_case_split(token)
+    # I will leave the logic for camel case splitting here for now.
+    # in case we want to use it later.
+    # for i, token in enumerate(search_tokens):
+    #     if len(token) >= 4:
+    #         search_tokens[i] = cf2tf.convert.camel_case_split(token)
 
     search_term = " ".join(search_tokens).lower().strip()
 
     log.debug(f"Converted CF type {resource_type} to search term {search_term}.")
 
     return search_term
```

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/doc_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import logging
+import re
 from io import TextIOWrapper
 from pathlib import Path
 from typing import List
-import re
-
-import logging
 
 log = logging.getLogger("cf2tf")
 
 
 def parse_attributes(docs_path: Path):
     with open(docs_path) as file:
         try:
@@ -85,15 +84,15 @@
             break
 
         # If line starts with whitespace its probably a multiline description
         if line.startswith((" ", "\t")):
             continue
 
         # These should be the attributes we are after
-        if line[0] == "*":
+        if line[0] == "*" or line[0] == "-":
             regex = r"`([\w.*]+)`"
 
             match = re.search(regex, line)
 
             if not match:
                 log.debug(f"Did not find an item to parse in {line}")
                 continue
```

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.2a6/PKG-INFO` & `cf2tf-0.8.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.7.2a6
+Version: 0.8.0a0
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.7.2a6 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.8.0a0 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

