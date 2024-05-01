# Comparing `tmp/qgoferutils-0.0.7.tar.gz` & `tmp/qgoferutils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgoferutils-0.0.7.tar", last modified: Thu Mar  7 21:23:27 2024, max compression
+gzip compressed data, was "qgoferutils-0.0.8.tar", last modified: Wed May  1 17:29:21 2024, max compression
```

## Comparing `qgoferutils-0.0.7.tar` & `qgoferutils-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 21:23:27.929858 qgoferutils-0.0.7/
--rw-rw-rw-   0        0        0    11337 2023-04-27 10:12:58.000000 qgoferutils-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      111 2023-04-27 10:12:58.000000 qgoferutils-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1544 2024-03-07 21:23:27.925852 qgoferutils-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      604 2024-03-07 21:09:30.000000 qgoferutils-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-07 21:23:27.845308 qgoferutils-0.0.7/qgoferutils/
--rw-rw-rw-   0        0        0       23 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-03-07 21:22:38.000000 qgoferutils-0.0.7/qgoferutils/_modidx.py
--rw-rw-rw-   0        0        0     5032 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/config.py
--rw-rw-rw-   0        0        0     1808 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/core.py
--rw-rw-rw-   0        0        0     3950 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/db.py
--rw-rw-rw-   0        0        0     1949 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/logger.py
--rw-rw-rw-   0        0        0     4895 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/manage_index.py
--rw-rw-rw-   0        0        0     1898 2024-03-07 21:22:37.000000 qgoferutils-0.0.7/qgoferutils/requests.py
-drwxrwxrwx   0        0        0        0 2024-03-07 21:23:27.922857 qgoferutils-0.0.7/qgoferutils.egg-info/
--rw-rw-rw-   0        0        0     1544 2024-03-07 21:23:26.000000 qgoferutils-0.0.7/qgoferutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-03-07 21:23:27.000000 qgoferutils-0.0.7/qgoferutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 21:23:26.000000 qgoferutils-0.0.7/qgoferutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-07 21:23:26.000000 qgoferutils-0.0.7/qgoferutils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-02 14:15:08.000000 qgoferutils-0.0.7/qgoferutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2024-03-07 21:23:26.000000 qgoferutils-0.0.7/qgoferutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-07 21:23:26.000000 qgoferutils-0.0.7/qgoferutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      954 2024-03-07 21:18:21.000000 qgoferutils-0.0.7/settings.ini
--rw-rw-rw-   0        0        0       42 2024-03-07 21:23:27.930863 qgoferutils-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2596 2023-04-27 10:12:58.000000 qgoferutils-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:29:21.290777 qgoferutils-0.0.8/
+-rw-rw-rw-   0        0        0    11337 2023-04-27 10:12:58.000000 qgoferutils-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      111 2023-04-27 10:12:58.000000 qgoferutils-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4614 2024-05-01 17:29:21.290777 qgoferutils-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3543 2024-05-01 17:21:06.000000 qgoferutils-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 17:29:21.194637 qgoferutils-0.0.8/qgoferutils/
+-rw-rw-rw-   0        0        0       23 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-05-01 17:28:52.000000 qgoferutils-0.0.8/qgoferutils/_modidx.py
+-rw-rw-rw-   0        0        0     5032 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/config.py
+-rw-rw-rw-   0        0        0     1808 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/core.py
+-rw-rw-rw-   0        0        0     3950 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/db.py
+-rw-rw-rw-   0        0        0     1949 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/logger.py
+-rw-rw-rw-   0        0        0     4906 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/manage_index.py
+-rw-rw-rw-   0        0        0     1898 2024-05-01 17:28:51.000000 qgoferutils-0.0.8/qgoferutils/requests.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:29:21.282833 qgoferutils-0.0.8/qgoferutils.egg-info/
+-rw-rw-rw-   0        0        0     4614 2024-05-01 17:29:20.000000 qgoferutils-0.0.8/qgoferutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-05-01 17:29:20.000000 qgoferutils-0.0.8/qgoferutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 17:29:20.000000 qgoferutils-0.0.8/qgoferutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-01 17:29:20.000000 qgoferutils-0.0.8/qgoferutils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-03-02 14:15:08.000000 qgoferutils-0.0.8/qgoferutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2024-05-01 17:29:20.000000 qgoferutils-0.0.8/qgoferutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 17:29:20.000000 qgoferutils-0.0.8/qgoferutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      954 2024-05-01 17:27:28.000000 qgoferutils-0.0.8/settings.ini
+-rw-rw-rw-   0        0        0       42 2024-05-01 17:29:21.290777 qgoferutils-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2596 2023-04-27 10:12:58.000000 qgoferutils-0.0.8/setup.py
```

### Comparing `qgoferutils-0.0.7/LICENSE` & `qgoferutils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/qgoferutils/_modidx.py` & `qgoferutils-0.0.8/qgoferutils/_modidx.py`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/qgoferutils/config.py` & `qgoferutils-0.0.8/qgoferutils/config.py`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/qgoferutils/core.py` & `qgoferutils-0.0.8/qgoferutils/core.py`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/qgoferutils/db.py` & `qgoferutils-0.0.8/qgoferutils/db.py`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/qgoferutils/logger.py` & `qgoferutils-0.0.8/qgoferutils/logger.py`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/qgoferutils/manage_index.py` & `qgoferutils-0.0.8/qgoferutils/manage_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     path = Path(path).expanduser().resolve()
     try:
         for item in path.iterdir():
             if item.name.startswith("."):
                 continue
             if item.is_dir():
                 if item.name in folders_to_index:
-                    yield from index_folders(item)
+                    yield from index_folders(item, data_type)
             elif item.is_file():
                 if data_type == "document":
                     if item.suffix not in (VIDEO + AUDIO + IMAGE):
                         yield item
                 elif data_type == "video":
                     if item.suffix in VIDEO:
                         yield item
```

### Comparing `qgoferutils-0.0.7/qgoferutils/requests.py` & `qgoferutils-0.0.8/qgoferutils/requests.py`

 * *Files identical despite different names*

### Comparing `qgoferutils-0.0.7/settings.ini` & `qgoferutils-0.0.8/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = qgoferutils
 lib_name = qgoferutils
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = True
 doc_path = _docs
 lib_path = qgoferutils
 nbs_path = nbs
 recursive = True
```

### Comparing `qgoferutils-0.0.7/setup.py` & `qgoferutils-0.0.8/setup.py`

 * *Files identical despite different names*

