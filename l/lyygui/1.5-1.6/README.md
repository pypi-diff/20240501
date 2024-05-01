# Comparing `tmp/lyygui-1.5.tar.gz` & `tmp/lyygui-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyygui-1.5.tar", last modified: Wed May  1 13:59:48 2024, max compression
+gzip compressed data, was "lyygui-1.6.tar", last modified: Wed May  1 14:00:53 2024, max compression
```

## Comparing `lyygui-1.5.tar` & `lyygui-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 13:59:48.794477 lyygui-1.5/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyygui-1.5/LICENSE
--rw-rw-rw-   0        0        0      143 2024-05-01 13:59:48.794477 lyygui-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyygui-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 13:59:48.793468 lyygui-1.5/lyygui.egg-info/
--rw-rw-rw-   0        0        0      143 2024-05-01 13:59:48.000000 lyygui-1.5/lyygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-01 13:59:48.000000 lyygui-1.5/lyygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 13:59:48.000000 lyygui-1.5/lyygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 13:59:48.000000 lyygui-1.5/lyygui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 13:59:48.000000 lyygui-1.5/lyygui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1071 2023-10-28 18:51:52.000000 lyygui-1.5/lyytkmain.py
--rw-rw-rw-   0        0        0       42 2024-05-01 13:59:48.795482 lyygui-1.5/setup.cfg
--rw-rw-rw-   0        0        0      268 2024-05-01 13:59:47.000000 lyygui-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:00:53.398977 lyygui-1.6/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyygui-1.6/LICENSE
+-rw-rw-rw-   0        0        0      143 2024-05-01 14:00:53.398977 lyygui-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyygui-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 14:00:53.397976 lyygui-1.6/lyygui.egg-info/
+-rw-rw-rw-   0        0        0      143 2024-05-01 14:00:53.000000 lyygui-1.6/lyygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-01 14:00:53.000000 lyygui-1.6/lyygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:00:53.000000 lyygui-1.6/lyygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-01 14:00:53.000000 lyygui-1.6/lyygui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 14:00:53.000000 lyygui-1.6/lyygui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1071 2023-10-28 18:51:52.000000 lyygui-1.6/lyytkfunction.py
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:00:53.398977 lyygui-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      268 2024-05-01 14:00:52.000000 lyygui-1.6/setup.py
```

### Comparing `lyygui-1.5/LICENSE` & `lyygui-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lyygui-1.5/lyytkmain.py` & `lyygui-1.6/lyytkfunction.py`

 * *Files identical despite different names*

