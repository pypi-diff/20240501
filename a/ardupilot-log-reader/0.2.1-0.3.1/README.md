# Comparing `tmp/ardupilot_log_reader-0.2.1.tar.gz` & `tmp/ardupilot_log_reader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardupilot_log_reader-0.2.1.tar", last modified: Thu Mar  7 13:23:36 2024, max compression
+gzip compressed data, was "ardupilot_log_reader-0.3.1.tar", last modified: Wed May  1 08:35:28 2024, max compression
```

## Comparing `ardupilot_log_reader-0.2.1.tar` & `ardupilot_log_reader-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-07 13:23:36.672870 ardupilot_log_reader-0.2.1/
--rw-r--r--   0 td6834    (1001) td6834    (1001)     1092 2024-03-07 13:23:36.672870 ardupilot_log_reader-0.2.1/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      718 2023-03-28 15:54:18.000000 ardupilot_log_reader-0.2.1/ReadMe.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-07 13:23:36.668870 ardupilot_log_reader-0.2.1/ardupilot_log_reader/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       29 2023-03-28 15:54:18.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6089 2024-02-25 15:59:57.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader/reader.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-07 13:23:36.672870 ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/
--rw-r--r--   0 td6834    (1001) td6834    (1001)     1092 2024-03-07 13:23:36.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      335 2024-03-07 13:23:36.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2024-03-07 13:23:36.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       30 2024-03-07 13:23:36.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       21 2024-03-07 13:23:36.000000 ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      455 2024-03-07 13:23:36.672870 ardupilot_log_reader-0.2.1/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      666 2023-03-28 15:54:18.000000 ardupilot_log_reader-0.2.1/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-07 13:23:36.672870 ardupilot_log_reader-0.2.1/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1642 2023-11-09 14:18:44.000000 ardupilot_log_reader-0.2.1/tests/test_ardupilot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:35:28.967401 ardupilot_log_reader-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-01 08:35:28.967401 ardupilot_log_reader-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-01 08:35:03.000000 ardupilot_log_reader-0.3.1/ReadMe.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:35:28.963401 ardupilot_log_reader-0.3.1/ardupilot_log_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 08:35:03.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-01 08:35:03.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:35:28.967401 ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-01 08:35:28.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-01 08:35:28.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:35:28.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 08:35:28.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 08:35:28.000000 ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 08:35:28.967401 ardupilot_log_reader-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-01 08:35:03.000000 ardupilot_log_reader-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:35:28.967401 ardupilot_log_reader-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-01 08:35:03.000000 ardupilot_log_reader-0.3.1/tests/test_ardupilot.py
```

### Comparing `ardupilot_log_reader-0.2.1/PKG-INFO` & `ardupilot_log_reader-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ardupilot_log_reader
-Version: 0.2.1
+Version: 0.3.1
 Summary: module to read ardupilot binary logs to memory
 Home-page: https://github.com/PyFlightCoach/ardupilot_log_reader
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
-Requires-Dist: future
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pymavlink
 
 # Ardupilot Log Reader
 
 This package wraps untidily around mavlogdump in pymavlink, to read an ardupilot log to a pandas dataframe.
@@ -18,14 +17,13 @@
 ## usage
 
 #set up the parser
 from ArdupilotLogReader import Ardupilot
 parser = Ardupilot(
     log_file, # the log file, .bin
     types = ['ARSP', 'ATT', 'BARO', 'GPS', 'IMU', 'RCIN', 'RCOU', 'BAT', 'MODE', 'NKF1', 'STAT', 'XKF1'],  # fields to read from the log
-    zero_time_base=True # arguments passed to pymavlink
     )
 
 parser.dfs # a dict containing a dataframes of log data for each field requested.
 parser.join_logs(['ARSP', 'ATT']) #returns a pandas dataframe containing the ARSP and ATT data joined on time
 parser.parms # returns the parameters read from the top of the log
```

### Comparing `ardupilot_log_reader-0.2.1/ReadMe.md` & `ardupilot_log_reader-0.3.1/ReadMe.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 ## usage
 
 #set up the parser
 from ArdupilotLogReader import Ardupilot
 parser = Ardupilot(
     log_file, # the log file, .bin
     types = ['ARSP', 'ATT', 'BARO', 'GPS', 'IMU', 'RCIN', 'RCOU', 'BAT', 'MODE', 'NKF1', 'STAT', 'XKF1'],  # fields to read from the log
-    zero_time_base=True # arguments passed to pymavlink
     )
 
 parser.dfs # a dict containing a dataframes of log data for each field requested.
 parser.join_logs(['ARSP', 'ATT']) #returns a pandas dataframe containing the ARSP and ATT data joined on time
 parser.parms # returns the parameters read from the top of the log
```

### Comparing `ardupilot_log_reader-0.2.1/ardupilot_log_reader.egg-info/PKG-INFO` & `ardupilot_log_reader-0.3.1/ardupilot_log_reader.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ardupilot_log_reader
-Version: 0.2.1
+Version: 0.3.1
 Summary: module to read ardupilot binary logs to memory
 Home-page: https://github.com/PyFlightCoach/ardupilot_log_reader
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
-Requires-Dist: future
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pymavlink
 
 # Ardupilot Log Reader
 
 This package wraps untidily around mavlogdump in pymavlink, to read an ardupilot log to a pandas dataframe.
@@ -18,14 +17,13 @@
 ## usage
 
 #set up the parser
 from ArdupilotLogReader import Ardupilot
 parser = Ardupilot(
     log_file, # the log file, .bin
     types = ['ARSP', 'ATT', 'BARO', 'GPS', 'IMU', 'RCIN', 'RCOU', 'BAT', 'MODE', 'NKF1', 'STAT', 'XKF1'],  # fields to read from the log
-    zero_time_base=True # arguments passed to pymavlink
     )
 
 parser.dfs # a dict containing a dataframes of log data for each field requested.
 parser.join_logs(['ARSP', 'ATT']) #returns a pandas dataframe containing the ARSP and ATT data joined on time
 parser.parms # returns the parameters read from the top of the log
```

### Comparing `ardupilot_log_reader-0.2.1/setup.py` & `ardupilot_log_reader-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ardupilot_log_reader-0.2.1/tests/test_ardupilot.py` & `ardupilot_log_reader-0.3.1/tests/test_ardupilot.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,46 +6,30 @@
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 from ardupilot_log_reader.reader import Ardupilot
-import numpy as np
-import pandas as pd
 
 import pytest
 
 
 @pytest.fixture(scope="session")
 def type_request():
     return ['XKF1', 'XKQ1', 'ARSP', 'GPS', 'RCIN', 'RCOU', 'IMU', 'BARO', 'MODE', 'RPM', 'MAG']
 
 @pytest.fixture(scope="session")
 def log(type_request):
-    return Ardupilot('tests/test_inputs/test_log_00000052.BIN', types=type_request, zero_time_base=True)
+    return Ardupilot.parse('tests/test_inputs/test_log_00000052.BIN', types=type_request, zero_time_base=True)
 
 @pytest.fixture(scope="session")
 def log2(type_request):
-    return Ardupilot('tests/test_inputs/00000129.BIN', types=type_request, zero_time_base=True)
-
+    return Ardupilot.parse('tests/test_inputs/00000129.BIN', types=type_request, zero_time_base=True)
 
 def test_dfs(type_request, log):
     assert set(log.dfs.keys()) == set(type_request + ['PARM'])
 
 
-def test_full_df_frequency(log, type_request):
-    fulldf = log.join_logs(type_request)
-    assert len(log.dfs['XKF1']) == len(fulldf)
-
-
-def test_time_epioch(log):
-    gpsdf = log.dfs['GPS']
-    assert "GPSTimeUS" in gpsdf.columns
-
-
-def test_time_index(log2):
-    assert "XKF1" in log2.dfs
-    assert log2.dfs["XKF1"].timestamp.is_monotonic_increasing
```

