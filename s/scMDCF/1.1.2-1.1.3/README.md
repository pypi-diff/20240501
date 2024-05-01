# Comparing `tmp/scMDCF-1.1.2.tar.gz` & `tmp/scMDCF-1.1.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scMDCF-1.1.2.tar", last modified: Mon Apr 22 10:38:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
