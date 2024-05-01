# Comparing `tmp/gridengine_framework-0.8.4.tar.gz` & `tmp/gridengine_framework-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridengine_framework-0.8.4.tar", last modified: Tue Apr 23 11:18:14 2024, max compression
+gzip compressed data, was "gridengine_framework-0.8.5.tar", last modified: Wed May  1 07:43:51 2024, max compression
```

## Comparing `gridengine_framework-0.8.4.tar` & `gridengine_framework-0.8.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/
--rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.8.4/LICENSE
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.8.4/README.md
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.830616 gridengine_framework-0.8.4/grid_engine/
--rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.8.4/grid_engine/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.8.4/grid_engine/__log__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.8.4/grid_engine/__main__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.830616 gridengine_framework-0.8.4/grid_engine/_blueprint/
--rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/_floorplan_classes.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/_floorplan_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-04-22 05:11:05.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/_grid_blueprint.py
--rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/_grid_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/_terrain_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/objects.json
--rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.8.4/grid_engine/_blueprint/terrains.json
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.830616 gridengine_framework-0.8.4/grid_engine/_cell/
--rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.8.4/grid_engine/_cell/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    32407 2024-04-23 10:41:35.000000 gridengine_framework-0.8.4/grid_engine/_cell/cell.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.8.4/grid_engine/_dungeon.py
--rw-r--r--   0 boss      (1000) boss      (1002)    54746 2024-04-23 10:41:49.000000 gridengine_framework-0.8.4/grid_engine/_grid.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_grid_feature/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_feature/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_feature/grid_feature.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_grid_group/
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 06:07:32.000000 gridengine_framework-0.8.4/grid_engine/_grid_group/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3648 2024-04-23 10:20:01.000000 gridengine_framework-0.8.4/grid_engine/_grid_group/grid_group.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_grid_object/
--rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/__init__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_item/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_item/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_item/grid_item.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_object.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_structure/
--rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_structure/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_structure/grid_structure.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_zone/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_zone/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.8.4/grid_engine/_grid_object/grid_zone/grid_zone.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/grid_engine/_terraform/
--rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.8.4/grid_engine/_terraform/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    13214 2024-04-23 11:18:05.000000 gridengine_framework-0.8.4/grid_engine/_terraform/terraformer.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.8.4/grid_engine/_utility.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.8.4/grid_engine/layout_test.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/gridengine_framework.egg-info/
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-23 11:18:14.000000 gridengine_framework-0.8.4/gridengine_framework.egg-info/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-23 11:18:14.000000 gridengine_framework-0.8.4/gridengine_framework.egg-info/SOURCES.txt
--rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-23 11:18:14.000000 gridengine_framework-0.8.4/gridengine_framework.egg-info/dependency_links.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-23 11:18:14.000000 gridengine_framework-0.8.4/gridengine_framework.egg-info/requires.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-23 11:18:14.000000 gridengine_framework-0.8.4/gridengine_framework.egg-info/top_level.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-23 11:18:14.833949 gridengine_framework-0.8.4/setup.cfg
--rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-23 11:18:11.000000 gridengine_framework-0.8.4/setup.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/
+-rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.8.5/LICENSE
+-rw-r--r--   0 boss      (1000) boss      (1002)     5832 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     5300 2024-05-01 07:43:13.000000 gridengine_framework-0.8.5/README.md
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.750058 gridengine_framework-0.8.5/grid_engine/
+-rw-r--r--   0 boss      (1000) boss      (1002)      370 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1293 2024-04-27 03:09:12.000000 gridengine_framework-0.8.5/grid_engine/__log__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4931 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/__main__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_blueprint/
+-rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/__main__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2689 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_floorplan_classes.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3820 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_floorplan_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-05-01 07:41:54.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_blueprint.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10986 2024-04-24 16:18:00.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_terrain_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/objects.json
+-rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/terrains.json
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_cell/
+-rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.8.5/grid_engine/_cell/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    32408 2024-05-01 07:24:21.000000 gridengine_framework-0.8.5/grid_engine/_cell/cell.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4756 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_dungeon.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    54929 2024-05-01 07:43:06.000000 gridengine_framework-0.8.5/grid_engine/_grid.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_feature/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_feature/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2975 2024-04-25 05:52:12.000000 gridengine_framework-0.8.5/grid_engine/_grid_feature/grid_feature.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_group/
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_grid_group/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3648 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_grid_group/grid_group.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/
+-rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/__init__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/grid_item.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2767 2024-04-25 07:25:29.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_object.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/
+-rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/grid_structure.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/grid_zone.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_terraform/
+-rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_terraform/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    13627 2024-05-01 07:41:17.000000 gridengine_framework-0.8.5/grid_engine/_terraform/terraformer.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     6614 2024-04-24 16:17:44.000000 gridengine_framework-0.8.5/grid_engine/_utility.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/layout_test.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/gridengine_framework.egg-info/
+-rw-r--r--   0 boss      (1000) boss      (1002)     5832 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/requires.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/top_level.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/setup.cfg
+-rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-05-01 07:43:29.000000 gridengine_framework-0.8.5/setup.py
```

### Comparing `gridengine_framework-0.8.4/LICENSE` & `gridengine_framework-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/PKG-INFO` & `gridengine_framework-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine_framework
-Version: 0.8.4
+Version: 0.8.5
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,28 +26,27 @@
 
     ```bash
     pip install grid_engine
     ```
 
 ## Usage
 
-To use **gridengine** you can import any number of the submodules and utilize its respective features.
+To use **gridengine** you can import any number of the submodules and utilize its respective features or you can import the main module.
 
     ```python
-    import gridengine
-    from gridengine import grid
+    import grid_engine as ge
     
     # Create a grid
-    grid = grid.Grid(cell_size=10, grid_dimensions=(1000, 1000))
+    grid = ge.grid.Grid(cell_size=10, grid_dimensions=(1000, 1000))
     
     # Save a grid
-    grid.save_grid()
+    ge.grid.save_grid(grid)
     
     # Load a grid
-    loaded_grid = grid.Grid.load_grid(1)
+    loaded_grid = ge.grid.Grid.load_grid(1)
     ```
 
 grid-engine also provides a command line interface. To use it, run the following command:
 
     ```bash
     python -m grid_engine --help
```

### Comparing `gridengine_framework-0.8.4/README.md` & `gridengine_framework-0.8.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 
     ```bash
     pip install grid_engine
     ```
 
 ## Usage
 
-To use **gridengine** you can import any number of the submodules and utilize its respective features.
+To use **gridengine** you can import any number of the submodules and utilize its respective features or you can import the main module.
 
     ```python
-    import gridengine
-    from gridengine import grid
+    import grid_engine as ge
     
     # Create a grid
-    grid = grid.Grid(cell_size=10, grid_dimensions=(1000, 1000))
+    grid = ge.grid.Grid(cell_size=10, grid_dimensions=(1000, 1000))
     
     # Save a grid
-    grid.save_grid()
+    ge.grid.save_grid(grid)
     
     # Load a grid
-    loaded_grid = grid.Grid.load_grid(1)
+    loaded_grid = ge.grid.Grid.load_grid(1)
     ```
 
 grid-engine also provides a command line interface. To use it, run the following command:
 
     ```bash
     python -m grid_engine --help
```

### Comparing `gridengine_framework-0.8.4/grid_engine/__log__.py` & `gridengine_framework-0.8.5/grid_engine/__log__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/__main__.py` & `gridengine_framework-0.8.5/grid_engine/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_blueprint/__main__.py` & `gridengine_framework-0.8.5/grid_engine/_blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_blueprint/_grid_blueprint.py` & `gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_blueprint.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_blueprint/_grid_processing.py` & `gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_blueprint/_terrain_processing.py` & `gridengine_framework-0.8.5/grid_engine/_blueprint/_terrain_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import json
 
 _COLORS = {
     'OCEAN_BLUE': (16, 78, 139, 255),
     'BARREN_BROWN': (77, 88, 77, 255),
     'GRASS_GREEN': (84, 139, 84, 255),
+    'FOREST_GREEN': (55, 201, 99, 255),
     'PLAIN_GREEN': (90, 154, 90, 255),
     'FOOTHILL_GREEN': (82, 144, 78, 255),
     'GULCH_GREEN': (74, 130, 70, 255),
     'GULCH_GREY': (80, 110, 90, 255),
     'BEACH_GREEN': (99, 170, 112, 255),
     'SEASHELL_WHITE': (249, 235, 231, 255),
     'SANDSTONE_GREY': (169, 169, 169, 255),
```

### Comparing `gridengine_framework-0.8.4/grid_engine/_blueprint/terrains.json` & `gridengine_framework-0.8.5/grid_engine/_blueprint/terrains.json`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_cell/cell.py` & `gridengine_framework-0.8.5/grid_engine/_cell/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from collections import deque
 
 from .._grid_group import GridGroup
 
 import logging as _logging
 
 from abc import ABC
```

### Comparing `gridengine_framework-0.8.4/grid_engine/_dungeon.py` & `gridengine_framework-0.8.5/grid_engine/_dungeon.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_grid.py` & `gridengine_framework-0.8.5/grid_engine/_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations as _annotations
+
 import random as _random
 
 import pyglet as _pyglet
 
 from .__log__ import logger as _logger, log_method as _log_method
 
 from ._terraform import Terraformer
@@ -898,15 +899,19 @@
         for count, step in enumerate(path):
             if not self[step].passable:
                 path = path[:count]
                 break
         return path, cost
 
     @_log_method
-    def get_walk(self, start_cell: _Optional[str] = None, end_cell: _Optional[str] = None):
+    def get_walk(self, start_cell: _Union[str, _Cell] = None, end_cell: _Union[str, _Cell] = None):
+        if isinstance(start_cell, _Cell):
+            start_cell = start_cell.designation
+        if isinstance(end_cell, _Cell):
+            end_cell = end_cell.designation
         walk_cells = [start_cell]
         if start_cell != end_cell:
             current_distance = self.get_distance(start_cell, end_cell, 'cells')
             while current_distance > 1:
                 current_cell = self.cells[walk_cells[-1]]
                 adjacent_cells = [adjacent_cell for adjacent_cell in current_cell.adjacent if
                                   self.cells[adjacent_cell].passable and adjacent_cell not in walk_cells]
```

### Comparing `gridengine_framework-0.8.4/grid_engine/_grid_feature/grid_feature.py` & `gridengine_framework-0.8.5/grid_engine/_grid_feature/grid_feature.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 class Grid(ABC):
     pass
 
 class Cell(ABC):
     pass
 
 class AbstractGridFeature(QuietDict, ABC):
+    """Abstract class for a grid feature. A grid feature is a collection of cells that share a common property or characteristic.
+    A grid feature differs from a grid group in that it is an implicit property of the grid, whereas a grid group is an explicit property of the grid.
+    A good example of a grid feature is a river, which is a collection of cells that share the property of being part of a river
+    or a mountain range, which is a collection of cells that share the property of being part of a mountain range."""
+    
     def __init__(self, grid: Grid, cells: List[Cell], title: str):
         self.grid = grid
         self.cells = cells
         self.title = title
         self.initiate_feature()
 
     def initiate_feature(self):
```

### Comparing `gridengine_framework-0.8.4/grid_engine/_grid_group/grid_group.py` & `gridengine_framework-0.8.5/grid_engine/_grid_group/grid_group.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_grid_object/grid_item/grid_item.py` & `gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/grid_item.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_grid_object/grid_structure/grid_structure.py` & `gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/grid_structure.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_grid_object/grid_zone/grid_zone.py` & `gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/grid_zone.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/grid_engine/_terraform/terraformer.py` & `gridengine_framework-0.8.5/grid_engine/_terraform/terraformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import itertools
 import random
 
 RIVER_BLUE = (16, 78, 139, 255)
 RIVERBANK_SAND = (188, 182, 134, 255)
 RIVERBANK_GRASS = (105, 105, 105, 255)
 RIVERBANK_MOUND = (112, 128, 136, 255)
+FOREST_GREEN = (0, 155, 22, 255)
 
 class Cell(ABC):
     pass
 
 class Grid(ABC):
     pass
 
@@ -49,19 +50,18 @@
     @property
     def rivers(self) -> list[list[Cell,]]:
         self.grid.rivers
 
     @_log_method
     def generate_realistic_river(self, start_cell: Cell, end_cell: Cell = None):
         # paths = self.get_river_bends(start_cell, end_cell)
-        print('Getting river cells by walk ...')
+        print('Generating river ...')
         path = self.get_river_by_walk(start_cell, end_cell)
         path = list(itertools.chain.from_iterable(path))
         path = [self.cells[cell] for cell in path]
-        print(f'River steps: {len(path)}')
         if path is not None:
             path = self.expand_river_path(path)
             step = 0
             total_steps = len(path)
             split = False
             # shaped_path = self.shape_river_path(expanded_path)
             for cell in path:
@@ -147,15 +147,14 @@
                             'cost_out': 2
                             }
                         riverbank_cells.append(adjacent_cell)
         return riverbank_cells
 
 
     def random_walk(self, river_cells: list[Cell,]):
-        print('Generating random river ...')
         for step in range(random.randint(199, 201)):
             current_cell = self.cells[river_cells[-1]]
             if adjacent_cells := [
                 adjacent_cell
                 for adjacent_cell in current_cell.adjacent
                 if adjacent_cell is not None and self.cells[adjacent_cell].passable
             ]:
@@ -167,29 +166,27 @@
                     else (direction + 2) % 8
                 )
                 next_cell = adjacent_cells[(direction + (0 if step % 3 else int(random.uniform(-5, 5)))) % len(adjacent_cells)]
                 river_cells.append(next_cell)
         return river_cells
 
     def deliberate_walk(self, river_cells: list[Cell,], start_cell: Cell, end_cell: Cell):
-        print('Generating river with end designated ...')
         start_distance = self.grid.get_distance(start_cell, end_cell)
         current_distance = self.grid.get_distance(start_cell, end_cell)
         while current_distance > 1:
             current_cell = self.cells[river_cells[-1]]
             adjacent_cells = [adjacent_cell for adjacent_cell in current_cell.adjacent if adjacent_cell is not None and self.cells[adjacent_cell].passable and adjacent_cell not in river_cells]
             if not adjacent_cells:
                 river_cells.pop(-1)
                 break
             else:
                 direction = random.randint(0, len(adjacent_cells)-1) if len(adjacent_cells) > 1 else 0
                 next_cell = adjacent_cells[direction]
             check_ = 0
             while self.grid.get_distance(next_cell, end_cell) > current_distance and check_  < 8:
-                print(f'Current distance: {current_distance} | Current cell: {current_cell.designation} | Next cell: {next_cell}', end='\r')
                 direction += 1
                 direction %= len(adjacent_cells)
                 check_ += 1
                 next_cell = adjacent_cells[direction]
                 continue
             river_cells.append(next_cell)
             current_distance = self.grid.get_distance(next_cell, end_cell)
@@ -199,20 +196,18 @@
     @_log_method
     def get_river_by_walk(self, start_cell: Cell, end_cell: Cell = None):
         river_cells = [start_cell]
         if end_cell is None:
             river_cells = self.random_walk(river_cells)
         else:
             river_cells = self.deliberate_walk(river_cells, start_cell, end_cell)
-            print(f'Cells in river: {len(river_cells)}')
         return [river_cells]
         
     @_log_method
     def set_rivers(self, river_count):
-        print('Finding start to river ...')
         for river in range(river_count):
             if self.grid.river_count > 0 and not river % 3:
                 start: Cell = random.choice(self.grid.rivers[-1])
                 end: Cell = random.choice(self.grid.landmasses[start.landmass_index]['coastal_cells'])
             elif river > 2:
                 if lake_coastal_cells := self.grid._get_lake_coastal_cells():
                     end: Cell = random.choice(lake_coastal_cells)
@@ -222,82 +217,97 @@
                 landmass = self.grid._get_largest_landmass()
                 coast_cells = landmass['coastal_cells']
                 start: Cell = random.choice(coast_cells)
                 if lake_coastal_cells := self.grid._get_lake_coastal_cells():
                     end: Cell = random.choice(lake_coastal_cells)
                 else:
                     end: Cell = random.choice(coast_cells)
-                print('Validating start/end of river ...')
-                print(f'Start cell: {start}, End cell: {end}', end = '\r')
                 while self.grid.get_distance(
                     start.designation, end.designation, 'cells'
                 ) < 100 or not [
                     adjacent_cell
                     for adjacent_cell in start.adjacent
                     if adjacent_cell is not None and self.cells[adjacent_cell].passable
                 ]:
                     start = random.choice(coast_cells)
                     end = random.choice(lake_coastal_cells) if lake_coastal_cells else random.choice(coast_cells)
-                    print(f'Start cell: {start}, End cell: {end}', end = '\r')
-            print(f'Start cell: {start}, End cell: {end}')
-            print('Building river ...')
             self.generate_realistic_river(start.designation, end.designation)
         riverbanks = self.get_river_banks()
         self.expand_riverbanks(riverbanks)
-        print('done')            
  
     def seed_forest(self):
         start_cell = self.grid.random_cell()
-        while start_cell.clearance_x < 10 or start_cell.clearance_y < 10:
+        while start_cell.clearance_left < 50 or start_cell.clearance_right < 50 or start_cell.clearance_up < 50 or start_cell.clearance_down < 50:
             start_cell = self.grid.random_cell()
         return start_cell
- 
-    def get_forest_borders(self, start_cells: Union[Cell, List[Cell]]):
-        forest_border_start = start_cells.get_diagonal(-1, -1, 5)[-1]
-        forest_border_step2 = start_cells.get_diagonal(-1, 1, 5)[-1]
-        forest_border_step3 = start_cells.get_diagonal(1, 1, 5)[-1]
-        forest_border_step4 = start_cells.get_diagonal(1, -1, 5)[-1]
+
+    def find_forest_points(self, start_cell: Cell):
+        forest_border_NW = self.grid[start_cell.get_diagonal(-1, -1, random.choice([10,12,16,20]))[-1]]
+        forest_border_NE = self.grid[start_cell.get_diagonal(-1, 1, random.choice([10,12,16,20]))[-1]]
+        forest_border_SE = self.grid[start_cell.get_diagonal(1, 1, random.choice([10,12,16,20]))[-1]]
+        forest_border_SW = self.grid[start_cell.get_diagonal(1, -1, random.choice([10,12,16,20]))[-1]]
+        return (forest_border_NW, forest_border_NE, forest_border_SE, forest_border_SW)
+        
+    def get_forest_borders(self, forest_points: Tuple[Cell, Cell, Cell, Cell]):
         forest_border = []
-        step1 = self.grid.get_walk(forest_border_start, forest_border_step2)
-        forest_border.extend(step1)
-        step2 = self.grid.get_walk(forest_border_step2, forest_border_step3)
-        forest_border.extend(step2)
-        step3 = self.grid.get_walk(forest_border_step3, forest_border_step4)
-        forest_border.extend(step3)
-        step4 = self.grid.get_walk(forest_border_step4, forest_border_start)
-        forest_border.extend(step4)
+        for step in range(4):
+            forest_step = self.grid.get_walk(forest_points[step], forest_points[(step+1)%4])
+            forest_border.extend(forest_step)
         return forest_border
+
+    def expand_forest_border(self, forest_border):
+        expanded_forest_border = []
+        for cell in forest_border:
+            cell = self.grid[cell]
+            for adjacent in cell.adjacent:
+                if adjacent is not None:
+                    adjacent = self.grid[adjacent]
+                    if adjacent.passable:
+                        expanded_forest_border.append(adjacent.designation)
+            expanded_forest_border.append(cell.designation)
+        return expanded_forest_border
         
     def get_inner_forest_cells(self, start_cell, forest_border):
         for cell in forest_border:
-            self.grid[cell].passable = False
+            cell = self.grid[cell]
+            for adjacent in cell.adjacent:
+                if adjacent is not None:
+                    adjacent = self.grid[adjacent]
+                    adjacent.passable = False
+            cell.passable = False
         inner_forest_cells = start_cell.get_clearance_zone()
         inner_forest_cells = inner_forest_cells.cells
         for cell in forest_border:
-            self.grid[cell].passable = True
+            cell = self.grid[cell]
+            for adjacent in cell.adjacent:
+                if adjacent is not None:
+                    adjacent = self.grid[adjacent]
+                    adjacent.passable = True
+            cell.passable = True
         forest_cells = []
         forest_cells.extend(forest_border)
         for cell in inner_forest_cells:
             forest_cells.append(cell.designation)
         return forest_cells
     
     def set_forest(self):
-        start_cells = self.seed_forest()
-        forest_borders = self.get_forest_borders(start_cells)
-        forest_cells = self.get_inner_forest_cells(start_cells, forest_borders)
+        start_cell = self.seed_forest()
+        forest_points = self.find_forest_points(start_cell)
+        forest_borders = self.get_forest_borders(forest_points)
+        expanded_forest_borders = self.expand_forest_border(forest_borders)
+        forest_cells = self.get_inner_forest_cells(start_cell, expanded_forest_borders)
         for cell in forest_cells:
             cell = self.grid[cell]
             cell.terrain_str = 'FOREST'
             cell.terrain_raw = 0.0
             cell.terrain_int = 4
-            cell.terrain_color = 'GRASS_GREEN'
+            cell.terrain_color = FOREST_GREEN
             cell.terrain_char = '^'
             self.dictTerrain[cell.designation] = {
                 'str': cell.terrain_str, 
                 'raw': cell.terrain_raw, 
                 'int': cell.terrain_int, 
                 'color': cell.terrain_color, 
                 'cost_in': 2, 
                 'cost_out': 2,
                 'char': '^'
                 }
-
```

### Comparing `gridengine_framework-0.8.4/grid_engine/_utility.py` & `gridengine_framework-0.8.5/grid_engine/_utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # This file contains utility functions for the grid engine.
 import os
 # Path: grid-engine/utility.py
 
+_COLORS = {
+    'OCEAN_BLUE': (16, 78, 139, 255),
+    'BARREN_BROWN': (77, 88, 77, 255),
+    'GRASS_GREEN': (84, 139, 84, 255),
+    'FOREST_GREEN': (55, 201, 99, 255),
+    'PLAIN_GREEN': (90, 154, 90, 255),
+    'FOOTHILL_GREEN': (82, 144, 78, 255),
+    'GULCH_GREEN': (74, 130, 70, 255),
+    'GULCH_GREY': (80, 110, 90, 255),
+    'BEACH_GREEN': (99, 170, 112, 255),
+    'SEASHELL_WHITE': (249, 235, 231, 255),
+    'SANDSTONE_GREY': (169, 169, 169, 255),
+    'SANDY_GREY': (188, 182, 134, 255),
+    'MOUND_GREY': (105, 105, 105, 255),
+    'BASIN_BROWN': (91, 101, 91, 255),
+    'BASE_GREY': (112, 128, 136, 255),
+    'SIDE_GREY': (79, 83, 72, 255),
+    'CRAG_GREY': (48, 42, 36, 255),
+    'SNOW_WHITE': (253, 245, 245, 255)
+}
+
 CWD = os.getcwd()
 if not os.path.exists(f'{CWD}/saves/'):
     os.mkdir(f'{CWD}/saves/')
 
 SAVES_DIR = f'{CWD}/saves/'
 
 def get_grid_dir(grid_id):
@@ -64,14 +85,16 @@
             random.shuffle(cat_cells)
             for count in range(0, cat_count, cat_count//60):
                 for cell in zip(range(cat_count//60), cat_cells[count:count+(cat_count//60)]):
                     i, cell = cell
                     x, y = cell[0]
                     color = cell[1]
                     ctgry = cell[2]
+                    if isinstance(color, str):
+                        color = _COLORS[color]                        
                     draw.rectangle((x, y, x+cell_size, y+cell_size), fill=color if ctgry == category else (90, 154, 90, 255))
                 frames.append(image.copy())
         river_count = categories.count('RIVER')
         river_cells = [cell for cell in cells if cell[2] == 'RIVER']
         for count in range(0, river_count, river_count//10):
             for cell in zip(range(river_count//10), river_cells[count:count+(river_count//10)]):
                 i, cell = cell
@@ -80,31 +103,32 @@
                 draw.rectangle((x, y, x+cell_size, y+cell_size), fill=color)
             frames.append(image.copy())
         print('Saving grid animation ...')
         grid_id = grid_id[-5:]
         grid_dir = get_grid_dir(grid_id)
         frames[0].save(f'{grid_dir}grid.gif', format='GIF', append_images=frames[1:], save_all=True, duration=0.001, loop=0)
         print(f'grid.gif saved to {grid_dir}.')
-        print('Press ')
-    else:
-        for i, cell in enumerate(cells):
-            print(f'Drawing cells         {round((i/total_cell_count)*100)}%', end='\r')
-            x = cell[0]
-            y = cell[1]
-            color = cell[2]
-            draw.rectangle((x, y, x+cell_size, y+cell_size), fill=color)
-        print('Cells drawn.                                   ')
-    print('Saving grid image ...')
+    for i, cell in enumerate(cells):
+        print(f'Drawing static image         {round((i/total_cell_count)*100)}%', end='\r')
+        x, y = cell[0]
+        color = cell[1]
+        draw.rectangle((x, y, x+cell_size, y+cell_size), fill=color)
+    print('Cells drawn.')
+    print('Saving static grid image ...')
     image.save(f'{grid_dir}grid.png')
     print(f'grid.png saved to {grid_dir}.')
-    
-    import matplotlib.pyplot as plt
-    
-    plt.imshow(image)
-    plt.show()   
+
+    print('Press ENTER to display the grid image using matplotlib.')
+    print('Press ctrl+C to exit.')
+    display = input()
+    if display == '':    
+        import matplotlib.pyplot as plt
+
+        plt.imshow(image)
+        plt.show()   
     
 # Define the QuietDict class
 
 from typing import Union
 
 class QuietDict:
     def __init__(self):
```

### Comparing `gridengine_framework-0.8.4/grid_engine/layout_test.py` & `gridengine_framework-0.8.5/grid_engine/layout_test.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/gridengine_framework.egg-info/PKG-INFO` & `gridengine_framework-0.8.5/gridengine_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine-framework
-Version: 0.8.4
+Version: 0.8.5
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,28 +26,27 @@
 
     ```bash
     pip install grid_engine
     ```
 
 ## Usage
 
-To use **gridengine** you can import any number of the submodules and utilize its respective features.
+To use **gridengine** you can import any number of the submodules and utilize its respective features or you can import the main module.
 
     ```python
-    import gridengine
-    from gridengine import grid
+    import grid_engine as ge
     
     # Create a grid
-    grid = grid.Grid(cell_size=10, grid_dimensions=(1000, 1000))
+    grid = ge.grid.Grid(cell_size=10, grid_dimensions=(1000, 1000))
     
     # Save a grid
-    grid.save_grid()
+    ge.grid.save_grid(grid)
     
     # Load a grid
-    loaded_grid = grid.Grid.load_grid(1)
+    loaded_grid = ge.grid.Grid.load_grid(1)
     ```
 
 grid-engine also provides a command line interface. To use it, run the following command:
 
     ```bash
     python -m grid_engine --help
```

### Comparing `gridengine_framework-0.8.4/gridengine_framework.egg-info/SOURCES.txt` & `gridengine_framework-0.8.5/gridengine_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.4/setup.py` & `gridengine_framework-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name='gridengine_framework',
-    version='0.8.4',
+    version='0.8.5',
     description='A framework for generating and manipulating grid-based game worlds',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='James Evans',
     author_email='joesaysahoy@gmail.com',
     url='https://github.com/primal-coder/grid-engine',
     packages=find_packages(),
```

