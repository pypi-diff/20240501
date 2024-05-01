# Comparing `tmp/apache_airflow_providers_teradata-2.0.0rc1.tar.gz` & `tmp/apache_airflow_providers_teradata-2.1.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_teradata-2.0.0rc1.tar", last modified: Thu Nov 16 15:21:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

