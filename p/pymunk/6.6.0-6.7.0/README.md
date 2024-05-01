# Comparing `tmp/pymunk-6.6.0.tar.gz` & `tmp/pymunk-6.7.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\pymunk\pymunk\dist\.tmp-6ke6ltm0\pymunk-6.6.0.tar", last modified: Thu Nov  2 14:06:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

