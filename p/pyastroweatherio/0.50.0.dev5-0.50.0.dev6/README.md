# Comparing `tmp/pyastroweatherio-0.50.0.dev5.tar.gz` & `tmp/pyastroweatherio-0.50.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.0.dev5.tar", last modified: Sun Apr 28 14:49:35 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.0.dev6.tar", last modified: Wed May  1 08:15:55 2024, max compression
```

## Comparing `pyastroweatherio-0.50.0.dev5.tar` & `pyastroweatherio-0.50.0.dev6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-28 14:49:35.270906 pyastroweatherio-0.50.0.dev5/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev5/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-28 14:49:35.270906 pyastroweatherio-0.50.0.dev5/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev5/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-28 14:49:35.262906 pyastroweatherio-0.50.0.dev5/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    40224 2024-04-28 14:49:17.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4031 2024-04-28 09:17:08.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20104 2024-04-28 12:53:36.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    46495 2024-04-28 14:40:54.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-28 14:49:35.270906 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-28 14:49:35.000000 pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-28 14:49:35.274906 pyastroweatherio-0.50.0.dev5/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-04-28 14:49:04.000000 pyastroweatherio-0.50.0.dev5/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-01 08:15:55.139840 pyastroweatherio-0.50.0.dev6/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev6/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-01 08:15:55.135840 pyastroweatherio-0.50.0.dev6/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev6/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-01 08:15:55.131840 pyastroweatherio-0.50.0.dev6/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    40772 2024-05-01 08:14:51.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4142 2024-04-29 14:09:59.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20142 2024-04-29 10:03:52.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    42090 2024-04-29 14:59:50.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-01 08:15:55.135840 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-01 08:15:55.000000 pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-01 08:15:55.139840 pyastroweatherio-0.50.0.dev6/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-05-01 08:15:27.000000 pyastroweatherio-0.50.0.dev6/setup.py
```

### Comparing `pyastroweatherio-0.50.0.dev5/LICENSE` & `pyastroweatherio-0.50.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev5/PKG-INFO` & `pyastroweatherio-0.50.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev5
+Version: 0.50.0.dev6
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev5/README.md` & `pyastroweatherio-0.50.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev5/pyastroweatherio/client.py` & `pyastroweatherio-0.50.0.dev6/pyastroweatherio/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     WIND10M_RANGE,
     HOME_LATITUDE,
     HOME_LONGITUDE,
     STIMER_OUTPUT,
     FORECAST_TYPE_HOURLY,
     SEEING,
     TRANSPARENCY,
+    MAG_DEGRATION_MAX,
+    LIFTED_INDEX,
 )
 from pyastroweatherio.dataclasses import (
     ForecastData,
     LocationData,
     NightlyConditionsData,
     DSOUpTonight,
 )
@@ -67,15 +69,15 @@
         cloudcover_medium_weakening=DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING,
         cloudcover_low_weakening=DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING,
         seeing_weight=DEFAULT_CONDITION_SEEING_WEIGHT,
         transparency_weight=DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
         calm_weight=DEFAULT_CONDITION_CALM_WEIGHT,
         uptonight_path="/conf/www",
         test_datetime=None,
-        seven_timer=True,
+        experimental_features=False,
     ):
         self._session: ClientSession = session
         self._latitude = latitude
         self._longitude = longitude
         self._elevation = elevation
         self._timezone_info = timezone_info
         self._weather_data_seventimer = []
@@ -91,15 +93,15 @@
         self._cloudcover_medium_weakening = cloudcover_medium_weakening
         self._cloudcover_low_weakening = cloudcover_low_weakening
         self._seeing_weight = seeing_weight
         self._transparency_weight = transparency_weight
         self._calm_weight = calm_weight
         self._uptonight_path = uptonight_path
         self._test_datetime = test_datetime
-        self._seven_timer = seven_timer
+        self._experimental_features = experimental_features
 
         self._forecast_data = None
 
         self.req = session
 
         # Astro Routines
         self._astro_routines = AstronomicalRoutines(
@@ -201,19 +203,23 @@
                 cloud_cover=details_metno.get("cloud_area_fraction", -1),
                 altitude=self._elevation,
                 air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
             )
         else:
             transparency = TRANSPARENCY[details_seventimer["transparency"] - 1]
 
-        await self._astro_lifted_index.calculate_lifted_index(
-            temperature=details_metno.get("air_temperature", -1),
-            dew_point_temperature=details_metno.get("dew_point_temperature", -1),
-            altitude=self._elevation,
-        )
+        lifted_index = 0
+        if details_seventimer["lifted_index"] == -1 or details_seventimer["lifted_index"] == -9999:
+            lifted_index = await self._astro_lifted_index.calculate_lifted_index(
+                temperature=details_metno.get("air_temperature", -1),
+                dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                altitude=self._elevation,
+            )
+        else:
+            lifted_index = LIFTED_INDEX[details_seventimer["lifted_index"] - 1]
      
         item = {
             # seventimer_init is "init" of 7timer astro data
             "seventimer_init": seventimer_init,  # init
             # seventimer_timepoint is "timepoint" of 7timer astro data and defines the data for init + timepoint
             "seventimer_timepoint": details_seventimer["timepoint"],  # timepoint
             # Forecast_time is the actual datetime for the forecast data onwards in UTC
@@ -225,15 +231,15 @@
             "forecast_length": (len(self._weather_data_metno) - metno_index),
             # Location
             "latitude": self._latitude,
             "longitude": self._longitude,
             "elevation": self._elevation,
             "seeing": seeing,
             "transparency": transparency,
-            "lifted_index": details_seventimer["lifted_index"],
+            "lifted_index": lifted_index,
             # Calculate
             "sun_next_rising": await self._astro_routines.sun_next_rising_civil(),
             "sun_next_rising_nautical": await self._astro_routines.sun_next_rising_nautical(),
             "sun_next_rising_astro": await self._astro_routines.sun_next_rising_astro(),
             "sun_next_setting": await self._astro_routines.sun_next_setting_civil(),
             "sun_next_setting_nautical": await self._astro_routines.sun_next_setting_nautical(),
             "sun_next_setting_astro": await self._astro_routines.sun_next_setting_astro(),
@@ -379,17 +385,14 @@
             )
 
             item = {
                 "seventimer_init": init_ts,
                 "seventimer_timepoint": details_seventimer["timepoint"],
                 "forecast_time": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"),
                 "hour": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ").hour,  # forecast_time.hour % 24,
-                "seeing": details_seventimer["seeing"],
-                "transparency": details_seventimer["transparency"],
-                "lifted_index": details_seventimer["lifted_index"],
             }
 
             seeing = 0
             if details_seventimer["seeing"] == -1 or details_seventimer["seeing"] == -9999:
                 seeing = await self._astro_seeing.calculate_seeing_model6(
                     temperature=details_metno.get("air_temperature", -1),
                     humidity=details_metno.get("relative_humidity", -1),
@@ -412,30 +415,36 @@
                     cloud_cover=details_metno.get("cloud_area_fraction", -1),
                     altitude=self._elevation,
                     air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
                 )
             else:
                 transparency = TRANSPARENCY[details_seventimer["transparency"] - 1]
 
-            await self._astro_lifted_index.calculate_lifted_index(
-                temperature=details_metno.get("air_temperature", -1),
-                dew_point_temperature=details_metno.get("dew_point_temperature", -1),
-                altitude=self._elevation,
-            )
+            lifted_index = 0
+            if details_seventimer["lifted_index"] == -1 or details_seventimer["lifted_index"] == -9999:
+                lifted_index = await self._astro_lifted_index.calculate_lifted_index(
+                    temperature=details_metno.get("air_temperature", -1),
+                    dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                    altitude=self._elevation,
+                )
+            else:
+                lifted_index = LIFTED_INDEX[details_seventimer["lifted_index"] - 1]
+            
             
             item["cloudcover"] = details_metno.get("cloud_area_fraction", -1)
             item["cloud_area_fraction"] = details_metno.get("cloud_area_fraction", -1)
             item["cloud_area_fraction_high"] = details_metno.get("cloud_area_fraction_high", -1)
             item["cloud_area_fraction_medium"] = details_metno.get("cloud_area_fraction_medium", -1)
             item["cloud_area_fraction_low"] = details_metno.get("cloud_area_fraction_low", -1)
             item["fog_area_fraction"] = details_metno.get("fog_area_fraction", -1)
             item["rh2m"] = details_metno.get("relative_humidity", -1)
             item["wind_speed"] = details_metno.get("wind_speed", -1)
             item["seeing"] = seeing
             item["transparency"] = transparency
+            item["lifted_index"] = lifted_index
             item["condition_percentage"] = await self.calc_condition_percentage(
                 item["cloud_area_fraction_high"],
                 item["cloud_area_fraction_medium"],
                 item["cloud_area_fraction_low"],
                 seeing,
                 transparency,
                 item["wind_speed"],
@@ -447,15 +456,15 @@
             if self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}) == {}:
                 # No more hourly data
                 _LOGGER.debug("No more hourly data at %s", self._weather_data_metno[metno_index].get("time", {}))
                 break
             if self._weather_data_metno[metno_index].get("data", {}).get("next_6_hours", {}) == {}:
                 # No more 6-hourly data
                 _LOGGER.debug("No more 6-hourly data at %s", self._weather_data_metno[metno_index].get("time", {}))
-                # break
+                break
             item["weather"] = (
                 self._weather_data_metno[metno_index]
                 .get("data", {})
                 .get("next_1_hours", {})
                 .get("summary", {})
                 .get("symbol_code", "")
             )
@@ -609,15 +618,15 @@
         self, cloudcover_high, cloudcover_medium, cloudcover_low, seeing, transparency, wind_speed
     ):
         """Return condition based on cloud cover, seeing, transparency, and wind speed"""
 
         # Seeing is something in between 0 and 2.5 arcsecs
         seeing = int(seeing * 40)  # arcsecs up to 2.5
         # transparency = int(transparency * 40)  # mag degration up to 2.5
-        transparency = int(transparency * 100)  # mag degration up to 1
+        transparency = int(transparency * 100 / MAG_DEGRATION_MAX)  # mag degration up to 1
         # Wind speed is something in between 0 and 16.5 m/s
         if wind_speed > 16.5:
             wind_speed = 16.5
         wind_speed_value = int(wind_speed * (100 / 16.5))  # m/s up to 16.5
 
         cloudcover = []
         cloudcover.append(cloudcover_high * self._cloudcover_high_weakening)
@@ -640,26 +649,26 @@
         #         + self._seeing_weight * (100 - seeing)
         #         + self._transparency_weight * (100 - transparency)
         #         + self._calm_weight * (100 - wind_speed_value)
         #     )
         #     / (self._cloudcover_weight + self._seeing_weight + self._transparency_weight + self._calm_weight)
         # )
 
-        _LOGGER.debug(
-            "Cloudcover: %s %s, Seeing: %s %s, Transparency: %s %s, Calmness: %s %s, Conditions: %s",
-            str(cloudcover),
-            str(self._cloudcover_weight),
-            str(seeing),
-            str(self._seeing_weight),
-            str(transparency),
-            str(self._transparency_weight),
-            str(wind_speed_value),
-            str(self._calm_weight),
-            condition,
-        )
+        # _LOGGER.debug(
+        #     "Cloudcover: %s %s, Seeing: %s %s, Transparency: %s %s, Calmness: %s %s, Conditions: %s",
+        #     str(cloudcover),
+        #     str(self._cloudcover_weight),
+        #     str(seeing),
+        #     str(self._seeing_weight),
+        #     str(transparency),
+        #     str(self._transparency_weight),
+        #     str(wind_speed_value),
+        #     str(self._calm_weight),
+        #     condition,
+        # )
 
         return condition
 
     async def _get_deepsky_objects(self):
         """Return Deepsky Objects for today"""
 
         items = []
@@ -702,44 +711,44 @@
         if ((datetime.now() - self._weather_data_seventimer_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
             self._weather_data_seventimer_timestamp = datetime.now()
             _LOGGER.debug("Updating data from 7Timer")
 
             astro_dataseries = {}
 
             # Testing
-            if self._seven_timer:
+            if not self._experimental_features:
                 if self._test_mode:
                     if os.path.isfile("debug/astro.json"):
                         _LOGGER.debug("Reading 7Timer from file")
                         with open("debug/astro.json") as json_file:
                             astro_dataseries_json = json.load(json_file)
                             astro_dataseries = astro_dataseries_json.get("dataseries", {})
                             json_data_astro = {"init": astro_dataseries_json.get("init")}
                     else:
                         json_data_astro = await self.async_request_seventimer("astro", "get")
                         astro_dataseries = json_data_astro.get("dataseries", {})
                 else:
                     json_data_astro = await self.async_request_seventimer("astro", "get")
                     astro_dataseries = json_data_astro.get("dataseries", {})
 
-            if astro_dataseries != {} and self._seven_timer:
+            if astro_dataseries != {} and not self._experimental_features:
                 self._weather_data_seventimer = astro_dataseries
                 self._weather_data_seventimer_init = json_data_astro.get("init")
             else:
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
                 # TODO: Think about a complete redesign of the calculations and potentially
                 #       make met.no the leading source instead of 7timer
                 # TODO: Eventually calculate seeing?
                 self._weather_data_seventimer = []
                 for index in range(0, 20):
                     self._weather_data_seventimer.append(
                         {"timepoint": index * 3, "seeing": -1, "transparency": -1, "lifted_index": -1}
                     )
-                self._weather_data_seventimer_init = datetime.now().strftime("%Y%m%d%H")
+                self._weather_data_seventimer_init = datetime.now(timezone.utc).replace(tzinfo=None).strftime("%Y%m%d%H")
         else:
             _LOGGER.debug("Using cached data for 7Timer")
 
     async def async_request_seventimer(self, product="astro", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
@@ -872,15 +881,15 @@
         if ((datetime.now() - self._data_uptonight_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
             self._data_uptonight_timestamp = datetime.now()
             _LOGGER.debug("Updating data from uptonight")
 
             dataseries = None
 
             if os.path.isfile(self._uptonight_path + "/uptonight-report.json"):
-                _LOGGER.debug(f"Uptonight report found")
+                # _LOGGER.debug(f"Uptonight report found")
                 with open(self._uptonight_path + "/uptonight-report.json") as json_file:
                     dataseries = json.load(json_file)
                     _LOGGER.debug(f"Uptonight imported")
             else:
                 _LOGGER.debug(
                     f"uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json"
                 )
```

### Comparing `pyastroweatherio-0.50.0.dev5/pyastroweatherio/const.py` & `pyastroweatherio-0.50.0.dev6/pyastroweatherio/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,36 +54,38 @@
 #     '1.5 to 2"',
 #     '2 to 2.5"',
 #     'Over 2.5"',
 # ]
 
 SEEING = [0.25, 0.625, 0.875, 1.125, 1.375, 1.75, 2.25, 2.5]
 TRANSPARENCY = [0.15, 0.35, 0.45, 0.55, 0.65, 0.775, 0.925, 1]
+MAG_DEGRATION_MAX = 1
+LIFTED_INDEX = [-7, -6, -4, -1.5, 2, 6, 9.5, 11]
 
-TRANSPARENCY_PLAIN = [
-    "Below 0.3 mag",
-    "0.3 to 0.4 mag",
-    "0.4 to 0.5 mag",
-    "0.5 to 0.6 mag",
-    "0.6 to 0.7 mag",
-    "0.7 to 0.85 mag",
-    "0.85 to 1 mag",
-    "Over 1 mag",
-]
+# TRANSPARENCY_PLAIN = [
+#     "Below 0.3 mag",
+#     "0.3 to 0.4 mag",
+#     "0.4 to 0.5 mag",
+#     "0.5 to 0.6 mag",
+#     "0.6 to 0.7 mag",
+#     "0.7 to 0.85 mag",
+#     "0.85 to 1 mag",
+#     "Over 1 mag",
+# ]
 
-LIFTED_INDEX_PLAIN = [
-    "Below -7, very unstable",
-    "-7 to -5, very unstable",
-    "-5 to -3, unstable",
-    "-3 to 0, slightly unstable",
-    "0 to 4, stable",
-    "4 to 8, stable",
-    "8 to 11, very stable",
-    "Over 11, very stable",
-]
+# LIFTED_INDEX_PLAIN = [
+#     "Below -7, very unstable",
+#     "-7 to -5, very unstable",
+#     "-5 to -3, unstable",
+#     "-3 to 0, slightly unstable",
+#     "0 to 4, stable",
+#     "4 to 8, stable",
+#     "8 to 11, very stable",
+#     "Over 11, very stable",
+# ]
 
 WIND10M_DIRECTON = ["N", "NE", "E", "SE", "S", "SW", "W", "NW"]
 
 # Wind
 # 0 --- Calm            less than 1 mph (0 m/s)      Smoke rises vertically
 # 1 --- Light air       1 - 3 mph     0.5-1.5 m/s    Smoke drifts with air, weather vanes inactive
 # 2 --- Light breeze    4 - 7 mph     2-3 m/s        Weather vanes active, wind felt on face, leaves rustle
```

### Comparing `pyastroweatherio-0.50.0.dev5/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.0.dev6/pyastroweatherio/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import math
 
 from pyastroweatherio.const import (
     # CLOUDCOVER_PLAIN,
     CONDITION,
     CONDITION_PLAIN,
     DEEP_SKY_THRESHOLD,
-    LIFTED_INDEX_PLAIN,
+    # LIFTED_INDEX_PLAIN,
     # SEEING_PLAIN,
-    TRANSPARENCY_PLAIN,
+    # TRANSPARENCY_PLAIN,
     WIND10M_PLAIN,
     WIND10M_DIRECTON,
     WIND10M_VALUE,
     WIND10M_RANGE,
 )
 
 
@@ -274,32 +274,32 @@
             if start <= wind10m_speed <= end:
                 wind_speed_value = derate
 
         if wind_speed_value >= 1 and wind_speed_value <= 8:
             return WIND10M_PLAIN[wind_speed_value - 1]
         return None
 
-    @property
-    def lifted_index_plain(self) -> str:
-        """Return Lifted Index."""
+    # @property
+    # def lifted_index_plain(self) -> str:
+    #     """Return Lifted Index."""
 
-        trans = {
-            -10: LIFTED_INDEX_PLAIN[0],
-            -6: LIFTED_INDEX_PLAIN[1],
-            -4: LIFTED_INDEX_PLAIN[2],
-            -1: LIFTED_INDEX_PLAIN[3],
-            2: LIFTED_INDEX_PLAIN[4],
-            6: LIFTED_INDEX_PLAIN[5],
-            10: LIFTED_INDEX_PLAIN[6],
-            15: LIFTED_INDEX_PLAIN[7],
-        }
-        lifted_index = self._lifted_index
-        if lifted_index in trans:
-            return trans.get(self._lifted_index, "")
-        return None
+    #     trans = {
+    #         -10: LIFTED_INDEX_PLAIN[0],
+    #         -6: LIFTED_INDEX_PLAIN[1],
+    #         -4: LIFTED_INDEX_PLAIN[2],
+    #         -1: LIFTED_INDEX_PLAIN[3],
+    #         2: LIFTED_INDEX_PLAIN[4],
+    #         6: LIFTED_INDEX_PLAIN[5],
+    #         10: LIFTED_INDEX_PLAIN[6],
+    #         15: LIFTED_INDEX_PLAIN[7],
+    #     }
+    #     lifted_index = self._lifted_index
+    #     if lifted_index in trans:
+    #         return trans.get(self._lifted_index, "")
+    #     return None
 
     @property
     def deep_sky_view(self) -> bool:
         """Return True if Deep Sky should be possible."""
         if self.condition_percentage >= DEEP_SKY_THRESHOLD:
             return True
         return False
```

### Comparing `pyastroweatherio-0.50.0.dev5/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.0.dev6/pyastroweatherio/helper_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     NAUTICAL_TWILIGHT,
     NAUTICAL_DUSK_DAWN,
     ASTRONOMICAL_TWILIGHT,
     ASTRONOMICAL_DUSK_DAWN,
     MAGNUS_COEFFICIENT_A,
     MAGNUS_COEFFICIENT_B,
     CONSTANT_C,
+    MAG_DEGRATION_MAX,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ConversionFunctions:
     """Convert between different Weather Units."""
@@ -65,15 +66,15 @@
 
         # Calculate temperature at lifting condensation level (LCL)
         temperature_LCL = dew_point_temperature - ((altitude / 1000) * lapse_rate)
 
         # Calculate lifted index
         lifted_index = temperature - temperature_LCL
 
-        print("Estimated Atmospheric Lifted Index: {:.2f}".format(lifted_index))
+        # print("Estimated Atmospheric Lifted Index: {:.2f}".format(lifted_index))
         return lifted_index
 
 
 class AstronomicalTransparency:
     """Calculate astronomical transparency"""
 
     # Write a python3 program to calculate atmospheric transparence based on humidity, temperature, clouds, wind, altitude, dew_point_temperature, and air_pressure_at_sea_level and convert the transparency to magnitude degradation
@@ -88,16 +89,16 @@
         # Wind speed in meters per second
         # Altitude in meters
         # Dew point temperature in Celsius
         # Air pressure at sea level in hPa
 
     def calculate_transparency(self, humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level):
         # Coefficients for the linear model (you can adjust these based on your requirements)
-        humidity_coefficient = 0.02
-        temperature_coefficient = 0.03
+        humidity_coefficient = 0.02  # 0.02
+        temperature_coefficient = 0.03  #0.03
         cloud_cover_coefficient = -0.1
         wind_speed_coefficient = -0.05
         altitude_coefficient = -0.01
         dew_point_temperature_coefficient = 0.02
         air_pressure_coefficient = 0.01
 
         # Calculate transparency using the linear model
@@ -105,15 +106,15 @@
                         (temperature * temperature_coefficient) +
                         (cloud_cover * cloud_cover_coefficient / 100) +
                         (wind_speed * wind_speed_coefficient) +
                         # (altitude * altitude_coefficient) +
                         # (air_pressure_at_sea_level * air_pressure_coefficient) +
                         (dew_point_temperature * dew_point_temperature_coefficient))
 
-        print(humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level, ":", transparency)
+        # print(humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level, ":", transparency)
         # Ensure transparency is within the valid range [0, 1]
         transparency = max(0, min(1, transparency))
 
         return transparency
 
     def transparency_to_magnitude_degradation(self, transparency):
 
@@ -123,31 +124,31 @@
         #     magnitude_degradation = -2.5 * math.log10(transparency)
         #     magnitude_degradation = max(0, min(2.5, magnitude_degradation))
 
         #     return magnitude_degradation
 
         # 7Timer
         if transparency == 0:
-            return float(1)  #float('inf')
+            return float(MAG_DEGRATION_MAX)  #float('inf')
         else:
-            magnitude_degradation = -1 * math.log10(transparency)
-            magnitude_degradation = max(0, min(1, magnitude_degradation))
+            magnitude_degradation = -2.5 * math.log10(transparency)
+            magnitude_degradation = max(0, min(MAG_DEGRATION_MAX, magnitude_degradation))
 
             return magnitude_degradation
 
     async def calculate_transparency_model(self, humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level):
 
         # Calculate transparency
         transparency = self.calculate_transparency(humidity, temperature, cloud_cover, wind_speed, altitude, dew_point_temperature, air_pressure_at_sea_level)
 
         # Convert transparency to magnitude degradation
         magnitude_degradation = self.transparency_to_magnitude_degradation(transparency)
 
-        print("Estimated Atmospheric Transparency: {:.2f}".format(transparency))
-        print("Magnitude Degradation: {:.2f}".format(magnitude_degradation))
+        # print("Estimated Atmospheric Transparency: {:.2f}".format(transparency))
+        # print("Magnitude Degradation: {:.2f}".format(magnitude_degradation))
         
         return magnitude_degradation
 
 
 class AstronomicalSeeing:
     """Calculate astronomical seeing"""
 
@@ -157,167 +158,37 @@
         _LOGGER.debug("AstronomicalSeeing calculation mode active")
         # temperature = 15  # in Celsius
         # wind_speed = 5  # in m/s
         # humidity = 50  # in Percent
         # aerosol_density = 0.1  # in kg/m^3
         # altitude = 1000  # in Meters
 
-    # Modell 0: Simple linear Model
-    async def calculate_seeing_model0(self, temperature, wind_speed, humidity, altitude):
-        constant_1 = 0.314 * temperature / 273
-        constant_2 = 20.8 * (1 - math.exp(-0.0695 * humidity))
-        constant_3 = 0.0017 * wind_speed**1.5
-        seeing = constant_1 + constant_2 + constant_3
-
-        _LOGGER.debug(
-            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
-            str(temperature),
-            str(wind_speed),
-            str(humidity),
-            str(altitude),
-            str(seeing),
-        )
-
-        if seeing > 2.5:
-            _LOGGER.debug('AstronomicalSeeing above 2.5"')
-            seeing = 2.5
-
-        return seeing
-
-    # Modell 1: Simple linear Model
-    async def calculate_seeing_model1(self, temperature, wind_speed, humidity, altitude):
-        seeing = 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity  # - 0.05 * altitude
-
-        _LOGGER.debug(
-            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
-            str(temperature),
-            str(wind_speed),
-            str(humidity),
-            str(altitude),
-            str(seeing),
-        )
-
-        if seeing > 2.5:
-            _LOGGER.debug('AstronomicalSeeing above 2.5"')
-            seeing = 2.5
-
-        return seeing
-
-    # Modell 2: Modell with Exponential functions
-    async def calculate_seeing_model2(self, temperature, wind_speed, humidity, altitude):
-        seeing = 0.05 * temperature + 0.1 * wind_speed**1.5 + 0.02 * humidity**2 - 0.03 * altitude**1.5
-
-        _LOGGER.debug(
-            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
-            str(temperature),
-            str(wind_speed),
-            str(humidity),
-            str(altitude),
-            str(seeing),
-        )
-
-        if seeing > 2.5:
-            _LOGGER.debug('AstronomicalSeeing above 2.5"')
-            seeing = 2.5
-
-        return seeing
-
-    # Modell 3: Modell based on empirical Data
-    async def calculate_seeing_model3(self, temperature, wind_speed, humidity, altitude):
-        seeing = 0.08 * temperature + 0.15 * math.log(wind_speed + 1) + 0.03 * humidity - 0.02 * altitude
-
-        _LOGGER.debug(
-            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
-            str(temperature),
-            str(wind_speed),
-            str(humidity),
-            str(altitude),
-            str(seeing),
-        )
-
-        if seeing > 2.5:
-            _LOGGER.debug('AstronomicalSeeing above 2.5"')
-            seeing = 2.5
-
-        return seeing
-
     # Modell 4:
     # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
     # and altitude above sea level. The seeing factor is then used to calculate the astronomical
     # seeing in arcseconds. The empirical relationship used here states that the seeing in arcseconds
     # is approximately equal to the reciprocal of the seeing factor multiplied by a conversion
     # factor of 0.98.
-    def calculate_dew_point(self, temperature, humidity):
-        alpha = math.log(humidity / 100) + (MAGNUS_COEFFICIENT_A * temperature) / (MAGNUS_COEFFICIENT_B + temperature)
-        dew_point = (MAGNUS_COEFFICIENT_B * alpha) / (MAGNUS_COEFFICIENT_A - alpha)
+    # def calculate_dew_point(self, temperature, humidity):
+    #     alpha = math.log(humidity / 100) + (MAGNUS_COEFFICIENT_A * temperature) / (MAGNUS_COEFFICIENT_B + temperature)
+    #     dew_point = (MAGNUS_COEFFICIENT_B * alpha) / (MAGNUS_COEFFICIENT_A - alpha)
 
-        return dew_point
+    #     return dew_point
 
     def calculate_saturation_vapor_pressure(self, dew_point):
         es = 6.11 * (10 ** (7.5 * dew_point / (237.7 + dew_point)))
 
         return es
 
-    def calculate_water_vapor_pressure(self, temperature, humidity):
-        dew_point = self.calculate_dew_point(temperature, humidity)
-        es = self.calculate_saturation_vapor_pressure(dew_point)
-        water_vapor_pressure = (humidity / 100) * es
-
-        return water_vapor_pressure
-
-    async def calculate_seeing_model4(self, temperature, humidity, wind_speed, altitude):
-        water_vapor_pressure = self.calculate_water_vapor_pressure(temperature, humidity)
-
-        adjusted_pressure = 1013.25 * math.exp(-0.00012 * altitude)
-        relative_pressure = adjusted_pressure / 1013.25
-
-        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.25 * (wind_speed / 10) ** 0.75 * relative_pressure
-        seeing = 0.98 / seeing_factor
-
-        _LOGGER.debug(
-            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
-            str(temperature),
-            str(wind_speed),
-            str(humidity),
-            str(altitude),
-            str(seeing),
-        )
-
-        if seeing > 2.5:
-            seeing = 2.5
-
-        return seeing
-
-    # Modell 5:
-    # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
-    # and altitude above sea level. It is similar to Model 4 but uses the air pressure at sea level
-    # provided by Met.no.
-    async def calculate_seeing_model5(self, temperature, humidity, wind_speed, altitude, air_pressure_at_sea_level):
-        water_vapor_pressure = self.calculate_water_vapor_pressure(temperature, humidity)
-
-        adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
-        relative_pressure = adjusted_pressure / air_pressure_at_sea_level
+    # def calculate_water_vapor_pressure(self, temperature, humidity):
+    #     dew_point = self.calculate_dew_point(temperature, humidity)
+    #     es = self.calculate_saturation_vapor_pressure(dew_point)
+    #     water_vapor_pressure = (humidity / 100) * es
 
-        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.25 * (wind_speed / 10) ** 0.75 * relative_pressure
-        seeing = 0.98 / seeing_factor
-
-        _LOGGER.debug(
-            "AstronomicalSeeing calculation model5: T %s, W %s, H %s, E %s, P %s - S %s",
-            str(temperature),
-            str(wind_speed),
-            str(humidity),
-            str(altitude),
-            str(air_pressure_at_sea_level),
-            str(seeing),
-        )
-
-        if seeing > 2.5:
-            seeing = 2.5
-
-        return seeing
+    #     return water_vapor_pressure
 
     def calculate_water_vapor_pressure6(self, dew_point_temperature, humidity):
         dew_point = dew_point_temperature
         es = self.calculate_saturation_vapor_pressure(dew_point)
         water_vapor_pressure = (humidity / 100) * es
 
         return water_vapor_pressure
@@ -334,21 +205,23 @@
         adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
         seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.35 * (wind_speed / 10) ** 0.65 * relative_pressure
         seeing = 0.98 / seeing_factor
 
         _LOGGER.debug(
-            "AstronomicalSeeing calculation model6: T %s, H %s, DP %s, W %s, E %s, P %s - S %s",
+            "AstronomicalSeeing calculation model6: T %s, H %s, DP %s, W %s, E %s, P %s - wvp %s rp %s - S %s",
             str(temperature),
             str(humidity),
             str(dew_point_temperature),
             str(wind_speed),
             str(altitude),
             str(air_pressure_at_sea_level),
+            str(water_vapor_pressure),
+            str(relative_pressure),
             str(seeing),
         )
 
         if seeing > 2.5:
             seeing = 2.5  # max out seeing
 
         return seeing
@@ -1105,16 +978,14 @@
             return True
         return False
 
     async def deep_sky_darkness(self) -> float:
         """Returns the remaining timespan of deep sky darkness"""
         dsd = timedelta(0)
 
-        _LOGGER.debug(f"DSD - Calculating")
-
         if self.astronomical_darkness():
             _LOGGER.debug(f"DSD - In astronomical darkness")
             if await self.deep_sky_darkness_moon_rises():
                 dsd = self._moon_next_rising - self._forecast_time
                 _LOGGER.debug(f"DSD - Sun down, Moon rises {dsd}")
 
             if await self.deep_sky_darkness_moon_sets():
```

### Comparing `pyastroweatherio-0.50.0.dev5/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.0.dev6/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev5
+Version: 0.50.0.dev6
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev5/setup.py` & `pyastroweatherio-0.50.0.dev6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.0.dev5",
+    version="0.50.0.dev6",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

