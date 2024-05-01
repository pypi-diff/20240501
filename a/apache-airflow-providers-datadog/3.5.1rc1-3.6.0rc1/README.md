# Comparing `tmp/apache_airflow_providers_datadog-3.5.1rc1.tar.gz` & `tmp/apache_airflow_providers_datadog-3.6.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_datadog-3.5.1rc1.tar", last modified: Fri Dec 22 23:35:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

