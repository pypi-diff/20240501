# Comparing `tmp/openstef_dbc-3.7.7.tar.gz` & `tmp/openstef_dbc-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.7.7.tar", last modified: Thu Apr  4 15:14:28 2024, max compression
+gzip compressed data, was "openstef_dbc-3.7.9.tar", last modified: Fri Apr 12 14:09:09 2024, max compression
```

## Comparing `openstef_dbc-3.7.7.tar` & `openstef_dbc-3.7.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.170999 openstef_dbc-3.7.7/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.170999 openstef_dbc-3.7.7/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.170999 openstef_dbc-3.7.7/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:09.428933 openstef_dbc-3.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-12 14:09:09.428933 openstef_dbc-3.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:09.424933 openstef_dbc-3.7.9/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:09.424933 openstef_dbc-3.7.9/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:09.424933 openstef_dbc-3.7.9/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:09.428933 openstef_dbc-3.7.9/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:09.428933 openstef_dbc-3.7.9/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-12 14:09:09.000000 openstef_dbc-3.7.9/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 14:09:09.000000 openstef_dbc-3.7.9/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:09:09.000000 openstef_dbc-3.7.9/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 14:09:09.000000 openstef_dbc-3.7.9/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 14:09:09.000000 openstef_dbc-3.7.9/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 14:09:09.428933 openstef_dbc-3.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-12 14:08:59.000000 openstef_dbc-3.7.9/setup.py
```

### Comparing `openstef_dbc-3.7.7/LICENSE` & `openstef_dbc-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/PKG-INFO` & `openstef_dbc-3.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.7.7
+Version: 3.7.9
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.7.7/README.md` & `openstef_dbc-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/__init__.py` & `openstef_dbc-3.7.9/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/data_interface.py` & `openstef_dbc-3.7.9/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/database.py` & `openstef_dbc-3.7.9/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/ktp_api.py` & `openstef_dbc-3.7.9/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/log/logging.py` & `openstef_dbc-3.7.9/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/log/processors.py` & `openstef_dbc-3.7.9/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/models/measurement.py` & `openstef_dbc-3.7.9/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/ems.py` & `openstef_dbc-3.7.9/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/model_input.py` & `openstef_dbc-3.7.9/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.7.9/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/predictions.py` & `openstef_dbc-3.7.9/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/predictor.py` & `openstef_dbc-3.7.9/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/splitting.py` & `openstef_dbc-3.7.9/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/systems.py` & `openstef_dbc-3.7.9/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/weather.py` & `openstef_dbc-3.7.9/openstef_dbc/services/weather.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,16 +161,17 @@
         Function that complete's the weatherdata from the influx database retrieved using get_weatherdata
         Additionally, weatherdata from several sources is combined to a single forecast.
         The preferred source_order is given as argument.
 
         Args:
             result (pd.DataFrame): return value from the function 'get_weatherdata'
             source_order (list): which weather models should be used (first).
-                Options: "OWM", "DSN", "WUN", "harmonie", "harm_arome", "optimum", "icon"
-                Default: '"harm_arome", "harmonie", "icon", "DSN"'. This combines harmonie, harm_arome, ICON and DSN,
+                Options: "OWM", "DSN", "WUN", "harmonie", "harm_arome", "harm_arome_fallback", "optimum", "icon"
+                Default: '"harm_arome", "harm_arome_fallback", "harmonie", "icon", "DSN"'.
+                This combines harmonie, harm_arome, harm_arome_fallback, ICON and DSN,
                 taking the (heuristicly) best available source for each moment in time
 
         Returns:
             pd.DataFrame: The most recent weather prediction of several sources combined into one dataframe
 
         Example:
             client = influxdb.DataFrameClient()
@@ -179,15 +180,22 @@
             print(df.head())
         """
         # Combine the multiple sources in the optimal way
         ####
         # step 1: Create list of multiple dataframes,
         # check which of the 'optimum' sources are actually in the list
         if source_order is None:
-            source_order = ["harm_arome", "GFS_50", "harmonie", "icon", "DSN"]
+            source_order = [
+                "harm_arome",
+                "harm_arome_fallback",
+                "GFS_50",
+                "harmonie",
+                "icon",
+                "DSN",
+            ]
 
         active_sources = [s for s in source_order if s in set(result.source)]
         # for each source a seperate dataframe
         df_list = [result[result.source == s] for s in active_sources]
 
         # Step two, combine the individual dataframe,
         # keeping data from the most-preferred datasource
@@ -218,15 +226,15 @@
             location (str): Location. Should be in the stored locations. e.g. Volkel
             weatherparams  (str or list of str): weatherparams that are required.
                 Params include: ["clouds", "radiation", "temp", "winddeg", "windspeed", "windspeed_100m", "pressure",
                 "humidity", "rain", 'mxlD', 'snowDepth', 'clearSky_ulf', 'clearSky_dlf', 'ssrunoff']
             datetime_start (datetime) : start date time. Default: 14 days ago
             datetime_end (datetime): end date time. Default: now + 2 days.
             source (str or list of str): which weather models should be used.
-                Options: "OWM", "DSN", "WUN", "harmonie", "harm_arome", "icon", "optimum",
+                Options: "OWM", "DSN", "WUN", "harmonie", "harm_arome", "harm_arome_fallback", "icon", "optimum",
                 Default: 'optimum'. This combines harmonie, harm_arome, icon and DSN,
                 taking the (heuristicly) best available source for each moment in time
             resolution (str): Time resolution of the returned data, default: "15T"
             country (str): Country code (2-letter: ISO 3166-1). e.g. NL
         Returns:
             pd.DataFrame: The most recent weather prediction
 
@@ -267,15 +275,22 @@
             source = [source]
         if isinstance(weatherparams, str):
             weatherparams = [weatherparams]
 
         # Try to get the data from influx.
         if "optimum" in source:
             # so the query return all
-            source = ["harm_arome", "GFS_50", "harmonie", "icon", "DSN"]
+            source = [
+                "harm_arome",
+                "harm_arome_fallback",
+                "GFS_50",
+                "harmonie",
+                "icon",
+                "DSN",
+            ]
             combine_sources = True
         else:
             combine_sources = False
 
         # Initialize binding params
         bind_params = {
             "_input_city": location_name,
```

### Comparing `openstef_dbc-3.7.7/openstef_dbc/services/write.py` & `openstef_dbc-3.7.9/openstef_dbc/services/write.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc/utils.py` & `openstef_dbc-3.7.9/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.7.9/openstef_dbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.7.7
+Version: 3.7.9
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.7.7/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.7.9/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.7/setup.py` & `openstef_dbc-3.7.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.7.7",
+    version="3.7.9",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

