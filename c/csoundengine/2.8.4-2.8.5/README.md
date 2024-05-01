# Comparing `tmp/csoundengine-2.8.4.tar.gz` & `tmp/csoundengine-2.8.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csoundengine-2.8.4.tar", last modified: Tue Apr 23 22:14:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

