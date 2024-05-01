# Comparing `tmp/dosmaster-1.8.6.tar.gz` & `tmp/dosmaster-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.8.6.tar", last modified: Tue Apr 30 13:44:40 2024, max compression
+gzip compressed data, was "dist/dosmaster-1.8.7.tar", last modified: Wed May  1 08:18:40 2024, max compression
```

## Comparing `dosmaster-1.8.6.tar` & `dosmaster-1.8.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.6/LICENSE
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.6/MANIFEST.in
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-30 13:44:40.000000 dosmaster-1.8.6/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2980 2024-04-26 15:26:24.000000 dosmaster-1.8.6/README.md
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/__init__.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/base/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/base/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/base/data_generation.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5322 2024-04-26 15:25:24.000000 dosmaster-1.8.6/dosmaster/base/printer.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/custom_setting/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/custom_setting/example_default.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/custom_setting/example_figure_size_up.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/custom_setting/example_font_size_up.yaml
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/features/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/a_add_atom_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/b_dos_projection.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/c_dos_sum.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/d_average_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/e_remove_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/f_change_sign.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/g_graph_editor.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5911 2024-04-30 13:40:39.000000 dosmaster-1.8.6/dosmaster/features/h_axis_optimization.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/i_import_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/j_save_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/k_import_dosmaster_data.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/features/l_save_dosmaster_data.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/fileparser/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/fileparser/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/fileparser/doscar_split.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/fileparser/procar_parser.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/fileparser/structure_parser.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/main/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-04-30 13:41:54.000000 dosmaster-1.8.6/dosmaster/main/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-04-30 13:42:29.000000 dosmaster-1.8.6/dosmaster/main/dosmaster.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/mainplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/mainplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/mainplotter/dosplot.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster/subplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/subplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/subplotter/colors.csv
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/subplotter/colortable.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/subplotter/dosplot_manager.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.6/dosmaster/subplotter/make_color_list.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/entry_points.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/requires.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-04-30 13:44:40.000000 dosmaster-1.8.6/dosmaster.egg-info/top_level.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-04-30 13:44:40.000000 dosmaster-1.8.6/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2024-04-24 17:41:51.000000 dosmaster-1.8.6/setup.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.7/LICENSE
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.7/MANIFEST.in
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      838 2024-05-01 08:18:40.000000 dosmaster-1.8.7/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3164 2024-05-01 08:17:39.000000 dosmaster-1.8.7/README.md
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/__init__.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/base/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/base/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5322 2024-04-26 15:25:24.000000 dosmaster-1.8.7/dosmaster/base/printer.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/custom_setting/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/custom_setting/example_default.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/custom_setting/example_figure_size_up.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/custom_setting/example_font_size_up.yaml
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/features/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/a_add_atom_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/b_dos_projection.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/c_dos_sum.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/d_average_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/e_remove_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/f_change_sign.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/g_graph_editor.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5911 2024-04-30 13:40:39.000000 dosmaster-1.8.7/dosmaster/features/h_axis_optimization.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/i_import_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/j_save_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/k_import_dosmaster_data.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/features/l_save_dosmaster_data.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/fileparser/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/fileparser/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/fileparser/doscar_split.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/fileparser/procar_parser.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/fileparser/structure_parser.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/main/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-05-01 08:14:41.000000 dosmaster-1.8.7/dosmaster/main/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-04-30 13:42:29.000000 dosmaster-1.8.7/dosmaster/main/dosmaster.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/mainplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/mainplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/mainplotter/dosplot.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster/subplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/subplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/subplotter/colors.csv
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/subplotter/colortable.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/subplotter/dosplot_manager.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.7/dosmaster/subplotter/make_color_list.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      838 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/requires.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-05-01 08:18:40.000000 dosmaster-1.8.7/dosmaster.egg-info/top_level.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-05-01 08:18:40.000000 dosmaster-1.8.7/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1556 2024-05-01 08:14:10.000000 dosmaster-1.8.7/setup.py
```

### Comparing `dosmaster-1.8.6/LICENSE` & `dosmaster-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/PKG-INFO` & `dosmaster-1.8.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.8.6
+Version: 1.8.7
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim in CNMD
 Author-email: yjpark29@postech.ac.kr
 License: MIT
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
@@ -12,8 +12,11 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7.13
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+DOS(Density Of States) Plot Smartly and Conveniently in Terminal Environment.
```

### Comparing `dosmaster-1.8.6/README.md` & `dosmaster-1.8.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # DOSMaster
 
 Link for dosmaster-pypi package(click the icon)
 
 [![PyPI](https://img.shields.io/pypi/v/dosmaster.svg)](https://pypi.org/project/dosmaster/)
+[![GitHub](https://img.shields.io/badge/GitHub-DOSMaster-green)](https://github.com/pyj6767/DOSMaster)
 
 Program Name : dosmaster Program
 
 Made by Youngjun Park (yjpark29@postech.ac.kr)
 
 Inspired by Jaesun Kim(CNMD)
 
@@ -35,14 +36,15 @@
 
 ver 1.8.3 : ISPIN = 1 calculation 지원 및 각종 버그 수정
 
 ver 1.8.4 : Lisence 수정
 
 ver 1.8.5 : f orbital error 수정
 
+ver 1.8.7 : Save plot in current directory - ylim optimization 시 오류 수정
 
 ## Features
 1) Add Atom DOS : 원하는 atom의 DOS를 추가합니다.
 2) DOS Projection : 특정 DOS를 원하는 orbital로 projection 시킵니다.
 3) Sum DOS : 특정 DOS들의 기여분을 합칩니다.
 4) Average DOS : 특정 DOS들의 기여분을 평균화합니다.
 5) Remove DOS : 특정 DOS를 지웁니다.
```

### Comparing `dosmaster-1.8.6/dosmaster/base/data_generation.py` & `dosmaster-1.8.7/dosmaster/base/data_generation.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/base/printer.py` & `dosmaster-1.8.7/dosmaster/base/printer.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/a_add_atom_dos.py` & `dosmaster-1.8.7/dosmaster/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/b_dos_projection.py` & `dosmaster-1.8.7/dosmaster/features/b_dos_projection.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/c_dos_sum.py` & `dosmaster-1.8.7/dosmaster/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/d_average_dos.py` & `dosmaster-1.8.7/dosmaster/features/d_average_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/e_remove_dos.py` & `dosmaster-1.8.7/dosmaster/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/f_change_sign.py` & `dosmaster-1.8.7/dosmaster/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/g_graph_editor.py` & `dosmaster-1.8.7/dosmaster/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/h_axis_optimization.py` & `dosmaster-1.8.7/dosmaster/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/i_import_custom_setting.py` & `dosmaster-1.8.7/dosmaster/features/i_import_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/j_save_custom_setting.py` & `dosmaster-1.8.7/dosmaster/features/j_save_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/k_import_dosmaster_data.py` & `dosmaster-1.8.7/dosmaster/features/k_import_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/features/l_save_dosmaster_data.py` & `dosmaster-1.8.7/dosmaster/features/l_save_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/fileparser/doscar_split.py` & `dosmaster-1.8.7/dosmaster/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/fileparser/structure_parser.py` & `dosmaster-1.8.7/dosmaster/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/main/dosmaster.py` & `dosmaster-1.8.7/dosmaster/main/dosmaster.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/mainplotter/dosplot.py` & `dosmaster-1.8.7/dosmaster/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/subplotter/colors.csv` & `dosmaster-1.8.7/dosmaster/subplotter/colors.csv`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/subplotter/colortable.py` & `dosmaster-1.8.7/dosmaster/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/subplotter/dosplot_manager.py` & `dosmaster-1.8.7/dosmaster/subplotter/dosplot_manager.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster/subplotter/make_color_list.py` & `dosmaster-1.8.7/dosmaster/subplotter/make_color_list.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.8.7/dosmaster.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.8.6
+Version: 1.8.7
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim in CNMD
 Author-email: yjpark29@postech.ac.kr
 License: MIT
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
@@ -12,8 +12,11 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7.13
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+DOS(Density Of States) Plot Smartly and Conveniently in Terminal Environment.
```

### Comparing `dosmaster-1.8.6/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.8.7/dosmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.6/setup.py` & `dosmaster-1.8.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 #with open("README.md") as file:
 #    long_description = file.read()
 
 setup(
     name="dosmaster",
     version=__version__,
     description="DOS(Density Of States) Plot Smartly in Terminal",
+    long_description="DOS(Density Of States) Plot Smartly and Conveniently in Terminal Environment.",
+    long_description_content_type="text/markdown",
     url="https://github.com/pyj6767/DOSMaster",
     author="Youngjun Park, Jaeson Kim in CNMD",
     author_email="yjpark29@postech.ac.kr",
     #long_description=long_description,
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
```

