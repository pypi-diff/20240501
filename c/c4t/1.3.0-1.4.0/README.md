# Comparing `tmp/c4t-1.3.0.tar.gz` & `tmp/c4t-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4t-1.3.0.tar", last modified: Mon Apr 29 09:45:29 2024, max compression
+gzip compressed data, was "c4t-1.4.0.tar", last modified: Wed May  1 00:04:31 2024, max compression
```

## Comparing `c4t-1.3.0.tar` & `c4t-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.426590 c4t-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 09:45:23.000000 c4t-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 09:45:29.426590 c4t-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-29 09:45:23.000000 c4t-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-29 09:45:23.000000 c4t-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:45:29.426590 c4t-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 09:45:23.000000 c4t-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/src/c4t/
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-04-29 09:45:23.000000 c4t-1.3.0/src/c4t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-29 09:45:23.000000 c4t-1.3.0/src/c4t/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/src/c4t.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-29 09:45:23.000000 c4t-1.3.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.285895 c4t-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 00:04:25.000000 c4t-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-01 00:04:31.281895 c4t-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-01 00:04:25.000000 c4t-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-01 00:04:25.000000 c4t-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:04:31.285895 c4t-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-01 00:04:25.000000 c4t-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.277896 c4t-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.277896 c4t-1.4.0/src/c4t/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-01 00:04:25.000000 c4t-1.4.0/src/c4t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-01 00:04:25.000000 c4t-1.4.0/src/c4t/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.281895 c4t-1.4.0/src/c4t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.281895 c4t-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-01 00:04:25.000000 c4t-1.4.0/tests/tests.py
```

### Comparing `c4t-1.3.0/LICENSE` & `c4t-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `c4t-1.3.0/PKG-INFO` & `c4t-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.3.0
+Version: 1.4.0
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -41,15 +41,15 @@
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 [![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.3.0
+# c4t: Chrome for Testing - v1.4.0
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 
@@ -123,17 +123,16 @@
 
 ```bash
 Python 3.8.10 (default, May 26 2023, 14:05:08) 
 [GCC 9.4.0] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import c4t
 >>> assets = c4t.Assets()
-Create "assets" directory.
 >>> assets.install()
-Create directory ./assets/117.0.5938.62
+Create directory ${HOME}/.c4t-assets/124.0.6367.91
 Downloading chrome-linux64.zip.
 100% [......................................................................] 146689409 / 146689409
 
 Downloading chromedriver-linux64.zip.
 100% [..........................................................................] 7508443 / 7508443
 
 Unzipping chrome-linux64.zip
@@ -166,26 +165,66 @@
 ```bash
 (venv) $ c4t install --help
 ```
 
 #### Install the default, the latest stable version
 
 ```bash
+# By default assets are installed in ${HOME}/.c4t-assets
+# To use a different path, set the C4T_PATH_TO_ASSETS environment variable.
+# e.g.: export C4T_PATH_TO_ASSETS=<path>
+# Add this export to your .bashrc so the path is set for every bash session.
 (venv) $ c4t install
 ```
 
 #### Install a specific version
 
 ```bash
 (venv) $ c4t install --version 116.0.5794.0
 ```
 
 #### Show the currently active version
 
 ```bash
 (venv) $ c4t --active
+Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
 ```
 
+#### Show installation path of assets
+
+```bash
+(venv) $ c4t path
+Path to assets: /home/p4irin/.c4t-assets
+```
+
+#### Show a list of installed versions
+
+```bash
+(venv) $ c4t list
+1 - 124.0.6367.91
+2 - 116.0.5794.0
+```
+
+#### Switch active version
+
+```bash
+(venv) $ c4t switch
+1 - 124.0.6367.91
+2 - 116.0.5794.0
+Select a version by number: 2
+Creating symlink to chrome version 116.0.5794.0
+Creating symlink to chromedriver version 116.0.5794.0
+Active version is now: 116.0.5794.0
+```
+
+### Common workflow
+
+1. Install one or more versions of Chrome for testing assets
+1. Set/switch the active version
+1. Run your Selenium Webdriver tests with the active version of Chrome for testing
+
+This allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
+
 ## Reference
 
 - [Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 - [GitHub](https://github.com/GoogleChromeLabs/chrome-for-testing)
```

### Comparing `c4t-1.3.0/README.md` & `c4t-1.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 [![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.3.0
+# c4t: Chrome for Testing - v1.4.0
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 
@@ -83,17 +83,16 @@
 
 ```bash
 Python 3.8.10 (default, May 26 2023, 14:05:08) 
 [GCC 9.4.0] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import c4t
 >>> assets = c4t.Assets()
-Create "assets" directory.
 >>> assets.install()
-Create directory ./assets/117.0.5938.62
+Create directory ${HOME}/.c4t-assets/124.0.6367.91
 Downloading chrome-linux64.zip.
 100% [......................................................................] 146689409 / 146689409
 
 Downloading chromedriver-linux64.zip.
 100% [..........................................................................] 7508443 / 7508443
 
 Unzipping chrome-linux64.zip
@@ -126,26 +125,66 @@
 ```bash
 (venv) $ c4t install --help
 ```
 
 #### Install the default, the latest stable version
 
 ```bash
+# By default assets are installed in ${HOME}/.c4t-assets
+# To use a different path, set the C4T_PATH_TO_ASSETS environment variable.
+# e.g.: export C4T_PATH_TO_ASSETS=<path>
+# Add this export to your .bashrc so the path is set for every bash session.
 (venv) $ c4t install
 ```
 
 #### Install a specific version
 
 ```bash
 (venv) $ c4t install --version 116.0.5794.0
 ```
 
 #### Show the currently active version
 
 ```bash
 (venv) $ c4t --active
+Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
 ```
 
+#### Show installation path of assets
+
+```bash
+(venv) $ c4t path
+Path to assets: /home/p4irin/.c4t-assets
+```
+
+#### Show a list of installed versions
+
+```bash
+(venv) $ c4t list
+1 - 124.0.6367.91
+2 - 116.0.5794.0
+```
+
+#### Switch active version
+
+```bash
+(venv) $ c4t switch
+1 - 124.0.6367.91
+2 - 116.0.5794.0
+Select a version by number: 2
+Creating symlink to chrome version 116.0.5794.0
+Creating symlink to chromedriver version 116.0.5794.0
+Active version is now: 116.0.5794.0
+```
+
+### Common workflow
+
+1. Install one or more versions of Chrome for testing assets
+1. Set/switch the active version
+1. Run your Selenium Webdriver tests with the active version of Chrome for testing
+
+This allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
+
 ## Reference
 
 - [Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 - [GitHub](https://github.com/GoogleChromeLabs/chrome-for-testing)
```

### Comparing `c4t-1.3.0/pyproject.toml` & `c4t-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c4t"
-version = "1.3.0"
+version = "1.4.0"
 authors = [
   { name="p4irin", email="139928764+p4irin@users.noreply.github.com" },
 ]
 description = "Install Chrome for Testing assets."
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -65,15 +65,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `c4t-1.3.0/setup.py` & `c4t-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `c4t-1.3.0/src/c4t/__init__.py` & `c4t-1.4.0/src/c4t/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Install 'Chrome for Testing' assets from the stable channel.
 
 By default, if none specified, the latest version of assets, compatible
 binaries of 'Chrome for Testing' and chromedriver, are installed. Different
-versions of assets will be installed in their own './assets/<version>'
-directory relative to the current working directory. Once a version is
+versions of assets will be installed in their own
+'${HOME}/.c4t-assets/<version>' directory. Once a version is
 successfully installed it will be the 'active' version by symlinking
-'./assets/chrome' and './assets/chromedriver' to the last installed version of
-assets in './assets/<version>/chrome-linux64/chrome' and
-'./assets/<version>/chromedriver-linux64/chromedriver' respectively.
+'${HOME}/.c4t-assets/chrome' and '${HOME}/.c4t-assets/chromedriver'
+to the last installed version of
+assets in '${HOME}/.c4t-assets/<version>/chrome-linux64/chrome' and
+'${HOME}/.c4t-assets/<version>/chromedriver-linux64/chromedriver' respectively.
 Installing the 'active' version of assets again will not touch the installation
 of that version. The same goes for installing a previously installed version
-except that it will change the symlinks in './assets/' to the assets of that
-version, effectively making that version 'active'.
+except that it will change the symlinks in '${HOME}/.c4t-assets/' to the assets
+of that version, effectively making that version 'active'.
 
 N.B: Currently installs assets for linux64 platform only
 
 usage:
 
     import c4t
     from selenium.webdriver import ChromeOptions, ChromeService, Chrome
@@ -32,26 +33,26 @@
     browser.close()
     browser.quit()
 """
 
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 
 
 import requests
 import os
 import json
 import wget
 import zipfile
 from typing import Literal, List, Union
 
 
-_default_path_to_assets = './assets'
+_default_path_to_assets = f'{os.environ["HOME"]}/.c4t-assets'
 _path_to_assets = os.getenv(
     'C4T_PATH_TO_ASSETS', _default_path_to_assets
 )
 
 
 class _Location:
     """Specify the location/path to the assets' binaries.
@@ -388,7 +389,16 @@
         self._create_symlink(
             to_binary='chromedriver',
             version=version,
             for_platform='linux64'
         )
 
         print(self._successful_installation_message.format(version=version))
+
+    @property
+    def path(self) -> str:
+        return _path_to_assets
+    
+    def switch(self, to_version: str) -> None:
+        self._create_symlink(to_binary='chrome', version=to_version)
+        self._create_symlink(to_binary='chromedriver', version=to_version)
+        print(f'Active version is now: {to_version}')
```

### Comparing `c4t-1.3.0/src/c4t.egg-info/PKG-INFO` & `c4t-1.4.0/src/c4t.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.3.0
+Version: 1.4.0
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -41,15 +41,15 @@
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 [![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.3.0
+# c4t: Chrome for Testing - v1.4.0
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 
@@ -123,17 +123,16 @@
 
 ```bash
 Python 3.8.10 (default, May 26 2023, 14:05:08) 
 [GCC 9.4.0] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import c4t
 >>> assets = c4t.Assets()
-Create "assets" directory.
 >>> assets.install()
-Create directory ./assets/117.0.5938.62
+Create directory ${HOME}/.c4t-assets/124.0.6367.91
 Downloading chrome-linux64.zip.
 100% [......................................................................] 146689409 / 146689409
 
 Downloading chromedriver-linux64.zip.
 100% [..........................................................................] 7508443 / 7508443
 
 Unzipping chrome-linux64.zip
@@ -166,26 +165,66 @@
 ```bash
 (venv) $ c4t install --help
 ```
 
 #### Install the default, the latest stable version
 
 ```bash
+# By default assets are installed in ${HOME}/.c4t-assets
+# To use a different path, set the C4T_PATH_TO_ASSETS environment variable.
+# e.g.: export C4T_PATH_TO_ASSETS=<path>
+# Add this export to your .bashrc so the path is set for every bash session.
 (venv) $ c4t install
 ```
 
 #### Install a specific version
 
 ```bash
 (venv) $ c4t install --version 116.0.5794.0
 ```
 
 #### Show the currently active version
 
 ```bash
 (venv) $ c4t --active
+Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
 ```
 
+#### Show installation path of assets
+
+```bash
+(venv) $ c4t path
+Path to assets: /home/p4irin/.c4t-assets
+```
+
+#### Show a list of installed versions
+
+```bash
+(venv) $ c4t list
+1 - 124.0.6367.91
+2 - 116.0.5794.0
+```
+
+#### Switch active version
+
+```bash
+(venv) $ c4t switch
+1 - 124.0.6367.91
+2 - 116.0.5794.0
+Select a version by number: 2
+Creating symlink to chrome version 116.0.5794.0
+Creating symlink to chromedriver version 116.0.5794.0
+Active version is now: 116.0.5794.0
+```
+
+### Common workflow
+
+1. Install one or more versions of Chrome for testing assets
+1. Set/switch the active version
+1. Run your Selenium Webdriver tests with the active version of Chrome for testing
+
+This allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
+
 ## Reference
 
 - [Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 - [GitHub](https://github.com/GoogleChromeLabs/chrome-for-testing)
```

### Comparing `c4t-1.3.0/tests/tests.py` & `c4t-1.4.0/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 from selenium.webdriver import ChromeOptions, ChromeService, Chrome
 import c4t
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 
 
 class C4tTests(unittest.TestCase):
 
     class _TestData:
         specific_version_of_assets = '116.0.5794.0'
```

