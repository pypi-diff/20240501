# Comparing `tmp/upowwalletpy-0.1.0.tar.gz` & `tmp/upowwalletpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upowwalletpy-0.1.0.tar", last modified: Wed May  1 06:29:44 2024, max compression
+gzip compressed data, was "upowwalletpy-1.0.1.tar", last modified: Wed May  1 06:51:12 2024, max compression
```

## Comparing `upowwalletpy-0.1.0.tar` & `upowwalletpy-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:29:44.489004 upowwalletpy-0.1.0/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      236 2024-05-01 06:29:44.488795 upowwalletpy-0.1.0/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       13 2024-05-01 06:24:13.000000 upowwalletpy-0.1.0/README.md
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-01 06:29:44.489103 upowwalletpy-0.1.0/setup.cfg
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      799 2024-05-01 06:23:29.000000 upowwalletpy-0.1.0/setup.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:29:44.484822 upowwalletpy-0.1.0/upow_transactions/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowwalletpy-0.1.0/upow_transactions/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1420 2024-03-01 05:05:06.000000 upowwalletpy-0.1.0/upow_transactions/coinbase_transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowwalletpy-0.1.0/upow_transactions/constants.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowwalletpy-0.1.0/upow_transactions/helpers.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     8658 2024-03-10 06:13:59.000000 upowwalletpy-0.1.0/upow_transactions/transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     4979 2024-03-10 06:13:49.000000 upowwalletpy-0.1.0/upow_transactions/transaction_input.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1556 2024-03-10 06:13:54.000000 upowwalletpy-0.1.0/upow_transactions/transaction_output.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:29:44.486956 upowwalletpy-0.1.0/upowwalletpy.egg-info/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      236 2024-05-01 06:29:44.000000 upowwalletpy-0.1.0/upowwalletpy.egg-info/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      494 2024-05-01 06:29:44.000000 upowwalletpy-0.1.0/upowwalletpy.egg-info/SOURCES.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-01 06:29:44.000000 upowwalletpy-0.1.0/upowwalletpy.egg-info/dependency_links.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-01 06:29:44.000000 upowwalletpy-0.1.0/upowwalletpy.egg-info/requires.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       24 2024-05-01 06:29:44.000000 upowwalletpy-0.1.0/upowwalletpy.egg-info/top_level.txt
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:29:44.488067 upowwalletpy-0.1.0/utils/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:03.000000 upowwalletpy-0.1.0/utils/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    17559 2024-05-01 06:12:53.000000 upowwalletpy-0.1.0/utils/repository.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    22627 2024-05-01 06:15:14.000000 upowwalletpy-0.1.0/utils/utils.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:51:12.543810 upowwalletpy-1.0.1/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       15 2024-05-01 06:49:26.000000 upowwalletpy-1.0.1/MANIFEST.in
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      225 2024-05-01 06:51:12.543673 upowwalletpy-1.0.1/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       13 2024-05-01 06:24:13.000000 upowwalletpy-1.0.1/README.md
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     5227 2024-05-01 06:06:41.000000 upowwalletpy-1.0.1/push.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-01 06:51:12.543861 upowwalletpy-1.0.1/setup.cfg
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      813 2024-05-01 06:51:08.000000 upowwalletpy-1.0.1/setup.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:51:12.540032 upowwalletpy-1.0.1/upow_transactions/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowwalletpy-1.0.1/upow_transactions/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1420 2024-03-01 05:05:06.000000 upowwalletpy-1.0.1/upow_transactions/coinbase_transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowwalletpy-1.0.1/upow_transactions/constants.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowwalletpy-1.0.1/upow_transactions/helpers.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     8658 2024-03-10 06:13:59.000000 upowwalletpy-1.0.1/upow_transactions/transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     4979 2024-03-10 06:13:49.000000 upowwalletpy-1.0.1/upow_transactions/transaction_input.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1556 2024-03-10 06:13:54.000000 upowwalletpy-1.0.1/upow_transactions/transaction_output.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:51:12.541108 upowwalletpy-1.0.1/upowwalletpy.egg-info/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      225 2024-05-01 06:51:12.000000 upowwalletpy-1.0.1/upowwalletpy.egg-info/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      514 2024-05-01 06:51:12.000000 upowwalletpy-1.0.1/upowwalletpy.egg-info/SOURCES.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-01 06:51:12.000000 upowwalletpy-1.0.1/upowwalletpy.egg-info/dependency_links.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-01 06:51:12.000000 upowwalletpy-1.0.1/upowwalletpy.egg-info/requires.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       29 2024-05-01 06:51:12.000000 upowwalletpy-1.0.1/upowwalletpy.egg-info/top_level.txt
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:51:12.543125 upowwalletpy-1.0.1/utils/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:03.000000 upowwalletpy-1.0.1/utils/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    17559 2024-05-01 06:12:53.000000 upowwalletpy-1.0.1/utils/repository.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    22627 2024-05-01 06:15:14.000000 upowwalletpy-1.0.1/utils/utils.py
```

### Comparing `upowwalletpy-0.1.0/setup.py` & `upowwalletpy-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="upowwalletpy",
-    version="0.1.0",
-    author="Your Name",
-    author_email="your.email@example.com",
+    version="1.0.1",
+    author="upow",
+    author_email="contact@upow.ai",
     description="A package for UPOW wallet transactions",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
+    py_modules=["push"],
     install_requires=[
         "asttokens==2.4.1",
         "base58==0.2.5",
         "certifi==2023.11.17",
         "charset-normalizer==2.0.12",
         "colorama==0.4.6",
         "executing==2.0.1",
@@ -21,9 +22,9 @@
         "idna==3.6",
         "pygments==2.17.2",
         "requests==2.26.0",
         "six==1.16.0",
         "urllib3==1.26.18",
         "pickleDB~=0.9.2",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.11",
 )
```

### Comparing `upowwalletpy-0.1.0/upow_transactions/coinbase_transaction.py` & `upowwalletpy-1.0.1/upow_transactions/coinbase_transaction.py`

 * *Files identical despite different names*

### Comparing `upowwalletpy-0.1.0/upow_transactions/helpers.py` & `upowwalletpy-1.0.1/upow_transactions/helpers.py`

 * *Files identical despite different names*

### Comparing `upowwalletpy-0.1.0/upow_transactions/transaction.py` & `upowwalletpy-1.0.1/upow_transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `upowwalletpy-0.1.0/upow_transactions/transaction_input.py` & `upowwalletpy-1.0.1/upow_transactions/transaction_input.py`

 * *Files identical despite different names*

### Comparing `upowwalletpy-0.1.0/upow_transactions/transaction_output.py` & `upowwalletpy-1.0.1/upow_transactions/transaction_output.py`

 * *Files identical despite different names*

### Comparing `upowwalletpy-0.1.0/utils/repository.py` & `upowwalletpy-1.0.1/utils/repository.py`

 * *Files identical despite different names*

### Comparing `upowwalletpy-0.1.0/utils/utils.py` & `upowwalletpy-1.0.1/utils/utils.py`

 * *Files identical despite different names*

