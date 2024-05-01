# Comparing `tmp/trytond_stock_lot-7.2.0.tar.gz` & `tmp/trytond_stock_lot-7.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot-7.2.0.tar", last modified: Mon Apr 29 15:51:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

