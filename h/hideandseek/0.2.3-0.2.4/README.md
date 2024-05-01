# Comparing `tmp/hideandseek-0.2.3.tar.gz` & `tmp/hideandseek-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hideandseek-0.2.3.tar", last modified: Tue Apr 23 18:13:54 2024, max compression
+gzip compressed data, was "hideandseek-0.2.4.tar", last modified: Wed May  1 16:22:58 2024, max compression
```

## Comparing `hideandseek-0.2.3.tar` & `hideandseek-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:13:54.724930 hideandseek-0.2.3/
--rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2757 2024-04-23 18:13:54.723929 hideandseek-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:13:54.679925 hideandseek-0.2.3/hideandseek/
--rw-rw-rw-   0        0        0      330 2024-04-23 18:13:36.000000 hideandseek-0.2.3/hideandseek/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.3/hideandseek/dataset.py
--rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.3/hideandseek/evaluation.py
--rw-rw-rw-   0        0        0    10064 2024-04-23 18:13:33.000000 hideandseek-0.2.3/hideandseek/fv.py
--rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.3/hideandseek/loss.py
--rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.3/hideandseek/model.py
--rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.3/hideandseek/plot.py
--rw-rw-rw-   0        0        0    24906 2024-04-22 20:07:36.000000 hideandseek-0.2.3/hideandseek/trainer.py
--rw-rw-rw-   0        0        0     4757 2024-04-22 19:32:15.000000 hideandseek-0.2.3/hideandseek/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:13:54.721946 hideandseek-0.2.3/hideandseek.egg-info/
--rw-rw-rw-   0        0        0     2757 2024-04-23 18:13:53.000000 hideandseek-0.2.3/hideandseek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-23 18:13:54.000000 hideandseek-0.2.3/hideandseek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:13:53.000000 hideandseek-0.2.3/hideandseek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-23 18:13:53.000000 hideandseek-0.2.3/hideandseek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-23 18:13:53.000000 hideandseek-0.2.3/hideandseek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 18:13:54.725930 hideandseek-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:22:58.110872 hideandseek-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2757 2024-05-01 16:22:58.108872 hideandseek-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:22:58.075727 hideandseek-0.2.4/hideandseek/
+-rw-rw-rw-   0        0        0      330 2024-05-01 16:22:41.000000 hideandseek-0.2.4/hideandseek/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.4/hideandseek/dataset.py
+-rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.4/hideandseek/evaluation.py
+-rw-rw-rw-   0        0        0    10064 2024-04-23 18:13:33.000000 hideandseek-0.2.4/hideandseek/fv.py
+-rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.4/hideandseek/loss.py
+-rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.4/hideandseek/model.py
+-rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.4/hideandseek/plot.py
+-rw-rw-rw-   0        0        0    24623 2024-05-01 16:22:32.000000 hideandseek-0.2.4/hideandseek/trainer.py
+-rw-rw-rw-   0        0        0     4757 2024-04-22 19:32:15.000000 hideandseek-0.2.4/hideandseek/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:22:58.106871 hideandseek-0.2.4/hideandseek.egg-info/
+-rw-rw-rw-   0        0        0     2757 2024-05-01 16:22:57.000000 hideandseek-0.2.4/hideandseek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-05-01 16:22:57.000000 hideandseek-0.2.4/hideandseek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:22:57.000000 hideandseek-0.2.4/hideandseek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-01 16:22:57.000000 hideandseek-0.2.4/hideandseek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 16:22:57.000000 hideandseek-0.2.4/hideandseek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:22:58.110872 hideandseek-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.4/setup.py
```

### Comparing `hideandseek-0.2.3/LICENSE` & `hideandseek-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/PKG-INFO` & `hideandseek-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.2.3
+Version: 0.2.4
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.2.3/README.md` & `hideandseek-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/dataset.py` & `hideandseek-0.2.4/hideandseek/dataset.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/evaluation.py` & `hideandseek-0.2.4/hideandseek/evaluation.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/fv.py` & `hideandseek-0.2.4/hideandseek/fv.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/loss.py` & `hideandseek-0.2.4/hideandseek/loss.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/model.py` & `hideandseek-0.2.4/hideandseek/model.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/plot.py` & `hideandseek-0.2.4/hideandseek/plot.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek/trainer.py` & `hideandseek-0.2.4/hideandseek/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # ]
 
 # %%
 log = logging.getLogger(__name__)
 
 # %%
 class Trainer:
-    def __init__(self, network, train_dataset=None, cfg_train={}, criterion=None, network_dir=None, model_dir=None, cfg_val=None, val_dataset=None, val_metrics=None, name='default', verbose=True, amp=False, reproduce=True):
+    def __init__(self, network, train_dataset=None, cfg_train={}, criterion=None, network_dir=None, cfg_val=None, val_dataset=None, val_metrics=None, name='default', verbose=True, amp=False, reproduce=True):
         '''
         Things Trainer do:
         - train network with early stopping, given hyperparameters
         - save/load network with necessary preprocessing pipeline
 
         :param network: torch.nn.Module object
         :param train_dataset: torch.utils.data.Dataset object
@@ -58,24 +58,23 @@
             criterion (optional, if val_metrics is dict for multiple metrics) 
 
         :param criterion: torch.nn.Module object, used to compute loss function
 
         Recommended way of making hs.node.Node object is like the following:
 
             kwargs = {'network': Network(), 'train_dataset': train_dataset, 'validation': None, 'cfg_train': cfg.train,
-                    'criterion': criterion, 'network_dir': path['network'], 'model_dir': path['node'], 'verbose': True, 'amp': True}
+                    'criterion': criterion, 'network_dir': path['network'], 'verbose': True, 'amp': True}
             node = hs.node.Node(**kwargs)
         '''
         # Store configurations
         self.network = network
         self.train_dataset = train_dataset
         self.cfg_train = dcopy(dict(cfg_train))
         self.criterion = criterion
         self.network_dir = network_dir
-        self.model_dir = model_dir
 
         self.cfg_val = dcopy(dict(cfg_val)) if cfg_val is not None else {}
         self.val_dataset = val_dataset
         self.val_metrics = val_metrics
         self.earlystopper = EarlyStopper(increase_better=cfg_val['increase_better'], patience=cfg_val['patience']) if self.val_dataset is not None else None
         if 'target_dataset' in self.cfg_val:
             if type(self.val_dataset)==dict:
@@ -88,18 +87,14 @@
         self.reproduce = reproduce
 
         # Initializations
         if self.network_dir is not None:
             if os.path.exists(self.network_dir): log.warning(f'path: {self.network_dir} exists. Be careful')
             os.makedirs(self.network_dir, exist_ok=True)
 
-        if self.model_dir is not None:
-            if os.path.exists(self.model_dir): log.warning(f'path: {self.model_dir} exists. Be careful')
-            os.makedirs(self.model_dir, exist_ok=True)
-
         self.train_meter = tools.modules.AverageMeter() # Tracks loss per epoch
         self.loss_tracker = tools.modules.ValueTracker() # Tracks loss over all training
         self.set_model()
         self.reset()
 
         self._targets_type = self.infer_targets_type()
 
@@ -454,19 +449,19 @@
         Save the following:
         state_dict() -> path/state_dict.p
         network.state_dict() -> path/network.pt
         '''
         path = self.network_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
-        self.print(f'[save] Saving Model info to: {state_dict_path}')
-        self.print(f'[save] state_dict: {list(state_dict.keys())}')
         state_dict_path = os.path.join(path, 'model.p')
         state_dict = self.state_dict()
         tools.save_pickle(state_dict, state_dict_path)
+        self.print(f'[save] Saving Model info to: {state_dict_path}')
+        self.print(f'[save] state_dict: {list(state_dict.keys())}')
 
         network_path = os.path.join(path, 'network.pt')
         if best:
             if self.earlystopper is None:
                 self.print(f'[save][best: {best}] earlystopper not defined. Saving current network -> [{network_path}]')
                 torch.save(self.network.state_dict(), network_path)
             else:
```

### Comparing `hideandseek-0.2.3/hideandseek/utils.py` & `hideandseek-0.2.4/hideandseek/utils.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.3/hideandseek.egg-info/PKG-INFO` & `hideandseek-0.2.4/hideandseek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.2.3
+Version: 0.2.4
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.2.3/setup.py` & `hideandseek-0.2.4/setup.py`

 * *Files identical despite different names*

