# Comparing `tmp/crossandra-2.0.0.tar.gz` & `tmp/crossandra-2.1.0-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossandra-2.0.0.tar", last modified: Sat Apr 29 17:52:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

