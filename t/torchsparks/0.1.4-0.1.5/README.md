# Comparing `tmp/torchsparks-0.1.4.tar.gz` & `tmp/torchsparks-0.1.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\torchsparks-0.1.4.tar", last modified: Sat Mar  9 13:26:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

