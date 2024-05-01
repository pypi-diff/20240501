# Comparing `tmp/coinanalyse-1.0.4.tar.gz` & `tmp/coinanalyse-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinanalyse-1.0.4.tar", last modified: Sun Apr 28 15:26:16 2024, max compression
+gzip compressed data, was "coinanalyse-1.0.5.tar", last modified: Wed May  1 17:20:24 2024, max compression
```

## Comparing `coinanalyse-1.0.4.tar` & `coinanalyse-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:26:13.414940 coinanalyse-1.0.4/
--rw-rw-rw-   0        0        0     1068 2024-03-28 10:30:36.000000 coinanalyse-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      242 2024-04-28 15:26:13.412993 coinanalyse-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 15:26:13.376013 coinanalyse-1.0.4/coinanalyse/
--rw-rw-rw-   0        0        0      877 2019-07-26 16:30:47.000000 coinanalyse-1.0.4/coinanalyse/colors.py
--rw-rw-rw-   0        0        0      955 2019-07-26 16:30:47.000000 coinanalyse-1.0.4/coinanalyse/exporter.py
--rw-rw-rw-   0        0        0      571 2024-04-26 10:57:09.000000 coinanalyse-1.0.4/coinanalyse/getQuark.py
--rw-rw-rw-   0        0        0      778 2024-04-26 10:57:22.000000 coinanalyse-1.0.4/coinanalyse/getTransactions.py
--rw-rw-rw-   0        0        0      535 2019-07-26 16:30:47.000000 coinanalyse-1.0.4/coinanalyse/prepareGraph.py
--rw-rw-rw-   0        0        0      104 2019-07-26 16:30:47.000000 coinanalyse-1.0.4/coinanalyse/requester.py
--rw-rw-rw-   0        0        0     1187 2019-07-26 16:30:47.000000 coinanalyse-1.0.4/coinanalyse/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:26:13.409107 coinanalyse-1.0.4/coinanalyse.egg-info/
--rw-rw-rw-   0        0        0      242 2024-04-28 15:26:12.000000 coinanalyse-1.0.4/coinanalyse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-04-28 15:26:13.000000 coinanalyse-1.0.4/coinanalyse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:26:12.000000 coinanalyse-1.0.4/coinanalyse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-28 15:26:12.000000 coinanalyse-1.0.4/coinanalyse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-28 15:26:12.000000 coinanalyse-1.0.4/coinanalyse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 15:26:13.414940 coinanalyse-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      383 2024-04-28 15:25:26.000000 coinanalyse-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:20:57.044438 coinanalyse-1.0.5/
+-rw-rw-rw-   0        0        0     1068 2024-03-28 10:30:36.000000 coinanalyse-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      242 2024-05-01 17:20:57.042491 coinanalyse-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4823 2024-05-01 17:02:17.000000 coinanalyse-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 17:20:57.019131 coinanalyse-1.0.5/coinanalyse/
+-rw-rw-rw-   0        0        0      877 2024-04-30 09:15:39.000000 coinanalyse-1.0.5/coinanalyse/colors.py
+-rw-rw-rw-   0        0        0      955 2019-07-26 16:30:47.000000 coinanalyse-1.0.5/coinanalyse/exporter.py
+-rw-rw-rw-   0        0        0      571 2024-04-26 10:57:09.000000 coinanalyse-1.0.5/coinanalyse/getQuark.py
+-rw-rw-rw-   0        0        0      778 2024-04-26 10:57:22.000000 coinanalyse-1.0.5/coinanalyse/getTransactions.py
+-rw-rw-rw-   0        0        0      535 2019-07-26 16:30:47.000000 coinanalyse-1.0.5/coinanalyse/prepareGraph.py
+-rw-rw-rw-   0        0        0      104 2019-07-26 16:30:47.000000 coinanalyse-1.0.5/coinanalyse/requester.py
+-rw-rw-rw-   0        0        0     1187 2019-07-26 16:30:47.000000 coinanalyse-1.0.5/coinanalyse/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:20:57.039571 coinanalyse-1.0.5/coinanalyse.egg-info/
+-rw-rw-rw-   0        0        0      242 2024-05-01 17:20:56.000000 coinanalyse-1.0.5/coinanalyse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-05-01 17:20:56.000000 coinanalyse-1.0.5/coinanalyse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 17:20:56.000000 coinanalyse-1.0.5/coinanalyse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-01 17:20:56.000000 coinanalyse-1.0.5/coinanalyse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 17:20:56.000000 coinanalyse-1.0.5/coinanalyse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 17:20:57.044438 coinanalyse-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-05-01 17:19:46.000000 coinanalyse-1.0.5/setup.py
```

### Comparing `coinanalyse-1.0.4/LICENSE.txt` & `coinanalyse-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coinanalyse-1.0.4/coinanalyse/colors.py` & `coinanalyse-1.0.5/coinanalyse/colors.py`

 * *Files identical despite different names*

### Comparing `coinanalyse-1.0.4/coinanalyse/exporter.py` & `coinanalyse-1.0.5/coinanalyse/exporter.py`

 * *Files identical despite different names*

### Comparing `coinanalyse-1.0.4/coinanalyse/getQuark.py` & `coinanalyse-1.0.5/coinanalyse/getQuark.py`

 * *Files identical despite different names*

### Comparing `coinanalyse-1.0.4/coinanalyse/getTransactions.py` & `coinanalyse-1.0.5/coinanalyse/getTransactions.py`

 * *Files identical despite different names*

### Comparing `coinanalyse-1.0.4/coinanalyse/prepareGraph.py` & `coinanalyse-1.0.5/coinanalyse/prepareGraph.py`

 * *Files identical despite different names*

### Comparing `coinanalyse-1.0.4/coinanalyse/utils.py` & `coinanalyse-1.0.5/coinanalyse/utils.py`

 * *Files identical despite different names*

