# Comparing `tmp/arnie-0.1.5.tar.gz` & `tmp/arnie-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arnie-0.1.5.tar", last modified: Fri Sep 15 20:10:57 2023, max compression
+gzip compressed data, was "/home/runner/work/arnie/arnie/dist/.tmp-azro7kue/arnie-0.1.6.tar", last modified: Wed May  1 05:10:38 2024, max compression
```

## Comparing `arnie-0.1.5.tar` & `arnie-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-15 20:10:57.865554 arnie-0.1.5/
--rw-r--r--   0 thomas     (501) staff       (20)     1090 2023-03-16 05:45:18.000000 arnie-0.1.5/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)     3525 2023-09-15 20:10:57.865274 arnie-0.1.5/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     2894 2023-09-01 19:05:44.000000 arnie-0.1.5/README.md
--rw-r--r--   0 thomas     (501) staff       (20)      704 2023-09-15 20:10:07.000000 arnie-0.1.5/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-09-15 20:10:57.865604 arnie-0.1.5/setup.cfg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-15 20:10:57.854624 arnie-0.1.5/src/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-15 20:10:57.858954 arnie-0.1.5/src/arnie/
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     9676 2023-09-15 19:48:37.000000 arnie-0.1.5/src/arnie/bpps.py
--rw-r--r--   0 thomas     (501) staff       (20)     2315 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/free_energy.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-15 20:10:57.861256 arnie-0.1.5/src/arnie/mea/
--rwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/mea/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     5897 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/mea/mea.py
--rw-r--r--   0 thomas     (501) staff       (20)     6303 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/mea/mea_utils.py
--rw-r--r--   0 thomas     (501) staff       (20)     1159 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/mea/threshknot.py
--rw-r--r--   0 thomas     (501) staff       (20)    16003 2023-09-01 22:29:58.000000 arnie-0.1.5/src/arnie/mfe.py
--rw-r--r--   0 thomas     (501) staff       (20)     2826 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/mfe_bootstrap.py
--rw-r--r--   0 thomas     (501) staff       (20)    22137 2023-09-15 20:07:48.000000 arnie-0.1.5/src/arnie/pfunc.py
--rw-r--r--   0 thomas     (501) staff       (20)    18977 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/pk_predictors.py
--rw-r--r--   0 thomas     (501) staff       (20)     5427 2023-09-01 19:05:44.000000 arnie-0.1.5/src/arnie/sample_structures.py
--rw-r--r--   0 thomas     (501) staff       (20)    36859 2023-09-15 20:04:56.000000 arnie-0.1.5/src/arnie/utils.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-15 20:10:57.860345 arnie-0.1.5/src/arnie.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     3525 2023-09-15 20:10:57.000000 arnie-0.1.5/src/arnie.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      795 2023-09-15 20:10:57.000000 arnie-0.1.5/src/arnie.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-09-15 20:10:57.000000 arnie-0.1.5/src/arnie.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       25 2023-09-15 20:10:57.000000 arnie-0.1.5/src/arnie.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)       10 2023-09-15 20:10:57.000000 arnie-0.1.5/src/arnie.egg-info/top_level.txt
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-15 20:10:57.864846 arnie-0.1.5/tests/
--rw-r--r--   0 thomas     (501) staff       (20)      721 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_bpps.py
--rw-r--r--   0 thomas     (501) staff       (20)   120803 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_converters.py
--rw-r--r--   0 thomas     (501) staff       (20)     3198 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_evaluation_metrics.py
--rw-r--r--   0 thomas     (501) staff       (20)     5811 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_file_readers.py
--rw-r--r--   0 thomas     (501) staff       (20)     4332 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_helix_getting_and_removing.py
--rw-r--r--   0 thomas     (501) staff       (20)      530 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_linearpartition.py
--rw-r--r--   0 thomas     (501) staff       (20)      749 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_pfunc.py
--rw-r--r--   0 thomas     (501) staff       (20)     6668 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_pk.py
--rw-r--r--   0 thomas     (501) staff       (20)      426 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_sample_struct.py
--rw-r--r--   0 thomas     (501) staff       (20)      281 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_settings.py
--rw-r--r--   0 thomas     (501) staff       (20)      546 2023-09-01 19:05:44.000000 arnie-0.1.5/tests/test_vfold_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:38.000000 arnie-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 05:10:33.000000 arnie-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-01 05:10:38.000000 arnie-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-01 05:10:33.000000 arnie-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-01 05:10:33.000000 arnie-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:10:38.000000 arnie-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:38.000000 arnie-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/bpps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/free_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie/mea/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/mea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/mea/mea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/mea/mea_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/mea/threshknot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/mfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/mfe_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22137 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/pfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/pk_predictors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/sample_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36926 2024-05-01 05:10:33.000000 arnie-0.1.6/src/arnie/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 05:10:38.000000 arnie-0.1.6/src/arnie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:10:38.000000 arnie-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_bpps.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120803 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_evaluation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_helix_getting_and_removing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_linearpartition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_pfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_pk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_sample_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 05:10:33.000000 arnie-0.1.6/tests/test_vfold_versions.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `arnie-0.1.5/LICENSE` & `arnie-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/PKG-INFO` & `arnie-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: arnie
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python utility library to estimate, compare, and reweight RNA energetics across many secondary structure algorithms.
 Author-email: Das Lab <thedaslab@stanford.edu>
 Project-URL: Homepage, https://github.com/DasLab/arnie
 Project-URL: Bug Tracker, https://github.com/DasLab/arnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.15
-Requires-Dist: scipy>=1.5.0
 
 # arnie
 Python API to compute RNA energetics and do structure prediction across multiple secondary structure packages.
 
 Currently supported:
 
 - Vienna \[1\] [https://www.tbi.univie.ac.at/RNA/#download]
@@ -47,14 +45,19 @@
 
 `test`: unit tests (still in work)
 
 `mea`: code for computing Maximum Expected Accuracy structures.
 
 `RNAGraph`: DEPRECATED, see https://github.com/DasLab/RiboGraphViz/ for current version of the code. Code to process and visualize secondary structures as graph objects.
 
+## Install:
+`arnie` is [available on PyPI](https://pypi.org/projectarnie/).
+
+`pip install arnie`
+
 ## Setup:
 
 1. To use Arnie, you will create a file that contains the paths to the software packages that Arnie is wrapping. See [`docs/setup_doc.md`](docs/setup_doc.md) for installation instructions and troubleshooting tips, as well as instructions for setting up the arnie file.
 
 Quickstart: an example file is provided in `example_arnie_file.txt`.
```

### Comparing `arnie-0.1.5/README.md` & `arnie-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 
 `test`: unit tests (still in work)
 
 `mea`: code for computing Maximum Expected Accuracy structures.
 
 `RNAGraph`: DEPRECATED, see https://github.com/DasLab/RiboGraphViz/ for current version of the code. Code to process and visualize secondary structures as graph objects.
 
+## Install:
+`arnie` is [available on PyPI](https://pypi.org/projectarnie/).
+
+`pip install arnie`
+
 ## Setup:
 
 1. To use Arnie, you will create a file that contains the paths to the software packages that Arnie is wrapping. See [`docs/setup_doc.md`](docs/setup_doc.md) for installation instructions and troubleshooting tips, as well as instructions for setting up the arnie file.
 
 Quickstart: an example file is provided in `example_arnie_file.txt`.
```

### Comparing `arnie-0.1.5/pyproject.toml` & `arnie-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arnie"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Das Lab", email="thedaslab@stanford.edu" },
 ]
 description = "A Python utility library to estimate, compare, and reweight RNA energetics across many secondary structure algorithms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arnie-0.1.5/src/arnie/bpps.py` & `arnie-0.1.6/src/arnie/bpps.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/free_energy.py` & `arnie-0.1.6/src/arnie/free_energy.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/mea/mea.py` & `arnie-0.1.6/src/arnie/mea/mea.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/mea/mea_utils.py` & `arnie-0.1.6/src/arnie/mea/mea_utils.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/mea/threshknot.py` & `arnie-0.1.6/src/arnie/mea/threshknot.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/mfe.py` & `arnie-0.1.6/src/arnie/mfe.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/mfe_bootstrap.py` & `arnie-0.1.6/src/arnie/mfe_bootstrap.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/pfunc.py` & `arnie-0.1.6/src/arnie/pfunc.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/pk_predictors.py` & `arnie-0.1.6/src/arnie/pk_predictors.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/sample_structures.py` & `arnie-0.1.6/src/arnie/sample_structures.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/src/arnie/utils.py` & `arnie-0.1.6/src/arnie/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,17 +767,17 @@
         for i, bpA in enumerate(max_group):
             for bpB in max_group[i:]:
                 if bpA not in to_remove and bpB not in to_remove:
                     if [bpA, bpB] in conflict_list or [bpB, bpA] in conflict_list:
                         to_remove.append(bpB)
         group = [bp for bp in max_group if bp not in to_remove]
         groups.append(group)
-        non_redudant_bp_list = current_bp_conflicts
-        conflict_list = [conflict for conflict in conflict_list if conflict[0]
-                         not in group and conflict[1] not in group]
+        # remove group from list
+        non_redudant_bp_list = [bp for bp in non_redudant_bp_list if bp not in group] # current_bp_conflicts
+        # conflict_list = [conflict for conflict in conflict_list if conflict[0] not in group and conflict[1] not in group]
     return groups
 
 
 ###############################################################################
 # ORPHANED unused anywhere in package
 # figure out utility, take outside of utils and document or depricate
 ###############################################################################
```

### Comparing `arnie-0.1.5/src/arnie.egg-info/PKG-INFO` & `arnie-0.1.6/src/arnie.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: arnie
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python utility library to estimate, compare, and reweight RNA energetics across many secondary structure algorithms.
 Author-email: Das Lab <thedaslab@stanford.edu>
 Project-URL: Homepage, https://github.com/DasLab/arnie
 Project-URL: Bug Tracker, https://github.com/DasLab/arnie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.15
-Requires-Dist: scipy>=1.5.0
 
 # arnie
 Python API to compute RNA energetics and do structure prediction across multiple secondary structure packages.
 
 Currently supported:
 
 - Vienna \[1\] [https://www.tbi.univie.ac.at/RNA/#download]
@@ -47,14 +45,19 @@
 
 `test`: unit tests (still in work)
 
 `mea`: code for computing Maximum Expected Accuracy structures.
 
 `RNAGraph`: DEPRECATED, see https://github.com/DasLab/RiboGraphViz/ for current version of the code. Code to process and visualize secondary structures as graph objects.
 
+## Install:
+`arnie` is [available on PyPI](https://pypi.org/projectarnie/).
+
+`pip install arnie`
+
 ## Setup:
 
 1. To use Arnie, you will create a file that contains the paths to the software packages that Arnie is wrapping. See [`docs/setup_doc.md`](docs/setup_doc.md) for installation instructions and troubleshooting tips, as well as instructions for setting up the arnie file.
 
 Quickstart: an example file is provided in `example_arnie_file.txt`.
```

### Comparing `arnie-0.1.5/src/arnie.egg-info/SOURCES.txt` & `arnie-0.1.6/src/arnie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_bpps.py` & `arnie-0.1.6/tests/test_bpps.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_converters.py` & `arnie-0.1.6/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_evaluation_metrics.py` & `arnie-0.1.6/tests/test_evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_file_readers.py` & `arnie-0.1.6/tests/test_file_readers.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_helix_getting_and_removing.py` & `arnie-0.1.6/tests/test_helix_getting_and_removing.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_linearpartition.py` & `arnie-0.1.6/tests/test_linearpartition.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_pfunc.py` & `arnie-0.1.6/tests/test_pfunc.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_pk.py` & `arnie-0.1.6/tests/test_pk.py`

 * *Files identical despite different names*

### Comparing `arnie-0.1.5/tests/test_vfold_versions.py` & `arnie-0.1.6/tests/test_vfold_versions.py`

 * *Files identical despite different names*

