# Comparing `tmp/algomodule-1.0.2.tar.gz` & `tmp/algomodule-1.0.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/algomodule-1.0.2.tar", last modified: Sat Aug  8 23:00:44 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

