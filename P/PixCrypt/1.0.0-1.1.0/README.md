# Comparing `tmp/PixCrypt-1.0.0.tar.gz` & `tmp/PixCrypt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PixCrypt-1.0.0.tar", last modified: Mon Apr 29 14:54:08 2024, max compression
+gzip compressed data, was "PixCrypt-1.1.0.tar", last modified: Wed May  1 06:22:49 2024, max compression
```

## Comparing `PixCrypt-1.0.0.tar` & `PixCrypt-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:54:08.244282 PixCrypt-1.0.0/
--rw-rw-rw-   0        0        0     1084 2024-04-29 11:57:03.000000 PixCrypt-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1279 2024-04-29 14:54:08.244282 PixCrypt-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 14:54:08.244282 PixCrypt-1.0.0/PixCrypt.egg-info/
--rw-rw-rw-   0        0        0     1279 2024-04-29 14:54:07.000000 PixCrypt-1.0.0/PixCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-04-29 14:54:07.000000 PixCrypt-1.0.0/PixCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:54:07.000000 PixCrypt-1.0.0/PixCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-29 14:54:07.000000 PixCrypt-1.0.0/PixCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 14:54:07.000000 PixCrypt-1.0.0/PixCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      828 2024-04-29 14:10:52.000000 PixCrypt-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 14:54:08.244282 PixCrypt-1.0.0/pixcrypt/
--rw-rw-rw-   0        0        0       31 2024-04-28 13:21:05.000000 PixCrypt-1.0.0/pixcrypt/__init__.py
--rw-rw-rw-   0        0        0     1533 2024-04-29 13:36:55.000000 PixCrypt-1.0.0/pixcrypt/_piximg.py
--rw-rw-rw-   0        0        0       42 2024-04-29 14:54:08.244282 PixCrypt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      670 2024-04-29 14:49:52.000000 PixCrypt-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:22:49.016192 PixCrypt-1.1.0/
+-rw-rw-rw-   0        0        0     1084 2024-04-29 11:57:03.000000 PixCrypt-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1273 2024-05-01 06:22:49.016192 PixCrypt-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 06:22:49.000567 PixCrypt-1.1.0/PixCrypt.egg-info/
+-rw-rw-rw-   0        0        0     1273 2024-05-01 06:22:48.000000 PixCrypt-1.1.0/PixCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-01 06:22:48.000000 PixCrypt-1.1.0/PixCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 06:22:48.000000 PixCrypt-1.1.0/PixCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 06:22:48.000000 PixCrypt-1.1.0/PixCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 06:22:48.000000 PixCrypt-1.1.0/PixCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      822 2024-05-01 06:19:24.000000 PixCrypt-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 06:22:49.016192 PixCrypt-1.1.0/pixcrypt/
+-rw-rw-rw-   0        0        0       31 2024-04-28 13:21:05.000000 PixCrypt-1.1.0/pixcrypt/__init__.py
+-rw-rw-rw-   0        0        0     1853 2024-05-01 06:10:04.000000 PixCrypt-1.1.0/pixcrypt/_piximg.py
+-rw-rw-rw-   0        0        0       42 2024-05-01 06:22:49.016192 PixCrypt-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-04-30 16:38:05.000000 PixCrypt-1.1.0/setup.py
```

### Comparing `PixCrypt-1.0.0/LICENSE` & `PixCrypt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PixCrypt-1.0.0/PKG-INFO` & `PixCrypt-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PixCrypt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for encrypting text into an image
 Author: ALhorm
 Author-email: gladkoam@gmail.com
 Keywords: pixcrypt pillow image encryption python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,27 +22,28 @@
 
 src = 'Hello World!'
 pix = PixImage(text=src)
 img = pix.getimage()
 
 img.save('hello_world.png')
 ```
-If you will be decrypting the image, save the file in PNG format. ```PixImage``` class contains a built-in method for saving:
+If you will be decrypting the image, save the file in PNG format. You can also specify a maximum width for the image:
 ```py
-pix.save('hello_world') # without extension
+img = pix.getimage(max_width=12)
 ```
 ### Decrypting image into text
 ```py
 from pixcrypt import PixImage
 
 pix = PixImage('hello_world.png')
 text = pix.getstr()
 
 print(text) # Hello World!
 ```
 ```PixImage``` can take an Image class object from Pillow as an argument:
 ```py
 pix = PixImage(text='some info')
 pix2 = PixImage(pix.getimage())
+text = pix2.getstr()
 
-print(pix2.getstr()) # some info
+print(text) # some info
 ```
```

### Comparing `PixCrypt-1.0.0/PixCrypt.egg-info/PKG-INFO` & `PixCrypt-1.1.0/PixCrypt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PixCrypt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for encrypting text into an image
 Author: ALhorm
 Author-email: gladkoam@gmail.com
 Keywords: pixcrypt pillow image encryption python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,27 +22,28 @@
 
 src = 'Hello World!'
 pix = PixImage(text=src)
 img = pix.getimage()
 
 img.save('hello_world.png')
 ```
-If you will be decrypting the image, save the file in PNG format. ```PixImage``` class contains a built-in method for saving:
+If you will be decrypting the image, save the file in PNG format. You can also specify a maximum width for the image:
 ```py
-pix.save('hello_world') # without extension
+img = pix.getimage(max_width=12)
 ```
 ### Decrypting image into text
 ```py
 from pixcrypt import PixImage
 
 pix = PixImage('hello_world.png')
 text = pix.getstr()
 
 print(text) # Hello World!
 ```
 ```PixImage``` can take an Image class object from Pillow as an argument:
 ```py
 pix = PixImage(text='some info')
 pix2 = PixImage(pix.getimage())
+text = pix2.getstr()
 
-print(pix2.getstr()) # some info
+print(text) # some info
 ```
```

### Comparing `PixCrypt-1.0.0/README.md` & `PixCrypt-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 
 src = 'Hello World!'
 pix = PixImage(text=src)
 img = pix.getimage()
 
 img.save('hello_world.png')
 ```
-If you will be decrypting the image, save the file in PNG format. ```PixImage``` class contains a built-in method for saving:
+If you will be decrypting the image, save the file in PNG format. You can also specify a maximum width for the image:
 ```py
-pix.save('hello_world') # without extension
+img = pix.getimage(max_width=12)
 ```
 ### Decrypting image into text
 ```py
 from pixcrypt import PixImage
 
 pix = PixImage('hello_world.png')
 text = pix.getstr()
 
 print(text) # Hello World!
 ```
 ```PixImage``` can take an Image class object from Pillow as an argument:
 ```py
 pix = PixImage(text='some info')
 pix2 = PixImage(pix.getimage())
+text = pix2.getstr()
 
-print(pix2.getstr()) # some info
+print(text) # some info
 ```
```

### Comparing `PixCrypt-1.0.0/setup.py` & `PixCrypt-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
 	with open('README.md', 'r') as f:
 		return f.read()
 
 
 setup(
 	name='PixCrypt',
-	version='1.0.0',
+	version='1.1.0',
 	author='ALhorm',
 	author_email='gladkoam@gmail.com',
 	description='Library for encrypting text into an image',
 	long_description=readme(),
 	long_description_content_type='text/markdown',
 	packages=find_packages(),
 	install_requires=['pillow>=10.0.0'],
```

