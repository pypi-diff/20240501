# Comparing `tmp/ctdfjorder-0.0.3.tar.gz` & `tmp/ctdfjorder-0.0.4.tar.gz`

## Comparing `ctdfjorder-0.0.3.tar` & `ctdfjorder-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/CTDFjorder.iml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/build.bat
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/build.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/environment.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/meta.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/setup.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/make.bat
--rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/CTDFjorder/CTDFjorder.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/CTDFjorder/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/src/CTDFjorder/make.bat
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/LICENSE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/README.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ctdfjorder-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/CTDFjorder.iml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/build.bat
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/build.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/environment.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/meta.yaml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/setup.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/src/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/src/make.bat
+-rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/src/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/src/CTDFjorder/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/src/CTDFjorder/make.bat
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/LICENSE
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/README.md
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 ctdfjorder-0.0.4/PKG-INFO
```

### Comparing `ctdfjorder-0.0.3/.idea/workspace.xml` & `ctdfjorder-0.0.4/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `ctdfjorder-0.0.3/.idea/workspace.xml` & `ctdfjorder-0.0.4/.idea/workspace.xml`

```diff
@@ -57,14 +57,17 @@
     "kotlin-language-version-configured": "true",
     "last_opened_file_path": "/Users/nik/IdeaProjects/CTDFjorder/src",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
+    "project.structure.last.edited": "Modules",
+    "project.structure.proportion": "0.0",
+    "project.structure.side.proportion": "0.0",
     "run.code.analysis.last.selected.profile": "pProject Default",
     "settings.editor.selected.configurable": "editor.preferences.completion",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
@@ -83,15 +86,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="79559f9c-5462-40fb-9c71-dbede6c21cc8" name="Changes" comment=""/>
       <created>1714542246341</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714542246341</updated>
-      <workItem from="1714542247510" duration="16074000"/>
+      <workItem from="1714542247510" duration="16542000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="XSLT-Support.FileAssociations.UIState">
```

### Comparing `ctdfjorder-0.0.3/src/Makefile` & `ctdfjorder-0.0.4/src/Makefile`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.3/src/make.bat` & `ctdfjorder-0.0.4/src/make.bat`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.3/src/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.4/src/CTDFjorder/CTDFjorder.py`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.3/src/CTDFjorder/Makefile` & `ctdfjorder-0.0.4/src/CTDFjorder/Makefile`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.3/src/CTDFjorder/make.bat` & `ctdfjorder-0.0.4/src/CTDFjorder/make.bat`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.3/LICENSE` & `ctdfjorder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.3/pyproject.toml` & `ctdfjorder-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [project]
 name = "CTDFjorder"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Nikolas Yanek-Chrones", email="nikojb1001@gmail.com" },
 ]
 description = "A package for processing and analyzing CTD data."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
-    "python>=3.8",
-    "numpy",
-    "pandas",
-    "gsw",
-    "matplotlib",
-    "scipy",
-    "statsmodels",
-    "tabulate"
+    "python>=3.11",
+    "numpy>=1.26.4",
+    "pandas>=2.2.1",
+    "gsw>=3.6.17",
+    "matplotlib>=3.8.4",
+    "scipy>=1.11.4",
+    "statsmodels>=0.14.0",
+    "tabulate>=0.9.0",
+    "pyrsktools>=0.1.9"
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
 
     # Indicate who your project is intended for
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ctdfjorder-0.0.3/PKG-INFO` & `ctdfjorder-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.3
 Name: CTDFjorder
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for processing and analyzing CTD data.
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Author-email: Nikolas Yanek-Chrones <nikojb1001@gmail.com>
 License-File: LICENSE
 Keywords: CTD
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
-Requires-Dist: gsw
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: python>=3.8
-Requires-Dist: scipy
-Requires-Dist: statsmodels
-Requires-Dist: tabulate
+Requires-Dist: gsw>=3.6.17
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pandas>=2.2.1
+Requires-Dist: pyrsktools>=0.1.9
+Requires-Dist: python>=3.11
+Requires-Dist: scipy>=1.11.4
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: tabulate>=0.9.0
 Description-Content-Type: text/markdown
 
 # CTDFjorder
 
 Package for processing CTD files.
```

