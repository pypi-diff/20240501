# Comparing `tmp/yedextended-1.0.7.tar.gz` & `tmp/yedextended-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.7.tar", last modified: Tue Apr 30 19:28:01 2024, max compression
+gzip compressed data, was "yedextended-1.0.8.tar", last modified: Wed May  1 12:20:46 2024, max compression
```

## Comparing `yedextended-1.0.7.tar` & `yedextended-1.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.635627 yedextended-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 19:27:55.000000 yedextended-1.0.7/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.627627 yedextended-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.631627 yedextended-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-30 19:27:55.000000 yedextended-1.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-30 19:27:55.000000 yedextended-1.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-30 19:27:55.000000 yedextended-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 19:27:55.000000 yedextended-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-30 19:28:01.635627 yedextended-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-30 19:27:55.000000 yedextended-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.631627 yedextended-1.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-basic-create-and-open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-basic-formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-basic_bulk_manage1.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-basic_bulk_manage2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-custom-properties-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-multilabels.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-round-robin_read_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-uml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/demo-url-description-groups-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/readme-1.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/readme-2.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/readme-3.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/test.graphml
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/yed_created_edges.graphml
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-30 19:27:55.000000 yedextended-1.0.7/examples/yed_modified_app_created.graphml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.635627 yedextended-1.0.7/images/
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/demo_multilabel.png
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/example-UML.png
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/example.png
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/excel_obj_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/excel_rel_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/graph.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/graph_from_excel_obj.gif
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-30 19:27:55.000000 yedextended-1.0.7/images/graph_from_excel_rel.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-30 19:27:55.000000 yedextended-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 19:27:55.000000 yedextended-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:28:01.635627 yedextended-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.627627 yedextended-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.635627 yedextended-1.0.7/src/yedextended/
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-30 19:27:55.000000 yedextended-1.0.7/src/yedextended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.635627 yedextended-1.0.7/src/yedextended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-30 19:28:01.000000 yedextended-1.0.7/src/yedextended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 19:28:01.000000 yedextended-1.0.7/src/yedextended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:28:01.000000 yedextended-1.0.7/src/yedextended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 19:28:01.000000 yedextended-1.0.7/src/yedextended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 19:28:01.000000 yedextended-1.0.7/src/yedextended.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-30 19:27:55.000000 yedextended-1.0.7/test_coverage.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:28:01.635627 yedextended-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:27:55.000000 yedextended-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-30 19:27:55.000000 yedextended-1.0.7/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 12:20:36.000000 yedextended-1.0.8/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.545099 yedextended-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.549100 yedextended-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-01 12:20:36.000000 yedextended-1.0.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-01 12:20:36.000000 yedextended-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 12:20:36.000000 yedextended-1.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-01 12:20:36.000000 yedextended-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:20:46.553099 yedextended-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-01 12:20:36.000000 yedextended-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic-create-and-open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic-formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic_bulk_manage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic_bulk_manage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-custom-properties-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-multilabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-round-robin_read_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-uml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-url-description-groups-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/readme-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/readme-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/readme-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/test.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/yed_created_edges.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/yed_modified_app_created.graphml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/demo_multilabel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/example-UML.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/excel_obj_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/excel_rel_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/graph.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/graph_from_excel_obj.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/graph_from_excel_rel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-01 12:20:36.000000 yedextended-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 12:20:36.000000 yedextended-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:20:46.553099 yedextended-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.549100 yedextended-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-05-01 12:20:36.000000 yedextended-1.0.8/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 12:20:36.000000 yedextended-1.0.8/test_coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:36.000000 yedextended-1.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-01 12:20:36.000000 yedextended-1.0.8/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.7/.github/workflows/ci.yml` & `yedextended-1.0.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/.github/workflows/python-publish.yml` & `yedextended-1.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/.gitignore` & `yedextended-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/LICENSE` & `yedextended-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/PKG-INFO` & `yedextended-1.0.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,65 @@
-Metadata-Version: 2.1
-Name: yedextended
-Version: 1.0.7
-Summary: Python library extending yEd functionality through programmatic interface to graphs.
-Author-email: Cole St John <info@colestjohn.com>
-Project-URL: Homepage, https://github.com/cole-st-john/yedextended
-Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: psutil
-Requires-Dist: pygetwindow
-Requires-Dist: openpyxl
-
 
 
 
 # Extended Python Support for yEd 
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
 ![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
-This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
+This Python library extends the functionality of the readily available and free interactive graph editing program [yEd](http://www.yworks.com/en/products_yed_about.html), through providing a programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following use case or functions:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
 - [x] management of the yEd application (starting, killing, maximizing)
 - [ ] enforcing rules on graphs
-- [ ] addition of standard sorting methods
+- [ ] additional layout methods
 - [ ] graph comparison tools
 
 ![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
 # Basic Usage
 
 Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
 
 
 ## Installing yEdExtended
-From Pypi, using pip:
+From PyPI, using pip:
 ```console
 $ pip install yedextended  
 ```
-Or from GITHUB:
+From GITHUB, using pip:
 ```console
 $ python -m pip install git+https://github.com/cole-st-john/yEdExtended
 ```
 
+From GITHUB, using git:
+```console
+$ git clone https://github.com/cole-st-john/yedextended
+```
+
 
 
 ## Importing yEdExtended for usage
 
 ```python
 import yedextended as yed
 ```
 
 
 ## Programmatically creating GraphML files
 
+With yEdExtended you can easily create graphs, either through hardcoding, or more practically, through porting data from any data source (databases, csv, xml, etc) into a graph and graph objects (nodes, groups, edges, properties):
+
+Hardcoding Example:
 ```python
 # Instantiate graph instance
 graph1 = yed.Graph()
 
 # Add arbitrary graph detail - nodes and edges
 graph1.add_node("a")
 graph1.add_node("b")
@@ -80,34 +68,39 @@
 # Add arbitrary graph detail - group and group objects
 group1 = graph1.add_group("group 1", shape="rectangle")
 group1.add_node("c")
 group1.add_node("d")
 group1.add_edge("c", "d")
 ```
 
+Programmatic Example:
 ```python
 # Adding graph objects based on csv input
 import csv
 with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
 	csv_reader = csv.reader(csv_file)
 	for row in csv_reader:
 	    graph1.add_node(row)
 ```
 
 ## Reading existing GraphML files
 
+yEdExtended can read GraphML files into a Python class structure, allowing for simple programmatic analysis and modification:
+
 ```python
 # Read graph file into python graph objects
 graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
 
 ```
 
 
 ## Using formatting
 
+yEdExtended provides for the majority of formatting one expects in yEd graphs.
+
 ```python
 # Add graph nodes and edges with some examples of non-default formatting
 graph1.add_node(
     "foo",
     font_family="Zapfino",
 )
 
@@ -150,41 +143,45 @@
     line_type="dotted",
 )
 ```
 
 
 ## Manipulating data in MS Excel 
 
+Sometimes, it is practical to mass edit or enter data in an interactive way.  yEdExtended includes functionality to enter basic to complex data and relationships using an interface to MS Excel interface. Note: to use this functionality, MS Excel must be installed and on path:
+
 ```python
 # Manage data in excel (add/remove/modify objects)
 graph1.manage_graph_data_in_excel() # default is object and hierachy management
 
 # Manage data in excel (add/remove/modify relations)
 graph1.manage_graph_data_in_excel(type="relations")
 ```
 
-### Adding Objects / Groups per Excel:
+### Excel - Adding Objects / Groups:
 
 ![Excel Object Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_obj_entry.gif)
 
 ### Result:
 
 ![Graph result of excel data entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_obj.gif)
 
-### Adding Relationships per Excel:
+### Excel - Adding Relationships:
 
 ![Excel Relation Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_rel_entry.gif)
 
 ### Result:
 
 ![Graph result of excel relation entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_rel.gif)
 
 
 ## Possible outputs of Graph
 
+Eventually, one normally wants to visualize or transmit the graph in some format.  Here are a few options:
+
 ```python
 # Demonstrate stringified GraphML version of structure
 print(graph1.stringify_graph())
 ```
 
 ```python
 # Several methods of writing graph to file ==============================
@@ -197,36 +194,36 @@
 graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
 
 ```
 
 
 ## Opening files in yEd Application *(assumes yEd installed and on PATH)*
 
-First install yEd application from [here](https://www.yworks.com/products/yed/download#download).
+To ease task switching between Python and yEd, functionality has been added to open graphs in yEd directly from Python.  Note: ensure you have installed yEd application from [here](https://www.yworks.com/products/yed/download#download) and that the app is on PATH (Win: "where yed.exe" in CMD should output a path).
 
 ```python
 # From existing handle
 graph_file.open_with_yed(force=True)
 
 # From file path
 yed.open_yed_file("examples/test.graphml")
 ```
 
 
 ## Visualizing in yEd Application (Layout)
 
-Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
+Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning (yEdExtended does not currently include functionality for layout, which is readily available in yEd):
 
 - ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
 - ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
 
 
 # Options
 
-Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
+Provides comprehensive support for great variety of ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
 
 
 
 # Development
 
 
 Interested in contributing or co-managing further development?  Just reach out!
```

### Comparing `yedextended-1.0.7/examples/demo-basic-create-and-open.py` & `yedextended-1.0.8/examples/demo-basic-create-and-open.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/demo-basic-formatting.py` & `yedextended-1.0.8/examples/demo-basic-formatting.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/demo-custom-properties-nodes-edges.py` & `yedextended-1.0.8/examples/demo-custom-properties-nodes-edges.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/demo-multilabels.py` & `yedextended-1.0.8/examples/demo-multilabels.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/demo-uml.py` & `yedextended-1.0.8/examples/demo-uml.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/demo-url-description-groups-nodes-edges.py` & `yedextended-1.0.8/examples/demo-url-description-groups-nodes-edges.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/readme-3.py` & `yedextended-1.0.8/examples/readme-3.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/test.graphml` & `yedextended-1.0.8/examples/test.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/yed_created_edges.graphml` & `yedextended-1.0.8/examples/yed_created_edges.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/examples/yed_modified_app_created.graphml` & `yedextended-1.0.8/examples/yed_modified_app_created.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/demo_multilabel.png` & `yedextended-1.0.8/images/demo_multilabel.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/example-UML.png` & `yedextended-1.0.8/images/example-UML.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/example.png` & `yedextended-1.0.8/images/example.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/excel_obj_entry.gif` & `yedextended-1.0.8/images/excel_obj_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/excel_rel_entry.gif` & `yedextended-1.0.8/images/excel_rel_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/graph.gif` & `yedextended-1.0.8/images/graph.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/graph_from_excel_obj.gif` & `yedextended-1.0.8/images/graph_from_excel_obj.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/images/graph_from_excel_rel.gif` & `yedextended-1.0.8/images/graph_from_excel_rel.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/pyproject.toml` & `yedextended-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/src/yedextended/__init__.py` & `yedextended-1.0.8/src/yedextended/__init__.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/src/yedextended.egg-info/PKG-INFO` & `yedextended-1.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,54 +24,62 @@
 # Extended Python Support for yEd 
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
 ![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
 
-This Python library extends [yEd](http://www.yworks.com/en/products_yed_about.html) functionality through programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following:
+This Python library extends the functionality of the readily available and free interactive graph editing program [yEd](http://www.yworks.com/en/products_yed_about.html), through providing a programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following use case or functions:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
 - [x] management of the yEd application (starting, killing, maximizing)
 - [ ] enforcing rules on graphs
-- [ ] addition of standard sorting methods
+- [ ] additional layout methods
 - [ ] graph comparison tools
 
 ![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
 # Basic Usage
 
 Below are some basic usages of yEdExtended in interfacing with yEd and GraphML files:
 
 
 ## Installing yEdExtended
-From Pypi, using pip:
+From PyPI, using pip:
 ```console
 $ pip install yedextended  
 ```
-Or from GITHUB:
+From GITHUB, using pip:
 ```console
 $ python -m pip install git+https://github.com/cole-st-john/yEdExtended
 ```
 
+From GITHUB, using git:
+```console
+$ git clone https://github.com/cole-st-john/yedextended
+```
+
 
 
 ## Importing yEdExtended for usage
 
 ```python
 import yedextended as yed
 ```
 
 
 ## Programmatically creating GraphML files
 
+With yEdExtended you can easily create graphs, either through hardcoding, or more practically, through porting data from any data source (databases, csv, xml, etc) into a graph and graph objects (nodes, groups, edges, properties):
+
+Hardcoding Example:
 ```python
 # Instantiate graph instance
 graph1 = yed.Graph()
 
 # Add arbitrary graph detail - nodes and edges
 graph1.add_node("a")
 graph1.add_node("b")
@@ -80,34 +88,39 @@
 # Add arbitrary graph detail - group and group objects
 group1 = graph1.add_group("group 1", shape="rectangle")
 group1.add_node("c")
 group1.add_node("d")
 group1.add_edge("c", "d")
 ```
 
+Programmatic Example:
 ```python
 # Adding graph objects based on csv input
 import csv
 with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
 	csv_reader = csv.reader(csv_file)
 	for row in csv_reader:
 	    graph1.add_node(row)
 ```
 
 ## Reading existing GraphML files
 
+yEdExtended can read GraphML files into a Python class structure, allowing for simple programmatic analysis and modification:
+
 ```python
 # Read graph file into python graph objects
 graph1 = yed.Graph().from_existing_graph("examples/yed_created_edges.graphml")
 
 ```
 
 
 ## Using formatting
 
+yEdExtended provides for the majority of formatting one expects in yEd graphs.
+
 ```python
 # Add graph nodes and edges with some examples of non-default formatting
 graph1.add_node(
     "foo",
     font_family="Zapfino",
 )
 
@@ -150,41 +163,45 @@
     line_type="dotted",
 )
 ```
 
 
 ## Manipulating data in MS Excel 
 
+Sometimes, it is practical to mass edit or enter data in an interactive way.  yEdExtended includes functionality to enter basic to complex data and relationships using an interface to MS Excel interface. Note: to use this functionality, MS Excel must be installed and on path:
+
 ```python
 # Manage data in excel (add/remove/modify objects)
 graph1.manage_graph_data_in_excel() # default is object and hierachy management
 
 # Manage data in excel (add/remove/modify relations)
 graph1.manage_graph_data_in_excel(type="relations")
 ```
 
-### Adding Objects / Groups per Excel:
+### Excel - Adding Objects / Groups:
 
 ![Excel Object Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_obj_entry.gif)
 
 ### Result:
 
 ![Graph result of excel data entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_obj.gif)
 
-### Adding Relationships per Excel:
+### Excel - Adding Relationships:
 
 ![Excel Relation Entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/excel_rel_entry.gif)
 
 ### Result:
 
 ![Graph result of excel relation entry](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph_from_excel_rel.gif)
 
 
 ## Possible outputs of Graph
 
+Eventually, one normally wants to visualize or transmit the graph in some format.  Here are a few options:
+
 ```python
 # Demonstrate stringified GraphML version of structure
 print(graph1.stringify_graph())
 ```
 
 ```python
 # Several methods of writing graph to file ==============================
@@ -197,36 +214,36 @@
 graph_file = graph1.persist_graph("pretty_example.graphml", pretty_print=True)  #  tool specific with formatting
 
 ```
 
 
 ## Opening files in yEd Application *(assumes yEd installed and on PATH)*
 
-First install yEd application from [here](https://www.yworks.com/products/yed/download#download).
+To ease task switching between Python and yEd, functionality has been added to open graphs in yEd directly from Python.  Note: ensure you have installed yEd application from [here](https://www.yworks.com/products/yed/download#download) and that the app is on PATH (Win: "where yed.exe" in CMD should output a path).
 
 ```python
 # From existing handle
 graph_file.open_with_yed(force=True)
 
 # From file path
 yed.open_yed_file("examples/test.graphml")
 ```
 
 
 ## Visualizing in yEd Application (Layout)
 
-Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning:
+Following programmatic creation or modification of a graph, consider using the following keystrokes in yEd to improve layout / positioning (yEdExtended does not currently include functionality for layout, which is readily available in yEd):
 
 - ``Tools -> Fit Node to Label``  (_Win: Alt + T + N_)
 - ``Layout -> Hierarchical``  (_Win: Alt + Shift + H_)
 
 
 # Options
 
-Provides comprehensive support for ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
+Provides comprehensive support for great variety of ``node_shapes``, ``line_types``, ``font_styles``, ``arrow_types``, custom parameters, UML, complex and deeply nested relationship structures and more.
 
 
 
 # Development
 
 
 Interested in contributing or co-managing further development?  Just reach out!
```

### Comparing `yedextended-1.0.7/src/yedextended.egg-info/SOURCES.txt` & `yedextended-1.0.8/src/yedextended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/test_coverage.svg` & `yedextended-1.0.8/test_coverage.svg`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.7/tests/test_yedextended.py` & `yedextended-1.0.8/tests/test_yedextended.py`

 * *Files identical despite different names*

