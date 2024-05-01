# Comparing `tmp/nixtla-0.4.0.tar.gz` & `tmp/nixtla-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtla-0.4.0.tar", last modified: Thu Apr 25 02:01:19 2024, max compression
+gzip compressed data, was "nixtla-0.5.0.tar", last modified: Wed May  1 19:51:14 2024, max compression
```

## Comparing `nixtla-0.4.0.tar` & `nixtla-0.5.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.340592 nixtla-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-04-25 02:01:13.000000 nixtla-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-25 02:01:19.340592 nixtla-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 02:01:13.000000 nixtla-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19978 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    48931 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/core/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/client_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/jsonable_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/core/remove_none_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/date_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/distributed/nixtla_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.332591 nixtla-0.4.0/nixtla/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/errors/unprocessable_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/nixtla_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.336591 nixtla-0.4.0/nixtla/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_anomaly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_cross_validation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/multi_series_insample_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/single_series_insample_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/types/validation_error_loc_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 02:01:13.000000 nixtla-0.4.0/nixtla/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:01:19.336591 nixtla-0.4.0/nixtla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 02:01:19.000000 nixtla-0.4.0/nixtla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:01:19.340592 nixtla-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 02:01:13.000000 nixtla-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.927730 nixtla-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-05-01 19:51:09.000000 nixtla-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-01 19:51:14.927730 nixtla-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-01 19:51:09.000000 nixtla-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.915730 nixtla-0.5.0/nixtla/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   304758 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.919730 nixtla-0.5.0/nixtla/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/jsonable_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/pydantic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/remove_none_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/request_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/date_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.919730 nixtla-0.5.0/nixtla/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/distributed/nixtla_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.919730 nixtla-0.5.0/nixtla/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/errors/unprocessable_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65345 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/nixtla_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.923730 nixtla-0.5.0/nixtla/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_cross_validation_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_cross_validation_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/validation_error_loc_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.923730 nixtla-0.5.0/nixtla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:51:14.927730 nixtla-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-01 19:51:09.000000 nixtla-0.5.0/setup.py
```

### Comparing `nixtla-0.4.0/LICENSE` & `nixtla-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtla-0.4.0/PKG-INFO` & `nixtla-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: nixtla
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: pandas
-Requires-Dist: pydantic<2
+Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: tenacity
 Requires-Dist: utilsforecast>=0.1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
 Requires-Dist: statsforecast; extra == "dev"
+Requires-Dist: hierarchicalforecast; extra == "dev"
 Requires-Dist: dask[dataframe]; extra == "dev"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "dev"
 Requires-Dist: pyspark; extra == "dev"
 Requires-Dist: ray[serve-grpc]; extra == "dev"
 Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "dev"
 Requires-Dist: holidays; extra == "dev"
 Provides-Extra: distributed
@@ -71,26 +72,26 @@
 With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtla>=0.1.0
+pip install nixtla>=0.4.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
 from nixtla import NixtlaClient
-nixtla = NixtlaClient(
+nixtla_client = NixtlaClient(
     # defaults to os.environ.get("NIXTLA_API_KEY")
     api_key = 'my_api_key_provided_by_nixtla'
 )
-fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
+fcst_df = nixtla_client.forecast(df, h=24, level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtla-0.4.0/README.md` & `nixtla-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtla>=0.1.0
+pip install nixtla>=0.4.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
 from nixtla import NixtlaClient
-nixtla = NixtlaClient(
+nixtla_client = NixtlaClient(
     # defaults to os.environ.get("NIXTLA_API_KEY")
     api_key = 'my_api_key_provided_by_nixtla'
 )
-fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
+fcst_df = nixtla_client.forecast(df, h=24, level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtla-0.4.0/nixtla/_modidx.py` & `nixtla-0.5.0/nixtla/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,20 @@
                 'doc_host': 'https://Nixtla.github.io',
                 'git_url': 'https://github.com/Nixtla/nixtla/',
                 'lib_path': 'nixtla'},
   'syms': { 'nixtla.client': {},
             'nixtla.core.api_error': {},
             'nixtla.core.client_wrapper': {},
             'nixtla.core.datetime_utils': {},
+            'nixtla.core.file': {},
+            'nixtla.core.http_client': {},
             'nixtla.core.jsonable_encoder': {},
+            'nixtla.core.pydantic_utilities': {},
             'nixtla.core.remove_none_from_dict': {},
+            'nixtla.core.request_options': {},
             'nixtla.date_features': { 'nixtla.date_features.CountryHolidays': ( 'date_features.html#countryholidays',
                                                                                 'nixtla/date_features.py'),
                                       'nixtla.date_features.CountryHolidays.__call__': ( 'date_features.html#countryholidays.__call__',
                                                                                          'nixtla/date_features.py'),
                                       'nixtla.date_features.CountryHolidays.__init__': ( 'date_features.html#countryholidays.__init__',
                                                                                          'nixtla/date_features.py'),
                                       'nixtla.date_features.CountryHolidays.__name__': ( 'date_features.html#countryholidays.__name__',
@@ -76,28 +80,34 @@
                                                                                        'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClient._cross_validation': ( 'nixtla_client.html#_nixtlaclient._cross_validation',
                                                                                                 'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClient._detect_anomalies': ( 'nixtla_client.html#_nixtlaclient._detect_anomalies',
                                                                                                 'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClient._forecast': ( 'nixtla_client.html#_nixtlaclient._forecast',
                                                                                         'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient._restore_uids': ( 'nixtla_client.html#_nixtlaclient._restore_uids',
+                                                                                            'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClient._uids_to_categorical': ( 'nixtla_client.html#_nixtlaclient._uids_to_categorical',
+                                                                                                   'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClient.plot': ( 'nixtla_client.html#_nixtlaclient.plot',
                                                                                    'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClient.validate_api_key': ( 'nixtla_client.html#_nixtlaclient.validate_api_key',
                                                                                                'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClient.validate_token': ( 'nixtla_client.html#_nixtlaclient.validate_token',
                                                                                              'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel': ( 'nixtla_client.html#_nixtlaclientmodel',
                                                                                    'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel.__init__': ( 'nixtla_client.html#_nixtlaclientmodel.__init__',
                                                                                             'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel._call_api': ( 'nixtla_client.html#_nixtlaclientmodel._call_api',
                                                                                              'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel._prepare_level_and_quantiles': ( 'nixtla_client.html#_nixtlaclientmodel._prepare_level_and_quantiles',
                                                                                                                 'nixtla/nixtla_client.py'),
+                                      'nixtla.nixtla_client._NixtlaClientModel._restrict_input_samples': ( 'nixtla_client.html#_nixtlaclientmodel._restrict_input_samples',
+                                                                                                           'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel._retry_strategy': ( 'nixtla_client.html#_nixtlaclientmodel._retry_strategy',
                                                                                                    'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel.add_date_features': ( 'nixtla_client.html#_nixtlaclientmodel.add_date_features',
                                                                                                      'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel.compute_date_feature': ( 'nixtla_client.html#_nixtlaclientmodel.compute_date_feature',
                                                                                                         'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client._NixtlaClientModel.cross_validation': ( 'nixtla_client.html#_nixtlaclientmodel.cross_validation',
@@ -133,29 +143,24 @@
                                       'nixtla.nixtla_client.partition_by_uid': ( 'nixtla_client.html#partition_by_uid',
                                                                                  'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client.remove_unused_categories': ( 'nixtla_client.html#remove_unused_categories',
                                                                                          'nixtla/nixtla_client.py'),
                                       'nixtla.nixtla_client.validate_model_parameter': ( 'nixtla_client.html#validate_model_parameter',
                                                                                          'nixtla/nixtla_client.py')},
             'nixtla.types.http_validation_error': {},
+            'nixtla.types.model': {},
             'nixtla.types.multi_series_anomaly': {},
-            'nixtla.types.multi_series_anomaly_model': {},
             'nixtla.types.multi_series_cross_validation': {},
             'nixtla.types.multi_series_cross_validation_fewshot_loss': {},
             'nixtla.types.multi_series_cross_validation_finetune_loss': {},
-            'nixtla.types.multi_series_cross_validation_model': {},
             'nixtla.types.multi_series_forecast': {},
             'nixtla.types.multi_series_forecast_fewshot_loss': {},
             'nixtla.types.multi_series_forecast_finetune_loss': {},
-            'nixtla.types.multi_series_forecast_model': {},
             'nixtla.types.multi_series_input': {},
             'nixtla.types.multi_series_insample_forecast': {},
-            'nixtla.types.multi_series_insample_forecast_model': {},
             'nixtla.types.single_series_forecast': {},
             'nixtla.types.single_series_forecast_fewshot_loss': {},
             'nixtla.types.single_series_forecast_finetune_loss': {},
-            'nixtla.types.single_series_forecast_model': {},
             'nixtla.types.single_series_insample_forecast': {},
-            'nixtla.types.single_series_insample_forecast_model': {},
             'nixtla.types.validation_error': {},
             'nixtla.types.validation_error_loc_item': {},
             'nixtla.utils': {'nixtla.utils.colab_badge': ('utils.html#colab_badge', 'nixtla/utils.py')}}}
```

### Comparing `nixtla-0.4.0/nixtla/core/client_wrapper.py` & `nixtla-0.5.0/nixtla/core/client_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 import httpx
 
+from .http_client import AsyncHttpClient, HttpClient
+
 
 class BaseClientWrapper:
-    def __init__(self, *, token: typing.Union[str, typing.Callable[[], str]], base_url: str):
+    def __init__(
+        self,
+        *,
+        token: typing.Union[str, typing.Callable[[], str]],
+        base_url: str,
+        timeout: typing.Optional[float] = None,
+    ):
         self._token = token
         self._base_url = base_url
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
-        headers: typing.Dict[str, str] = {
-            "X-Fern-Language": "Python",
-            "X-Fern-SDK-Name": "nixtla",
-            "X-Fern-SDK-Version": "0.0.0",
-        }
+        headers: typing.Dict[str, str] = {"X-Fern-Language": "Python"}
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
             return self._token
         else:
             return self._token()
 
     def get_base_url(self) -> str:
         return self._base_url
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
     def __init__(
-        self, *, token: typing.Union[str, typing.Callable[[], str]], base_url: str, httpx_client: httpx.Client
+        self,
+        *,
+        token: typing.Union[str, typing.Callable[[], str]],
+        base_url: str,
+        timeout: typing.Optional[float] = None,
+        httpx_client: httpx.Client,
     ):
-        super().__init__(token=token, base_url=base_url)
-        self.httpx_client = httpx_client
+        super().__init__(token=token, base_url=base_url, timeout=timeout)
+        self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
     def __init__(
-        self, *, token: typing.Union[str, typing.Callable[[], str]], base_url: str, httpx_client: httpx.AsyncClient
+        self,
+        *,
+        token: typing.Union[str, typing.Callable[[], str]],
+        base_url: str,
+        timeout: typing.Optional[float] = None,
+        httpx_client: httpx.AsyncClient,
     ):
-        super().__init__(token=token, base_url=base_url)
-        self.httpx_client = httpx_client
+        super().__init__(token=token, base_url=base_url, timeout=timeout)
+        self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `nixtla-0.4.0/nixtla/core/datetime_utils.py` & `nixtla-0.5.0/nixtla/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.4.0/nixtla/core/jsonable_encoder.py` & `nixtla-0.5.0/nixtla/core/jsonable_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,45 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-from pydantic import BaseModel
-from pydantic.json import ENCODERS_BY_TYPE
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -59,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -78,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in ENCODERS_BY_TYPE:
-        return ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `nixtla-0.4.0/nixtla/date_features.py` & `nixtla-0.5.0/nixtla/date_features.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.4.0/nixtla/distributed/nixtla_client.py` & `nixtla-0.5.0/nixtla/distributed/nixtla_client.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.4.0/nixtla/nixtla_client.py` & `nixtla-0.5.0/nixtla/nixtla_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import functools
 import inspect
 import json
 import logging
 import os
 import requests
 import warnings
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from functools import partial, wraps
 from multiprocessing import cpu_count
 from concurrent.futures import ThreadPoolExecutor
 from threading import Lock
 
 import numpy as np
@@ -26,26 +26,19 @@
     wait_fixed,
     stop_after_delay,
     RetryCallState,
     retry_if_exception,
     retry_if_not_exception_type,
 )
 from utilsforecast.preprocessing import fill_gaps
-from utilsforecast.processing import (
-    backtest_splits,
-    drop_index_if_pandas,
-    join,
-    maybe_compute_sort_indices,
-    take_rows,
-    vertical_concat,
-)
 
 from .client import Nixtla
 from .core import ApiError
 from .types.multi_series_anomaly import MultiSeriesAnomaly
+from .types.multi_series_cross_validation import MultiSeriesCrossValidation
 from .types.multi_series_forecast import MultiSeriesForecast
 from .types.multi_series_insample_forecast import MultiSeriesInsampleForecast
 from .types.single_series_forecast import SingleSeriesForecast
 
 logging.basicConfig(level=logging.INFO)
 main_logger = logging.getLogger(__name__)
 httpx_logger = logging.getLogger("httpx")
@@ -184,15 +177,14 @@
         self.max_retries = max_retries
         self.retry_interval = retry_interval
         self.max_wait_time = max_wait_time
         # variables defined by each flow
         self.weights_x: pd.DataFrame = None
         self.freq: str = self.base_freq
         self.drop_uid: bool = False
-        self.x_cols: List[str]
         self.input_size: int
         self.model_horizon: int
 
     @staticmethod
     def _prepare_level_and_quantiles(
         level: Optional[List[Union[int, float]]],
         quantiles: Optional[List[float]],
@@ -383,14 +375,39 @@
         return feat_vals
 
     def add_date_features(
         self,
         df: pd.DataFrame,
         X_df: Optional[pd.DataFrame],
     ):
+        # add date features logic
+        if isinstance(self.date_features, list):
+            # user provided list of features
+            date_features = self.date_features
+        elif self.date_features:
+            # try to get default features based on freq
+            date_features = date_features_by_freq.get(self.freq, [])
+            if not date_features:
+                warnings.warn(
+                    f"Non default date features for {self.freq} "
+                    "please pass a list of date features"
+                )
+        else:
+            date_features = []
+        if not date_features:
+            return df, X_df
+
+        if isinstance(self.date_features_to_one_hot, list):
+            date_features_to_one_hot = self.date_features_to_one_hot
+        elif self.date_features_to_one_hot:
+            date_features_to_one_hot = [
+                feat for feat in date_features if not callable(feat)
+            ]
+        else:
+            date_features_to_one_hot = []
         # df contains exogenous variables
         # X_df are the future values of the exogenous variables
         # construct dates
         train_dates = df["ds"].unique().tolist()
         # if we dont have future exogenos variables
         # we need to compute the future dates
         if (self.h is not None) and X_df is None:
@@ -398,23 +415,23 @@
             future_dates = X_df["ds"].unique().tolist()
         elif X_df is not None:
             future_dates = X_df["ds"].unique().tolist()
         else:
             future_dates = []
         dates = pd.DatetimeIndex(np.unique(train_dates + future_dates).tolist())
         date_features_df = pd.DataFrame({"ds": dates})
-        for feature in self.date_features:
+        for feature in date_features:
             feat_df = self.compute_date_feature(dates, feature)
             date_features_df = date_features_df.merge(feat_df, on=["ds"], how="left")
         if df.dtypes["ds"] == "object":
             date_features_df["ds"] = date_features_df["ds"].astype(str)
-        if self.date_features_to_one_hot is not None:
+        if date_features_to_one_hot:
             date_features_df = pd.get_dummies(
                 date_features_df,
-                columns=self.date_features_to_one_hot,
+                columns=date_features_to_one_hot,
                 dtype=int,
             )
         # remove duplicated columns if any
         date_features_df = date_features_df.drop(
             columns=[
                 col
                 for col in date_features_df.columns
@@ -436,42 +453,17 @@
         return X_df
 
     def preprocess_dataframes(
         self,
         df: pd.DataFrame,
         X_df: Optional[pd.DataFrame],
     ):
-        self.infer_freq(df=df)
         """Returns Y_df and X_df dataframes in the structure expected by the endpoints."""
-        # add date features logic
-        if isinstance(self.date_features, bool):
-            if self.date_features:
-                self.date_features = date_features_by_freq.get(self.freq)
-                if self.date_features is None:
-                    warnings.warn(
-                        f"Non default date features for {self.freq} "
-                        "please pass a list of date features"
-                    )
-            else:
-                self.date_features = None
-
-        if self.date_features is not None:
-            if isinstance(self.date_features_to_one_hot, bool):
-                if self.date_features_to_one_hot:
-                    self.date_features_to_one_hot = [
-                        feat for feat in self.date_features if not callable(feat)
-                    ]
-                    self.date_features_to_one_hot = (
-                        None
-                        if not self.date_features_to_one_hot
-                        else self.date_features_to_one_hot
-                    )
-                else:
-                    self.date_features_to_one_hot = None
-            df, X_df = self.add_date_features(df=df, X_df=X_df)
+        self.infer_freq(df=df)
+        df, X_df = self.add_date_features(df=df, X_df=X_df)
         y_cols = ["unique_id", "ds", "y"]
         Y_df = df[y_cols]
         if Y_df["y"].isna().any():
             raise Exception("Your target variable contains NA, please check")
         # Azul: efficient this code
         # and think about returning dates that are not in the training set
         Y_df = self.resample_dataframe(Y_df)
@@ -495,16 +487,15 @@
             X_df = self.preprocess_X_df(X_df)
         elif (X_df is None) and (self.h is None) and (len(y_cols) < df.shape[1]):
             # case for just insample,
             # we dont need h
             X_df = df.drop(columns="y")
             x_cols = X_df.drop(columns=["unique_id", "ds"]).columns.to_list()
             X_df = self.preprocess_X_df(X_df)
-        self.x_cols = x_cols
-        return Y_df, X_df
+        return Y_df, X_df, x_cols
 
     def dataframes_to_dict(self, Y_df: pd.DataFrame, X_df: pd.DataFrame):
         to_dict_args = {"orient": "split"}
         if "index" in inspect.signature(pd.DataFrame.to_dict).parameters:
             to_dict_args["index"] = False
         y = Y_df.to_dict(**to_dict_args)
         x = X_df.to_dict(**to_dict_args) if X_df is not None else None
@@ -526,59 +517,64 @@
         model_params = model_params["detail"]
         self.input_size, self.model_horizon = (
             model_params["input_size"],
             model_params["horizon"],
         )
 
     def validate_input_size(self, Y_df: pd.DataFrame):
-        min_history = Y_df.groupby("unique_id").size().min()
+        min_history = Y_df.groupby("unique_id", observed=True).size().min()
         if min_history < self.input_size + self.model_horizon:
             raise Exception(
                 "Your time series data is too short "
                 "Please be sure that your unique time series contain "
                 f"at least {self.input_size + self.model_horizon} observations"
             )
 
+    def _restrict_input_samples(self) -> int:
+        main_logger.info("Restricting input...")
+        if self.level is not None:
+            # add sufficient info to compute
+            # conformal interval
+            # @AzulGarza
+            #  this is an old opinionated decision
+            #  about reducing the data sent to the api
+            #  to reduce latency when
+            #  a user passes level. since currently the model
+            #  uses conformal prediction, we can change a minimum
+            #  amount of data if the series are too large
+            new_input_size = 3 * self.input_size + max(self.model_horizon, self.h)
+        else:
+            # we only want to forecast
+            new_input_size = self.input_size
+        return new_input_size
+
     def forecast(
         self,
         df: pd.DataFrame,
         X_df: Optional[pd.DataFrame] = None,
         add_history: bool = False,
     ):
         df, X_df = self.transform_inputs(df=df, X_df=X_df)
         main_logger.info("Preprocessing dataframes...")
-        Y_df, X_df = self.preprocess_dataframes(df=df, X_df=X_df)
+        Y_df, X_df, x_cols = self.preprocess_dataframes(df=df, X_df=X_df)
         self.set_model_params()
         if self.h > self.model_horizon:
             main_logger.warning(
                 'The specified horizon "h" exceeds the model horizon. '
                 "This may lead to less accurate forecasts. "
                 "Please consider using a smaller horizon."
             )
         # restrict input if
-        # - we dont want to finetune
-        # - we dont have exogenous regegressors
-        # - and we dont want to produce pred intervals
-        # - no add history
-        restrict_input = (
-            self.finetune_steps == 0
-            and X_df is None
-            and self.level is not None
-            and not add_history
-        )
+        #  we dont want to fine-tune
+        #  we dont have exogenous regressors
+        #  no add history
+        restrict_input = self.finetune_steps == 0 and X_df is None and not add_history
         if restrict_input:
-            # add sufficient info to compute
-            # conformal interval
-            main_logger.info("Restricting input...")
-            new_input_size = 3 * self.input_size + max(self.model_horizon, self.h)
+            new_input_size = self._restrict_input_samples()
             Y_df = Y_df.groupby("unique_id").tail(new_input_size)
-            if X_df is not None:
-                X_df = X_df.groupby("unique_id").tail(
-                    new_input_size + self.h
-                )  # history plus exogenous
         if self.finetune_steps > 0 or self.level is not None:
             self.validate_input_size(Y_df=Y_df)
         y, x = self.dataframes_to_dict(Y_df, X_df)
         main_logger.info("Calling Forecast Endpoint...")
         payload = MultiSeriesForecast(
             y=y,
             x=x,
@@ -593,15 +589,15 @@
         response_timegpt = self._call_api(
             self.client.forecast_multi_series,
             payload,
         )
         if "weights_x" in response_timegpt:
             self.weights_x = pd.DataFrame(
                 {
-                    "features": self.x_cols,
+                    "features": x_cols,
                     "weights": response_timegpt["weights_x"],
                 }
             )
         fcst_df = pd.DataFrame(**response_timegpt["forecast"])
         if add_history:
             main_logger.info("Calling Historical Forecast Endpoint...")
             self.validate_input_size(Y_df=Y_df)
@@ -628,15 +624,15 @@
         # there is a misleading notation here
         # because X_df inputs in the following methods
         # returns X_df outputs that means something different
         # ie X_df = [X_df_history, X_df]
         # exogenous variables are passed after df
         df, _ = self.transform_inputs(df=df, X_df=None)
         main_logger.info("Preprocessing dataframes...")
-        Y_df, X_df = self.preprocess_dataframes(df=df, X_df=None)
+        Y_df, X_df, x_cols = self.preprocess_dataframes(df=df, X_df=None)
         main_logger.info("Calling Anomaly Detector Endpoint...")
         y, x = self.dataframes_to_dict(Y_df, X_df)
         response_timegpt = self._call_api(
             self.client.anomaly_detection_multi_series,
             MultiSeriesAnomaly(
                 y=y,
                 x=x,
@@ -649,82 +645,69 @@
                 clean_ex_first=self.clean_ex_first,
                 model=self.model,
             ),
         )
         if "weights_x" in response_timegpt:
             self.weights_x = pd.DataFrame(
                 {
-                    "features": self.x_cols,
+                    "features": x_cols,
                     "weights": response_timegpt["weights_x"],
                 }
             )
         anomalies_df = pd.DataFrame(**response_timegpt["forecast"])
         anomalies_df = anomalies_df.drop(columns="y")
         anomalies_df = self.transform_outputs(anomalies_df)
         return anomalies_df
 
     def cross_validation(
         self,
         df: pd.DataFrame,
         n_windows: int = 1,
         step_size: Optional[int] = None,
     ):
-        # A: see `transform_inputs`
-        # the code always will return X_df=None
-        # if X_df=None
         df, _ = self.transform_inputs(df=df, X_df=None)
         self.infer_freq(df)
-        df["ds"] = pd.to_datetime(df["ds"])
-        # mlforecast cv code
-        results = []
-        sort_idxs = maybe_compute_sort_indices(df, "unique_id", "ds")
-        if sort_idxs is not None:
-            df = take_rows(df, sort_idxs)
-        splits = backtest_splits(
-            df,
+        df = self.resample_dataframe(df)
+        df, _ = self.add_date_features(df=df, X_df=None)
+        Y_df = df[["unique_id", "ds", "y"]]
+        if Y_df["y"].isna().any():
+            raise Exception("Your target variable contains NA, please check")
+        x_cols = df.columns.drop(Y_df.columns).tolist()
+        self.set_model_params()
+        if x_cols:
+            X_df = df[["unique_id", "ds", *x_cols]]
+            restrict_input = False
+        else:
+            X_df = None
+            restrict_input = True
+        if restrict_input:
+            if step_size is None:
+                step_size = self.h
+            test_size = self.h + step_size * (n_windows - 1)
+            new_input_size = self._restrict_input_samples() + test_size
+            Y_df = Y_df.groupby("unique_id").tail(new_input_size)
+        y, x = self.dataframes_to_dict(Y_df, X_df)
+        main_logger.info("Calling Cross Validation Endpoint...")
+        payload = MultiSeriesCrossValidation(
+            finetune_steps=self.finetune_steps,
+            finetune_loss=self.finetune_loss,
+            freq=self.freq,
+            level=self.level,
+            fh=self.h,
+            y=y,
+            x=x,
             n_windows=n_windows,
-            h=self.h,
-            id_col="unique_id",
-            time_col="ds",
-            freq=pd.tseries.frequencies.to_offset(self.freq),
-            step_size=self.h if step_size is None else step_size,
+            step_size=step_size,
+            clean_ex_first=self.clean_ex_first,
         )
-        for i_window, (cutoffs, train, valid) in enumerate(splits):
-            if len(valid.columns) > 3:
-                # if we have uid, ds, y + exogenous vars
-                train_future = valid.drop(columns="y")
-            else:
-                train_future = None
-            y_pred = self.forecast(
-                df=train,
-                X_df=train_future,
-            )
-            y_pred, _ = self.transform_inputs(df=y_pred, X_df=None)
-            y_pred = join(y_pred, cutoffs, on="unique_id", how="left")
-            y_pred["ds"] = pd.to_datetime(y_pred["ds"])
-            result = join(
-                valid[["unique_id", "ds", "y"]],
-                y_pred,
-                on=["unique_id", "ds"],
-            )
-            if result.shape[0] < valid.shape[0]:
-                raise ValueError(
-                    "Cross validation result produced less results than expected. "
-                    "Please verify that the frequency parameter (freq) matches your series' "
-                    "and that there aren't any missing periods."
-                )
-            results.append(result)
-        out = vertical_concat(results)
-        out = drop_index_if_pandas(out)
-        first_out_cols = ["unique_id", "ds", "cutoff", "y"]
-        remaining_cols = [c for c in out.columns if c not in first_out_cols]
-        fcst_cv_df = out[first_out_cols + remaining_cols]
-        fcst_cv_df["ds"] = fcst_cv_df["ds"].astype(str)
-        fcst_cv_df = self.transform_outputs(fcst_cv_df)
-        return fcst_cv_df
+        response = self._call_api(self.client.cross_validation_multi_series, payload)
+        cv_df = pd.DataFrame(**response["forecast"])
+        cv_df["cutoff"] = pd.to_datetime(cv_df["cutoff"])
+        cv_df = self.transform_outputs(cv_df, level_to_quantiles=True)
+        return cv_df
 
 # %% ../nbs/nixtla_client.ipynb 11
 def validate_model_parameter(func):
     def wrapper(self, *args, **kwargs):
         if "model" in kwargs:
             model = kwargs["model"]
             rename_models_dict = {
@@ -902,14 +885,50 @@
         elif "detail" in validation:
             if "Forecasting! :)" in validation["detail"]:
                 valid = True
         if "support" in validation and log:
             main_logger.info(f'Happy Forecasting! :), {validation["support"]}')
         return valid
 
+    def _uids_to_categorical(
+        self,
+        df: pd.DataFrame,
+        X_df: Optional[pd.DataFrame],
+        id_col: str,
+    ) -> Tuple[pd.DataFrame, Optional[pd.DataFrame], Optional[pd.CategoricalDtype]]:
+        if id_col not in df:
+            return df, X_df, None
+        df = df.copy(deep=False)
+        if isinstance(df[id_col].dtype, pd.CategoricalDtype):
+            dtype = df[id_col].dtype
+        else:
+            dtype = pd.CategoricalDtype(categories=df[id_col].unique())
+            df[id_col] = df[id_col].astype(dtype)
+        df[id_col] = df[id_col].cat.codes
+        if X_df is not None:
+            X_df = X_df.copy(deep=False)
+            if X_df[id_col].dtype != dtype:
+                X_df[id_col] = X_df[id_col].astype(dtype)
+            X_df[id_col] = X_df[id_col].cat.codes
+        return df, X_df, dtype
+
+    def _restore_uids(
+        self,
+        df: pd.DataFrame,
+        dtype: Optional[pd.CategoricalDtype],
+        id_col: str,
+    ) -> pd.DataFrame:
+        if id_col not in df:
+            return df
+        assert dtype is not None
+        df = df.copy(deep=False)
+        code2cat = dict(enumerate(dtype.categories))
+        df[id_col] = df[id_col].map(code2cat)
+        return df
+
     @validate_model_parameter
     @partition_by_uid
     def _forecast(
         self,
         df: pd.DataFrame,
         h: int,
         freq: Optional[str] = None,
@@ -946,17 +965,21 @@
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
+        df, X_df, uids_dtype = self._uids_to_categorical(
+            df=df, X_df=X_df, id_col=id_col
+        )
         fcst_df = nixtla_client_model.forecast(
             df=df, X_df=X_df, add_history=add_history
         )
+        fcst_df = self._restore_uids(fcst_df, dtype=uids_dtype, id_col=id_col)
         self.weights_x = nixtla_client_model.weights_x
         return fcst_df
 
     @validate_model_parameter
     @partition_by_uid
     def _detect_anomalies(
         self,
@@ -987,15 +1010,19 @@
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
+        df, X_df, uids_dtype = self._uids_to_categorical(
+            df=df, X_df=None, id_col=id_col
+        )
         anomalies_df = nixtla_client_model.detect_anomalies(df=df)
+        anomalies_df = self._restore_uids(anomalies_df, dtype=uids_dtype, id_col=id_col)
         self.weights_x = nixtla_client_model.weights_x
         return anomalies_df
 
     @validate_model_parameter
     @partition_by_uid
     def _cross_validation(
         self,
@@ -1035,17 +1062,21 @@
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
+        df, X_df, uids_dtype = self._uids_to_categorical(
+            df=df, X_df=None, id_col=id_col
+        )
         cv_df = nixtla_client_model.cross_validation(
             df=df, n_windows=n_windows, step_size=step_size
         )
+        cv_df = self._restore_uids(cv_df, dtype=uids_dtype, id_col=id_col)
         self.weights_x = nixtla_client_model.weights_x
         return cv_df
 
     def plot(
         self,
         df: pd.DataFrame,
         forecasts_df: Optional[pd.DataFrame] = None,
```

### Comparing `nixtla-0.4.0/nixtla/types/__init__.py` & `nixtla-0.5.0/nixtla/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .http_validation_error import HttpValidationError
+from .model import Model
 from .multi_series_anomaly import MultiSeriesAnomaly
-from .multi_series_anomaly_model import MultiSeriesAnomalyModel
 from .multi_series_cross_validation import MultiSeriesCrossValidation
 from .multi_series_cross_validation_fewshot_loss import MultiSeriesCrossValidationFewshotLoss
 from .multi_series_cross_validation_finetune_loss import MultiSeriesCrossValidationFinetuneLoss
-from .multi_series_cross_validation_model import MultiSeriesCrossValidationModel
 from .multi_series_forecast import MultiSeriesForecast
 from .multi_series_forecast_fewshot_loss import MultiSeriesForecastFewshotLoss
 from .multi_series_forecast_finetune_loss import MultiSeriesForecastFinetuneLoss
-from .multi_series_forecast_model import MultiSeriesForecastModel
 from .multi_series_input import MultiSeriesInput
 from .multi_series_insample_forecast import MultiSeriesInsampleForecast
-from .multi_series_insample_forecast_model import MultiSeriesInsampleForecastModel
 from .single_series_forecast import SingleSeriesForecast
 from .single_series_forecast_fewshot_loss import SingleSeriesForecastFewshotLoss
 from .single_series_forecast_finetune_loss import SingleSeriesForecastFinetuneLoss
-from .single_series_forecast_model import SingleSeriesForecastModel
 from .single_series_insample_forecast import SingleSeriesInsampleForecast
-from .single_series_insample_forecast_model import SingleSeriesInsampleForecastModel
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "HttpValidationError",
+    "Model",
     "MultiSeriesAnomaly",
-    "MultiSeriesAnomalyModel",
     "MultiSeriesCrossValidation",
     "MultiSeriesCrossValidationFewshotLoss",
     "MultiSeriesCrossValidationFinetuneLoss",
-    "MultiSeriesCrossValidationModel",
     "MultiSeriesForecast",
     "MultiSeriesForecastFewshotLoss",
     "MultiSeriesForecastFinetuneLoss",
-    "MultiSeriesForecastModel",
     "MultiSeriesInput",
     "MultiSeriesInsampleForecast",
-    "MultiSeriesInsampleForecastModel",
     "SingleSeriesForecast",
     "SingleSeriesForecastFewshotLoss",
     "SingleSeriesForecastFinetuneLoss",
-    "SingleSeriesForecastModel",
     "SingleSeriesInsampleForecast",
-    "SingleSeriesInsampleForecastModel",
     "ValidationError",
     "ValidationErrorLocItem",
 ]
```

### Comparing `nixtla-0.4.0/nixtla/types/http_validation_error.py` & `nixtla-0.5.0/nixtla/types/http_validation_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .validation_error import ValidationError
 
 
-class HttpValidationError(pydantic.BaseModel):
-    detail: typing.Optional[typing.List[ValidationError]]
+class HttpValidationError(pydantic_v1.BaseModel):
+    detail: typing.Optional[typing.List[ValidationError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla/types/multi_series_anomaly.py` & `nixtla-0.5.0/nixtla/types/single_series_insample_forecast.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
-from .multi_series_anomaly_model import MultiSeriesAnomalyModel
-from .multi_series_input import MultiSeriesInput
+from ..core.pydantic_utilities import pydantic_v1
+from .model import Model
 
 
-class MultiSeriesAnomaly(pydantic.BaseModel):
-    model: typing.Optional[MultiSeriesAnomalyModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
-    )
-    freq: typing.Optional[str] = pydantic.Field(
-        description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
-    )
-    level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
-        description="Specifies the confidence level for the prediction interval used in anomaly detection. It is represented as a percentage between 0 and 100. For instance, a level of 95 indicates that the generated prediction interval captures the true future observation 95% of the time. Any observed values outside of this interval would be considered anomalies. A higher level leads to wider prediction intervals and potentially fewer detected anomalies, whereas a lower level results in narrower intervals and potentially more detected anomalies. Default: 99."
-    )
-    y: typing.Optional[typing.Any]
-    x: typing.Optional[MultiSeriesInput] = pydantic.Field(
-        description='The exogenous  variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.'
-    )
-    clean_ex_first: typing.Optional[bool] = pydantic.Field(
-        description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
-    )
+class SingleSeriesInsampleForecast(pydantic_v1.BaseModel):
+    model: typing.Optional[Model] = pydantic_v1.Field(default=None)
+    """
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    """
+
+    freq: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available.
+    """
+
+    level: typing.Optional[typing.List[typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals.
+    """
+
+    y: typing.Optional[typing.Any] = None
+    x: typing.Optional[typing.Any] = None
+    clean_ex_first: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla/types/multi_series_cross_validation.py` & `nixtla-0.5.0/nixtla/types/multi_series_cross_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,88 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .model import Model
 from .multi_series_cross_validation_fewshot_loss import MultiSeriesCrossValidationFewshotLoss
 from .multi_series_cross_validation_finetune_loss import MultiSeriesCrossValidationFinetuneLoss
-from .multi_series_cross_validation_model import MultiSeriesCrossValidationModel
 from .multi_series_input import MultiSeriesInput
 
 
-class MultiSeriesCrossValidation(pydantic.BaseModel):
-    fewshot_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use finetune_steps instead.")
-    fewshot_loss: typing.Optional[MultiSeriesCrossValidationFewshotLoss] = pydantic.Field(
-        description="Deprecated. Please use finetune_loss instead."
-    )
-    model: typing.Optional[MultiSeriesCrossValidationModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
-    )
-    freq: typing.Optional[str] = pydantic.Field(
-        description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
-    )
-    level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
-        description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
-    )
-    fh: typing.Optional[int] = pydantic.Field(
-        description="The forecasting horizon. This represents the number of time steps into the future that the forecast should predict."
-    )
-    y: typing.Optional[typing.Any]
-    x: typing.Optional[MultiSeriesInput] = pydantic.Field(
-        description='The exogenous  variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.'
-    )
-    n_windows: typing.Optional[int] = pydantic.Field(description="Number of windows to evaluate.")
-    step_size: typing.Optional[int] = pydantic.Field(
-        description="Step size between each cross validation window. If None it will be equal to the forecasting horizon."
-    )
-    clean_ex_first: typing.Optional[bool] = pydantic.Field(
-        description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
-    )
-    finetune_steps: typing.Optional[int] = pydantic.Field(
-        description="The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning."
-    )
-    finetune_loss: typing.Optional[MultiSeriesCrossValidationFinetuneLoss] = pydantic.Field(
-        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
-    )
+class MultiSeriesCrossValidation(pydantic_v1.BaseModel):
+    fewshot_steps: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Deprecated. Please use finetune_steps instead.
+    """
+
+    fewshot_loss: typing.Optional[MultiSeriesCrossValidationFewshotLoss] = pydantic_v1.Field(default=None)
+    """
+    Deprecated. Please use finetune_loss instead.
+    """
+
+    model: typing.Optional[Model] = pydantic_v1.Field(default=None)
+    """
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    """
+
+    freq: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available.
+    """
+
+    level: typing.Optional[typing.List[typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals.
+    """
+
+    fh: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The forecasting horizon. This represents the number of time steps into the future that the forecast should predict.
+    """
+
+    y: typing.Optional[typing.Any] = None
+    x: typing.Optional[MultiSeriesInput] = pydantic_v1.Field(default=None)
+    """
+    The exogenous variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.
+    """
+
+    n_windows: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Number of windows to evaluate.
+    """
+
+    step_size: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Step size between each cross validation window. If None it will be equal to the forecasting horizon.
+    """
+
+    clean_ex_first: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model.
+    """
+
+    finetune_steps: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning.
+    """
+
+    finetune_loss: typing.Optional[MultiSeriesCrossValidationFinetuneLoss] = pydantic_v1.Field(default=None)
+    """
+    The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla/types/multi_series_forecast.py` & `nixtla-0.5.0/nixtla/types/multi_series_forecast.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,78 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .model import Model
 from .multi_series_forecast_fewshot_loss import MultiSeriesForecastFewshotLoss
 from .multi_series_forecast_finetune_loss import MultiSeriesForecastFinetuneLoss
-from .multi_series_forecast_model import MultiSeriesForecastModel
 from .multi_series_input import MultiSeriesInput
 
 
-class MultiSeriesForecast(pydantic.BaseModel):
-    fewshot_steps: typing.Optional[int] = pydantic.Field(description="Deprecated. Please use finetune_steps instead.")
-    fewshot_loss: typing.Optional[MultiSeriesForecastFewshotLoss] = pydantic.Field(
-        description="Deprecated. Please use finetune_loss instead."
-    )
-    model: typing.Optional[MultiSeriesForecastModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
-    )
-    freq: typing.Optional[str] = pydantic.Field(
-        description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
-    )
-    level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
-        description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
-    )
-    fh: typing.Optional[int] = pydantic.Field(
-        description="The forecasting horizon. This represents the number of time steps into the future that the forecast should predict."
-    )
-    y: typing.Optional[typing.Any]
-    x: typing.Optional[MultiSeriesInput] = pydantic.Field(
-        description='The exogenous  variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.'
-    )
-    clean_ex_first: typing.Optional[bool] = pydantic.Field(
-        description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
-    )
-    finetune_steps: typing.Optional[int] = pydantic.Field(
-        description="The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning."
-    )
-    finetune_loss: typing.Optional[MultiSeriesForecastFinetuneLoss] = pydantic.Field(
-        description="The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers."
-    )
+class MultiSeriesForecast(pydantic_v1.BaseModel):
+    fewshot_steps: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Deprecated. Please use finetune_steps instead.
+    """
+
+    fewshot_loss: typing.Optional[MultiSeriesForecastFewshotLoss] = pydantic_v1.Field(default=None)
+    """
+    Deprecated. Please use finetune_loss instead.
+    """
+
+    model: typing.Optional[Model] = pydantic_v1.Field(default=None)
+    """
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    """
+
+    freq: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available.
+    """
+
+    level: typing.Optional[typing.List[typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals.
+    """
+
+    fh: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The forecasting horizon. This represents the number of time steps into the future that the forecast should predict.
+    """
+
+    y: typing.Optional[typing.Any] = None
+    x: typing.Optional[MultiSeriesInput] = pydantic_v1.Field(default=None)
+    """
+    The exogenous variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.
+    """
+
+    clean_ex_first: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model.
+    """
+
+    finetune_steps: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The number of tuning steps used to train the large time model on the data. Set this value to 0 for zero-shot inference, i.e., to make predictions without any further model tuning.
+    """
+
+    finetune_loss: typing.Optional[MultiSeriesForecastFinetuneLoss] = pydantic_v1.Field(default=None)
+    """
+    The loss used to train the large time model on the data. Select from ['default', 'mae', 'mse', 'rmse', 'mape', 'smape']. It will only be used if finetune_steps larger than 0. Default is a robust loss function that is less sensitive to outliers.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla/types/multi_series_input.py` & `nixtla-0.5.0/nixtla/types/multi_series_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
 
-class MultiSeriesInput(pydantic.BaseModel):
+class MultiSeriesInput(pydantic_v1.BaseModel):
     columns: typing.List[str]
     data: typing.List[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla/types/multi_series_insample_forecast.py` & `nixtla-0.5.0/nixtla/types/multi_series_insample_forecast.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .model import Model
 from .multi_series_input import MultiSeriesInput
-from .multi_series_insample_forecast_model import MultiSeriesInsampleForecastModel
 
 
-class MultiSeriesInsampleForecast(pydantic.BaseModel):
-    model: typing.Optional[MultiSeriesInsampleForecastModel] = pydantic.Field(
-        description="Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data."
-    )
-    freq: typing.Optional[str] = pydantic.Field(
-        description="The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available."
-    )
-    level: typing.Optional[typing.List[typing.Any]] = pydantic.Field(
-        description="A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals."
-    )
-    y: typing.Optional[typing.Any]
-    x: typing.Optional[MultiSeriesInput] = pydantic.Field(
-        description='The exogenous  variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.'
-    )
-    clean_ex_first: typing.Optional[bool] = pydantic.Field(
-        description="A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model."
-    )
+class MultiSeriesInsampleForecast(pydantic_v1.BaseModel):
+    model: typing.Optional[Model] = pydantic_v1.Field(default=None)
+    """
+    Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon.` We recommend using `timegpt-1-long-horizon` for forecasting if you want to predict more than one seasonal period given the frequency of your data.
+    """
+
+    freq: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The frequency of the data represented as a string. 'D' for daily, 'M' for monthly, 'H' for hourly, and 'W' for weekly frequencies are available.
+    """
+
+    level: typing.Optional[typing.List[typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    A list of values representing the prediction intervals. Each value is a percentage that indicates the level of certainty for the corresponding prediction interval. For example, [80, 90] defines 80% and 90% prediction intervals.
+    """
+
+    y: typing.Optional[typing.Any] = None
+    x: typing.Optional[MultiSeriesInput] = pydantic_v1.Field(default=None)
+    """
+    The exogenous variables provided as a dictionary of two colums: columns and data. The columns contains the columns of the dataframe and data contains eaach data point. For example: {"columns": ["unique_id", "ds", "ex_1", "ex_2"], "data": [["ts_0", "2021-01-01", 0.2, 0.67], ["ts_0", "2021-01-02", 0.4, 0.7]}. This should also include forecasting horizon (fh) additional timestamps for each unique_id to calculate the future values.
+    """
+
+    clean_ex_first: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    A boolean flag that indicates whether the API should preprocess (clean) the exogenous signal before applying the large time model. If True, the exogenous signal is cleaned; if False, the exogenous variables are applied after the large time model.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla/types/validation_error.py` & `nixtla-0.5.0/nixtla/types/validation_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class ValidationError(pydantic.BaseModel):
+class ValidationError(pydantic_v1.BaseModel):
     loc: typing.List[ValidationErrorLocItem]
     msg: str
     type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `nixtla-0.4.0/nixtla.egg-info/PKG-INFO` & `nixtla-0.5.0/nixtla.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: nixtla
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: pandas
-Requires-Dist: pydantic<2
+Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: tenacity
 Requires-Dist: utilsforecast>=0.1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
 Requires-Dist: statsforecast; extra == "dev"
+Requires-Dist: hierarchicalforecast; extra == "dev"
 Requires-Dist: dask[dataframe]; extra == "dev"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "dev"
 Requires-Dist: pyspark; extra == "dev"
 Requires-Dist: ray[serve-grpc]; extra == "dev"
 Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "dev"
 Requires-Dist: holidays; extra == "dev"
 Provides-Extra: distributed
@@ -71,26 +72,26 @@
 With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtla>=0.1.0
+pip install nixtla>=0.4.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
 from nixtla import NixtlaClient
-nixtla = NixtlaClient(
+nixtla_client = NixtlaClient(
     # defaults to os.environ.get("NIXTLA_API_KEY")
     api_key = 'my_api_key_provided_by_nixtla'
 )
-fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
+fcst_df = nixtla_client.forecast(df, h=24, level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtla-0.4.0/nixtla.egg-info/SOURCES.txt` & `nixtla-0.5.0/nixtla.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,36 +13,35 @@
 nixtla.egg-info/dependency_links.txt
 nixtla.egg-info/requires.txt
 nixtla.egg-info/top_level.txt
 nixtla/core/__init__.py
 nixtla/core/api_error.py
 nixtla/core/client_wrapper.py
 nixtla/core/datetime_utils.py
+nixtla/core/file.py
+nixtla/core/http_client.py
 nixtla/core/jsonable_encoder.py
+nixtla/core/pydantic_utilities.py
 nixtla/core/remove_none_from_dict.py
+nixtla/core/request_options.py
 nixtla/distributed/__init__.py
 nixtla/distributed/nixtla_client.py
 nixtla/errors/__init__.py
 nixtla/errors/unprocessable_entity_error.py
 nixtla/types/__init__.py
 nixtla/types/http_validation_error.py
+nixtla/types/model.py
 nixtla/types/multi_series_anomaly.py
-nixtla/types/multi_series_anomaly_model.py
 nixtla/types/multi_series_cross_validation.py
 nixtla/types/multi_series_cross_validation_fewshot_loss.py
 nixtla/types/multi_series_cross_validation_finetune_loss.py
-nixtla/types/multi_series_cross_validation_model.py
 nixtla/types/multi_series_forecast.py
 nixtla/types/multi_series_forecast_fewshot_loss.py
 nixtla/types/multi_series_forecast_finetune_loss.py
-nixtla/types/multi_series_forecast_model.py
 nixtla/types/multi_series_input.py
 nixtla/types/multi_series_insample_forecast.py
-nixtla/types/multi_series_insample_forecast_model.py
 nixtla/types/single_series_forecast.py
 nixtla/types/single_series_forecast_fewshot_loss.py
 nixtla/types/single_series_forecast_finetune_loss.py
-nixtla/types/single_series_forecast_model.py
 nixtla/types/single_series_insample_forecast.py
-nixtla/types/single_series_insample_forecast_model.py
 nixtla/types/validation_error.py
 nixtla/types/validation_error_loc_item.py
```

### Comparing `nixtla-0.4.0/setup.py` & `nixtla-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,37 +7,38 @@
     "black",
     "datasetsforecast",
     "nbdev",
     "plotly",
     "pre-commit",
     "python-dotenv",
     "statsforecast",
+    "hierarchicalforecast",
 ]
 distributed = ["dask[dataframe]", "fugue[ray]>=0.8.7", "pyspark", "ray[serve-grpc]"]
 plotting = ["utilsforecast[plotting]>=0.1.7"]
 date_extras = ["holidays"]
 
 setuptools.setup(
     name="nixtla",
-    version="0.4.0",
+    version="0.5.0",
     description="Python SDK for Nixtla API (TimeGPT)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/nixtla",
     packages=setuptools.find_packages(exclude=["action_files"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     install_requires=[
         "httpx",
         "pandas",
-        "pydantic<2",
+        "pydantic",
         "requests",
         "tenacity",
         "utilsforecast>=0.1.7",
     ],
     extras_require={
         "dev": dev + distributed + plotting + date_extras,
         "distributed": distributed,
```

