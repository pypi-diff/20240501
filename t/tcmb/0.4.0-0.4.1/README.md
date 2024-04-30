# Comparing `tmp/tcmb-0.4.0.tar.gz` & `tmp/tcmb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcmb-0.4.0.tar", last modified: Sun Apr 14 11:30:24 2024, max compression
+gzip compressed data, was "tcmb-0.4.1.tar", last modified: Tue Apr 30 23:10:11 2024, max compression
```

## Comparing `tcmb-0.4.0.tar` & `tcmb-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-14 11:30:24.568287 tcmb-0.4.0/
--rw-r--r--   0 stba       (501) staff       (20)     2736 2023-01-12 22:31:50.000000 tcmb-0.4.0/.gitignore
--rw-r--r--   0 stba       (501) staff       (20)     1186 2023-04-25 23:39:26.000000 tcmb-0.4.0/CHANGELOG.md
--rw-r--r--   0 stba       (501) staff       (20)      129 2023-04-26 21:24:38.000000 tcmb-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 stba       (501) staff       (20)     1065 2023-01-12 21:37:38.000000 tcmb-0.4.0/LICENSE
--rw-r--r--   0 stba       (501) staff       (20)     7197 2024-04-14 11:30:24.567848 tcmb-0.4.0/PKG-INFO
--rw-r--r--   0 stba       (501) staff       (20)     5238 2023-04-26 21:10:17.000000 tcmb-0.4.0/README.md
--rw-r--r--   0 stba       (501) staff       (20)      781 2023-04-26 21:29:48.000000 tcmb-0.4.0/TODO.md
--rw-r--r--   0 stba       (501) staff       (20)      920 2024-04-14 11:29:26.000000 tcmb-0.4.0/pyproject.toml
--rw-r--r--   0 stba       (501) staff       (20)       21 2023-05-31 21:53:29.000000 tcmb-0.4.0/requirements.in
--rw-r--r--   0 stba       (501) staff       (20)      576 2023-05-31 21:53:29.000000 tcmb-0.4.0/requirements.txt
--rw-r--r--   0 stba       (501) staff       (20)       38 2024-04-14 11:30:24.568342 tcmb-0.4.0/setup.cfg
--rw-r--r--   0 stba       (501) staff       (20)       37 2023-01-12 21:38:29.000000 tcmb-0.4.0/setup.py
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-14 11:30:24.560992 tcmb-0.4.0/tcmb/
--rw-r--r--   0 stba       (501) staff       (20)       58 2024-04-14 11:28:53.000000 tcmb-0.4.0/tcmb/__init__.py
--rw-r--r--   0 stba       (501) staff       (20)     1506 2024-04-14 11:09:13.000000 tcmb-0.4.0/tcmb/_data.py
--rw-r--r--   0 stba       (501) staff       (20)     2166 2024-04-14 11:24:47.000000 tcmb-0.4.0/tcmb/auth.py
--rw-r--r--   0 stba       (501) staff       (20)      331 2023-01-12 22:32:13.000000 tcmb-0.4.0/tcmb/const.py
--rw-r--r--   0 stba       (501) staff       (20)    14022 2024-04-14 11:24:47.000000 tcmb-0.4.0/tcmb/core.py
--rw-r--r--   0 stba       (501) staff       (20)      562 2023-04-25 23:35:52.000000 tcmb-0.4.0/tcmb/errors.py
--rw-r--r--   0 stba       (501) staff       (20)     2017 2024-04-14 10:55:53.000000 tcmb-0.4.0/tcmb/fetch.py
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-14 11:30:24.563296 tcmb-0.4.0/tcmb/resources/
--rw-r--r--   0 stba       (501) staff       (20)   811490 2024-04-14 11:10:25.000000 tcmb-0.4.0/tcmb/resources/series.json
--rw-r--r--   0 stba       (501) staff       (20)     4512 2023-04-25 23:35:52.000000 tcmb-0.4.0/tcmb/utils.py
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-14 11:30:24.566998 tcmb-0.4.0/tcmb.egg-info/
--rw-r--r--   0 stba       (501) staff       (20)     7197 2024-04-14 11:30:24.000000 tcmb-0.4.0/tcmb.egg-info/PKG-INFO
--rw-r--r--   0 stba       (501) staff       (20)      498 2024-04-14 11:30:24.000000 tcmb-0.4.0/tcmb.egg-info/SOURCES.txt
--rw-r--r--   0 stba       (501) staff       (20)        1 2024-04-14 11:30:24.000000 tcmb-0.4.0/tcmb.egg-info/dependency_links.txt
--rw-r--r--   0 stba       (501) staff       (20)       22 2024-04-14 11:30:24.000000 tcmb-0.4.0/tcmb.egg-info/requires.txt
--rw-r--r--   0 stba       (501) staff       (20)        5 2024-04-14 11:30:24.000000 tcmb-0.4.0/tcmb.egg-info/top_level.txt
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-14 11:30:24.566512 tcmb-0.4.0/tests/
--rw-r--r--   0 stba       (501) staff       (20)        0 2023-01-07 22:09:47.000000 tcmb-0.4.0/tests/__init__.py
--rw-r--r--   0 stba       (501) staff       (20)      167 2023-01-25 21:50:00.000000 tcmb-0.4.0/tests/test_auth.py
--rw-r--r--   0 stba       (501) staff       (20)     1449 2023-01-25 21:50:00.000000 tcmb-0.4.0/tests/test_core.py
--rw-r--r--   0 stba       (501) staff       (20)        0 2023-04-26 21:12:34.000000 tcmb-0.4.0/tests/test_fetch.py
--rw-r--r--   0 stba       (501) staff       (20)        0 2023-04-26 21:11:58.000000 tcmb-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.970350 tcmb-0.4.1/
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.957710 tcmb-0.4.1/.github/
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.960334 tcmb-0.4.1/.github/workflows/
+-rw-r--r--   0 stba       (501) staff       (20)     1366 2024-04-30 21:47:35.000000 tcmb-0.4.1/.github/workflows/python-package.yml
+-rw-r--r--   0 stba       (501) staff       (20)     2736 2023-01-12 22:31:50.000000 tcmb-0.4.1/.gitignore
+-rw-r--r--   0 stba       (501) staff       (20)     1186 2023-04-25 23:39:26.000000 tcmb-0.4.1/CHANGELOG.md
+-rw-r--r--   0 stba       (501) staff       (20)      129 2023-04-26 21:24:38.000000 tcmb-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 stba       (501) staff       (20)     1065 2023-01-12 21:37:38.000000 tcmb-0.4.1/LICENSE
+-rw-r--r--   0 stba       (501) staff       (20)     7299 2024-04-30 23:10:11.970123 tcmb-0.4.1/PKG-INFO
+-rw-r--r--   0 stba       (501) staff       (20)     5340 2024-04-30 21:57:34.000000 tcmb-0.4.1/README.md
+-rw-r--r--   0 stba       (501) staff       (20)      781 2023-04-26 21:29:48.000000 tcmb-0.4.1/TODO.md
+-rw-r--r--   0 stba       (501) staff       (20)      920 2024-04-30 23:06:38.000000 tcmb-0.4.1/pyproject.toml
+-rw-r--r--   0 stba       (501) staff       (20)       21 2023-05-31 21:53:29.000000 tcmb-0.4.1/requirements.in
+-rw-r--r--   0 stba       (501) staff       (20)      576 2023-05-31 21:53:29.000000 tcmb-0.4.1/requirements.txt
+-rw-r--r--   0 stba       (501) staff       (20)       38 2024-04-30 23:10:11.970514 tcmb-0.4.1/setup.cfg
+-rw-r--r--   0 stba       (501) staff       (20)       37 2023-01-12 21:38:29.000000 tcmb-0.4.1/setup.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.962776 tcmb-0.4.1/tcmb/
+-rw-r--r--   0 stba       (501) staff       (20)       58 2024-04-30 23:06:52.000000 tcmb-0.4.1/tcmb/__init__.py
+-rw-r--r--   0 stba       (501) staff       (20)     1506 2024-04-30 21:40:55.000000 tcmb-0.4.1/tcmb/_data.py
+-rw-r--r--   0 stba       (501) staff       (20)     2240 2024-04-30 23:02:32.000000 tcmb-0.4.1/tcmb/auth.py
+-rw-r--r--   0 stba       (501) staff       (20)      331 2023-01-12 22:32:13.000000 tcmb-0.4.1/tcmb/const.py
+-rw-r--r--   0 stba       (501) staff       (20)    14083 2024-04-30 23:02:32.000000 tcmb-0.4.1/tcmb/core.py
+-rw-r--r--   0 stba       (501) staff       (20)      562 2023-04-25 23:35:52.000000 tcmb-0.4.1/tcmb/errors.py
+-rw-r--r--   0 stba       (501) staff       (20)     2017 2024-04-14 10:55:53.000000 tcmb-0.4.1/tcmb/fetch.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.963926 tcmb-0.4.1/tcmb/resources/
+-rw-r--r--   0 stba       (501) staff       (20)   811490 2024-04-30 20:24:50.000000 tcmb-0.4.1/tcmb/resources/series.json
+-rw-r--r--   0 stba       (501) staff       (20)     4873 2024-04-30 23:02:32.000000 tcmb-0.4.1/tcmb/utils.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.969597 tcmb-0.4.1/tcmb.egg-info/
+-rw-r--r--   0 stba       (501) staff       (20)     7299 2024-04-30 23:10:11.000000 tcmb-0.4.1/tcmb.egg-info/PKG-INFO
+-rw-r--r--   0 stba       (501) staff       (20)      535 2024-04-30 23:10:11.000000 tcmb-0.4.1/tcmb.egg-info/SOURCES.txt
+-rw-r--r--   0 stba       (501) staff       (20)        1 2024-04-30 23:10:11.000000 tcmb-0.4.1/tcmb.egg-info/dependency_links.txt
+-rw-r--r--   0 stba       (501) staff       (20)       22 2024-04-30 23:10:11.000000 tcmb-0.4.1/tcmb.egg-info/requires.txt
+-rw-r--r--   0 stba       (501) staff       (20)        5 2024-04-30 23:10:11.000000 tcmb-0.4.1/tcmb.egg-info/top_level.txt
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2024-04-30 23:10:11.968607 tcmb-0.4.1/tests/
+-rw-r--r--   0 stba       (501) staff       (20)        0 2023-01-07 22:09:47.000000 tcmb-0.4.1/tests/__init__.py
+-rw-r--r--   0 stba       (501) staff       (20)      167 2023-01-25 21:50:00.000000 tcmb-0.4.1/tests/test_auth.py
+-rw-r--r--   0 stba       (501) staff       (20)     1449 2023-01-25 21:50:00.000000 tcmb-0.4.1/tests/test_core.py
+-rw-r--r--   0 stba       (501) staff       (20)        0 2023-04-26 21:12:34.000000 tcmb-0.4.1/tests/test_fetch.py
+-rw-r--r--   0 stba       (501) staff       (20)      720 2024-04-30 23:02:32.000000 tcmb-0.4.1/tests/test_utils.py
```

### Comparing `tcmb-0.4.0/.gitignore` & `tcmb-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/CHANGELOG.md` & `tcmb-0.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/LICENSE` & `tcmb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/PKG-INFO` & `tcmb-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcmb
-Version: 0.4.0
+Version: 0.4.1
 Summary: Central Bank of the Republic of Türkiye (TCMB) Python API.
 Author-email: Kaymal <gutkyle@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 T.Kaymal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 # tcmb
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/tcmb)](https://pypi.org/project/tcmb/)
 [![License](https://img.shields.io/github/license/kaymal/tcmb-py)](https://github.com/kaymal/tcmb-py/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/tcmb)](https://pepy.tech/project/tcmb)
 [![Python Version](https://img.shields.io/pypi/pyversions/tcmb)]()
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Package workflow](https://github.com/kaymal/tcmb-py/actions/workflows/python-package.yml/badge.svg)
 
 `tcmb` is a Python API wrapper around the Central Bank of the Republic of Türkiye (TCMB) Web Service. It is an _unofficial_ open-source Python package intended for personal use ([Disclaimer](#disclaimer)).
 
 ---
 
 _`tcmb`, Türkiye Cumhuriyeti Merkez Bankası (TCMB) Web Servisi'ne Python aracılığıyla erişimi sağlayan resmi olmayan API uygulamasıdır. Kişisel kullanım ve araştırma maksadıyla hazırlanmıştır ([Elektronik Veri Dağıtım Sistemi (EVDS) Kullanım Koşulları](https://evds2.tcmb.gov.tr/help/videos/EVDS_Kullanim_Sartlari.pdf))._
```

### Comparing `tcmb-0.4.0/README.md` & `tcmb-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # tcmb
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/tcmb)](https://pypi.org/project/tcmb/)
 [![License](https://img.shields.io/github/license/kaymal/tcmb-py)](https://github.com/kaymal/tcmb-py/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/tcmb)](https://pepy.tech/project/tcmb)
 [![Python Version](https://img.shields.io/pypi/pyversions/tcmb)]()
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Package workflow](https://github.com/kaymal/tcmb-py/actions/workflows/python-package.yml/badge.svg)
 
 `tcmb` is a Python API wrapper around the Central Bank of the Republic of Türkiye (TCMB) Web Service. It is an _unofficial_ open-source Python package intended for personal use ([Disclaimer](#disclaimer)).
 
 ---
 
 _`tcmb`, Türkiye Cumhuriyeti Merkez Bankası (TCMB) Web Servisi'ne Python aracılığıyla erişimi sağlayan resmi olmayan API uygulamasıdır. Kişisel kullanım ve araştırma maksadıyla hazırlanmıştır ([Elektronik Veri Dağıtım Sistemi (EVDS) Kullanım Koşulları](https://evds2.tcmb.gov.tr/help/videos/EVDS_Kullanim_Sartlari.pdf))._
```

### Comparing `tcmb-0.4.0/TODO.md` & `tcmb-0.4.1/TODO.md`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/pyproject.toml` & `tcmb-0.4.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tcmb"
-version = "0.4.0"
+version = "0.4.1"
 authors = [{ name = "Kaymal", email = "gutkyle@gmail.com" }]
 description = "Central Bank of the Republic of Türkiye (TCMB) Python API."
 readme = "README.md"
 license = { file = 'LICENSE' }
 requires-python = ">=3.8"
 classifiers = [
     'Operating System :: OS Independent',
```

### Comparing `tcmb-0.4.0/requirements.txt` & `tcmb-0.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/tcmb/_data.py` & `tcmb-0.4.1/tcmb/_data.py`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/tcmb/auth.py` & `tcmb-0.4.1/tcmb/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,17 @@
             print(f"Response Error Message: {error_msg}")
 
             # evds responds with an 500 Internal Server Error for almost
             # any issues. This error response is a generic "catch-all" response.
             # Therefore the traceback is printed as well as the most
             # probable cause of the HTTPError: ApiKeyError
             print(err.with_traceback(None))
-            raise ApiKeyError("API key is invalid.") from err
+            raise ApiKeyError(
+                "API key is invalid or wrong key. See error message for details."
+            ) from err
     else:
         try:
             response.json()
         except JSONDecodeError:
             if "error-title" in response.text:
                 raise InvalidSeriesCode()
             else:
```

### Comparing `tcmb-0.4.0/tcmb/core.py` & `tcmb-0.4.1/tcmb/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,28 +118,30 @@
     if isinstance(series, str):
         if ("*" in series) or ("?" in series) or (".." in series):
             series = utils.wildcard_search(series)
 
     # convert list to str seperated by "-"
     # as descibed in the api reference
     if isinstance(series, list):
-        series = "-".join(series)
+        series_str = "-".join(series)
+    else:
+        series_str = series
 
     # convert list to str seperated by "-"
     if isinstance(agg, list):
         agg = "-".join(agg)
 
     # convert date string formats to "DD-MM-YYYY"
     if start:
         start = utils.standardize_date(start)
     if end:
         end = utils.standardize_date(end)
 
     params = {
-        "series": series,
+        "series": series_str,
         "startDate": start or "01-01-1970",
         "endDate": end or date.today().strftime("%d-%m-%Y"),
         "type": "json",  # csv, xml, json
         "aggregationTypes": agg,
         "formulas": formulas,
         "frequency": freq,
         "decimalSeperator": seperator,
@@ -152,15 +154,15 @@
     elif "key" not in headers:
         headers["key"] = api_key
 
     res = fetch.get_response(params=params, headers=headers)
 
     # convert response JSON to DataFrame
     #   time series data is in the "items"
-    data = utils.to_dataframe(res.json()["items"])
+    data = utils.to_dataframe(res.json()["items"], series=series)
 
     return data
 
 
 class Client:
     """Base class for TCMB web service access.
```

### Comparing `tcmb-0.4.0/tcmb/errors.py` & `tcmb-0.4.1/tcmb/errors.py`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/tcmb/fetch.py` & `tcmb-0.4.1/tcmb/fetch.py`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/tcmb/resources/series.json` & `tcmb-0.4.1/tcmb/resources/series.json`

 * *Files identical despite different names*

### Comparing `tcmb-0.4.0/tcmb/utils.py` & `tcmb-0.4.1/tcmb/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Utilities module."""
+from __future__ import annotations
+
 import json
 import re
 import os.path
 from datetime import datetime
 
 
 import numpy as np
 import pandas as pd
 
+from tcmb._data import fetch_dg_series_codes
+
 
 def standardize_date(date_str: str) -> str:
     """Standardize date string format to output DD-MM-YYYY.
 
     TCMB Web Service accepts dates in DD-MM-YYYY format only.
     This function converts datetime dtype and date string
     in YYYY-MM-DD format into the default TCMB format.
@@ -39,32 +43,41 @@
         date_format = "%Y-%m-%d"
     elif re.match(r"\d{4}.\d{1,2}.\d{1,2}", date_str):
         date_format = "%Y.%m.%d"
 
     return datetime.strptime(date_str, date_format).strftime("%d-%m-%Y")
 
 
-def to_dataframe(data: dict) -> pd.DataFrame:
+def to_dataframe(data: dict, series: str | list) -> pd.DataFrame:
     """Convert data from the json response to pandas DataFrame."""
+    if isinstance(series, str):
+        series = [series]
+
+    # generate column names from series keys by replacing "." with "_"
+    # these columns will be selected as the value columns
+    # the columns other than date (Tarih) and value columns will be dropped
+    value_cols = [col.replace(".", "_") for col in series]
+
     df = pd.DataFrame(data)
     # drop unused column
-    df = df.drop("UNIXTIME", axis=1)
+    df = df[["Tarih", *value_cols]]
     # set date as index
-    # TODO: check if "Tarih" always the first column
-    df = df.set_index(df.columns[0])
+    # TODO: check if "Tarih" always the date column
+    df = df.set_index("Tarih")
 
     # detect date format
     if re.match(r"\d+-\d+-\d{4}", df.index[0]):
         date_format = "%d-%m-%Y"
     elif re.match(r"\d+-\d{4}", df.index[0]):
         date_format = "%m-%Y"
     elif re.match(r"\d{4}-\d+", df.index[0]):
         date_format = "%Y-%m"
     elif re.match(r"\d{4}", df.index[0]):
         date_format = "%Y"
+
     # convert date strings to datetime
     df.index = pd.to_datetime(df.index, format=date_format)
 
     # replace None with NaN
     df = df.fillna(np.nan)
     # convert object columns to float
     # TODO: convert to integer when possible
@@ -122,16 +135,14 @@
                 os.path.dirname(__file__), "resources", "series.json"
             )
 
             with open(file_path, "r") as file:
                 dg_series = json.load(file)
 
         else:
-            from tcmb._data import fetch_dg_series_codes
-
             dg_series = fetch_dg_series_codes()
 
         # merge series of all datagroups into one list
         for item in dg_series.values():
             items.extend(item)
 
     # Replace the wildcard characters with a regex-friendly equivalent.
```

### Comparing `tcmb-0.4.0/tcmb.egg-info/PKG-INFO` & `tcmb-0.4.1/tcmb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcmb
-Version: 0.4.0
+Version: 0.4.1
 Summary: Central Bank of the Republic of Türkiye (TCMB) Python API.
 Author-email: Kaymal <gutkyle@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 T.Kaymal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 # tcmb
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/tcmb)](https://pypi.org/project/tcmb/)
 [![License](https://img.shields.io/github/license/kaymal/tcmb-py)](https://github.com/kaymal/tcmb-py/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/tcmb)](https://pepy.tech/project/tcmb)
 [![Python Version](https://img.shields.io/pypi/pyversions/tcmb)]()
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Package workflow](https://github.com/kaymal/tcmb-py/actions/workflows/python-package.yml/badge.svg)
 
 `tcmb` is a Python API wrapper around the Central Bank of the Republic of Türkiye (TCMB) Web Service. It is an _unofficial_ open-source Python package intended for personal use ([Disclaimer](#disclaimer)).
 
 ---
 
 _`tcmb`, Türkiye Cumhuriyeti Merkez Bankası (TCMB) Web Servisi'ne Python aracılığıyla erişimi sağlayan resmi olmayan API uygulamasıdır. Kişisel kullanım ve araştırma maksadıyla hazırlanmıştır ([Elektronik Veri Dağıtım Sistemi (EVDS) Kullanım Koşulları](https://evds2.tcmb.gov.tr/help/videos/EVDS_Kullanim_Sartlari.pdf))._
```

### Comparing `tcmb-0.4.0/tests/test_core.py` & `tcmb-0.4.1/tests/test_core.py`

 * *Files identical despite different names*

