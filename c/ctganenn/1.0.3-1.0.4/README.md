# Comparing `tmp/ctganenn-1.0.3.tar.gz` & `tmp/ctganenn-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctganenn-1.0.3.tar", last modified: Tue Apr 30 15:17:22 2024, max compression
+gzip compressed data, was "ctganenn-1.0.4.tar", last modified: Wed May  1 10:04:16 2024, max compression
```

## Comparing `ctganenn-1.0.3.tar` & `ctganenn-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 15:17:22.116398 ctganenn-1.0.3/
--rw-rw-rw-   0        0        0     1543 2024-04-30 15:17:22.116398 ctganenn-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1304 2024-04-30 15:12:46.000000 ctganenn-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 15:17:22.097622 ctganenn-1.0.3/ctganenn/
--rw-rw-rw-   0        0        0       26 2024-04-30 10:51:54.000000 ctganenn-1.0.3/ctganenn/__init__.py
--rw-rw-rw-   0        0        0      732 2024-04-30 10:04:43.000000 ctganenn-1.0.3/ctganenn/main.py
-drwxrwxrwx   0        0        0        0 2024-04-30 15:17:22.115400 ctganenn-1.0.3/ctganenn.egg-info/
--rw-rw-rw-   0        0        0     1543 2024-04-30 15:17:21.000000 ctganenn-1.0.3/ctganenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-30 15:17:22.000000 ctganenn-1.0.3/ctganenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 15:17:21.000000 ctganenn-1.0.3/ctganenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-30 15:17:21.000000 ctganenn-1.0.3/ctganenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 15:17:21.000000 ctganenn-1.0.3/ctganenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 15:17:22.116398 ctganenn-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-30 15:17:10.000000 ctganenn-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:04:16.677388 ctganenn-1.0.4/
+-rw-rw-rw-   0        0        0     1550 2024-05-01 10:04:16.676376 ctganenn-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2024-05-01 10:02:43.000000 ctganenn-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:04:16.646848 ctganenn-1.0.4/ctganenn/
+-rw-rw-rw-   0        0        0       26 2024-04-30 10:51:54.000000 ctganenn-1.0.4/ctganenn/__init__.py
+-rw-rw-rw-   0        0        0      742 2024-05-01 10:00:16.000000 ctganenn-1.0.4/ctganenn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:04:16.674371 ctganenn-1.0.4/ctganenn.egg-info/
+-rw-rw-rw-   0        0        0     1550 2024-05-01 10:04:16.000000 ctganenn-1.0.4/ctganenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-01 10:04:16.000000 ctganenn-1.0.4/ctganenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:04:16.000000 ctganenn-1.0.4/ctganenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-01 10:04:16.000000 ctganenn-1.0.4/ctganenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 10:04:16.000000 ctganenn-1.0.4/ctganenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 10:04:16.677388 ctganenn-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-05-01 10:02:03.000000 ctganenn-1.0.4/setup.py
```

### Comparing `ctganenn-1.0.3/PKG-INFO` & `ctganenn-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ctganenn
-Version: 1.0.3
+Version: 1.0.4
 Summary: CTGAN-ENN : Tabular GAN-based Hybrid sampling method
 Home-page: 
 Author: Mahayasa Adiputra
 Author-email: mahayasa.a@kkumail.com
 Description-Content-Type: text/markdown
 
 # CTGAN-ENN
 
 CTGAN-ENN : Tabular GAN-based Hybrid sampling method.
-A sampling method that combine CTGAN (Conditional Tabular GAN) and ENN(Edited Nearest Neighboor)
-CTGAN is a powerfull oversampling method based on GAN for tabular data
-ENN is an efficient undersampling method to remove overlapped data 
+- A sampling method that combine CTGAN (Conditional Tabular GAN) and ENN(Edited Nearest Neighboor)
+- CTGAN is a powerfull oversampling method based on GAN for tabular data
+- ENN is an efficient undersampling method to remove overlapped data 
 
 ## Installation
 
 Install CTGAN-ENN using pip:
 
 ```bash
 pip install ctganenn
@@ -42,16 +42,15 @@
 ```
 ### Output
 the output of method are X and y :
 - X : all features of your dataset
 - y : target label of your dataset
 
 ### Classification process
-you can process the X and y variable to the next step for classification stage
-For example using Decision Tree Classifier
+you can process the X and y variable to the next step for classification stage. For example using Decision Tree Classifier:
 
 ```bash
 model = tree.DecisionTreeClassifier()
 classification = model.fit(X, y)
 ```
 
 ## Limitation
```

### Comparing `ctganenn-1.0.3/README.md` & `ctganenn-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CTGAN-ENN
 
 CTGAN-ENN : Tabular GAN-based Hybrid sampling method.
-A sampling method that combine CTGAN (Conditional Tabular GAN) and ENN(Edited Nearest Neighboor)
-CTGAN is a powerfull oversampling method based on GAN for tabular data
-ENN is an efficient undersampling method to remove overlapped data 
+- A sampling method that combine CTGAN (Conditional Tabular GAN) and ENN(Edited Nearest Neighboor)
+- CTGAN is a powerfull oversampling method based on GAN for tabular data
+- ENN is an efficient undersampling method to remove overlapped data 
 
 ## Installation
 
 Install CTGAN-ENN using pip:
 
 ```bash
 pip install ctganenn
@@ -33,16 +33,15 @@
 ```
 ### Output
 the output of method are X and y :
 - X : all features of your dataset
 - y : target label of your dataset
 
 ### Classification process
-you can process the X and y variable to the next step for classification stage
-For example using Decision Tree Classifier
+you can process the X and y variable to the next step for classification stage. For example using Decision Tree Classifier:
 
 ```bash
 model = tree.DecisionTreeClassifier()
 classification = model.fit(X, y)
 ```
 
 ## Limitation
```

### Comparing `ctganenn-1.0.3/ctganenn/main.py` & `ctganenn-1.0.4/ctganenn/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from imblearn.under_sampling import EditedNearestNeighbours
 from ctgan import CTGAN
 import pandas as pd
 
 def CTGANENN(minClass,majClass,genData,targetLabel):
+    global X
+    global y
     batch_size = 5000
     epochs = 100
     model = CTGAN(batch_size=batch_size, epochs=epochs, verbose=True)
     model.fit(minClass)
     n_generated_data = genData
     generated_df = model.sample(n_generated_data)
 
@@ -14,9 +16,7 @@
     data_concat = pd.concat([minClass, generated_df])
     # combine data churn and not churn
     data=pd.concat([majClass, data_concat])
     enn = EditedNearestNeighbours(n_neighbors=3)
     X=data.drop([targetLabel],axis=1)
     y=data[targetLabel]
     X, y = enn.fit_resample(X, y)
-
-    return X,y
```

### Comparing `ctganenn-1.0.3/ctganenn.egg-info/PKG-INFO` & `ctganenn-1.0.4/ctganenn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ctganenn
-Version: 1.0.3
+Version: 1.0.4
 Summary: CTGAN-ENN : Tabular GAN-based Hybrid sampling method
 Home-page: 
 Author: Mahayasa Adiputra
 Author-email: mahayasa.a@kkumail.com
 Description-Content-Type: text/markdown
 
 # CTGAN-ENN
 
 CTGAN-ENN : Tabular GAN-based Hybrid sampling method.
-A sampling method that combine CTGAN (Conditional Tabular GAN) and ENN(Edited Nearest Neighboor)
-CTGAN is a powerfull oversampling method based on GAN for tabular data
-ENN is an efficient undersampling method to remove overlapped data 
+- A sampling method that combine CTGAN (Conditional Tabular GAN) and ENN(Edited Nearest Neighboor)
+- CTGAN is a powerfull oversampling method based on GAN for tabular data
+- ENN is an efficient undersampling method to remove overlapped data 
 
 ## Installation
 
 Install CTGAN-ENN using pip:
 
 ```bash
 pip install ctganenn
@@ -42,16 +42,15 @@
 ```
 ### Output
 the output of method are X and y :
 - X : all features of your dataset
 - y : target label of your dataset
 
 ### Classification process
-you can process the X and y variable to the next step for classification stage
-For example using Decision Tree Classifier
+you can process the X and y variable to the next step for classification stage. For example using Decision Tree Classifier:
 
 ```bash
 model = tree.DecisionTreeClassifier()
 classification = model.fit(X, y)
 ```
 
 ## Limitation
```

### Comparing `ctganenn-1.0.3/setup.py` & `ctganenn-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ctganenn',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     install_requires=[
         'scikit-learn==1.2.2',
         'ctgan==0.9.1',
         'sdv==1.11.0',
         'pandas==2.0.3',
         # Add any dependencies your package needs
```

