# Comparing `tmp/pssr-1.1.1.tar.gz` & `tmp/pssr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.1.1.tar", max compression
+gzip compressed data, was "pssr-1.2.0.tar", max compression
```

## Comparing `pssr-1.1.1.tar` & `pssr-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.1.1/LICENSE
--rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.1.1/README.md
--rw-r--r--   0        0        0     4388 2024-04-26 16:18:41.417948 pssr-1.1.1/_pssr.py
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.1.1/pssr/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-26 04:19:02.573621 pssr-1.1.1/pssr/crappifiers.py
--rw-r--r--   0        0        0    32538 2024-04-26 16:07:25.348267 pssr-1.1.1/pssr/data.py
--rw-r--r--   0        0        0     2610 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/loss.py
--rw-r--r--   0        0        0       60 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/__init__.py
--rw-r--r--   0        0        0     1531 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/_blocks.py
--rw-r--r--   0        0        0     3449 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/resunet.py
--rw-r--r--   0        0        0     6143 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/resuneta.py
--rw-r--r--   0        0        0    11102 2024-04-26 16:28:39.578874 pssr-1.1.1/pssr/predict.py
--rw-r--r--   0        0        0    13012 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/train.py
--rw-r--r--   0        0        0     1125 2024-04-28 22:16:40.978868 pssr-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pssr-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.2.0/pssr/__init__.py
+-rw-r--r--   0        0        0     4934 2024-05-01 03:00:25.746754 pssr-1.2.0/pssr/__main__.py
+-rw-r--r--   0        0        0     4510 2024-04-26 04:19:02.573621 pssr-1.2.0/pssr/crappifiers.py
+-rw-r--r--   0        0        0    32491 2024-05-01 00:39:30.861136 pssr-1.2.0/pssr/data.py
+-rw-r--r--   0        0        0     2595 2024-04-27 20:27:44.061746 pssr-1.2.0/pssr/loss.py
+-rw-r--r--   0        0        0       84 2024-05-01 02:54:05.539283 pssr-1.2.0/pssr/models/__init__.py
+-rw-r--r--   0        0        0     4482 2024-04-30 02:37:25.112937 pssr-1.2.0/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     8121 2024-05-01 03:09:21.643561 pssr-1.2.0/pssr/models/_rdnet.py
+-rw-r--r--   0        0        0     7617 2024-05-01 03:09:33.671764 pssr-1.2.0/pssr/models/rdresunet.py
+-rw-r--r--   0        0        0     6955 2024-05-01 03:02:41.421290 pssr-1.2.0/pssr/models/resunet.py
+-rw-r--r--   0        0        0    11090 2024-05-01 02:20:11.913442 pssr-1.2.0/pssr/predict.py
+-rw-r--r--   0        0        0    12990 2024-04-27 20:27:14.761332 pssr-1.2.0/pssr/train.py
+-rw-r--r--   0        0        0     1197 2024-05-01 03:14:42.305162 pssr-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 pssr-1.2.0/PKG-INFO
```

### Comparing `pssr-1.1.1/LICENSE` & `pssr-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.1.1/README.md` & `pssr-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pssr-1.1.1/_pssr.py` & `pssr-1.2.0/pssr/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import torch, argparse, sys
+import sys
+sys.path.append("..")
+
+import torch, argparse
 from torch.nn import MSELoss
-from pssr.models import ResUNet, ResUNetA
+from pssr.models import ResUNet, ResUNetA, RDResUNet, RDResUNetA
 from pssr.data import ImageDataset, SlidingDataset, PairedImageDataset, PairedSlidingDataset
 from pssr.crappifiers import MultiCrappifier, Poisson, AdditiveGaussian, SaltPepper
 from pssr.loss import SSIMLoss
 from pssr.train import train_paired
 from pssr.predict import predict_images, test_metrics
 
 def _handle_declaration(arg, defaults, req=None):
@@ -21,15 +24,15 @@
     parser = argparse.ArgumentParser(prog="pssr", description="PSSR CLI for basic usage", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument("-t", "--train", action="store_true", help="enable train mode")
 
     parser.add_argument("-dp", "--data-path", type=str, help="specify dataset path")
     parser.add_argument("-dt", "--data-type", type=str, default="ImageDataset", help="specify dataset type")
     parser.add_argument("-mt", "--model-type", type=str, default="ResUNet", help="specify model type")
-    parser.add_argument("-mp", "--model-path", type=str, default="model.pth", help="specify model path")
+    parser.add_argument("-mp", "--model-path", type=str, help="specify model path")
 
     parser.add_argument("-e", "--epochs", type=int, default=10, help="specify number of training epochs")
     parser.add_argument("-b", "--batch-size", type=int, default=16, help="specify batch size")
     parser.add_argument("-lr", "--lr", type=float, default=1e-3, help="specify learning rate")
     parser.add_argument("-p", "--patience", type=int, default=3, help="specify learning rate decay patience")
     parser.add_argument("-mse", "--mse", action="store_true", help="use MSE loss instead of SSIM loss")
     parser.add_argument("-sl", "--save-losses", action="store_true", help="save training losses")
@@ -42,18 +45,25 @@
         parser.print_help(sys.stderr)
         return
     args = parser.parse_args()
 
     if "Paired" not in args.data_type and args.data_path is None:
         print("--data-path(-dp) must be provided for semi-synthetic datasets")
         return
+    
+    if args.model_path is None and not args.train:
+        print("--model-path(-mp) must be provided in predict mode")
+        return
 
-    model = _handle_declaration(args.model_type, ["ResUNet", "ResUNetA"])
+    model = _handle_declaration(args.model_type, ["ResUNet", "RDResUNet"])
     dataset = _handle_declaration(args.data_type, ["ImageDataset", "SlidingDataset"], 
         req=[f"'{args.data_path}'"] if args.train else [f'''{f"'{args.data_path}', " if "Paired" not in args.data_type else ""}val_split=1'''])
+    
+    print(f"\nModel:\n{_tab_string(model.extra_repr())}")
+    print(f"\nDataset:\n{_tab_string(str(dataset))}")
 
     if torch.cuda.is_available():
         device = "cuda"
         print("\nCUDA enabled device detected, running on GPU.")
     else:
         device = "cpu"
         print("\nCUDA enabled device NOT detected, running on CPU.")
@@ -79,16 +89,17 @@
             device=device,
             scheduler=scheduler,
             log_frequency=50,
             dataloader_kwargs=kwargs,
         )
         print("\nTraining complete!")
 
-        torch.save(model, args.model_path)
-        print(f"Saved trained model to {args.model_path}")
+        model_path = args.model_path if args.model_path else f"{model.__class__.__name__}_{losses[-1]:.3f}.pth"
+        torch.save(model.state_dict(), model_path)
+        print(f"Saved trained model to {model_path}")
 
         if args.save_losses:
             with open("train_loss.txt", "w") as file:
                 for loss in losses:
                     file.write(f"{loss}\n")
 
     else:
@@ -103,9 +114,14 @@
 
             print("\nMetrics:")
             for metric in metrics:
                 print(f"{metric}: {metrics[metric]}")
     
     print("\n")
 
+def _tab_string(text):
+    lines = text.split("\n")
+    indented_lines = ["\t" + line for line in lines]
+    return "\n".join(indented_lines)
+
 if __name__ == "__main__":
     run()
```

### Comparing `pssr-1.1.1/pssr/crappifiers.py` & `pssr-1.2.0/pssr/crappifiers.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.1/pssr/data.py` & `pssr-1.2.0/pssr/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
         if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
 
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
+        self.hr_files = sorted(glob.glob(Path(self.path, f"*.{extension}")))
         if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
 
         self.slices, max_size = [], 0
         for image_idx in range(len(self.hr_files)):
@@ -126,15 +126,15 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
         if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
         
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
+        self.hr_files = sorted(glob.glob(Path(self.path, f"*.{extension}")))
         if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
         if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
         self.stack = stack.upper()
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
@@ -212,16 +212,16 @@
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         for path in [self.hr_path, self.lr_path]:
             if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
         if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using ImageDataset instead.", stacklevel=2)
 
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
-        self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
+        self.hr_files = sorted(glob.glob(Path(self.hr_path, f"*.{extension}")))
+        self.lr_files = sorted(glob.glob(Path(self.lr_path, f"*.{extension}")))
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
             if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
         if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
 
@@ -299,16 +299,16 @@
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         for path in [self.hr_path, self.lr_path]:
             if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
         if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using SlidingDataset instead.", stacklevel=2)
         
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
-        self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
+        self.hr_files = sorted(glob.glob(Path(self.hr_path, f"*.{extension}")))
+        self.lr_files = sorted(glob.glob(Path(self.lr_path, f"*.{extension}")))
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
             if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
         if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
         if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
         self.stack = stack.upper()
@@ -495,25 +495,24 @@
         axes_idx = [out_axes.rfind(axis) for axis in slice_axes]
         image = np.moveaxis(image, range(len(image.shape)), axes_idx)
 
         # TODO: Assumes images must have all out_axes?
         # Disregard additional channels and/or reorder
         if mode == "L":
             image = np.mean(image, axis=2)
-        match stack:
-            case "T":
-                image = image[:,0]
-            case "Z":
-                image = image[0]
-            case "ZT":
-                image = np.moveaxis(image, 0, 1)
-            case "TZ":
-                pass
-            case _:
-                raise ValueError(f"Stack type {stack} is not valid.")
+        if stack == "T":
+            image = image[:,0]
+        elif stack == "Z":
+            image = image[0]
+        elif stack == "ZT":
+            image = np.moveaxis(image, 0, 1)
+        elif stack == "TZ":
+            pass
+        else:
+            raise ValueError(f"Stack type {stack} is not valid.")
         
         # Flatten channel dimensions
         image = np.reshape(image, [-1, image.shape[-2], image.shape[-1]])
         if image.max() != 0:
             image = image / (image.max() / 255)
         return image.astype(np.uint8)
     else:
```

### Comparing `pssr-1.1.1/pssr/loss.py` & `pssr-1.2.0/pssr/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,9 +53,9 @@
     Args:
         mse (float) : Mean squared error between predicted and ground truth images.
 
         image_range (int) : Value range of image. Default is 255.
     """
     return math.sqrt(mse) * image_range
 
-def _psnr_metric(mse : float, max : float):
-    return 20 * torch.log10(max / torch.sqrt(mse))
+def _psnr_metric(mse : float):
+    return 20 * torch.log10(1 / torch.sqrt(mse))
```

### Comparing `pssr-1.1.1/pssr/models/resunet.py` & `pssr-1.2.0/pssr/models/_blocks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,27 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ._blocks import Reconstruction
-from ..data import _force_list
+import numpy as np
 
-class ResUNet(nn.Module):
-    def __init__(self, channels : int = 1, hidden : list[int] = [64, 128, 256, 512, 1024], scale : int = 4, depth : int = 3):
-        r"""A modified Residual UNet as detailed in Zhang et al., 2017 with an additional image upscaling block.
-
-        Args:
-            channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
-
-            hidden (list[int]) : Elementwise list of hidden layer channels controlling width and length of model.
-
-            scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
-
-            depth (int) : Number of hidden layers per residual block. Default is 3.
-        """
+class Reconstruction(nn.Module):
+    def __init__(self, in_channels : int, out_channels : int, hidden : int, scale : int = 4):
         super().__init__()
-        channels = _force_list(channels)
-        channels = channels*2 if len(channels) == 1 else channels
-        
-        self.norm = nn.BatchNorm2d(channels[0])
-        
-        self.encoder, self.decoder, self.upscale = nn.ModuleList(), nn.ModuleList(), nn.ModuleList()
-        layers = [channels[0], *hidden]
-        n_layers = len(layers) - 1
-        for layer_idx in range(n_layers):
-            self.encoder.append(_ResBlock(in_channels=layers[layer_idx], out_channels=layers[layer_idx+1], depth=depth))
-            if layer_idx + 1 < n_layers:
-                self.decoder.append(_ResBlock(in_channels=layers[-layer_idx-1] - int(layers[-layer_idx-2]/2), out_channels=layers[-layer_idx-2], depth=depth))
-                self.upscale.append(nn.PixelShuffle(2))
-
-        self.reconstuction = Reconstruction(channels[0], channels[1], hidden[0], scale)
-
-    def forward(self, x):
-        x = x / 128 - 1 # Scale input approx from [0, 255] to [-1, 1]
-        x = self.norm(x)
-
-        skips = [x]
-        for idx, layer in enumerate(self.encoder):
-            x = layer(x) # ResBlock
 
-            if idx + 1 < len(self.encoder): # Downscale
-                skips.append(x)
-                x = F.max_pool2d(x, kernel_size=2)
+        self.pre = nn.Conv2d(in_channels=hidden + in_channels, out_channels=scale**2 * hidden, kernel_size=3, padding=1)
+        self.conv = nn.Conv2d(in_channels=hidden, out_channels=out_channels, kernel_size=3, padding=1)
 
-        for idx, layer in enumerate(self.decoder):
-            x = self.upscale[idx](x) # Upscale
+        self.scale = scale
 
-            x = torch.cat([x, skips.pop()], dim=1) # ResBlock
-            x = layer(x)
-
-        x = torch.cat([x, skips.pop()], dim=1) # Final skip connection before reconstruction
-        if len(skips) != 0: raise IndexError(f"Skip connection mismatch between encoder and decoder. {len(skips)} skip connections are unused.")
-
-        x = self.reconstuction(x)
-
-        x = x * 128 + 128 # Scale output approx from [-1, 1] to [0, 255]
+    def forward(self, x):
+        x = F.relu(self.pre(x), inplace=True)
+        x = self.conv(F.pixel_shuffle(x, self.scale))
         return x
     
-class _ResBlock(nn.Module):
+class ResBlock(nn.Module):
     def __init__(self, in_channels : int, out_channels : int, depth : int, norm : bool = True):
         super().__init__()
 
         self.conv = nn.Sequential()
         
         n_layers = max(depth, 0) + 1
         for layer_idx in range(n_layers):
@@ -73,10 +30,86 @@
             if norm:
                 self.conv.append(nn.BatchNorm2d(out_channels))
             if layer_idx + 1 < n_layers:
                 self.conv.append(nn.ReLU(inplace=True))
 
         self.respass = nn.Conv2d(in_channels, out_channels, kernel_size=1)
 
+        self.depth = depth
+
     def forward(self, x):
         x = F.relu(self.conv(x) + self.respass(x))
         return x
+
+class ResBlockA(nn.Module):
+    def __init__(self, in_channels : int, out_channels : int, dilations : list[int], depth : int, norm : bool = True):
+        super().__init__()
+
+        self.dilations = nn.ModuleList()
+        for dilation in dilations:
+            conv = nn.Sequential()
+
+            n_layers = max(depth, 0) + 1
+            for layer_idx in range(n_layers):
+                if norm:
+                    conv.append(nn.BatchNorm2d(in_channels if layer_idx == 0 else out_channels))
+                conv.append(nn.ReLU(inplace=True))
+
+                conv.append(nn.Conv2d(in_channels if layer_idx == 0 else out_channels, out_channels, kernel_size=3, padding="same", dilation=dilation))
+            self.dilations.append(conv)
+
+        self.respass = nn.Conv2d(in_channels, out_channels, kernel_size=1)
+
+        self.depth = depth
+
+    def forward(self, x):
+        x = F.relu(sum([conv(x) for conv in self.dilations]) + self.respass(x))
+        return x
+
+class PSP_Pooling(nn.Module):
+    def __init__(self, channels, sizes):
+        super().__init__()
+
+        small = channels//len(sizes)
+        self.convs = nn.ModuleList([nn.Sequential(nn.Conv2d(small, small, kernel_size=1), nn.BatchNorm2d(small)) for size in sizes])
+
+        self.conv_out = nn.Conv2d(channels, channels, kernel_size=1)
+        self.norm_out = nn.BatchNorm2d(channels)
+
+        self.sizes = sizes
+
+    def forward(self, x):
+        size = x.shape[-2:]
+
+        # Split x along sizes and apply poolings
+        x = torch.chunk(x, chunks=len(self.sizes), dim=1)
+        x = [F.interpolate(input=F.max_pool2d(x_chunk, kernel_size=self.sizes[idx]), size=size, mode="bilinear") for idx, x_chunk in enumerate(x)]
+        x = [F.relu(self.convs[idx](x_chunk)) for idx, x_chunk in enumerate(x)]
+        x = torch.concat(x, dim=1)
+
+        x = F.relu(self.norm_out(self.conv_out(x)))
+        return x
+
+class GradHist(nn.Module):
+    # https://discuss.pytorch.org/t/differentiable-torch-histc/25865/38
+    def __init__(self, bins : int = 512, range : list[int, int] = (-256, 256), sigma : int = 5):
+        super().__init__()
+        assert range[1] > range[0]
+        
+        self.delta = float(range[1]-range[0]) / float(bins)
+        self.centers = float(range[0]) + self.delta * (torch.arange(bins).float() + 0.5)
+
+        self.sigma = sigma
+
+    def forward(self, x):
+        batch, size = x.shape[0], np.prod(x.shape[2:])
+        x = x.flatten(start_dim=1)[:, np.newaxis, :] - self.centers[:, np.newaxis].to(device=x.device)
+        x = torch.sigmoid(x * self.sigma)
+        diff = torch.cat([torch.ones((batch, 1, size), device=x.device), x], dim=1) - torch.cat([x, torch.zeros((batch, 1, size), device=x.device)], dim=1)
+
+        diff = diff.sum(dim=-1)
+        return diff[:, :-1]
+    
+def get_resblock(in_channels : int, out_channels : int, dilations : list[int], depth : int, norm : bool = True):
+    if dilations:
+        return ResBlockA(in_channels, out_channels, dilations, depth, norm)
+    return ResBlock(in_channels, out_channels, depth, norm)
```

### Comparing `pssr-1.1.1/pssr/models/resuneta.py` & `pssr-1.2.0/pssr/models/resunet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,128 +1,139 @@
-import torch, warnings
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ._blocks import Reconstruction
+from ._blocks import PSP_Pooling, Reconstruction, get_resblock
 from ..data import _force_list
 
-class ResUNetA(nn.Module):
-    def __init__(self, channels : int = 1, hidden : list[int] = [64, 128, 256, 512, 1024], scale : int = 4, depth : int = 3, dilations : list[list[int]] = [[1,3,15,31],[1,3,15],[1,3],[1],[1]], pool_sizes : list[int] = [1, 2, 4, 8], encoder_pool : bool = False):
-        r"""A modified Atrous Residual UNet as detailed in Diakogiannis et al., 2019 with an additional image upscaling block.
+class ResUNet(nn.Module):
+    def __init__(
+            self,
+            channels : int = 1,
+            hidden : list[int] = [64, 128, 256, 512, 1024],
+            scale : int = 4,
+            depth : int = 3,
+            dilations : list[list[int]] = None,
+            pool_sizes : list[int] = None,
+            encoder_pool : bool = False,
+        ):
+        r"""A Residual UNet as detailed in Zhang et al., 2017 with an additional image upscaling block.
+        If ``dilations`` is provided, instead use a Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
 
-        Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by len(pool_sizes).
+        Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by pool_sizes.
 
         Args:
             channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
 
-            hidden (list[int]) : Elementwise list of hidden layer channels controlling width and length of model.
+            hidden (list[int]) : Elementwise list of channels per residual block controlling width and length of model.
 
             scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
             depth (int) : Number of hidden layers per residual block. Default is 3.
 
-            dilations (list[list[int]]) : List of dilation values per layer. If value is none, atrous convolutions will not be used.
+            dilations (list[list[int]]) : List of dilation values per layer. If value is None, atrous convolutions will not be used. Default is None.
 
-            pool_sizes (list[int]) : Pooling ratios for PSP pooling.
+            pool_sizes (list[int]) : Pooling ratios for PSP pooling. If value is None, PSP pooling will not be used. Default is None.
 
-            encoder_pool (bool) : Whether to include PSP pooling layer at end of encoder. Should not be used if last layer has a size of less than 16 pixels. Default is False.
+            encoder_pool (bool) : Whether to include additional PSP pooling layer at end of encoder. Should not be used if last layer has a size of less than 16 pixels. Default is False.
         """
         super().__init__()
         channels = _force_list(channels)
         channels = channels*2 if len(channels) == 1 else channels
 
-        if dilations is None:
-            warnings.warn("dilations is None, atrous convolutions will not be used.", stacklevel=2)
-            dilations = [1]*len(hidden)
-        if len(dilations) != len(hidden): raise ValueError(f"len(dilations) must equal len(hidden). Lengths are {len(dilations)} and {len(hidden)}.")
-        if hidden[0] % len(pool_sizes) != 0: raise ValueError(f"hidden[0] must be divisible by len(pool_sizes). Sizes are {hidden[0]} and {len(pool_sizes)}.")
-        if hidden[-1] % len(pool_sizes) != 0 and encoder_pool: raise ValueError(f"hidden[-1] must be divisible by len(pool_sizes) if encoder_pool is True. Sizes are {hidden[-1]} and {len(pool_sizes)}.")
-        
-        self.encoder, self.decoder, self.upscale = nn.ModuleList(), nn.ModuleList(), nn.ModuleList()
+        if dilations and len(dilations) != len(hidden): raise ValueError(f"Amount of dilations must equal amount of hidden residual blocks. Given values are {len(dilations)} and {len(hidden)} respectively.")
+
+        if pool_sizes:
+            if hidden[0] % len(pool_sizes) != 0: raise ValueError(f"hidden[0] must be divisible by len(pool_sizes). Given values are {hidden[0]} and {len(pool_sizes)} respectively.")
+            if encoder_pool and hidden[-1] % len(pool_sizes) != 0: raise ValueError(f"hidden[-1] must be divisible by len(pool_sizes) if encoder_pool is True. Given values are {hidden[-1]} and {len(pool_sizes)} respectively.")
+        else:
+            if encoder_pool: raise ValueError(f"encoder_pool cannot be True if pool_sizes are not provided.")
+
+        self.norm = nn.BatchNorm2d(channels[0]) if not dilations else None
+
+        self.encoder, self.decoder = nn.ModuleList(), nn.ModuleList()
         layers = [channels[0], *hidden]
         n_layers = len(layers) - 1
         for layer_idx in range(n_layers):
-            self.encoder.append(_ResBlockA(in_channels=layers[layer_idx], out_channels=layers[layer_idx+1], dilations=dilations[layer_idx], depth=depth))
+            self.encoder.append(get_resblock(in_channels=layers[layer_idx], out_channels=layers[layer_idx+1], dilations=dilations[layer_idx] if dilations else None, depth=depth))
             if layer_idx + 1 < n_layers:
-                self.decoder.append(_ResBlockA(in_channels=layers[-layer_idx-1] - int(layers[-layer_idx-2]/2), out_channels=layers[-layer_idx-2], dilations=dilations[-layer_idx-1], depth=depth))
-                self.upscale.append(nn.PixelShuffle(2))
+                self.decoder.append(get_resblock(in_channels=layers[-layer_idx-1]-int(layers[-layer_idx-2]/2), out_channels=layers[-layer_idx-2], dilations=dilations[-layer_idx-1] if dilations else None, depth=depth))
 
-        self.encoder_pool = _PSP_Pooling(hidden[-1], pool_sizes) if encoder_pool else None
-        self.reconstuction_pool = _PSP_Pooling(hidden[0], pool_sizes)
+        self.encoder_pool = PSP_Pooling(hidden[-1], pool_sizes) if pool_sizes and encoder_pool else None
+        self.reconstruction_pool = PSP_Pooling(hidden[0], pool_sizes) if pool_sizes else None
 
-        self.reconstuction = Reconstruction(channels[0], channels[1], hidden[0], scale)
+        self.reconstruction = Reconstruction(channels[0], channels[1], hidden[0], scale)
 
     def forward(self, x):
         x = x / 128 - 1 # Scale input approx from [0, 255] to [-1, 1]
+        if self.norm is not None:
+            x = self.norm(x)
 
         skips = [x]
         for idx, layer in enumerate(self.encoder):
             x = layer(x) # ResBlock
 
             if idx + 1 < len(self.encoder): # Downscale
                 skips.append(x)
                 x = F.max_pool2d(x, kernel_size=2)
-        
+
         if self.encoder_pool is not None:
             x = self.encoder_pool(x)
 
         for idx, layer in enumerate(self.decoder):
-            x = self.upscale[idx](x) # Upscale
+            x = x = F.pixel_shuffle(x, 2) # Upscale
 
             x = torch.cat([x, skips.pop()], dim=1) # ResBlock
             x = layer(x)
 
-        x = self.reconstuction_pool(x)
+        if self.reconstruction_pool is not None:
+            x = self.reconstruction_pool(x)
 
         x = torch.cat([x, skips.pop()], dim=1) # Final skip connection before reconstruction
         if len(skips) != 0: raise IndexError(f"Skip connection mismatch between encoder and decoder. {len(skips)} skip connections are unused.")
 
-        x = self.reconstuction(x)
+        x = self.reconstruction(x)
 
         x = x * 128 + 128 # Scale output approx from [-1, 1] to [0, 255]
         return x
+    
+    def extra_repr(self):
+        return f"{'Atrous ' if self.norm is None else ''}ResUNet with {self.reconstruction.scale}x upscaling\n{len(self.encoder)} residual decoder blocks with {self.encoder[0].depth} hidden layers each\nPSP pooling {'enabled' if self.reconstruction_pool else 'disabled'}"
+
+class ResUNetA():
+    def __new__(cls,
+            channels : int = 1,
+            hidden : list[int] = [64, 128, 256, 512, 1024],
+            scale : int = 4,
+            depth : int = 3,
+            dilations : list[list[int]] = [[1,3,15,31],[1,3,15],[1,3],[1],[1]],
+            pool_sizes : list[int] = [1, 2, 4, 8],
+            encoder_pool : bool = False,
+        ):
+        r""":class:`ResUNet` wrapper of Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
+        Provides alternative default arguments for an atrous network.
 
-class _ResBlockA(nn.Module):
-    def __init__(self, in_channels : int, out_channels : int, dilations : list[int], depth : int, norm : bool = True):
-        super().__init__()
-
-        self.dilations = nn.ModuleList()
-        for dilation in dilations:
-            conv = nn.Sequential()
-
-            n_layers = max(depth, 0) + 1
-            for layer_idx in range(n_layers):
-                if norm:
-                    conv.append(nn.BatchNorm2d(in_channels if layer_idx == 0 else out_channels))
-                conv.append(nn.ReLU(inplace=True))
-
-                conv.append(nn.Conv2d(in_channels if layer_idx == 0 else out_channels, out_channels, kernel_size=3, padding="same", dilation=dilation))
-            self.dilations.append(conv)
-
-        self.respass = nn.Conv2d(in_channels, out_channels, kernel_size=1)
+        Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by pool_sizes.
 
-    def forward(self, x):
-        x = F.relu(sum([conv(x) for conv in self.dilations]) + self.respass(x))
-        return x
-
-class _PSP_Pooling(nn.Module):
-    def __init__(self, channels, sizes):
-        super().__init__()
+        Args:
+            channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
 
-        small = channels//len(sizes)
-        self.convs = nn.ModuleList([nn.Sequential(nn.Conv2d(small, small, kernel_size=1), nn.BatchNorm2d(small)) for size in sizes])
+            hidden (list[int]) : Elementwise list of channels per residual block controlling width and length of model.
 
-        self.conv_out = nn.Conv2d(channels, channels, kernel_size=1)
-        self.norm_out = nn.BatchNorm2d(channels)
+            scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
-        self.sizes = sizes
+            depth (int) : Number of hidden layers per residual block. Default is 3.
 
-    def forward(self, x):
-        size = x.shape[-2:]
+            dilations (list[list[int]]) : List of dilation values per layer. If value is None, atrous convolutions will not be used. Default is [[1,3,15,31],[1,3,15],[1,3],[1],[1]].
 
-        # Split x along sizes and apply poolings
-        x = torch.chunk(x, chunks=len(self.sizes), dim=1)
-        x = [F.interpolate(input=F.max_pool2d(x_chunk, kernel_size=self.sizes[idx]), size=size, mode='bilinear') for idx, x_chunk in enumerate(x)]
-        x = [F.relu(self.convs[idx](x_chunk)) for idx, x_chunk in enumerate(x)]
-        x = torch.concat(x, dim=1)
+            pool_sizes (list[int]) : Pooling ratios for PSP pooling. If value is None, PSP pooling will not be used. Default is [1, 2, 4, 8].
 
-        x = F.relu(self.norm_out(self.conv_out(x)))
-        return x
+            encoder_pool (bool) : Whether to include additional PSP pooling layer at end of encoder. Should not be used if last layer has a size of less than 16 pixels. Default is False.
+        """
+        return ResUNet(
+            channels,
+            hidden,
+            scale,
+            depth,
+            dilations,
+            pool_sizes,
+            encoder_pool,
+        )
```

### Comparing `pssr-1.1.1/pssr/predict.py` & `pssr-1.2.0/pssr/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch, os, tifffile
 import torch.nn as nn
 import numpy as np
-from torch.utils.data import DataLoader, Dataset
+from torch.utils.data import Dataset
 from skimage.metrics import peak_signal_noise_ratio, structural_similarity
 from skimage.transform import resize
 from tqdm import tqdm
 from PIL import Image
 from .data import _RandomIterIdx, _slice_center
 from .loss import pixel_metric
```

### Comparing `pssr-1.1.1/pssr/train.py` & `pssr-1.2.0/pssr/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             optim.step()
             optim.zero_grad()
 
             if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
                 losses.append(loss.item())
 
                 mse = nn.functional.mse_loss(hr_hat/image_range, hr/image_range)
-                progress.set_description(f"pixel[{pixel_metric(mse, image_range):.2f}], psnr[{_psnr_metric(mse, hr.max()/image_range):.2f}], ssim[{ssim(hr_hat, hr, data_range=image_range):.3f}]")
+                progress.set_description(f"pixel[{pixel_metric(mse, image_range):.2f}], psnr[{_psnr_metric(mse):.2f}], ssim[{ssim(hr_hat, hr, data_range=image_range):.3f}]")
 
         # Validation
         model.eval()
 
         val_loss = []
         progress = tqdm(val_dataloader)
         progress.set_description(f"Epoch {epoch} validation...")
```

### Comparing `pssr-1.1.1/pyproject.toml` & `pssr-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pssr"
-version = "1.1.1"
+version = "1.2.0"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ucsdmanorlab/PSSR"
 documentation = "https://ucsdmanorlab.github.io/PSSR/"
 classifiers = [
@@ -14,28 +14,32 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Environment :: GPU :: NVIDIA CUDA",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Documentation :: Sphinx",
 ]
-include = ["_pssr.py"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 torch = "^2.0.0"
 numpy = "^1.26.4"
 pillow = "^10.2.0"
 czifile = "^2019.7.2"
 tifffile = "^2024.4.24"
-scikit-image = "^0.23.1"
+scikit-image = ">=0.18.0"
 scikit-optimize = "^0.9.0"
 tqdm = "^4.66.2"
 pytorch-msssim = "^1.0.0"
 psutil = "^5.9.8"
 
+timm = {version = "^0.9.12", optional = true}
+
+[tool.poetry.extras]
+models = ["timm"]
+
 [tool.poetry.scripts]
-pssr = "_pssr:run"
+pssr = "pssr.__main__:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pssr-1.1.1/PKG-INFO` & `pssr-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.1.1
+Version: 1.2.0
 Summary: Point-Scanning Super-Resolution
 Home-page: https://github.com/ucsdmanorlab/PSSR
 License: MIT
 Author: Hayden Stites
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
+Provides-Extra: models
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pytorch-msssim (>=1.0.0,<2.0.0)
-Requires-Dist: scikit-image (>=0.23.1,<0.24.0)
+Requires-Dist: scikit-image (>=0.18.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
 Requires-Dist: tifffile (>=2024.4.24,<2025.0.0)
+Requires-Dist: timm (>=0.9.12,<0.10.0) ; extra == "models"
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Documentation, https://ucsdmanorlab.github.io/PSSR/
 Project-URL: Repository, https://github.com/ucsdmanorlab/PSSR
 Description-Content-Type: text/markdown
 
 # Point-Scanning Super-Resolution (**PSSR**)
```

