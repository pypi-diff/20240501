# Comparing `tmp/pytse_filter-1.33.tar.gz` & `tmp/pytse_filter-1.42-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytse_filter-1.33.tar", last modified: Thu Apr 18 12:16:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

