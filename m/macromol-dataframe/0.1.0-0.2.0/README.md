# Comparing `tmp/macromol_dataframe-0.1.0.tar.gz` & `tmp/macromol_dataframe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macromol_dataframe-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "macromol_dataframe-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `macromol_dataframe-0.1.0.tar` & `macromol_dataframe-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1136 2024-03-27 21:05:57.506057 macromol_dataframe-0.1.0/README.rst
--rw-r--r--   0        0        0      157 2024-03-27 21:05:58.322054 macromol_dataframe-0.1.0/macromol_dataframe/__init__.py
--rw-r--r--   0        0        0     2387 2024-03-27 21:05:57.506057 macromol_dataframe-0.1.0/macromol_dataframe/atoms.py
--rw-r--r--   0        0        0     4460 2024-03-27 21:05:57.506057 macromol_dataframe-0.1.0/macromol_dataframe/coords.py
--rw-r--r--   0        0        0    12364 2024-03-27 21:05:57.506057 macromol_dataframe-0.1.0/macromol_dataframe/mmcif.py
--rw-r--r--   0        0        0     3098 2024-03-27 21:05:57.506057 macromol_dataframe-0.1.0/macromol_dataframe/testing.py
--rw-r--r--   0        0        0     1605 2024-03-27 21:05:57.506057 macromol_dataframe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 macromol_dataframe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3977 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/README.md
+-rw-r--r--   0        0        0      199 2024-05-01 20:08:43.874938 macromol_dataframe-0.2.0/macromol_dataframe/__init__.py
+-rw-r--r--   0        0        0     2389 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/atoms.py
+-rw-r--r--   0        0        0     4460 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/coords.py
+-rw-r--r--   0        0        0      953 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/error.py
+-rw-r--r--   0        0        0    20127 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/mmcif.py
+-rw-r--r--   0        0        0     1017 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/pymol.py
+-rw-r--r--   0        0        0     7009 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/testing.py
+-rw-r--r--   0        0        0     1617 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5118 1970-01-01 00:00:00.000000 macromol_dataframe-0.2.0/PKG-INFO
```

### Comparing `macromol_dataframe-0.1.0/macromol_dataframe/atoms.py` & `macromol_dataframe-0.2.0/macromol_dataframe/atoms.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     - High resolution structures are much more likely to include hydrogens, but 
       we don't want our model to be able to distinguish between high- and
       low-resolution structures.  That means either adding hydrogens to low- 
       resolution structures, or removing them from high-resolution structures.  
       The latter is easier and doesn't involve adding data that's not in the 
       actual dataset.
     """
-    return atoms.filter(pl.col('element').is_in(['H', 'D']))
+    return atoms.filter(~pl.col('element').is_in(['H', 'D']))
 
 def prune_water(atoms):
     """
     Remove all water molecules from the structure.
 
     There are two reasons for doing this:
 
@@ -40,15 +40,15 @@
 
     - Even in high-resolution structures, many of the waters that end up in 
       the model are not very highly structured, and may not be informative.  
       Removing all the water makes the input less noisy.  Plus, the presence of 
       highly-structured waters can still be inferred from the macromolecule 
       itself.
     """
-    return atoms.filter(pl.col('comp_id').is_in(['HOH', 'DOD']))
+    return atoms.filter(~pl.col('comp_id').is_in(['HOH', 'DOD']))
 
 
 def get_atom_coords(
         atoms: Atoms,
         *,
         homogeneous: bool=False,
 ) -> Coords3 | Coords4:
```

### Comparing `macromol_dataframe-0.1.0/macromol_dataframe/coords.py` & `macromol_dataframe-0.2.0/macromol_dataframe/coords.py`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.1.0/pyproject.toml` & `macromol_dataframe-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "macromol_dataframe"
 authors = [
   {name = "Kale Kundert", email = "kale@thekunderts.net"},
 ]
-readme = 'README.rst'
+readme = 'README.md'
 dynamic = ["version", "description"]
 requires-python = "~=3.10"
 classifiers = [
   'Programming Language :: Python :: 3',
 ]
 dependencies = [
     'gemmi',
     'numpy',
+    'parsy',
     'polars',
     'scipy',
 ]
 
 [project.optional-dependencies]
 test = [
   'pytest',
```

