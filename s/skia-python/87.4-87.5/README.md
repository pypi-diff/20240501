# Comparing `tmp/skia_python-87.4-cp39-cp39-win_amd64.whl.zip` & `tmp/skia_python-87.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4454894 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat 11681280 b- defN 22-Jan-20 08:35 skia.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1551 b- defN 22-Jan-20 08:35 skia_python-87.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2877 b- defN 22-Jan-20 08:35 skia_python-87.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Jan-20 08:35 skia_python-87.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Jan-20 08:35 skia_python-87.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      485 b- defN 22-Jan-20 08:35 skia_python-87.4.dist-info/RECORD
-6 files, 11686298 bytes uncompressed, 4454022 bytes compressed:  61.9%
+Zip file size: 4373511 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat 11247616 b- defN 22-Nov-07 14:49 skia.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1551 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2891 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      485 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/RECORD
+6 files, 11252648 bytes uncompressed, 4372639 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: skia.cp39-win_amd64.pyd
 Comment: 
 
-Filename: skia_python-87.4.dist-info/LICENSE
+Filename: skia_python-87.5.dist-info/LICENSE
 Comment: 
 
-Filename: skia_python-87.4.dist-info/METADATA
+Filename: skia_python-87.5.dist-info/METADATA
 Comment: 
 
-Filename: skia_python-87.4.dist-info/WHEEL
+Filename: skia_python-87.5.dist-info/WHEEL
 Comment: 
 
-Filename: skia_python-87.4.dist-info/top_level.txt
+Filename: skia_python-87.5.dist-info/top_level.txt
 Comment: 
 
-Filename: skia_python-87.4.dist-info/RECORD
+Filename: skia_python-87.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `skia_python-87.4.dist-info/LICENSE` & `skia_python-87.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `skia_python-87.4.dist-info/METADATA` & `skia_python-87.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: skia-python
-Version: 87.4
+Version: 87.5
 Summary: Skia python binding
 Home-page: https://github.com/kyamagu/skia-python
 Author: Kota Yamaguchi
 Author-email: KotaYamaguchi1984@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pybind11 (>=2.6)
 
@@ -78,9 +77,7 @@
 
 - [Tutorial](https://kyamagu.github.io/skia-python/tutorial/)
 - [Reference](https://kyamagu.github.io/skia-python/reference.html)
 
 ## Contributing
 
 Feel free to [post an issue](https://github.com/kyamagu/skia-python/issues) or [PR](https://github.com/kyamagu/skia-python/pulls).
-
-
```

