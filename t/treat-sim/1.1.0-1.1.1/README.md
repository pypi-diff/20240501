# Comparing `tmp/treat-sim-1.1.0.tar.gz` & `tmp/treat_sim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat-sim-1.1.0.tar", last modified: Sat Apr  6 15:43:35 2024, max compression
+gzip compressed data, was "treat_sim-1.1.1.tar", last modified: Wed May  1 16:04:26 2024, max compression
```

## Comparing `treat-sim-1.1.0.tar` & `treat_sim-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 15:43:31.000000 treat-sim-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 15:43:31.000000 treat-sim-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-06 15:43:35.280857 treat-sim-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-06 15:43:31.000000 treat-sim-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-06 15:43:31.000000 treat-sim-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:43:35.280857 treat-sim-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-06 15:43:31.000000 treat-sim-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/treat_sim/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/treat_sim/data/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/data/ed_arrivals.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/treat_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-01 16:04:22.000000 treat_sim-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 16:04:22.000000 treat_sim-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-01 16:04:26.666568 treat_sim-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-01 16:04:22.000000 treat_sim-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 16:04:22.000000 treat_sim-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:04:26.666568 treat_sim-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-01 16:04:22.000000 treat_sim-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/treat_sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/treat_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/data/ed_arrivals.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38338 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/treat_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/top_level.txt
```

### Comparing `treat-sim-1.1.0/LICENSE` & `treat_sim-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `treat-sim-1.1.0/PKG-INFO` & `treat_sim-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat-sim
-Version: 1.1.0
+Version: 1.1.1
 Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
 Home-page: https://github.com/pythonhealthdatascience/stars-treat-sim
 Author: Thomas Monks
 Author-email: forecast-tools@gmail.com
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `treat-sim-1.1.0/README.md` & `treat_sim-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `treat-sim-1.1.0/setup.py` & `treat_sim-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `treat-sim-1.1.0/treat_sim/distributions.py` & `treat_sim-1.1.1/treat_sim/distributions.py`

 * *Files identical despite different names*

### Comparing `treat-sim-1.1.0/treat_sim/model.py` & `treat_sim-1.1.1/treat_sim/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,21 +296,21 @@
         self.n_cubicles_1 = n_cubicles_1
         self.n_cubicles_2 = n_cubicles_2
 
     def init_sampling(self):
         '''
         Create the distributions used by the model and initialise 
         the random seeds of each.
-        '''
+        '''       
         # MODIFICATION. Better method for producing n non-overlapping streams
         seed_sequence = np.random.SeedSequence(self.random_number_set)
     
         # Generate n high quality child seeds
         self.seeds = seed_sequence.spawn(N_STREAMS)
-
+        
         # create distributions
         
         # Triage duration
         self.triage_dist = Exponential(self.triage_mean, 
                                        random_seed=self.seeds[0])
         
         # Registration duration (non-trauma only)
@@ -330,15 +330,15 @@
         # Non-trauma treatment
         self.nt_treat_dist = Lognormal(self.non_trauma_treat_mean, 
                                        np.sqrt(self.non_trauma_treat_var),
                                        random_seed=self.seeds[4])
         
         # treatment of trauma patients
         self.treat_dist = Lognormal(self.trauma_treat_mean, 
-                                    np.sqrt(self.non_trauma_treat_var),
+                                    np.sqrt(self.trauma_treat_var),
                                     random_seed=self.seeds[5])
         
         # probability of non-trauma patient requiring treatment
         self.nt_p_treat_dist = Bernoulli(self.non_trauma_treat_p, 
                                          random_seed=self.seeds[6])
         
         
@@ -461,15 +461,15 @@
             
             # record the waiting time for trauma
             self.wait_treat = self.env.now - start_wait
             trace(f'treatment of patient {self.identifier} at '
                   f'{self.env.now:.3f}')
             
             # sample treatment duration.
-            self.treat_duration = self.args.trauma_dist.sample()
+            self.treat_duration = self.args.treat_dist.sample()
             yield self.env.timeout(self.treat_duration)
             
             self.treatment_complete()
         
         # total time in system
         self.total_time = self.env.now - self.arrival
```

### Comparing `treat-sim-1.1.0/treat_sim.egg-info/PKG-INFO` & `treat_sim-1.1.1/treat_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat-sim
-Version: 1.1.0
+Version: 1.1.1
 Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
 Home-page: https://github.com/pythonhealthdatascience/stars-treat-sim
 Author: Thomas Monks
 Author-email: forecast-tools@gmail.com
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

