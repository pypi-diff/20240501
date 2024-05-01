# Comparing `tmp/python_trading212-1.0.0.tar.gz` & `tmp/python_trading212-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_trading212-1.0.0.tar", max compression
+gzip compressed data, was "python_trading212-2.0.0.tar", max compression
```

## Comparing `python_trading212-1.0.0.tar` & `python_trading212-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-27 13:55:45.063219 python_trading212-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     2090 2024-04-27 13:55:45.063219 python_trading212-1.0.0/README.md
--rw-r--r--   0        0        0      449 2024-04-27 13:55:45.063219 python_trading212-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      324 2024-04-27 13:55:45.063219 python_trading212-1.0.0/python_trading212/__init__.py
--rw-r--r--   0        0        0     5287 2024-04-27 13:55:45.063219 python_trading212-1.0.0/python_trading212/models.py
--rw-r--r--   0        0        0    12528 2024-04-27 13:55:45.063219 python_trading212-1.0.0/python_trading212/trading212.py
--rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 python_trading212-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-01 08:27:35.956775 python_trading212-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2083 2024-05-01 08:27:35.956775 python_trading212-2.0.0/README.md
+-rw-r--r--   0        0        0      507 2024-05-01 08:27:35.956775 python_trading212-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-01 08:27:35.956775 python_trading212-2.0.0/trading212/__init__.py
+-rw-r--r--   0        0        0     5287 2024-05-01 08:27:35.956775 python_trading212-2.0.0/trading212/models.py
+-rw-r--r--   0        0        0    12521 2024-05-01 08:27:35.956775 python_trading212-2.0.0/trading212/trading212.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 python_trading212-2.0.0/PKG-INFO
```

### Comparing `python_trading212-1.0.0/LICENSE.md` & `python_trading212-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_trading212-1.0.0/README.md` & `python_trading212-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Set your API key in the environment variable:
 ```bash
 export TRADING_212_KEY=<your-api-key>
 ```
 
 ```python
-from python_trading212 import Trading212, Pie
+from trading212 import Trading212, Pie
 
 trading212 = Trading212()
 pie: Pie = trading212.fetch_pie(123)
 positions: List[Position] = trading212.fetch_all_open_positions()
 
 trading212.create_pie(
     Pie(
```

### Comparing `python_trading212-1.0.0/python_trading212/models.py` & `python_trading212-2.0.0/trading212/models.py`

 * *Files identical despite different names*

### Comparing `python_trading212-1.0.0/python_trading212/trading212.py` & `python_trading212-2.0.0/trading212/trading212.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import requests
 from typing import List, Dict
 from requests.exceptions import HTTPError
-from python_trading212.models import (
+from trading212.models import (
     Position, Exchange, Instrument,
     Pie, Order, AccountCash, AccountMetadata,
     HistoricalOrderData, LimitOrder, MarketOrder,
     StopOrder, StopLimitOrder, PaidOutDividends,
     Export, Report, TransactionList
 )
```

### Comparing `python_trading212-1.0.0/PKG-INFO` & `python_trading212-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-trading212
-Version: 1.0.0
+Version: 2.0.0
 Summary: An unofficial client for the official Trading212 API
 Author: José Coelho
 Author-email: 16445494+jcoelho93@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
@@ -32,15 +32,15 @@
 
 Set your API key in the environment variable:
 ```bash
 export TRADING_212_KEY=<your-api-key>
 ```
 
 ```python
-from python_trading212 import Trading212, Pie
+from trading212 import Trading212, Pie
 
 trading212 = Trading212()
 pie: Pie = trading212.fetch_pie(123)
 positions: List[Position] = trading212.fetch_all_open_positions()
 
 trading212.create_pie(
     Pie(
```

