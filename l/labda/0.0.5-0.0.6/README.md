# Comparing `tmp/labda-0.0.5.tar.gz` & `tmp/labda-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labda-0.0.5.tar", max compression
+gzip compressed data, was "labda-0.0.6.tar", max compression
```

## Comparing `labda-0.0.5.tar` & `labda-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0      548 2024-04-16 15:00:43.660729 labda-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      570 2024-04-16 15:00:43.660729 labda-0.0.5/README.md
--rw-r--r--   0        0        0      151 2024-04-16 15:00:43.680729 labda-0.0.5/labda/__init__.py
--rw-r--r--   0        0        0      142 2024-04-16 15:00:43.680729 labda-0.0.5/labda/assets/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-20 09:53:19.784358 labda-0.0.5/labda/assets/counts_cut_points.py
--rw-r--r--   0        0        0      459 2024-04-16 15:00:43.680729 labda-0.0.5/labda/assets/transportation_cut_points.py
--rw-r--r--   0        0        0      152 2024-04-16 15:00:43.680729 labda-0.0.5/labda/expanders/__init__.py
--rw-r--r--   0        0        0      656 2024-04-16 15:00:43.680729 labda-0.0.5/labda/expanders/accelerometer.py
--rw-r--r--   0        0        0      964 2024-04-16 15:00:43.680729 labda-0.0.5/labda/expanders/extras.py
--rw-r--r--   0        0        0     7377 2024-04-16 15:00:43.680729 labda-0.0.5/labda/expanders/spatial.py
--rw-r--r--   0        0        0     1150 2024-04-21 13:40:22.346206 labda-0.0.5/labda/logging.py
--rw-r--r--   0        0        0     1073 2024-04-16 15:00:43.680729 labda-0.0.5/labda/parallel.py
--rw-r--r--   0        0        0      201 2024-04-21 13:06:17.646205 labda-0.0.5/labda/parsers/__init__.py
--rw-r--r--   0        0        0     6854 2024-04-16 15:00:43.680729 labda-0.0.5/labda/parsers/actigraph.py
--rw-r--r--   0        0        0      930 2024-04-16 15:00:43.680729 labda-0.0.5/labda/parsers/bulk.py
--rw-r--r--   0        0        0     6508 2024-04-16 15:00:43.680729 labda-0.0.5/labda/parsers/gadgetbridge.py
--rw-r--r--   0        0        0     2332 2024-04-16 15:00:43.680729 labda-0.0.5/labda/parsers/garmin.py
--rw-r--r--   0        0        0    10928 2024-04-20 19:56:16.098319 labda-0.0.5/labda/parsers/qstarz.py
--rw-r--r--   0        0        0     5246 2024-04-21 14:00:33.876205 labda-0.0.5/labda/parsers/sens.py
--rw-r--r--   0        0        0     4975 2024-04-21 13:34:56.546207 labda-0.0.5/labda/parsers/traccar.py
--rw-r--r--   0        0        0     1737 2024-04-20 17:10:08.365165 labda-0.0.5/labda/parsers/utils.py
--rw-r--r--   0        0        0       36 2024-04-16 15:00:43.680729 labda-0.0.5/labda/processing/__init__.py
--rw-r--r--   0        0        0       88 2024-04-16 15:00:43.680729 labda-0.0.5/labda/processing/accelerometer/__init__.py
--rw-r--r--   0        0        0     1580 2024-04-16 15:00:43.680729 labda-0.0.5/labda/processing/accelerometer/activity_intensity.py
--rw-r--r--   0        0        0      616 2024-04-16 15:00:43.680729 labda-0.0.5/labda/processing/accelerometer/steps.py
--rw-r--r--   0        0        0      913 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/accelerometer/wear.py
--rw-r--r--   0        0        0     2803 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/bouts.py
--rw-r--r--   0        0        0      860 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/domains.py
--rw-r--r--   0        0        0      488 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/manipulations.py
--rw-r--r--   0        0        0      197 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/spatial/__init__.py
--rw-r--r--   0        0        0     6142 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/spatial/manipulations.py
--rw-r--r--   0        0        0     3277 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/spatial/timeline.py
--rw-r--r--   0        0        0     3771 2024-04-20 11:46:40.994360 labda-0.0.5/labda/processing/spatial/transportation.py
--rw-r--r--   0        0        0    25960 2024-04-21 17:06:22.915719 labda-0.0.5/labda/processing/spatial/trips.py
--rw-r--r--   0        0        0     2247 2024-04-16 15:00:43.690729 labda-0.0.5/labda/processing/wear_validity.py
--rw-r--r--   0        0        0      250 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/__init__.py
--rw-r--r--   0        0        0     4586 2024-04-18 20:03:45.509841 labda-0.0.5/labda/structure/collection.py
--rw-r--r--   0        0        0      704 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/domains.py
--rw-r--r--   0        0        0      600 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/linkage.py
--rw-r--r--   0        0        0     5000 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/merging.py
--rw-r--r--   0        0        0     3008 2024-04-21 13:40:30.406206 labda-0.0.5/labda/structure/resampling.py
--rw-r--r--   0        0        0     9175 2024-04-20 14:54:17.534360 labda-0.0.5/labda/structure/subject.py
--rw-r--r--   0        0        0        0 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/validation/__init__.py
--rw-r--r--   0        0        0      963 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/validation/domains.py
--rw-r--r--   0        0        0      833 2024-04-16 15:00:43.690729 labda-0.0.5/labda/structure/validation/linkage.py
--rw-r--r--   0        0        0    11122 2024-04-21 13:40:25.486206 labda-0.0.5/labda/structure/validation/subject.py
--rw-r--r--   0        0        0     8345 2024-04-21 13:34:59.116207 labda-0.0.5/labda/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 15:00:43.690729 labda-0.0.5/labda/visualisation/__init__.py
--rw-r--r--   0        0        0     3707 2024-04-16 15:00:43.690729 labda-0.0.5/labda/visualisation/spatial.py
--rw-r--r--   0        0        0     1520 2024-04-22 12:44:30.823453 labda-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 labda-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      570 2024-04-10 12:25:11.794327 labda-0.0.6/README.md
+-rw-r--r--   0        0        0      190 2024-04-23 14:37:04.188505 labda-0.0.6/labda/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.6/labda/assets/__init__.py
+-rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.6/labda/assets/counts_cut_points.py
+-rw-r--r--   0        0        0      459 2024-04-02 11:28:47.324035 labda-0.0.6/labda/assets/transportation_cut_points.py
+-rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.6/labda/expanders/__init__.py
+-rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.6/labda/expanders/accelerometer.py
+-rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.6/labda/expanders/extras.py
+-rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.6/labda/expanders/spatial.py
+-rw-r--r--   0        0        0     1246 2024-04-23 14:37:16.071524 labda-0.0.6/labda/logging.py
+-rw-r--r--   0        0        0     1073 2024-04-02 14:15:23.256237 labda-0.0.6/labda/parallel.py
+-rw-r--r--   0        0        0      201 2024-04-23 07:15:17.838214 labda-0.0.6/labda/parsers/__init__.py
+-rw-r--r--   0        0        0     6854 2024-04-02 08:51:54.456305 labda-0.0.6/labda/parsers/actigraph.py
+-rw-r--r--   0        0        0      930 2024-04-02 08:48:51.335892 labda-0.0.6/labda/parsers/bulk.py
+-rw-r--r--   0        0        0     6508 2024-04-08 08:01:34.897150 labda-0.0.6/labda/parsers/gadgetbridge.py
+-rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.6/labda/parsers/garmin.py
+-rw-r--r--   0        0        0    10952 2024-04-23 07:15:17.838214 labda-0.0.6/labda/parsers/qstarz.py
+-rw-r--r--   0        0        0     8602 2024-05-01 11:09:20.815127 labda-0.0.6/labda/parsers/sens.py
+-rw-r--r--   0        0        0     8322 2024-05-01 07:54:55.911821 labda-0.0.6/labda/parsers/traccar.py
+-rw-r--r--   0        0        0     1737 2024-04-23 07:15:17.838214 labda-0.0.6/labda/parsers/utils.py
+-rw-r--r--   0        0        0       36 2024-02-09 10:52:49.204568 labda-0.0.6/labda/processing/__init__.py
+-rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.6/labda/processing/accelerometer/__init__.py
+-rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.6/labda/processing/accelerometer/activity_intensity.py
+-rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/accelerometer/steps.py
+-rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/accelerometer/wear.py
+-rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/bouts.py
+-rw-r--r--   0        0        0      860 2024-04-16 07:17:13.024246 labda-0.0.6/labda/processing/domains.py
+-rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/manipulations.py
+-rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.6/labda/processing/spatial/__init__.py
+-rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.6/labda/processing/spatial/manipulations.py
+-rw-r--r--   0        0        0     3277 2024-04-03 14:44:06.593954 labda-0.0.6/labda/processing/spatial/timeline.py
+-rw-r--r--   0        0        0     3792 2024-05-01 14:19:00.081204 labda-0.0.6/labda/processing/spatial/transportation.py
+-rw-r--r--   0        0        0    25960 2024-04-23 07:15:17.848219 labda-0.0.6/labda/processing/spatial/trips.py
+-rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.6/labda/processing/wear_validity.py
+-rw-r--r--   0        0        0      250 2024-03-12 09:04:33.383063 labda-0.0.6/labda/structure/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-02 13:58:21.046661 labda-0.0.6/labda/structure/collection.py
+-rw-r--r--   0        0        0      704 2024-04-08 08:01:34.897150 labda-0.0.6/labda/structure/domains.py
+-rw-r--r--   0        0        0      600 2024-04-08 08:01:34.897150 labda-0.0.6/labda/structure/linkage.py
+-rw-r--r--   0        0        0     5000 2024-04-02 08:48:51.335892 labda-0.0.6/labda/structure/merging.py
+-rw-r--r--   0        0        0     3008 2024-05-01 14:17:08.613103 labda-0.0.6/labda/structure/resampling.py
+-rw-r--r--   0        0        0     9175 2024-05-01 14:20:35.742466 labda-0.0.6/labda/structure/subject.py
+-rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.6/labda/structure/validation/__init__.py
+-rw-r--r--   0        0        0      963 2024-02-09 12:27:12.019606 labda-0.0.6/labda/structure/validation/domains.py
+-rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.6/labda/structure/validation/linkage.py
+-rw-r--r--   0        0        0    11122 2024-05-01 14:19:06.349985 labda-0.0.6/labda/structure/validation/subject.py
+-rw-r--r--   0        0        0     8345 2024-04-23 07:15:17.848219 labda-0.0.6/labda/utils.py
+-rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.6/labda/visualisation/__init__.py
+-rw-r--r--   0        0        0     3707 2024-04-08 11:46:48.951159 labda-0.0.6/labda/visualisation/spatial.py
+-rw-r--r--   0        0        0     1668 2024-05-01 14:22:23.526187 labda-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2068 1970-01-01 00:00:00.000000 labda-0.0.6/PKG-INFO
```

### Comparing `labda-0.0.5/README.md` & `labda-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/assets/counts_cut_points.py` & `labda-0.0.6/labda/assets/counts_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/expanders/accelerometer.py` & `labda-0.0.6/labda/expanders/accelerometer.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/expanders/extras.py` & `labda-0.0.6/labda/expanders/extras.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/expanders/spatial.py` & `labda-0.0.6/labda/expanders/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/logging.py` & `labda-0.0.6/labda/logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return (
         f"<{color}>"
         + "{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}\n"
         + f"</{color}>"
     )
 
 
-def configure_logger(level: str):
+def configure_logging(level: str):
     logger.remove()
     logger.add(
         sys.stderr,
         format=formatter,
         colorize=True,
         level=level,
     )
@@ -45,10 +45,10 @@
     meta = subject.metadata
     sampling_frequency = (
         f"SF: {meta.sampling_frequency}s" if meta.sampling_frequency else ""
     )
     timezone = f", TZ: {meta.timezone}" if meta.timezone else ""
     crs = f", CRS: {meta.crs}" if meta.crs else ""
 
-    logger.success(
-        f"{func} | {source} | Parsed {len(subject.df)} records ({sampling_frequency}{timezone}{crs})"
+    logger.opt(ansi=True).success(
+        f"{func} | <bold>Source:</bold> {source} | <bold>Subject:</bold> {subject.metadata.id} | <bold>Parsed {len(subject.df)} records</bold> ({sampling_frequency}{timezone}{crs})"
     )
```

### Comparing `labda-0.0.5/labda/parallel.py` & `labda-0.0.6/labda/parallel.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/parsers/actigraph.py` & `labda-0.0.6/labda/parsers/actigraph.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/parsers/bulk.py` & `labda-0.0.6/labda/parsers/bulk.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/parsers/gadgetbridge.py` & `labda-0.0.6/labda/parsers/gadgetbridge.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/parsers/garmin.py` & `labda-0.0.6/labda/parsers/garmin.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/parsers/qstarz.py` & `labda-0.0.6/labda/parsers/qstarz.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             break
 
     nsat = "NSAT"
 
     if nsat_uv in df.columns:
         if df[nsat_uv].str.contains("/").any():
             df[nsat_uv] = df[nsat_uv].str.split("/")
-        elif df[nsat_uv].str.contains("\(").any():
+        elif df[nsat_uv].str.contains(r"\(").any():  # Maybe this is wrong
             df[nsat_uv] = df[nsat_uv].str.replace(")", "").str.split("(")
         df[Column.NSAT_USED] = pd.to_numeric(df[nsat_uv].str[0])
         df[Column.NSAT_VIEWED] = pd.to_numeric(df[nsat_uv].str[1])
     elif nsat in df.columns:
         df.rename(columns={nsat: Column.NSAT_USED}, inplace=True)
         df[Column.NSAT_USED] = pd.to_numeric(df[Column.NSAT_USED])
```

### Comparing `labda-0.0.5/labda/parsers/utils.py` & `labda-0.0.6/labda/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/accelerometer/activity_intensity.py` & `labda-0.0.6/labda/processing/accelerometer/activity_intensity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/accelerometer/steps.py` & `labda-0.0.6/labda/processing/accelerometer/steps.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/accelerometer/wear.py` & `labda-0.0.6/labda/processing/accelerometer/wear.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/bouts.py` & `labda-0.0.6/labda/processing/bouts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/domains.py` & `labda-0.0.6/labda/processing/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/spatial/manipulations.py` & `labda-0.0.6/labda/processing/spatial/manipulations.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/spatial/timeline.py` & `labda-0.0.6/labda/processing/spatial/timeline.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/spatial/transportation.py` & `labda-0.0.6/labda/processing/spatial/transportation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _trip_mode_from_activity(df: pd.DataFrame) -> None:
     df.loc[
         (df[Column.TRIP_MODE] == "vehicle")
         & (
             df[Column.ACTIVITY_INTENSITY].isin(
-                ["moderate", "vigorous", "very_vigorous"]
+                ["moderate", "moderate-vigorous", "vigorous", "very_vigorous"]
             )
         ),
         Column.TRIP_MODE,
     ] = "bicycle"
 
     df.loc[
         (df[Column.TRIP_MODE].isin(["bicycle", "walk/run"]))
```

### Comparing `labda-0.0.5/labda/processing/spatial/trips.py` & `labda-0.0.6/labda/processing/spatial/trips.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/processing/wear_validity.py` & `labda-0.0.6/labda/processing/wear_validity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/collection.py` & `labda-0.0.6/labda/structure/collection.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/domains.py` & `labda-0.0.6/labda/structure/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/linkage.py` & `labda-0.0.6/labda/structure/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/merging.py` & `labda-0.0.6/labda/structure/merging.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/resampling.py` & `labda-0.0.6/labda/structure/resampling.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/subject.py` & `labda-0.0.6/labda/structure/subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from .validation.domains import SCHEMA as DOMAINS_SCHEMA
 from .validation.subject import SCHEMA, Column
 
 
 class Vendor(StrEnum):
     ACTIGRAPH = "ActiGraph"
     XIAOMI = "Xiaomi"
-    SENS = "SENS"
+    SENS = "Sens"
     GARMIN = "Garmin"
     QSTARZ = "Qstarz"
     GGIR = "GGIR"
     SENSECAP = "SenseCap"
     TRACCAR = "Traccar"
```

### Comparing `labda-0.0.5/labda/structure/validation/domains.py` & `labda-0.0.6/labda/structure/validation/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/validation/linkage.py` & `labda-0.0.6/labda/structure/validation/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/structure/validation/subject.py` & `labda-0.0.6/labda/structure/validation/subject.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/utils.py` & `labda-0.0.6/labda/utils.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/labda/visualisation/spatial.py` & `labda-0.0.6/labda/visualisation/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.5/pyproject.toml` & `labda-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labda"
-version = "0.0.5"
+version = "0.0.6"
 description = "Library for Advanced Behavioural Data Analysis"
 authors = ["Josef Heidler <jheidler@health.sdu.dk>"]
 maintainers = ["Josef Heidler <jheidler@health.sdu.dk>"]
 
 readme = "README.md"
 license = "	CC-BY-SA-4.0"
 homepage = "https://labda.josefheidler.cz"
@@ -34,21 +34,25 @@
 pyarrow = "^15.0.0"
 pandera = "^0.18.0"
 openpyxl = "^3.1.2"
 sqlalchemy = "^2.0.25"
 pydeck = "^0.8.0"
 loguru = "^0.7.2"
 actipy = "^3.0.5"
+black = "^24.4.0"
+plotly = "^5.21.0"
+requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.5.6"
-mkdocstrings = "^0.24.0"
+mkdocstrings = { extras = ["python"], version = "^0.24.3" }
 scikit-learn = "^1.4.0"
-resampy = "^0.4.2"         # Remove after Axivity CWA/CSV parser and RAW to counts conversion is implemented
+resampy = "^0.4.2"                                          # Remove after Axivity CWA/CSV parser and RAW to counts conversion is implemented
+matplotlib = "^3.8.4"
 
 [tool.poetry.group.jupyter.dependencies]
 ipykernel = "^6.29.0"
 nbformat = "^5.9.2"
 
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `labda-0.0.5/PKG-INFO` & `labda-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labda
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for Advanced Behavioural Data Analysis
 Home-page: https://labda.josefheidler.cz
 License: 	CC-BY-SA-4.0
 Keywords: analysis,health,behaviour,data,spatial,temporal
 Author: Josef Heidler
 Author-email: jheidler@health.sdu.dk
 Maintainer: Josef Heidler
@@ -16,21 +16,24 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: actipy (>=3.0.5,<4.0.0)
+Requires-Dist: black (>=24.4.0,<25.0.0)
 Requires-Dist: geopandas (>=0.14.2,<0.15.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pandera (>=0.18.0,<0.19.0)
+Requires-Dist: plotly (>=5.21.0,<6.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
 Requires-Dist: timezonefinder (>=6.2.0,<7.0.0)
 Project-URL: Documentation, https://labda.josefheidler.cz
 Project-URL: Repository, https://github.com/josefheidler/labda
 Description-Content-Type: text/markdown
 
 # LABDA: Library for Advanced Behavioural Data Analysis
```

