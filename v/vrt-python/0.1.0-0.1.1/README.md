# Comparing `tmp/vrt-python-0.1.0.tar.gz` & `tmp/vrt-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrt-python-0.1.0.tar", last modified: Wed May  1 14:35:10 2024, max compression
+gzip compressed data, was "vrt-python-0.1.1.tar", last modified: Wed May  1 15:00:12 2024, max compression
```

## Comparing `vrt-python-0.1.0.tar` & `vrt-python-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 14:35:10.278988 vrt-python-0.1.0/
--rw-r--r--   0 vshkodin   (501) staff       (20)     1615 2024-04-30 21:07:14.000000 vrt-python-0.1.0/LICENSE
--rw-r--r--   0 vshkodin   (501) staff       (20)     1991 2024-05-01 14:35:10.278780 vrt-python-0.1.0/PKG-INFO
--rw-r--r--   0 vshkodin   (501) staff       (20)     1499 2024-04-30 21:03:39.000000 vrt-python-0.1.0/README.md
-drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 14:35:10.276931 vrt-python-0.1.0/image_diff/
--rw-r--r--   0 vshkodin   (501) staff       (20)        0 2024-04-30 19:39:12.000000 vrt-python-0.1.0/image_diff/__init__.py
--rw-r--r--   0 vshkodin   (501) staff       (20)     2524 2024-04-30 20:58:10.000000 vrt-python-0.1.0/image_diff/image_diff.py
--rw-r--r--   0 vshkodin   (501) staff       (20)       38 2024-05-01 14:35:10.279027 vrt-python-0.1.0/setup.cfg
--rw-r--r--   0 vshkodin   (501) staff       (20)      797 2024-05-01 14:35:08.000000 vrt-python-0.1.0/setup.py
-drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 14:35:10.277357 vrt-python-0.1.0/tests/
--rw-r--r--   0 vshkodin   (501) staff       (20)        0 2024-04-30 19:39:12.000000 vrt-python-0.1.0/tests/__init__.py
--rw-r--r--   0 vshkodin   (501) staff       (20)     1819 2024-04-30 20:48:33.000000 vrt-python-0.1.0/tests/test_vrt.py
-drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 14:35:10.277660 vrt-python-0.1.0/tests/testing_images/
--rw-r--r--   0 vshkodin   (501) staff       (20)        0 2024-04-30 19:39:12.000000 vrt-python-0.1.0/tests/testing_images/__init__.py
-drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 14:35:10.278536 vrt-python-0.1.0/vrt_python.egg-info/
--rw-r--r--   0 vshkodin   (501) staff       (20)     1991 2024-05-01 14:35:10.000000 vrt-python-0.1.0/vrt_python.egg-info/PKG-INFO
--rw-r--r--   0 vshkodin   (501) staff       (20)      349 2024-05-01 14:35:10.000000 vrt-python-0.1.0/vrt_python.egg-info/SOURCES.txt
--rw-r--r--   0 vshkodin   (501) staff       (20)        1 2024-05-01 14:35:10.000000 vrt-python-0.1.0/vrt_python.egg-info/dependency_links.txt
--rw-r--r--   0 vshkodin   (501) staff       (20)       64 2024-05-01 14:35:10.000000 vrt-python-0.1.0/vrt_python.egg-info/entry_points.txt
--rw-r--r--   0 vshkodin   (501) staff       (20)       29 2024-05-01 14:35:10.000000 vrt-python-0.1.0/vrt_python.egg-info/requires.txt
--rw-r--r--   0 vshkodin   (501) staff       (20)       17 2024-05-01 14:35:10.000000 vrt-python-0.1.0/vrt_python.egg-info/top_level.txt
+drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 15:00:12.028188 vrt-python-0.1.1/
+-rw-r--r--   0 vshkodin   (501) staff       (20)     1615 2024-04-30 21:07:14.000000 vrt-python-0.1.1/LICENSE
+-rw-r--r--   0 vshkodin   (501) staff       (20)     1991 2024-05-01 15:00:12.028011 vrt-python-0.1.1/PKG-INFO
+-rw-r--r--   0 vshkodin   (501) staff       (20)     1499 2024-04-30 21:03:39.000000 vrt-python-0.1.1/README.md
+drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 15:00:12.026305 vrt-python-0.1.1/image_diff/
+-rw-r--r--   0 vshkodin   (501) staff       (20)        0 2024-04-30 19:39:12.000000 vrt-python-0.1.1/image_diff/__init__.py
+-rw-r--r--   0 vshkodin   (501) staff       (20)     2626 2024-05-01 14:57:15.000000 vrt-python-0.1.1/image_diff/image_diff.py
+-rw-r--r--   0 vshkodin   (501) staff       (20)       38 2024-05-01 15:00:12.028230 vrt-python-0.1.1/setup.cfg
+-rw-r--r--   0 vshkodin   (501) staff       (20)      797 2024-05-01 15:00:03.000000 vrt-python-0.1.1/setup.py
+drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 15:00:12.026717 vrt-python-0.1.1/tests/
+-rw-r--r--   0 vshkodin   (501) staff       (20)        0 2024-04-30 19:39:12.000000 vrt-python-0.1.1/tests/__init__.py
+-rw-r--r--   0 vshkodin   (501) staff       (20)     1819 2024-04-30 20:48:33.000000 vrt-python-0.1.1/tests/test_vrt.py
+drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 15:00:12.027028 vrt-python-0.1.1/tests/testing_images/
+-rw-r--r--   0 vshkodin   (501) staff       (20)        0 2024-04-30 19:39:12.000000 vrt-python-0.1.1/tests/testing_images/__init__.py
+drwxr-xr-x   0 vshkodin   (501) staff       (20)        0 2024-05-01 15:00:12.027780 vrt-python-0.1.1/vrt_python.egg-info/
+-rw-r--r--   0 vshkodin   (501) staff       (20)     1991 2024-05-01 15:00:11.000000 vrt-python-0.1.1/vrt_python.egg-info/PKG-INFO
+-rw-r--r--   0 vshkodin   (501) staff       (20)      349 2024-05-01 15:00:12.000000 vrt-python-0.1.1/vrt_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vshkodin   (501) staff       (20)        1 2024-05-01 15:00:11.000000 vrt-python-0.1.1/vrt_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vshkodin   (501) staff       (20)       64 2024-05-01 15:00:11.000000 vrt-python-0.1.1/vrt_python.egg-info/entry_points.txt
+-rw-r--r--   0 vshkodin   (501) staff       (20)       29 2024-05-01 15:00:11.000000 vrt-python-0.1.1/vrt_python.egg-info/requires.txt
+-rw-r--r--   0 vshkodin   (501) staff       (20)       17 2024-05-01 15:00:11.000000 vrt-python-0.1.1/vrt_python.egg-info/top_level.txt
```

### Comparing `vrt-python-0.1.0/LICENSE` & `vrt-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vrt-python-0.1.0/PKG-INFO` & `vrt-python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrt-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility to compare images and screenshots
 Home-page: https://github.com/vshkodin/python-vrt
 Author: Vladimir Shkodin
 Author-email: v.s.shkodin@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `vrt-python-0.1.0/README.md` & `vrt-python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vrt-python-0.1.0/image_diff/image_diff.py` & `vrt-python-0.1.1/image_diff/image_diff.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,32 +34,34 @@
 
     def generate_difference_image(self, difference_path=None, test=None):
         if test == True:
             self.last_part = os.path.basename(self.actual_path)
             self.last_part=self.last_part.replace('.png', '')
             self.last_part = f"{self.last_part}_difference.png"
             difference_path = self.last_part
-
+        else:
+            difference_path = "result_difference.png"
         self.load_images()
         mask, difference_percentage = self.calculate_difference()
         result_array = self.apply_overlay(mask)
         result_image = Image.fromarray(result_array)
         result_image.save(difference_path)
         #print(f"Difference percentage: {difference_percentage:.2f}%")
         return difference_percentage
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Compare two images for differences.")
-    parser.add_argument('--expectation', required=True, help='Path to the expected image file.')
-    parser.add_argument('--actual', required=True, help='Path to the actual image file.')
-    parser.add_argument('--output', required=True, help='Path where the difference image will be saved.')
-
-    args = parser.parse_args()
-
-    image_diff = ImageDifference(expectation_path=args.expectation, actual_path=args.actual)
-    difference_percentage = image_diff.generate_difference_image(args.output)
-    print(f"Generated difference image with {difference_percentage:.2f}% difference.")
+    pass
+    # parser = argparse.ArgumentParser(description="Compare two images for differences.")
+    # parser.add_argument('--expectation', required=True, help='Path to the expected image file.')
+    # parser.add_argument('--actual', required=True, help='Path to the actual image file.')
+    # parser.add_argument('--output', required=True, help='Path where the difference image will be saved.')
+    #
+    # args = parser.parse_args()
+    #
+    # image_diff = ImageDifference(expectation_path=args.expectation, actual_path=args.actual)
+    # difference_percentage = image_diff.generate_difference_image(args.output)
+    # print(f"Generated difference image with {difference_percentage:.2f}% difference.")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `vrt-python-0.1.0/setup.py` & `vrt-python-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vrt-python',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'numpy==1.26.4',
         'Pillow==10.2.0'
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `vrt-python-0.1.0/tests/test_vrt.py` & `vrt-python-0.1.1/tests/test_vrt.py`

 * *Files identical despite different names*

### Comparing `vrt-python-0.1.0/vrt_python.egg-info/PKG-INFO` & `vrt-python-0.1.1/vrt_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrt-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility to compare images and screenshots
 Home-page: https://github.com/vshkodin/python-vrt
 Author: Vladimir Shkodin
 Author-email: v.s.shkodin@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

