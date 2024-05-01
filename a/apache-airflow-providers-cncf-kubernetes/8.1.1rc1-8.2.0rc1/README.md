# Comparing `tmp/apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar.gz` & `tmp/apache_airflow_providers_cncf_kubernetes-8.2.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar", last modified: Tue Apr 16 07:37:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
