# Comparing `tmp/runpynb-0.2.0.tar.gz` & `tmp/runpynb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpynb-0.2.0.tar", last modified: Mon Feb 13 06:54:43 2023, max compression
+gzip compressed data, was "runpynb-0.3.0.tar", last modified: Wed May  1 03:17:25 2024, max compression
```

## Comparing `runpynb-0.2.0.tar` & `runpynb-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 06:54:43.323049 runpynb-0.2.0/
--rw-rw-rw-   0        0        0     1096 2022-08-04 02:48:51.000000 runpynb-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     7218 2023-02-13 06:54:43.343631 runpynb-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6355 2022-09-08 04:41:10.000000 runpynb-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 06:54:43.328626 runpynb-0.2.0/runpynb/
--rw-rw-rw-   0        0        0       59 2023-02-13 06:54:01.000000 runpynb-0.2.0/runpynb/__init__.py
--rw-rw-rw-   0        0        0     3348 2023-02-13 06:54:01.000000 runpynb-0.2.0/runpynb/runpynb.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:54:43.340630 runpynb-0.2.0/runpynb/scripts/
--rw-rw-rw-   0        0        0     2198 2023-02-13 06:54:01.000000 runpynb-0.2.0/runpynb/scripts/runpynb
-drwxrwxrwx   0        0        0        0 2023-02-13 06:54:43.339630 runpynb-0.2.0/runpynb.egg-info/
--rw-rw-rw-   0        0        0     7218 2023-02-13 06:54:42.000000 runpynb-0.2.0/runpynb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-02-13 06:54:43.000000 runpynb-0.2.0/runpynb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 06:54:42.000000 runpynb-0.2.0/runpynb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-02-13 06:54:42.000000 runpynb-0.2.0/runpynb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-13 06:54:42.000000 runpynb-0.2.0/runpynb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-13 06:54:43.343631 runpynb-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1316 2023-02-13 06:54:01.000000 runpynb-0.2.0/setup.py
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-05-01 03:17:25.555159 runpynb-0.3.0/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     1096 2024-05-01 02:30:33.000000 runpynb-0.3.0/LICENSE
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     6682 2024-05-01 03:17:25.555159 runpynb-0.3.0/PKG-INFO
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     5995 2024-05-01 03:11:40.000000 runpynb-0.3.0/README.md
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-05-01 03:17:25.555159 runpynb-0.3.0/runpynb/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       59 2024-05-01 03:02:52.000000 runpynb-0.3.0/runpynb/__init__.py
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     3474 2024-05-01 03:11:40.000000 runpynb-0.3.0/runpynb/runpynb.py
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-05-01 03:17:25.555159 runpynb-0.3.0/runpynb/scripts/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     2196 2024-05-01 03:11:40.000000 runpynb-0.3.0/runpynb/scripts/runpynb
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-05-01 03:17:25.555159 runpynb-0.3.0/runpynb.egg-info/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     6682 2024-05-01 03:17:25.000000 runpynb-0.3.0/runpynb.egg-info/PKG-INFO
+-rw-r--r--   0 lsys      (1000) lsys      (1000)      243 2024-05-01 03:17:25.000000 runpynb-0.3.0/runpynb.egg-info/SOURCES.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)        1 2024-05-01 03:17:25.000000 runpynb-0.3.0/runpynb.egg-info/dependency_links.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       19 2024-05-01 03:17:25.000000 runpynb-0.3.0/runpynb.egg-info/requires.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)        8 2024-05-01 03:17:25.000000 runpynb-0.3.0/runpynb.egg-info/top_level.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       38 2024-05-01 03:17:25.555159 runpynb-0.3.0/setup.cfg
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     1316 2024-05-01 03:11:40.000000 runpynb-0.3.0/setup.py
```

### Comparing `runpynb-0.2.0/LICENSE` & `runpynb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runpynb-0.2.0/PKG-INFO` & `runpynb-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,163 +1,153 @@
-Metadata-Version: 2.1
-Name: runpynb
-Version: 0.2.0
-Summary: Run (and time) Jupyter Notebooks for command-line and makefile
-Home-page: https://github.com/lsys/runPyNB
-Author: Lucas Shen
-Author-email: lucas@lucasshen.com
-Maintainer: Lucas Shen
-Maintainer-email: lucas@lucasshen.com
-License: MIT
-Keywords: jupyter notebook,jupyter,command-line,makefile,make,nbconvert
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div id="top"></div> 
-
-# Run Jupyter notebooks quietly from command-line
-[![PyPI](https://img.shields.io/pypi/v/runpynb?color=brightgreen&label=PyPI)](https://pypi.org/project/runpynb/)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/runpynb?label=Latest%20release)
-<br>
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runpynb?label=Python%203.6%2B)](https://pypi.org/project/runpynb/)
-<br>
-[![DOI](https://zenodo.org/badge/520408889.svg)](https://zenodo.org/badge/latestdoi/520408889)
-
-`runPyNB` is a quick and dirty utility to run (and time) Jupyter notebooks from command-line and makefiles.
-
-<!------------------- Quickstart ------------------->
-## Quickstart
-Install from PyPI
-```bash
-pip install runpynb
-```
-
-General usage: `runpynb <notebook(s)> [options]` (".ipynb" not required)
-
-* `runpynb`: Run all notebooks in directory.
-
-    <pre>
-    $ runpynb</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/runall.gif)
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!------------------------ Usage ---------------------->
-## Usage
-
-* `runpynb <notebook(s)> -q`: Run quietly (`-q`).
-
-    <pre>
-    $ runpynb hello.ipynb -q</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/be-quiet.gif)
-    
-* `runpynb <notebook(s)> -qs`: Run quietly (`-q`) as a sequence of workflow (`-s`). Errors (eg in `error.ipynb`) will break the workflow.
-
-    <pre>
-    $ runpynb error.ipynb hello.ipynb -qs</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/as-sequence.gif)
-    
-* `runpynb <notebook(s)> -o`: Save output as separate notebook (`-o`), instead of overwriting existing notebook(s).
-
-    <pre>
-    $ runpynb hello.ipynb -o</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/output-as-separate-notebook.gif)
-    
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!---------------------- Options ---------------------->
-## Options
-```bash
-usage: runpynb [-h] [-t TIMEOUT] [-s] [-o] [-v VERSION] [-q] [notebooks ...]
-
-Run (and time) Jupyter notebooks silently in command-line.
-
-positional arguments:
-  notebooks             List of Jupyter notebooks (*.ipynb) to be run
-                        (default=all notebooks in path).
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -t TIMEOUT, --timeout TIMEOUT
-                        Seconds until a cell in the notebook timesout, which
-                        raises a Timeouterror exception (default is 3000=5
-                        mins).
-  -s, --sequence        Sequence implicit in notebook lists. If error occurs
-                        somewhere, stop entire pipeline.
-  -o, --output          Save output as a separate notebook with "-out"-suffix
-                        (e.g. *-out.ipynb) instead of overwriting existing
-                        file.
-  -v VERSION, --version VERSION
-                        Version of notebook to return (Default=No conversion).
-                        Notebook will be converted if necessary.
-  -q, --quiet           Be quiet and don't print messages (including run
-                        time). Caution: Does not suppress error messages.
-```
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-
-<!----------------- Project status ----------------->
-## Status
-[![Documentation Status](https://readthedocs.org/projects/runpynb/badge/?version=latest)](https://runpynb.readthedocs.io/en/latest/?badge=latest)
-<br>
-[![Build Status](https://app.travis-ci.com/LSYS/runPyNB.svg?branch=main)](https://app.travis-ci.com/LSYS/runPyNB)
-<br>
-[![Tests](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml)
-[![codecov](https://codecov.io/gh/LSYS/runPyNB/branch/main/graph/badge.svg?token=ZtC2IJ07Fa)](https://codecov.io/gh/LSYS/runPyNB)
-<br>
-[![CI](https://github.com/LSYS/runPyNB/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/build.yml)
-<br>
-[![CLI](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml)
-<br>
-[![Doclinks](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml)
-<p align="right">(<a href="#top">back to top</a>)</p>
-<br>
-
-
-<!---------------------- About --------------------->
-## More on this package
-
-This is a lightweight package that wraps around the official Jupyter [`nbformat`](https://nbformat.readthedocs.io/en/latest/) and [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/) modules.
-
-My workflow involves using [`Jupyter notebooks`](https://jupyter.org/) to clean, and analyze data.
-I use this utility to run notebooks silently from the command-line and [`Makefiles`](#usage-with-makefiles) (without converting from `.ipynb` files to `.py` files). 
-
-Related packages are [`guoquan/runnb`](https://github.com/guoquan/runnb) and [`vinayak-mehta/nbcommands`](https://github.com/vinayak-mehta/nbcommands) with a planned enhancement `nbtime` to run Jupyter notebooks from command-line.
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!---------------------- Build --------------------->
-## Usage with Makefiles
-A minimal workflow where `get-data.ipynb` takes 5000 seconds to prepare `data.csv`.
-And where `analyze.ipynb` uses `data.csv` to produce `output.png`.
-```makefile
-.DEFAULT_GOAL := output.png
-
-data.csv: get-data.ipynb
-	runpynb $^ -t 5000
-	
-output.png: analyze.ipynb data.csv
-	runpynb $< 
-```
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-
-<!----------------- Known issues ---------------->
-## Known Issues
-* [Build fails](https://github.com/LSYS/runPyNB/runs/7627883361?check_suite_focus=true) with Python 3.6 in Windows OS.
-* Notebooks with long execution time will require the `timeout` option (eg `runpynb notebook.ipynb -t 10000`).
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!-------------------- License ------------------->
-## License
-This package is licensed under the [MIT License](https://github.com/LSYS/runPyNB/blob/main/LICENSE).
-
-
+Metadata-Version: 2.1
+Name: runpynb
+Version: 0.3.0
+Summary: Run (and time) Jupyter Notebooks for command-line and makefile
+Home-page: https://github.com/lsys/runPyNB
+Author: Lucas Shen
+Author-email: lucas@lucasshen.com
+Maintainer: Lucas Shen
+Maintainer-email: lucas@lucasshen.com
+License: MIT
+Keywords: jupyter notebook,jupyter,command-line,makefile,make,nbconvert
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div id="top"></div> 
+
+# Run Jupyter notebooks quietly from command-line
+[![PyPI](https://img.shields.io/pypi/v/runpynb?color=brightgreen&label=PyPI)](https://pypi.org/project/runpynb/)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/runpynb?label=Latest%20release)
+<br>
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runpynb?label=Python%203.6%2B)](https://pypi.org/project/runpynb/)
+<br>
+[![DOI](https://zenodo.org/badge/520408889.svg)](https://zenodo.org/badge/latestdoi/520408889)
+
+`runPyNB` is a quick and dirty utility to run (and time) Jupyter notebooks from command-line and makefiles.
+
+<!------------------- Quickstart ------------------->
+## Quickstart
+Install from PyPI
+```bash
+pip install runpynb
+```
+
+General usage: `runpynb <notebook(s)> [options]` (".ipynb" not required)
+
+* `runpynb`: Run all notebooks in directory.
+
+    <pre>
+    $ runpynb</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/runall.gif)
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!------------------------ Usage ---------------------->
+## Usage
+
+* `runpynb <notebook(s)> -q`: Run quietly (`-q`).
+
+    <pre>
+    $ runpynb hello.ipynb -q</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/be-quiet.gif)
+    
+* `runpynb <notebook(s)> -qs`: Run quietly (`-q`) as a sequence of workflow (`-s`). Errors (eg in `error.ipynb`) will break the workflow.
+
+    <pre>
+    $ runpynb error.ipynb hello.ipynb -qs</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/as-sequence.gif)
+    
+* `runpynb <notebook(s)> -o`: Save output as separate notebook (`-o`), instead of overwriting existing notebook(s).
+
+    <pre>
+    $ runpynb hello.ipynb -o</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/output-as-separate-notebook.gif)
+    
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!---------------------- Options ---------------------->
+## Options
+```bash
+usage: runpynb [-h] [-t TIMEOUT] [-s] [-o] [-v VERSION] [-q] [notebooks ...]
+
+Run (and time) Jupyter notebooks silently in command-line.
+
+positional arguments:
+  notebooks             List of Jupyter notebooks (*.ipynb) to be run
+                        (default=all notebooks in path).
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -t TIMEOUT, --timeout TIMEOUT
+                        Seconds until a cell in the notebook timesout, which
+                        raises a Timeouterror exception (default is 3000=5
+                        mins).
+  -s, --sequence        Sequence implicit in notebook lists. If error occurs
+                        somewhere, stop entire pipeline.
+  -o, --output          Save output as a separate notebook with "-out"-suffix
+                        (e.g. *-out.ipynb) instead of overwriting existing
+                        file.
+  -v VERSION, --version VERSION
+                        Version of notebook to return (Default=No conversion).
+                        Notebook will be converted if necessary.
+  -q, --quiet           Be quiet and don't print messages (including run
+                        time). Caution: Does not suppress error messages.
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!----------------- Project status ----------------->
+## Status
+[![Documentation Status](https://readthedocs.org/projects/runpynb/badge/?version=latest)](https://runpynb.readthedocs.io/en/latest/?badge=latest)
+<br>
+[![Build Status](https://app.travis-ci.com/LSYS/runPyNB.svg?branch=main)](https://app.travis-ci.com/LSYS/runPyNB)
+<br>
+[![Tests](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/LSYS/runPyNB/branch/main/graph/badge.svg?token=ZtC2IJ07Fa)](https://codecov.io/gh/LSYS/runPyNB)
+<br>
+[![CI](https://github.com/LSYS/runPyNB/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/build.yml)
+<br>
+[![CLI](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml)
+<br>
+[![Doclinks](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml)
+<p align="right">(<a href="#top">back to top</a>)</p>
+<br>
+
+
+<!---------------------- About --------------------->
+## More on this package
+
+This is a lightweight package that wraps around the official Jupyter [`nbformat`](https://nbformat.readthedocs.io/en/latest/) and [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/) modules.
+
+My workflow involves using [`Jupyter notebooks`](https://jupyter.org/) to clean, and analyze data.
+I use this utility to run notebooks silently from the command-line and [`Makefiles`](#usage-with-makefiles) (without converting from `.ipynb` files to `.py` files). 
+
+Related packages are [`guoquan/runnb`](https://github.com/guoquan/runnb) and [`vinayak-mehta/nbcommands`](https://github.com/vinayak-mehta/nbcommands) with a planned enhancement `nbtime` to run Jupyter notebooks from command-line.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!---------------------- Build --------------------->
+## Usage with Makefiles
+A minimal workflow where `get-data.ipynb` takes 5000 seconds to prepare `data.csv`.
+And where `analyze.ipynb` uses `data.csv` to produce `output.png`.
+```makefile
+.DEFAULT_GOAL := output.png
+
+data.csv: get-data.ipynb
+	runpynb $^ -t 5000
+	
+output.png: analyze.ipynb data.csv
+	runpynb $< 
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!-------------------- License ------------------->
+## License
+This package is licensed under the [MIT License](https://github.com/LSYS/runPyNB/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: runpynb Version: 0.2.0 Summary: Run (and time)
+Metadata-Version: 2.1 Name: runpynb Version: 0.3.0 Summary: Run (and time)
 Jupyter Notebooks for command-line and makefile Home-page: https://github.com/
 lsys/runPyNB Author: Lucas Shen Author-email: lucas@lucasshen.com Maintainer:
 Lucas Shen Maintainer-email: lucas@lucasshen.com License: MIT Keywords: jupyter
-notebook,jupyter,command-line,makefile,make,nbconvert Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
+notebook,jupyter,command-line,makefile,make,nbconvert Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
+Content-Type: text/markdown License-File: LICENSE
 # Run Jupyter notebooks quietly from command-line [![PyPI](https://
 img.shields.io/pypi/v/runpynb?color=brightgreen&label=PyPI)](https://pypi.org/
 project/runpynb/) ![GitHub release (latest by date)](https://img.shields.io/
 github/v/release/lsys/runpynb?label=Latest%20release)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 runpynb?label=Python%203.6%2B)](https://pypi.org/project/runpynb/)
 [![DOI](https://zenodo.org/badge/520408889.svg)](https://zenodo.org/badge/
@@ -87,14 +87,9 @@
 notebooks from command-line.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage with Makefiles A minimal workflow where `get-data.ipynb` takes 5000
 seconds to prepare `data.csv`. And where `analyze.ipynb` uses `data.csv` to
 produce `output.png`. ```makefile .DEFAULT_GOAL := output.png data.csv: get-
 data.ipynb runpynb $^ -t 5000 output.png: analyze.ipynb data.csv runpynb $< ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Known Issues * [Build fails](https://github.com/LSYS/runPyNB/runs/
-7627883361?check_suite_focus=true) with Python 3.6 in Windows OS. * Notebooks
-with long execution time will require the `timeout` option (eg `runpynb
-notebook.ipynb -t 10000`).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## License This package is licensed under the [MIT License](https://github.com/
 LSYS/runPyNB/blob/main/LICENSE).
```

### Comparing `runpynb-0.2.0/README.md` & `runpynb-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -122,17 +122,10 @@
 	
 output.png: analyze.ipynb data.csv
 	runpynb $< 
 ```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
-<!----------------- Known issues ---------------->
-## Known Issues
-* [Build fails](https://github.com/LSYS/runPyNB/runs/7627883361?check_suite_focus=true) with Python 3.6 in Windows OS.
-* Notebooks with long execution time will require the `timeout` option (eg `runpynb notebook.ipynb -t 10000`).
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
 <!-------------------- License ------------------->
 ## License
 This package is licensed under the [MIT License](https://github.com/LSYS/runPyNB/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -76,14 +76,9 @@
 notebooks from command-line.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage with Makefiles A minimal workflow where `get-data.ipynb` takes 5000
 seconds to prepare `data.csv`. And where `analyze.ipynb` uses `data.csv` to
 produce `output.png`. ```makefile .DEFAULT_GOAL := output.png data.csv: get-
 data.ipynb runpynb $^ -t 5000 output.png: analyze.ipynb data.csv runpynb $< ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Known Issues * [Build fails](https://github.com/LSYS/runPyNB/runs/
-7627883361?check_suite_focus=true) with Python 3.6 in Windows OS. * Notebooks
-with long execution time will require the `timeout` option (eg `runpynb
-notebook.ipynb -t 10000`).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## License This package is licensed under the [MIT License](https://github.com/
 LSYS/runPyNB/blob/main/LICENSE).
```

### Comparing `runpynb-0.2.0/runpynb/runpynb.py` & `runpynb-0.3.0/runpynb/runpynb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import asyncio
 import os
 import sys
-from typing import Sequence
+from typing import Optional, Sequence
 
 import nbformat
 from nbconvert.preprocessors import ExecutePreprocessor
 from nbconvert.preprocessors.execute import CellExecutionError
 
 if sys.version_info[0] == 3 and sys.version_info[1] >= 8 and sys.platform.startswith("win"):
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 
 def run_notebooks(
     notebooks: Sequence[str],
-    timeout: int = 3600,
-    ver: int = None,
+    timeout: int = -1,
+    ver: Optional[int] = None,
     assequence: bool = False,
     output: bool = False,
     quiet: bool = False,
 ) -> None:
     """
     Takes a list of Jupyter notebooks and execute one by one.
     Parameters
     ----------
     notebooks (list-like)
             List of notebooks to be executed. ".ipynb" extension is implied and not required.
     timeout (int)
             Threshold in seconds before cell execution timeouts and throws a cell timeout error.
-            (Default = 3600 -> 1 hr)
+            (Default = -1 -> no limit)
     ver (int)
             Version of notebook to convert to and return.
             (Default is None)
     assequence (bool)
             If True, order of notebooks imply workflow and and error in any one notebook will stop
             entire pipeline.
             (Default = False. If a notebook fails, move on to executing the next notebook.)
@@ -61,16 +61,17 @@
 
             ep = ExecutePreprocessor(timeout=timeout, kernel_name="python3")
             print_or_quiet(f"Running notebook {ix+1}/{size_work}: {filename}", quiet=quiet)
 
             try:
                 ep.preprocess(nb)
                 print_or_quiet(f"Done {filename}.\n", quiet=quiet)
-            except CellExecutionError:
+            except CellExecutionError as cell_error:
                 print(f"Error executing {ix+1}/{size_work}: {filename}.\n")
+                print_or_quiet(f"Error executing {filename}: {cell_error}\n", quiet=quiet)
                 if assequence:
                     sys.exit(seq_err_msg)
             except TimeoutError:
                 print(f"Cell timeout error with {filename}.\n")
                 if assequence:
                     sys.exit(seq_err_msg)
             finally:
```

### Comparing `runpynb-0.2.0/runpynb/scripts/runpynb` & `runpynb-0.3.0/runpynb/scripts/runpynb`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     default=glob("*.ipynb"),
     help="List of Jupyter notebooks (*.ipynb) to be run (default=all notebooks in path).",
 )
 PARSER.add_argument(
     "-t",
     "--timeout",
     type=int,
-    default=3600,
+    default=-1,
     help="Seconds until a cell in the notebook timesout, which raises a Timeouterror exception (default is 3600 = 1 hr).",
 )
 PARSER.add_argument(
     "-s",
     "--sequence",
     action="store_true",
     help="Sequence implicit in notebook lists. If error occurs somewhere, stop entire pipeline.",
```

### Comparing `runpynb-0.2.0/runpynb.egg-info/PKG-INFO` & `runpynb-0.3.0/runpynb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,163 +1,153 @@
-Metadata-Version: 2.1
-Name: runpynb
-Version: 0.2.0
-Summary: Run (and time) Jupyter Notebooks for command-line and makefile
-Home-page: https://github.com/lsys/runPyNB
-Author: Lucas Shen
-Author-email: lucas@lucasshen.com
-Maintainer: Lucas Shen
-Maintainer-email: lucas@lucasshen.com
-License: MIT
-Keywords: jupyter notebook,jupyter,command-line,makefile,make,nbconvert
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div id="top"></div> 
-
-# Run Jupyter notebooks quietly from command-line
-[![PyPI](https://img.shields.io/pypi/v/runpynb?color=brightgreen&label=PyPI)](https://pypi.org/project/runpynb/)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/runpynb?label=Latest%20release)
-<br>
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runpynb?label=Python%203.6%2B)](https://pypi.org/project/runpynb/)
-<br>
-[![DOI](https://zenodo.org/badge/520408889.svg)](https://zenodo.org/badge/latestdoi/520408889)
-
-`runPyNB` is a quick and dirty utility to run (and time) Jupyter notebooks from command-line and makefiles.
-
-<!------------------- Quickstart ------------------->
-## Quickstart
-Install from PyPI
-```bash
-pip install runpynb
-```
-
-General usage: `runpynb <notebook(s)> [options]` (".ipynb" not required)
-
-* `runpynb`: Run all notebooks in directory.
-
-    <pre>
-    $ runpynb</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/runall.gif)
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!------------------------ Usage ---------------------->
-## Usage
-
-* `runpynb <notebook(s)> -q`: Run quietly (`-q`).
-
-    <pre>
-    $ runpynb hello.ipynb -q</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/be-quiet.gif)
-    
-* `runpynb <notebook(s)> -qs`: Run quietly (`-q`) as a sequence of workflow (`-s`). Errors (eg in `error.ipynb`) will break the workflow.
-
-    <pre>
-    $ runpynb error.ipynb hello.ipynb -qs</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/as-sequence.gif)
-    
-* `runpynb <notebook(s)> -o`: Save output as separate notebook (`-o`), instead of overwriting existing notebook(s).
-
-    <pre>
-    $ runpynb hello.ipynb -o</pre>
-    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/output-as-separate-notebook.gif)
-    
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!---------------------- Options ---------------------->
-## Options
-```bash
-usage: runpynb [-h] [-t TIMEOUT] [-s] [-o] [-v VERSION] [-q] [notebooks ...]
-
-Run (and time) Jupyter notebooks silently in command-line.
-
-positional arguments:
-  notebooks             List of Jupyter notebooks (*.ipynb) to be run
-                        (default=all notebooks in path).
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -t TIMEOUT, --timeout TIMEOUT
-                        Seconds until a cell in the notebook timesout, which
-                        raises a Timeouterror exception (default is 3000=5
-                        mins).
-  -s, --sequence        Sequence implicit in notebook lists. If error occurs
-                        somewhere, stop entire pipeline.
-  -o, --output          Save output as a separate notebook with "-out"-suffix
-                        (e.g. *-out.ipynb) instead of overwriting existing
-                        file.
-  -v VERSION, --version VERSION
-                        Version of notebook to return (Default=No conversion).
-                        Notebook will be converted if necessary.
-  -q, --quiet           Be quiet and don't print messages (including run
-                        time). Caution: Does not suppress error messages.
-```
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-
-<!----------------- Project status ----------------->
-## Status
-[![Documentation Status](https://readthedocs.org/projects/runpynb/badge/?version=latest)](https://runpynb.readthedocs.io/en/latest/?badge=latest)
-<br>
-[![Build Status](https://app.travis-ci.com/LSYS/runPyNB.svg?branch=main)](https://app.travis-ci.com/LSYS/runPyNB)
-<br>
-[![Tests](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml)
-[![codecov](https://codecov.io/gh/LSYS/runPyNB/branch/main/graph/badge.svg?token=ZtC2IJ07Fa)](https://codecov.io/gh/LSYS/runPyNB)
-<br>
-[![CI](https://github.com/LSYS/runPyNB/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/build.yml)
-<br>
-[![CLI](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml)
-<br>
-[![Doclinks](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml)
-<p align="right">(<a href="#top">back to top</a>)</p>
-<br>
-
-
-<!---------------------- About --------------------->
-## More on this package
-
-This is a lightweight package that wraps around the official Jupyter [`nbformat`](https://nbformat.readthedocs.io/en/latest/) and [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/) modules.
-
-My workflow involves using [`Jupyter notebooks`](https://jupyter.org/) to clean, and analyze data.
-I use this utility to run notebooks silently from the command-line and [`Makefiles`](#usage-with-makefiles) (without converting from `.ipynb` files to `.py` files). 
-
-Related packages are [`guoquan/runnb`](https://github.com/guoquan/runnb) and [`vinayak-mehta/nbcommands`](https://github.com/vinayak-mehta/nbcommands) with a planned enhancement `nbtime` to run Jupyter notebooks from command-line.
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!---------------------- Build --------------------->
-## Usage with Makefiles
-A minimal workflow where `get-data.ipynb` takes 5000 seconds to prepare `data.csv`.
-And where `analyze.ipynb` uses `data.csv` to produce `output.png`.
-```makefile
-.DEFAULT_GOAL := output.png
-
-data.csv: get-data.ipynb
-	runpynb $^ -t 5000
-	
-output.png: analyze.ipynb data.csv
-	runpynb $< 
-```
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-
-<!----------------- Known issues ---------------->
-## Known Issues
-* [Build fails](https://github.com/LSYS/runPyNB/runs/7627883361?check_suite_focus=true) with Python 3.6 in Windows OS.
-* Notebooks with long execution time will require the `timeout` option (eg `runpynb notebook.ipynb -t 10000`).
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-<!-------------------- License ------------------->
-## License
-This package is licensed under the [MIT License](https://github.com/LSYS/runPyNB/blob/main/LICENSE).
-
-
+Metadata-Version: 2.1
+Name: runpynb
+Version: 0.3.0
+Summary: Run (and time) Jupyter Notebooks for command-line and makefile
+Home-page: https://github.com/lsys/runPyNB
+Author: Lucas Shen
+Author-email: lucas@lucasshen.com
+Maintainer: Lucas Shen
+Maintainer-email: lucas@lucasshen.com
+License: MIT
+Keywords: jupyter notebook,jupyter,command-line,makefile,make,nbconvert
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div id="top"></div> 
+
+# Run Jupyter notebooks quietly from command-line
+[![PyPI](https://img.shields.io/pypi/v/runpynb?color=brightgreen&label=PyPI)](https://pypi.org/project/runpynb/)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/runpynb?label=Latest%20release)
+<br>
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runpynb?label=Python%203.6%2B)](https://pypi.org/project/runpynb/)
+<br>
+[![DOI](https://zenodo.org/badge/520408889.svg)](https://zenodo.org/badge/latestdoi/520408889)
+
+`runPyNB` is a quick and dirty utility to run (and time) Jupyter notebooks from command-line and makefiles.
+
+<!------------------- Quickstart ------------------->
+## Quickstart
+Install from PyPI
+```bash
+pip install runpynb
+```
+
+General usage: `runpynb <notebook(s)> [options]` (".ipynb" not required)
+
+* `runpynb`: Run all notebooks in directory.
+
+    <pre>
+    $ runpynb</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/runall.gif)
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!------------------------ Usage ---------------------->
+## Usage
+
+* `runpynb <notebook(s)> -q`: Run quietly (`-q`).
+
+    <pre>
+    $ runpynb hello.ipynb -q</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/be-quiet.gif)
+    
+* `runpynb <notebook(s)> -qs`: Run quietly (`-q`) as a sequence of workflow (`-s`). Errors (eg in `error.ipynb`) will break the workflow.
+
+    <pre>
+    $ runpynb error.ipynb hello.ipynb -qs</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/as-sequence.gif)
+    
+* `runpynb <notebook(s)> -o`: Save output as separate notebook (`-o`), instead of overwriting existing notebook(s).
+
+    <pre>
+    $ runpynb hello.ipynb -o</pre>
+    ![](https://raw.githubusercontent.com/lsys/runpynb/main/assets/_docs/output-as-separate-notebook.gif)
+    
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!---------------------- Options ---------------------->
+## Options
+```bash
+usage: runpynb [-h] [-t TIMEOUT] [-s] [-o] [-v VERSION] [-q] [notebooks ...]
+
+Run (and time) Jupyter notebooks silently in command-line.
+
+positional arguments:
+  notebooks             List of Jupyter notebooks (*.ipynb) to be run
+                        (default=all notebooks in path).
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -t TIMEOUT, --timeout TIMEOUT
+                        Seconds until a cell in the notebook timesout, which
+                        raises a Timeouterror exception (default is 3000=5
+                        mins).
+  -s, --sequence        Sequence implicit in notebook lists. If error occurs
+                        somewhere, stop entire pipeline.
+  -o, --output          Save output as a separate notebook with "-out"-suffix
+                        (e.g. *-out.ipynb) instead of overwriting existing
+                        file.
+  -v VERSION, --version VERSION
+                        Version of notebook to return (Default=No conversion).
+                        Notebook will be converted if necessary.
+  -q, --quiet           Be quiet and don't print messages (including run
+                        time). Caution: Does not suppress error messages.
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!----------------- Project status ----------------->
+## Status
+[![Documentation Status](https://readthedocs.org/projects/runpynb/badge/?version=latest)](https://runpynb.readthedocs.io/en/latest/?badge=latest)
+<br>
+[![Build Status](https://app.travis-ci.com/LSYS/runPyNB.svg?branch=main)](https://app.travis-ci.com/LSYS/runPyNB)
+<br>
+[![Tests](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/LSYS/runPyNB/branch/main/graph/badge.svg?token=ZtC2IJ07Fa)](https://codecov.io/gh/LSYS/runPyNB)
+<br>
+[![CI](https://github.com/LSYS/runPyNB/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/build.yml)
+<br>
+[![CLI](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/cli.yml)
+<br>
+[![Doclinks](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml/badge.svg?branch=main)](https://github.com/LSYS/runPyNB/actions/workflows/doclinks.yml)
+<p align="right">(<a href="#top">back to top</a>)</p>
+<br>
+
+
+<!---------------------- About --------------------->
+## More on this package
+
+This is a lightweight package that wraps around the official Jupyter [`nbformat`](https://nbformat.readthedocs.io/en/latest/) and [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/) modules.
+
+My workflow involves using [`Jupyter notebooks`](https://jupyter.org/) to clean, and analyze data.
+I use this utility to run notebooks silently from the command-line and [`Makefiles`](#usage-with-makefiles) (without converting from `.ipynb` files to `.py` files). 
+
+Related packages are [`guoquan/runnb`](https://github.com/guoquan/runnb) and [`vinayak-mehta/nbcommands`](https://github.com/vinayak-mehta/nbcommands) with a planned enhancement `nbtime` to run Jupyter notebooks from command-line.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!---------------------- Build --------------------->
+## Usage with Makefiles
+A minimal workflow where `get-data.ipynb` takes 5000 seconds to prepare `data.csv`.
+And where `analyze.ipynb` uses `data.csv` to produce `output.png`.
+```makefile
+.DEFAULT_GOAL := output.png
+
+data.csv: get-data.ipynb
+	runpynb $^ -t 5000
+	
+output.png: analyze.ipynb data.csv
+	runpynb $< 
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!-------------------- License ------------------->
+## License
+This package is licensed under the [MIT License](https://github.com/LSYS/runPyNB/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: runpynb Version: 0.2.0 Summary: Run (and time)
+Metadata-Version: 2.1 Name: runpynb Version: 0.3.0 Summary: Run (and time)
 Jupyter Notebooks for command-line and makefile Home-page: https://github.com/
 lsys/runPyNB Author: Lucas Shen Author-email: lucas@lucasshen.com Maintainer:
 Lucas Shen Maintainer-email: lucas@lucasshen.com License: MIT Keywords: jupyter
-notebook,jupyter,command-line,makefile,make,nbconvert Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
+notebook,jupyter,command-line,makefile,make,nbconvert Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
+Content-Type: text/markdown License-File: LICENSE
 # Run Jupyter notebooks quietly from command-line [![PyPI](https://
 img.shields.io/pypi/v/runpynb?color=brightgreen&label=PyPI)](https://pypi.org/
 project/runpynb/) ![GitHub release (latest by date)](https://img.shields.io/
 github/v/release/lsys/runpynb?label=Latest%20release)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 runpynb?label=Python%203.6%2B)](https://pypi.org/project/runpynb/)
 [![DOI](https://zenodo.org/badge/520408889.svg)](https://zenodo.org/badge/
@@ -87,14 +87,9 @@
 notebooks from command-line.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage with Makefiles A minimal workflow where `get-data.ipynb` takes 5000
 seconds to prepare `data.csv`. And where `analyze.ipynb` uses `data.csv` to
 produce `output.png`. ```makefile .DEFAULT_GOAL := output.png data.csv: get-
 data.ipynb runpynb $^ -t 5000 output.png: analyze.ipynb data.csv runpynb $< ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Known Issues * [Build fails](https://github.com/LSYS/runPyNB/runs/
-7627883361?check_suite_focus=true) with Python 3.6 in Windows OS. * Notebooks
-with long execution time will require the `timeout` option (eg `runpynb
-notebook.ipynb -t 10000`).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## License This package is licensed under the [MIT License](https://github.com/
 LSYS/runPyNB/blob/main/LICENSE).
```

### Comparing `runpynb-0.2.0/setup.py` & `runpynb-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 install_requires = ['nbformat', 'nbconvert']
 setup(
     name="runpynb",
-    version="0.2.0",
+    version="0.3.0",
     license='MIT',
     author="Lucas Shen",
     author_email="lucas@lucasshen.com",
     maintainer="Lucas Shen",
     maintainer_email="lucas@lucasshen.com",    
 
     url="https://github.com/lsys/runPyNB",
```

