# Comparing `tmp/arxify-1.0.1.tar.gz` & `tmp/arxify-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxify-1.0.1.tar", last modified: Wed Dec  7 18:09:24 2022, max compression
+gzip compressed data, was "arxify-1.0.2.tar", last modified: Wed May  1 08:17:49 2024, max compression
```

## Comparing `arxify-1.0.1.tar` & `arxify-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-12-07 18:09:24.922068 arxify-1.0.1/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1070 2022-12-07 16:01:11.000000 arxify-1.0.1/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)     1952 2022-12-07 18:09:24.922068 arxify-1.0.1/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1452 2022-12-07 18:07:27.000000 arxify-1.0.1/README.md
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-12-07 18:09:24.922068 arxify-1.0.1/arxify/
--rw-rw-r--   0 tim       (1000) tim       (1000)       31 2022-12-07 17:40:13.000000 arxify-1.0.1/arxify/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5293 2022-12-07 17:59:47.000000 arxify-1.0.1/arxify/arxify.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-12-07 18:09:24.922068 arxify-1.0.1/arxify.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1952 2022-12-07 18:09:24.000000 arxify-1.0.1/arxify.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      254 2022-12-07 18:09:24.000000 arxify-1.0.1/arxify.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-12-07 18:09:24.000000 arxify-1.0.1/arxify.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       39 2022-12-07 18:09:24.000000 arxify-1.0.1/arxify.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       16 2022-12-07 18:09:24.000000 arxify-1.0.1/arxify.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        7 2022-12-07 18:09:24.000000 arxify-1.0.1/arxify.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       79 2022-12-07 18:09:24.922068 arxify-1.0.1/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      871 2022-12-07 18:08:31.000000 arxify-1.0.1/setup.py
+drwxr-xr-x   0 tim       (1000) users      (985)        0 2024-05-01 08:17:49.790041 arxify-1.0.2/
+-rw-r--r--   0 tim       (1000) users      (985)     1070 2024-05-01 08:08:17.000000 arxify-1.0.2/LICENSE
+-rw-r--r--   0 tim       (1000) users      (985)     1983 2024-05-01 08:17:49.790041 arxify-1.0.2/PKG-INFO
+-rw-r--r--   0 tim       (1000) users      (985)     1452 2024-05-01 08:08:17.000000 arxify-1.0.2/README.md
+drwxr-xr-x   0 tim       (1000) users      (985)        0 2024-05-01 08:17:49.786708 arxify-1.0.2/arxify/
+-rw-r--r--   0 tim       (1000) users      (985)       31 2024-05-01 08:08:17.000000 arxify-1.0.2/arxify/__init__.py
+-rw-r--r--   0 tim       (1000) users      (985)     5294 2024-05-01 08:12:53.000000 arxify-1.0.2/arxify/arxify.py
+drwxr-xr-x   0 tim       (1000) users      (985)        0 2024-05-01 08:17:49.790041 arxify-1.0.2/arxify.egg-info/
+-rw-r--r--   0 tim       (1000) users      (985)     1983 2024-05-01 08:17:49.000000 arxify-1.0.2/arxify.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) users      (985)      254 2024-05-01 08:17:49.000000 arxify-1.0.2/arxify.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) users      (985)        1 2024-05-01 08:17:49.000000 arxify-1.0.2/arxify.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) users      (985)       39 2024-05-01 08:17:49.000000 arxify-1.0.2/arxify.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) users      (985)       16 2024-05-01 08:17:49.000000 arxify-1.0.2/arxify.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) users      (985)        7 2024-05-01 08:17:49.000000 arxify-1.0.2/arxify.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) users      (985)       79 2024-05-01 08:17:49.790041 arxify-1.0.2/setup.cfg
+-rw-r--r--   0 tim       (1000) users      (985)      871 2024-05-01 08:13:34.000000 arxify-1.0.2/setup.py
```

### Comparing `arxify-1.0.1/LICENSE` & `arxify-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arxify-1.0.1/PKG-INFO` & `arxify-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: arxify
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pack a latex project into an arxiv compatible archive.
 Home-page: https://github.com/TimSchneider42/arxify
 Author: Tim Schneider
 Author-email: tim@robot-learning.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: inotify==0.2.10
 
 # arxify - Arxiv Packaging Tool
 `arxify` is a command line tool that packs latex projects into an arxiv compatible archives.
 It removes comments from you *.tex files and removes any files that are not needed during the compile process.
 The latter is achieved by compiling the project once and observing which files are being accessed by the compiler using `inotify`.
 Due to the reliance on `inotify`, this tool is currently available only for Linux.
```

### Comparing `arxify-1.0.1/README.md` & `arxify-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arxify-1.0.1/arxify/arxify.py` & `arxify-1.0.2/arxify/arxify.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def find_files(root: Path) -> List[Path]:
     own_files = (f for f in root.iterdir() if f.is_file())
     sub_files = (find_files(d) for d in root.iterdir() if d.is_dir())
     return list(chain(own_files, *sub_files))
 
 
 def remove_comment(line: str):
-    results = re.findall("((?:[^%]|%%)*%?).*", line)[:-1]
+    results = re.findall("((?:[^%]|\\%)*%?).*", line)[:-1]
     if len(results) == 0:
         return ""
     return results[0]
 
 
 def process_tex_file(path: Path) -> str:
     with path.open() as f:
```

### Comparing `arxify-1.0.1/arxify.egg-info/PKG-INFO` & `arxify-1.0.2/arxify.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: arxify
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pack a latex project into an arxiv compatible archive.
 Home-page: https://github.com/TimSchneider42/arxify
 Author: Tim Schneider
 Author-email: tim@robot-learning.de
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: inotify==0.2.10
 
 # arxify - Arxiv Packaging Tool
 `arxify` is a command line tool that packs latex projects into an arxiv compatible archives.
 It removes comments from you *.tex files and removes any files that are not needed during the compile process.
 The latter is achieved by compiling the project once and observing which files are being accessed by the compiler using `inotify`.
 Due to the reliance on `inotify`, this tool is currently available only for Linux.
```

### Comparing `arxify-1.0.1/setup.py` & `arxify-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="arxify",
-    version="1.0.1",
+    version="1.0.2",
     description="Pack a latex project into an arxiv compatible archive.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TimSchneider42/arxify",
     author="Tim Schneider",
     author_email="tim@robot-learning.de",
     license="MIT",
```

