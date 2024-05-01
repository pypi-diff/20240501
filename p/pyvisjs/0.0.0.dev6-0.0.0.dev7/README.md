# Comparing `tmp/pyvisjs-0.0.0.dev6.tar.gz` & `tmp/pyvisjs-0.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev6.tar", last modified: Sun Apr 28 18:39:03 2024, max compression
+gzip compressed data, was "pyvisjs-0.0.0.dev7.tar", last modified: Wed May  1 16:40:09 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev6.tar` & `pyvisjs-0.0.0.dev7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.864136 pyvisjs-0.0.0.dev6/
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-28 18:39:03.863136 pyvisjs-0.0.0.dev6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.858136 pyvisjs-0.0.0.dev6/examples/
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.860136 pyvisjs-0.0.0.dev6/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     3006 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.861136 pyvisjs-0.0.0.dev6/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.863136 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      637 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-28 18:39:03.000000 pyvisjs-0.0.0.dev6/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 18:39:03.864136 pyvisjs-0.0.0.dev6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:39:03.862136 pyvisjs-0.0.0.dev6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     7893 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-28 18:38:47.000000 pyvisjs-0.0.0.dev6/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.839229 pyvisjs-0.0.0.dev7/
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4004 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-05-01 16:40:09.838229 pyvisjs-0.0.0.dev7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.833229 pyvisjs-0.0.0.dev7/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/examples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.835229 pyvisjs-0.0.0.dev7/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2014 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     5161 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    12282 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.836229 pyvisjs-0.0.0.dev7/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.838229 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      637 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 16:40:09.839229 pyvisjs-0.0.0.dev7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.838229 pyvisjs-0.0.0.dev7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev6/.gitignore` & `pyvisjs-0.0.0.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/.gitlab-ci.yml` & `pyvisjs-0.0.0.dev7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/LICENSE` & `pyvisjs-0.0.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/PKG-INFO` & `pyvisjs-0.0.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev6
+Version: 0.0.0.dev7
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev6/README.md` & `pyvisjs-0.0.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/examples/main.py` & `pyvisjs-0.0.0.dev7/examples/main.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/folder_structure.txt` & `pyvisjs-0.0.0.dev7/folder_structure.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 pyvisjs-dev/
 ├── pyvisjs/
 │   ├── templates/
 │   │   └── basic.html
 │   ├── __init__.py
 │   ├── _version.py
+│   ├── base_dictable.py
+│   ├── edge.py
 │   ├── network.py
 │   ├── node.py
-│   ├── edge.py
+│   ├── options.py
 │   └── utils.py
 ├── tests/
 │   ├── __init__.py
-│   ├── test_units.py
-│   └── test_network.py
+│   ├── test_base_dictable.py
+│   ├── test_edge.py
+│   ├── test_network.py
+│   ├── test_node.py
+│   ├── test_options.py
+│   └── test_utils.py
 ├── examples/
+│   ├── readme_usage.py
 │   └── main.py
 ├── .gitignore
-├── requirements.txt
-├── pyproject.toml
-├── README.md
+├── .gitlab-ci.yml
+├── CONTRIBUTING.md
 ├── LICENSE
-└── .venv/
+├── README.md
+├── requirements.txt
+├── folder_structure.txt
+└── pyproject.toml
```

### Comparing `pyvisjs-0.0.0.dev6/pyproject.toml` & `pyvisjs-0.0.0.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/pyvisjs/base_dictable.py` & `pyvisjs-0.0.0.dev7/pyvisjs/base_dictable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+from typing import Dict
+
 class BaseDictable:
 
     def __init__(self, attr_filter_func=None, attr_map_func=None):
         self.attr_filter_func = attr_filter_func or (lambda x: x)
         self.attr_map_func = attr_map_func or (lambda x: x)
 
+    def _update_dict_with_locals(self, _dict:Dict, _locals:Dict):
+        for attr_name, attr_value in _locals.items():
+            if attr_value is not None and attr_name != "self":
+                _dict.update({attr_name: attr_value})
+
     def to_dict(self):
         result = {}
 
         def has_to_dict(attr):
             return hasattr(attr, "to_dict") and callable(getattr(attr, "to_dict"))
         
         def process_attr(attr):
@@ -26,14 +33,18 @@
                 attr_value = getattr(self, attr_name)
                 attr_name = self.attr_map_func(attr_name)
                 if callable(attr_value):
                     continue
                 elif isinstance(attr_value, list):
                     result[attr_name] = process_list(attr_value)
                 elif isinstance(attr_value, dict):
+                    if not attr_value: continue
                     result[attr_name] = process_dict(attr_value)
                 elif has_to_dict(attr_value):
-                    result[attr_name] = attr_value.to_dict()
+                    obj_dict = attr_value.to_dict()
+                    if not obj_dict: continue
+                    result[attr_name] = obj_dict
                 else:
+                    if not attr_value: continue
                     result[attr_name] = attr_value
                     
         return result
```

### Comparing `pyvisjs-0.0.0.dev6/pyvisjs/templates/basic.html` & `pyvisjs-0.0.0.dev7/pyvisjs/templates/basic.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/pyvisjs/utils.py` & `pyvisjs-0.0.0.dev7/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-0.0.0.dev7/pyvisjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev6
+Version: 0.0.0.dev7
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev6/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-0.0.0.dev7/pyvisjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/tests/test_base_dictable.py` & `pyvisjs-0.0.0.dev7/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev6/tests/test_network.py` & `pyvisjs-0.0.0.dev7/tests/test_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,38 +20,24 @@
     assert n.env is not None
     assert n.to_dict() == DEFAULT_DICT
 
 def test_network_init_with_data():
     # init
     NETWORK_DICT = {
         "nodes": [
-            { "id": 1, "label": "node 1", "color": None, "shape": "dot", "size": None, "cid": None },
-            { "id": 2, "label": "node 2", "color": None, "shape": "dot", "size": None, "cid": None },
-            { "id": 3, "label": "node 3", "color": None, "shape": "dot", "size": None, "cid": None },
+            { "id": 1, "label": "node 1", "shape": "dot" },
+            { "id": 2, "label": "node 2", "shape": "dot" },
+            { "id": 3, "label": "node 3", "shape": "dot" },
         ],
         "edges": [
             { "from": 1, "to": 2 },
             { "from": 2, "to": 3 },
             { "from": 3, "to": 4 }
         ],
-        "options": {
-            "width": "100%",
-            "height": "100%",
-            "edges": {"color": "GRAY", "smooth": False},
-            "nodes": {
-                "scaling": {
-                    "max": 60, 
-                    "min": 10
-                }
-            },
-            "physics": {
-                "barnesHut": {"gravitationalConstant": None},
-                "stabilization": {"iterations": None}
-            }
-        }
+        "options": {}
     }
     # mock
 
 
     # call
     nd1 = Node(1, "node 1")
     nd2 = Node(2, "node 2")
@@ -104,53 +90,56 @@
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_node(2) # duplicate node
+    n.add_node(3, "hello", "red", "circle", None, None, category="high")
     
     # assert
-    assert len(n.nodes) == 2
+    assert len(n.nodes) == 3
     assert n.nodes[0].id == 1
     assert n.nodes[0].label == "1"
     assert n.nodes[1].id == 2
     assert n.nodes[1].label == "name2"
+    assert n.nodes[2].category == "high"
 
 def test_network_add_edges():
     # init
 
     # mock
 
     # call
     n = Network("Network1")
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_edge(1, 2) # both nodes exist
-    n.add_edge(2, 3) # one node missing
+    n.add_edge(2, 3, country="LV") # one node missing
     n.add_edge(2, 3) # duplicate edge
     
     # assert
     assert n.nodes[0].id == 1
     assert n.nodes[1].id == 2
     assert n.nodes[2].id == 3
 
     assert len(n.edges) == 2
     assert n.edges[0].start == 1
     assert n.edges[0].end == 2
     assert n.edges[1].start == 2
     assert n.edges[1].end == 3
+    assert n.edges[1].country == "LV"
 
 def test_network_to_dict():
     # init
     NETWORK_DICT = {
         "nodes": [
-            { "id": 1, "label": "1", "color": None, "shape": "dot", "size": None, "cid": None },
-            { "id": 2, "label": "name2", "color": None, "shape": "dot", "size": None, "cid": None },
-            { "id": 3, "label": "3", "color": None, "shape": "dot", "size": None, "cid": None },
+            { "id": 1, "label": "1", "shape": "dot" },
+            { "id": 2, "label": "name2", "shape": "dot" },
+            { "id": 3, "label": "3", "shape": "dot" },
         ],
         "edges": [
             { "from": 1, "to": 2 },
             { "from": 2, "to": 3 }
         ],
         "options": {}
     }
```

### Comparing `pyvisjs-0.0.0.dev6/tests/test_node.py` & `pyvisjs-0.0.0.dev7/tests/test_node.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     # call
     n = Node(NODE_ID)
     
     # assert
     assert n.id == NODE_ID
 
-def test_node_init_positional_params():
+def test_node_init_positional_args():
     # init
     NODE_ID = 1
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
     NODE_SIZE = 50
 
@@ -24,31 +24,70 @@
 
     # call
     n = Node(NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
     
     # assert
     assert (n.id, n.label, n.color, n.shape, n.size) == (NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
 
+def test_node_init_keyword_args():
+    # init
+    NODE_ID = 1
+    NODE_LABEL = "label"
+    NODE_COLOR = "lime"
+    NODE_SHAPE = "circle"
+    NODE_SIZE = 50
+    NODE_CID = 1
+
+    # mock
+
+    # call
+    n = Node(NODE_ID, label=NODE_LABEL, cid=NODE_CID, size=NODE_SIZE, shape=NODE_SHAPE, color=NODE_COLOR)
+    
+    # assert
+    assert (n.id, n.label, n.color, n.shape, n.size, n.cid) == (NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE, NODE_CID)
+
+def test_node_init_kwargs():
+    # init
+    NODE_ID = 1
+    NODE_LABEL = "label"
+    NODE_COLOR = "lime"
+    NODE_SHAPE = "circle"
+    NODE_SIZE = 50
+    NODE_CID = 1
+    NODE_CATEGORY = "category1"
+    NODE_AMOUNT = 1009.4
+    NODE_HASVALUE = False
+
+    # mock
+
+    # call
+    n = Node(NODE_ID, label=NODE_LABEL, cid=NODE_CID, size=NODE_SIZE, shape=NODE_SHAPE, color=NODE_COLOR
+             , category=NODE_CATEGORY, amount=NODE_AMOUNT, has_value=NODE_HASVALUE)
+    
+    # assert
+    assert (n.id, n.label, n.color, n.shape, n.size, n.cid, n.category, n.amount, n.has_value) \
+        == (NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE, NODE_CID, NODE_CATEGORY, NODE_AMOUNT, NODE_HASVALUE)
+
 def test_node_to_dict():
     # init
     NODE_ID = 1
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
     NODE_CID = None
     NODE_SIZE = 50
     NODE_DICT = {
             "id": NODE_ID,
             "label": NODE_LABEL,
             "color": NODE_COLOR,
             "shape": NODE_SHAPE,
             "size": NODE_SIZE,
-            "cid": NODE_CID,
+            # no element for cid, because it was set to None
         }
 
     # mock
 
     # call
-    n = Node(NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
+    n = Node(NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE, NODE_CID)
     
     # assert
     assert n.to_dict() == NODE_DICT
```

### Comparing `pyvisjs-0.0.0.dev6/tests/test_utils.py` & `pyvisjs-0.0.0.dev7/tests/test_utils.py`

 * *Files identical despite different names*

