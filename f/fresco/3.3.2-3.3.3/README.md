# Comparing `tmp/fresco-3.3.2.tar.gz` & `tmp/fresco-3.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fresco-3.3.2.tar", last modified: Wed May 31 12:10:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

