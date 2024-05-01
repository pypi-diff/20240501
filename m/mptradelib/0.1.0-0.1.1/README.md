# Comparing `tmp/mptradelib-0.1.0.tar.gz` & `tmp/mptradelib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.1.0.tar", max compression
+gzip compressed data, was "mptradelib-0.1.1.tar", max compression
```

## Comparing `mptradelib-0.1.0.tar` & `mptradelib-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3150 2024-04-30 11:45:07.267788 mptradelib-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.1.0/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.1.0/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     8152 2024-04-30 11:43:29.264148 mptradelib-0.1.0/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.1.0/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2384 2024-04-30 08:45:09.478921 mptradelib-0.1.0/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.1.0/mptradelib/feed.py
--rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.1.0/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34081 2024-04-30 11:05:54.498358 mptradelib-0.1.0/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.1.0/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.1.0/mptradelib/utils.py
--rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.1.0/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-04-30 11:44:49.608590 mptradelib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 mptradelib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.1.1/mptradelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.1.1/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     8152 2024-04-30 11:43:29.264148 mptradelib-0.1.1/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.1.1/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2384 2024-04-30 08:45:09.478921 mptradelib-0.1.1/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.1.1/mptradelib/feed.py
+-rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.1.1/mptradelib/livetrading.py
+-rw-r--r--   0        0        0    34081 2024-04-30 11:05:54.498358 mptradelib-0.1.1/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.1.1/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.1.1/mptradelib/utils.py
+-rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.1.1/mptradelib/vectorised_backtest.py
+-rw-r--r--   0        0        0      561 2024-04-30 11:50:20.256288 mptradelib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.1.1/PKG-INFO
```

### Comparing `mptradelib-0.1.0/README.md` & `mptradelib-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,24 +44,28 @@
 
 ```
 
 Compute `df['entries']` with `1` for `BUY` and `-1` for `SELL`.
 
 ### Run
 ```
+from mptradelib.vectorised_backtest import Backtest
+
 b = Backtest(df, compute)
 result = b.run(ema_fast=20, ema_slow=50, ema_trend=200, sl=1, tp=2)
 ```
 
 `sl` and `tp` are in percentage and mandatory.
 
 params passed in `run` can be accessed using `params` inside `compute`
 
 ### Optimize
 ```
+from mptradelib.vectorised_backtest import Backtest
+
 optimization_params = {
     ema_fast: range(1, 20, 1),
     ema_slow: range(20, 50, 1),
     ema_trend: range(100, 200, 1),
     sl: range(0, 1),
     tp: range(1, 10),
 }
```

### Comparing `mptradelib-0.1.0/mptradelib/broker/broker.py` & `mptradelib-0.1.1/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/broker/session.py` & `mptradelib-0.1.1/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/broker/ticker.py` & `mptradelib-0.1.1/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/feed.py` & `mptradelib-0.1.1/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/livetrading.py` & `mptradelib-0.1.1/mptradelib/livetrading.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/shoonya.py` & `mptradelib-0.1.1/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/test_renko.py` & `mptradelib-0.1.1/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/utils.py` & `mptradelib-0.1.1/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/mptradelib/vectorised_backtest.py` & `mptradelib-0.1.1/mptradelib/vectorised_backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.1.0/pyproject.toml` & `mptradelib-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.1.0/PKG-INFO` & `mptradelib-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -62,24 +62,28 @@
 
 ```
 
 Compute `df['entries']` with `1` for `BUY` and `-1` for `SELL`.
 
 ### Run
 ```
+from mptradelib.vectorised_backtest import Backtest
+
 b = Backtest(df, compute)
 result = b.run(ema_fast=20, ema_slow=50, ema_trend=200, sl=1, tp=2)
 ```
 
 `sl` and `tp` are in percentage and mandatory.
 
 params passed in `run` can be accessed using `params` inside `compute`
 
 ### Optimize
 ```
+from mptradelib.vectorised_backtest import Backtest
+
 optimization_params = {
     ema_fast: range(1, 20, 1),
     ema_slow: range(20, 50, 1),
     ema_trend: range(100, 200, 1),
     sl: range(0, 1),
     tp: range(1, 10),
 }
```

