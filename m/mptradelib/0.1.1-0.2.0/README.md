# Comparing `tmp/mptradelib-0.1.1.tar.gz` & `tmp/mptradelib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.1.1.tar", max compression
+gzip compressed data, was "mptradelib-0.2.0.tar", max compression
```

## Comparing `mptradelib-0.1.1.tar` & `mptradelib-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.1.1/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.1.1/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     8152 2024-04-30 11:43:29.264148 mptradelib-0.1.1/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.1.1/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2384 2024-04-30 08:45:09.478921 mptradelib-0.1.1/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.1.1/mptradelib/feed.py
--rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.1.1/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34081 2024-04-30 11:05:54.498358 mptradelib-0.1.1/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.1.1/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.1.1/mptradelib/utils.py
--rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.1.1/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-04-30 11:50:20.256288 mptradelib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.2.0/mptradelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.2.0/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5750 2024-05-01 10:07:01.546960 mptradelib-0.2.0/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.2.0/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2384 2024-04-30 08:45:09.478921 mptradelib-0.2.0/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.2.0/mptradelib/feed.py
+-rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.2.0/mptradelib/livetrading.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.2.0/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.2.0/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.2.0/mptradelib/utils.py
+-rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.2.0/mptradelib/vectorised_backtest.py
+-rw-r--r--   0        0        0      561 2024-05-01 10:07:22.791661 mptradelib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.2.0/PKG-INFO
```

### Comparing `mptradelib-0.1.1/README.md` & `mptradelib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/broker/broker.py` & `mptradelib-0.2.0/mptradelib/broker/broker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,22 @@
 import datetime as dt
-import os
 
 try:
     import pandas as pd
 except ImportError:
     pass
 
 import os
 from .. import utils
 from .session import FyersSession, ShoonyaSession
 from ..shoonya import *
 from pydantic import BaseModel, Field
 
 
-DATA_PATH = "./data"
-
-
 class Historical:
-    def __init__(self, sesson: FyersSession, data_path=DATA_PATH) -> None:
-        self._session = sesson
-        self._client = None
-        self._data_path = data_path
-
-    def _fetch_data_online(self, data_location, market, symbol, compression_format):
-        for s, e in utils.iterdaterange(step=100):
-            if os.path.exists(f"{data_location}/{e}.csv.{compression_format}"):
-                print(f"skipping {s} to {e}")
-                continue
-
-            payload = {
-                "symbol": f"{market}:{symbol}",
-                "resolution": "1",
-                "date_format": "1",
-                "range_from": s,
-                "range_to": e,
-                "cont_flag": "1",
-            }
-            if self._client is None:
-                self._client = self._session.init_client()
-            data = self._client.history(data=payload)
-            if len(data["candles"]) == 0:
-                break
-
-            df = pd.DataFrame(data["candles"], columns=["datetime", "open", "high", "low", "close", "volume"])
-            df.index = pd.to_datetime(df["datetime"], unit="s", utc=True).map(
-                lambda x: x.tz_convert("Asia/Kolkata")
-            )
-
-            for date, part in df.groupby([df.index.date]):
-                filename = f'{data_location}/{date[0].strftime("%Y-%m-%d")}.csv.zip'
-                part.to_csv(
-                    filename,
-                    index=False,
-                    compression={"method": "zip", "archive_name": filename},
-                )
-
-            print(s, e, "fetching...")
-
-    def _get_data_from_files(self, data_location):
-        return pd.concat(
-            [pd.read_csv(f"{data_location}/{e}") for e in os.listdir(data_location)]
-        )
-
-    def historical(self, market, symbol, compression_format="zip"):
-        data_location = os.path.join(self._data_path, f"{market}_{symbol}")
-
-        if not utils.unpack_data(data_location, compression_format):
-            self._fetch_data_online(data_location, market, symbol, compression_format)
-
-        df = self._get_data_from_files(data_location)
-        df = df.set_index("datetime")
-        df.index = pd.to_datetime(df.index, unit="s", utc=True).tz_convert(
-            "Asia/Kolkata"
-        )
-        df = df.sort_index()
-
-        utils.pack_data(data_location, compression_format)
-        return df
-
-class HistoricalV2:
     def __init__(self, session: FyersSession) -> None:
         self._session = session
         self._client = None
 
     def historical(self, market, symbol, resolution, start, end):
         curr = start
         delta = dt.timedelta(days=100)
```

### Comparing `mptradelib-0.1.1/mptradelib/broker/session.py` & `mptradelib-0.2.0/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/broker/ticker.py` & `mptradelib-0.2.0/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/feed.py` & `mptradelib-0.2.0/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/livetrading.py` & `mptradelib-0.2.0/mptradelib/livetrading.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/shoonya.py` & `mptradelib-0.2.0/mptradelib/shoonya.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import requests
 import threading
 import websocket
 import logging
-import datetime
+import datetime as dt
 import hashlib
 import time
 import urllib
 from time import sleep
-from datetime import datetime as dt
 
 logger = logging.getLogger(__name__)
 
 class position:
     prd:str
     exch:str
     instname:str
@@ -919,19 +918,19 @@
         #prepare the uri
         #url = f"{config['eoddata_endpoint']}" 
         url = f"{config['host']}{config['routes']['get_daily_price_series']}" 
         reportmsg(url)
 
         #prepare the data
         if startdate == None:  
-            week_ago = datetime.date.today() - datetime.timedelta(days=7)
-            startdate = dt.combine(week_ago, dt.min.time()).timestamp()
+            week_ago = dt.date.today() - dt.timedelta(days=7)
+            startdate = dt.datetime.combine(week_ago, dt.datetime.min.time()).timestamp()
 
         if enddate == None:            
-            enddate = dt.now().timestamp()
+            enddate = dt.datetime.now().timestamp()
 
         #
         values              = {}
         values["uid"]       = self.__username
         values["sym"]      = '{0}:{1}'.format(exchange, tradingsymbol)
         values["from"]     = str(startdate)
         values["to"]       = str(enddate)
```

### Comparing `mptradelib-0.1.1/mptradelib/test_renko.py` & `mptradelib-0.2.0/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/utils.py` & `mptradelib-0.2.0/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/mptradelib/vectorised_backtest.py` & `mptradelib-0.2.0/mptradelib/vectorised_backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.1/pyproject.toml` & `mptradelib-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.1.1/PKG-INFO` & `mptradelib-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

