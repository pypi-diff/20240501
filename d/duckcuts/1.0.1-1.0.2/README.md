# Comparing `tmp/duckcuts-1.0.1.tar.gz` & `tmp/duckcuts-1.0.2.tar.gz`

## Comparing `duckcuts-1.0.1.tar` & `duckcuts-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    14340 2020-02-02 00:00:00.000000 duckcuts-1.0.1/.DS_Store
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 duckcuts-1.0.1/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/entry_points.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/main.css
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/main.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/data/terminal.csv
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/data/vim-multiple-files.csv
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/data/vim-operators.csv
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/data/vim-search-replace.csv
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/data/vim-text-objects.csv
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 duckcuts-1.0.1/src/duckcuts/data/vim.csv
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 duckcuts-1.0.1/.gitignore
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 duckcuts-1.0.1/README.md
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 duckcuts-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 duckcuts-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    14340 2020-02-02 00:00:00.000000 duckcuts-1.0.2/.DS_Store
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 duckcuts-1.0.2/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/entry_points.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/main.css
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/main.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/data/terminal.csv
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/data/vim-multiple-files.csv
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/data/vim-operators.csv
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/data/vim-search-replace.csv
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/data/vim-text-objects.csv
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 duckcuts-1.0.2/src/duckcuts/data/vim.csv
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 duckcuts-1.0.2/.gitignore
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 duckcuts-1.0.2/README.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 duckcuts-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 duckcuts-1.0.2/PKG-INFO
```

### Comparing `duckcuts-1.0.1/.DS_Store` & `duckcuts-1.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/.DS_Store` & `duckcuts-1.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/.DS_Store` & `duckcuts-1.0.2/src/duckcuts/.DS_Store`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/main.css` & `duckcuts-1.0.2/src/duckcuts/main.css`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/main.py` & `duckcuts-1.0.2/src/duckcuts/main.py`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/data/vim-multiple-files.csv` & `duckcuts-1.0.2/src/duckcuts/data/vim-multiple-files.csv`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/data/vim-operators.csv` & `duckcuts-1.0.2/src/duckcuts/data/vim-operators.csv`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/data/vim-text-objects.csv` & `duckcuts-1.0.2/src/duckcuts/data/vim-text-objects.csv`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/src/duckcuts/data/vim.csv` & `duckcuts-1.0.2/src/duckcuts/data/vim.csv`

 * *Files identical despite different names*

### Comparing `duckcuts-1.0.1/pyproject.toml` & `duckcuts-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 [project.scripts]
 duckcuts = "duckcuts.entry_points:duckcuts"
 
 [tool.hatch.build.targets.wheel]
 "data/" = "/"
 
 [tool.hatch.build.targets.sdist]
-exclude = ["pypitoken.txt", "dev_server.sh", "run.sh"]
+exclude = ["pypitoken.txt", "dev_server.sh", "run.sh", "pyproject.toml"]
 
-[project.urls]
-Documentation = "https://github.com/unknown/duckcuts#readme"
-Issues = "https://github.com/unknown/duckcuts/issues"
-Source = "https://github.com/unknown/duckcuts"
+# [project.urls]
+# Documentation = "https://github.com/unknown/duckcuts#readme"
+# Issues = "https://github.com/unknown/duckcuts/issues"
+# Source = "https://github.com/unknown/duckcuts"
 
 [tool.hatch.version]
 path = "src/duckcuts/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["coverage[toml]>=6.5", "pytest"]
 [tool.hatch.envs.default.scripts]
```

### Comparing `duckcuts-1.0.1/PKG-INFO` & `duckcuts-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Metadata-Version: 2.1
 Name: duckcuts
-Version: 1.0.1
+Version: 1.0.2
 Summary: An application for aiding learning shortcuts.
-Project-URL: Documentation, https://github.com/unknown/duckcuts#readme
-Project-URL: Issues, https://github.com/unknown/duckcuts/issues
-Project-URL: Source, https://github.com/unknown/duckcuts
 Author-email: vikbytes <55359319+vikbytes@users.noreply.github.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

