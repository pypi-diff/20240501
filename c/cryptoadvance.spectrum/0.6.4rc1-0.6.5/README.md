# Comparing `tmp/cryptoadvance.spectrum-0.6.4rc1.tar.gz` & `tmp/cryptoadvance.spectrum-0.6.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptoadvance.spectrum-0.6.4rc1.tar", last modified: Fri Mar 24 17:17:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

