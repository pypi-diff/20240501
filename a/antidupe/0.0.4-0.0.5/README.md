# Comparing `tmp/antidupe-0.0.4.tar.gz` & `tmp/antidupe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidupe-0.0.4.tar", last modified: Wed May  1 17:53:06 2024, max compression
+gzip compressed data, was "antidupe-0.0.5.tar", last modified: Wed May  1 19:39:22 2024, max compression
```

## Comparing `antidupe-0.0.4.tar` & `antidupe-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:53:06.671077 antidupe-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 17:52:59.000000 antidupe-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 17:53:06.671077 antidupe-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 17:52:59.000000 antidupe-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:53:06.667077 antidupe-0.0.4/antidupe/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 17:52:59.000000 antidupe-0.0.4/antidupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-01 17:52:59.000000 antidupe-0.0.4/antidupe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-01 17:52:59.000000 antidupe-0.0.4/antidupe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:53:06.671077 antidupe-0.0.4/antidupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:53:06.671077 antidupe-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-01 17:52:59.000000 antidupe-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:39:22.934507 antidupe-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 19:39:19.000000 antidupe-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:39:22.934507 antidupe-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 19:39:19.000000 antidupe-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:39:22.930507 antidupe-0.0.5/antidupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 19:39:19.000000 antidupe-0.0.5/antidupe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-01 19:39:19.000000 antidupe-0.0.5/antidupe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-01 19:39:19.000000 antidupe-0.0.5/antidupe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:39:22.934507 antidupe-0.0.5/antidupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:39:22.934507 antidupe-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-01 19:39:19.000000 antidupe-0.0.5/setup.py
```

### Comparing `antidupe-0.0.4/LICENSE` & `antidupe-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.4/PKG-INFO` & `antidupe-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: SSIM-PIL
+Requires-Dist: imagededup
 Requires-Dist: matplotlib
 Requires-Dist: imagehash
 Requires-Dist: efficientnet_pytorch
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
@@ -61,18 +62,19 @@
 ### Customizing Thresholds
 
 You can customize the similarity thresholds for each technique during runtime or initialization:
 
 ```python
 # Initialize Antidupe with custom thresholds
 custom_thresholds = {
-    'ih': 0.2,   # Image Hash
-    'ssim': 0.2, # SSIM
-    'cs': 0.2,   # Cosine Similarity
-    'cnn': 0.2   # CNN
+    'ih': 0.2,    # Image Hash
+    'ssim': 0.2,  # SSIM
+    'cs': 0.2,    # Cosine Similarity
+    'cnn': 0.2,   # CNN
+    'dedup': 0.85 # Mobilenet
 }
 antidupe = Antidupe(limits=custom_thresholds)
 
 # Check for duplicates
 is_duplicate = antidupe.predict([image1, image2])
 ```
 
@@ -94,30 +96,34 @@
 
 ```python
 # Set new limits during runtime
 new_thresholds = {
     'ih': 0.1,
     'ssim': 0.1,
     'cs': 0.1,
-    'cnn': 0.1
+    'cnn': 0.1,
+    'dedup': 0.8
 }
 antidupe.set_limits(limits=new_thresholds)
 
 # Check for duplicates
 is_duplicate = antidupe.predict([image1, image2])
 ```
 
 ## Requirements
 
 - Python 3.x
+- SSIM PIL
+- ImageDeDup
 - NumPy
+- MatPlotLib
 - Pillow
-- imagehash
-- torch
-- efficientnet_pytorch
-- torchvision
+- ImageHash
+- Torch
+- Efficientnet Pytorch
+- TorchVision
 
 ---
 
 ## License
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `antidupe-0.0.4/README.md` & `antidupe-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 ### Customizing Thresholds
 
 You can customize the similarity thresholds for each technique during runtime or initialization:
 
 ```python
 # Initialize Antidupe with custom thresholds
 custom_thresholds = {
-    'ih': 0.2,   # Image Hash
-    'ssim': 0.2, # SSIM
-    'cs': 0.2,   # Cosine Similarity
-    'cnn': 0.2   # CNN
+    'ih': 0.2,    # Image Hash
+    'ssim': 0.2,  # SSIM
+    'cs': 0.2,    # Cosine Similarity
+    'cnn': 0.2,   # CNN
+    'dedup': 0.85 # Mobilenet
 }
 antidupe = Antidupe(limits=custom_thresholds)
 
 # Check for duplicates
 is_duplicate = antidupe.predict([image1, image2])
 ```
 
@@ -72,30 +73,34 @@
 
 ```python
 # Set new limits during runtime
 new_thresholds = {
     'ih': 0.1,
     'ssim': 0.1,
     'cs': 0.1,
-    'cnn': 0.1
+    'cnn': 0.1,
+    'dedup': 0.8
 }
 antidupe.set_limits(limits=new_thresholds)
 
 # Check for duplicates
 is_duplicate = antidupe.predict([image1, image2])
 ```
 
 ## Requirements
 
 - Python 3.x
+- SSIM PIL
+- ImageDeDup
 - NumPy
+- MatPlotLib
 - Pillow
-- imagehash
-- torch
-- efficientnet_pytorch
-- torchvision
+- ImageHash
+- Torch
+- Efficientnet Pytorch
+- TorchVision
 
 ---
 
 ## License
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `antidupe-0.0.4/antidupe/main.py` & `antidupe-0.0.5/antidupe/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,48 @@
     from utilities import (
         euclidean_distance,
         image_hash,
         ssim,
         cosine_similarity,
         CNN,
         resize_image,
+        ImageDeDup,
     )
 except ImportError:
     from .utilities import (
         euclidean_distance,
         image_hash,
         ssim,
         cosine_similarity,
         CNN,
         resize_image,
+        ImageDeDup,
     )
 
 
 DEFAULTS = {
     'ih': 0.1,
     'ssim': 0.15,
     'cs': 0.1,
-    'cnn': 0.15
+    'cnn': 0.15,
+    'dedup': 0.85,
 }
 
 
 class Antidupe:
     """
     Discover duplicate images.
     """
     def __init__(self, limits: dict = DEFAULTS, device: str = 'cpu', debug: bool = False, show_plots: bool = False):  # noqa
         self.show_plots = show_plots
         self.device = device
         self.limits = limits
         self.debug = debug
         self.cnn = CNN(device=device)
+        self.dedup = ImageDeDup()
 
     def d_print(self, *args, **kwargs):
         """
         Debug messanger.
         """
         if self.debug:
             print(*args, **kwargs)
@@ -81,19 +85,23 @@
                 self.d_print('ssim found duplicate')
                 return True
             cs = cosine_similarity(im_1, im_2, self.device)
             self.d_print(f'cosine similarity detected: {cs}')
             if cs < self.limits['cs']:
                 self.d_print('cosine similarity found duplicate')
                 return True
-            cnn = self.cnn.cnn(im_1, im_2)
+            cnn = self.cnn.predict(im_1, im_2)
             self.d_print(f'cnn detected: {cnn}')
             if cnn < self.limits['cnn']:
                 self.d_print('cnn found duplicate')
                 return True
+            dedup = self.dedup.predict(im_1, im_2)
+            if dedup < self.limits['dedup']:
+                self.d_print('dedup found duplicate')
+                return True
         return False
 
     def test(self, images: [list, tuple, None] = None):
         """
         Tests the prediction logic.
         """
         self.debug = True
```

### Comparing `antidupe-0.0.4/antidupe/utilities.py` & `antidupe-0.0.5/antidupe/utilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     FInd differences using convolutional neural networks.
     """
     def __init__(self, device: str = 'cpu'):
         self.device = torch.device(device)
         self.model = EfficientNet.from_pretrained('efficientnet-b0')
         self.model.eval().to(self.device)
 
-    def cnn(self, image_1: Image.Image, image_2: Image.Image) -> float:
+    def predict(self, image_1: Image.Image, image_2: Image.Image) -> float:
         """
         Calculates the CNN similarity between two images.
         """
         image_1 = image_converter(image_1, size=224)
         image_2 = image_converter(image_2, size=224)
         transform = transforms.Compose([
 
@@ -186,19 +186,64 @@
         image2_tensor = transform(image_2).to(self.device)
         features1 = self.model.extract_features(image1_tensor.unsqueeze(0))
         features2 = self.model.extract_features(image2_tensor.unsqueeze(0))
         value = round(np.linalg.norm(np.array(features1.detach()) - np.array(features2.detach())), 4)
         return value / 1000
 
 
+class ImageDeDup:
+    """
+    Perform duplicate identifications using imagededup
+    """
+    def __init__(self, target_size: int = 512, grayscale: bool = True):
+        from imagededup.methods import CNN as CN  # noqa
+        from imagededup.utils import CustomModel  # noqa
+        from imagededup.utils.models import EfficientNet as EN  # noqa
+        from imagededup.utils.image_utils import preprocess_image  # noqa
+        self.cnn_encoder = CN()
+        self.prep = preprocess_image
+        self.target_size = target_size
+        self.grayscale = grayscale
+
+    def preprocess_image(self, image: Image.Image) -> np.ndarray:
+        """
+        Preps the image to gather encodings.
+        """
+        if image.mode != 'RGB':
+            image = image.convert('RGBA').convert('RGB')
+        image = self.prep(image, target_size=(self.target_size, self.target_size), grayscale=self.grayscale)
+        return image
+
+    def predict(self, image_1: Image.Image, image_2: Image.Image, threshold: float = 0.0):
+        """
+        Calculates the CNN similarity between two images.
+        """
+        image_1 = self.preprocess_image(image_1)
+        image_2 = self.preprocess_image(image_2)
+        embeddings1 = self.cnn_encoder.encode_image(image_array=image_1)
+        embeddings2 = self.cnn_encoder.encode_image(image_array=image_2)
+        embeddings_dict = {
+            1: embeddings1[0],
+            2: embeddings2[0]
+        }
+
+        similarity_score = self.cnn_encoder._find_duplicates_dict(  # noqa
+            embeddings_dict,  # noqa
+            min_similarity_threshold=threshold,
+            scores=True
+        )  # noqa
+        return similarity_score[1][0][1]
+
+
 def test():
     """
     This will test the various math functions
     """
     cnn = CNN()
+    dedup = ImageDeDup()
     print('resources loaded')
 
     image_unique = image_converter(Image.open('images/unique_1.jpg'))
     image_duplicate_1 = image_converter(Image.open('images/Bead_necklace_1.jpg'))
     image_duplicate_2 = image_converter(Image.open('images/Bead_necklace_2.jpg'))
 
     e_d_u = euclidean_distance(image_unique, image_duplicate_1)
@@ -221,12 +266,18 @@
 
     c_s_u = cosine_similarity(image_unique, image_duplicate_1)
     c_s_d = cosine_similarity(image_duplicate_1, image_duplicate_2)
     c_s_d_d = cosine_similarity(image_duplicate_1, image_duplicate_1)
     report += (f"cosine_similarity unique: {c_s_u}\ncosine_similarity duplicate size_difference: {c_s_d}\n"
                f"cosine_similarity identical: {c_s_d_d}\n")
 
-    c_n_u = cnn.cnn(image_unique, image_duplicate_1)
-    c_n_d = cnn.cnn(image_duplicate_1, image_duplicate_2)
-    c_n_d_d = cnn.cnn(image_duplicate_1, image_duplicate_1)
-    report += f"CNN unique: {c_n_u}\nCNN duplicate size_difference: {c_n_d}\nCNN identical: {c_n_d_d}"
+    c_n_u = cnn.predict(image_unique, image_duplicate_1)
+    c_n_d = cnn.predict(image_duplicate_1, image_duplicate_2)
+    c_n_d_d = cnn.predict(image_duplicate_1, image_duplicate_1)
+    report += f"CNN unique: {c_n_u}\nCNN duplicate size_difference: {c_n_d}\nCNN identical: {c_n_d_d}\n"
+
+    d_d_u = dedup.predict(image_unique, image_duplicate_1)
+    d_d_d = dedup.predict(image_duplicate_1, image_duplicate_2)
+    d_d_d_d = dedup.predict(image_duplicate_1, image_duplicate_1)
+    report += (f"dedup unique: {d_d_u}\ndedup duplicate size_difference: {d_d_d}\n"
+               f"dedup duplicate identical: {d_d_d_d}")
     print(report)
```

### Comparing `antidupe-0.0.4/antidupe.egg-info/PKG-INFO` & `antidupe-0.0.5/antidupe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: SSIM-PIL
+Requires-Dist: imagededup
 Requires-Dist: matplotlib
 Requires-Dist: imagehash
 Requires-Dist: efficientnet_pytorch
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
@@ -61,18 +62,19 @@
 ### Customizing Thresholds
 
 You can customize the similarity thresholds for each technique during runtime or initialization:
 
 ```python
 # Initialize Antidupe with custom thresholds
 custom_thresholds = {
-    'ih': 0.2,   # Image Hash
-    'ssim': 0.2, # SSIM
-    'cs': 0.2,   # Cosine Similarity
-    'cnn': 0.2   # CNN
+    'ih': 0.2,    # Image Hash
+    'ssim': 0.2,  # SSIM
+    'cs': 0.2,    # Cosine Similarity
+    'cnn': 0.2,   # CNN
+    'dedup': 0.85 # Mobilenet
 }
 antidupe = Antidupe(limits=custom_thresholds)
 
 # Check for duplicates
 is_duplicate = antidupe.predict([image1, image2])
 ```
 
@@ -94,30 +96,34 @@
 
 ```python
 # Set new limits during runtime
 new_thresholds = {
     'ih': 0.1,
     'ssim': 0.1,
     'cs': 0.1,
-    'cnn': 0.1
+    'cnn': 0.1,
+    'dedup': 0.8
 }
 antidupe.set_limits(limits=new_thresholds)
 
 # Check for duplicates
 is_duplicate = antidupe.predict([image1, image2])
 ```
 
 ## Requirements
 
 - Python 3.x
+- SSIM PIL
+- ImageDeDup
 - NumPy
+- MatPlotLib
 - Pillow
-- imagehash
-- torch
-- efficientnet_pytorch
-- torchvision
+- ImageHash
+- Torch
+- Efficientnet Pytorch
+- TorchVision
 
 ---
 
 ## License
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `antidupe-0.0.4/setup.py` & `antidupe-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 except ImportError:
     import pip  # noqa
     pip.main(['install', 'install-preserve'])
     from install_preserve import preserve  # noqa
 
 install_requires = [
     'SSIM-PIL',
+    'imagededup',
     'matplotlib',
     'imagehash',
     'efficientnet_pytorch',
     'numpy',
     'Pillow',
     'torch>=2.0.0',
     'torchvision>=0.17.0',
@@ -27,15 +28,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='antidupe',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

