# Comparing `tmp/apache_airflow_providers_fab-1.0.4rc1.tar.gz` & `tmp/apache_airflow_providers_fab-1.1.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_fab-1.0.4rc1.tar", last modified: Tue Apr 16 07:37:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
