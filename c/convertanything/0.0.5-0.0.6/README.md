# Comparing `tmp/convertanything-0.0.5.tar.gz` & `tmp/convertanything-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convertanything-0.0.5.tar", last modified: Wed May  1 21:13:18 2024, max compression
+gzip compressed data, was "convertanything-0.0.6.tar", last modified: Wed May  1 21:26:12 2024, max compression
```

## Comparing `convertanything-0.0.5.tar` & `convertanything-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:13:18.880257 convertanything-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 21:13:08.000000 convertanything-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 21:13:08.000000 convertanything-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 21:13:08.000000 convertanything-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 21:13:18.880257 convertanything-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-01 21:13:08.000000 convertanything-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:13:18.880257 convertanything-0.0.5/convertanything/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-01 21:13:08.000000 convertanything-0.0.5/convertanything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:13:18.880257 convertanything-0.0.5/convertanything.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 21:13:18.000000 convertanything-0.0.5/convertanything.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 21:13:18.000000 convertanything-0.0.5/convertanything.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:13:18.000000 convertanything-0.0.5/convertanything.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 21:13:18.000000 convertanything-0.0.5/convertanything.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 21:13:18.000000 convertanything-0.0.5/convertanything.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-01 21:13:08.000000 convertanything-0.0.5/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 21:13:08.000000 convertanything-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 21:13:08.000000 convertanything-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:13:18.880257 convertanything-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-01 21:13:08.000000 convertanything-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:26:12.036835 convertanything-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 21:26:07.000000 convertanything-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 21:26:07.000000 convertanything-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 21:26:07.000000 convertanything-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 21:26:12.032835 convertanything-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-01 21:26:07.000000 convertanything-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:26:12.032835 convertanything-0.0.6/convertanything/
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-01 21:26:07.000000 convertanything-0.0.6/convertanything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:26:12.032835 convertanything-0.0.6/convertanything.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 21:26:12.000000 convertanything-0.0.6/convertanything.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 21:26:12.000000 convertanything-0.0.6/convertanything.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:26:12.000000 convertanything-0.0.6/convertanything.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 21:26:12.000000 convertanything-0.0.6/convertanything.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 21:26:12.000000 convertanything-0.0.6/convertanything.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-01 21:26:07.000000 convertanything-0.0.6/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 21:26:07.000000 convertanything-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 21:26:07.000000 convertanything-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:26:12.036835 convertanything-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-01 21:26:07.000000 convertanything-0.0.6/setup.py
```

### Comparing `convertanything-0.0.5/LICENSE` & `convertanything-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `convertanything-0.0.5/PKG-INFO` & `convertanything-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convertanything
-Version: 0.0.5
+Version: 0.0.6
 Summary: convertanything is a Python package that allows you to convert any text into a structured format according to the schema provided.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
```

### Comparing `convertanything-0.0.5/README.md` & `convertanything-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `convertanything-0.0.5/convertanything/__init__.py` & `convertanything-0.0.6/convertanything/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,18 @@
         top_p=0.95,
         stream=False,
         extra_body={
             "system_message": system_message,
         },
     )
     response = completion.choices[0].message.content
-    response = str(response).split("```json")[1].split("```")[0].strip()
+    if "```json" in response:
+        response = response.split("```json")[1].split("```")[0].strip()
+    elif "```" in response:
+        response = response.split("```")[1].strip()
     try:
         response = json.loads(response)
         return model(**response)
     except:
         print(response)
         print("Failed to convert the response to the model, trying again.")
         return convertanything(input_string=input_string, model=model)
```

### Comparing `convertanything-0.0.5/convertanything.egg-info/PKG-INFO` & `convertanything-0.0.6/convertanything.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convertanything
-Version: 0.0.5
+Version: 0.0.6
 Summary: convertanything is a Python package that allows you to convert any text into a structured format according to the schema provided.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
```

### Comparing `convertanything-0.0.5/example.ipynb` & `convertanything-0.0.6/example.ipynb`

 * *Files identical despite different names*

### Comparing `convertanything-0.0.5/setup.py` & `convertanything-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="convertanything",
-    version="0.0.5",
+    version="0.0.6",
     description="convertanything is a Python package that allows you to convert any text into a structured format according to the schema provided.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

