# Comparing `tmp/rtc_tools_simulation-0.1.0a2.tar.gz` & `tmp/rtc_tools_simulation-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc_tools_simulation-0.1.0a2.tar", max compression
+gzip compressed data, was "rtc_tools_simulation-0.1.0a3.tar", max compression
```

## Comparing `rtc_tools_simulation-0.1.0a2.tar` & `rtc_tools_simulation-0.1.0a3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      414 2024-05-01 09:40:38.038622 rtc_tools_simulation-0.1.0a2/README.md
--rw-r--r--   0        0        0     1246 2024-05-01 09:40:54.891556 rtc_tools_simulation-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 09:40:38.069622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/__init__.py
--rw-r--r--   0        0        0     1100 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/cli/reservoir.py
--rw-r--r--   0        0        0      108 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/empty_plot_table.csv
--rw-r--r--   0        0        0     7050 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/lookup_table.py
--rw-r--r--   0        0        0     5348 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/model.py
--rw-r--r--   0        0        0     3219 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/model_config.py
--rw-r--r--   0        0        0      140 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/modelica/reservoir/lookup_table_equations.csv
--rw-r--r--   0        0        0     1955 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/modelica/reservoir/reservoir.mo
--rw-r--r--   0        0        0        0 2024-05-01 09:40:38.071622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/__init__.py
--rw-r--r--   0        0        0    10918 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/model.py
--rw-r--r--   0        0        0     7385 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/read_csv.py
--rw-r--r--   0        0        0     1315 2024-05-01 09:40:38.040622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/rule_curve.py
--rw-r--r--   0        0        0    10970 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/setq_help_functions.py
--rw-r--r--   0        0        0     1755 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template.py
--rw-r--r--   0        0        0      203 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/plot_table.csv
--rw-r--r--   0        0        0     1598 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/rtcDataConfig.xml
--rw-r--r--   0        0        0      660 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/rtcParameterConfig.xml
--rw-r--r--   0        0        0     4384 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/timeseries_import.xml
--rw-r--r--   0        0        0       33 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/lookup_tables/h_qspill.csv
--rw-r--r--   0        0        0      201 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/lookup_tables/lookup_tables.csv
--rw-r--r--   0        0        0       32 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/lookup_tables/qout_v.csv
--rw-r--r--   0        0        0       26 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/lookup_tables/v_area.csv
--rw-r--r--   0        0        0       27 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/lookup_tables/v_h.csv
--rw-r--r--   0        0        0        0 2024-05-01 09:40:38.071622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/output/timeseries_export.csv
--rw-r--r--   0        0        0      637 2024-05-01 09:40:38.041622 rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/reservoir.txt
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 rtc_tools_simulation-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      484 2024-05-01 15:21:12.438739 rtc_tools_simulation-0.1.0a3/README.md
+-rw-r--r--   0        0        0     1245 2024-05-01 15:21:29.526267 rtc_tools_simulation-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-01 15:21:12.471739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/__init__.py
+-rw-r--r--   0        0        0     1100 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/cli/reservoir.py
+-rw-r--r--   0        0        0      108 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/empty_plot_table.csv
+-rw-r--r--   0        0        0     7050 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/lookup_table.py
+-rw-r--r--   0        0        0     5348 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/model.py
+-rw-r--r--   0        0        0     3219 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/model_config.py
+-rw-r--r--   0        0        0      140 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/modelica/reservoir/lookup_table_equations.csv
+-rw-r--r--   0        0        0     1955 2024-05-01 15:21:12.440739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/modelica/reservoir/reservoir.mo
+-rw-r--r--   0        0        0        0 2024-05-01 15:21:12.475739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/__init__.py
+-rw-r--r--   0        0        0    10918 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/model.py
+-rw-r--r--   0        0        0     7385 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/read_csv.py
+-rw-r--r--   0        0        0     1315 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/rule_curve.py
+-rw-r--r--   0        0        0    10970 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/setq_help_functions.py
+-rw-r--r--   0        0        0     1755 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template.py
+-rw-r--r--   0        0        0      203 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/plot_table.csv
+-rw-r--r--   0        0        0     1598 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/rtcDataConfig.xml
+-rw-r--r--   0        0        0      660 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/rtcParameterConfig.xml
+-rw-r--r--   0        0        0     4384 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/timeseries_import.xml
+-rw-r--r--   0        0        0       33 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/lookup_tables/h_qspill.csv
+-rw-r--r--   0        0        0      201 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/lookup_tables/lookup_tables.csv
+-rw-r--r--   0        0        0       32 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/lookup_tables/qout_v.csv
+-rw-r--r--   0        0        0       26 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/lookup_tables/v_area.csv
+-rw-r--r--   0        0        0       27 2024-05-01 15:21:12.441739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/lookup_tables/v_h.csv
+-rw-r--r--   0        0        0        0 2024-05-01 15:21:12.475739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/output/timeseries_export.csv
+-rw-r--r--   0        0        0      637 2024-05-01 15:21:12.442739 rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/reservoir.txt
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 rtc_tools_simulation-0.1.0a3/PKG-INFO
```

### Comparing `rtc_tools_simulation-0.1.0a2/pyproject.toml` & `rtc_tools_simulation-0.1.0a3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "rtc-tools-simulation"
 packages = [{ include = "rtctools_simulation" }]
-version = "0.1.0-a.2"
+version = "0.1.0-a.3"
 authors = ["Deltares"]
 description = "Extension for building models used for simulation in rtc-tools."
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-casadi = "^3.6.3"
+casadi = "3.6.*"
 Jinja2 = "*"
 numpy = "*"
 pandas = "*"
 rtc-tools = "^2.6"
 rtc-tools-interface = "0.7.*"
 
 [tool.poetry.scripts]
```

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/cli/reservoir.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/cli/reservoir.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/lookup_table.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/lookup_table.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/model.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/model.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/model_config.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/model_config.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/modelica/reservoir/reservoir.mo` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/modelica/reservoir/reservoir.mo`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/model.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/model.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/read_csv.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/read_csv.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/rule_curve.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/rule_curve.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/setq_help_functions.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/setq_help_functions.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template.py` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template.py`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/rtcDataConfig.xml` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/rtcDataConfig.xml`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/rtcParameterConfig.xml` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/rtcParameterConfig.xml`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/input/timeseries_import.xml` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/input/timeseries_import.xml`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/rtctools_simulation/reservoir/template_data/reservoir.txt` & `rtc_tools_simulation-0.1.0a3/rtctools_simulation/reservoir/template_data/reservoir.txt`

 * *Files identical despite different names*

### Comparing `rtc_tools_simulation-0.1.0a2/PKG-INFO` & `rtc_tools_simulation-0.1.0a3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: rtc-tools-simulation
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Extension for building models used for simulation in rtc-tools.
 Author: Deltares
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2
-Requires-Dist: casadi (>=3.6.3,<4.0.0)
+Requires-Dist: casadi (==3.6.*)
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rtc-tools (>=2.6,<3.0)
 Requires-Dist: rtc-tools-interface (==0.7.*)
 Description-Content-Type: text/markdown
 
 # rtc-tools-simulation
@@ -29,9 +29,9 @@
 
 ## Documentation
 
 Documentation and examples can be found on [readthedocs](https://rtc-tools-simulation.readthedocs.io).
 
 ## Developer guidelines
 
-Developer guidelines can be found [here](Contributing.md)
+Developer guidelines can be found [here](https://gitlab.com/rtc-tools-project/rtc-tools-simulation/-/blob/main/CONTRIBUTING.md)
```

