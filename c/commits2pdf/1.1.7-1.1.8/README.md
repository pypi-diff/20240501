# Comparing `tmp/commits2pdf-1.1.7.tar.gz` & `tmp/commits2pdf-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commits2pdf-1.1.7.tar", last modified: Thu Apr 11 06:39:42 2024, max compression
+gzip compressed data, was "commits2pdf-1.1.8.tar", last modified: Wed May  1 09:15:24 2024, max compression
```

## Comparing `commits2pdf-1.1.7.tar` & `commits2pdf-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:39:42.271887 commits2pdf-1.1.7/
--rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.1.7/LICENCE.md
--rw-rw-rw-   0        0        0     8340 2024-04-11 06:39:42.270891 commits2pdf-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     7454 2024-04-10 07:27:14.000000 commits2pdf-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 06:39:42.252431 commits2pdf-1.1.7/commits2pdf/
--rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.1.7/commits2pdf/__init__.py
--rw-rw-rw-   0        0        0    10749 2024-04-09 05:21:34.000000 commits2pdf-1.1.7/commits2pdf/cli.py
--rw-rw-rw-   0        0        0    13044 2024-04-11 06:34:51.000000 commits2pdf-1.1.7/commits2pdf/commits.py
--rw-rw-rw-   0        0        0     3264 2024-04-11 06:17:00.000000 commits2pdf-1.1.7/commits2pdf/constants.py
--rw-rw-rw-   0        0        0      308 2024-04-07 03:56:00.000000 commits2pdf-1.1.7/commits2pdf/logger.py
--rw-rw-rw-   0        0        0     7100 2024-04-07 10:55:21.000000 commits2pdf-1.1.7/commits2pdf/render_cairo.py
--rw-rw-rw-   0        0        0    10118 2024-04-11 06:35:28.000000 commits2pdf-1.1.7/commits2pdf/render_fpdf.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:39:42.268894 commits2pdf-1.1.7/commits2pdf.egg-info/
--rw-rw-rw-   0        0        0     8340 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 06:39:42.271887 commits2pdf-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1223 2024-04-11 06:37:14.000000 commits2pdf-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/commits2pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/render_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/commits2pdf/render_fpdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/commits2pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 09:15:24.000000 commits2pdf-1.1.8/commits2pdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:15:24.061236 commits2pdf-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 09:15:18.000000 commits2pdf-1.1.8/setup.py
```

### Comparing `commits2pdf-1.1.7/LICENCE.md` & `commits2pdf-1.1.8/LICENCE.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Tomas Vana
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 Tomas Vana
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `commits2pdf-1.1.7/README.md` & `commits2pdf-1.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-# commits2pdf
-Visualise a GitHub repo's commit history in PDF form via the command-line
-<br><br>
-## Dependencies
-`pycairo`<br>
-`GitPython`<br>
-`fpdf`
-<br><br>
-## Installation
-**Requires [pip](https://pip.pypa.io/en/stable/installation/)**
-
-Make a virtual environment (recommended)
-```
-pip install virtualenv OR pip3 install virtualenv
-python -m venv venv OR python3 -m venv venv
-ON MACOS/UNIX: source venv/bin/activate
-ON WINDOW: venv\scripts\activate
-```
-
-Install the package:
-```
-pip install commits2pdf OR pip3 install commits2pdf
-```
-**Scroll down for usage information**.
-
-If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)
-<br><br>
-## Command-line parameters
-```
-  -h, --help            show this help message and exit
-  -O OWNER, --owner OWNER
-                        The owner of the git repository. Required.
-  -o OUTPUT, --output OUTPUT
-                        Path to your PDF output. Set to "." by default.
-  -b BRANCH, --branch BRANCH
-                        The repository branch. Set to "main" by default.
-  -a AUTHORS, --authors AUTHORS
-                        Filter commits from a comma-separated list of authors. Format: <author@email.com> OR <author1@email.com,author2@email.com> etc. Set to all authors   
-                        by default.
-  -s START_DATE, --start_date START_DATE
-                        Filter from start date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
-  -e END_DATE, --end_date END_DATE
-                        Filter to end date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
-  -r, --reverse         Output the commits from newest to oldest. Set to oldest to newest by default
-  -d, --dark            Toggle dark mode for the output PDF. Set to "light" by default.
-  -po, --prevent-open   Prevent the program from automatically opening the directory the PDF was created in.
-  -sc SCALING, --scaling SCALING
-                        Set the scaling of the output PDF. Only available with gen2a and gen2b.
-  -gen1, --pdf_gen_1    PDF rendering implementation with ``pycairo``.
-  -gen2a, --pdf_gen_2a  The first PDF rendering implementation with ``fpdf``.
-  -gen2b, --pdf_gen_2b  The second PDF rendering implementation with ``pycairo``. The default option.
-  -qa QUERIES_ANY, --query-any QUERIES_ANY
-                        Select the commits whose title OR description match ANY part of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have      
-                        leading or trailing whitespace.
-  -QA QUERIES_ALL, --query-all QUERIES_ALL
-                        Select the commits whose title OR description match ALL parts of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have     
-                        leading or trailing whitespace.
-  -rp RPATH, --repo-path RPATH
-                        Path to your repository directory. Set to "." by default.
-  -fc RNAME, --repo-from-clone RNAME
-                        Clone a repo into the working directory and generate the commits PDF from it automatically. Format: <repo name> (case insensitive).
-  -nnc NEWEST_N_COMMITS, --newest-n-commits NEWEST_N_COMMITS
-                        Select the newest n number amount of commits to include after filtering.
-  -onc OLDEST_N_COMMITS, --oldest-n-commits OLDEST_N_COMMITS
-                        Select the oldest n number amount of commits to include after filtering.
-```
-<br>
-
-## Usage
-**See usage info in the command-line**:
-Run `c2p -h`
-
-<br>**Simple usage**:
-```
-c2p -O tomasvana10
-```
-_Explanation_: Run the commmits2pdf cli tool in the current directory (assuming it is a repository). The owner name must be provided in all cases.
-
-<br>**Advanced usage example #1**:
-```
-c2p -O tomasvana10 -rp ../seriescalculator_sdd -a person@email.com,other_person@gmail.com -s 2024-11-30 -e 2024-12-30 -b other_branch -d
-```
-_Explanation_: 
-1. Override the default repository path with the ``seriescalculator_sdd`` folder in the parent directory
-2. Look for specific commit emails (separated by commas)
-3. Search for commits from the -s date until the -e date
-4. Search for commits only made to `other_branch`
-5. Toggle dark mode for the PDF output
-
-<br>**Advanced usage example #2**
-```
-c2p -O tomasvana10 -nnc 10 -r
-```
-_Explanation_: Display the newest ten commits (after any filtering) in reverse order (newest to oldest instead of the default, which is oldest to newest).
-
-<br>**Advanced usage example #3**
-```
-c2p -O tomasvana10 -qa "javascript,test " -onc 5 -po -o ..
-```
-_Explanation_: 
-1. Display the 5 oldest commits after querying the current repository's commits for either "javascript" OR "test "
-2. Prevent the PDF directory from being automatically opened.
-3. Output the PDF to the parent directory (`..`)
-
-**NOTE**: -qa selects commits that include **any** query criteria in the title **OR** description, while -QA selects commits that include **ALL** query criteria in the title or description.
-
-<br>**Advanced usage example #4**
-```
-c2p -O tomasvana10 -QA "dev ,testing" -gen2a -sc 0.8
-```
-_Explanation_:
-1. Query the repo for both "dev " AND "testing"
-2. Use the `gen2a` PDF renderer to visualise the PDF
-3. Set the scaling of the PDF output to 0.8
-
-**NOTE**: Scaling (`-sc`) is only available when using `gen2a` or `gen2b`. `gen2b` is default.
-
-<br>**Clone the repo you want to document on-demand**:
-```
-c2p -O tomasvana10 -fc some_repo_name
-```
-_Explanation_: Create the repo you have specified and make the PDF. This repo is always cloned into the current working directory.
-<br><br>
-## PDF Generation implementations
-### pycairo (gen1)
-- **Positives**
-  - Fast
-- **Negatives**
-  - Not scalable
-  - Occasional rendering inconsistencies
-  - Not as good looking at the other generation implementations
-  - No hyperlinks
-- **Sample use case**: You want to quickly generate a large amount of commits and do not care about the sizing of the PDF.
-
-### fpdf (gen2a)
-- **Positives**
-  - Fast
-  - Scalable
-  - Detailed title page
-  - Sleek design
-  - Hyperlinks
-  - Saves metadata
-- **Negatives**
-  - Inconsistent page breaks in some cases due to the difficulty of precalculating the height of a commit, a general limitation with this generation method.
-- **Sample use case**: You do not mind if your PDF has occasionally inconsistent spacing, but you want a nice design that can be generated very fast.
-
-### fpdf (gen2b - Default)
-- **Positives**
-   - Same as gen2a but with consistent page breaks that do not leave any whitespace.
-- **Negatives**
-  - Slow when generating large 
-- **Sample use case**: You want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed.
-<br><br>
-## Gallery
-**gen1 title page**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
-
-**gen2 title page in dark mode**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
-
-**gen2 commit page in dark mode**<br>
-<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/a9fd3341-e661-4355-91e7-0dc3182e7239" alt="gen2 pdf commit page dark" width=561.12>
-
-
+![Licence](https://img.shields.io/badge/licence-MIT-green?style=flat?logo=licence)
+[![PyPI version](https://img.shields.io/pypi/v/commits2pdf?style=flat-square)](https://pypi.org/project/commits2pdf/)
+[![Publish to PyPI.org](https://github.com/tomasvana10/commits2pdf/actions/workflows/publish.yml/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/publish.yml)
+[![Release)](https://img.shields.io/github/v/release/tomasvana10/commits2pdf?logo=github)](https://github.com/tomasvana10/commits2pdf/releases/latest)
+[![Issues](https://img.shields.io/github/issues-raw/tomasvana10/commits2pdf.svg?maxAge=25000)](https://github.com/tomasvana10/commits2pdf/issues)
+[![CodeQL](https://github.com/tomasvana10/commits2pdf/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/github-code-scanning/codeql)
+[![Tests](https://github.com/tomasvana10/commits2pdf/actions/workflows/tox-tests.yml/badge.svg)](https://github.com/tomasvana10/commits2pdf/actions/workflows/tox-tests.yml)
+
+# commits2pdf
+Visualise a GitHub repository's commit history in PDF form via the command-line
+<br><br>
+## Dependencies
+`pycairo`<br>
+`GitPython`<br>
+`fpdf`
+<br><br>
+## Installation
+**Requires [pip](https://pip.pypa.io/en/stable/installation/)**
+
+Make a virtual environment (recommended)
+```
+pip install virtualenv OR pip3 install virtualenv
+python -m venv venv OR python3 -m venv venv
+ON MACOS/UNIX: source venv/bin/activate
+ON WINDOWS: venv\scripts\activate
+```
+
+Install the package in your system directory/virtual environment:
+```
+pip install -U commits2pdf OR pip3 install -U commits2pdf
+```
+OR, install the package in your home directory (good if you aren't using a virtual environment):
+```
+pip install --user -U commits2pdf
+```
+
+
+**If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)**
+<br><br>
+## Command-line parameters
+```
+positional arguments:
+  owner                 The owner of the git repository. Required.
+
+options:
+  -h, --help            show this help message and exit
+  -o OUTPUT, --output OUTPUT
+                        Directory path to your PDF output. Set to "." by default. Will be created if it does not exist. Example: -o ./work/my_pdfs
+  -b BRANCH, --branch BRANCH
+                        The repository branch. Set to "main" by default.
+  -a AUTHORS, --authors AUTHORS
+                        Filter commits from a comma-separated list of authors. Format: <author@email.com> OR <author1@email.com,author2@email.com> etc. Set to all authors by
+                        default.
+  -s START_DATE, --start_date START_DATE
+                        Filter from start date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
+  -e END_DATE, --end_date END_DATE
+                        Filter to end date of commits. Format: YYYY-mm-dd or YYYY-m-d. Example: 2023-12-05
+  -r, --reverse         Output the commits from newest to oldest. Set to oldest to newest by default
+  -d, --dark            Toggle dark mode for the output PDF. Set to "light" by default.
+  -po, --prevent-open   Prevent commits2pdf from automatically opening the directory the PDF was created in.
+  -sc SCALING, --scaling SCALING
+                        Set the scaling of the output PDF. Only available with gen2a and gen2b.
+  -gen1, --pdf_gen_1    PDF rendering implementation with ``pycairo``.
+  -gen2a, --pdf_gen_2a  The first PDF rendering implementation with ``fpdf``.
+  -gen2b, --pdf_gen_2b  The second PDF rendering implementation with ``pycairo``. The default option.
+  -qa QUERIES_ANY, --query-any QUERIES_ANY
+                        Select the commits whose title OR description match ANY part of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have leading or    
+                        trailing whitespace.
+  -QA QUERIES_ALL, --query-all QUERIES_ALL
+                        Select the commits whose title OR description match ALL parts of your query. Format: "<query1>" OR "<query1,query2>" etc. Note: queries can have leading or   
+                        trailing whitespace.
+  -rp RPATH, --repo-path RPATH
+                        Path to your repository directory. Set to "." by default.
+  -fc RNAME, --repo-from-clone RNAME
+                        Clone a repo into the working directory and generate the commits PDF from it automatically. Format: <repo name> (case insensitive).
+  -nnc NEWEST_N_COMMITS, --newest-n-commits NEWEST_N_COMMITS
+                        Select the newest n number amount of commits to include after filtering.
+  -onc OLDEST_N_COMMITS, --oldest-n-commits OLDEST_N_COMMITS
+                        Select the oldest n number amount of commits to include after filtering.
+```
+<br>
+
+## Usage
+<br>**Simple usage - what you will be using the most**:
+```
+c2p tomasvana10
+```
+_Explanation_: Run the CLI tool in the current directory (assuming it is a Git repository). The owner name must be provided in all cases.
+
+<br>**Advanced usage example #1**:
+```
+c2p tomasvana10 -rp ../seriescalculator_sdd -a person@email.com,other_person@gmail.com -s 2024-11-30 -e 2024-12-30 -b other_branch -d
+```
+_Explanation_: 
+1. Override the default repository path (``-rp ..\seriescalculator_sdd``) with a folder in the parent directory.
+2. Look for specific commit emails (separated by commas)
+3. Search for commits from the -s date until the -e date
+4. Search for commits only made to `other_branch`
+5. Toggle dark mode for the PDF output
+
+<br>**Advanced usage example #2**
+```
+c2p tomasvana10 -nnc 10 -r
+```
+_Explanation_: Display the newest ten commits (after any filtering) in reverse order (newest to oldest instead of the default, which is oldest to newest).
+
+<br>**Advanced usage example #3**
+```
+c2p tomasvana10 -qa "javascript,test " -onc 5 -po -o ..
+```
+_Explanation_: 
+1. Display the 5 oldest commits after querying the current repository's commits for either "javascript" OR "test "
+2. Prevent the PDF directory from being automatically opened.
+3. Output the PDF to the parent directory (`..`)
+
+**NOTE**: -qa selects commits that include **any** query criteria in the title **OR** description, while -QA selects commits that include **ALL** query criteria in the title or description.
+
+<br>**Advanced usage example #4**
+```
+c2p tomasvana10 -QA "dev ,testing" -gen2a -sc 0.8
+```
+_Explanation_:
+1. Query the repo for both "dev " AND "testing"
+2. Use the `gen2a` PDF renderer to visualise the PDF
+3. Set the scaling of the PDF output to 0.8
+
+**NOTE**: Scaling (`-sc`) is only available when using `gen2a` or `gen2b`. `gen2b` is default.
+
+<br>**Clone the repo you want to document on-demand**:
+```
+c2p tomasvana10 -fc some_repo_name
+```
+_Explanation_: Create the repo you have specified and make the PDF. This repo is always cloned into the current working directory.
+<br><br>
+## PDF Generation implementations
+### pycairo (gen1)
++ Fast
+- Looks like crap 
+- No hyperlinks, therefore the entire link to a commit's diff is displayed
+- Occasional bugs in rendering
+
+### fpdf (gen2a)
++ Fast
++ Can be scaled with the `-sc <float>` argument 
++ Sleek design
++ Information title page
++ Contains hyperlinks
++ Stores PDF metadata
+- Inconsistent page breaks, a general limitation with FPDF when trying to fit as many whole commits on a single page 
+
+### fpdf (gen2b - Default)
++ Same as gen2a but with perfectly accurate page breaking
+- Slow when generating large amounts of commits (generally, it is a good idea to switch to gen2a when drawing over 5000 commits)
+
+<br><br>
+## Gallery
+**gen1 title page**<br>
+<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
+
+**gen2 title page in dark mode**<br>
+<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
+
+**gen2 commit page in dark mode**<br>
+<img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/a9fd3341-e661-4355-91e7-0dc3182e7239" alt="gen2 pdf commit page dark" width=561.12>
```

### Comparing `commits2pdf-1.1.7/commits2pdf/commits.py` & `commits2pdf-1.1.8/commits2pdf/commits.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,262 +1,359 @@
-from os import path, listdir
-from datetime import datetime
-from shutil import rmtree
-from typing import List, Optional, Dict, Union
-
-from git import Repo, GitCommandError, InvalidGitRepositoryError
-
-from .logger import logger
-from .constants import (
-    REPO_ALREADY_EXISTS_WARNING, DETACHED_BRANCH_ERROR, 
-    BRANCH_ALREADY_EXISTS_WARNING, INVALID_REPO_ERROR, INVALID_REPO_ERROR_2,
-    FILTER_INFO, N_COMMITS_INFO, N_COMMITS_WARN, GATHERED_COMMITS_INFO, CODING
-)
-
-
-class Commits(object):
-    """Represents a filtered set of commits along with filter information."""
-    def __init__(self, **kwargs) -> None:
-        """Save filter and repo information from kwargs."""
-        self.err_flag: bool = False # Detected in ``cli.py`` to stop execution
-        
-        self.rpath: str = kwargs["rpath"]
-        self.owner: str = kwargs["owner"]
-        self.url: Optional[str] = kwargs["url"]
-        self.branch: Optional[str] = kwargs["branch"]
-        self.authors: Optional[List[str]] = kwargs["authors"]
-        self.start_date: Optional[datetime] = kwargs["start_date"]
-        self.end_date: Optional[datetime] = kwargs["end_date"]
-        self.reverse: Optional[bool] = kwargs["reverse"]
-        self.newest_n_commits: Optional[int] = kwargs["newest_n_commits"]
-        self.oldest_n_commits: Optional[int] = kwargs["oldest_n_commits"]
-        self.queries_any: Option[List[str]] = kwargs["queries_any"]
-        self.queries_all: Optional[List[str]] = kwargs["queries_all"]
-
-        self.r: Repo = self.get_repo()  
-        if isinstance(self.r, Repo): # Repo was successfully found, continue
-            self.init_repo_data()
-        elif self.r == "deltree": # Buffered deletion due to errors in
-                                  # ``get_repo``.
-            rmtree(self.rpath, ignore_errors=True)
-            self.err_flag = True
-        elif not self.r: # ``get_repo`` returned nothing, so the repo could not
-                         # be accessed
-            self.err_flag = True
-            
-    def init_repo_data(self) -> None:
-        """Find the repo name (preferrably from the remote), then sequentially
-        build the filtered commits from the commits of the repo.
-        """
-        if len(self.r.remotes) > 0: # Use remote name
-            self.rname = self.r.remotes.origin.url.split(".git")[0].split("/")[-1]
-        else: # No remote exists, just get the name of the directory
-            self.rname = path.basename(self.r.working_tree_dir.split("/")[-1])
-            
-        self.raw_commits: list[Repo.commit] = self.gather_commits()
-        self.commit_objects: list[Commit] = self.instantiate_commits()
-        self.filtered_commits: list[Commit] = self.filter_commits()
-
-    def get_repo(self) -> Union[Repo, str, None]: 
-        """Access a repo, or clone it and then access it. Complete with extensive
-        error handling, ensuring a high chance of the user's requests being
-        adequately processed.
-        """
-        if self.url: # User wants to clone a repo
-            if path.exists(self.rpath) and path.isdir(self.rpath): # Repo may exist
-                if path.exists(path.join(self.rpath, ".git")):  # .git exists
-                    logger.warn(REPO_ALREADY_EXISTS_WARNING)
-                    r = Repo(self.rpath) # Attempt to access repo
-                    if self.branch: # User is looking for specific branch
-                        try:
-                            b = r.active_branch
-                        except TypeError: # Branch is detached
-                            return logger.error(
-                                DETACHED_BRANCH_ERROR.format(self.branch))
-                        if not str(b) == str(self.branch): # Branch of existing 
-                                                           # repo is not the 
-                                                           # branch the user wants
-                            logger.warning(
-                                BRANCH_ALREADY_EXISTS_WARNING.format(self.branch, 
-                                                                     b))
-                            self.branch = b # Update the branch to the repo's 
-                                            # active branch
-                    return r # Repo was accessed with no problems
-
-                else: # .git does not exist, delete the existing folder and 
-                      # clone the repo
-                    rmtree(self.rpath, ignore_errors=True)
-                    try:
-                        r = Repo.clone_from(self.url, self.rpath, 
-                                            branch=self.branch, no_checkout=True)
-                    except GitCommandError as e:
-                        if "remote branch" in str(e).casefold(): # User entered 
-                                                                 # invalid branch
-                            r = Repo.clone_from(self.url, self.rpath, 
-                                                no_checkout=True)
-                            try:
-                                b = r.active_branch
-                            except TypeError:
-                                return logger.error(
-                                    DETACHED_BRANCH_ERROR.format(self.branch))
-                            logger.warning(
-                                BRANCH_ALREADY_EXISTS_WARNING.format(self.branch, 
-                                                                     b))
-                            self.branch = b # Update the branch to the repo's 
-                                            # active branch
-                        else: # Some other error occurred
-                            logger.error(INVALID_REPO_ERROR.format(self.url))
-                            return "deltree"
-
-            else:  # Repo does not exist, just clone it
-                try:
-                    r = Repo.clone_from(self.url, self.rpath, 
-                                        branch=self.branch, no_checkout=True)
-                except GitCommandError as e:
-                    if "remote branch" in str(e).casefold():
-                        r = Repo.clone_from(self.url, self.rpath, 
-                                            no_checkout=True)
-                        try:
-                            b = r.active_branch
-                        except TypeError:
-                            return logger.error(
-                                DETACHED_BRANCH_ERROR.format(self.branch))
-                        logger.warning(
-                            BRANCH_ALREADY_EXISTS_WARNING.format(self.branch, 
-                                                                 b))
-                        self.branch = b
-                    else: # Some other error occurred
-                        logger.error(INVALID_REPO_ERROR.format(self.url))
-                        return "deltree"
-
-        else: # Just access the repo normally
-            try:
-                r = Repo(self.rpath)
-                if self.branch:
-                    try:
-                        b = r.active_branch
-                    except TypeError:
-                        return logger.error(
-                            DETACHED_BRANCH_ERROR.format(self.branch))
-                    if not str(b) == str(self.branch):  # Branch of repo is not 
-                                                        # the branch the user wants
-                        logger.warning(
-                            BRANCH_ALREADY_EXISTS_WARNING.format(self.branch, 
-                                                                 b))
-                        self.branch = b  # Update the branch to the repo's 
-                                         # active branch
-
-            except InvalidGitRepositoryError:
-                return logger.error(INVALID_REPO_ERROR_2)
-
-        return r
-
-    def gather_commits(self) -> List[Repo.commit]:
-        """Find all the commits that match the user's since, until and branch
-        specifications.
-        """
-        commits = list(
-            self.r.iter_commits( # If any of the params are NoneType, no prob!
-                since=self.start_date,
-                until=self.end_date,
-                rev=self.branch,
-            )
-        )
-        logger.info(GATHERED_COMMITS_INFO.format(len(commits)))
-        
-        return commits
-    
-    def instantiate_commits(self) -> List[Dict[str, str]]: 
-        """Instantiate all the filtered ``Repo.commit`` objects into my own
-        simple class that inherits from a dictionary.
-        """
-        commit_objects = []
-        for commit in self.raw_commits:
-            commit_objects.append(Commit(self.owner, self.rname, self.branch, 
-                                         commit))
-
-        return commit_objects
-
-    def filter_commits(self) -> List[dict]:
-        """Process the Commit objects based on user-specified criteria such as
-        authors and queries. 
-        """
-        filtered_commits = self.commit_objects
-        if self.queries_any or self.queries_all:
-            queries, query_func = (self.queries_any, any) if self.queries_any \
-                                  else (self.queries_all, all)
-            filtered_commits = [commit for commit in self.commit_objects \
-                                if query_func(q in commit["description"] \
-                                or q in commit["title"] for q in queries)]        
-            logger.info(FILTER_INFO.format(len(filtered_commits), 
-                                           len(self.commit_objects), "query"))
-        if self.authors:
-            prior_len = len(filtered_commits)
-            filtered_commits = [commit for commit in filtered_commits \
-                                if commit["author_email"] in self.authors]
-            logger.info(FILTER_INFO.format(len(filtered_commits), prior_len, 
-                                           "author_email"))
-            
-        if self.newest_n_commits:
-            if not self.newest_n_commits >= len(filtered_commits):
-                filtered_commits = filtered_commits[:self.newest_n_commits]
-                logger.info(N_COMMITS_INFO.format("newest", 
-                                                  self.newest_n_commits))
-            else:
-                logger.warn(N_COMMITS_WARN.format("Newest", 
-                                                  self.newest_n_commits,
-                                                  len(filtered_commits)))
-        elif self.oldest_n_commits:
-            if not self.oldest_n_commits >= len(filtered_commits):
-                filtered_commits = filtered_commits[-self.oldest_n_commits:]
-                logger.info(N_COMMITS_INFO.format("oldest", 
-                                                  self.oldest_n_commits,
-                                                  len(filtered_commits)))
-            else: 
-                logger.warn(N_COMMITS_WARN("Oldest", self.oldest_n_commits))
-
-        step = -1 if not self.reverse else 1
-        filtered_commits = filtered_commits[::step] 
-        
-        return filtered_commits
-
-class Commit(dict):
-    """A simple way of representing a commit as a dictionary."""
-    def __init__(self, 
-                 owner: str, 
-                 rname: str, 
-                 branch: str, 
-                 commit: Repo.commit):
-        """Assign commit data to the instance."""
-        self["rname"] = rname 
-        self["branch"] = branch
-        self["author_name"] = commit.author
-        self["author_email"] = commit.author.email
-        self["date"] = datetime.fromtimestamp(commit.committed_date)
-        self["hexsha_short"] = commit.hexsha[:7]
-        self["hexsha_long"] = commit.hexsha
-        self["diff_url"] = f"https://github.com/{owner}/{rname}/commit/{commit.hexsha}"
-
-        self["info"] = f"{self['hexsha_short']} | Branch: {self['branch']} | " \
-                       f"By {self['author_name']} ({self['author_email']}) | " \
-                       f"At {self['date'].strftime('%Y-%m-%d')}"
-        self["info"] = Commit._code(self["info"])
-         
-        # Extract the message from the title
-        msg = commit.message.split("\n")
-        self["title"] = Commit._code(msg[0])
-        self["description"] = Commit._code("\n".join(msg[1:])) if len(msg) > 1 else ""
-    
-    @staticmethod
-    def _code(text, coding=CODING):
-        return text.encode(CODING, "replace").decode(CODING)
-    
-    def __str__(self): 
-        """View the commit in the terminal."""
-        return \
-            "=============================\n" \
-            f"Repository: {self['rname']}\n" \
-            f"{self['info']}\n" \
-            f"{self['title']}\n" \
-            f"{self['description']}\n" \
-            f"View diff: {self['diff_url']}\n" \
-            "=============================\n"
+from datetime import datetime
+from os import path
+from shutil import rmtree
+from typing import Optional
+
+from git import (
+    GitCommandError,
+    InvalidGitRepositoryError,
+    NoSuchPathError,
+    Repo,
+)
+
+from .constants import (
+    CLONING_REPO_INFO,
+    CODING,
+    DETACHED_BRANCH_ERROR,
+    FILTER_INFO,
+    GATHERED_COMMITS_INFO,
+    INVALID_GIT_REPO_ERROR,
+    N_COMMITS_INFO,
+    N_COMMITS_WARNING,
+    NONEXISTING_BRANCH_WARNING,
+    NONEXISTING_OR_INVALID_REPO_ERROR,
+    NONEXISTING_REPO_ERROR,
+    REPO_ALREADY_EXISTS_WARNING,
+    UNEXPECTED_BUG_ERROR,
+)
+from .logger import logger
+
+
+class Commits(object):
+    """Represents a filtered set of commits along with filter information."""
+
+    def __init__(self, **kwargs) -> None:
+        """Save filter and repo information from kwargs."""
+        self.err_flag: bool = False  # Detected in ``cli.py`` to stop execution
+
+        self.rpath: str = kwargs["rpath"]
+        self.owner: str = kwargs["owner"]
+        self.url: Optional[str] = kwargs["url"]
+        self.branch: Optional[str] = kwargs["branch"]
+        self.authors: Optional[list[str]] = kwargs["authors"]
+        self.start_date: Optional[datetime] = kwargs["start_date"]
+        self.end_date: Optional[datetime] = kwargs["end_date"]
+        self.reverse: Optional[bool] = kwargs["reverse"]
+        self.newest_n_commits: Optional[int] = kwargs["newest_n_commits"]
+        self.oldest_n_commits: Optional[int] = kwargs["oldest_n_commits"]
+        self.queries_any: Optional[list[str]] = kwargs["queries_any"]
+        self.queries_all: Optional[list[str]] = kwargs["queries_all"]
+
+        self.r: Repo = self._get_repo()
+        if isinstance(self.r, Repo):  # Repo was successfully found, continue
+            self._init_repo_data()
+        elif self.r == "DELTREE":  # Perform buffered deletion due to errors in
+            # ``_get_repo``.
+            rmtree(self.rpath, ignore_errors=True)
+            self.err_flag = True
+        elif not self.r:  # ``_get_repo`` returned NoneType, so the repo could 
+                          # not be accessed
+            self.err_flag = True
+
+    def _init_repo_data(self) -> None:
+        """Find the repo name (preferrably from the remote), then
+        sequentially build the filtered commits from the commits of the
+        repo.
+        """
+        if len(self.r.remotes) > 0:  # Use remote name
+            self.rname = self.r.remotes.origin.url.split(".git")[0].split("/")[
+                -1
+            ]
+        else:  # No remote exists, just get the name of the directory
+            self.rname = path.basename(self.r.working_tree_dir.split("/")[-1])
+
+        self.raw_commits: list[Repo.commit] = self._gather_commits()
+        self.commit_objects: list[Commit] = self._instantiate_commits()
+        self.filtered_commits: list[Commit] = self._filter_commits()
+
+    def _get_repo(self) -> Repo | str | None:
+        """Access a repo, or clone it and then access it, and update
+        ``self.branch`` if necessary. Complete with extensive error handling,
+        ensuring a high chance of the user's requests being processed.
+        """
+        if self.url:  # User wants to clone a repo
+            if path.exists(self.rpath) and path.isdir(self.rpath):  # Repo may
+                                                                    # exist
+                if path.exists(path.join(self.rpath, ".git")):  # .git exists
+                    logger.warn(REPO_ALREADY_EXISTS_WARNING)
+                    try:
+                        r = Repo(self.rpath)  # Attempt to access repo
+                    except NoSuchPathError:
+                        return logger.error(NONEXISTING_REPO_ERROR)
+
+                    if self.branch:  # User is looking for specific branch
+                        try:
+                            b = r.active_branch
+                        except TypeError:  # Branch is detached
+                            return logger.error(
+                                DETACHED_BRANCH_ERROR.format(self.branch)
+                            )
+
+                        if not str(b) == str(
+                            self.branch
+                        ):  # Branch of existing repo is not the branch the user wants
+                            logger.warning(
+                                NONEXISTING_BRANCH_WARNING.format(
+                                    self.branch, b
+                                )
+                            )
+                            self.branch = b  # Update the branch to the repo's
+                                             # active branch
+
+                    return r  # Repo was accessed with no problems
+
+                else:  # .git does not exist, delete the existing folder and
+                       # clone the repo
+                    rmtree(self.rpath, ignore_errors=True)
+                    try:
+                        logger.info(CLONING_REPO_INFO)
+                        r = Repo.clone_from(
+                            self.url,
+                            self.rpath,
+                            branch=self.branch,
+                            no_checkout=True,
+                        )
+                    except GitCommandError as e:
+                        if (
+                            "remote branch" in str(e).casefold()
+                        ):  # User entered invalid branch
+                            logger.info(CLONING_REPO_INFO)
+                            r = Repo.clone_from(
+                                self.url, self.rpath, no_checkout=True
+                            )
+                            try:
+                                b = r.active_branch
+                            except TypeError:
+                                return logger.error(
+                                    DETACHED_BRANCH_ERROR.format(self.branch)
+                                )
+                            logger.warning(
+                                NONEXISTING_BRANCH_WARNING.format(
+                                    self.branch, b
+                                )
+                            )
+                            self.branch = b  # Update the branch to the repo's
+                                             # active branch
+                        else:  # Some other error occurred
+                            logger.error(
+                                NONEXISTING_OR_INVALID_REPO_ERROR.format(
+                                    self.url
+                                )
+                            )
+                            return "DELTREE"
+
+            else:  # Repo does not exist, just clone it
+                try:
+                    logger.info(CLONING_REPO_INFO)
+                    r = Repo.clone_from(
+                        self.url,
+                        self.rpath,
+                        branch=self.branch,
+                        no_checkout=True,
+                    )
+                except GitCommandError as e:
+                    if "remote branch" in str(e).casefold():
+                        logger.info(CLONING_REPO_INFO)
+                        r = Repo.clone_from(
+                            self.url, self.rpath, no_checkout=True
+                        )
+                        try:
+                            b = r.active_branch
+                        except TypeError:
+                            return logger.error(
+                                DETACHED_BRANCH_ERROR.format(self.branch)
+                            )
+                        logger.warning(
+                            NONEXISTING_BRANCH_WARNING.format(self.branch, b)
+                        )
+                        self.branch = b
+                    else:  # Some other error occurred
+                        logger.error(
+                            NONEXISTING_OR_INVALID_REPO_ERROR.format(self.url)
+                        )
+                        return "DELTREE"
+
+        else:  # Just access the repo normally
+            try:
+                r = Repo(self.rpath)
+                if self.branch:
+                    try:
+                        b = r.active_branch
+                    except TypeError:
+                        return logger.error(
+                            DETACHED_BRANCH_ERROR.format(self.branch)
+                        )
+                    if not str(b) == str(self.branch):  # Branch of repo is not
+                                                        # the branch the user wants
+                        logger.warning(
+                            NONEXISTING_BRANCH_WARNING.format(self.branch, b)
+                        )
+                        self.branch = b  # Update the branch to the repo's
+                                         # active branch
+
+            except InvalidGitRepositoryError:
+                return logger.error(INVALID_GIT_REPO_ERROR.format(self.rpath))
+            except NoSuchPathError:
+                return logger.error(NONEXISTING_REPO_ERROR)
+
+        return r
+
+    def _gather_commits(self) -> list[Repo.commit]:
+        """Find all the commits that match the user's since, until and branch
+        specifications.
+        """
+        try:
+            commits = list(
+                self.r.iter_commits(  # If any of the params are NoneType, no prob!
+                    since=self.start_date,
+                    until=self.end_date,
+                    rev=self.branch,
+                )
+            )
+        except Exception:
+            logger.error(UNEXPECTED_BUG_ERROR)
+            self.err_flag = True
+            exit(1)
+
+        logger.info(GATHERED_COMMITS_INFO.format(len(commits)))
+
+        return commits
+
+    def _instantiate_commits(self) -> list[dict[str, str]]:
+        """Instantiate all the filtered ``Repo.commit`` objects into my own
+        simple class that inherits from a dictionary.
+        """
+        commit_objects = []
+        for commit in self.raw_commits:
+            commit_objects.append(
+                Commit(self.owner, self.rname, self.branch, commit)
+            )
+
+        return commit_objects
+
+    def _filter_commits(self) -> list[dict[str, str]]:
+        """Process the Commit objects based on user-specified criteria such as
+        authors and queries.
+        """
+        filtered_commits = self.commit_objects
+        if self.queries_any or self.queries_all:
+            queries, query_func = (
+                (self.queries_any, any)
+                if self.queries_any
+                else (self.queries_all, all)
+            )
+            filtered_commits = [
+                commit
+                for commit in self.commit_objects
+                if query_func(
+                    q in commit["description"] or q in commit["title"]
+                    for q in queries
+                )
+            ]
+            logger.info(
+                FILTER_INFO.format(
+                    len(filtered_commits), len(self.commit_objects), "query"
+                )
+            )
+        if self.authors:
+            prior_len = len(filtered_commits)
+            filtered_commits = [
+                commit
+                for commit in filtered_commits
+                if commit["author_email"] in self.authors
+            ]
+            logger.info(
+                FILTER_INFO.format(
+                    len(filtered_commits), prior_len, "author_email"
+                )
+            )
+
+        if self.newest_n_commits:
+            if not self.newest_n_commits >= len(filtered_commits):
+                filtered_commits = filtered_commits[: self.newest_n_commits]
+                logger.info(
+                    N_COMMITS_INFO.format("newest", self.newest_n_commits)
+                )
+            else:
+                logger.warn(
+                    N_COMMITS_WARNING.format(
+                        "Newest", self.newest_n_commits, len(filtered_commits)
+                    )
+                )
+        elif self.oldest_n_commits:
+            if not self.oldest_n_commits >= len(filtered_commits):
+                filtered_commits = filtered_commits[-self.oldest_n_commits :]
+                logger.info(
+                    N_COMMITS_INFO.format(
+                        "oldest", self.oldest_n_commits, len(filtered_commits)
+                    )
+                )
+            else:
+                logger.warn(
+                    N_COMMITS_WARNING.format(
+                        "Oldest", self.oldest_n_commits, len(filtered_commits)
+                    )
+                )
+
+        step = -1 if not self.reverse else 1
+        filtered_commits = filtered_commits[::step]
+
+        return filtered_commits
+
+
+class Commit(dict):
+    """A simple way of representing a commit as a dictionary."""
+
+    def __init__(
+        self, owner: str, rname: str, branch: str, commit: Repo.commit
+    ) -> None:
+        """Assign commit data to the instance."""
+        self["rname"] = rname
+        self["branch"] = branch
+        self["author_name"] = commit.author
+        self["author_email"] = commit.author.email
+        self["date"] = datetime.fromtimestamp(commit.committed_date)
+        self["hexsha_short"] = commit.hexsha[:7]
+        self["hexsha_long"] = commit.hexsha
+        self["diff_url"] = (
+            f"https://github.com/{owner}/{rname}/commit/{commit.hexsha}"
+        )
+
+        self["info"] = (
+            f"{self['hexsha_short']} | Branch: {self['branch']} | "
+            f"By {self['author_name']} ({self['author_email']}) | "
+            f"At {self['date'].strftime('%Y-%m-%d')}"
+        )
+        self["info"] = Commit._code(self["info"])
+
+        # Extract the message from the title
+        msg = commit.message.split("\n")
+        self["title"] = Commit._code(msg[0])
+        self["description"] = (
+            Commit._code("\n".join(msg[1:])) if len(msg) > 1 else ""
+        )
+
+    @staticmethod
+    def _code(text: str, coding: str = CODING) -> str:
+        return text.encode(CODING, "replace").decode(CODING)
+
+    def __str__(self) -> str:
+        """View the commit in the terminal."""
+        return (
+            "=============================\n"
+            f"Repository: {self['rname']}\n"
+            f"{self['info']}\n"
+            f"{self['title']}\n"
+            f"{self['description']}\n"
+            f"View diff: {self['diff_url']}\n"
+            "=============================\n"
+        )
```

### Comparing `commits2pdf-1.1.7/commits2pdf/render_cairo.py` & `commits2pdf-1.1.8/commits2pdf/render_cairo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,212 @@
-from os import path
-from textwrap import wrap
-from time import time
-from datetime import datetime
-from typing import List, Tuple, Dict
-
-from cairo import (
-    PDFSurface, Context, FONT_SLANT_ITALIC, FONT_SLANT_NORMAL, 
-    FONT_WEIGHT_NORMAL, FONT_WEIGHT_BOLD
-)
-
-from .constants import WIDTH, HEIGHT, MARGIN
-
-
-class Cairo_PDF:
-    def __init__(self, 
-                 commits: object, 
-                 output: str, 
-                 filename: str, 
-                 appearance: Dict[str, Tuple[int]]
-                 ) -> None:
-        """Assign attributes for use across the instance and instantiate the
-        core parts of a pycairo PDF.
-        """
-        self._commits, self._output, self._filename, self._ap = \
-            commits, output, filename, appearance
-        self.timestamp = datetime.fromtimestamp(
-            int(time())).strftime('%Y-%m-%d %H:%M:%S')
-        
-        self._s = PDFSurface(path.join(output, filename), WIDTH, HEIGHT)
-        self._c = Context(self._s)
-        self.page: int = 1
-        self.y: int = MARGIN
-        
-        self._draw_bg()
-        self._draw_footer()
-        self._draw_title("Commit Report", self.y)
-        self.y += 30
-        self._draw_rname(commits.rname, self.y)
-        self.y += 40
-        
-        if len(self._commits.filtered_commits) > 0: self._draw_commits()
-        
-    def _draw_commits(self) -> None:
-        """Driver function to draw all the commits."""
-        for commit in self._commits.filtered_commits:
-            text = self._get_commit_text(commit)
-            height = sum(len(t) for t in text) * 14 + 50
-            if self.y + height + 25 > HEIGHT - MARGIN:
-                self._s.show_page()
-                self.page += 1
-                self.y = MARGIN
-                
-                self._draw_bg()
-                self._draw_footer()
-            
-            self.draw_commit(commit, self.y, *text)
-            self.y += height + 50
-        
-        self._s.finish() 
-
-    def _set_font(self, 
-                  t: str, 
-                  font: str = "Arial"
-                  ) -> None:
-        """Set the font face, consisting of the family, slant and weight."""
-        if t == "n":
-            self._c.select_font_face(font, FONT_SLANT_NORMAL, 
-                                     FONT_WEIGHT_NORMAL)
-        elif t == "b":
-            self._c.select_font_face(font, FONT_SLANT_NORMAL, 
-                                     FONT_WEIGHT_BOLD)
-        elif t == "i":
-            self._c.select_font_face(font, FONT_SLANT_ITALIC, 
-                                     FONT_WEIGHT_NORMAL)
-
-    def _draw_bg(self) -> None:
-        """Draw the page background."""
-        self._c.set_source_rgb(*self._ap["background"])
-        self._c.rectangle(0, 0, WIDTH, HEIGHT)
-        self._c.fill()
-
-    def _draw_title(self, 
-                    text: str, 
-                    y: int
-                    ) -> None:
-        """Draw the "Commits Report" title for the first page."""
-        self._c.set_source_rgb(*self._ap["text"]) 
-        self._set_font("b")
-        self._c.set_font_size(24)
-        self._c.move_to(MARGIN, y)
-        self._c.show_text(text)
-
-    def _draw_footer(self) -> None:
-        """Draw the footer for the current page."""
-        self._c.set_source_rgb(*self._ap["text"]) 
-        self._set_font("n")
-        self._c.set_font_size(10)
-        self._c.move_to(MARGIN, HEIGHT - MARGIN)
-        self._c.show_text(f"Page {self.page}")
-        self._set_font("i")
-        self._c.move_to(MARGIN, HEIGHT - MARGIN + 20)
-        self._c.show_text(f"Generated by commits2pdf on {self.timestamp}")
-
-    def _draw_rname(self, 
-                    rname: str, 
-                    y: int
-                    ) -> None:
-        """Draw the repository name."""
-        w_rname: List[str] = wrap(f"Repository: {rname}", width=(WIDTH 
-                                                                 - MARGIN 
-                                                                 * 2) // 8)
-        self._draw_wrapped_text(w_rname, y, 18, "b")
-
-    def _get_commit_text(self, 
-                         commit: object
-                         ) -> Tuple[List[str]]:
-        """Get the commit text for a commit and wrap it with a bunch of magic
-        numbers.
-        """
-        info: List[str] = wrap(commit["info"], width=(WIDTH - MARGIN * 2) 
-                                                      // 6.5)
-        title: List[str] = wrap(commit["title"], width=(WIDTH - MARGIN * 2) 
-                                                        // 8)
-        diff_url: List[str] = wrap(commit["diff_url"], width=(WIDTH - MARGIN 
-                                                              * 2) // 5)
-        
-        desc_lines: List[str] = commit["description"].split("\n")
-        desc = []
-        for line in desc_lines:
-            lines = wrap(line, width=(WIDTH - MARGIN * 2) // 5.075)
-            desc.extend(lines)
-            if len(lines) > 1:
-                desc.append("")  
-
-        return info, title, desc, diff_url
-
-    def _draw_wrapped_text(self, 
-                           lines: List[str], 
-                           y: int, 
-                           font_size: int, 
-                           font_type: str, 
-                           font_family: str = "Arial", 
-                           rgb: str = "text"
-                           ) -> int:
-        """Draw the wrapped text for a commit component line by line."""
-        self._c.set_source_rgb(*self._ap[rgb])
-        self._c.set_font_size(font_size)
-        self._set_font(font_type, font=font_family)
-        this_y: int = y
-        for line in lines:
-            self._c.move_to(MARGIN, this_y)
-            self._c.show_text(line)
-            this_y += 15
-        
-        return this_y + 15
-
-    def draw_commit(self, 
-                    commit: object, 
-                    y: int, 
-                    *args: Tuple[List[str]]
-                    ) -> None:
-        """Driver function for its own driver function idk."""
-        new_y = self._draw_wrapped_text(args[0], y, 11, "n", 
-                                        font_family="Courier New") # Info
-        new_y = self._draw_wrapped_text(args[1], new_y, 16, "b") # Commit Title
-        new_y = self._draw_wrapped_text(args[2], new_y, 11, "n") # Description
-        new_y = self._draw_wrapped_text(args[3], new_y, 11, "n", 
-                                        rgb="diff_url") # Diff Url
-        self._draw_divider(new_y) # Horizontal Divider
-    
-    def _draw_divider(self, 
-                      y: int
-                      ) -> None:
-        """Draw the horizontal divider between commits which is only centered 
-        around half the time for some reason.
-        """
-        self._c.set_source_rgb(*self._ap["text"])  
-        self._c.set_line_width(1)  
-        self._c.move_to(MARGIN, y) 
-        self._c.line_to(WIDTH - MARGIN, y)  
-        self._c.stroke() 
+from datetime import datetime
+from os import path
+from textwrap import wrap
+from time import time
+
+from cairo import (
+    FONT_SLANT_ITALIC,
+    FONT_SLANT_NORMAL,
+    FONT_WEIGHT_BOLD,
+    FONT_WEIGHT_NORMAL,
+    Context,
+    PDFSurface,
+)
+from progressbar import ETA, Bar, Percentage, ProgressBar
+
+from .constants import (
+    GENERATING_PDF_INFO,
+    HEIGHT,
+    MARGIN,
+    WIDTH,
+    WRITING_PDF_INFO,
+)
+from .logger import logger
+
+
+class Cairo_PDF:
+    def __init__(
+        self,
+        commits: object,
+        output: str,
+        filename: str,
+        appearance: dict[str, tuple[int]],
+    ) -> None:
+        """Assign attributes for use across the instance and instantiate the
+        core parts of a pycairo PDF.
+        """
+        self._commits, self._output, self._filename, self._ap = (
+            commits,
+            output,
+            filename,
+            appearance,
+        )
+        self.timestamp = datetime.fromtimestamp(int(time())).strftime(
+            "%Y-%m-%d %H:%M:%S"
+        )
+        # Keep track of generation progress for the user
+        self._progress = ProgressBar(
+            maxval=len(self._commits.filtered_commits),
+            widgets=[Percentage(), Bar(), ETA()],
+        )
+
+        self._s = PDFSurface(path.join(output, filename), WIDTH, HEIGHT)
+        self._c = Context(self._s)
+        self.page: int = 1
+        self.y: int = MARGIN
+
+        self._draw_bg()
+        self._draw_footer()
+        self._draw_title("Commit Report", self.y)
+        self.y += 30
+        self._draw_rname(commits.rname, self.y)
+        self.y += 40
+
+        if len(self._commits.filtered_commits) > 0:
+            logger.info(GENERATING_PDF_INFO)
+            self._draw_commits()
+            logger.info(
+                WRITING_PDF_INFO.format(
+                    self._output + " ..."
+                    if self._output != "."
+                    else "your current directory..."
+                )
+            )
+            self._s.finish()
+
+    def _draw_commits(self) -> None:
+        """Driver function to draw all the commits."""
+        counter: int = 0
+        self._progress.start()
+        for commit in self._commits.filtered_commits:
+            text = self._get_commit_text(commit)
+            height = sum(len(t) for t in text) * 14 + 50
+            if self.y + height + 25 > HEIGHT - MARGIN:
+                self._s.show_page()
+                self.page += 1
+                self.y = MARGIN
+
+                self._draw_bg()
+                self._draw_footer()
+
+            self.draw_commit(commit, self.y, *text)
+            counter += 1
+            self._progress.update(counter)
+            self.y += height + 50
+
+        self._progress.finish()
+
+    def _set_font(self, t: str, font: str = "Arial") -> None:
+        """Set the font face, consisting of the family, slant and weight."""
+        if t == "n":
+            self._c.select_font_face(
+                font, FONT_SLANT_NORMAL, FONT_WEIGHT_NORMAL
+            )
+        elif t == "b":
+            self._c.select_font_face(font, FONT_SLANT_NORMAL, FONT_WEIGHT_BOLD)
+        elif t == "i":
+            self._c.select_font_face(
+                font, FONT_SLANT_ITALIC, FONT_WEIGHT_NORMAL
+            )
+
+    def _draw_bg(self) -> None:
+        """Draw the page background."""
+        self._c.set_source_rgb(*self._ap["background"])
+        self._c.rectangle(0, 0, WIDTH, HEIGHT)
+        self._c.fill()
+
+    def _draw_title(self, text: str, y: int) -> None:
+        """Draw the "Commits Report" title for the first page."""
+        self._c.set_source_rgb(*self._ap["text"])
+        self._set_font("b")
+        self._c.set_font_size(24)
+        self._c.move_to(MARGIN, y)
+        self._c.show_text(text)
+
+    def _draw_footer(self) -> None:
+        """Draw the footer for the current page."""
+        self._c.set_source_rgb(*self._ap["text"])
+        self._set_font("n")
+        self._c.set_font_size(10)
+        self._c.move_to(MARGIN, HEIGHT - MARGIN)
+        self._c.show_text(f"Page {self.page}")
+        self._set_font("i")
+        self._c.move_to(MARGIN, HEIGHT - MARGIN + 20)
+        self._c.show_text(f"Generated by commits2pdf on {self.timestamp}")
+
+    def _draw_rname(self, rname: str, y: int) -> None:
+        """Draw the repository name."""
+        w_rname: list[str] = wrap(
+            f"Repository: {rname}", width=(WIDTH - MARGIN * 2) // 8
+        )
+        self._draw_wrapped_text(w_rname, y, 18, "b")
+
+    def _get_commit_text(self, commit: object) -> tuple[list[str]]:
+        """Get the commit text for a commit and wrap it with a bunch of magic
+        numbers.
+        """
+        info: list[str] = wrap(
+            commit["info"], width=(WIDTH - MARGIN * 2) // 6.5
+        )
+        title: list[str] = wrap(
+            commit["title"], width=(WIDTH - MARGIN * 2) // 8
+        )
+        diff_url: list[str] = wrap(
+            commit["diff_url"], width=(WIDTH - MARGIN * 2) // 5
+        )
+
+        desc_lines: list[str] = commit["description"].split("\n")
+        desc = []
+        for line in desc_lines:
+            lines = wrap(line, width=(WIDTH - MARGIN * 2) // 5)
+            desc.extend(lines)
+            if len(lines) > 1:
+                desc.append("")
+
+        return info, title, desc, diff_url
+
+    def _draw_wrapped_text(
+        self,
+        lines: list[str],
+        y: int,
+        font_size: int,
+        font_type: str,
+        font_family: str = "Arial",
+        rgb: str = "text",
+    ) -> int:
+        """Draw the wrapped text for a commit component line by line."""
+        self._c.set_source_rgb(*self._ap[rgb])
+        self._c.set_font_size(font_size)
+        self._set_font(font_type, font=font_family)
+        this_y: int = y
+        for line in lines:
+            self._c.move_to(MARGIN, this_y)
+            self._c.show_text(line)
+            this_y += 15
+
+        return this_y + 15
+
+    def draw_commit(
+        self, commit: object, y: int, *args: tuple[list[str]]
+    ) -> None:
+        """Driver function for its own driver function idk."""
+        new_y = self._draw_wrapped_text(
+            args[0], y, 11, "n", font_family="Courier New"
+        )  # Info
+        new_y = self._draw_wrapped_text(
+            args[1], new_y, 16, "b"
+        )  # Commit Title
+        new_y = self._draw_wrapped_text(args[2], new_y, 11, "n")  # Description
+        new_y = self._draw_wrapped_text(
+            args[3], new_y, 11, "n", rgb="diff_url"
+        )  # Diff Url
+        self._draw_divider(new_y)  # Horizontal Divider
+
+    def _draw_divider(self, y: int) -> None:
+        """Draw the horizontal divider between commits which is only centered
+        around half the time for some reason.
+        """
+        self._c.set_source_rgb(*self._ap["text"])
+        self._c.set_line_width(1)
+        self._c.move_to(MARGIN, y)
+        self._c.line_to(WIDTH - MARGIN, y)
+        self._c.stroke()
```

