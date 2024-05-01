# Comparing `tmp/jra-tools-0.0.8.tar.gz` & `tmp/jra-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jra-tools-0.0.8.tar", last modified: Tue Aug 22 05:12:28 2023, max compression
+gzip compressed data, was "jra-tools-0.0.9.tar", last modified: Thu Aug 24 11:16:18 2023, max compression
```

## Comparing `jra-tools-0.0.8.tar` & `jra-tools-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.603508 jra-tools-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-11 08:17:30.000000 jra-tools-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      498 2023-08-22 05:12:28.603508 jra-tools-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-11 08:17:30.000000 jra-tools-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      763 2023-08-22 05:12:28.603508 jra-tools-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.599508 jra-tools-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.599508 jra-tools-0.0.8/src/jra_tools/
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-11 08:17:30.000000 jra-tools-0.0.8/src/jra_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.603508 jra-tools-0.0.8/src/jra_tools/database/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 08:17:30.000000 jra-tools-0.0.8/src/jra_tools/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5008 2023-07-11 10:40:09.000000 jra-tools-0.0.8/src/jra_tools/database/bao_importer.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-08-21 07:29:11.000000 jra-tools-0.0.8/src/jra_tools/database/db_checker.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-08-22 04:41:28.000000 jra-tools-0.0.8/src/jra_tools/database/pred_race_updater.py
--rw-r--r--   0 root         (0) root         (0)     1738 2023-08-22 01:57:25.000000 jra-tools-0.0.8/src/jra_tools/database/schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.603508 jra-tools-0.0.8/src/jra_tools/machine_learning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 08:17:30.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-08-22 04:57:18.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/category_data.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-08-22 04:40:32.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/input_creator.py
--rw-r--r--   0 root         (0) root         (0)     6848 2023-07-11 08:17:30.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/jrdbdummies.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-08-22 04:41:54.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/kaisai_creator.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-08-22 04:42:26.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/label_creator.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-07-11 08:17:30.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/labelutil.py
--rw-r--r--   0 root         (0) root         (0)     4871 2023-08-22 05:05:56.000000 jra-tools-0.0.8/src/jra_tools/machine_learning/training_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.599508 jra-tools-0.0.8/src/jra_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      498 2023-08-22 05:12:28.000000 jra-tools-0.0.8/src/jra_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      864 2023-08-22 05:12:28.000000 jra-tools-0.0.8/src/jra_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-22 05:12:28.000000 jra-tools-0.0.8/src/jra_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-08-22 05:12:28.000000 jra-tools-0.0.8/src/jra_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-08-22 05:12:28.000000 jra-tools-0.0.8/src/jra_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 05:12:28.603508 jra-tools-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)      486 2023-08-22 01:57:25.000000 jra-tools-0.0.8/tests/test_integration_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-08-22 01:57:25.000000 jra-tools-0.0.8/tests/test_schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.324367 jra-tools-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-11 08:17:30.000000 jra-tools-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      498 2023-08-24 11:16:18.324367 jra-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-11 08:17:30.000000 jra-tools-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      763 2023-08-24 11:16:18.324367 jra-tools-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.320367 jra-tools-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.320367 jra-tools-0.0.9/src/jra_tools/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-08-24 11:11:29.000000 jra-tools-0.0.9/src/jra_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.324367 jra-tools-0.0.9/src/jra_tools/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 08:17:30.000000 jra-tools-0.0.9/src/jra_tools/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-07-11 10:40:09.000000 jra-tools-0.0.9/src/jra_tools/database/bao_importer.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-08-21 07:29:11.000000 jra-tools-0.0.9/src/jra_tools/database/db_checker.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-08-24 10:51:02.000000 jra-tools-0.0.9/src/jra_tools/database/predict_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3629 2023-08-24 11:06:56.000000 jra-tools-0.0.9/src/jra_tools/database/predict_race_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-08-22 01:57:25.000000 jra-tools-0.0.9/src/jra_tools/database/schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.324367 jra-tools-0.0.9/src/jra_tools/machine_learning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 08:17:30.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-08-22 04:57:18.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/category_data.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-08-22 04:40:32.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/input_creator.py
+-rw-r--r--   0 root         (0) root         (0)     6848 2023-07-11 08:17:30.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/jrdbdummies.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-08-22 04:41:54.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/kaisai_creator.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-08-22 04:42:26.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/label_creator.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-07-11 08:17:30.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/labelutil.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-08-24 10:34:58.000000 jra-tools-0.0.9/src/jra_tools/machine_learning/training_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.324367 jra-tools-0.0.9/src/jra_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      498 2023-08-24 11:16:18.000000 jra-tools-0.0.9/src/jra_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      909 2023-08-24 11:16:18.000000 jra-tools-0.0.9/src/jra_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-24 11:16:18.000000 jra-tools-0.0.9/src/jra_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-08-24 11:16:18.000000 jra-tools-0.0.9/src/jra_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-24 11:16:18.000000 jra-tools-0.0.9/src/jra_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-24 11:16:18.324367 jra-tools-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-08-22 01:57:25.000000 jra-tools-0.0.9/tests/test_integration_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-08-22 01:57:25.000000 jra-tools-0.0.9/tests/test_schedule.py
```

### Comparing `jra-tools-0.0.8/LICENSE` & `jra-tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/setup.cfg` & `jra-tools-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jra-tools
-version = 0.0.8
+version = 0.0.9
 author = Requrd
 author_email = requrd1989@gmail.com
 description = Data Analisys Tools for JRDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/astroripple/jra-tools
 project_urls =
```

### Comparing `jra-tools-0.0.8/src/jra_tools/database/bao_importer.py` & `jra-tools-0.0.9/src/jra_tools/database/bao_importer.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/database/schedule.py` & `jra-tools-0.0.9/src/jra_tools/database/schedule.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/category_data.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/category_data.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/input_creator.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/input_creator.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/jrdbdummies.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/jrdbdummies.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/kaisai_creator.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/kaisai_creator.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/label_creator.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/label_creator.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/labelutil.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/labelutil.py`

 * *Files identical despite different names*

### Comparing `jra-tools-0.0.8/src/jra_tools/machine_learning/training_tool.py` & `jra-tools-0.0.9/src/jra_tools/machine_learning/training_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import reduce
 from sklearn.preprocessing import StandardScaler
 from jrdb_model import KaisaiData, BangumiData, RacehorseData
 
 
 def createScoreDataMatrix(kaisais: List[KaisaiData]) -> np.ndarray:
     num_max_horse = 18
-    num_race = numberOfRaces(kaisais)
+    num_race = reduce(lambda x, y: x + len(y.races), kaisais, 0)
     num_score = numberOfScoreFeatures(kaisais[0])
     baseMatrix = np.zeros([num_race, num_max_horse, num_score])
     return _setScores(baseMatrix, kaisais)
 
 
 def _setScores(score_data: np.ndarray, kaisais: List[KaisaiData]) -> np.ndarray:
     w = 0
@@ -40,18 +40,14 @@
     for i in range(len(matrix)):
         ss = StandardScaler()
         ss.fit(matrix[i])
         sds[i] = ss.transform(matrix[i])
     return sds
 
 
-def numberOfRaces(kaisais: List[KaisaiData]) -> int:
-    return reduce(lambda x, y: x + len(y.races), kaisais)
-
-
 def numberOfScoreFeatures(kaisai: KaisaiData) -> int:
     dummyScores = _addKaisaiScores([], kaisai)
     dummyScores.append(kaisai.races[0].num_of_all_horse)
     dummyScores = _addHorseScores(dummyScores, kaisai.races[0].racehorses[0])
     return len(dummyScores)
```

### Comparing `jra-tools-0.0.8/src/jra_tools.egg-info/SOURCES.txt` & `jra-tools-0.0.9/src/jra_tools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 src/jra_tools.egg-info/SOURCES.txt
 src/jra_tools.egg-info/dependency_links.txt
 src/jra_tools.egg-info/requires.txt
 src/jra_tools.egg-info/top_level.txt
 src/jra_tools/database/__init__.py
 src/jra_tools/database/bao_importer.py
 src/jra_tools/database/db_checker.py
-src/jra_tools/database/pred_race_updater.py
+src/jra_tools/database/predict_factory.py
+src/jra_tools/database/predict_race_factory.py
 src/jra_tools/database/schedule.py
 src/jra_tools/machine_learning/__init__.py
 src/jra_tools/machine_learning/category_data.py
 src/jra_tools/machine_learning/input_creator.py
 src/jra_tools/machine_learning/jrdbdummies.py
 src/jra_tools/machine_learning/kaisai_creator.py
 src/jra_tools/machine_learning/label_creator.py
```

### Comparing `jra-tools-0.0.8/tests/test_schedule.py` & `jra-tools-0.0.9/tests/test_schedule.py`

 * *Files identical despite different names*

