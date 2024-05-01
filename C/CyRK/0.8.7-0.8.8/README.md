# Comparing `tmp/cyrk-0.8.7.tar.gz` & `tmp/CyRK-0.8.8-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyrk-0.8.7.tar", last modified: Fri Apr 26 22:47:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

