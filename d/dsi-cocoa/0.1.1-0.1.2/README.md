# Comparing `tmp/dsi_cocoa-0.1.1.tar.gz` & `tmp/dsi_cocoa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.1.1.tar", last modified: Thu Apr 25 19:05:10 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.1.2.tar", last modified: Wed May  1 18:02:13 2024, max compression
```

## Comparing `dsi_cocoa-0.1.1.tar` & `dsi_cocoa-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:10.203073 dsi_cocoa-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:10.199073 dsi_cocoa-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:10.199073 dsi_cocoa-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-25 19:05:10.203073 dsi_cocoa-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-25 19:05:10.203073 dsi_cocoa-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:10.199073 dsi_cocoa-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:10.199073 dsi_cocoa-0.1.1/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 19:05:05.000000 dsi_cocoa-0.1.1/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:10.203073 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-25 19:05:10.000000 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-25 19:05:10.000000 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:05:10.000000 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 19:05:10.000000 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 19:05:10.000000 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 19:05:10.000000 dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.037971 dsi_cocoa-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.037971 dsi_cocoa-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.1.1/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.1.2/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.1.2/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/.gitignore` & `dsi_cocoa-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/.pre-commit-config.yaml` & `dsi_cocoa-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/PKG-INFO` & `dsi_cocoa-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.1
+Version: 0.1.2
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.1/README.md` & `dsi_cocoa-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/pyproject.toml` & `dsi_cocoa-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.1.2/src/cocoa/evaluate_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,21 +50,22 @@
             os.path.join(root, f)
             for root, _, files in os.walk(dir_path)
             for f in files
             if not any(x in os.path.join(root, f) for x in paths_to_flag)
         ]
 
     for file_path in files_to_process:
-        if file_path.endswith(".ipynb") or file_path.endswith(".py"):
-            print(f"Analyzing {file_path}:")
-            if file_path.endswith(".ipynb"):
-                analyze_notebook(file_path, no_filter_flag, verbose)
-            elif file_path.endswith(".py"):
-                analyze_python_file(file_path, lint_flag, verbose)
-            print("-" * 80)
+        if os.path.exists(file_path):
+            if file_path.endswith(".ipynb") or file_path.endswith(".py"):
+                print(f"Analyzing {file_path}:")
+                if file_path.endswith(".ipynb"):
+                    analyze_notebook(file_path, no_filter_flag, verbose)
+                elif file_path.endswith(".py"):
+                    analyze_python_file(file_path, lint_flag, verbose)
+                print("-" * 80)
 
 
 def analyze_notebook(file_path, no_filter_flag, verbose):
     """Analyze a notebook"""
     num_cells, num_lines, num_functions, max_lines_in_cell = process_notebook(
         file_path
     )
```

### Comparing `dsi_cocoa-0.1.1/src/cocoa/linting.py` & `dsi_cocoa-0.1.2/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/src/cocoa/notebooks.py` & `dsi_cocoa-0.1.2/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/src/cocoa/repo.py` & `dsi_cocoa-0.1.2/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/src/cocoa/spring2024.py` & `dsi_cocoa-0.1.2/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.1
+Version: 0.1.2
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.1/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

