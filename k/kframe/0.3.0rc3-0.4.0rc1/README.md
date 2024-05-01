# Comparing `tmp/kframe-0.3.0rc3.tar.gz` & `tmp/kframe-0.4.0rc1.tar.gz`

## Comparing `kframe-0.3.0rc3.tar` & `kframe-0.4.0rc1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.tool-versions
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/CHANGELOG.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.github/workflows/main_build.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/.gitignore
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/README.md
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/pyproject.toml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 kframe-0.3.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.tool-versions
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 kframe-0.4.0rc1/PKG-INFO
```

### Comparing `kframe-0.3.0rc3/CHANGELOG.md` & `kframe-0.4.0rc1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,51 @@
-## v0.2.3.dev8900459389 (2024-04-30)
-
-## v0.2.3a4 (2024-04-30)
+## v0.4.0a1 (2024-05-01)
 
 ### Fix
 
-- Merge branch 'main' of github.com:kaeus-sgarcia/kframe
-
-## v0.2.3a3 (2024-04-30)
+- Update license format
 
-## v0.2.3a2 (2024-04-30)
+## v0.3.0 (2024-05-01)
 
 ### Fix
 
+- Update github actions versions
 - Merge branch 'main' of github.com:kaeus-sgarcia/kframe
-- Fix development, qa, and main branches CI/CD
-
-## v0.2.3a1 (2024-04-30)
-
-### Fix
-
 - Merge branch 'main' of github.com:kaeus-sgarcia/kframe
 - Fix development, qa, and main branches CI/CD
+- Merge branch 'main' of github.com:kaeus-sgarcia/kframe
 
 ## v0.2.2 (2024-04-30)
 
 ### Fix
 
 - Fix development, qa, and main branches CI/CD
-
-## v0.2.2a1 (2024-04-30)
-
-### Fix
-
 - Fix development, qa, and main branches CI/CD
 
 ## v0.2.1 (2024-04-30)
 
 ### Fix
 
 - Fix development, qa, and main branches CI/CD
+- Fix development, qa, and main branches CI/CD
 
 ## v0.2.0 (2024-04-30)
 
-## v0.2.0b3 (2024-04-30)
-
-## v0.2.0b2 (2024-04-30)
+### Feat
 
-## v0.2.0a5 (2024-04-30)
+- Initial project structure and cicd action
 
 ### Fix
 
 - Fix development, qa, and main branches CI/CD
-
-## v0.2.0a4 (2024-04-30)
-
-### Fix
-
 - Merge branch 'development' of github.com:kaeus-sgarcia/kframe into development
 - Fix development, qa, and main branches CI/CD
-
-## v0.2.0b1 (2024-04-30)
-
-## v0.2.0a3 (2024-04-30)
-
-### Fix
-
 - Merge branch 'development' of github.com:kaeus-sgarcia/kframe into development
 - Fix development, qa, and main branches CI/CD
-
-## v0.2.0a2 (2024-04-30)
-
-### Fix
-
 - Fix development, qa, and main branches CI/CD
-
-## v0.2.0a1 (2024-04-30)
-
-### Feat
-
-- Initial project structure and cicd action
-
-### Fix
-
 - Fix development, qa, and main branches CI/CD
 - Fix development, qa, and main branches CI/CD
 - Fix development, qa, and main branches CI/CD
 - Fix development, qa, and main branches CI/CD
 - Fix development, qa, and main branches CI/CD
 - Fix development, qa, and main branches CI/CD
 - Fix development, qa, and main branches CI/CD
```

### Comparing `kframe-0.3.0rc3/.github/workflows/main_ci.yml` & `kframe-0.4.0rc1/.github/workflows/main_ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -14,19 +14,14 @@
   PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
   ci:
     name: CI Python 3.10 on linux
     runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        os: [ubuntu-latest]
-        python-version: ['3.10']
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python 3.10
       uses: actions/setup-python@v5
       with:
@@ -38,15 +33,15 @@
     - name: Run static analysis
       run: hatch fmt --check
 
     - name: Run tests
       run: hatch run cov
 
   version_bump:
-    name: "Version bump to dev version"
+    name: "Version bump to alpha version"
     runs-on: "ubuntu-latest"
     needs: ci
     permissions:
       contents: write
 
     steps:
       - name: Check out
```

### Comparing `kframe-0.3.0rc3/.github/workflows/main_pre_release.yml` & `kframe-0.4.0rc1/.github/workflows/main_pre_release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
           token: "${{ github.token }}"
 
       - name: Create bump and changelog
         id: cz
         uses: commitizen-tools/commitizen-action@master
         with:
           github_token: ${{ github.token }}
-          changelog: false
           prerelease: "rc"
 
       - name: New revision
         id: set_new_revision
         run: |
           echo "new_revision=v${{ env.REVISION}}" 
           echo "new_revision=v${{ env.REVISION}}" >> $GITHUB_OUTPUT
```

### Comparing `kframe-0.3.0rc3/.github/workflows/main_release.yml` & `kframe-0.4.0rc1/.github/workflows/main_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
           token: "${{ github.token }}"
 
       - name: Create bump and changelog
         id: cz
         uses: commitizen-tools/commitizen-action@master
         with:
           github_token: ${{ github.token }}
-          changelog: false
 
       - name: New revision
         id: set_new_revision
         run: |
           echo "new_revision=v${{ env.REVISION}}" 
           echo "new_revision=v${{ env.REVISION}}" >> $GITHUB_OUTPUT
 
@@ -138,15 +137,14 @@
         python-version: "3.12"
 
     - name: Create release
       uses: softprops/action-gh-release@v1
       with:
         tag_name: ${{ needs.version_bump.outputs.new_revision }}
         files: dist/*
-        prerelease: true
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
   
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Publish
```

### Comparing `kframe-0.3.0rc3/src/kframe/config/configattr.py` & `kframe-0.4.0rc1/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.3.0rc3/src/kframe/config/configentity.py` & `kframe-0.4.0rc1/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.3.0rc3/tests/test_secretattr.py` & `kframe-0.4.0rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.3.0rc3/LICENSE.txt` & `kframe-0.4.0rc1/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,34 +16,34 @@
    (A) Copyright Grant- Subject to the terms of this license, including the 
        license conditions and limitations in section 3, each contributor grants you 
        a non-exclusive, worldwide, royalty-free copyright license to reproduce its 
        contribution, prepare derivative works of its contribution, and distribute 
        its contribution or any derivative works that you create.
    
    (B) Patent Grant- Subject to the terms of this license, including the license
-      conditions and limitations in section 3, each contributor grants you a 
-      non-exclusive, worldwide, royalty-free license under its licensed patents to make,
-      have made, use, sell, offer for sale, import, and/or otherwise dispose of its
-      contribution in the software or derivative works of the contribution in the 
-      software.
+       conditions and limitations in section 3, each contributor grants you a 
+       non-exclusive, worldwide, royalty-free license under its licensed patents to make,
+       have made, use, sell, offer for sale, import, and/or otherwise dispose of its
+       contribution in the software or derivative works of the contribution in the 
+       software.
 
 3. Conditions and Limitations
    (A) No Trademark License- This license does not grant you rights to use any 
-      contributors' name, logo, or trademarks.
+       contributors' name, logo, or trademarks.
 
    (B) If you bring a patent claim against any contributor over patents that you 
-      claim are infringed by the software, your patent license from such contributor 
-      to the software ends automatically.
+       claim are infringed by the software, your patent license from such contributor 
+       to the software ends automatically.
 
    (C) If you distribute any portion of the software, you must retain all copyright,
-      patent, trademark, and attribution notices that are present in the software.
+       patent, trademark, and attribution notices that are present in the software.
 
    (D) If you distribute any portion of the software in source code form, you may do 
-      so only under this license by including a complete copy of this license with your 
-      distribution. If you distribute any portion of the software in compiled or object 
-      code form, you may only do so under a license that complies with this license.
+       so only under this license by including a complete copy of this license with your 
+       distribution. If you distribute any portion of the software in compiled or object 
+       code form, you may only do so under a license that complies with this license.
 
    (E) The software is licensed "as-is." You bear the risk of using it. The 
-      contributors give no express warranties, guarantees, or conditions. You may have 
-      additional consumer rights under your local laws which this license cannot change. 
-      To the extent permitted under your local laws, the contributors exclude the implied 
-      warranties of merchantability, fitness for a particular purpose and non-infringement.
+       contributors give no express warranties, guarantees, or conditions. You may have 
+       additional consumer rights under your local laws which this license cannot change. 
+       To the extent permitted under your local laws, the contributors exclude the implied 
+       warranties of merchantability, fitness for a particular purpose and non-infringement.
```

### Comparing `kframe-0.3.0rc3/README.md` & `kframe-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.3.0rc3/pyproject.toml` & `kframe-0.4.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.3.0rc3"
+version = "0.4.0rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
@@ -107,11 +107,12 @@
 name = "cz_conventional_commits"
 tag_format = "v$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 annoted_tag = true
 major_version_zero = true
 prerelease_offset = 1
+changelog_merge_prerelease = true
 version_files = [
     "pyproject.toml/project:^version",
     "src/kframe/__about__.py:^__version__"
 ]
```

### Comparing `kframe-0.3.0rc3/PKG-INFO` & `kframe-0.4.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.3.0rc3
+Version: 0.4.0rc1
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
```

