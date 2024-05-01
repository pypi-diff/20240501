# Comparing `tmp/jaal-0.1.5.tar.gz` & `tmp/jaal-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaal-0.1.5.tar", last modified: Sun Jul 30 06:41:20 2023, max compression
+gzip compressed data, was "jaal-0.1.7.tar", last modified: Wed May  1 18:28:33 2024, max compression
```

## Comparing `jaal-0.1.5.tar` & `jaal-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.457198 jaal-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-30 06:41:05.000000 jaal-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:41:20.457198 jaal-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-30 06:41:05.000000 jaal-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.453198 jaal-0.1.5/jaal/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.457198 jaal-0.1.5/jaal/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/datasets/load_got.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/datasets/parse_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/jaal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.457198 jaal-0.1.5/jaal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:41:20.457198 jaal-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-30 06:41:05.000000 jaal-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:28:33.559533 jaal-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 18:28:25.000000 jaal-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-01 18:28:33.559533 jaal-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-01 18:28:25.000000 jaal-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:28:33.559533 jaal-0.1.7/jaal/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-01 18:28:25.000000 jaal-0.1.7/jaal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:28:33.559533 jaal-0.1.7/jaal/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 18:28:25.000000 jaal-0.1.7/jaal/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-01 18:28:25.000000 jaal-0.1.7/jaal/datasets/load_got.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-01 18:28:25.000000 jaal-0.1.7/jaal/datasets/parse_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14666 2024-05-01 18:28:25.000000 jaal-0.1.7/jaal/jaal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-01 18:28:25.000000 jaal-0.1.7/jaal/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:28:33.559533 jaal-0.1.7/jaal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-01 18:28:33.000000 jaal-0.1.7/jaal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-01 18:28:33.000000 jaal-0.1.7/jaal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:28:33.000000 jaal-0.1.7/jaal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-01 18:28:33.000000 jaal-0.1.7/jaal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 18:28:33.000000 jaal-0.1.7/jaal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:28:33.559533 jaal-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-01 18:28:25.000000 jaal-0.1.7/setup.py
```

### Comparing `jaal-0.1.5/LICENSE` & `jaal-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jaal-0.1.5/PKG-INFO` & `jaal-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaal
-Version: 0.1.5
+Version: 0.1.7
 Summary: jaal - your interactive network visualizer dashboard
 Home-page: https://github.com/imohitmayank/jaal
 Author: Mohit Mayank
 Author-email: mohitmayank1@gmail.com
 License: UNKNOWN
 Description: <img src="jaal/assets/logo.png" alt="jaal logo"/>
         
@@ -111,14 +111,18 @@
         
         By default, `Jaal` plot undirected edges. This setting can be changed by,
         
         ```python
         Jaal(edge_df, node_df).plot(directed=True)
         ```
         
+        ### Showing Custom Title
+        
+        By default, `id` is shown as title. To overwrite this, include a `title` column with the respective data.
+        
         ### Showing Tooltip
         
         By default, `nodeid` is shown as tooltip. To overwrite this, include a `title` column with the respective data.
         
         ### Using vis.js settings
         
         We can tweak any of the `vis.js` related network visualization settings. An example is,
```

### Comparing `jaal-0.1.5/README.md` & `jaal-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,18 @@
 
 By default, `Jaal` plot undirected edges. This setting can be changed by,
 
 ```python
 Jaal(edge_df, node_df).plot(directed=True)
 ```
 
+### Showing Custom Title
+
+By default, `id` is shown as title. To overwrite this, include a `title` column with the respective data.
+
 ### Showing Tooltip
 
 By default, `nodeid` is shown as tooltip. To overwrite this, include a `title` column with the respective data.
 
 ### Using vis.js settings
 
 We can tweak any of the `vis.js` related network visualization settings. An example is,
```

### Comparing `jaal-0.1.5/jaal/datasets/load_got.py` & `jaal-0.1.7/jaal/datasets/load_got.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.5/jaal/datasets/parse_dataframe.py` & `jaal-0.1.7/jaal/datasets/parse_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         if 'title' not in node_df.columns:
             node_df['title'] = node_df['id']
         # see if node imge url is present or not
         node_image_url_flag = 'node_image_url' in node_df.columns
         # create the node data
         for node in node_df.to_dict(orient='records'):
             if not node_image_url_flag:
-                nodes.append({**node, **{'label': node['id'], 'shape': 'dot', 'size': 7}})
+                nodes.append({**node, **{'label': node['title'], 'shape': 'dot', 'size': 7}})
             else:
-                nodes.append({**node, **{'label': node['id'], 'shape': 'circularImage',
+                nodes.append({**node, **{'label': node['title'], 'shape': 'circularImage',
                                 'image': node['node_image_url'], 
                                 'size': 20}})
 
     # create edges from df
     edges = []
     for row in edge_df.to_dict(orient='records'):
         edges.append({**row, **{'id': row['from'] + "__" + row['to'],  'color': {'color': '#97C2FC'}}})
```

### Comparing `jaal-0.1.5/jaal/jaal.py` & `jaal-0.1.7/jaal/jaal.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.5/jaal/layout.py` & `jaal-0.1.7/jaal/layout.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.5/jaal.egg-info/PKG-INFO` & `jaal-0.1.7/jaal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaal
-Version: 0.1.5
+Version: 0.1.7
 Summary: jaal - your interactive network visualizer dashboard
 Home-page: https://github.com/imohitmayank/jaal
 Author: Mohit Mayank
 Author-email: mohitmayank1@gmail.com
 License: UNKNOWN
 Description: <img src="jaal/assets/logo.png" alt="jaal logo"/>
         
@@ -111,14 +111,18 @@
         
         By default, `Jaal` plot undirected edges. This setting can be changed by,
         
         ```python
         Jaal(edge_df, node_df).plot(directed=True)
         ```
         
+        ### Showing Custom Title
+        
+        By default, `id` is shown as title. To overwrite this, include a `title` column with the respective data.
+        
         ### Showing Tooltip
         
         By default, `nodeid` is shown as tooltip. To overwrite this, include a `title` column with the respective data.
         
         ### Using vis.js settings
         
         We can tweak any of the `vis.js` related network visualization settings. An example is,
```

### Comparing `jaal-0.1.5/setup.py` & `jaal-0.1.7/setup.py`

 * *Files identical despite different names*

