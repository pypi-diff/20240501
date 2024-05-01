# Comparing `tmp/stylepy-0.3.tar.gz` & `tmp/stylepy-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stylepy-0.3.tar", last modified: Wed May  1 14:52:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

