# Comparing `tmp/backgroundremover-0.2.7.tar.gz` & `tmp/backgroundremover-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backgroundremover-0.2.7.tar", last modified: Fri Apr 12 18:43:02 2024, max compression
+gzip compressed data, was "backgroundremover-0.2.8.tar", last modified: Wed May  1 21:43:58 2024, max compression
```

## Comparing `backgroundremover-0.2.7.tar` & `backgroundremover-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      183 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     6908 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     6409 2023-11-12 00:46:28.000000 backgroundremover-0.2.7/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.911448 backgroundremover-0.2.7/backgroundremover/
--rw-rw-r--   0 john      (1000) john      (1000)      175 2024-04-12 18:41:21.000000 backgroundremover-0.2.7/backgroundremover/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     7172 2023-12-06 01:26:54.000000 backgroundremover-0.2.7/backgroundremover/bg.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.915448 backgroundremover-0.2.7/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/cmd/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/cmd/server.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)    12566 2023-11-12 00:45:07.000000 backgroundremover-0.2.7/backgroundremover/utilities.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.915448 backgroundremover-0.2.7/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     6908 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      654 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       69 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      358 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)      230 2023-07-01 21:34:32.000000 backgroundremover-0.2.7/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)      358 2024-03-03 17:23:59.000000 backgroundremover-0.2.7/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       78 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1027 2024-04-12 18:41:32.000000 backgroundremover-0.2.7/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-01 21:43:58.258017 backgroundremover-0.2.8/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     7541 2024-05-01 21:43:58.258017 backgroundremover-0.2.8/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     7042 2024-05-01 21:36:37.000000 backgroundremover-0.2.8/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-01 21:43:58.254017 backgroundremover-0.2.8/backgroundremover/
+-rw-rw-r--   0 john      (1000) john      (1000)      175 2024-05-01 21:43:52.000000 backgroundremover-0.2.8/backgroundremover/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7160 2024-04-12 19:08:45.000000 backgroundremover-0.2.8/backgroundremover/bg.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-01 21:43:58.258017 backgroundremover-0.2.8/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/backgroundremover/cmd/server.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1750 2024-04-12 19:08:45.000000 backgroundremover-0.2.8/backgroundremover/github.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-01 21:43:58.258017 backgroundremover-0.2.8/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11553 2024-04-12 19:08:45.000000 backgroundremover-0.2.8/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4422 2024-05-01 21:36:37.000000 backgroundremover-0.2.8/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-07-01 21:34:29.000000 backgroundremover-0.2.8/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10843 2024-04-12 19:08:45.000000 backgroundremover-0.2.8/backgroundremover/utilities.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-05-01 21:43:58.258017 backgroundremover-0.2.8/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     7541 2024-05-01 21:43:58.000000 backgroundremover-0.2.8/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      682 2024-05-01 21:43:58.000000 backgroundremover-0.2.8/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-05-01 21:43:58.000000 backgroundremover-0.2.8/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       69 2024-05-01 21:43:58.000000 backgroundremover-0.2.8/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      358 2024-05-01 21:43:58.000000 backgroundremover-0.2.8/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       18 2024-05-01 21:43:58.000000 backgroundremover-0.2.8/backgroundremover.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2023-07-01 21:34:32.000000 backgroundremover-0.2.8/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      358 2024-03-03 17:23:59.000000 backgroundremover-0.2.8/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2024-05-01 21:43:58.262017 backgroundremover-0.2.8/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1027 2024-05-01 21:43:52.000000 backgroundremover-0.2.8/setup.py
```

### Comparing `backgroundremover-0.2.7/LICENSE.txt` & `backgroundremover-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.7/PKG-INFO` & `backgroundremover-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.7
+Version: 0.2.8
 Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 Keywords: remove,background,u2net,remove background,background remover
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,15 +23,15 @@
 * python >= 3.6
 * python3.6-dev #or what ever version of python you use
 * torch and torchvision stable version (https://pytorch.org)
 * ffmpeg 4.4+
 
 * To clarify, you must install both python and whatever dev version of python you installed. IE; python3.10-dev with python3.10 or python3.8-dev with python3.8
 
-#### How to install torch and fmpeg
+#### How to install torch and ffmpeg
 
 Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
 
 For example:
 
 ```
 PyTorch Build: Stable (1.7.1)
@@ -147,14 +147,35 @@
 backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
 ```
 change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
 ```bash
 backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
 ```
 
+## As a library
+### Remove background image
+
+```
+from backgroundremover.bg import remove
+def remove_bg(src_img_path, out_img_path):
+    model_choices = ["u2net", "u2net_human_seg", "u2netp"]
+    f = open(src_img_path, "rb")
+    data = f.read()
+    img = remove(data, model_name=model_choices[0],
+                 alpha_matting=True,
+                 alpha_matting_foreground_threshold=240,
+                 alpha_matting_background_threshold=10,
+                 alpha_matting_erode_structure_size=10,
+                 alpha_matting_base_size=1000)
+    f.close()
+    f = open(out_img_path, "wb")
+    f.write(img)
+    f.close()
+```
+
 ## Todo
 
 - convert logic from video to image to utilize more GPU on image removal
 - clean up documentation a bit more
 - add ability to adjust and give feedback images or videos to datasets
 - add ability to realtime background removal for videos, for streaming
 - finish flask server api
```

### Comparing `backgroundremover-0.2.7/README.md` & `backgroundremover-0.2.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * python >= 3.6
 * python3.6-dev #or what ever version of python you use
 * torch and torchvision stable version (https://pytorch.org)
 * ffmpeg 4.4+
 
 * To clarify, you must install both python and whatever dev version of python you installed. IE; python3.10-dev with python3.10 or python3.8-dev with python3.8
 
-#### How to install torch and fmpeg
+#### How to install torch and ffmpeg
 
 Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
 
 For example:
 
 ```
 PyTorch Build: Stable (1.7.1)
@@ -133,14 +133,35 @@
 backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
 ```
 change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
 ```bash
 backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
 ```
 
+## As a library
+### Remove background image
+
+```
+from backgroundremover.bg import remove
+def remove_bg(src_img_path, out_img_path):
+    model_choices = ["u2net", "u2net_human_seg", "u2netp"]
+    f = open(src_img_path, "rb")
+    data = f.read()
+    img = remove(data, model_name=model_choices[0],
+                 alpha_matting=True,
+                 alpha_matting_foreground_threshold=240,
+                 alpha_matting_background_threshold=10,
+                 alpha_matting_erode_structure_size=10,
+                 alpha_matting_base_size=1000)
+    f.close()
+    f = open(out_img_path, "wb")
+    f.write(img)
+    f.close()
+```
+
 ## Todo
 
 - convert logic from video to image to utilize more GPU on image removal
 - clean up documentation a bit more
 - add ability to adjust and give feedback images or videos to datasets
 - add ability to realtime background removal for videos, for streaming
 - finish flask server api
```

### Comparing `backgroundremover-0.2.7/backgroundremover/bg.py` & `backgroundremover-0.2.8/backgroundremover/bg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import moviepy.editor as mpy
 import numpy as np
 import torch
 import torch.nn.functional
 import torch.nn.functional
 from hsh.library.hash import Hasher
 from .u2net import detect, u2net
-from . import utilities
+from . import github
 
 # closes https://github.com/nadermx/backgroundremover/issues/18
 # closes https://github.com/nadermx/backgroundremover/issues/112
 try:
     if torch.cuda.is_available():
         DEVICE = torch.device('cuda:0')
     elif torch.backends.mps.is_available():
@@ -52,43 +52,43 @@
             path = os.environ.get(
                 "U2NETP_PATH",
                 os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
             )
             if (
                 not os.path.exists(path)
             ):
-                utilities.download_files_from_github(
+                github.download_files_from_github(
                     path, model_name
                 )
 
         elif model_name == "u2net":
             net = u2net.U2NET(3, 1)
             path = os.environ.get(
                 "U2NET_PATH",
                 os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
             )
             if (
                 not os.path.exists(path)
                 #or hasher.md5(path) != "09fb4e49b7f785c9f855baf94916840a"
             ):
-                utilities.download_files_from_github(
+                github.download_files_from_github(
                     path, model_name
                 )
 
         elif model_name == "u2net_human_seg":
             net = u2net.U2NET(3, 1)
             path = os.environ.get(
                 "U2NET_PATH",
                 os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
             )
             if (
                 not os.path.exists(path)
                 #or hasher.md5(path) != "347c3d51b01528e5c6c071e3cff1cb55"
             ):
-                utilities.download_files_from_github(
+                github.download_files_from_github(
                     path, model_name
                 )
         else:
             print("Choose between u2net, u2net_human_seg or u2netp", file=sys.stderr)
 
         net.load_state_dict(torch.load(path, map_location=torch.device(DEVICE)))
         net.to(device=DEVICE, dtype=torch.float32, non_blocking=True)
```

### Comparing `backgroundremover-0.2.7/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.8/backgroundremover/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.7/backgroundremover/cmd/server.py` & `backgroundremover-0.2.8/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.7/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.8/backgroundremover/u2net/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             tmpImg[:, :, 2] = (image[:, :, 2] - 0.406) / 0.225
 
         tmpLbl[:, :, 0] = label[:, :, 0]
 
         # change the r,g,b to b,r,g from [0,255] to [0,1]
         # transforms.Normalize(mean = (0.485, 0.456, 0.406), std = (0.229, 0.224, 0.225))
         tmpImg = tmpImg.transpose((2, 0, 1))
-        tmpLbl = label.transpose((2, 0, 1))
+        tmpLbl = tmpLbl.transpose((2, 0, 1))
 
         return {
             "imidx": torch.from_numpy(imidx),
             "image": torch.from_numpy(tmpImg),
             "label": torch.from_numpy(tmpLbl),
         }
```

### Comparing `backgroundremover-0.2.7/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.8/backgroundremover/u2net/detect.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import numpy as np
 import torch
 from hsh.library.hash import Hasher
 from PIL import Image
 from torchvision import transforms
 
 from . import data_loader, u2net
-from .. import utilities
+from .. import github
+
 
 def load_model(model_name: str = "u2net"):
     hasher = Hasher()
 
     model = {
         'u2netp': (u2net.U2NETP,
                    'e4f636406ca4e2af789941e7f139ee2e',
@@ -34,43 +35,46 @@
             "U2NETP_PATH",
             os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
         )
         if (
             not os.path.exists(path)
             #or hasher.md5(path) != "e4f636406ca4e2af789941e7f139ee2e"
         ):
-            utilities.download_files_from_github(
+            github.download_files_from_github(
                 path, model_name
             )
 
     elif model_name == "u2net":
         net = u2net.U2NET(3, 1)
         path = os.environ.get(
             "U2NET_PATH",
             os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
         )
+
+        print(f"DEBUG: path to be checked: {path}")
+
         if (
             not os.path.exists(path)
             #or hasher.md5(path) != "09fb4e49b7f785c9f855baf94916840a"
         ):
-            utilities.download_files_from_github(
+            github.download_files_from_github(
                 path, model_name
             )
 
     elif model_name == "u2net_human_seg":
         net = u2net.U2NET(3, 1)
         path = os.environ.get(
             "U2NET_PATH",
             os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
         )
         if (
             not os.path.exists(path)
             #or hasher.md5(path) != "347c3d51b01528e5c6c071e3cff1cb55"
         ):
-            utilities.download_files_from_github(
+            github.download_files_from_github(
                 path, model_name
             )
 
     else:
         print("Choose between u2net, u2net_human_seg or u2netp", file=sys.stderr)
 
     try:
@@ -143,9 +147,10 @@
         predict = norm_pred(pred)
 
         predict = predict.squeeze()
         predict_np = predict.cpu().detach().numpy()
         img = Image.fromarray(predict_np * 255).convert("RGB")
 
         del d1, d2, d3, d4, d5, d6, d7, pred, predict, predict_np, inputs_test, sample
+        torch.cuda.empty_cache() if torch.cuda.is_available() else None
 
         return img
```

### Comparing `backgroundremover-0.2.7/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.8/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.7/backgroundremover/utilities.py` & `backgroundremover-0.2.8/backgroundremover/utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -324,42 +324,7 @@
     sp.run(cmd)
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
     return
-
-def download_files_from_github(path, model_name):
-    if model_name not in ["u2net", "u2net_human_seg", "u2netp"]:
-        print("Invalid model name, please use 'u2net' or 'u2net_human_seg' or 'u2netp'")
-        return
-    print(f"downloading model [{model_name}] to {path} ...")
-    urls = []
-    if model_name == "u2net":
-        urls = ['https://github.com/nadermx/backgroundremover/raw/main/models/u2aa',
-                'https://github.com/nadermx/backgroundremover/raw/main/models/u2ab',
-                'https://github.com/nadermx/backgroundremover/raw/main/models/u2ac',
-                'https://github.com/nadermx/backgroundremover/raw/main/models/u2ad']
-    elif model_name == "u2net_human_seg":
-        urls = ['https://github.com/nadermx/backgroundremover/raw/main/models/u2haa',
-                'https://github.com/nadermx/backgroundremover/raw/main/models/u2hab',
-                'https://github.com/nadermx/backgroundremover/raw/main/models/u2hac',
-                'https://github.com/nadermx/backgroundremover/raw/main/models/u2had']
-    elif model_name == 'u2netp':
-        urls = ['https://github.com/nadermx/backgroundremover/raw/main/models/u2netp.pth']
-    try:
-        os.makedirs(os.path.expanduser("~/.u2net"), exist_ok=True)
-    except Exception as e:
-        print(f"Error creating directory: {e}")
-        return
-
-    try:
-
-        with open(path, 'wb') as out_file:
-            for i, url in enumerate(urls):
-                print(f'downloading part {i+1} of {model_name}')
-                part_content = requests.get(url)
-                out_file.write(part_content.content)
-                print(f'finished downloading part {i+1} of {model_name}')
-    except Exception as e:
-        print(e)
```

### Comparing `backgroundremover-0.2.7/backgroundremover.egg-info/PKG-INFO` & `backgroundremover-0.2.8/backgroundremover.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.7
+Version: 0.2.8
 Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 Keywords: remove,background,u2net,remove background,background remover
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,15 +23,15 @@
 * python >= 3.6
 * python3.6-dev #or what ever version of python you use
 * torch and torchvision stable version (https://pytorch.org)
 * ffmpeg 4.4+
 
 * To clarify, you must install both python and whatever dev version of python you installed. IE; python3.10-dev with python3.10 or python3.8-dev with python3.8
 
-#### How to install torch and fmpeg
+#### How to install torch and ffmpeg
 
 Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
 
 For example:
 
 ```
 PyTorch Build: Stable (1.7.1)
@@ -147,14 +147,35 @@
 backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
 ```
 change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
 ```bash
 backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
 ```
 
+## As a library
+### Remove background image
+
+```
+from backgroundremover.bg import remove
+def remove_bg(src_img_path, out_img_path):
+    model_choices = ["u2net", "u2net_human_seg", "u2netp"]
+    f = open(src_img_path, "rb")
+    data = f.read()
+    img = remove(data, model_name=model_choices[0],
+                 alpha_matting=True,
+                 alpha_matting_foreground_threshold=240,
+                 alpha_matting_background_threshold=10,
+                 alpha_matting_erode_structure_size=10,
+                 alpha_matting_base_size=1000)
+    f.close()
+    f = open(out_img_path, "wb")
+    f.write(img)
+    f.close()
+```
+
 ## Todo
 
 - convert logic from video to image to utilize more GPU on image removal
 - clean up documentation a bit more
 - add ability to adjust and give feedback images or videos to datasets
 - add ability to realtime background removal for videos, for streaming
 - finish flask server api
```

### Comparing `backgroundremover-0.2.7/backgroundremover.egg-info/SOURCES.txt` & `backgroundremover-0.2.8/backgroundremover.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 backgroundremover/__init__.py
 backgroundremover/bg.py
+backgroundremover/github.py
 backgroundremover/utilities.py
 backgroundremover.egg-info/PKG-INFO
 backgroundremover.egg-info/SOURCES.txt
 backgroundremover.egg-info/dependency_links.txt
 backgroundremover.egg-info/entry_points.txt
 backgroundremover.egg-info/requires.txt
 backgroundremover.egg-info/top_level.txt
```

### Comparing `backgroundremover-0.2.7/setup.py` & `backgroundremover-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.2.7",
+    version="0.2.8",
     description="Background remover from image and video using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
```

