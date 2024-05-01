# Comparing `tmp/intake-nwp-0.3.4.tar.gz` & `tmp/intake_nwp-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-nwp-0.3.4.tar", last modified: Tue Dec  5 04:40:55 2023, max compression
+gzip compressed data, was "intake_nwp-0.3.5.tar", last modified: Wed May  1 05:31:40 2024, max compression
```

## Comparing `intake-nwp-0.3.4.tar` & `intake_nwp-0.3.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 04:40:55.454812 intake-nwp-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-12-05 04:40:55.450812 intake-nwp-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 04:40:55.450812 intake-nwp-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 04:40:55.450812 intake-nwp-0.3.4/intake_nwp/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/intake_nwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/intake_nwp/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 04:40:55.450812 intake-nwp-0.3.4/intake_nwp/source/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/intake_nwp/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/intake_nwp/source/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13851 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/intake_nwp/source/nwp.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/intake_nwp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 04:40:55.450812 intake-nwp-0.3.4/intake_nwp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-12-05 04:40:55.000000 intake-nwp-0.3.4/intake_nwp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-12-05 04:40:55.000000 intake-nwp-0.3.4/intake_nwp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 04:40:55.000000 intake-nwp-0.3.4/intake_nwp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-05 04:40:55.000000 intake-nwp-0.3.4/intake_nwp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-05 04:40:55.000000 intake-nwp-0.3.4/intake_nwp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-05 04:40:55.000000 intake-nwp-0.3.4/intake_nwp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 04:40:55.454812 intake-nwp-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 04:40:55.450812 intake-nwp-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/tests/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-12-05 04:39:12.000000 intake-nwp-0.3.4/tests/test_nwp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:31:40.403305 intake_nwp-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-01 05:31:40.403305 intake_nwp-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:31:40.399305 intake_nwp-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:31:40.399305 intake_nwp-0.3.5/intake_nwp/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/intake_nwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/intake_nwp/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:31:40.403305 intake_nwp-0.3.5/intake_nwp/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/intake_nwp/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/intake_nwp/source/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/intake_nwp/source/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/intake_nwp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:31:40.403305 intake_nwp-0.3.5/intake_nwp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-01 05:31:40.000000 intake_nwp-0.3.5/intake_nwp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-01 05:31:40.000000 intake_nwp-0.3.5/intake_nwp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:31:40.000000 intake_nwp-0.3.5/intake_nwp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 05:31:40.000000 intake_nwp-0.3.5/intake_nwp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 05:31:40.000000 intake_nwp-0.3.5/intake_nwp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 05:31:40.000000 intake_nwp-0.3.5/intake_nwp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:31:40.403305 intake_nwp-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:31:40.403305 intake_nwp-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/tests/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-01 05:30:34.000000 intake_nwp-0.3.5/tests/test_nwp.py
```

### Comparing `intake-nwp-0.3.4/CONTRIBUTING.rst` & `intake_nwp-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/LICENSE` & `intake_nwp-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/PKG-INFO` & `intake_nwp-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-nwp
-Version: 0.3.4
+Version: 0.3.5
 Summary: Intake drivers for numerical weather prediction data
 Author-email: Oceanum Developers <developers@oceanum.science>
 Maintainer-email: Oceanum Developers <developers@oceanum.science>
 License: MIT License
         
         Copyright (c) 2022, Oceanum Developers
         
@@ -47,14 +47,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: click
 Requires-Dist: cartopy
 Requires-Dist: cfgrib
 Requires-Dist: herbie-data
 Requires-Dist: intake
+Requires-Dist: jinja2
 Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: extra
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `intake-nwp-0.3.4/docs/Makefile` & `intake_nwp-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/docs/conf.py` & `intake_nwp-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/docs/installation.rst` & `intake_nwp-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/docs/make.bat` & `intake_nwp-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/intake_nwp/source/base.py` & `intake_nwp-0.3.5/intake_nwp/source/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
-from intake.source.base import CacheMixin, PersistMixin, DataSourceBase
+from intake.source.base import DataSource
 
 
 logger = logging.getLogger(__name__)
 
 
-class DataSourceMixin(CacheMixin, PersistMixin, DataSourceBase):
+class DataSourceBase(DataSource):
     """Base behaviours for plugins in this repo."""
 
     container = "xarray"
     partition_access = True
 
     def _get_schema(self):
         """Make schema object, which embeds xarray object and some details"""
         from intake.source.base import Schema
 
         if self._ds is None:
             self._open_dataset()
 
             metadata = {
-                "dims": dict(self._ds.dims),
+                "dims": dict(self._ds.sizes),
                 "data_vars": {
                     k: list(self._ds[k].coords) for k in self._ds.data_vars.keys()
                 },
                 "coords": tuple(self._ds.coords.keys()),
             }
             metadata.update(self._ds.attrs)
             self._schema = Schema(
```

### Comparing `intake-nwp-0.3.4/intake_nwp/source/nwp.py` & `intake_nwp-0.3.5/intake_nwp/source/nwp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import numpy as np
 import pandas as pd
 from datetime import datetime, timedelta
 from typing import Union, Literal
 
-from intake_nwp.source import DataSourceMixin
+from intake_nwp.source import DataSourceBase
 from intake_nwp.utils import round_time
 
 
 logger = logging.getLogger(__name__)
 
 
-class ForecastSource(DataSourceMixin):
+class ForecastSource(DataSourceBase):
     """Forecast data source.
 
     This driver opens a forecast dataset using the Herbies package.
 
     Parameters
     ----------
     model: str
@@ -69,28 +69,30 @@
         stepback=1,
         priority=["google", "aws", "nomads", "azure"],
         max_threads=None,
         mapping={},
         sorted=False,
         metadata=None,
         check_inventory=True,
+        verbose=False,
         **kwargs
     ):
         super().__init__(metadata=metadata, **kwargs)
 
         self.model = model
         self.product = product
         self.pattern = pattern
         self.cycle = cycle
         self.cycle_step = cycle_step
         self.stepback = stepback
         self.priority = priority
         self.mapping = mapping
         self.sorted = sorted
         self.check_inventory = check_inventory
+        self.verbose=verbose
 
         self._fxx = fxx
         self._stepback = 0
         self._max_threads = max_threads
 
         # Set latest available cycle
         self._latest = round_time(datetime.utcnow(), hour_resolution=self.cycle_step)
@@ -135,15 +137,15 @@
             model=self.model,
             fxx=self.fxx[-1],
             product=self.product,
             priority=self.priority,
         )
         try:
             # Inventory raises a ValueError if no data can be found
-            f.inventory(self.pattern)
+            f.inventory(self.pattern, verbose=self.verbose)
             self.cycle = self._latest
         except ValueError:
             # Step back a cycle only if stepback limit is not reached
             if self._stepback >= self.stepback:
                 raise ValueError(
                     f"No data found after {self.stepback} stepbacks for the given "
                     f"parameters: {self}"
@@ -173,28 +175,38 @@
             try:
                 logger.debug(f"Inventory:\n{fh.inventory(self.pattern)}")
             except ValueError as e:
                 raise ValueError(f"No data found for the parameters: {self}") from e
 
         # Open the xarray dataset
         try:
-            ds = fh.xarray(self.pattern, max_threads=self.max_threads, remove_grib=True)
+            ds = fh.xarray(
+                self.pattern,
+                max_threads=self.max_threads,
+                remove_grib=True,
+                verbose=self.verbose,
+            )
         except TypeError as e:
             logger.warning(f"Error using multithreading: {e}, trying without it")
-            ds = fh.xarray(self.pattern, max_threads=None, remove_grib=True)
+            ds = fh.xarray(
+                self.pattern,
+                max_threads=None,
+                remove_grib=True,
+                verbose=self.verbose,
+            )
 
         # Ensure single dataset is returned
         if isinstance(ds, list):
             raise ValueError(
                 f"The given parameters: {self} returned multiple datasets that cannot "
                 f"be concatenated, please review your selected pattern: {self.pattern}"
             )
 
         # Turn step index into time index
-        ds = ds.assign_coords({"step": ds.valid_time}).drop(["time", "valid_time"])
+        ds = ds.assign_coords({"step": ds.valid_time}).drop_vars(["time", "valid_time"])
         ds = ds.rename({"step": "time"}).reset_coords()
 
         # Ensure the entire lead time period requested is available
         times = ds.time.to_index()
         t1 = times[0] + timedelta(hours=self.fxx[-1])
         if t1 > times[-1]:
             raise ValueError(
@@ -209,15 +221,15 @@
 
         # Renaming
         ds = ds.rename(self.mapping)
 
         self._ds = ds
 
 
-class NowcastSource(DataSourceMixin):
+class NowcastSource(DataSourceBase):
     """Nowcast data source.
 
     This driver opens a nowcast dataset using the Herbies package.
 
     Parameters
     ----------
     model: str
@@ -259,14 +271,15 @@
         cycle_step=6,
         time_step=1,
         stepback=1,
         priority=["google", "aws", "nomads", "azure"],
         max_threads=None,
         mapping={},
         sorted=False,
+        verbose=False,
         metadata=None,
         **kwargs
     ):
         super().__init__(metadata=metadata, **kwargs)
 
         self.model = model
         self.product = product
@@ -275,14 +288,15 @@
         self.stop = stop
         self.cycle_step = cycle_step
         self.time_step = time_step
         self.stepback = stepback
         self.priority = priority
         self.mapping = mapping
         self.sorted = sorted
+        self.verbose = verbose
 
         self._stepback = 0
         self._max_threads = max_threads
 
         # Set latest available cycle
         self._latest = round_time(datetime.utcnow(), hour_resolution=self.cycle_step)
 
@@ -343,15 +357,15 @@
             model=self.model,
             fxx=self.cycle_step,
             product=self.product,
             priority=self.priority,
         )
         try:
             # Inventory raises a ValueError if no data can be found
-            f.inventory(self.pattern)
+            f.inventory(self.pattern, verbose=self.verbose)
             self.stop = self._latest
         except ValueError:
             # Step back a cycle only if stepback limit is not reached
             if self._stepback >= self.stepback:
                 raise ValueError(
                     f"No data found after {self.stepback} stepbacks for the given "
                     f"parameters: {self}"
@@ -361,15 +375,15 @@
             return self._set_latest_cycle()
 
     def _format_dataset(self, ds):
         """Format the dataset."""
         # Convert time and step indices into single time index.
         ds = ds.stack(times=["time", "step"], create_index=False)
         ds = ds.assign_coords({"times": ds.time + ds.step}).transpose("times", ...)
-        ds = ds.drop(["time", "step", "valid_time"]).rename({"times": "time"})
+        ds = ds.drop_vars(["time", "step", "valid_time"]).rename({"times": "time"})
         ds = ds.reset_coords()
         # Sorting
         if self.sorted:
             for coord in ds.coords:
                 ds = ds.sortby(coord)
         # Renaming
         ds = ds.rename(self.mapping)
@@ -395,18 +409,28 @@
         try:
             logger.debug(f"Inventory:\n{fh.inventory(self.pattern)}")
         except ValueError as e:
             raise ValueError(f"No data found for the given parameters: {self}") from e
 
         # Open the xarray dataset
         try:
-            ds = fh.xarray(self.pattern, max_threads=self.max_threads, remove_grib=True)
+            ds = fh.xarray(
+                self.pattern,
+                max_threads=self.max_threads,
+                remove_grib=True,
+                verbose=self.verbose,
+            )
         except TypeError as e:
             logger.warning(f"Error using multithreading: {e}, trying without it")
-            ds = fh.xarray(self.pattern, max_threads=None, remove_grib=True)
+            ds = fh.xarray(
+                self.pattern,
+                max_threads=None,
+                remove_grib=True,
+                verbose=self.verbose,
+            )
 
         # Ensure single dataset is returned
         if isinstance(ds, list):
             raise ValueError(
                 f"The given parameters: {self} returned multiple datasets that cannot "
                 f"be concatenated, please review your selected pattern: {self.pattern}"
             )
```

### Comparing `intake-nwp-0.3.4/intake_nwp.egg-info/PKG-INFO` & `intake_nwp-0.3.5/intake_nwp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-nwp
-Version: 0.3.4
+Version: 0.3.5
 Summary: Intake drivers for numerical weather prediction data
 Author-email: Oceanum Developers <developers@oceanum.science>
 Maintainer-email: Oceanum Developers <developers@oceanum.science>
 License: MIT License
         
         Copyright (c) 2022, Oceanum Developers
         
@@ -47,14 +47,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: click
 Requires-Dist: cartopy
 Requires-Dist: cfgrib
 Requires-Dist: herbie-data
 Requires-Dist: intake
+Requires-Dist: jinja2
 Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: extra
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `intake-nwp-0.3.4/intake_nwp.egg-info/SOURCES.txt` & `intake_nwp-0.3.5/intake_nwp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/pyproject.toml` & `intake_nwp-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 requires-python = ">=3.8"
 dependencies = [
   "click",
   "cartopy",
   "cfgrib",
   "herbie-data",
   "intake",
+  "jinja2", # for intake2
   "psutil",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
   "pytest",
```

### Comparing `intake-nwp-0.3.4/tests/catalog.yml` & `intake_nwp-0.3.5/tests/catalog.yml`

 * *Files identical despite different names*

### Comparing `intake-nwp-0.3.4/tests/test_nwp.py` & `intake_nwp-0.3.5/tests/test_nwp.py`

 * *Files identical despite different names*

