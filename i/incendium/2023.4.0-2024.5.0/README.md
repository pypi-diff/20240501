# Comparing `tmp/incendium-2023.4.0.tar.gz` & `tmp/incendium-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/incendium/incendium/dist/tmpn3HAbp/incendium-2023.4.0.tar", last modified: Wed Apr 19 00:28:20 2023, max compression
+gzip compressed data, was "/__w/incendium/incendium/dist/tmpSVzpCs/incendium-2024.5.0.tar", last modified: Wed May  1 08:02:27 2024, max compression
```

## Comparing `incendium-2023.4.0.tar` & `incendium-2024.5.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    14336 2023-04-19 00:28:20.000000 incendium-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-04-19 00:28:09.000000 incendium-2023.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-19 00:28:09.000000 incendium-2023.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14336 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium/
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium/vision/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/vision/gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/vision/nav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium/helper/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/helper/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/net.py
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7468 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    17135 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/db.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-19 00:28:20.000000 incendium-2023.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-04-19 00:28:09.000000 incendium-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-19 00:28:09.000000 incendium-2023.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-04-19 00:28:09.000000 incendium-2023.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-19 00:28:09.000000 incendium-2023.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:02:26.000000 incendium-2024.5.0/
+-rw-rw-r--   0 root         (0) root         (0)     2065 2024-05-01 07:56:56.000000 incendium-2024.5.0/setup.py
+-rw-rw-r--   0 root         (0) root         (0)     5201 2024-05-01 07:56:56.000000 incendium-2024.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 08:02:26.000000 incendium-2024.5.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4479 2024-05-01 07:56:56.000000 incendium-2024.5.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-05-01 08:02:26.000000 incendium-2024.5.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      707 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      121 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium/vision/
+-rw-rw-r--   0 root         (0) root         (0)     2735 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/vision/nav.py
+-rw-rw-r--   0 root         (0) root         (0)    11217 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/vision/gui.py
+-rw-rw-r--   0 root         (0) root         (0)      175 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/vision/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17135 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/db.py
+-rw-rw-r--   0 root         (0) root         (0)     1453 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/date.py
+-rw-rw-r--   0 root         (0) root         (0)     1992 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/constants.py
+-rw-rw-r--   0 root         (0) root         (0)      524 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/l10n.py
+-rw-rw-r--   0 root         (0) root         (0)     1082 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/time.py
+-rw-rw-r--   0 root         (0) root         (0)     3277 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/net.py
+-rw-rw-r--   0 root         (0) root         (0)     2234 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1292 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/tag.py
+-rw-rw-r--   0 root         (0) root         (0)     7468 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/dataset.py
+-rw-rw-r--   0 root         (0) root         (0)      211 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:02:26.000000 incendium-2024.5.0/src/incendium/helper/
+-rw-rw-r--   0 root         (0) root         (0)       21 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/helper/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/helper/types.py
+-rw-rw-r--   0 root         (0) root         (0)     6553 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/user.py
+-rw-rw-r--   0 root         (0) root         (0)     3354 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/util.py
+-rw-rw-r--   0 root         (0) root         (0)     4254 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      364 2024-05-01 07:56:56.000000 incendium-2024.5.0/src/incendium/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)       21 2024-05-01 07:56:56.000000 incendium-2024.5.0/MANIFEST.in
```

### Comparing `incendium-2023.4.0/README.md` & `incendium-2024.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,47 @@
 # incendium
 
 <!--- Badges --->
-[![GitHub contributors](https://img.shields.io/github/contributors/thecesrom/incendium)](https://github.com/thecesrom/incendium/graphs/contributors)
-[![Downloads](https://pepy.tech/badge/incendium)](https://pepy.tech/project/incendium)
-[![PyPI](https://img.shields.io/pypi/v/incendium)](https://pypi.org/project/incendium/)
-![GitHub last commit (code)](https://img.shields.io/github/last-commit/thecesrom/incendium)
-[![time tracker](https://wakatime.com/badge/github/thecesrom/incendium.svg)](https://wakatime.com/badge/github/thecesrom/incendium)
-[![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)
+[![ci](https://github.com/ignition-incendium/incendium/actions/workflows/ci.yml/badge.svg)](https://github.com/ignition-incendium/incendium/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Imports: flake8](https://img.shields.io/badge/%20imports-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
-[![Imports: pydocstyle](https://img.shields.io/badge/%20imports-pydocstyle-%231674b1?style=flat&labelColor=ef8336)](https://www.pydocstyle.org/en/stable/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/thecesrom/incendium/code.svg)](https://results.pre-commit.ci/latest/github/thecesrom/incendium/code)
-[![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/thecesrom/incendium/discussions)
-
->(/inˈken.di.um/)
->
->_noun_.
->
->1. A fire, inferno, conflagration; heat; torch.
->1. (heat of) passion, vehemence
-
-:package: Package that extends and wraps some functions from Ignition's Scripting API.
-
-For more information, please refer to the [Wiki](https://github.com/thecesrom/incendium/wiki).
+[![Downloads](https://pepy.tech/badge/incendium)](https://pepy.tech/project/incendium)
+[![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/ignition-incendium/incendium/discussions)
 
-## `incendium` Project
+:package: Package that extends and wraps some functions from Ignition's
+Scripting API.
 
-We have moved the `project` branch to its own repo, [`incendium-project`](https://github.com/thecesrom/incendium-project)
+For more information, please refer to the [Wiki].
 
 ## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 
-* You have installed Python 2.7.18 ([download here](https://www.python.org/downloads/release/python-2718/))
-* You are familiar with [Ignition 8.1 System Functions](https://docs.inductiveautomation.com/display/DOC81/System+Functions)
+- You are familiar with [Ignition 8.1 System Functions]
 
 ## Installation and usage
 
-To use incendium, you may install it by doing any of the following.
+### Installing as a dependency for your scripting projects
 
-### Installing with `pip`
+To use `incendium` in your scripting projects, you may install it by doing any
+of the following.
 
-The preferred method is to install it by running `pip`. It requires Python 2.7.18.
+> [!TIP]
+> To install `incendium` as a Jython package for your Gateway, follow
+> [these instructions]
+
+The preferred method is to install it by running `pip` on a virtual environment
+using [Python 2.7.18].
 
 ```bash
 python2 -m pip install incendium
 ```
 
-This will install it as package to your Python installation, which will allow you to call `incendium`'s Scripting functions from Python's REPL, and get code completion using an IDE (Pycharm or Visual Studio Code).
+This will install it as package to your Python installation, which will allow
+you to call `incendium`'s Scripting functions from Python's REPL, and get code
+completion using an IDE (PyCharm or Visual Studio Code).
 
 ```bash
 $ python2
 Python 2.7.18 (default, Nov  9 2020, 16:23:15)
 [GCC Apple LLVM 12.0.0 (clang-1200.0.32.21)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 >>> from __future__ import print_function
@@ -68,55 +56,100 @@
 
 And to uninstall:
 
 ```bash
 python2 -m pip uninstall incendium
 ```
 
-### Downloading from releases
+### Using as a dependency in PyCharm
 
-You may also download the code targeted to your desired version from the [releases page](https://github.com/thecesrom/incendium/releases) and add it as a dependency to your scripting project.
+To include `incendium` as a dependency in PyCharm, you will need to attach it to
+your project.
 
-#### Using as a dependency in PyCharm
+1. Clone the repo or download from [releases]
+2. With your project open where you want to include `incendium`, navigate to
+  `File > Open` and select the `incendium` project folder
+3. Choose `Attach` when prompted
+4. Under the `incendium` project folder, right-click on the `src/` folder and
+  choose `Mark Directory as > Sources Root`
 
-To include `incendium` as a dependency in PyCharm, you will need to attach it to your project.
+### Installing `incendium` on your Gateway
 
-1. Clone the repo or download from [releases](https://github.com/thecesrom/incendium/releases)
-2. With your project open where you want to include `incendium`, navigate to `File > Open` and select the `incendium` project folder
-3. Choose `Attach` when prompted
-4. Under the `incendium` project folder, right-click on the `src/` folder and choose `Mark Directory as > Sources Root`
+#### As a Jython package
 
-#### Installing `incendium` as a Project on your Gateway
+Starting with version 2024.4.0, this package can be installed using Jython. You
+may use the [Python in Ignition] guide as reference. But here are the basic
+steps:
+
+1. Install [Java 17]
+2. Install [Jython 2.7.3]
+3. Run `jython -m pip install incendium`
+4. Copy the `incendium` directory and `typing.py` from
+  `$JYTHON_HOME/Lib/site-packages` to
+  `$IGNITION_DIR/user-lib/pylib/site-packages`
+5. Done
+
+```sh
+$ jython
+Jython 2.7.3 (tags/v2.7.3:5f29801fe, Sep 10 2022, 18:52:49)
+[OpenJDK 64-Bit Server VM (Azul Systems, Inc.)] on java17.0.11
+Type "help", "copyright", "credits" or "license" for more information.
+>>> from __future__ import print_function
+>>> import incendium
+>>> print(incendium.__doc__)
+incendium.
+
+incendium is a package that extends and wraps some functions from
+Ignition Scripting API.
 
-To install incendium on your Gateway follow these steps:
+For more information, please refer to the Wiki.
+https://github.com/ignition-incendium/incendium/wiki
+```
+
+#### As a Python package
 
-1. Download **incendium.x.x.x.zip** from the [latest release](https://github.com/thecesrom/incendium/releases/latest) or from [Ignition Exchange](https://inductiveautomation.com/exchange/2104)
-1. Browse to your Ignition Gateway (version 8.0+)
-1. Go to **Config > Projects** and click on **Import project...**
-1. Click on **Choose File** and select the downloaded ZIP file
-1. Enter **incendium** as the **Project Name**
-    1. If you're replacing a previous version, make sure to check Allow Overwrite
-1. Click on **Import**
+To install `incendium` as a Python package on your Gateway, simply follow these
+steps:
 
-Alternatively you could follow the instructions for cloning the `project` branch directly into `$IGNITION_DIR/data/projects` found [here](https://github.com/thecesrom/incendium/tree/project#cloning-this-branch).
+1. Install [Python 2.7.18]
+2. Run `python -m pip install incendium`
+3. Copy the `incendium` directory and `typing.py` from
+  `$PYTHON2_HOME/Lib/site-packages` to
+  `$IGNITION_DIR/user-lib/pylib/site-packages`
+4. Done
 
 ## Contributing to `incendium`
 
-See [CONTRIBUTING.md](./CONTRIBUTING.md).
+See [CONTRIBUTING.md].
 
 ## Discussions
 
-Feel free to post your questions and/or ideas at [Discussions](https://github.com/thecesrom/incendium/discussions).
+Feel free to post your questions and/or ideas at [Discussions].
 
 ## Contributors
 
 Thanks to everyone who has contributed to this project.
 
-Up-to-date list of contributors can be found [here](https://github.com/thecesrom/incendium/graphs/contributors).
+Up-to-date list of [contributors].
 
 ## License
 
-See [LICENSE](./LICENSE).
+See [LICENSE].
 
 ## Code of conduct
 
-See [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).
+See [CODE_OF_CONDUCT.md].
+
+<!-- Links -->
+[CODE_OF_CONDUCT.md]: https://github.com/ignition-incendium/.github/blob/main/CODE_OF_CONDUCT.md
+[CONTRIBUTING.md]: https://github.com/ignition-incendium/.github/blob/main/CONTRIBUTING.md#contributing-to-incendium
+[contributors]: https://github.com/ignition-incendium/incendium/graphs/contributors
+[Discussions]: https://github.com/ignition-incendium/incendium/discussions
+[Ignition 8.1 System Functions]: https://docs.inductiveautomation.com/docs/8.1/appendix/scripting-functions
+[Java 17]: https://www.azul.com/downloads/?version=java-17-lts&package=jre#zulu
+[Jython 2.7.3]: https://repo1.maven.org/maven2/org/python/jython-installer/2.7.3/jython-installer-2.7.3.jar
+[LICENSE]: ./LICENSE
+[Python 2.7.18]: https://www.python.org/downloads/release/python-2718/
+[Python in Ignition]: https://support.inductiveautomation.com/hc/en-us/articles/360056397252-Python-In-Ignition
+[releases]: https://github.com/ignition-incendium/incendium/releases
+[these instructions]: #as-a-jython-package
+[Wiki]: https://github.com/ignition-incendium/incendium/wiki
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `incendium-2023.4.0/src/incendium.egg-info/SOURCES.txt` & `incendium-2024.5.0/src/incendium.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 CHANGELOG.md
-LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
-setup.cfg
 setup.py
 src/incendium/__init__.py
+src/incendium/__version__.py
 src/incendium/constants.py
 src/incendium/dataset.py
 src/incendium/date.py
 src/incendium/db.py
 src/incendium/exceptions.py
+src/incendium/gui.py
+src/incendium/l10n.py
 src/incendium/net.py
 src/incendium/tag.py
+src/incendium/time.py
 src/incendium/user.py
 src/incendium/util.py
 src/incendium.egg-info/PKG-INFO
 src/incendium.egg-info/SOURCES.txt
 src/incendium.egg-info/dependency_links.txt
 src/incendium.egg-info/requires.txt
 src/incendium.egg-info/top_level.txt
```

### Comparing `incendium-2023.4.0/src/incendium/vision/gui.py` & `incendium-2024.5.0/src/incendium/vision/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""GUI module."""
+"""Vision GUI module."""
 
 from __future__ import unicode_literals
 
 __all__ = [
     "CURSOR_CROSSHAIR",
     "CURSOR_DEFAULT",
     "CURSOR_E_RESIZE",
@@ -49,16 +49,21 @@
 CURSOR_S_RESIZE = 9
 CURSOR_W_RESIZE = 10
 CURSOR_E_RESIZE = 11
 CURSOR_HAND = 12
 CURSOR_MOVE = 13
 
 
-def authentication(auth_profile="", title="Authentication"):
-    # type: (AnyStr, AnyStr) -> bool
+def authentication(
+    auth_profile="",  # type: AnyStr
+    title="Authentication",  # type: AnyStr
+    username_label_text="Username",  # type: AnyStr
+    password_label_text="Password",  # type: AnyStr
+):
+    # type: (...) -> bool
     """Open up a popup input dialog box.
 
     This dialog box will show a prompt message, and allow the user to
     type in their username and password. When the user is done, they can
     press "OK" or "Cancel". If "OK" is pressed, this function will
     attempt to validate the User credentials against the Authentication
     Profile. If "Cancel" is pressed, this function will return
@@ -66,28 +71,32 @@
 
     Args:
         auth_profile: The name of the authentication profile to run
             against. Leaving this out will use the project's default
             profile. Optional.
         title: A title for the input box. This will be translated to the
             selected Locale. Optional.
+        username_label_text: The text to display for the username label.
+            This will be translated to the selected Locale. Optional.
+        password_label_text: The text to display for the password label.
+            This will be translated to the selected Locale. Optional.
 
     Returns:
         ``True`` if the user was validated, ``False`` otherwise.
     """
     options = [
         system.util.translate(constants.OK_TEXT),
         system.util.translate(constants.CANCEL_TEXT),
     ]
 
     panel = JPanel()
 
     labels = JPanel(GridLayout(0, 1, 2, 2))
-    labels.add(JLabel("{}: ".format(system.util.translate("Username"))))
-    labels.add(JLabel("{}: ".format(system.util.translate("Password"))))
+    labels.add(JLabel("{}: ".format(system.util.translate(username_label_text))))
+    labels.add(JLabel("{}: ".format(system.util.translate(password_label_text))))
     panel.add(labels)
 
     fields = JPanel(GridLayout(0, 1, 2, 2))
     username_field = JTextField(25)
     fields.add(username_field)
     password_field = JPasswordField(25)
     fields.add(password_field)
@@ -109,16 +118,22 @@
         password="".join(password_field.getPassword()),
         authProfile=auth_profile,
     )
 
     return choice == JOptionPane.OK_OPTION and valid
 
 
-def authorization(role, auth_profile="", title="Athorization"):
-    # type: (AnyStr, AnyStr, AnyStr) -> bool
+def authorization(
+    role,  # type: AnyStr
+    auth_profile="",  # type: AnyStr
+    title="Authorization",  # type: AnyStr
+    username_label_text="Username",  # type: AnyStr
+    password_label_text="Password",  # type: AnyStr
+):
+    # type: (...) -> bool
     """Open up a popup input dialog box.
 
     This dialog box will show a prompt message, and allow the user to
     type in their username and password. When the user is done, they can
     press "OK" or "Cancel". If "OK" is pressed, this function will
     attempt to validate the User credentials against the Authentication
     Profile and verify if the User belongs to the ``role``. If "Cancel"
@@ -127,30 +142,34 @@
     Args:
         role: Required role.
         auth_profile: The name of the authentication profile to run
             against. Leaving this out will use the project's default
             profile. Optional.
         title: A title for the input box. This will be translated to the
             selected Locale. Optional.
+        username_label_text: The text to display for the username label.
+            This will be translated to the selected Locale. Optional.
+        password_label_text: The text to display for the password label.
+            This will be translated to the selected Locale. Optional.
 
     Returns:
         ``True`` if the user was validated, ``False`` otherwise.
     """
-    has_role = False
-
     options = [
         system.util.translate(constants.OK_TEXT),
         system.util.translate(constants.CANCEL_TEXT),
     ]
 
+    has_role = False
+
     panel = JPanel()
 
     labels = JPanel(GridLayout(0, 1, 2, 2))
-    labels.add(JLabel("{}: ".format(system.util.translate("Username"))))
-    labels.add(JLabel("{}: ".format(system.util.translate("Password"))))
+    labels.add(JLabel("{}: ".format(system.util.translate(username_label_text))))
+    labels.add(JLabel("{}: ".format(system.util.translate(password_label_text))))
     panel.add(labels)
 
     fields = JPanel(GridLayout(0, 1, 2, 2))
     username_field = JTextField(25)
     fields.add(username_field)
     password_field = JPasswordField(25)
     fields.add(password_field)
@@ -231,18 +250,20 @@
         message: The message to display in an error box. This will be
             translated to the selected Locale.
         title: A title for the error box. This will be translated to the
             selected Locale. Optional.
         detail: Additional text to display. This will be translated to
             the selected Locale. Optional.
     """
-    if detail is None:
-        msg = system.util.translate(message)
-    else:
-        msg = "\n".join([system.util.translate(message), system.util.translate(detail)])
+    msg = (
+        system.util.translate(message)
+        if detail is None
+        else "\n".join([system.util.translate(message), system.util.translate(detail)])
+    )
+
     JOptionPane.showMessageDialog(
         None, msg, system.util.translate(title), JOptionPane.ERROR_MESSAGE
     )
 
 
 def info(message, title="Information", detail=None):
     # type: (AnyStr, AnyStr, Optional[AnyStr]) -> None
@@ -252,18 +273,20 @@
         message: The message to display. This will be translated to the
             selected Locale. Will accept html formatting.
         title: A title for the message box. This will be translated to
             the selected Locale. Optional.
         detail: Additional text to display. This will be translated to
             the selected Locale. Optional.
     """
-    if detail is None:
-        msg = system.util.translate(message)
-    else:
-        msg = "\n".join([system.util.translate(message), system.util.translate(detail)])
+    msg = (
+        system.util.translate(message)
+        if detail is None
+        else "\n".join([system.util.translate(message), system.util.translate(detail)])
+    )
+
     JOptionPane.showMessageDialog(
         None,
         msg,
         system.util.translate(title),
         JOptionPane.INFORMATION_MESSAGE,
     )
 
@@ -289,15 +312,15 @@
     """
     options = [
         system.util.translate(constants.OK_TEXT),
         system.util.translate(constants.CANCEL_TEXT),
     ]
 
     panel = JPanel()
-    label = JLabel("{}: ".format(system.util.translate(message)))
+    label = JLabel("{}: ".format(message))
     panel.add(label)
     text_field = JTextField(25)
     panel.add(text_field)
 
     choice = JOptionPane.showOptionDialog(
         None,
         panel,
@@ -320,14 +343,16 @@
         message: The message to display in a warning box. This will be
             translated to the selected Locale.
         title: A title for the warning box. This will be translated to
             the selected Locale. Optional.
         detail: Additional text to display. This will be translated to
             the selected Locale. Optional.
     """
-    if detail is None:
-        msg = system.util.translate(message)
-    else:
-        msg = "\n".join([system.util.translate(message), system.util.translate(detail)])
+    msg = (
+        system.util.translate(message)
+        if detail is None
+        else "\n".join([system.util.translate(message), system.util.translate(detail)])
+    )
+
     JOptionPane.showMessageDialog(
         None, msg, system.util.translate(title), JOptionPane.WARNING_MESSAGE
     )
```

### Comparing `incendium-2023.4.0/src/incendium/vision/nav.py` & `incendium-2024.5.0/src/incendium/vision/nav.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/src/incendium/tag.py` & `incendium-2024.5.0/src/incendium/tag.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/src/incendium/user.py` & `incendium-2024.5.0/src/incendium/user.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/src/incendium/net.py` & `incendium-2024.5.0/src/incendium/net.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/src/incendium/date.py` & `incendium-2024.5.0/src/incendium/date.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/src/incendium/constants.py` & `incendium-2024.5.0/src/incendium/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,7 +50,13 @@
     "Would you like to proceed without saving your changes?"
 )
 SUCCESS_WINDOW_TITLE = "Success"
 TABBED_LINE = "    - "
 UNEXPECTED_ERROR = "An unexpected error occurred in {}.\n{}"
 UNEXPECTED_ERROR_CAUSED_BY = "An unexpected error occurred in {}.\n{}\nCaused by: {}"
 WARNING_WINDOW_TITLE = "Warning"
+
+# Exceptions
+GATEWAY_EXCEPTION = (
+    "com.inductiveautomation.ignition.client.gateway_interface.GatewayException: "
+)
+MSSQL_SERVER_EXCEPTION = "com.microsoft.sqlserver.jdbc.SQLServerException: "
```

### Comparing `incendium-2023.4.0/src/incendium/dataset.py` & `incendium-2024.5.0/src/incendium/dataset.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/src/incendium/db.py` & `incendium-2024.5.0/src/incendium/db.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.4.0/CHANGELOG.md` & `incendium-2024.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2024.5.0 (2024-05-01)
+
+### Refactor
+
+- **util**: move functions out of util (#199)
+
 ## v2023.4.0 (2023-04-18)
 
 ### Feat
 
 - **db**: handle concurrent DisposableConnection connections (#142)
 
 ## v2023.3.0 (2023-03-30)
```

