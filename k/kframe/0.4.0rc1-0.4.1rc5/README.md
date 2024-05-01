# Comparing `tmp/kframe-0.4.0rc1.tar.gz` & `tmp/kframe-0.4.1rc5.tar.gz`

## Comparing `kframe-0.4.0rc1.tar` & `kframe-0.4.1rc5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.tool-versions
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.gitignore
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/README.md
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/.tool-versions
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/CHANGELOG.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/src/kframe/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/tests/test_secretattr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/LICENSE.txt
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/README.md
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/pyproject.toml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 kframe-0.4.1rc5/PKG-INFO
```

### Comparing `kframe-0.4.0rc1/.github/workflows/main_ci.yml` & `kframe-0.4.1rc5/.github/workflows/main_ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Create development version
+name: Dev
 
 on:
   pull_request:
     branches: [main]
   push:
     branches: [main]
```

### Comparing `kframe-0.4.0rc1/.github/workflows/main_pre_release.yml` & `kframe-0.4.1rc5/.github/workflows/main_release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Create pre-release
+name: Production
 
 on:
   workflow_dispatch
 
 concurrency:
   group: build-${{ github.head_ref }}
   cancel-in-progress: true
@@ -29,15 +29,20 @@
           token: "${{ github.token }}"
 
       - name: Create bump and changelog
         id: cz
         uses: commitizen-tools/commitizen-action@master
         with:
           github_token: ${{ github.token }}
-          prerelease: "rc"
+          changelog_increment_filename: "body.md"
+
+      - uses: actions/upload-artifact@v4
+        with:
+          name: changelog-body
+          path: ./body.md
 
       - name: New revision
         id: set_new_revision
         run: |
           echo "new_revision=v${{ env.REVISION}}" 
           echo "new_revision=v${{ env.REVISION}}" >> $GITHUB_OUTPUT
 
@@ -59,15 +64,15 @@
         echo "From bump: ${{ needs.version_bump.outputs.new_revision }}"
 
     - uses: actions/checkout@v4
       with:
         ref: ${{ needs.version_bump.outputs.new_revision }}
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Run tests
@@ -94,15 +99,15 @@
         echo "From bump: ${{ needs.version_bump.outputs.new_revision }}"
 
     - uses: actions/checkout@v4
       with:
         ref: ${{ needs.version_bump.outputs.new_revision }}
 
     - name: Set up Python 3.12
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.12"
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Build
@@ -127,26 +132,31 @@
         ref: ${{ needs.version_bump.outputs.new_revision }}
 
     - uses: actions/download-artifact@v4
       with:
         pattern: kframe-*
         path: dist
         merge-multiple: true
+
+    - uses: actions/download-artifact@v4
+      with:
+        name: changelog-body
+        path: ./body.md
     
     - name: Set up Python 3.12
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.12"
 
     - name: Create release
       uses: softprops/action-gh-release@v1
       with:
         tag_name: ${{ needs.version_bump.outputs.new_revision }}
         files: dist/*
-        prerelease: true
+        body_path: body.md
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
   
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Publish
```

### Comparing `kframe-0.4.0rc1/.github/workflows/main_release.yml` & `kframe-0.4.1rc5/.github/workflows/main_pre_release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Create release
+name: QA
 
 on:
   workflow_dispatch
 
 concurrency:
   group: build-${{ github.head_ref }}
   cancel-in-progress: true
@@ -29,14 +29,21 @@
           token: "${{ github.token }}"
 
       - name: Create bump and changelog
         id: cz
         uses: commitizen-tools/commitizen-action@master
         with:
           github_token: ${{ github.token }}
+          prerelease: "rc"
+          changelog_increment_filename: "body.md"
+
+      - uses: actions/upload-artifact@v4
+        with:
+          name: changelog-body
+          path: ./body.md
 
       - name: New revision
         id: set_new_revision
         run: |
           echo "new_revision=v${{ env.REVISION}}" 
           echo "new_revision=v${{ env.REVISION}}" >> $GITHUB_OUTPUT
 
@@ -58,15 +65,15 @@
         echo "From bump: ${{ needs.version_bump.outputs.new_revision }}"
 
     - uses: actions/checkout@v4
       with:
         ref: ${{ needs.version_bump.outputs.new_revision }}
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Run tests
@@ -93,15 +100,15 @@
         echo "From bump: ${{ needs.version_bump.outputs.new_revision }}"
 
     - uses: actions/checkout@v4
       with:
         ref: ${{ needs.version_bump.outputs.new_revision }}
 
     - name: Set up Python 3.12
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.12"
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Build
@@ -126,25 +133,31 @@
         ref: ${{ needs.version_bump.outputs.new_revision }}
 
     - uses: actions/download-artifact@v4
       with:
         pattern: kframe-*
         path: dist
         merge-multiple: true
+
+    - uses: actions/download-artifact@v4
+      with:
+        name: changelog-body
     
     - name: Set up Python 3.12
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.12"
 
     - name: Create release
       uses: softprops/action-gh-release@v1
       with:
         tag_name: ${{ needs.version_bump.outputs.new_revision }}
         files: dist/*
+        prerelease: true
+        body_path: body.md
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
   
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Publish
```

### Comparing `kframe-0.4.0rc1/src/kframe/config/configattr.py` & `kframe-0.4.1rc5/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0rc1/src/kframe/config/configentity.py` & `kframe-0.4.1rc5/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0rc1/tests/test_secretattr.py` & `kframe-0.4.1rc5/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0rc1/LICENSE.txt` & `kframe-0.4.1rc5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.4.0rc1/pyproject.toml` & `kframe-0.4.1rc5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.4.0rc1"
+version = "0.4.1rc5"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
@@ -108,11 +108,12 @@
 tag_format = "v$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 annoted_tag = true
 major_version_zero = true
 prerelease_offset = 1
 changelog_merge_prerelease = true
+changelog_incremental = true
 version_files = [
     "pyproject.toml/project:^version",
     "src/kframe/__about__.py:^__version__"
 ]
```

### Comparing `kframe-0.4.0rc1/PKG-INFO` & `kframe-0.4.1rc5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.4.0rc1
+Version: 0.4.1rc5
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
@@ -15,19 +15,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# kframe
+# Kaeus Development Framework
 
-<!-- [![PyPI - Version](https://img.shields.io/pypi/v/kframe.svg)](https://pypi.org/project/kframe)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kframe.svg)](https://pypi.org/project/kframe) -->
+[![PyPI - Version](https://img.shields.io/pypi/v/kframe.svg)](https://pypi.org/project/kframe)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kframe.svg)](https://pypi.org/project/kframe)
 [![CI](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_ci.yml/badge.svg)](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_ci.yml)
+[![Test](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_pre_release.yml/badge.svg)](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_pre_release.yml)
+[![CD](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_release.yml/badge.svg)](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_release.yml)
+[![GitHub release](https://img.shields.io/github/v/release/kaeus-sgarcia/kframe)](https://github.com/kaeus-sgarcia/kframe)
+
+
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
```

