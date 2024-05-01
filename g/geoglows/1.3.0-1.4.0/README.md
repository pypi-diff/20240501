# Comparing `tmp/geoglows-1.3.0.tar.gz` & `tmp/geoglows-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.3.0.tar", last modified: Thu Apr 25 14:44:51 2024, max compression
+gzip compressed data, was "geoglows-1.4.0.tar", last modified: Wed May  1 04:46:45 2024, max compression
```

## Comparing `geoglows-1.3.0.tar` & `geoglows-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.527587 geoglows-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-25 14:44:43.000000 geoglows-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 14:44:43.000000 geoglows-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 14:44:51.527587 geoglows-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 14:44:43.000000 geoglows-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.523587 geoglows-1.3.0/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.527587 geoglows-1.3.0/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-25 14:44:43.000000 geoglows-1.3.0/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:44:51.527587 geoglows-1.3.0/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 14:44:51.000000 geoglows-1.3.0/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-25 14:44:43.000000 geoglows-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:44:51.527587 geoglows-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-25 14:44:43.000000 geoglows-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-01 04:46:41.000000 geoglows-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 04:46:41.000000 geoglows-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-01 04:46:45.913283 geoglows-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-01 04:46:41.000000 geoglows-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-01 04:46:41.000000 geoglows-1.4.0/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:46:45.913283 geoglows-1.4.0/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 04:46:45.000000 geoglows-1.4.0/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 04:46:41.000000 geoglows-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:46:45.917284 geoglows-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 04:46:41.000000 geoglows-1.4.0/setup.py
```

### Comparing `geoglows-1.3.0/LICENSE` & `geoglows-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/PKG-INFO` & `geoglows-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.3.0
+Version: 1.4.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Requires-Python: >=3.10.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dask>=2024
+Requires-Dist: dask>=2022
 Requires-Dist: fastparquet
 Requires-Dist: requests
 Requires-Dist: pandas>=1
 Requires-Dist: plotly>=5
 Requires-Dist: scipy>=1
-Requires-Dist: s3fs>=2024
+Requires-Dist: s3fs>=2022
 Requires-Dist: numpy>=1
 Requires-Dist: hydrostats
 Requires-Dist: HydroErr
-Requires-Dist: xarray>=2024
+Requires-Dist: xarray>=2022
 Requires-Dist: zarr
 
 # GEOGLOWS
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoglows.svg)](https://anaconda.org/conda-forge/geoglows)
 [![PyPI](https://img.shields.io/pypi/v/geoglows)](https://pypi.org/project/geoglows)
```

### Comparing `geoglows-1.3.0/README.md` & `geoglows-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/__init__.py` & `geoglows-1.4.0/geoglows/_plots/__init__.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/format_tools.py` & `geoglows-1.4.0/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.4.0/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.4.0/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/plotly_helpers.py` & `geoglows-1.4.0/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.4.0/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/_plots/plots.py` & `geoglows-1.4.0/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/analyze.py` & `geoglows-1.4.0/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/bias.py` & `geoglows-1.4.0/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/data.py` & `geoglows-1.4.0/geoglows/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,17 +53,18 @@
 
         return_format = kwargs.get('format', 'df')
         assert return_format in ('df', 'xarray'), f'Unsupported return format requested: {return_format}'
 
         s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
         date = kwargs.get('date', False)
         if not date:
-            dates = sorted([x.split('/')[-1] for x in s3.ls(ODP_FORECAST_S3_BUCKET_URI)], reverse=True)
-            dates = [x.split('.')[0] for x in dates if x.endswith('.zarr')]  # ignore the index.html file
-            dates = [x.replace('00.zarr', '') for x in dates]
+            zarr_vars = ['rivid', 'Qout', 'time', 'ensemble']
+            dates = [s3.glob(os.path.join(ODP_FORECAST_S3_BUCKET_URI, f'*.zarr/{var}')) for var in zarr_vars]
+            dates = [set([d.split('/')[1].replace('.zarr', '') for d in date]) for date in dates]
+            dates = sorted(set.intersection(*dates), reverse=True)
             if product_name == 'dates':
                 return pd.DataFrame(dict(dates=dates))
             date = dates[0]
         if len(date) == 8:
             date = f'{date}00.zarr'
         elif len(date) == 10:
             date = f'{date}.zarr'
@@ -117,15 +118,15 @@
         # parse out the information necessary to build a request url
         endpoint = kwargs.get('endpoint', DEFAULT_REST_ENDPOINT)
         endpoint = endpoint[:-1] if endpoint[-1] == '/' else endpoint
         endpoint = endpoint + '/api' if not endpoint.endswith('/api') else endpoint
         endpoint = f'https://{endpoint}' if not endpoint.startswith(('https://', 'http://')) else endpoint
 
         version = kwargs.get('version', DEFAULT_REST_ENDPOINT_VERSION)
-        assert version in ('v2', ), ValueError(f'Unrecognized model version parameter: {version}')
+        assert version in ('v2',), ValueError(f'Unrecognized model version parameter: {version}')
 
         product_name = function.__name__.replace("_", "").lower()
 
         river_id = args[0] if len(args) > 0 else None
         river_id = kwargs.get('river_id', '') if not river_id else river_id
         if isinstance(river_id, list):
             raise ValueError('Multiple river_ids are not available via REST API or on v1. '
@@ -176,14 +177,15 @@
 
     def main(*args, **kwargs):
         source = kwargs.get('data_source', 'aws')
         assert source in ('rest', 'aws'), ValueError(f'Unrecognized data source requested: {source}')
         if source == 'rest':
             return from_rest(*args, **kwargs)
         return from_aws(*args, **kwargs)
+
     main.__doc__ = function.__doc__  # necessary for code documentation auto generators
     return main
 
 
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
@@ -292,19 +294,14 @@
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/retrospective.zarr', s3=s3, check=False)
     ds = xr.open_zarr(s3store).sel(rivid=river_id)
     if format == 'xarray':
         return ds
     return ds.to_dataframe().reset_index().set_index('time').pivot(columns='rivid', values='Qout')
 
 
-def historical(*args, **kwargs):
-    """Alias for retrospective"""
-    return retrospective(*args, **kwargs)
-
-
 def daily_averages(river_id: int or list) -> pd.DataFrame:
     """
     Retrieves daily average streamflow for a given river_id
 
     Args:
         river_id (int): the ID of a stream, should be a 9 digit integer
 
@@ -339,32 +336,40 @@
     Returns:
         pd.DataFrame
     """
     df = retrospective(river_id)
     return calc_annual_averages(df)
 
 
-def return_periods(river_id: int or list, format: str = 'df') -> pd.DataFrame or xr.Dataset:
+def return_periods(river_id: int or list, format: str = 'df', method: str = 'gumbel1') -> pd.DataFrame or xr.Dataset:
     """
     Retrieves the return period thresholds based on a specified historic simulation forcing on a certain river_id.
 
     Args:
         river_id (int): the ID of a stream, should be a 9 digit integer
         format (str): the format to return the data, either 'df' or 'xarray'. default is 'df'
+        method (str): the method to use to estimate the return period thresholds. default is 'gumbel1'
+
+    Changelog:
+        v1.4.0: adds method parameter for future expansion of multiple return period methods
 
     Returns:
         pd.DataFrame
     """
+    rp_methods = {
+        'gumbel1': 'gumbel1_return_period',
+    }
+    assert method in rp_methods, f'Unrecognized return period estimation method given: {method}'
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/return-periods.zarr', s3=s3, check=False)
     ds = xr.open_zarr(s3store).sel(rivid=river_id)
     if format == 'xarray':
         return ds
-    return (ds['return_period_flow'].to_dataframe().reset_index()
-            .pivot(index='rivid', columns='return_period', values='return_period_flow'))
+    return (ds[rp_methods[method]].to_dataframe().reset_index()
+            .pivot(index='rivid', columns='return_period', values=rp_methods[method]))
 
 
 # model config and supplementary data
 def metadata_tables(columns: list = None) -> pd.DataFrame:
     """
     Retrieves the master table of rivers metadata and properties as a pandas DataFrame
     Args:
```

### Comparing `geoglows-1.3.0/geoglows/streamflow.py` & `geoglows-1.4.0/geoglows/streamflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.forecast_stats(12341234)
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'ForecastStats/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return f'{endpoint}{method}?reach_id={reach_id}'
     params = {'reach_id': reach_id, 'return_format': return_format}
     if forecast_date is not None:
@@ -109,15 +109,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.forecast_warnings('australia-geoglows')
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'ForecastWarnings/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return endpoint + method + f'?region={region}'
 
     # return the requested data
@@ -144,15 +144,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.forecast_warnings('australia-geoglows')
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'ForecastRecords/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return f'{endpoint}{method}?reach_id={reach_id}'
 
     params = {'reach_id': reach_id, 'return_format': return_format}
@@ -184,15 +184,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.historic_simulation(12341234)
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'HistoricSimulation/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return f'{endpoint}{method}?reach_id={reach_id}&forcing={forcing}'
 
     # return the requested data
@@ -219,15 +219,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.seasonal_average(12341234)
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'DailyAverages/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return f'{endpoint}{method}?reach_id={reach_id}&forcing={forcing}'
 
     # return the requested data
@@ -254,15 +254,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.seasonal_average(12341234)
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'MonthlyAverages/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return f'{endpoint}{method}?reach_id={reach_id}&forcing={forcing}'
 
     # return the requested data
@@ -289,15 +289,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.return_periods(12341234)
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'ReturnPeriods/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return f'{endpoint}{method}?reach_id={reach_id}&forcing={forcing}'
 
     # return the requested data
@@ -320,15 +320,15 @@
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.available_data()
 
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'AvailableData/'
 
     # if you only wanted the url, quit here
     if return_format == 'url':
         return endpoint + method
 
     # return the requested data
@@ -352,15 +352,15 @@
         - return_format='url' returns a url string for using in a request or web browser
 
     Example:
         .. code-block:: python
 
             data = streamflow.rst.available_dates(12341234)
     """
-    warnings.warn(DEPRECATIONWARNING, DeprecationWarning)
+    warnings.warn(DEPRECATIONWARNING, DeprecationWarning, stacklevel=2)
     method = 'AvailableDates/'
 
     # you need a region for the api call, so the user needs to provide one or a valid reach_id to get it from
     params = {'region': 'africa-geoglows'}
     # if you only wanted the url, quit here
     if return_format == 'url':
         return endpoint + method
```

### Comparing `geoglows-1.3.0/geoglows/streams.py` & `geoglows-1.4.0/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows/tables.py` & `geoglows-1.4.0/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/geoglows.egg-info/PKG-INFO` & `geoglows-1.4.0/geoglows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.3.0
+Version: 1.4.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Requires-Python: >=3.10.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dask>=2024
+Requires-Dist: dask>=2022
 Requires-Dist: fastparquet
 Requires-Dist: requests
 Requires-Dist: pandas>=1
 Requires-Dist: plotly>=5
 Requires-Dist: scipy>=1
-Requires-Dist: s3fs>=2024
+Requires-Dist: s3fs>=2022
 Requires-Dist: numpy>=1
 Requires-Dist: hydrostats
 Requires-Dist: HydroErr
-Requires-Dist: xarray>=2024
+Requires-Dist: xarray>=2022
 Requires-Dist: zarr
 
 # GEOGLOWS
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)](https://img.shields.io/conda/vn/conda-forge/geoglows.svg)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoglows.svg)](https://anaconda.org/conda-forge/geoglows)
 [![PyPI](https://img.shields.io/pypi/v/geoglows)](https://pypi.org/project/geoglows)
```

### Comparing `geoglows-1.3.0/geoglows.egg-info/SOURCES.txt` & `geoglows-1.4.0/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.3.0/setup.py` & `geoglows-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 NAME = 'geoglows'
 DESCRIPTION = 'Package for accessing data from the GEOGLOWS Hydrological Model'
 URL = 'https://data.geoglows.org'
 AUTHOR = 'Riley Hales PhD'
-REQUIRES_PYTHON = '>=3.10.0'
+REQUIRES_PYTHON = '>=3.7.0'
 LICENSE = 'BSD 3-Clause Clear License'
 
 with open("README.md", "r") as readme:
     LONG_DESCRIPTION = readme.read()
 
 with open(f'./{NAME}/__init__.py') as f:
     version_pattern = r'__version__ = [\'"](.+)[\'"]'
```

