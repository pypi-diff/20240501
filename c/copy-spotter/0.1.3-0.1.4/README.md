# Comparing `tmp/copy-spotter-0.1.3.tar.gz` & `tmp/copy-spotter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-spotter-0.1.3.tar", last modified: Fri Apr 26 17:54:11 2024, max compression
+gzip compressed data, was "copy-spotter-0.1.4.tar", last modified: Wed May  1 14:49:21 2024, max compression
```

## Comparing `copy-spotter-0.1.3.tar` & `copy-spotter-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/copy_spotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/copy_spotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 14:49:21.000000 copy-spotter-0.1.4/copy_spotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:21.966608 copy-spotter-0.1.4/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-01 14:49:06.000000 copy-spotter-0.1.4/tests/scripts/test_utils.py
```

### Comparing `copy-spotter-0.1.3/LICENSE` & `copy-spotter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.3/PKG-INFO` & `copy-spotter-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -69,15 +69,15 @@
 $ pre-commit install
 
 # Run tests
 $ pip install pytest
 $ pytest tests/
 
 # Run package locally
-$ python -m scripts.main.py [-s] [-o] [-h] input_directory
+$ python -m scripts.main [-s] [-o] [-h] input_directory
 ```
 
 **Recommandations**
 ---
 - Please make sure that all text files are closed before running the program.
 - In order to get the best results please provide text files of the same languages.
 - Pdf files that are made from scanned images won't be processed correctly.
```

### Comparing `copy-spotter-0.1.3/README.md` & `copy-spotter-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 $ pre-commit install
 
 # Run tests
 $ pip install pytest
 $ pytest tests/
 
 # Run package locally
-$ python -m scripts.main.py [-s] [-o] [-h] input_directory
+$ python -m scripts.main [-s] [-o] [-h] input_directory
 ```
 
 **Recommandations**
 ---
 - Please make sure that all text files are closed before running the program.
 - In order to get the best results please provide text files of the same languages.
 - Pdf files that are made from scanned images won't be processed correctly.
```

### Comparing `copy-spotter-0.1.3/copy_spotter.egg-info/PKG-INFO` & `copy-spotter-0.1.4/copy_spotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -69,15 +69,15 @@
 $ pre-commit install
 
 # Run tests
 $ pip install pytest
 $ pytest tests/
 
 # Run package locally
-$ python -m scripts.main.py [-s] [-o] [-h] input_directory
+$ python -m scripts.main [-s] [-o] [-h] input_directory
 ```
 
 **Recommandations**
 ---
 - Please make sure that all text files are closed before running the program.
 - In order to get the best results please provide text files of the same languages.
 - Pdf files that are made from scanned images won't be processed correctly.
```

### Comparing `copy-spotter-0.1.3/copy_spotter.egg-info/SOURCES.txt` & `copy-spotter-0.1.4/copy_spotter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 copy_spotter.egg-info/PKG-INFO
 copy_spotter.egg-info/SOURCES.txt
 copy_spotter.egg-info/dependency_links.txt
 copy_spotter.egg-info/entry_points.txt
 copy_spotter.egg-info/requires.txt
```

### Comparing `copy-spotter-0.1.3/scripts/html_utils.py` & `copy-spotter-0.1.4/scripts/html_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     return final_directory
 
 
 def get_color_from_similarity(similarity_score: float) -> str:
     """Return css style according to similarity score"""
 
-    if float(similarity_score) > 15:
+    if similarity_score > 15:
         return "#990033; font-weight: bold"
-    if float(similarity_score) > 10:
+    if similarity_score > 10:
         return "#ff6600"
-    if float(similarity_score) > 5:
+    if similarity_score > 5:
         return "#ffcc00"
 
     return "green"
```

### Comparing `copy-spotter-0.1.3/scripts/html_writing.py` & `copy-spotter-0.1.4/scripts/html_writing.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 It adds links to HTML table.
 It generates span tags for un/colored matching blocks.
 It compares two text files
 It inserts comparison results in corresponding html files
 
 """
 
-from os import fsync, rename, path
+from os import fsync, path
 from random import randint
 from shutil import copy
 from typing import Any, List
 
 from bs4 import BeautifulSoup as Bs
 from tabulate import tabulate
 
@@ -39,15 +39,15 @@
 
         for td_tag in soup.findAll("td"):  # Retrieve all data celss from html table in path
             if is_float(td_tag.text):  # If td is not filename or -1
                 tmp = soup.new_tag(
                     "a",
                     href="file:///" + html_path.replace("_results", str(file_ind)),
                     target="_blank",
-                    style="color:" + get_color_from_similarity(td_tag.text),
+                    style="color:" + get_color_from_similarity(float(td_tag.text)),
                 )
 
                 td_tag.string.wrap(tmp)  # We wrap the td string between the hyperlink
                 file_ind += 1
 
         # We update the HTML of the file at path
         with open(html_path, "wb") as f_output:
@@ -110,32 +110,34 @@
         results[num].append(span)
 
     return results
 
 
 def papers_comparison(save_dir: str, ind: int, text1: list, text2: list, filenames: tuple, block_size: int) -> None:
     """Write to HTML file texts that have been compared with highlighted similar blocks"""
-
-    copy(path.join("templates", "template.html"), save_dir)  # Copy comparison template to curr dir
+    template_path = path.join("templates", "template.html")
     comp_path = path.join(save_dir, str(ind) + ".html")
-    rename(path.join(save_dir, "template.html"), comp_path)
+
+    # Copy the template to the save directory under a new name
+    copy(template_path, comp_path)
 
     with open(comp_path, encoding="utf-8") as html:
         soup = Bs(html, "html.parser")
         res = get_span_blocks(soup, text1, text2, block_size)
-        blocks = soup.findAll(attrs={"class": "block"})
+        blocks = [soup.find(id="leftContent"), soup.find(id="rightContent")]
 
         # Append filename tags and span tags to html
         for i, filename in enumerate(filenames):
             temp_tag = soup.new_tag("h3")
             temp_tag.string = filename
             blocks[i].append(temp_tag)
             for tag in res[i]:
                 blocks[i].append(tag)
 
+    # Write the modified content back to the file
     with open(comp_path, "wb") as f_output:
         f_output.write(soup.prettify("utf-8"))
 
 
 def results_to_html(scores: list, files_names: list, html_path: str) -> None:
     """Write similarity results to HTML page"""
```

### Comparing `copy-spotter-0.1.3/scripts/main.py` & `copy-spotter-0.1.4/scripts/main.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.3/scripts/processing_files.py` & `copy-spotter-0.1.4/scripts/processing_files.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.3/scripts/similarity.py` & `copy-spotter-0.1.4/scripts/similarity.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.3/scripts/utils.py` & `copy-spotter-0.1.4/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.3/setup.py` & `copy-spotter-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.3/tests/scripts/test_utils.py` & `copy-spotter-0.1.4/tests/scripts/test_utils.py`

 * *Files identical despite different names*

