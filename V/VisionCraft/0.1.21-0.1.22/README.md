# Comparing `tmp/VisionCraft-0.1.21.tar.gz` & `tmp/VisionCraft-0.1.22-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraft-0.1.21.tar", last modified: Tue Apr 30 08:25:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

