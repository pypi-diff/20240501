# Comparing `tmp/botocore-a-la-carte-mobile-1.34.94.tar.gz` & `tmp/botocore_a_la_carte_mobile-1.34.95-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-mobile-1.34.94.tar", last modified: Tue Apr 30 01:01:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
