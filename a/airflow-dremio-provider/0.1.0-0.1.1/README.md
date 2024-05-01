# Comparing `tmp/airflow_dremio_provider-0.1.0.tar.gz` & `tmp/airflow_dremio_provider-0.1.1.tar.gz`

## Comparing `airflow_dremio_provider-0.1.0.tar` & `airflow_dremio_provider-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.0/LICENSE
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.0/README.md
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.1/README.md
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 airflow_dremio_provider-0.1.1/PKG-INFO
```

### Comparing `airflow_dremio_provider-0.1.0/.gitignore` & `airflow_dremio_provider-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_dremio_provider-0.1.0/LICENSE` & `airflow_dremio_provider-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_dremio_provider-0.1.0/README.md` & `airflow_dremio_provider-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airflow_dremio_provider-0.1.0/pyproject.toml` & `airflow_dremio_provider-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 requires-python = ">= 3.7"
 keywords = ["airflow", "provider", "dremio", "apache-airflow"]
 
 [project.entry-points."apache_airflow_provider"]
 provider_info = "dremio_provider.__init__:get_provider_info"
 
 [project.urls]
-Homepage = "https://www.dremio.com/"
+Homepage = "https://github.com/sanchitsreekanth/airflow-provider-dremio"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/dremio_provider"]
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/dremio_provider",
```

### Comparing `airflow_dremio_provider-0.1.0/PKG-INFO` & `airflow_dremio_provider-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: airflow-dremio-provider
-Version: 0.1.0
+Version: 0.1.1
 Summary: A provider package for managing reflections and executing queries via Dremio.
-Project-URL: Homepage, https://www.dremio.com/
+Project-URL: Homepage, https://github.com/sanchitsreekanth/airflow-provider-dremio
 Author-email: Sanchit Sreekanth <sanchitsreekanth@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,dremio,provider
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.7
```

