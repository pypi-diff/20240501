# Comparing `tmp/potatorch-0.0.3.tar.gz` & `tmp/potatorch-0.0.4.tar.gz`

## Comparing `potatorch-0.0.3.tar` & `potatorch-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 potatorch-0.0.3/.dockerignore
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 potatorch-0.0.3/Dockerfile.gpu
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 potatorch-0.0.3/build.sh
--rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 potatorch-0.0.3/run.sh
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 potatorch-0.0.3/setup.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 potatorch-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0 12024910 2020-02-02 00:00:00.000000 potatorch-0.0.3/docs/potatorch-banner.png
--rw-r--r--   0        0        0   277664 2020-02-02 00:00:00.000000 potatorch-0.0.3/docs/potatorch.png
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 potatorch-0.0.3/examples/grid_search.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 potatorch-0.0.3/examples/mlp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/__init__.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/callbacks.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/training.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/datasets/FilteredDataset.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/datasets/__init__.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/datasets/utils.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/losses/MSRELoss.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/losses/WDLLoss.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/losses/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/models/__init__.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/models/cnn.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/optimization/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/optimization/bayesian_optimizer.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/optimization/tuning.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 potatorch-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 potatorch-0.0.3/LICENSE
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 potatorch-0.0.3/README.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 potatorch-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 potatorch-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 potatorch-0.0.4/.dockerignore
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 potatorch-0.0.4/Dockerfile.gpu
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 potatorch-0.0.4/build.sh
+-rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 potatorch-0.0.4/run.sh
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 potatorch-0.0.4/setup.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 potatorch-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  1065315 2020-02-02 00:00:00.000000 potatorch-0.0.4/docs/potatorch-banner.png
+-rw-r--r--   0        0        0   277664 2020-02-02 00:00:00.000000 potatorch-0.0.4/docs/potatorch.png
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 potatorch-0.0.4/examples/grid_search.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 potatorch-0.0.4/examples/mlp.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 potatorch-0.0.4/examples/mnist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/__init__.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/callbacks.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/training.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/datasets/FilteredDataset.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/datasets/__init__.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/datasets/utils.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/losses/MSRELoss.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/losses/WDLLoss.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/losses/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/models/__init__.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/models/cnn.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/optimization/__init__.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/optimization/bayesian_optimizer.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 potatorch-0.0.4/src/potatorch/optimization/tuning.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 potatorch-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 potatorch-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 potatorch-0.0.4/README.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 potatorch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 potatorch-0.0.4/PKG-INFO
```

### Comparing `potatorch-0.0.3/.github/workflows/python-publish.yml` & `potatorch-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/docs/potatorch.png` & `potatorch-0.0.4/docs/potatorch.png`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/examples/grid_search.py` & `potatorch-0.0.4/examples/grid_search.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/examples/mlp.py` & `potatorch-0.0.4/examples/mlp.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Define your model as a pytorch Module
 model = nn.Sequential(nn.Linear(1, 128), nn.ReLU(), 
         nn.Linear(128, 128), nn.ReLU(),
         nn.Linear(128, 1))
 
 # Create your dataset as a torch.data.Dataset
-dataset = TensorDataset(torch.arange(1000).view(1000, 1), torch.sin(torch.arange(1000)))
+dataset = TensorDataset(torch.arange(1000).view(1000, 1), torch.sin(torch.arange(1000).view(1000, 1)))
 
 # Provide a loss function and an optimizer
 loss_fn = torch.nn.MSELoss()
 optimizer = make_optimizer(torch.optim.Adam, lr=lr)
 
 # Construct a TrainingLoop object.
 # TrainingLoop handles the initialization of dataloaders, dataset splitting,
```

### Comparing `potatorch-0.0.3/src/potatorch/callbacks.py` & `potatorch-0.0.4/src/potatorch/callbacks.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/training.py` & `potatorch-0.0.4/src/potatorch/training.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from contextlib import ExitStack
 import numpy as np
 import gc
 
 def make_optimizer(optimizer_init: callable, *args, **kwargs):
     return lambda m: optimizer_init(m.parameters(), *args, **kwargs)
 
+# TODO: args filter for evaluation metrics
 class TrainingLoop():
     def __init__(self,
                  dataset,
                  loss_fn,
                  optimizer_fn,
                  train_p=0.7,
                  val_p=0.15,
@@ -23,36 +24,42 @@
                  random_split=True,
                  batch_size=1024,
                  shuffle=False,
                  random_subsampling=None,
                  filter_fn=None,
                  num_workers=4,
                  mixed_precision=False,
+                 loss_arg_filter=None,
                  callbacks=[],
                  val_metrics={},
                  device='cpu',
                  seed=42):
+        
         self.dataset = dataset
         self.loss_fn = loss_fn
         self.optimizer_fn = optimizer_fn
         self.train_p = train_p
         self.val_p = val_p
         self.test_p = test_p
         self.random_split = random_split
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.random_subsampling = random_subsampling
         self.filter_fn = filter_fn
         self.num_workers = num_workers
         self.device = device
         self.mixed_precision = mixed_precision
+        self.loss_arg_filter = loss_arg_filter
         self.callbacks = callbacks
         self.val_metrics = val_metrics
         self.device = device
         self.seed = 42
+        
+        if not self.loss_arg_filter:
+            self.loss_arg_filter = lambda x, pred, y: (pred, *y)
 
         self._clear_state()
         self._init_dataloaders()
 
     def _clear_state(self):
         """ Clear internal training state """
         self.state = {}
@@ -128,30 +135,33 @@
         initial_epoch = self.get_state('epoch', 1)
 
         for epoch in range(initial_epoch, initial_epoch + epochs):
             self.on_train_epoch_start(epoch)
 
             self.model.train()
             # TODO: provide interface to more than one input
-            for batch, (X, y) in enumerate(self.train_dataloader):
+            for batch, (X, *ys) in enumerate(self.train_dataloader):
                 self.on_train_batch_start(batch)
                 # TODO: generalize variable type
                 # TODO: memory_format (e.g. torch.channels_last for 4D tensors)
                 X = X.float().to(self.device, non_blocking=True)
-                y = y.float().to(self.device, non_blocking=True)
+                
+                if ys and not isinstance(ys, torch.Tensor) > 0:
+                    ys = [y.float().to(self.device, non_blocking=True) for y in ys]
 
                 # Clear gradients
                 self.optimizer.zero_grad(set_to_none=True)
 
                 # Forward pass
                 with ExitStack() as stack:
                     if self.mixed_precision:
                         stack.enter_context(torch.cuda.amp.autocast())
-                pred = self.model(X).squeeze()
-                loss = self.loss_fn(pred, y)
+                pred = self.model(X)
+                # loss = self.loss_fn(pred, target)
+                loss = self.loss_fn(*self.loss_arg_filter(X, pred, ys))
 
                 # Backpropagation
                 if self.mixed_precision:
                     scaler.scale(loss).backward()
                     scaler.step(self.optimizer)
                     scaler.update()
                 else:
@@ -169,23 +179,26 @@
     def _test(self, dataloader, metrics):
         num_batches = len(dataloader)
         self.model.eval()
         test_loss = 0.0
         test_metrics = dict.fromkeys(metrics.keys(), 0.0)
         # test_metrics = [0.0 for _ in metrics.keys()]
         with torch.no_grad():
-            for X, y in dataloader:
+            for (X, *ys) in dataloader:
                 # TODO: generalize variable type
                 X = X.float().to(self.device, non_blocking=True)
-                y = y.float().to(self.device, non_blocking=True)
-
-                pred = self.model(X).squeeze().detach()
-                test_loss += self.loss_fn(pred, y).detach()
+                
+                if ys and not isinstance(ys, torch.Tensor) > 0:
+                    ys = [y.float().to(self.device, non_blocking=True) for y in ys]
+
+                # pred = self.model(X).squeeze().detach()
+                pred = self.model(X)
+                test_loss += self.loss_fn(*self.loss_arg_filter(X, pred, ys)).detach()
                 for name, fn in metrics.items():
-                    test_metrics[name] += fn(pred, y).detach()
+                    test_metrics[name] += fn(pred, *ys).detach()
 
         test_loss /= num_batches
         test_metrics = {k: v / num_batches for k, v in test_metrics.items()}
         return test_loss, test_metrics
 
     def predict(self, data):
         """ Run inference over a set of datapoints,
```

### Comparing `potatorch-0.0.3/src/potatorch/datasets/FilteredDataset.py` & `potatorch-0.0.4/src/potatorch/datasets/FilteredDataset.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/datasets/utils.py` & `potatorch-0.0.4/src/potatorch/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/losses/MSRELoss.py` & `potatorch-0.0.4/src/potatorch/losses/MSRELoss.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/losses/WDLLoss.py` & `potatorch-0.0.4/src/potatorch/losses/WDLLoss.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/models/cnn.py` & `potatorch-0.0.4/src/potatorch/models/cnn.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/optimization/bayesian_optimizer.py` & `potatorch-0.0.4/src/potatorch/optimization/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/src/potatorch/optimization/tuning.py` & `potatorch-0.0.4/src/potatorch/optimization/tuning.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/.gitignore` & `potatorch-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/LICENSE` & `potatorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/README.md` & `potatorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.3/pyproject.toml` & `potatorch-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "potatorch"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Marco Pampaloni", email="marco.pampaloni1@gmail.com" },
 ]
 description = "Lightweight high-level PyTorch framework that runs on potato machines"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `potatorch-0.0.3/PKG-INFO` & `potatorch-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: potatorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lightweight high-level PyTorch framework that runs on potato machines
 Project-URL: Homepage, https://github.com/crybot/potatorch
 Project-URL: Bug Tracker, https://github.com/crybot/potatorch/issues
 Author-email: Marco Pampaloni <marco.pampaloni1@gmail.com>
 License-File: LICENSE
 Keywords: deep learning,framework,limited resources,machine learning,python,pytorch
 Classifier: License :: OSI Approved :: MIT License
```

