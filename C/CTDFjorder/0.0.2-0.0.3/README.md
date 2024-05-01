# Comparing `tmp/ctdfjorder-0.0.2.tar.gz` & `tmp/ctdfjorder-0.0.3.tar.gz`

## Comparing `ctdfjorder-0.0.2.tar` & `ctdfjorder-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/CTDFjorder.iml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/build.bat
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/build.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/environment.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/meta.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/setup.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/src/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/src/make.bat
--rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/src/CTDFjorder/CTDFjorder.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/src/CTDFjorder/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/src/CTDFjorder/make.bat
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/LICENSE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ctdfjorder-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/CTDFjorder.iml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/build.bat
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/build.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/environment.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/meta.yaml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/setup.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/make.bat
+-rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/CTDFjorder/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/CTDFjorder/make.bat
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/LICENSE
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/README.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/PKG-INFO
```

### Comparing `ctdfjorder-0.0.2/.idea/workspace.xml` & `ctdfjorder-0.0.3/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `ctdfjorder-0.0.2/.idea/workspace.xml` & `ctdfjorder-0.0.3/.idea/workspace.xml`

```diff
@@ -83,15 +83,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="79559f9c-5462-40fb-9c71-dbede6c21cc8" name="Changes" comment=""/>
       <created>1714542246341</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714542246341</updated>
-      <workItem from="1714542247510" duration="15853000"/>
+      <workItem from="1714542247510" duration="16074000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="XSLT-Support.FileAssociations.UIState">
```

### Comparing `ctdfjorder-0.0.2/src/Makefile` & `ctdfjorder-0.0.3/src/Makefile`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.2/src/make.bat` & `ctdfjorder-0.0.3/src/make.bat`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.2/src/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.3/src/CTDFjorder/CTDFjorder.py`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.2/src/CTDFjorder/Makefile` & `ctdfjorder-0.0.3/src/CTDFjorder/Makefile`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.2/src/CTDFjorder/make.bat` & `ctdfjorder-0.0.3/src/CTDFjorder/make.bat`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.2/LICENSE` & `ctdfjorder-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.2/pyproject.toml` & `ctdfjorder-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "CTDFjorder"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Nikolas Yanek-Chrones", email="nikojb1001@gmail.com" },
 ]
 description = "A package for processing and analyzing CTD data."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
-    "python>=3.11",
+    "python>=3.8",
     "numpy",
     "pandas",
     "gsw",
     "matplotlib",
     "scipy",
     "statsmodels",
     "tabulate"
```

### Comparing `ctdfjorder-0.0.2/PKG-INFO` & `ctdfjorder-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CTDFjorder
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for processing and analyzing CTD data.
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Author-email: Nikolas Yanek-Chrones <nikojb1001@gmail.com>
 License-File: LICENSE
 Keywords: CTD
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: gsw
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: python>=3.11
+Requires-Dist: python>=3.8
 Requires-Dist: scipy
 Requires-Dist: statsmodels
 Requires-Dist: tabulate
 Description-Content-Type: text/markdown
 
 # CTDFjorder
```

