# Comparing `tmp/Kavach-0.2.tar.gz` & `tmp/Kavach-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kavach-0.2.tar", last modified: Wed Apr 10 13:08:06 2024, max compression
+gzip compressed data, was "Kavach-0.3.tar", last modified: Wed May  1 12:39:51 2024, max compression
```

## Comparing `Kavach-0.2.tar` & `Kavach-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.050175 Kavach-0.2/
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.047957 Kavach-0.2/Kavach/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       50 2024-04-08 09:32:22.000000 Kavach-0.2/Kavach/__init__.py
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.048804 Kavach-0.2/Kavach/data/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)    61101 2024-04-08 08:57:15.000000 Kavach-0.2/Kavach/data/logo.png
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     3076 2024-04-10 13:02:59.000000 Kavach-0.2/Kavach/gradio_app.py
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2013 2024-04-09 16:28:35.000000 Kavach-0.2/Kavach/utils.py
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.048694 Kavach-0.2/Kavach.egg-info/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/PKG-INFO
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      327 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/SOURCES.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        1 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/dependency_links.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       60 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/entry_points.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       33 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/requires.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       13 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/top_level.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       29 2024-04-09 16:26:05.000000 Kavach-0.2/MANIFEST.in
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-04-10 13:08:06.049981 Kavach-0.2/PKG-INFO
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2513 2024-04-08 09:16:45.000000 Kavach-0.2/README.md
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       38 2024-04-10 13:08:06.050215 Kavach-0.2/setup.cfg
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      427 2024-04-10 13:07:36.000000 Kavach-0.2/setup.py
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.049764 Kavach-0.2/tests/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-08 09:17:41.000000 Kavach-0.2/tests/__init__.py
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     1739 2024-04-09 16:27:46.000000 Kavach-0.2/tests/test_utils.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-05-01 12:39:51.245234 Kavach-0.3/
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-05-01 12:39:51.243101 Kavach-0.3/Kavach/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       50 2024-04-08 09:32:22.000000 Kavach-0.3/Kavach/__init__.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-05-01 12:39:51.243866 Kavach-0.3/Kavach/data/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)    61101 2024-04-08 08:57:15.000000 Kavach-0.3/Kavach/data/logo.png
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2859 2024-05-01 12:30:34.000000 Kavach-0.3/Kavach/gradio_app.py
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2315 2024-05-01 12:30:23.000000 Kavach-0.3/Kavach/utils.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-05-01 12:39:51.243765 Kavach-0.3/Kavach.egg-info/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-05-01 12:39:51.000000 Kavach-0.3/Kavach.egg-info/PKG-INFO
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      327 2024-05-01 12:39:51.000000 Kavach-0.3/Kavach.egg-info/SOURCES.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        1 2024-05-01 12:39:51.000000 Kavach-0.3/Kavach.egg-info/dependency_links.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       60 2024-05-01 12:39:51.000000 Kavach-0.3/Kavach.egg-info/entry_points.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       33 2024-05-01 12:39:51.000000 Kavach-0.3/Kavach.egg-info/requires.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       13 2024-05-01 12:39:51.000000 Kavach-0.3/Kavach.egg-info/top_level.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       29 2024-04-09 16:26:05.000000 Kavach-0.3/MANIFEST.in
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-05-01 12:39:51.245076 Kavach-0.3/PKG-INFO
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2513 2024-04-08 09:16:45.000000 Kavach-0.3/README.md
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       38 2024-05-01 12:39:51.245271 Kavach-0.3/setup.cfg
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      427 2024-05-01 11:37:24.000000 Kavach-0.3/setup.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-05-01 12:39:51.244801 Kavach-0.3/tests/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      204 2024-05-01 12:16:23.000000 Kavach-0.3/tests/__init__.py
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     1739 2024-04-09 16:27:46.000000 Kavach-0.3/tests/test_utils.py
```

### Comparing `Kavach-0.2/Kavach/data/logo.png` & `Kavach-0.3/Kavach/data/logo.png`

 * *Files identical despite different names*

### Comparing `Kavach-0.2/Kavach/utils.py` & `Kavach-0.3/Kavach/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # utils.py
 from transformers import pipeline
 import torch
 import pandas as pd
 import base64
 from io import StringIO
+import logging
+import sys
+
+# Setup logging
+logging.basicConfig(filename='error2.log', level=logging.ERROR, format='%(asctime)s:%(levelname)s:%(message)s')
 
 # Initialize the tokenizer and model globally to avoid reloading them every time the function is called
 
 device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
 pipe = pipeline("token-classification", model="Isotonic/mdeberta-v3-base_finetuned_ai4privacy_v2",device=device)
 
@@ -33,19 +38,23 @@
             text = text.replace(entity['word'], f"[REDACTED {entity['entity']}]")
 
         processed_texts.append(text)
 
     return processed_texts
 
 def modify_csv(file, columns_to_redact):
-    df = pd.read_csv(file)
-    for column_name in columns_to_redact:
-        if column_name in df.columns:
-            df[column_name] = process_column(df[column_name].astype(str))
-    output = StringIO()
-    df.to_csv(output, index=False)
-    output.seek(0)
-    return df
+    try : 
+        df = pd.read_csv(file)
+        for column_name in columns_to_redact:
+            if column_name in df.columns:
+                df[column_name] = process_column(df[column_name].astype(str))
+        output = StringIO()
+        df.to_csv(output, index=False)
+        output.seek(0)
+        return df
+    except Exception as exc: 
+        logging.error(f"Error processing columns: {exc}", exc_info=True)
+
 
 def image_to_base64(image_path):
     with open(image_path, "rb") as image_file:
         return base64.b64encode(image_file.read()).decode('utf-8')
```

### Comparing `Kavach-0.2/README.md` & `Kavach-0.3/README.md`

 * *Files identical despite different names*

### Comparing `Kavach-0.2/tests/test_utils.py` & `Kavach-0.3/tests/test_utils.py`

 * *Files identical despite different names*

