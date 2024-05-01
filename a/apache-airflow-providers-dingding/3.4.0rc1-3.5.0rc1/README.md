# Comparing `tmp/apache_airflow_providers_dingding-3.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_dingding-3.5.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_dingding-3.4.0rc1.tar", last modified: Thu Dec  7 21:09:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

