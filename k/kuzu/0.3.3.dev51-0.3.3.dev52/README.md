# Comparing `tmp/kuzu-0.3.3.dev51.tar.gz` & `tmp/kuzu-0.3.3.dev52-cp39-cp39-manylinux_2_27_aarch64.manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev51.tar", last modified: Tue Apr 30 08:04:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

