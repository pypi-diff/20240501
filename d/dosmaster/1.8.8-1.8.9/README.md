# Comparing `tmp/dosmaster-1.8.8.tar.gz` & `tmp/dosmaster-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.8.8.tar", last modified: Wed May  1 08:22:48 2024, max compression
+gzip compressed data, was "dist/dosmaster-1.8.9.tar", last modified: Wed May  1 17:39:08 2024, max compression
```

## Comparing `dosmaster-1.8.8.tar` & `dosmaster-1.8.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.8/LICENSE
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.8/MANIFEST.in
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3924 2024-05-01 08:22:48.000000 dosmaster-1.8.8/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3164 2024-05-01 08:20:34.000000 dosmaster-1.8.8/README.md
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/__init__.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/base/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/base/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/base/data_generation.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5322 2024-04-26 15:25:24.000000 dosmaster-1.8.8/dosmaster/base/printer.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/custom_setting/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/custom_setting/example_default.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/custom_setting/example_figure_size_up.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/custom_setting/example_font_size_up.yaml
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/features/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/a_add_atom_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/b_dos_projection.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/c_dos_sum.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/d_average_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/e_remove_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/f_change_sign.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/g_graph_editor.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5911 2024-04-30 13:40:39.000000 dosmaster-1.8.8/dosmaster/features/h_axis_optimization.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/i_import_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/j_save_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/k_import_dosmaster_data.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/features/l_save_dosmaster_data.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/fileparser/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/fileparser/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/fileparser/doscar_split.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/fileparser/procar_parser.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/fileparser/structure_parser.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/main/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-05-01 08:20:24.000000 dosmaster-1.8.8/dosmaster/main/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-04-30 13:42:29.000000 dosmaster-1.8.8/dosmaster/main/dosmaster.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/mainplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/mainplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/mainplotter/dosplot.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster/subplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/subplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/subplotter/colors.csv
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/subplotter/colortable.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/subplotter/dosplot_manager.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.8/dosmaster/subplotter/make_color_list.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3924 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/entry_points.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/requires.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-05-01 08:22:48.000000 dosmaster-1.8.8/dosmaster.egg-info/top_level.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-05-01 08:22:48.000000 dosmaster-1.8.8/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1491 2024-05-01 08:22:11.000000 dosmaster-1.8.8/setup.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.9/LICENSE
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.9/MANIFEST.in
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3964 2024-05-01 17:39:08.000000 dosmaster-1.8.9/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3204 2024-05-01 17:38:27.000000 dosmaster-1.8.9/README.md
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/__init__.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/base/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/base/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5322 2024-04-26 15:25:24.000000 dosmaster-1.8.9/dosmaster/base/printer.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/custom_setting/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/custom_setting/example_default.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/custom_setting/example_figure_size_up.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/custom_setting/example_font_size_up.yaml
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/features/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/a_add_atom_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/b_dos_projection.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/c_dos_sum.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/d_average_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/e_remove_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/f_change_sign.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/g_graph_editor.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5911 2024-04-30 13:40:39.000000 dosmaster-1.8.9/dosmaster/features/h_axis_optimization.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/i_import_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/j_save_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/k_import_dosmaster_data.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/features/l_save_dosmaster_data.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/fileparser/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/fileparser/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/fileparser/doscar_split.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/fileparser/procar_parser.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/fileparser/structure_parser.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/main/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-05-01 17:37:49.000000 dosmaster-1.8.9/dosmaster/main/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-04-30 13:42:29.000000 dosmaster-1.8.9/dosmaster/main/dosmaster.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/mainplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/mainplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/mainplotter/dosplot.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster/subplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/subplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/subplotter/colors.csv
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/subplotter/colortable.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     7574 2024-05-01 17:37:32.000000 dosmaster-1.8.9/dosmaster/subplotter/dosplot_manager.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.9/dosmaster/subplotter/make_color_list.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3964 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/requires.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-05-01 17:39:08.000000 dosmaster-1.8.9/dosmaster.egg-info/top_level.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-05-01 17:39:08.000000 dosmaster-1.8.9/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1491 2024-05-01 08:22:11.000000 dosmaster-1.8.9/setup.py
```

### Comparing `dosmaster-1.8.8/LICENSE` & `dosmaster-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/PKG-INFO` & `dosmaster-1.8.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.8.8
+Version: 1.8.9
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim in CNMD
 Author-email: yjpark29@postech.ac.kr
 License: MIT
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
@@ -59,14 +59,16 @@
 
 ver 1.8.4 : Lisence 수정
 
 ver 1.8.5 : f orbital error 수정
 
 ver 1.8.8 : Save plot in current directory - ylim optimization 시 오류 수정
 
+ver 1.8.9 : f orbital sum error 수정
+
 ## Features
 1) Add Atom DOS : 원하는 atom의 DOS를 추가합니다.
 2) DOS Projection : 특정 DOS를 원하는 orbital로 projection 시킵니다.
 3) Sum DOS : 특정 DOS들의 기여분을 합칩니다.
 4) Average DOS : 특정 DOS들의 기여분을 평균화합니다.
 5) Remove DOS : 특정 DOS를 지웁니다.
 6) Plot only Positive/Negative part : DOS plot의 양/음수 부분만 plot합니다.
```

### Comparing `dosmaster-1.8.8/README.md` & `dosmaster-1.8.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 ver 1.8.4 : Lisence 수정
 
 ver 1.8.5 : f orbital error 수정
 
 ver 1.8.8 : Save plot in current directory - ylim optimization 시 오류 수정
 
+ver 1.8.9 : f orbital sum error 수정
+
 ## Features
 1) Add Atom DOS : 원하는 atom의 DOS를 추가합니다.
 2) DOS Projection : 특정 DOS를 원하는 orbital로 projection 시킵니다.
 3) Sum DOS : 특정 DOS들의 기여분을 합칩니다.
 4) Average DOS : 특정 DOS들의 기여분을 평균화합니다.
 5) Remove DOS : 특정 DOS를 지웁니다.
 6) Plot only Positive/Negative part : DOS plot의 양/음수 부분만 plot합니다.
```

### Comparing `dosmaster-1.8.8/dosmaster/base/data_generation.py` & `dosmaster-1.8.9/dosmaster/base/data_generation.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/base/printer.py` & `dosmaster-1.8.9/dosmaster/base/printer.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/a_add_atom_dos.py` & `dosmaster-1.8.9/dosmaster/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/b_dos_projection.py` & `dosmaster-1.8.9/dosmaster/features/b_dos_projection.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/c_dos_sum.py` & `dosmaster-1.8.9/dosmaster/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/d_average_dos.py` & `dosmaster-1.8.9/dosmaster/features/d_average_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/e_remove_dos.py` & `dosmaster-1.8.9/dosmaster/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/f_change_sign.py` & `dosmaster-1.8.9/dosmaster/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/g_graph_editor.py` & `dosmaster-1.8.9/dosmaster/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/h_axis_optimization.py` & `dosmaster-1.8.9/dosmaster/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/i_import_custom_setting.py` & `dosmaster-1.8.9/dosmaster/features/i_import_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/j_save_custom_setting.py` & `dosmaster-1.8.9/dosmaster/features/j_save_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/k_import_dosmaster_data.py` & `dosmaster-1.8.9/dosmaster/features/k_import_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/features/l_save_dosmaster_data.py` & `dosmaster-1.8.9/dosmaster/features/l_save_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/fileparser/doscar_split.py` & `dosmaster-1.8.9/dosmaster/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/fileparser/structure_parser.py` & `dosmaster-1.8.9/dosmaster/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/main/dosmaster.py` & `dosmaster-1.8.9/dosmaster/main/dosmaster.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/mainplotter/dosplot.py` & `dosmaster-1.8.9/dosmaster/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/subplotter/colors.csv` & `dosmaster-1.8.9/dosmaster/subplotter/colors.csv`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/subplotter/colortable.py` & `dosmaster-1.8.9/dosmaster/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster/subplotter/dosplot_manager.py` & `dosmaster-1.8.9/dosmaster/subplotter/dosplot_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,24 @@
             for cn in column_names[1:]:
                 if cn[0] == 'd' or cn == 'x2-y2':
                     if cn.split('_')[1] == 'up':
                         dos_up += np.array(dataframe_object[cn])
                     elif cn.split('_')[1] == 'down':
                         dos_down += np.array(dataframe_object[cn])
 
+        elif orbital_select_element == 'f':
+            dos_up = np.array([0 for e in energy], dtype=np.float64)
+            dos_down = np.array([0 for e in energy], dtype=np.float64)
+            for cn in column_names[1:]:
+                if cn[0] == 'd':
+                    if cn.split('_')[1] == 'up':
+                        dos_up += np.array(dataframe_object[cn])
+                    elif cn.split('_')[1] == 'down':
+                        dos_down += np.array(dataframe_object[cn])
+
         else:
             for cn in column_names[1:]:
                 if cn == orbital_select_element+'_up':
                     dos_up = np.array(dataframe_object[cn], dtype=np.float64)
                 elif cn == orbital_select_element+'_down':
                     dos_down = np.array(dataframe_object[cn], dtype=np.float64)
         
@@ -172,8 +182,8 @@
 def data_collection(data_list, is_save, graph_config, energy, dos_data):
     if is_save == True:
         if len(data_list) == 0:
             data_list.append(energy)
             data_list.append(dos_data)
         else:
             data_list.append(dos_data)
-    return data_list
+    return data_list
```

### Comparing `dosmaster-1.8.8/dosmaster/subplotter/make_color_list.py` & `dosmaster-1.8.9/dosmaster/subplotter/make_color_list.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.8.9/dosmaster.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.8.8
+Version: 1.8.9
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim in CNMD
 Author-email: yjpark29@postech.ac.kr
 License: MIT
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
@@ -59,14 +59,16 @@
 
 ver 1.8.4 : Lisence 수정
 
 ver 1.8.5 : f orbital error 수정
 
 ver 1.8.8 : Save plot in current directory - ylim optimization 시 오류 수정
 
+ver 1.8.9 : f orbital sum error 수정
+
 ## Features
 1) Add Atom DOS : 원하는 atom의 DOS를 추가합니다.
 2) DOS Projection : 특정 DOS를 원하는 orbital로 projection 시킵니다.
 3) Sum DOS : 특정 DOS들의 기여분을 합칩니다.
 4) Average DOS : 특정 DOS들의 기여분을 평균화합니다.
 5) Remove DOS : 특정 DOS를 지웁니다.
 6) Plot only Positive/Negative part : DOS plot의 양/음수 부분만 plot합니다.
```

### Comparing `dosmaster-1.8.8/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.8.9/dosmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.8/setup.py` & `dosmaster-1.8.9/setup.py`

 * *Files identical despite different names*

