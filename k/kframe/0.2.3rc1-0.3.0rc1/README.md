# Comparing `tmp/kframe-0.2.3rc1.tar.gz` & `tmp/kframe-0.3.0rc1.tar.gz`

## Comparing `kframe-0.2.3rc1.tar` & `kframe-0.3.0rc1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.tool-versions
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/CHANGELOG.md
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/dev_ci.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/main_release.yml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/qa_cd.yml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/qa_ci.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.gitignore
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/README.md
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/pyproject.toml
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.tool-versions
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.github/workflows/main_build.yml
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/.gitignore
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/README.md
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 kframe-0.3.0rc1/PKG-INFO
```

### Comparing `kframe-0.2.3rc1/CHANGELOG.md` & `kframe-0.3.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3rc1/.github/workflows/dev_ci.yml` & `kframe-0.3.0rc1/.github/workflows/main_build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-name: Development CI
+name: Build
 
 on:
-  push:
-    branches: [development]
+  release:
+    types: [published]
 
 concurrency:
-  group: test-${{ github.head_ref }}
+  group: build-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
-  ci:
-    name: CI Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
+  build:
+    name: Build for Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
-        python-version: ['3.10']
+        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ['3.10', '3.11', '3.12']
+    permissions:
+      contents: write
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
-    - name: Run static analysis
-      run: hatch fmt --check
-
     - name: Run tests
       run: hatch run cov
 
-  cd:
-    name: CD
-    runs-on: ubuntu-latest
-    concurrency: release
-    needs: ci
-    permissions:
-      id-token: write
-      contents: write
+    - name: Build
+      run: hatch build
 
-    steps:
-    - uses: actions/checkout@v3
+    - name: Upload artifact to release
+      uses: svenstaro/upload-release-action@v2
       with:
-        fetch-depth: 0
+        repo_token: ${{ secrets.GITHUB_TOKEN }}
+        file: dist/*
+        tag: ${{ github.ref }}
+        overwrite: true
+        file_glob: true
+      
 
-    - name: Python Semantic Release
-      uses: python-semantic-release/python-semantic-release@master
-      with:
-        github_token: ${{ secrets.GITHUB_TOKEN }}
 
-    
 
-  
+
+
+        
+
+
```

### Comparing `kframe-0.2.3rc1/.github/workflows/main_ci.yml` & `kframe-0.3.0rc1/.github/workflows/main_ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: CI
+name: Create development version
 
 on:
   pull_request:
     branches: [main]
   push:
     branches: [main]
 
@@ -12,29 +12,29 @@
 
 env:
   PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
   ci:
-    name: CI Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
-    runs-on: ${{ matrix.os }}
+    name: CI Python 3.10 on linux
+    runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
         python-version: ['3.10']
 
     steps:
     - uses: actions/checkout@v4
 
-    - name: Set up Python ${{ matrix.python-version }}
+    - name: Set up Python 3.10
       uses: actions/setup-python@v5
       with:
-        python-version: ${{ matrix.python-version }}
+        python-version: "3.10"
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Run static analysis
       run: hatch fmt --check
```

### Comparing `kframe-0.2.3rc1/.github/workflows/main_pre_release.yml` & `kframe-0.3.0rc1/.github/workflows/main_release.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,61 @@
-name: Pre-release
+name: Release
 
 on:
   workflow_dispatch
 
 concurrency:
-  group: build-${{ github.head_ref }}
+  group: test-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
+  # ci:
+  #   name: CI Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
+  #   runs-on: ${{ matrix.os }}
+  #   strategy:
+  #     fail-fast: false
+  #     matrix:
+  #       os: [ubuntu-latest, windows-latest, macos-latest]
+  #       python-version: ['3.10', '3.11', '3.12']
+
+  #   steps:
+  #   - uses: actions/checkout@v3
+
+  #   - name: Set up Python ${{ matrix.python-version }}
+  #     uses: actions/setup-python@v4
+  #     with:
+  #       python-version: ${{ matrix.python-version }}
+
+  #   - name: Install Hatch
+  #     run: pip install --upgrade hatch
+
+  #   - name: Run static analysis
+  #     run: hatch fmt --check
+
+  #   - name: Run tests
+  #     run: hatch run cov
+
   version_bump:
-    name: "Version bump to beta version"
+    name: "Version bump to alpha"
     runs-on: "ubuntu-latest"
+    needs: ci
     permissions:
       contents: write
 
     steps:
       - name: Check out
-        uses: actions/checkout@v4
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
-          token: "${{ github.token }}"
+          TOKEN: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Create bump and changelog
         uses: commitizen-tools/commitizen-action@master
         with:
-          github_token: ${{ github.token }}
-          changelog: false
-          prerelease: "rc"
-
-  build:
-    name: Build for Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
-    runs-on: ${{ matrix.os }}
-    needs: version_bump
-    strategy:
-      fail-fast: false
-      matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.10', '3.11', '3.12']
-
-    steps:
-    - uses: actions/checkout@v4
-
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Install Hatch
-      run: pip install --upgrade hatch
-
-    - name: Run tests
-      run: hatch run cov
-
-    - name: Build
-      run: hatch build
-
-    - name: Publish
-      run: hatch publish --user __token__
-
-
-
-
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+          changelog_increment_filename: "body.md"
```

### Comparing `kframe-0.2.3rc1/src/kframe/config/configattr.py` & `kframe-0.3.0rc1/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3rc1/src/kframe/config/configentity.py` & `kframe-0.3.0rc1/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3rc1/tests/test_secretattr.py` & `kframe-0.3.0rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3rc1/LICENSE.txt` & `kframe-0.3.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3rc1/README.md` & `kframe-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3rc1/pyproject.toml` & `kframe-0.3.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.2.3rc1"
+version = "0.3.0rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
@@ -24,17 +24,17 @@
   "Operating System :: MacOS",
 ]
 dependencies = [
 ]
 
 [project.urls]
 # TODO: Update these URLs
-Documentation = "https://github.com/unknown/kframe#readme"
-Issues = "https://github.com/unknown/kframe/issues"
-Source = "https://github.com/unknown/kframe"
+Documentation = "https://github.com/kaeus-sgarcia/kframe#readme"
+Issues = "https://github.com/kaeus-sgarcia/kframe/issues"
+Source = "https://github.com/kaeus-sgarcia/kframe"
 
 # Development environment
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "ruff",
```

### Comparing `kframe-0.2.3rc1/PKG-INFO` & `kframe-0.3.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.2.3rc1
+Version: 0.3.0rc1
 Summary: Kaeus development framework
-Project-URL: Documentation, https://github.com/unknown/kframe#readme
-Project-URL: Issues, https://github.com/unknown/kframe/issues
-Project-URL: Source, https://github.com/unknown/kframe
+Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
+Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
+Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
```

