# Comparing `tmp/gmnspy-0.3.3.tar.gz` & `tmp/gmnspy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmnspy-0.3.3.tar", last modified: Tue Feb  6 19:12:51 2024, max compression
+gzip compressed data, was "gmnspy-0.3.4.tar", last modified: Tue Apr 30 22:26:06 2024, max compression
```

## Comparing `gmnspy-0.3.3.tar` & `gmnspy-0.3.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.453755 gmnspy-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-02-06 19:12:43.000000 gmnspy-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-06 19:12:43.000000 gmnspy-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-02-06 19:12:51.453755 gmnspy-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-06 19:12:43.000000 gmnspy-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.445755 gmnspy-0.3.3/gmnspy/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/in_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.449755 gmnspy-0.3.3/gmnspy/spec/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/geometry.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/gmns.spec.json
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/lane.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/lane_tod.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/link.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/link_tod.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/location.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/movement.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/movement_tod.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/node.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/segment.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/segment_lane.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/segment_lane_tod.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/segment_tod.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/signal_controller.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/signal_coordination.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/signal_detector.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/signal_phase_mvmt.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/signal_timing_phase.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/signal_timing_plan.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/time_set_definitions.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/use_definition.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/use_group.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/spec/zone.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.449755 gmnspy-0.3.3/gmnspy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/utils/list_to_md_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/utils/set_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.449755 gmnspy-0.3.3/gmnspy/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/validation/constraint_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/validation/foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/validation/required_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/validation/resources_existance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-02-06 19:12:43.000000 gmnspy-0.3.3/gmnspy/validation/schema_to_df.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.453755 gmnspy-0.3.3/gmnspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-02-06 19:12:51.000000 gmnspy-0.3.3/gmnspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-06 19:12:51.000000 gmnspy-0.3.3/gmnspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 19:12:51.000000 gmnspy-0.3.3/gmnspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 19:12:51.000000 gmnspy-0.3.3/gmnspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-06 19:12:51.000000 gmnspy-0.3.3/gmnspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-06 19:12:43.000000 gmnspy-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-06 19:12:43.000000 gmnspy-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 19:12:51.453755 gmnspy-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.449755 gmnspy-0.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:12:51.453755 gmnspy-0.3.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-02-06 19:12:43.000000 gmnspy-0.3.3/tests/data/geometry.csv
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-06 19:12:43.000000 gmnspy-0.3.3/tests/data/link.csv
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-06 19:12:43.000000 gmnspy-0.3.3/tests/data/node.csv
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-06 19:12:43.000000 gmnspy-0.3.3/tests/data/use_definition.csv
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-06 19:12:43.000000 gmnspy-0.3.3/tests/data/use_group.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-06 19:12:43.000000 gmnspy-0.3.3/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-30 22:26:00.000000 gmnspy-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 22:26:00.000000 gmnspy-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-30 22:26:06.663453 gmnspy-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-30 22:26:00.000000 gmnspy-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.655453 gmnspy-0.3.4/gmnspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/in_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/gmnspy/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/geometry.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/gmns.spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/lane.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/lane_tod.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/link.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/link_tod.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/location.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/movement.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/movement_tod.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/node.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/segment.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/segment_lane.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/segment_lane_tod.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/segment_tod.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/signal_controller.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/signal_coordination.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/signal_detector.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/signal_phase_mvmt.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/signal_timing_phase.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/signal_timing_plan.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/time_set_definitions.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/use_definition.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/use_group.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/spec/zone.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/gmnspy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/utils/list_to_md_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/utils/set_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/gmnspy/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/validation/constraint_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/validation/foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/validation/required_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/validation/resources_existance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-30 22:26:00.000000 gmnspy-0.3.4/gmnspy/validation/schema_to_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/gmnspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-30 22:26:06.000000 gmnspy-0.3.4/gmnspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 22:26:06.000000 gmnspy-0.3.4/gmnspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:26:06.000000 gmnspy-0.3.4/gmnspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 22:26:06.000000 gmnspy-0.3.4/gmnspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 22:26:06.000000 gmnspy-0.3.4/gmnspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-30 22:26:00.000000 gmnspy-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 22:26:00.000000 gmnspy-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 22:26:06.663453 gmnspy-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:26:06.663453 gmnspy-0.3.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-30 22:26:00.000000 gmnspy-0.3.4/tests/data/geometry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 22:26:00.000000 gmnspy-0.3.4/tests/data/link.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 22:26:00.000000 gmnspy-0.3.4/tests/data/node.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 22:26:00.000000 gmnspy-0.3.4/tests/data/use_definition.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-30 22:26:00.000000 gmnspy-0.3.4/tests/data/use_group.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 22:26:00.000000 gmnspy-0.3.4/tests/test_basic.py
```

### Comparing `gmnspy-0.3.3/LICENSE` & `gmnspy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/PKG-INFO` & `gmnspy-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmnspy
-Version: 0.3.3
+Version: 0.3.4
 Project-URL: Source, https://github.com/e-lo/GMNSpy
 Project-URL: Homepage, https://e-lo.github.io/GMNSpy
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: frictionless
 Requires-Dist: pandas>=1.0
```

### Comparing `gmnspy-0.3.3/README.md` & `gmnspy-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/in_out.py` & `gmnspy-0.3.4/gmnspy/in_out.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/schema.py` & `gmnspy-0.3.4/gmnspy/schema.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/geometry.schema.json` & `gmnspy-0.3.4/gmnspy/spec/geometry.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/gmns.spec.json` & `gmnspy-0.3.4/gmnspy/spec/gmns.spec.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/lane.schema.json` & `gmnspy-0.3.4/gmnspy/spec/lane.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/lane_tod.schema.json` & `gmnspy-0.3.4/gmnspy/spec/lane_tod.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/link.schema.json` & `gmnspy-0.3.4/gmnspy/spec/link.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/link_tod.schema.json` & `gmnspy-0.3.4/gmnspy/spec/link_tod.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/location.schema.json` & `gmnspy-0.3.4/gmnspy/spec/location.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/movement.schema.json` & `gmnspy-0.3.4/gmnspy/spec/movement.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/movement_tod.schema.json` & `gmnspy-0.3.4/gmnspy/spec/movement_tod.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/node.schema.json` & `gmnspy-0.3.4/gmnspy/spec/node.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/segment.schema.json` & `gmnspy-0.3.4/gmnspy/spec/segment.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/segment_lane.schema.json` & `gmnspy-0.3.4/gmnspy/spec/segment_lane.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/segment_lane_tod.schema.json` & `gmnspy-0.3.4/gmnspy/spec/segment_lane_tod.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/segment_tod.schema.json` & `gmnspy-0.3.4/gmnspy/spec/segment_tod.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/signal_coordination.schema.json` & `gmnspy-0.3.4/gmnspy/spec/signal_coordination.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/signal_detector.schema.json` & `gmnspy-0.3.4/gmnspy/spec/signal_detector.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/signal_phase_mvmt.schema.json` & `gmnspy-0.3.4/gmnspy/spec/signal_phase_mvmt.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/signal_timing_phase.schema.json` & `gmnspy-0.3.4/gmnspy/spec/signal_timing_phase.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/signal_timing_plan.schema.json` & `gmnspy-0.3.4/gmnspy/spec/signal_timing_plan.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/time_set_definitions.schema.json` & `gmnspy-0.3.4/gmnspy/spec/time_set_definitions.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/use_definition.schema.json` & `gmnspy-0.3.4/gmnspy/spec/use_definition.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/use_group.schema.json` & `gmnspy-0.3.4/gmnspy/spec/use_group.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/spec/zone.schema.json` & `gmnspy-0.3.4/gmnspy/spec/zone.schema.json`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/utils/list_to_md_table.py` & `gmnspy-0.3.4/gmnspy/utils/list_to_md_table.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/utils/set_logger.py` & `gmnspy-0.3.4/gmnspy/utils/set_logger.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/validation/constraint_checking.py` & `gmnspy-0.3.4/gmnspy/validation/constraint_checking.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/validation/foreign_keys.py` & `gmnspy-0.3.4/gmnspy/validation/foreign_keys.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/validation/required_files.py` & `gmnspy-0.3.4/gmnspy/validation/required_files.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/validation/resources_existance.py` & `gmnspy-0.3.4/gmnspy/validation/resources_existance.py`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/gmnspy/validation/schema_to_df.py` & `gmnspy-0.3.4/gmnspy/validation/schema_to_df.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Returns:
         DataFrame with fields coerced to appropriate type and constraints
             and warnings evaluated.
     """
     if not schema_file:
         schema_filename = os.path.split(originating_file)[-1].split(".")[0] + ".schema.json"
         schema_file = join(join(dirname(realpath(__file__)), "../spec"), schema_filename)
-    logger.info("SCHEMA", schema_file)
+    logger.info("SCHEMA: {}".format(schema_file))
     logger.info("...validating {} against {}".format(df, schema_file))
     schema = read_schema(schema_file=schema_file)
 
     """
     1. Check field names and requirements
     - Required fields present (strict)
     - Extra fields that aren't in spec (warn)
```

### Comparing `gmnspy-0.3.3/gmnspy.egg-info/PKG-INFO` & `gmnspy-0.3.4/gmnspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmnspy
-Version: 0.3.3
+Version: 0.3.4
 Project-URL: Source, https://github.com/e-lo/GMNSpy
 Project-URL: Homepage, https://e-lo.github.io/GMNSpy
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: frictionless
 Requires-Dist: pandas>=1.0
```

### Comparing `gmnspy-0.3.3/gmnspy.egg-info/SOURCES.txt` & `gmnspy-0.3.4/gmnspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/pyproject.toml` & `gmnspy-0.3.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmnspy"
-version = "0.3.3"
+version = "0.3.4"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 dependencies = [
     "frictionless",
     "pandas>= 1.0"
 ]
 classifiers = [
```

### Comparing `gmnspy-0.3.3/tests/data/geometry.csv` & `gmnspy-0.3.4/tests/data/geometry.csv`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/tests/data/link.csv` & `gmnspy-0.3.4/tests/data/link.csv`

 * *Files identical despite different names*

### Comparing `gmnspy-0.3.3/tests/test_basic.py` & `gmnspy-0.3.4/tests/test_basic.py`

 * *Files identical despite different names*

