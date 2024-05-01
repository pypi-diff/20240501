# Comparing `tmp/FrustrationDynamiX-0.2.8.tar.gz` & `tmp/FrustrationDynamiX-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.2.8.tar", last modified: Sat Apr 27 19:13:36 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.2.9.tar", last modified: Wed May  1 11:01:28 2024, max compression
```

## Comparing `FrustrationDynamiX-0.2.8.tar` & `FrustrationDynamiX-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 19:13:36.201536 FrustrationDynamiX-0.2.8/
-drwxrwxrwx   0        0        0        0 2024-04-27 19:13:36.166936 FrustrationDynamiX-0.2.8/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25578 2024-04-27 19:13:25.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:13:36.198536 FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-04-27 19:13:36.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-27 19:13:36.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 19:13:36.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-27 19:13:36.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 19:13:36.000000 FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-04-27 19:13:36.199536 FrustrationDynamiX-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 19:13:36.202536 FrustrationDynamiX-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-04-27 19:13:29.000000 FrustrationDynamiX-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:01:28.313255 FrustrationDynamiX-0.2.9/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:01:28.253629 FrustrationDynamiX-0.2.9/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25620 2024-04-30 21:29:06.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:01:28.307247 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 11:01:28.000000 FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-05-01 11:01:28.311251 FrustrationDynamiX-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:01:28.313255 FrustrationDynamiX-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-04-30 21:29:23.000000 FrustrationDynamiX-0.2.9/setup.py
```

### Comparing `FrustrationDynamiX-0.2.8/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.2.9/FrustrationDynamiX/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         Function to plot the time series with legend and labels
         """
         for col in self.dynamic_var:
             plt.plot(self.time, self.time_series[col], label=col)
         plt.xlabel(xlabel)
         plt.ylabel(ylabel)
         plt.title(title)
-        plt.legend()
+        plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
         if save_plot != None:
             assert type(save_plot) == str, "save_plot variable should have type string, type " + str(type(save_plot)) + " was given instead"
             plt.savefig(save_plot)
         plt.show()
     
     def round_series(self, number_figures):
         """
```

### Comparing `FrustrationDynamiX-0.2.8/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.2.9/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.8/LICENSE` & `FrustrationDynamiX-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.8/PKG-INFO` & `FrustrationDynamiX-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.8/README.md` & `FrustrationDynamiX-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.8/setup.py` & `FrustrationDynamiX-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.2.8',
+    version='0.2.9',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
```

