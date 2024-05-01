# Comparing `tmp/FrustrationDynamiX-0.2.9.tar.gz` & `tmp/FrustrationDynamiX-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.2.9.tar", last modified: Wed May  1 11:01:28 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.3.0.tar", last modified: Wed May  1 15:56:35 2024, max compression
```

## Comparing `FrustrationDynamiX-0.2.9.tar` & `FrustrationDynamiX-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 11:01:28.313255 FrustrationDynamiX-0.2.9/
-drwxrwxrwx   0        0        0        0 2024-05-01 11:01:28.253629 FrustrationDynamiX-0.2.9/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25620 2024-04-30 21:29:06.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:01:28.307247 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-05-01 11:01:28.311251 FrustrationDynamiX-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 11:01:28.313255 FrustrationDynamiX-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-04-30 21:29:23.000000 FrustrationDynamiX-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:56:35.799161 FrustrationDynamiX-0.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-01 15:56:35.789621 FrustrationDynamiX-0.3.0/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25717 2024-05-01 15:45:05.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:56:35.797848 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-05-01 15:56:35.799161 FrustrationDynamiX-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 15:56:35.799161 FrustrationDynamiX-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-05-01 15:48:57.000000 FrustrationDynamiX-0.3.0/setup.py
```

### Comparing `FrustrationDynamiX-0.2.9/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.3.0/FrustrationDynamiX/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,37 +269,39 @@
         """
         Helper function to compute the cohesiveness and divisiveness ratios in macroscale
         """
         Ei_pos = 0  # Number of internally cohesive edges within positive edges
         Ee_neg = 0  # Number of externally divisive edges within negative edges
         Ei = 0      # Total number of internal edges
         Ee = 0      # Total number of external edges
+        allPositive = True
 
         # Iterate over all edges in the graph
         for u, v, data in nx_graph.edges(data=True):
             color_u = solution[u].solution_value()
             color_v = solution[v].solution_value()
             # Check if the edge is positive
             if data.get('sign', 1) > 0:
                 if color_u == color_v:
                     Ei_pos += 1
                     Ei += 1
                 else:
                     Ee += 1
             # Check if the edge is negative
             elif data.get('sign', -1) < 0:
+                allPositive = False
                 if color_u != color_v:
                     Ee_neg += 1
                     Ee += 1
                 else:
                     Ei += 1
 
         # Calculate cohesiveness and divisiveness
         C = Ei_pos / Ei if Ei != 0 else 0  # Cohesiveness
-        D = Ee_neg / Ee if Ee != 0 else 0  # Divisiveness
+        D = Ee_neg / Ee if Ee != 0 else 1  # Divisiveness
 
         return C, D
         
     @staticmethod
     def plot_colored_graph(G, solution, color_0 = "red", color_1 = "blue"):
         """
         Helper function to plot the colored partitioned graph based on ILP solution
@@ -575,24 +577,24 @@
             warnings.warn("If data points are not normalized between -1 and 1, plot might be out of scale")
         
         for col in self.dynamic_var:
             plt.plot(self.time, self.time_series[col], label=col)
             
         if method == "MIC":
             #assert self.triadic_balance != None, "Missing call: compute_triadic_evolution method should be called first"
-            plt.plot(self.time_vector, self.triadic_balance, marker = "x", label = "Triadic Balance")
+            plt.plot(self.time_vector[1:], self.triadic_balance[1:], marker = "x", label = "Triadic Balance")
         
         elif method == "MAC":
             #assert self.frustration != None, "Missing call: compute_frustration_evolution method should be called first"
-            plt.plot(self.time_vector, self.frustration, marker = "x", label = "Global Frustration")
+            plt.plot(self.time_vector[1:], self.frustration[1:], marker = "x", label = "Global Frustration")
         
         elif method == "MES":
             #assert self.frustration != None, "Missing call: compute_frustration_evolution method should be called first"
-            plt.plot(self.time_vector, self.cohesiveness, marker = "x", label = "Cohesiveness")
-            plt.plot(self.time_vector, self.divisiveness, marker = "x", label = "Divisiveness")
+            plt.plot(self.time_vector[1:], self.cohesiveness[1:], marker = "x", label = "Cohesiveness")
+            plt.plot(self.time_vector[1:], self.divisiveness[1:], marker = "x", label = "Divisiveness")
         
         plt.xlabel(xlabel)
         plt.ylabel(ylabel)
         plt.title(title)
         plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
         if save_plot != None:
             assert type(save_plot) == str, "save_plot variable should have type string, type " + str(type(save_plot)) + " was given instead"
```

### Comparing `FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.9
+Version: 0.3.0
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.9/LICENSE` & `FrustrationDynamiX-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.9/PKG-INFO` & `FrustrationDynamiX-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.9
+Version: 0.3.0
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.9/README.md` & `FrustrationDynamiX-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.9/setup.py` & `FrustrationDynamiX-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.2.9',
+    version='0.3.0',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
```

