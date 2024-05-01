# Comparing `tmp/ddtrace-2.8.3.tar.gz` & `tmp/ddtrace-2.9.0rc1-cp312-cp312-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddtrace-2.8.3.tar", last modified: Mon Apr 29 14:29:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

