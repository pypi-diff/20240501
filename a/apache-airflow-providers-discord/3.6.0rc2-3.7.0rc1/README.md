# Comparing `tmp/apache_airflow_providers_discord-3.6.0rc2.tar.gz` & `tmp/apache_airflow_providers_discord-3.7.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_discord-3.6.0rc2.tar", last modified: Mon Jan 22 08:27:42 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

