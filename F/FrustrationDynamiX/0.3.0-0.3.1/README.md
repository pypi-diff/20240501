# Comparing `tmp/FrustrationDynamiX-0.3.0.tar.gz` & `tmp/FrustrationDynamiX-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.3.0.tar", last modified: Wed May  1 15:56:35 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.3.1.tar", last modified: Wed May  1 20:02:21 2024, max compression
```

## Comparing `FrustrationDynamiX-0.3.0.tar` & `FrustrationDynamiX-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:56:35.799161 FrustrationDynamiX-0.3.0/
-drwxrwxrwx   0        0        0        0 2024-05-01 15:56:35.789621 FrustrationDynamiX-0.3.0/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25717 2024-05-01 15:45:05.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:56:35.797848 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 15:56:35.000000 FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-05-01 15:56:35.799161 FrustrationDynamiX-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 15:56:35.799161 FrustrationDynamiX-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-05-01 15:48:57.000000 FrustrationDynamiX-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:02:21.105080 FrustrationDynamiX-0.3.1/
+drwxrwxrwx   0        0        0        0 2024-05-01 20:02:21.078218 FrustrationDynamiX-0.3.1/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25864 2024-05-01 20:00:26.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:02:21.099511 FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-05-01 20:02:20.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-01 20:02:20.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:02:20.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-01 20:02:20.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 20:02:20.000000 FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-05-01 20:02:21.103053 FrustrationDynamiX-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:02:21.106078 FrustrationDynamiX-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-05-01 20:01:34.000000 FrustrationDynamiX-0.3.1/setup.py
```

### Comparing `FrustrationDynamiX-0.3.0/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.3.1/FrustrationDynamiX/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,19 +111,21 @@
         for t in tqdm(range(1,self.duration-window_size,window_size)):
             for u in range(self.num_var): #1 loop for each variable
                 result = pyEDM.SMap(dataFrame = self.time_series, lib = [t,t+window_size], pred = [t,t+window_size], 
                                     embedded = True, columns = self.dynamic_var, target = self.dynamic_var[u], showPlot= showPlot)
                 var = result['coefficients'].columns[2:]
                 for v in range(len(var)):
                     if u != v:
-                        J[u,v,T_ind] = result['coefficients'][var[v]][window_size//2]
+                        #J[u,v,T_ind] = result['coefficients'][var[v]][window_size//2]
+                        J[u,v,T_ind] = result['coefficients'][var[v]][window_size-1]
                         
             #Update iterators
             T_ind += 1
-            time_vector += [self.time[t + window_size//2]]
+            #time_vector += [self.time[t + window_size//2]]
+            time_vector += [self.time[t + window_size-1]]
 
         return np.nan_to_num(J), time_vector
    
     @staticmethod
     def saveas_coo(jacobian_matrix, path):
         """
         Function to save the Jacobian coefficients as csv files in COO format
```

### Comparing `FrustrationDynamiX-0.3.0/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.3.1/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.3.0/LICENSE` & `FrustrationDynamiX-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.3.0/PKG-INFO` & `FrustrationDynamiX-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.3.0/README.md` & `FrustrationDynamiX-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.3.0/setup.py` & `FrustrationDynamiX-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
```

