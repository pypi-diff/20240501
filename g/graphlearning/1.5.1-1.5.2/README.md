# Comparing `tmp/graphlearning-1.5.1.tar.gz` & `tmp/graphlearning-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlearning-1.5.1.tar", last modified: Mon Mar 18 21:02:10 2024, max compression
+gzip compressed data, was "graphlearning-1.5.2.tar", last modified: Wed May  1 20:50:56 2024, max compression
```

## Comparing `graphlearning-1.5.1.tar` & `graphlearning-1.5.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:02:10.867792 graphlearning-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-18 21:01:53.000000 graphlearning-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 21:01:53.000000 graphlearning-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-18 21:02:10.867792 graphlearning-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-18 21:01:53.000000 graphlearning-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:02:10.863792 graphlearning-1.5.1/c_code/
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/cextensions.c
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/hjsolvers.c
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/hjsolvers.h
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/lp_iterate.c
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/lp_iterate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/maj_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/maj_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/maj_simple_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/mbo_convolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/mbo_speedy_volume_preserving.c
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/memory_allocation.c
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/memory_allocation.h
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/mnist_benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/mnist_benchmark.h
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-18 21:01:53.000000 graphlearning-1.5.1/c_code/vector_operations.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:02:10.867792 graphlearning-1.5.1/graphlearning/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23310 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    77849 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/trainsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22463 2024-03-18 21:01:53.000000 graphlearning-1.5.1/graphlearning/weightmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 21:02:10.867792 graphlearning-1.5.1/graphlearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-18 21:02:10.000000 graphlearning-1.5.1/graphlearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-18 21:02:10.000000 graphlearning-1.5.1/graphlearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 21:02:10.000000 graphlearning-1.5.1/graphlearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-18 21:02:10.000000 graphlearning-1.5.1/graphlearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-18 21:02:10.000000 graphlearning-1.5.1/graphlearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-18 21:01:54.000000 graphlearning-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 21:02:10.867792 graphlearning-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-18 21:01:54.000000 graphlearning-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.137328 graphlearning-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-01 20:50:41.000000 graphlearning-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 20:50:41.000000 graphlearning-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-01 20:50:56.137328 graphlearning-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-01 20:50:41.000000 graphlearning-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.133328 graphlearning-1.5.2/c_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/cextensions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/hjsolvers.c
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/hjsolvers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/lp_iterate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/lp_iterate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/maj_dijkstra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/maj_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/maj_simple_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mbo_convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mbo_speedy_volume_preserving.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/memory_allocation.c
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/memory_allocation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mnist_benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mnist_benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/vector_operations.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.133328 graphlearning-1.5.2/graphlearning/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77849 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/trainsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22463 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/weightmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.137328 graphlearning-1.5.2/graphlearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-01 20:50:42.000000 graphlearning-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:50:56.137328 graphlearning-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-01 20:50:42.000000 graphlearning-1.5.2/setup.py
```

### Comparing `graphlearning-1.5.1/LICENSE` & `graphlearning-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/PKG-INFO` & `graphlearning-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.1/README.md` & `graphlearning-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/cextensions.c` & `graphlearning-1.5.2/c_code/cextensions.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/hjsolvers.c` & `graphlearning-1.5.2/c_code/hjsolvers.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/hjsolvers.h` & `graphlearning-1.5.2/c_code/hjsolvers.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/lp_iterate.c` & `graphlearning-1.5.2/c_code/lp_iterate.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/lp_iterate.h` & `graphlearning-1.5.2/c_code/lp_iterate.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/maj_dijkstra.h` & `graphlearning-1.5.2/c_code/maj_dijkstra.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/maj_implicit_heap.h` & `graphlearning-1.5.2/c_code/maj_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/maj_simple_implicit_heap.h` & `graphlearning-1.5.2/c_code/maj_simple_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/mbo_convolution.h` & `graphlearning-1.5.2/c_code/mbo_convolution.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/mbo_speedy_volume_preserving.c` & `graphlearning-1.5.2/c_code/mbo_speedy_volume_preserving.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/memory_allocation.c` & `graphlearning-1.5.2/c_code/memory_allocation.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/mnist_benchmark.c` & `graphlearning-1.5.2/c_code/mnist_benchmark.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/mnist_benchmark.h` & `graphlearning-1.5.2/c_code/mnist_benchmark.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/c_code/vector_operations.h` & `graphlearning-1.5.2/c_code/vector_operations.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/active_learning.py` & `graphlearning-1.5.2/graphlearning/active_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
 
 # update the labeled data of active_learner object (including the graph-based ssl ``model`` outputs)
 AL.update(query_points, query_labels) 
 ```
 
 Some clarification of terms:
-* ``acquisition function``: a function that quantifies "how useful" it would be to label a currently unlabeled node. Oftentimes, this is reflected in the "uncertainty" of the current classifier's output for each node. 
-    * __NOTE:__ users can provide their own acquisition functions that inherit from the ``acquisition_function`` class, being sure to implement it so that __larger values__ of the acquisition function correspond to __more desirable__ nodes to be labeled.
-* ``policy``: the active learning policy determines which node(s) will be selected as query points, given the set of acquisition function values evaluated on the unlabeled nodes. 
-    * The default value ``max`` indicates that query points will be the maximizers of the acquisition function on the unlabeled nodes. The policy ``prop`` selects the query points proportional to the ''softmax'' of the acquisition function values; namely, 
+- ``acquisition function``: a function that quantifies "how useful" it would be to label a currently unlabeled node. Oftentimes, this is reflected in the "uncertainty" of the current classifier's output for each node. 
+- __NOTE:__ users can provide their own acquisition functions that inherit from the ``acquisition_function`` class, being sure to implement it so that __larger values__ of the acquisition function correspond to __more desirable__ nodes to be labeled.
+- ``policy``: the active learning policy determines which node(s) will be selected as query points, given the set of acquisition function values evaluated on the unlabeled nodes. 
+- The default value ``max`` indicates that query points will be the maximizers of the acquisition function on the unlabeled nodes. The policy ``prop`` selects the query points proportional to the ''softmax'' of the acquisition function values; namely, 
 \\[\mathbb{P}(X = x) \\propto e^{\\gamma \\mathcal{A}(x)}\\]
 """
 
 import numpy as np
 from scipy.special import softmax
 from abc import ABCMeta, abstractmethod
 import matplotlib.pyplot as plt
@@ -77,15 +77,15 @@
             if (candidate_ind.min() < 0) or (candidate_ind.max() > self.n):
                 raise ValueError(f"candidate_ind must have integer values between 0 and {self.n}")
         elif candidate_ind == 'full':
             if allow_repeat:
                 candidate_ind = np.arange(self.all_inds)
             else:
                 candidate_ind = np.setdiff1d(self.all_inds, self.labeled_ind)
-        elif (candidate_set == 'rand') and (rand_frac>0 and rand_frac<1):
+        elif (candidate_ind == 'rand') and (rand_frac>0 and rand_frac<1):
             if allow_repeat:
                 candidate_ind = np.random.choice(self.all_inds, size=int(rand_frac * self.n), replace=False)
             else:
                 candidate_ind = np.random.choice(self.unlabeled_ind, size=int(rand_frac * len(self.unlabeled_ind)), replace=False)
         else:
             raise ValueError("Invalid input for candidate_ind")
         
@@ -230,15 +230,15 @@
             unc_terms = 1.-(u_sort[:,-1] - u_sort[:,0])
         elif self.unc_method == "unc_2norm":
             unc_terms = 1. - np.linalg.norm(u[candidate_ind], axis=1)
         return unc_terms
 
 
 
-class v_opt(acquisition_function):
+class var_opt(acquisition_function):
     """Variance Optimization
     ===================
 
     Active learning algorithm that selects points that minimizes the variance of the distribution of unlabeled nodes.
 
     Examples
     --------
@@ -255,15 +255,15 @@
     plt.scatter(X[:,0],X[:,1], c=labels)
     plt.scatter(X[train_ind,0],X[train_ind,1], c='r')
     plt.show()
 
     # compute initial, low-rank (spectral truncation) covariance matrix 
     evals, evecs = model.graph.eigen_decomp(normalization='normalized', k=50)
     C = np.diag(1. / (evals + 1e-11))
-    AL = gl.active_learning.active_learner(model, gl.active_learning.v_opt, train_ind, y[train_ind], C=C.copy(), V=evecs.copy())
+    AL = gl.active_learning.active_learner(model, gl.active_learning.var_opt, train_ind, y[train_ind], C=C.copy(), V=evecs.copy())
 
     for i in range(10):
         query_points = AL.select_queries() # return this iteration's newly chosen points
         query_labels = y[query_points] # simulate the human in the loop process
         AL.update(query_points, query_labels) # update the active_learning object's labeled set
 
         # plot
@@ -303,15 +303,15 @@
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
             
         return col_norms / diag_terms
 
     def update(self, query_ind, query_labels):
         for k in query_ind:
             if self.storage == 'full':
-                self.C -= np.outer(C[:,k], C[:,k]) / (self.gamma2 + C[k,k])
+                self.C -= np.outer(self.C[:,k], self.C[:,k]) / (self.gamma2 + self.C[k,k])
             else:
                 vk = self.V[k]
                 Cavk = self.C @ vk
                 ip = np.inner(vk, Cavk)
                 self.C -= np.outer(Cavk, Cavk)/(self.gamma2 + ip) 
 
         return 
@@ -389,15 +389,15 @@
             
         return col_sums/ diag_terms
 
 
     def update(self, query_ind, query_labels):
         for k in query_ind:
             if self.storage == 'full':
-                self.C -= np.outer(C[:,k], C[:,k]) / (self.gamma2 + C[k,k])
+                self.C -= np.outer(self.C[:,k], self.C[:,k]) / (self.gamma2 + self.C[k,k])
             else:
                 vk = self.V[k]
                 Cavk = self.C @ vk
                 ip = np.inner(vk, Cavk)
                 self.C -= np.outer(Cavk, Cavk)/(self.gamma2 + ip) 
 
         return
@@ -454,15 +454,15 @@
     Journal on Selected Areas in Information Theory 1, 167–177 (May 2020).
     """
     def __init__(self, C, V=None, gamma2=0.1**2., unc_method='smallest_margin'):
         assert (C.shape[0] == C.shape[1]) or (V is not None)
         self.C = C.copy()
         self.V = V
         self.gamma2 = gamma2
-        self.unc_sampling = uncertainty_sampling(unc_method=unc_method)
+        self.unc_sampling = unc_sampling(unc_method=unc_method)
         if self.V is None:
             self.storage = 'full'
         else:
             self.storage = 'trunc'
         
     def compute(self, u, candidate_ind):
         unc_terms = self.unc_sampling.compute_values(active_learning, u)
@@ -475,24 +475,24 @@
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
         return unc_terms * col_norms / diag_terms  
 
 
     def update(self, query_ind, query_labels):
         for k in query_ind:
             if self.storage == 'full':
-                self.C -= np.outer(C[:,k], C[:,k]) / (self.gamma2 + C[k,k])
+                self.C -= np.outer(self.C[:,k], self.C[:,k]) / (self.gamma2 + self.C[k,k])
             else:
                 vk = self.V[k]
                 Cavk = self.C @ vk
                 ip = np.inner(vk, Cavk)
                 self.C -= np.outer(Cavk, Cavk)/(self.gamma2 + ip) 
         return
         
 
-class model_change_vopt(acquisition_function):
+class model_change_var_opt(acquisition_function):
     """Model Change Variance Optimization
     ===================
 
     Active learning algorithm that is a combination of Model Change and Variance Optimization.
 
     Examples
     --------
@@ -509,15 +509,15 @@
     plt.scatter(X[:,0],X[:,1], c=labels)
     plt.scatter(X[train_ind,0],X[train_ind,1], c='r')
     plt.show()
 
     # compute initial, low-rank (spectral truncation) covariance matrix 
     evals, evecs = model.graph.eigen_decomp(normalization='normalized', k=50)
     C = np.diag(1. / (evals + 1e-11))
-    AL = gl.active_learning.active_learner(model, gl.active_learning.mc_vopt, train_ind, y[train_ind], C=C.copy(), V=evecs.copy())
+    AL = gl.active_learning.active_learner(model, gl.active_learning.model_change_var_opt, train_ind, y[train_ind], C=C.copy(), V=evecs.copy())
 
     for i in range(10):
         query_points = AL.select_queries() # return this iteration's newly chosen points
         query_labels = y[query_points] # simulate the human in the loop process
         AL.update(query_points, query_labels) # update the active_learning object's labeled set
 
         # plot
@@ -541,15 +541,15 @@
     Journal on Selected Areas in Information Theory 1, 167–177 (May 2020).
     """
     def __init__(self, C, V=None, gamma2=0.1**2., unc_method='smallest_margin'):
         assert (C.shape[0] == C.shape[1]) or (V is not None)
         self.C = C.copy()
         self.V = V
         self.gamma2 = gamma2
-        self.unc_sampling = uncertainty_sampling(method=unc_method)
+        self.unc_sampling = unc_sampling(method=unc_method)
         if self.V is None:
             self.storage = 'full'
         else:
             self.storage = 'trunc'
         
     def compute(self, u, candidate_ind):
         unc_terms = self.unc_sampling.compute_values(active_learning, u)
@@ -562,14 +562,14 @@
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
         return unc_terms * col_norms / diag_terms  
 
 
     def update(self, query_ind, query_labels):
         for k in query_ind:
             if self.storage == 'full':
-                self.C -= np.outer(C[:,k], C[:,k]) / (self.gamma2 + C[k,k])
+                self.C -= np.outer(self.C[:,k], self.C[:,k]) / (self.gamma2 + self.C[k,k])
             else:
                 vk = self.V[k]
                 Cavk = self.C @ vk
                 ip = np.inner(vk, Cavk)
                 self.C -= np.outer(Cavk, Cavk)/(self.gamma2 + ip) 
         return
```

### Comparing `graphlearning-1.5.1/graphlearning/clustering.py` & `graphlearning-1.5.2/graphlearning/clustering.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/datasets.py` & `graphlearning-1.5.2/graphlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/graph.py` & `graphlearning-1.5.2/graphlearning/graph.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/ssl.py` & `graphlearning-1.5.2/graphlearning/ssl.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/trainsets.py` & `graphlearning-1.5.2/graphlearning/trainsets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/utils.py` & `graphlearning-1.5.2/graphlearning/utils.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning/weightmatrix.py` & `graphlearning-1.5.2/graphlearning/weightmatrix.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/graphlearning.egg-info/PKG-INFO` & `graphlearning-1.5.2/graphlearning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.1/graphlearning.egg-info/SOURCES.txt` & `graphlearning-1.5.2/graphlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.1/pyproject.toml` & `graphlearning-1.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools]
 packages = ['graphlearning']
 
 
 [project]
 name = "graphlearning"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="Jeff Calder", email="jwcalder@umn.edu" },
 ]
 description = "Python package for graph-based clustering and semi-supervised learning"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.6"
```

### Comparing `graphlearning-1.5.1/setup.py` & `graphlearning-1.5.2/setup.py`

 * *Files identical despite different names*

