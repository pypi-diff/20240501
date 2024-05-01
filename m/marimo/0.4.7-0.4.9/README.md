# Comparing `tmp/marimo-0.4.7.tar.gz` & `tmp/marimo-0.4.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marimo-0.4.7.tar", last modified: Sat Apr 27 20:33:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

