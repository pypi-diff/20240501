# Comparing `tmp/app-store-scraper-mod-0.3.6.tar.gz` & `tmp/app_store_scraper_mod-0.3.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app-store-scraper-mod-0.3.6.tar", last modified: Wed May  1 08:18:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

