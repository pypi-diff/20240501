# Comparing `tmp/pytrials-0.3.0.tar.gz` & `tmp/pytrials-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrials-0.3.0.tar", last modified: Sun Jul  9 18:09:49 2023, max compression
+gzip compressed data, was "pytrials-1.0.0.tar", last modified: Wed May  1 14:55:01 2024, max compression
```

## Comparing `pytrials-0.3.0.tar` & `pytrials-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      235 2023-07-09 18:08:52.000000 pytrials-0.3.0/AUTHORS.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3275 2023-07-09 17:21:39.000000 pytrials-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      443 2023-07-09 18:08:10.000000 pytrials-0.3.0/HISTORY.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2023-07-09 17:21:39.000000 pytrials-0.3.0/LICENSE
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      262 2023-07-09 17:21:39.000000 pytrials-0.3.0/MANIFEST.in
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3311 2023-07-09 18:09:49.270042 pytrials-0.3.0/PKG-INFO
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2088 2023-07-09 17:21:39.000000 pytrials-0.3.0/README.rst
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/docs/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      609 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/Makefile
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/authors.rst
--rwxr-xr-x   0 jvfe      (1000) jvfe      (1000)     4911 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/conf.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       33 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/contributing.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/history.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      305 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/index.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1106 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/installation.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      770 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/make.bat
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       61 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/modules.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      445 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/pytrials.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       27 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/readme.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       71 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/usage.rst
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/pytrials/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      137 2023-07-09 18:09:34.000000 pytrials-0.3.0/pytrials/__init__.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     6029 2023-07-09 18:07:29.000000 pytrials-0.3.0/pytrials/client.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      963 2023-07-09 17:58:10.000000 pytrials-0.3.0/pytrials/utils.py
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/pytrials.egg-info/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3311 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/PKG-INFO
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      597 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/SOURCES.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/dependency_links.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/not-zip-safe
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/requires.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/top_level.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      542 2023-07-09 18:09:49.270042 pytrials-0.3.0/setup.cfg
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1467 2023-07-09 18:09:34.000000 pytrials-0.3.0/setup.py
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/tests/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       38 2023-07-09 17:21:39.000000 pytrials-0.3.0/tests/__init__.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2941 2023-07-09 17:21:39.000000 pytrials-0.3.0/tests/test_client.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      151 2023-07-09 17:21:39.000000 pytrials-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.570495 pytrials-1.0.0/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      235 2023-07-09 18:08:52.000000 pytrials-1.0.0/AUTHORS.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3275 2023-07-09 17:21:39.000000 pytrials-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      683 2024-05-01 14:49:31.000000 pytrials-1.0.0/HISTORY.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2023-07-09 17:21:39.000000 pytrials-1.0.0/LICENSE
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      295 2024-05-01 13:18:49.000000 pytrials-1.0.0/MANIFEST.in
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3279 2024-05-01 14:55:01.570495 pytrials-1.0.0/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1816 2024-05-01 14:09:27.000000 pytrials-1.0.0/README.rst
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.570495 pytrials-1.0.0/docs/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      609 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/Makefile
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.567162 pytrials-1.0.0/docs/_build/
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.567162 pytrials-1.0.0/docs/_build/html/
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.570495 pytrials-1.0.0/docs/_build/html/_static/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      286 2024-05-01 14:34:49.000000 pytrials-1.0.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       90 2024-05-01 14:34:49.000000 pytrials-1.0.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       90 2024-05-01 14:34:49.000000 pytrials-1.0.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/authors.rst
+-rwxr-xr-x   0 jvfe      (1000) jvfe      (1000)     4768 2024-05-01 14:39:26.000000 pytrials-1.0.0/docs/conf.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       33 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/contributing.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/history.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      305 2024-05-01 14:39:06.000000 pytrials-1.0.0/docs/index.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1106 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/installation.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      770 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/make.bat
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       61 2024-05-01 14:39:30.000000 pytrials-1.0.0/docs/modules.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      445 2024-05-01 14:40:19.000000 pytrials-1.0.0/docs/pytrials.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       27 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/readme.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       71 2023-07-09 17:21:39.000000 pytrials-1.0.0/docs/usage.rst
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.570495 pytrials-1.0.0/pytrials/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      244 2024-05-01 14:53:07.000000 pytrials-1.0.0/pytrials/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     5673 2024-05-01 14:08:29.000000 pytrials-1.0.0/pytrials/client.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1215 2024-05-01 12:39:18.000000 pytrials-1.0.0/pytrials/fields.csv
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      878 2024-05-01 13:26:45.000000 pytrials-1.0.0/pytrials/utils.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.570495 pytrials-1.0.0/pytrials.egg-info/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3279 2024-05-01 14:55:01.000000 pytrials-1.0.0/pytrials.egg-info/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      720 2024-05-01 14:55:01.000000 pytrials-1.0.0/pytrials.egg-info/SOURCES.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2024-05-01 14:55:01.000000 pytrials-1.0.0/pytrials.egg-info/dependency_links.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2024-05-01 14:55:01.000000 pytrials-1.0.0/pytrials.egg-info/not-zip-safe
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2024-05-01 14:55:01.000000 pytrials-1.0.0/pytrials.egg-info/requires.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2024-05-01 14:55:01.000000 pytrials-1.0.0/pytrials.egg-info/top_level.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      542 2024-05-01 14:55:01.570495 pytrials-1.0.0/setup.cfg
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1467 2024-05-01 14:53:07.000000 pytrials-1.0.0/setup.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2024-05-01 14:55:01.570495 pytrials-1.0.0/tests/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       38 2023-07-09 17:21:39.000000 pytrials-1.0.0/tests/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2404 2024-05-01 14:23:29.000000 pytrials-1.0.0/tests/test_client.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      151 2023-07-09 17:21:39.000000 pytrials-1.0.0/tests/test_utils.py
```

### Comparing `pytrials-0.3.0/CONTRIBUTING.rst` & `pytrials-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.3.0/LICENSE` & `pytrials-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrials-0.3.0/PKG-INFO` & `pytrials-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrials
-Version: 0.3.0
+Version: 1.0.0
 Summary: Python wrapper around the clinicaltrials.gov API
 Home-page: https://github.com/jvfe/pytrials
 Author: João Vitor F. Cavalcante
 Author-email: jvfe@ufrn.edu.br
 License: BSD license
 Keywords: pytrials clinical-trials clinical trials tabular text-mining text opendata
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -58,31 +58,25 @@
 ^^^^^^^^^^^
 ::
 
     from pytrials.client import ClinicalTrials
 
     ct = ClinicalTrials()
 
-    # Get 50 full studies related to Coronavirus and COVID in json format.
+    # Get 50 full studies related to Coronavirus and COVID in csv format.
     ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=50)
 
-    # Get the NCTId, Condition and Brief title fields from 500 studies related to Coronavirus and Covid, in csv format.
+    # Get the NCTId, Condition and Brief title fields from 1000 studies related to Coronavirus and Covid, in csv format.
     corona_fields = ct.get_study_fields(
         search_expr="Coronavirus+COVID",
-        fields=["NCTId", "Condition", "BriefTitle"],
-        max_studies=500,
+        fields=["NCT Number", "Conditions", "Study Title"],
+        max_studies=1000,
         fmt="csv",
     )
 
-    # Get the count of studies related to Coronavirus and COVID.
-    # ClinicalTrials limits API queries to 1000 records
-    # Count of studies may be useful to build loops when you want to retrieve more than 1000 records
-
-    ct.get_study_count(search_expr="Coronavirus+COVID")
-
     # Read the csv data in Pandas
     import pandas as pd
 
     pd.DataFrame.from_records(corona_fields[1:], columns=corona_fields[0])
 
 Credits
 -------
@@ -119,7 +113,18 @@
 * Add classic prefix to url - #10
 * Raise error if API status is not ok - #11
 
 0.3.0 (2023-07-09)
 ------------------
 
 * Add min_rnk option to get_study_fields - #12
+
+
+1.0.0 (2024-05-01)
+------------------
+
+Migrates to version 2.0 of the ClinicalTrials API
+
+* Add support for the new API version
+* Add support for the new API fields
+* **Remove get_study_count function**
+* Allow CSV format in full_studies
```

### Comparing `pytrials-0.3.0/README.rst` & `pytrials-1.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -37,31 +37,25 @@
 ^^^^^^^^^^^
 ::
 
     from pytrials.client import ClinicalTrials
 
     ct = ClinicalTrials()
 
-    # Get 50 full studies related to Coronavirus and COVID in json format.
+    # Get 50 full studies related to Coronavirus and COVID in csv format.
     ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=50)
 
-    # Get the NCTId, Condition and Brief title fields from 500 studies related to Coronavirus and Covid, in csv format.
+    # Get the NCTId, Condition and Brief title fields from 1000 studies related to Coronavirus and Covid, in csv format.
     corona_fields = ct.get_study_fields(
         search_expr="Coronavirus+COVID",
-        fields=["NCTId", "Condition", "BriefTitle"],
-        max_studies=500,
+        fields=["NCT Number", "Conditions", "Study Title"],
+        max_studies=1000,
         fmt="csv",
     )
 
-    # Get the count of studies related to Coronavirus and COVID.
-    # ClinicalTrials limits API queries to 1000 records
-    # Count of studies may be useful to build loops when you want to retrieve more than 1000 records
-
-    ct.get_study_count(search_expr="Coronavirus+COVID")
-
     # Read the csv data in Pandas
     import pandas as pd
 
     pd.DataFrame.from_records(corona_fields[1:], columns=corona_fields[0])
 
 Credits
 -------
```

### Comparing `pytrials-0.3.0/docs/Makefile` & `pytrials-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytrials-0.3.0/docs/conf.py` & `pytrials-1.0.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,45 +15,44 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-
-sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath('..'))
 
 import pytrials
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode", "sphinxcontrib.napoleon"]
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
+templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = ".rst"
+source_suffix = '.rst'
 
 # The master toctree document.
-master_doc = "index"
+master_doc = 'index'
 
 # General information about the project.
-project = "pytrials"
-copyright = "2020, João Vitor F. Cavalcante"
-author = "João Vitor F. Cavalcante"
+project = 'Pytrials'
+copyright = "2024, jvfe"
+author = "jvfe"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = pytrials.__version__
@@ -66,96 +65,99 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
+pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "alabaster"
+html_theme = 'alabaster'
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+html_static_path = ['_static']
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "pytrialsdoc"
+htmlhelp_basename = 'pytrialsdoc'
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
+
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
+
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
+
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (
-        master_doc,
-        "pytrials.tex",
-        "pytrials Documentation",
-        "João Vitor F. Cavalcante",
-        "manual",
-    ),
+    (master_doc, 'pytrials.tex',
+     'Pytrials Documentation',
+     'jvfe', 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "pytrials", "pytrials Documentation", [author], 1)]
+man_pages = [
+    (master_doc, 'pytrials',
+     'Pytrials Documentation',
+     [author], 1)
+]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (
-        master_doc,
-        "pytrials",
-        "pytrials Documentation",
-        author,
-        "pytrials",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
+    (master_doc, 'pytrials',
+     'Pytrials Documentation',
+     author,
+     'pytrials',
+     'One line description of project.',
+     'Miscellaneous'),
 ]
 
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytrials-0.3.0/docs/installation.rst` & `pytrials-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.3.0/docs/make.bat` & `pytrials-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytrials-0.3.0/pytrials/client.py` & `pytrials-1.0.0/pytrials/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from pytrials.utils import json_handler, csv_handler
+from pytrials import study_fields
+import csv
 
 
 class ClinicalTrials:
     """ClinicalTrials API client
 
     Provides functions to easily access the ClinicalTrials.gov API
     (https://classic.clinicaltrials.gov/api/)
@@ -10,42 +12,48 @@
 
     Attributes:
         study_fields: List of all study fields you can use in your query.
         api_info: Tuple containing the API version number and the last
         time the database was updated.
     """
 
-    _BASE_URL = "https://classic.clinicaltrials.gov/api/"
-    _INFO = "info/"
-    _QUERY = "query/"
-    _JSON = "fmt=json"
-    _CSV = "fmt=csv"
+    _BASE_URL = "https://clinicaltrials.gov/api/v2/"
+    _JSON = "format=json"
+    _CSV = "format=csv"
 
     def __init__(self):
         self.api_info = self.__api_info()
 
     @property
     def study_fields(self):
-        fields_list = json_handler(
-            f"{self._BASE_URL}{self._INFO}study_fields_list?{self._JSON}"
-        )
-        return fields_list["StudyFields"]["Fields"]
+        """List of all study fields you can use in your query."""
+
+        csv_fields = []
+        json_fields = []
+        with open(study_fields, "r") as f:
+            reader = csv.DictReader(f)
+            for row in reader:
+                csv_fields.append(row["Column Name"])
+                json_fields.append(row["Included Data Fields"].split("|"))
+
+        return {
+            "csv": csv_fields,
+            "json": [item for sublist in json_fields for item in sublist],
+        }
 
     def __api_info(self):
         """Returns information about the API"""
-        last_updated = json_handler(
-            f"{self._BASE_URL}{self._INFO}data_vrs?{self._JSON}"
-        )["DataVrs"]
-        api_version = json_handler(f"{self._BASE_URL}{self._INFO}api_vrs?{self._JSON}")[
-            "APIVrs"
-        ]
+        req = json_handler(f"{self._BASE_URL}version")
+        last_updated = req["dataTimestamp"]
+
+        api_version = req["apiVersion"]
 
         return api_version, last_updated
 
-    def get_full_studies(self, search_expr, max_studies=50):
+    def get_full_studies(self, search_expr, max_studies=50, fmt="csv"):
         """Returns all content for a maximum of 100 study records.
 
         Retrieves information from the full studies endpoint, which gets all study fields.
         This endpoint can only output JSON (Or not-supported XML) format and does not allow
         requests for more than 100 studies at once.
 
         Args:
@@ -56,24 +64,35 @@
 
         Returns:
             dict: Object containing the information queried with the search expression.
 
         Raises:
             ValueError: The number of studies can only be between 1 and 100
         """
-        if max_studies > 100 or max_studies < 1:
-            raise ValueError("The number of studies can only be between 1 and 100")
+        if fmt == "csv":
+            format = self._CSV
+            handler = csv_handler
+        elif fmt == "json":
+            format = self._JSON
+            handler = json_handler
+        else:
+            raise ValueError("Format argument has to be either 'csv' or 'json")
+
+        if max_studies > 1000 or max_studies < 1:
+            raise ValueError("The number of studies can only be between 1 and 1000")
 
-        req = f"full_studies?expr={search_expr}&max_rnk={max_studies}&{self._JSON}"
+        req = f"studies?{format}&markupFormat=legacy&query.term={search_expr}&pageSize={max_studies}"
 
-        full_studies = json_handler(f"{self._BASE_URL}{self._QUERY}{req}")
+        full_studies = handler(f"{self._BASE_URL}{req}")
 
         return full_studies
 
-    def get_study_fields(self, search_expr, fields, max_studies=50, min_rnk=1, fmt="csv"):
+    def get_study_fields(
+        self, search_expr, fields, max_studies=50, fmt="csv"
+    ):
         """Returns study content for specified fields
 
         Retrieves information from the study fields endpoint, which acquires specified information
         from a large (max 1000) studies. To see a list of all possible fields, check the class'
         study_fields attribute.
 
         Args:
@@ -92,53 +111,32 @@
 
         Raises:
             ValueError: The number of studies can only be between 1 and 1000
             ValueError: One of the fields is not valid! Check the study_fields attribute
                 for a list of valid ones.
             ValueError: Format argument has to be either 'csv' or 'json'
         """
+        if fmt == "csv":
+            format = self._CSV
+            handler = csv_handler
+        elif fmt == "json":
+            format = self._JSON
+            handler = json_handler
+        else:
+            raise ValueError("Format argument has to be either 'csv' or 'json")
+
         if max_studies > 1000 or max_studies < 1:
             raise ValueError("The number of studies can only be between 1 and 1000")
-        elif not set(fields).issubset(self.study_fields):
+        elif not set(fields).issubset(self.study_fields[fmt]):
             raise ValueError(
-                "One of the fields is not valid! Check the study_fields attribute for a list of valid ones."
+                "One of the fields is not valid!"
+                "Check the study_fields attribute for a list of valid ones."
+                "They are different depending on the return format, json or csv."
             )
         else:
-            concat_fields = ",".join(fields)
-            req = f"study_fields?expr={search_expr}&min_rnk={min_rnk}&max_rnk={max_studies+min_rnk-1}&fields={concat_fields}"
-            if fmt == "csv":
-                url = f"{self._BASE_URL}{self._QUERY}{req}&{self._CSV}"
-                return csv_handler(url)
-
-            elif fmt == "json":
-                url = f"{self._BASE_URL}{self._QUERY}{req}&{self._JSON}"
-                return json_handler(url)
-
-            else:
-                raise ValueError("Format argument has to be either 'csv' or 'json'")
-
-    def get_study_count(self, search_expr):
-        """Returns study count for specified search expression
-
-        Retrieves the count of studies matching the text entered in search_expr.
-
-        Args:
-            search_expr (str): A string containing a search expression as specified by
-                `their documentation <https://clinicaltrials.gov/api/gui/ref/syntax#searchExpr>`_.
-
-        Returns:
-            An integer
-
-        Raises:
-            ValueError: The search expression cannot be blank.
-        """
-        if not set(search_expr):
-            raise ValueError("The search expression cannot be blank.")
-        else:
-            req = f"study_fields?expr={search_expr}&max_rnk=1&fields=NCTId"
-            url = f"{self._BASE_URL}{self._QUERY}{req}&{self._JSON}"
-            returned_data = json_handler(url)
-            study_count = returned_data["StudyFieldsResponse"]["NStudiesFound"]
-            return study_count
+            concat_fields = "|".join(fields)
+            req = f"&query.term={search_expr}&markupFormat=legacy&fields={concat_fields}&pageSize={max_studies}"
+            url = f"{self._BASE_URL}studies?{format}{req}"
+            return handler(url)
 
     def __repr__(self):
         return f"ClinicalTrials.gov client v{self.api_info[0]}, database last updated {self.api_info[1]}"
```

### Comparing `pytrials-0.3.0/pytrials/utils.py` & `pytrials-1.0.0/pytrials/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,12 +26,11 @@
 
 def csv_handler(url):
     """Returns request in CSV (list of records) format"""
 
     response = request_ct(url)
     decoded_content = response.content.decode("utf-8")
 
-    split_by_blank = re.split(r"\n\s*\n", decoded_content)  # Extracts header info
-    cr = csv.reader(split_by_blank[1].splitlines(), delimiter=",")
+    cr = csv.reader(decoded_content.splitlines(), delimiter=",")
     records = list(cr)
 
     return records
```

### Comparing `pytrials-0.3.0/pytrials.egg-info/PKG-INFO` & `pytrials-1.0.0/pytrials.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrials
-Version: 0.3.0
+Version: 1.0.0
 Summary: Python wrapper around the clinicaltrials.gov API
 Home-page: https://github.com/jvfe/pytrials
 Author: João Vitor F. Cavalcante
 Author-email: jvfe@ufrn.edu.br
 License: BSD license
 Keywords: pytrials clinical-trials clinical trials tabular text-mining text opendata
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -58,31 +58,25 @@
 ^^^^^^^^^^^
 ::
 
     from pytrials.client import ClinicalTrials
 
     ct = ClinicalTrials()
 
-    # Get 50 full studies related to Coronavirus and COVID in json format.
+    # Get 50 full studies related to Coronavirus and COVID in csv format.
     ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=50)
 
-    # Get the NCTId, Condition and Brief title fields from 500 studies related to Coronavirus and Covid, in csv format.
+    # Get the NCTId, Condition and Brief title fields from 1000 studies related to Coronavirus and Covid, in csv format.
     corona_fields = ct.get_study_fields(
         search_expr="Coronavirus+COVID",
-        fields=["NCTId", "Condition", "BriefTitle"],
-        max_studies=500,
+        fields=["NCT Number", "Conditions", "Study Title"],
+        max_studies=1000,
         fmt="csv",
     )
 
-    # Get the count of studies related to Coronavirus and COVID.
-    # ClinicalTrials limits API queries to 1000 records
-    # Count of studies may be useful to build loops when you want to retrieve more than 1000 records
-
-    ct.get_study_count(search_expr="Coronavirus+COVID")
-
     # Read the csv data in Pandas
     import pandas as pd
 
     pd.DataFrame.from_records(corona_fields[1:], columns=corona_fields[0])
 
 Credits
 -------
@@ -119,7 +113,18 @@
 * Add classic prefix to url - #10
 * Raise error if API status is not ok - #11
 
 0.3.0 (2023-07-09)
 ------------------
 
 * Add min_rnk option to get_study_fields - #12
+
+
+1.0.0 (2024-05-01)
+------------------
+
+Migrates to version 2.0 of the ClinicalTrials API
+
+* Add support for the new API version
+* Add support for the new API fields
+* **Remove get_study_count function**
+* Allow CSV format in full_studies
```

### Comparing `pytrials-0.3.0/pytrials.egg-info/SOURCES.txt` & `pytrials-1.0.0/pytrials.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/pytrials.rst
 docs/readme.rst
 docs/usage.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 pytrials/__init__.py
 pytrials/client.py
+pytrials/fields.csv
 pytrials/utils.py
 pytrials.egg-info/PKG-INFO
 pytrials.egg-info/SOURCES.txt
 pytrials.egg-info/dependency_links.txt
 pytrials.egg-info/not-zip-safe
 pytrials.egg-info/requires.txt
 pytrials.egg-info/top_level.txt
```

### Comparing `pytrials-0.3.0/setup.cfg` & `pytrials-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 1.0.0
 commit = True
 tag = True
 
 [bumpversion:file:pytrials/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `pytrials-0.3.0/setup.py` & `pytrials-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords="pytrials clinical-trials clinical trials tabular text-mining text opendata",
     name="pytrials",
     packages=find_packages(include=["pytrials", "pytrials.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/jvfe/pytrials",
-    version="0.3.0",
+    version="1.0.0",
     zip_safe=False,
 )
```

### Comparing `pytrials-0.3.0/tests/test_client.py` & `pytrials-1.0.0/tests/test_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,95 +4,81 @@
 from pytest import raises
 from pytrials.client import ClinicalTrials
 
 ct = ClinicalTrials()
 
 
 def test_full_studies():
-    fifty_studies = ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=50)
+    fifty_studies = ct.get_full_studies(
+        search_expr="Coronavirus+COVID", max_studies=50, fmt="json"
+    )
 
-    assert [*fifty_studies["FullStudiesResponse"].keys()] == [
-        "APIVrs",
-        "DataVrs",
-        "Expression",
-        "NStudiesAvail",
-        "NStudiesFound",
-        "MinRank",
-        "MaxRank",
-        "NStudiesReturned",
-        "FullStudies",
+    assert [*fifty_studies["studies"][0].keys()] == [
+        "protocolSection",
+        "derivedSection",
+        "hasResults",
     ]
 
-    assert len(fifty_studies["FullStudiesResponse"]["FullStudies"]) == 50
+    assert len(fifty_studies["studies"]) == 50
 
 
 def test_full_studies_max():
     hundred_studies = ct.get_full_studies(
-        search_expr="Coronavirus+COVID", max_studies=100
+        search_expr="Coronavirus+COVID", max_studies=100, fmt="json"
     )
 
-    assert [*hundred_studies["FullStudiesResponse"].keys()] == [
-        "APIVrs",
-        "DataVrs",
-        "Expression",
-        "NStudiesAvail",
-        "NStudiesFound",
-        "MinRank",
-        "MaxRank",
-        "NStudiesReturned",
-        "FullStudies",
+    assert [*hundred_studies["studies"][0].keys()] == [
+        "protocolSection",
+        "derivedSection",
+        "hasResults",
     ]
 
-    assert len(hundred_studies["FullStudiesResponse"]["FullStudies"]) == 100
+    assert len(hundred_studies["studies"]) == 100
 
 
 def test_full_studies_below():
     with raises(ValueError):
         ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=-100)
 
 
 def test_full_studies_above():
     with raises(ValueError):
-        ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=150)
+        ct.get_full_studies(search_expr="Coronavirus+COVID", max_studies=2000)
 
 
 def test_study_fields_csv():
     study_fields_csv = ct.get_study_fields(
         search_expr="Coronavirus+COVID",
-        fields=["NCTId", "Condition", "BriefTitle"],
+        fields=["NCT Number", "Conditions", "Study Title"],
         max_studies=50,
         fmt="csv",
     )
 
     assert len(study_fields_csv) == 51
-    assert study_fields_csv[0] == ["Rank", "NCTId", "Condition", "BriefTitle"]
+    assert study_fields_csv[0] == ["NCT Number", "Study Title", "Conditions"]
 
 
 def test_study_fields_json():
     study_fields_json = ct.get_study_fields(
         search_expr="Coronavirus+COVID",
         fields=["NCTId", "Condition", "BriefTitle"],
         max_studies=50,
         fmt="json",
     )
 
-    assert [*study_fields_json["StudyFieldsResponse"].keys()] == [
-        "APIVrs",
-        "DataVrs",
-        "Expression",
-        "NStudiesAvail",
-        "NStudiesFound",
-        "MinRank",
-        "MaxRank",
-        "NStudiesReturned",
-        "FieldList",
-        "StudyFields",
+    assert [
+        *study_fields_json["studies"][0]["protocolSection"][
+            "identificationModule"
+        ].keys()
+    ] == [
+        "nctId",
+        "briefTitle",
     ]
 
-    assert len(study_fields_json["StudyFieldsResponse"]["StudyFields"]) == 50
+    assert len(study_fields_json["studies"]) == 50
 
 
 def test_study_fake_fields():
     with raises(ValueError):
         ct.get_study_fields(
             search_expr="Coronavirus+COVID",
             fields=["NCTId", "I AM NOT A REAL FIELD"],
@@ -105,13 +91,7 @@
     with raises(ValueError):
         ct.get_study_fields(
             search_expr="Coronavirus+COVID",
             fields=["NCTId", "BriefTitle"],
             max_studies=50,
             fmt="I AM NOT A REAL FORMAT",
         )
-
-
-def test_study_count():
-    study_count = ct.get_study_count(search_expr="Coronavirus+COVID")
-
-    assert study_count > 2200
```

