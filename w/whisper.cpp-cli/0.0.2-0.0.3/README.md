# Comparing `tmp/whisper_cpp_cli-0.0.2.tar.gz` & `tmp/whisper_cpp_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "whisper_cpp_cli-0.0.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `whisper_cpp_cli-0.0.2.tar` & `whisper_cpp_cli-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/requirements-dev.in
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/.github/workflows/workflow.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/whisper_cpp/__init__.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/whisper_cpp/__main__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/LICENSE
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/README.md
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/hatch_build.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3005 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0     3127 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/.gitignore
+-rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1611 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/README.md
+-rw-r--r--   0        0        0      761 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/requirements-dev.in
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/whisper_cpp/__init__.py
+-rw-r--r--   0        0        0     1082 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/whisper_cpp/__main__.py
+-rw-r--r--   0        0        0     3080 2022-11-09 12:37:21.000000 whisper_cpp_cli-0.0.3/PKG-INFO
```

### Comparing `whisper_cpp_cli-0.0.2/.github/workflows/workflow.yml` & `whisper_cpp_cli-0.0.3/.github/workflows/workflow.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,45 +11,42 @@
       - published
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref_name }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 jobs:
-  build_macos_wheels:
-    name: macOS (${{ matrix.os }})
+  build_wheels:
+    name: Wheels (${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
-        os: [ macos-13, macos-14 ]
+        os: [ macos-13, macos-14, windows-2022 ]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_TEST_COMMAND: >
-            whisper-cpp -h &&
-            python -m whisper_cpp -h
-          CIBW_ARCHS_MACOS: "native"
           CIBW_BUILD: "cp312-*"
-          MACOSX_DEPLOYMENT_TARGET: ${{ matrix.os == 'macos-13' && '10.12' || '11.0' }}
 
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
 
   build_linux_wheels:
     runs-on: ubuntu-latest
     name: Linux (${{ matrix.arch }}, ${{ matrix.tag }})
     strategy:
+      fail-fast: false
       matrix:
-        arch: [ x86_64, i686, aarch64, ppc64le, s390x ]
+        arch: [ x86_64, i686, aarch64, ppc64le ]
         tag: [ manylinux, musllinux ]
         # TODO(charlie): Fails to compile, root cause is unexplored.
         exclude:
           - arch: aarch64
             tag: musllinux
 
     steps:
@@ -60,17 +57,14 @@
         uses: docker/setup-qemu-action@v3
         with:
           platforms: all
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_TEST_COMMAND: >
-            whisper-cpp -h &&
-            python -m whisper_cpp -h
           CIBW_ARCHS_LINUX: ${{ matrix.arch }}
           CIBW_BUILD: "cp312-${{ matrix.tag }}_*"
 
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-linux-${{ matrix.arch }}-${{ matrix.tag }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
@@ -89,15 +83,15 @@
           name: cibw-sdist
           path: dist/*.tar.gz
 
   # Verify that the x86_64 wheels work on macOS 11.
   test_macos_11:
     name: Test macOS 11
     runs-on: macos-11
-    needs: build_macos_wheels
+    needs: build_wheels
     steps:
     - uses: actions/checkout@v4
 
     - uses: actions/download-artifact@v4
       with:
         name: cibw-wheels-macos-13-0
         path: wheelhouse
@@ -105,15 +99,15 @@
     - name: Install wheel
       run: pip install wheelhouse/*.whl
 
     - name: Test wheel
       run: python -m whisper_cpp -h
 
   upload_pypi:
-    needs: [ build_macos_wheels, build_linux_wheels, build_sdist ]
+    needs: [ build_wheels, build_linux_wheels, build_sdist ]
     runs-on: ubuntu-latest
     environment: pypi
     permissions:
       id-token: write
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v4
```

### Comparing `whisper_cpp_cli-0.0.2/whisper_cpp/__main__.py` & `whisper_cpp_cli-0.0.3/whisper_cpp/__main__.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.2/.gitignore` & `whisper_cpp_cli-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.2/LICENSE` & `whisper_cpp_cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.2/README.md` & `whisper_cpp_cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.2/pyproject.toml` & `whisper_cpp_cli-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["scikit-build-core"]
+build-backend = "scikit_build_core.build"
 
 [project]
 name = "whisper.cpp-cli"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Python package for the whisper.cpp CLI."
 authors = [{ name = "Charlie Marsh", email = "charlie.r.marsh@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 dependencies = []
 
-[tool.hatch.build.targets.wheel]
-packages = ["whisper_cpp"]
-
-[tool.hatch.build.hooks.custom]
-path = "hatch_build.py"
+[tool.scikit-build]
+minimum-version = "0.9"
+cmake.define.BUILD_SHARED_LIBS = false
+cmake.version = ">=3.28"
+wheel.packages = ["whisper_cpp"]
+wheel.py-api = "py3"
 
 [tool.ruff]
 line-length = 100
 
 [tool.ruff.lint]
 extend-select = ["I", "B", "UP"]
+
+[tool.cibuildwheel]
+test-command = [
+    "whisper-cpp -h",
+    "python -m whisper_cpp -h",
+]
+environment.MACOSX_DEPLOYMENT_TARGET = "10.12"
+
```

### Comparing `whisper_cpp_cli-0.0.2/PKG-INFO` & `whisper_cpp_cli-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: whisper.cpp-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for the whisper.cpp CLI.
-Author-email: Charlie Marsh <charlie.r.marsh@gmail.com>
+Author-Email: Charlie Marsh <charlie.r.marsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Charles Marsh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,15 +20,14 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # whisper.cpp-cli
 
 A Python wrapper around the [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) CLI.
```

