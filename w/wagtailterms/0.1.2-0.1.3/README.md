# Comparing `tmp/wagtailterms-0.1.2.tar.gz` & `tmp/wagtailterms-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailterms-0.1.2.tar", last modified: Fri Apr 12 17:14:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

