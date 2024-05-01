# Comparing `tmp/trysts-0.0.1.tar.gz` & `tmp/trysts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trysts-0.0.1.tar", max compression
+gzip compressed data, was "trysts-0.0.2.tar", max compression
```

## Comparing `trysts-0.0.1.tar` & `trysts-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,26 @@
--rwxr-xr-x   0        0        0      459 2024-04-27 22:34:48.917264 trysts-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 trysts-0.0.1/readme.md
--rw-r--r--   0        0        0       36 2024-04-23 18:57:06.249310 trysts-0.0.1/venues/stages/trysts/__init__.py
--rw-r--r--   0        0        0       77 2024-03-23 20:03:57.719484 trysts-0.0.1/venues/stages/trysts/__itinerary/later.S.HTML
--rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 trysts-0.0.1/venues/stages/trysts/_licenses/gpl-3.0-standalone.html
--rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 trysts-0.0.1/venues/stages/trysts/_ops/_clique/__init__.py
--rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 trysts-0.0.1/venues/stages/trysts/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 trysts-0.0.1/venues/stages/trysts/_ops/_clique/group/__init__.py
--rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 trysts-0.0.1/venues/stages/trysts/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 trysts-0.0.1/venues/stages/trysts/_status/DB/records.json
--rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 trysts-0.0.1/venues/stages/trysts/_status/monitors/status_1.py
--rw-r--r--   0        0        0     1375 2024-04-09 23:13:50.708900 trysts-0.0.1/venues/stages/trysts/_status/status.proc.py
--rw-r--r--   0        0        0       58 2024-04-23 19:29:47.178916 trysts-0.0.1/venues/stages/trysts/adventures/stack.S.HTML
--rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 trysts-0.0.1/venues/stages/trysts/license.S.HTML
--rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 trysts-0.0.1/venues/stages/trysts/mixer.MD
--rw-r--r--   0        0        0      154 2024-03-23 19:57:06.959925 trysts-0.0.1/venues/stages/trysts/mixer.S.HTML
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 trysts-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      477 2024-05-01 01:54:08.822286 trysts-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 trysts-0.0.2/readme.md
+-rw-r--r--   0        0        0       36 2024-04-23 18:57:06.249310 trysts-0.0.2/venues/stages/trysts/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-28 16:30:06.063101 trysts-0.0.2/venues/stages/trysts/__objectives/OSM/OSM.S.HTML
+-rw-r--r--   0        0        0      582 2024-04-28 17:49:38.011024 trysts-0.0.2/venues/stages/trysts/__objectives/objectives.S.HTML
+-rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 trysts-0.0.2/venues/stages/trysts/_licenses/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 trysts-0.0.2/venues/stages/trysts/_ops/_clique/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 trysts-0.0.2/venues/stages/trysts/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 trysts-0.0.2/venues/stages/trysts/_ops/_clique/group/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 trysts-0.0.2/venues/stages/trysts/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 trysts-0.0.2/venues/stages/trysts/_status/DB/records.json
+-rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 trysts-0.0.2/venues/stages/trysts/_status/monitors/status_1.py
+-rw-r--r--   0        0        0     1375 2024-04-09 23:13:50.708900 trysts-0.0.2/venues/stages/trysts/_status/status.proc.py
+-rw-r--r--   0        0        0      228 2024-05-01 01:48:49.881968 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/assets/AboutView-B_a93Z7o.js
+-rw-r--r--   0        0        0       85 2024-05-01 01:48:49.881968 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/assets/AboutView-C6Dx7pxG.css
+-rw-r--r--   0        0        0    88911 2024-05-01 01:48:49.881968 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/assets/index-C7uNmA4t.js
+-rw-r--r--   0        0        0     4207 2024-05-01 01:48:49.881968 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/assets/index-DHqK1tyo.css
+-rw-r--r--   0        0        0      455 2024-05-01 01:48:49.881968 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/index.html
+-rwxr-xr-x   0        0        0     1435 2024-05-01 01:48:49.809969 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-01 01:48:49.809969 trysts-0.0.2/venues/stages/trysts/adventures/sanique/public/vite.svg
+-rw-r--r--   0        0        0       58 2024-04-23 19:29:47.178916 trysts-0.0.2/venues/stages/trysts/adventures/stack.S.HTML
+-rw-r--r--   0        0        0      100 2024-04-28 16:43:11.892387 trysts-0.0.2/venues/stages/trysts/besties/OSM/OSM.S.HTML
+-rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 trysts-0.0.2/venues/stages/trysts/license.S.HTML
+-rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 trysts-0.0.2/venues/stages/trysts/mixer.MD
+-rw-r--r--   0        0        0      160 2024-04-28 16:40:29.620947 trysts-0.0.2/venues/stages/trysts/mixer.S.HTML
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 trysts-0.0.2/PKG-INFO
```

### Comparing `trysts-0.0.1/venues/stages/trysts/_licenses/gpl-3.0-standalone.html` & `trysts-0.0.2/venues/stages/trysts/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `trysts-0.0.1/venues/stages/trysts/_status/DB/records.json` & `trysts-0.0.2/venues/stages/trysts/_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `trysts-0.0.1/venues/stages/trysts/_status/status.proc.py` & `trysts-0.0.2/venues/stages/trysts/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `trysts-0.0.1/PKG-INFO` & `trysts-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trysts
-Version: 0.0.1
+Version: 0.0.2
 Summary: Drawings of the trysts and fields.
 License: licensed
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

