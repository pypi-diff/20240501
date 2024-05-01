# Comparing `tmp/tap_readme-0.0.1a4.tar.gz` & `tmp/tap_readme-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Mar 18 17:40:14 2024, max compression
+gzip compressed data, last modified: Wed May  1 20:39:47 2024, max compression
```

## Comparing `tap_readme-0.0.1a4.tar` & `tap_readme-0.0.1a5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      829 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.copier-answers.yml
--rw-r--r--   0        0        0      862 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      733 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/meltano.yml
--rw-r--r--   0        0        0     1248 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.github/dependabot.yml
--rw-r--r--   0        0        0      856 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.github/workflows/build.yml
--rw-r--r--   0        0        0       23 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1709 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.github/workflows/test.yml
--rw-r--r--   0        0        0      409 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.secrets/.gitignore
--rw-r--r--   0        0        0      577 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.vscode/launch.json
--rw-r--r--   0        0        0       51 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.vscode/settings.json
--rw-r--r--   0        0        0       14 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/output/.gitignore
--rw-r--r--   0        0        0       81 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tap_readme/__init__.py
--rw-r--r--   0        0        0      113 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tap_readme/__main__.py
--rw-r--r--   0        0        0     2057 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tap_readme/client.py
--rw-r--r--   0        0        0     4037 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tap_readme/streams.py
--rw-r--r--   0        0        0     1022 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tap_readme/tap.py
--rw-r--r--   0        0        0       24 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tests/__init__.py
--rw-r--r--   0        0        0       92 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tests/conftest.py
--rw-r--r--   0        0        0      417 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/tests/test_core.py
--rw-r--r--   0        0        0     1863 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/.gitignore
--rw-r--r--   0        0        0    11355 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/LICENSE
--rw-r--r--   0        0        0     3033 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/README.md
--rw-r--r--   0        0        0     3222 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0    17371 2024-03-18 17:40:14.000000 tap_readme-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      829 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.copier-answers.yml
+-rw-r--r--   0        0        0      862 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      733 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/meltano.yml
+-rw-r--r--   0        0        0     1174 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.github/dependabot.yml
+-rw-r--r--   0        0        0      856 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.github/workflows/build.yml
+-rw-r--r--   0        0        0       23 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1733 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      409 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.secrets/.gitignore
+-rw-r--r--   0        0        0      577 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.vscode/launch.json
+-rw-r--r--   0        0        0       51 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.vscode/settings.json
+-rw-r--r--   0        0        0       14 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/output/.gitignore
+-rw-r--r--   0        0        0       81 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tap_readme/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tap_readme/__main__.py
+-rw-r--r--   0        0        0     2057 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tap_readme/client.py
+-rw-r--r--   0        0        0     4037 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tap_readme/streams.py
+-rw-r--r--   0        0        0     1022 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tap_readme/tap.py
+-rw-r--r--   0        0        0       24 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tests/conftest.py
+-rw-r--r--   0        0        0      417 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/tests/test_core.py
+-rw-r--r--   0        0        0     1863 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/.gitignore
+-rw-r--r--   0        0        0    11355 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/LICENSE
+-rw-r--r--   0        0        0     3033 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/README.md
+-rw-r--r--   0        0        0     3214 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0    17523 2024-05-01 20:39:47.000000 tap_readme-0.0.1a5/PKG-INFO
```

### Comparing `tap_readme-0.0.1a4/.copier-answers.yml` & `tap_readme-0.0.1a5/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/.pre-commit-config.yaml` & `tap_readme-0.0.1a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/meltano.yml` & `tap_readme-0.0.1a5/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/.github/dependabot.yml` & `tap_readme-0.0.1a5/.github/dependabot.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,14 @@
       time: "10:00"
     reviewers:
       - "edgarrmondragon"
     versioning-strategy: increase-if-necessary
     commit-message:
       prefix: "feat(deps): "
       prefix-development: "chore(deps-dev): "
-    groups:
-      singer-sdk:
-        patterns:
-          - "singer-sdk*"
   - package-ecosystem: pip
     directory: "/.github/workflows"
     schedule:
       interval: "monthly"
       timezone: "Etc/UTC"
       time: "10:00"
     reviewers:
```

### Comparing `tap_readme-0.0.1a4/.github/workflows/build.yml` & `tap_readme-0.0.1a5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/.github/workflows/test.yml` & `tap_readme-0.0.1a5/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - .github/workflows/constraints.txt
 
 jobs:
   test:
     runs-on: ubuntu-latest
     env:
       FORCE_COLOR: "1"
-      PIP_CONSTRAINT: .github/workflows/constraints.txt
+      PIP_CONSTRAINT: ${{ github.workspace }}/.github/workflows/constraints.txt
     strategy:
       fail-fast: false
       matrix:
         script: ["test:integration"]
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         include:
         - { script: "test:dependencies", python-version: "3.12" }
```

### Comparing `tap_readme-0.0.1a4/.vscode/launch.json` & `tap_readme-0.0.1a5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/tap_readme/client.py` & `tap_readme-0.0.1a5/tap_readme/client.py`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/tap_readme/streams.py` & `tap_readme-0.0.1a5/tap_readme/streams.py`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/tap_readme/tap.py` & `tap_readme-0.0.1a5/tap_readme/tap.py`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/.gitignore` & `tap_readme-0.0.1a5/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/LICENSE` & `tap_readme-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/README.md` & `tap_readme-0.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `tap_readme-0.0.1a4/pyproject.toml` & `tap_readme-0.0.1a5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -27,23 +27,23 @@
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "requests<3,>=2",
-  "singer-sdk~=0.36.1",
+  "singer-sdk~=0.37.0",
 ]
 optional-dependencies.dev = [
   "tap-readme[testing,typing]",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=8",
-  "singer-sdk[testing]~=0.36.1",
+  "singer-sdk[testing]",
 ]
 optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
 urls.Documentation = "https://github.com/edgarrmondragon/tap-readme#readme"
 urls.Homepage = "https://github.com/edgarrmondragon/tap-readme"
```

### Comparing `tap_readme-0.0.1a4/PKG-INFO` & `tap_readme-0.0.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tap-readme
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: `tap-readme` is a Singer tap for ReadMe.com, built with the Meltano SDK for Singer Taps.
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-readme#readme
 Project-URL: Homepage, https://github.com/edgarrmondragon/tap-readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-readme
 Author-email: Edgar Ramírez-Mondragón <edgarrmondragon@hey.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrmondragon@hey.com>
 License:                                  Apache License
@@ -214,21 +214,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: requests<3,>=2
-Requires-Dist: singer-sdk~=0.36.1
+Requires-Dist: singer-sdk~=0.37.0
 Provides-Extra: dev
-Requires-Dist: tap-readme[testing,typing]; extra == 'dev'
+Requires-Dist: deptry>=0.12; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest>=8; extra == 'dev'
+Requires-Dist: singer-sdk[testing]; extra == 'dev'
+Requires-Dist: types-requests; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=8; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.36.1; extra == 'testing'
+Requires-Dist: singer-sdk[testing]; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
 Description-Content-Type: text/markdown
 
 # `tap-readme`
```

