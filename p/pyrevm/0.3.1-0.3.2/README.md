# Comparing `tmp/pyrevm-0.3.1.tar.gz` & `tmp/pyrevm-0.3.2.tar.gz`

## Comparing `pyrevm-0.3.1.tar` & `pyrevm-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 pyrevm-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127      613 2024-04-19 13:15:32.000000 pyrevm-0.3.1/.github/workflows/py.yml
--rw-r--r--   0     1001      127     3522 2024-04-19 13:15:32.000000 pyrevm-0.3.1/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1537 2024-04-19 13:15:32.000000 pyrevm-0.3.1/.github/workflows/rust.yml
--rw-r--r--   0     1001      127       30 2024-04-19 13:15:32.000000 pyrevm-0.3.1/.gitignore
--rw-r--r--   0     1001      127      206 2024-04-19 13:15:32.000000 pyrevm-0.3.1/Makefile
--rw-r--r--   0     1001      127     2264 2024-04-19 13:15:32.000000 pyrevm-0.3.1/README.md
--rw-r--r--   0     1001      127    35461 2024-04-19 13:15:32.000000 pyrevm-0.3.1/bench/snailtracer/snailtracer.evm
--rw-r--r--   0     1001      127     1715 2024-04-19 13:15:32.000000 pyrevm-0.3.1/bench/snailtracer/snailtracer.py
--rw-r--r--   0     1001      127    23877 2024-04-19 13:15:32.000000 pyrevm-0.3.1/poetry.lock
--rw-r--r--   0     1001      127     9017 2024-04-19 13:15:32.000000 pyrevm-0.3.1/pyrevm.pyi
--rw-r--r--   0     1001      127      265 2024-04-19 13:15:32.000000 pyrevm-0.3.1/pytest/contracts/blueprint.bin
--rw-r--r--   0     1001      127     1194 2024-04-19 13:15:32.000000 pyrevm-0.3.1/pytest/contracts/full_math.bin
--rw-r--r--   0     1001      127     6248 2024-04-19 13:15:32.000000 pyrevm-0.3.1/pytest/contracts/weth_9.bin
--rw-r--r--   0     1001      127     6325 2024-04-19 13:15:32.000000 pyrevm-0.3.1/pytest/test.py
--rw-r--r--   0     1001      127     4400 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/database.rs
--rw-r--r--   0     1001      127     1202 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/empty_db_wrapper.rs
--rw-r--r--   0     1001      127    12405 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/evm.rs
--rw-r--r--   0     1001      127     6232 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/executor.rs
--rw-r--r--   0     1001      127      801 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127      786 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/pystdout.rs
--rw-r--r--   0     1001      127      193 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/types/checkpoint.rs
--rw-r--r--   0     1001      127     6657 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/types/evm_env.rs
--rw-r--r--   0     1001      127     2431 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/types/execution_result.rs
--rw-r--r--   0     1001      127     1898 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/types/info.rs
--rw-r--r--   0     1001      127      321 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/types/mod.rs
--rw-r--r--   0     1001      127      591 2024-04-19 13:15:32.000000 pyrevm-0.3.1/src/utils.rs
--rw-r--r--   0     1001      127    82487 2024-04-19 13:15:32.000000 pyrevm-0.3.1/Cargo.lock
--rw-r--r--   0     1001      127      759 2024-04-19 13:15:32.000000 pyrevm-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 pyrevm-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pyrevm-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127      612 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.github/workflows/py.yml
+-rw-r--r--   0     1001      127     3522 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1537 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       30 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.gitignore
+-rw-r--r--   0     1001      127      205 2024-05-01 13:03:54.000000 pyrevm-0.3.2/Makefile
+-rw-r--r--   0     1001      127     2265 2024-05-01 13:03:54.000000 pyrevm-0.3.2/README.md
+-rw-r--r--   0     1001      127    35461 2024-05-01 13:03:54.000000 pyrevm-0.3.2/bench/snailtracer/snailtracer.evm
+-rw-r--r--   0     1001      127     1715 2024-05-01 13:03:54.000000 pyrevm-0.3.2/bench/snailtracer/snailtracer.py
+-rw-r--r--   0     1001      127    16997 2024-05-01 13:03:54.000000 pyrevm-0.3.2/poetry.lock
+-rw-r--r--   0     1001      127    10135 2024-05-01 13:03:54.000000 pyrevm-0.3.2/pyrevm.pyi
+-rw-r--r--   0     1001      127     4400 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/database.rs
+-rw-r--r--   0     1001      127     1202 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/empty_db_wrapper.rs
+-rw-r--r--   0     1001      127    12521 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/evm.rs
+-rw-r--r--   0     1001      127     6226 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/executor.rs
+-rw-r--r--   0     1001      127      894 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      127      786 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/pystdout.rs
+-rw-r--r--   0     1001      127      193 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/checkpoint.rs
+-rw-r--r--   0     1001      127     8830 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/evm_env.rs
+-rw-r--r--   0     1001      127     2431 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/execution_result.rs
+-rw-r--r--   0     1001      127     1898 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/info.rs
+-rw-r--r--   0     1001      127      321 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/mod.rs
+-rw-r--r--   0     1001      127      991 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/utils.rs
+-rw-r--r--   0     1001      127        0 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/__init__.py
+-rw-r--r--   0     1001      127      320 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/blob_base_fee.bin
+-rw-r--r--   0     1001      127      492 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/blob_hash.bin
+-rw-r--r--   0     1001      127      265 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/blueprint.bin
+-rw-r--r--   0     1001      127     1194 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/full_math.bin
+-rw-r--r--   0     1001      127     6248 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/weth_9.bin
+-rw-r--r--   0     1001      127     7995 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/test_evm.py
+-rw-r--r--   0     1001      127      511 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/utils.py
+-rw-r--r--   0     1001      127    82487 2024-05-01 13:03:54.000000 pyrevm-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      127      711 2024-05-01 13:03:54.000000 pyrevm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 pyrevm-0.3.2/PKG-INFO
```

### Comparing `pyrevm-0.3.1/.github/workflows/py.yml` & `pyrevm-0.3.2/.github/workflows/py.yml`

 * *Files 3% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         run: poetry install
 
       # May need to install Rust?
       - name: Build the Rust package
         run: poetry run maturin develop
 
       - name: Run tests
-        run: poetry run pytest ./pytest/*
+        run: poetry run pytest ./tests/*
```

### Comparing `pyrevm-0.3.1/.github/workflows/release.yml` & `pyrevm-0.3.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/.github/workflows/rust.yml` & `pyrevm-0.3.2/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/README.md` & `pyrevm-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     value=...,
 )
 evm.revert(checkpoint)  # or: evm.commit() to clear all checkpoints
 ```
 
 **Note**: in contrast to the Rust library, the Python library does not automatically commit to database.
 
-See more usage examples in the [pytests](./pytest/test.py).
+See more usage examples in the [pytests](tests/test_evm.py).
 
 ## Develop
 
 We use Poetry for virtual environment management and [Maturin](https://github.com/PyO3/maturin) as our Rust <> Python FFI build system. The Rust bindings are auto-generated from the macros provided by [PyO3](https://pyo3.rs/v0.17.1/).
 
 To build the library, run `make build`. To run the tests, run `make test`.
```

### Comparing `pyrevm-0.3.1/bench/snailtracer/snailtracer.evm` & `pyrevm-0.3.2/bench/snailtracer/snailtracer.evm`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/bench/snailtracer/snailtracer.py` & `pyrevm-0.3.2/bench/snailtracer/snailtracer.py`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/poetry.lock` & `pyrevm-0.3.2/poetry.lock`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.7.1 and should not be changed by hand.
 
 [[package]]
 name = "black"
-version = "22.12.0"
+version = "24.4.0"
 description = "The uncompromising code formatter."
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "black-22.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eedd20838bd5d75b80c9f5487dbcb06836a43833a37846cf1d8c1cc01cef59d"},
-    {file = "black-22.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:159a46a4947f73387b4d83e87ea006dbb2337eab6c879620a3ba52699b1f4351"},
-    {file = "black-22.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d30b212bffeb1e252b31dd269dfae69dd17e06d92b87ad26e23890f3efea366f"},
-    {file = "black-22.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:7412e75863aa5c5411886804678b7d083c7c28421210180d67dfd8cf1221e1f4"},
-    {file = "black-22.12.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c116eed0efb9ff870ded8b62fe9f28dd61ef6e9ddd28d83d7d264a38417dcee2"},
-    {file = "black-22.12.0-cp37-cp37m-win_amd64.whl", hash = "sha256:1f58cbe16dfe8c12b7434e50ff889fa479072096d79f0a7f25e4ab8e94cd8350"},
-    {file = "black-22.12.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:77d86c9f3db9b1bf6761244bc0b3572a546f5fe37917a044e02f3166d5aafa7d"},
-    {file = "black-22.12.0-cp38-cp38-win_amd64.whl", hash = "sha256:82d9fe8fee3401e02e79767016b4907820a7dc28d70d137eb397b92ef3cc5bfc"},
-    {file = "black-22.12.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:101c69b23df9b44247bd88e1d7e90154336ac4992502d4197bdac35dd7ee3320"},
-    {file = "black-22.12.0-cp39-cp39-win_amd64.whl", hash = "sha256:559c7a1ba9a006226f09e4916060982fd27334ae1998e7a38b3f33a37f7a2148"},
-    {file = "black-22.12.0-py3-none-any.whl", hash = "sha256:436cc9167dd28040ad90d3b404aec22cedf24a6e4d7de221bec2730ec0c97bcf"},
-    {file = "black-22.12.0.tar.gz", hash = "sha256:229351e5a18ca30f447bf724d007f890f97e13af070bb6ad4c0a441cd7596a2f"},
+    {file = "black-24.4.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436"},
+    {file = "black-24.4.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf"},
+    {file = "black-24.4.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad"},
+    {file = "black-24.4.0-cp310-cp310-win_amd64.whl", hash = "sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb"},
+    {file = "black-24.4.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8"},
+    {file = "black-24.4.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745"},
+    {file = "black-24.4.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070"},
+    {file = "black-24.4.0-cp311-cp311-win_amd64.whl", hash = "sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397"},
+    {file = "black-24.4.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2"},
+    {file = "black-24.4.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33"},
+    {file = "black-24.4.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965"},
+    {file = "black-24.4.0-cp312-cp312-win_amd64.whl", hash = "sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd"},
+    {file = "black-24.4.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1"},
+    {file = "black-24.4.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8"},
+    {file = "black-24.4.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d"},
+    {file = "black-24.4.0-cp38-cp38-win_amd64.whl", hash = "sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3"},
+    {file = "black-24.4.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665"},
+    {file = "black-24.4.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6"},
+    {file = "black-24.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e"},
+    {file = "black-24.4.0-cp39-cp39-win_amd64.whl", hash = "sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702"},
+    {file = "black-24.4.0-py3-none-any.whl", hash = "sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e"},
+    {file = "black-24.4.0.tar.gz", hash = "sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
+packaging = ">=22.0"
 pathspec = ">=0.9.0"
 platformdirs = ">=2"
-tomli = {version = ">=1.1.0", markers = "python_full_version < \"3.11.0a7\""}
-typed-ast = {version = ">=1.4.2", markers = "python_version < \"3.8\" and implementation_name == \"cpython\""}
-typing-extensions = {version = ">=3.10.0.0", markers = "python_version < \"3.10\""}
+tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
+typing-extensions = {version = ">=4.0.1", markers = "python_version < \"3.11\""}
 
 [package.extras]
 colorama = ["colorama (>=0.4.3)"]
-d = ["aiohttp (>=3.7.4)"]
+d = ["aiohttp (>=3.7.4)", "aiohttp (>=3.7.4,!=3.9.0)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "click"
 version = "8.1.7"
 description = "Composable command line interface toolkit"
@@ -45,62 +55,41 @@
 files = [
     {file = "click-8.1.7-py3-none-any.whl", hash = "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28"},
     {file = "click-8.1.7.tar.gz", hash = "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
-importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.2.0"
+version = "1.2.1"
 description = "Backport of PEP 654 (exception groups)"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.2.0-py3-none-any.whl", hash = "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14"},
-    {file = "exceptiongroup-1.2.0.tar.gz", hash = "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
-name = "importlib-metadata"
-version = "6.7.0"
-description = "Read metadata from Python packages"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
-    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
-]
-
-[package.dependencies]
-typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
-zipp = ">=0.5"
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-perf = ["ipython"]
-testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
-
-[[package]]
 name = "iniconfig"
 version = "2.0.0"
 description = "brain-dead simple config-ini parsing"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
@@ -134,54 +123,57 @@
 
 [package.extras]
 patchelf = ["patchelf"]
 zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
 name = "mypy"
-version = "0.981"
+version = "1.9.0"
 description = "Optional static typing for Python"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "mypy-0.981-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:4bc460e43b7785f78862dab78674e62ec3cd523485baecfdf81a555ed29ecfa0"},
-    {file = "mypy-0.981-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:756fad8b263b3ba39e4e204ee53042671b660c36c9017412b43af210ddee7b08"},
-    {file = "mypy-0.981-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a16a0145d6d7d00fbede2da3a3096dcc9ecea091adfa8da48fa6a7b75d35562d"},
-    {file = "mypy-0.981-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ce65f70b14a21fdac84c294cde75e6dbdabbcff22975335e20827b3b94bdbf49"},
-    {file = "mypy-0.981-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:6e35d764784b42c3e256848fb8ed1d4292c9fc0098413adb28d84974c095b279"},
-    {file = "mypy-0.981-cp310-cp310-win_amd64.whl", hash = "sha256:e53773073c864d5f5cec7f3fc72fbbcef65410cde8cc18d4f7242dea60dac52e"},
-    {file = "mypy-0.981-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:6ee196b1d10b8b215e835f438e06965d7a480f6fe016eddbc285f13955cca659"},
-    {file = "mypy-0.981-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8ad21d4c9d3673726cf986ea1d0c9fb66905258709550ddf7944c8f885f208be"},
-    {file = "mypy-0.981-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d1debb09043e1f5ee845fa1e96d180e89115b30e47c5d3ce53bc967bab53f62d"},
-    {file = "mypy-0.981-cp37-cp37m-win_amd64.whl", hash = "sha256:9f362470a3480165c4c6151786b5379351b790d56952005be18bdbdd4c7ce0ae"},
-    {file = "mypy-0.981-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:c9e0efb95ed6ca1654951bd5ec2f3fa91b295d78bf6527e026529d4aaa1e0c30"},
-    {file = "mypy-0.981-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e178eaffc3c5cd211a87965c8c0df6da91ed7d258b5fc72b8e047c3771317ddb"},
-    {file = "mypy-0.981-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:06e1eac8d99bd404ed8dd34ca29673c4346e76dd8e612ea507763dccd7e13c7a"},
-    {file = "mypy-0.981-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fa38f82f53e1e7beb45557ff167c177802ba7b387ad017eab1663d567017c8ee"},
-    {file = "mypy-0.981-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:64e1f6af81c003f85f0dfed52db632817dabb51b65c0318ffbf5ff51995bbb08"},
-    {file = "mypy-0.981-cp38-cp38-win_amd64.whl", hash = "sha256:e1acf62a8c4f7c092462c738aa2c2489e275ed386320c10b2e9bff31f6f7e8d6"},
-    {file = "mypy-0.981-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b6ede64e52257931315826fdbfc6ea878d89a965580d1a65638ef77cb551f56d"},
-    {file = "mypy-0.981-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:eb3978b191b9fa0488524bb4ffedf2c573340e8c2b4206fc191d44c7093abfb7"},
-    {file = "mypy-0.981-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:77f8fcf7b4b3cc0c74fb33ae54a4cd00bb854d65645c48beccf65fa10b17882c"},
-    {file = "mypy-0.981-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f64d2ce043a209a297df322eb4054dfbaa9de9e8738291706eaafda81ab2b362"},
-    {file = "mypy-0.981-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2ee3dbc53d4df7e6e3b1c68ac6a971d3a4fb2852bf10a05fda228721dd44fae1"},
-    {file = "mypy-0.981-cp39-cp39-win_amd64.whl", hash = "sha256:8e8e49aa9cc23aa4c926dc200ce32959d3501c4905147a66ce032f05cb5ecb92"},
-    {file = "mypy-0.981-py3-none-any.whl", hash = "sha256:794f385653e2b749387a42afb1e14c2135e18daeb027e0d97162e4b7031210f8"},
-    {file = "mypy-0.981.tar.gz", hash = "sha256:ad77c13037d3402fbeffda07d51e3f228ba078d1c7096a73759c9419ea031bf4"},
+    {file = "mypy-1.9.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f"},
+    {file = "mypy-1.9.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed"},
+    {file = "mypy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150"},
+    {file = "mypy-1.9.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374"},
+    {file = "mypy-1.9.0-cp310-cp310-win_amd64.whl", hash = "sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03"},
+    {file = "mypy-1.9.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3"},
+    {file = "mypy-1.9.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc"},
+    {file = "mypy-1.9.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129"},
+    {file = "mypy-1.9.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612"},
+    {file = "mypy-1.9.0-cp311-cp311-win_amd64.whl", hash = "sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3"},
+    {file = "mypy-1.9.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd"},
+    {file = "mypy-1.9.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6"},
+    {file = "mypy-1.9.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185"},
+    {file = "mypy-1.9.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913"},
+    {file = "mypy-1.9.0-cp312-cp312-win_amd64.whl", hash = "sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6"},
+    {file = "mypy-1.9.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b"},
+    {file = "mypy-1.9.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2"},
+    {file = "mypy-1.9.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e"},
+    {file = "mypy-1.9.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04"},
+    {file = "mypy-1.9.0-cp38-cp38-win_amd64.whl", hash = "sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89"},
+    {file = "mypy-1.9.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02"},
+    {file = "mypy-1.9.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4"},
+    {file = "mypy-1.9.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d"},
+    {file = "mypy-1.9.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf"},
+    {file = "mypy-1.9.0-cp39-cp39-win_amd64.whl", hash = "sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9"},
+    {file = "mypy-1.9.0-py3-none-any.whl", hash = "sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e"},
+    {file = "mypy-1.9.0.tar.gz", hash = "sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974"},
 ]
 
 [package.dependencies]
-mypy-extensions = ">=0.4.3"
+mypy-extensions = ">=1.0.0"
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
-typed-ast = {version = ">=1.4.0,<2", markers = "python_version < \"3.8\""}
-typing-extensions = ">=3.10"
+typing-extensions = ">=4.1.0"
 
 [package.extras]
 dmypy = ["psutil (>=4.0)"]
-python2 = ["typed-ast (>=1.4.0,<2)"]
+install-types = ["pip"]
+mypyc = ["setuptools (>=50)"]
 reports = ["lxml"]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 description = "Type system extensions for programs checked with the mypy type checker."
 optional = false
@@ -200,166 +192,95 @@
 files = [
     {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
     {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "pathspec"
-version = "0.11.2"
+version = "0.12.1"
 description = "Utility library for gitignore style pattern matching of file paths."
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "pathspec-0.11.2-py3-none-any.whl", hash = "sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20"},
-    {file = "pathspec-0.11.2.tar.gz", hash = "sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3"},
+    {file = "pathspec-0.12.1-py3-none-any.whl", hash = "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08"},
+    {file = "pathspec-0.12.1.tar.gz", hash = "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "4.0.0"
-description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
+version = "4.2.1"
+description = "A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`."
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "platformdirs-4.0.0-py3-none-any.whl", hash = "sha256:118c954d7e949b35437270383a3f2531e99dd93cf7ce4dc8340d3356d30f173b"},
-    {file = "platformdirs-4.0.0.tar.gz", hash = "sha256:cb633b2bcf10c51af60beb0ab06d2f1d69064b43abf4c185ca6b28865f3f9731"},
+    {file = "platformdirs-4.2.1-py3-none-any.whl", hash = "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"},
+    {file = "platformdirs-4.2.1.tar.gz", hash = "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf"},
 ]
 
-[package.dependencies]
-typing-extensions = {version = ">=4.7.1", markers = "python_version < \"3.8\""}
-
 [package.extras]
-docs = ["furo (>=2023.7.26)", "proselint (>=0.13)", "sphinx (>=7.1.1)", "sphinx-autodoc-typehints (>=1.24)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.4)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)"]
+docs = ["furo (>=2023.9.10)", "proselint (>=0.13)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.25.2)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)"]
+type = ["mypy (>=1.8)"]
 
 [[package]]
 name = "pluggy"
-version = "1.2.0"
+version = "1.5.0"
 description = "plugin and hook calling mechanisms for python"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
-    {file = "pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
-[package.dependencies]
-importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
-
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "pytest"
-version = "7.4.4"
+version = "8.1.1"
 description = "pytest: simple powerful testing with Python"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "pytest-7.4.4-py3-none-any.whl", hash = "sha256:b090cdf5ed60bf4c45261be03239c2c1c22df034fbffe691abe93cd80cea01d8"},
-    {file = "pytest-7.4.4.tar.gz", hash = "sha256:2cf0005922c6ace4a3e2ec8b4080eb0d9753fdc93107415332f50ce9e7994280"},
+    {file = "pytest-8.1.1-py3-none-any.whl", hash = "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7"},
+    {file = "pytest-8.1.1.tar.gz", hash = "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
-importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
 iniconfig = "*"
 packaging = "*"
-pluggy = ">=0.12,<2.0"
-tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
+pluggy = ">=1.4,<2.0"
+tomli = {version = ">=1", markers = "python_version < \"3.11\""}
 
 [package.extras]
-testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
+testing = ["argcomplete", "attrs (>=19.2)", "hypothesis (>=3.56)", "mock", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
-name = "typed-ast"
-version = "1.5.5"
-description = "a fork of Python 2 and 3 ast modules with type comment support"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "typed_ast-1.5.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4bc1efe0ce3ffb74784e06460f01a223ac1f6ab31c6bc0376a21184bf5aabe3b"},
-    {file = "typed_ast-1.5.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5f7a8c46a8b333f71abd61d7ab9255440d4a588f34a21f126bbfc95f6049e686"},
-    {file = "typed_ast-1.5.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:597fc66b4162f959ee6a96b978c0435bd63791e31e4f410622d19f1686d5e769"},
-    {file = "typed_ast-1.5.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d41b7a686ce653e06c2609075d397ebd5b969d821b9797d029fccd71fdec8e04"},
-    {file = "typed_ast-1.5.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:5fe83a9a44c4ce67c796a1b466c270c1272e176603d5e06f6afbc101a572859d"},
-    {file = "typed_ast-1.5.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d5c0c112a74c0e5db2c75882a0adf3133adedcdbfd8cf7c9d6ed77365ab90a1d"},
-    {file = "typed_ast-1.5.5-cp310-cp310-win_amd64.whl", hash = "sha256:e1a976ed4cc2d71bb073e1b2a250892a6e968ff02aa14c1f40eba4f365ffec02"},
-    {file = "typed_ast-1.5.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c631da9710271cb67b08bd3f3813b7af7f4c69c319b75475436fcab8c3d21bee"},
-    {file = "typed_ast-1.5.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b445c2abfecab89a932b20bd8261488d574591173d07827c1eda32c457358b18"},
-    {file = "typed_ast-1.5.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cc95ffaaab2be3b25eb938779e43f513e0e538a84dd14a5d844b8f2932593d88"},
-    {file = "typed_ast-1.5.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61443214d9b4c660dcf4b5307f15c12cb30bdfe9588ce6158f4a005baeb167b2"},
-    {file = "typed_ast-1.5.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6eb936d107e4d474940469e8ec5b380c9b329b5f08b78282d46baeebd3692dc9"},
-    {file = "typed_ast-1.5.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e48bf27022897577d8479eaed64701ecaf0467182448bd95759883300ca818c8"},
-    {file = "typed_ast-1.5.5-cp311-cp311-win_amd64.whl", hash = "sha256:83509f9324011c9a39faaef0922c6f720f9623afe3fe220b6d0b15638247206b"},
-    {file = "typed_ast-1.5.5-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:44f214394fc1af23ca6d4e9e744804d890045d1643dd7e8229951e0ef39429b5"},
-    {file = "typed_ast-1.5.5-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:118c1ce46ce58fda78503eae14b7664163aa735b620b64b5b725453696f2a35c"},
-    {file = "typed_ast-1.5.5-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be4919b808efa61101456e87f2d4c75b228f4e52618621c77f1ddcaae15904fa"},
-    {file = "typed_ast-1.5.5-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:fc2b8c4e1bc5cd96c1a823a885e6b158f8451cf6f5530e1829390b4d27d0807f"},
-    {file = "typed_ast-1.5.5-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:16f7313e0a08c7de57f2998c85e2a69a642e97cb32f87eb65fbfe88381a5e44d"},
-    {file = "typed_ast-1.5.5-cp36-cp36m-win_amd64.whl", hash = "sha256:2b946ef8c04f77230489f75b4b5a4a6f24c078be4aed241cfabe9cbf4156e7e5"},
-    {file = "typed_ast-1.5.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2188bc33d85951ea4ddad55d2b35598b2709d122c11c75cffd529fbc9965508e"},
-    {file = "typed_ast-1.5.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0635900d16ae133cab3b26c607586131269f88266954eb04ec31535c9a12ef1e"},
-    {file = "typed_ast-1.5.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:57bfc3cf35a0f2fdf0a88a3044aafaec1d2f24d8ae8cd87c4f58d615fb5b6311"},
-    {file = "typed_ast-1.5.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:fe58ef6a764de7b4b36edfc8592641f56e69b7163bba9f9c8089838ee596bfb2"},
-    {file = "typed_ast-1.5.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d09d930c2d1d621f717bb217bf1fe2584616febb5138d9b3e8cdd26506c3f6d4"},
-    {file = "typed_ast-1.5.5-cp37-cp37m-win_amd64.whl", hash = "sha256:d40c10326893ecab8a80a53039164a224984339b2c32a6baf55ecbd5b1df6431"},
-    {file = "typed_ast-1.5.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:fd946abf3c31fb50eee07451a6aedbfff912fcd13cf357363f5b4e834cc5e71a"},
-    {file = "typed_ast-1.5.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:ed4a1a42df8a3dfb6b40c3d2de109e935949f2f66b19703eafade03173f8f437"},
-    {file = "typed_ast-1.5.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:045f9930a1550d9352464e5149710d56a2aed23a2ffe78946478f7b5416f1ede"},
-    {file = "typed_ast-1.5.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:381eed9c95484ceef5ced626355fdc0765ab51d8553fec08661dce654a935db4"},
-    {file = "typed_ast-1.5.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:bfd39a41c0ef6f31684daff53befddae608f9daf6957140228a08e51f312d7e6"},
-    {file = "typed_ast-1.5.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8c524eb3024edcc04e288db9541fe1f438f82d281e591c548903d5b77ad1ddd4"},
-    {file = "typed_ast-1.5.5-cp38-cp38-win_amd64.whl", hash = "sha256:7f58fabdde8dcbe764cef5e1a7fcb440f2463c1bbbec1cf2a86ca7bc1f95184b"},
-    {file = "typed_ast-1.5.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:042eb665ff6bf020dd2243307d11ed626306b82812aba21836096d229fdc6a10"},
-    {file = "typed_ast-1.5.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:622e4a006472b05cf6ef7f9f2636edc51bda670b7bbffa18d26b255269d3d814"},
-    {file = "typed_ast-1.5.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1efebbbf4604ad1283e963e8915daa240cb4bf5067053cf2f0baadc4d4fb51b8"},
-    {file = "typed_ast-1.5.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0aefdd66f1784c58f65b502b6cf8b121544680456d1cebbd300c2c813899274"},
-    {file = "typed_ast-1.5.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:48074261a842acf825af1968cd912f6f21357316080ebaca5f19abbb11690c8a"},
-    {file = "typed_ast-1.5.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:429ae404f69dc94b9361bb62291885894b7c6fb4640d561179548c849f8492ba"},
-    {file = "typed_ast-1.5.5-cp39-cp39-win_amd64.whl", hash = "sha256:335f22ccb244da2b5c296e6f96b06ee9bed46526db0de38d2f0e5a6597b81155"},
-    {file = "typed_ast-1.5.5.tar.gz", hash = "sha256:94282f7a354f36ef5dbce0ef3467ebf6a258e370ab33d5b40c249fa996e590dd"},
-]
-
-[[package]]
 name = "typing-extensions"
-version = "4.7.1"
-description = "Backported and Experimental Type Hints for Python 3.7+"
+version = "4.11.0"
+description = "Backported and Experimental Type Hints for Python 3.8+"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
-    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
-[[package]]
-name = "zipp"
-version = "3.15.0"
-description = "Backport of pathlib-compatible object wrapper for zip files"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
-    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
-]
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
-
 [metadata]
 lock-version = "2.0"
-python-versions = ">=3.7"
-content-hash = "c109ad8e8b2f7f84f9c2be46a4fc121c3fc78ee69b87545063b28f052efdc54d"
+python-versions = ">=3.8"
+content-hash = "e118dc4af16e5de00387077e7c8aac5e644d5d58b600edb84472e462c165f249"
```

### Comparing `pyrevm-0.3.1/pyrevm.pyi` & `pyrevm-0.3.2/pyrevm.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,39 @@
     def prevrandao(self) -> Optional[bytes]: ...
     @property
     def basefee(self) -> Optional[int]: ...
     @property
     def gas_limit(self) -> Optional[int]: ...
     @property
     def excess_blob_gas(self) -> Optional[int]: ...
+    @property
+    def blob_gasprice(self) -> Optional[int]: ...
+    @number.setter
+    def number(self, value: Optional[int]) -> None: ...
+    @timestamp.setter
+    def timestamp(self, value: Optional[int]) -> None: ...
+    @excess_blob_gas.setter
+    def excess_blob_gas(self, value: Optional[int]) -> None: ...
 
 class TxEnv:
     def __new__(
         cls: Type["TxEnv"],
         caller: Optional[str] = None,
         gas_limit: Optional[int] = None,
         gas_price: Optional[int] = None,
         gas_priority_fee: Optional[int] = None,
         to: Optional[str] = None,
         value: Optional[int] = None,
         data: Optional[bytes] = None,
         chain_id: Optional[int] = None,
         nonce: Optional[int] = None,
         salt: Optional[int] = None,
+        access_list: Optional[list[tuple[str, list[int]]]] = None,
+        blob_hashes: Optional[list[bytes]] = None,
+        max_fee_per_blob_gas: Optional[int] = None,
     ) -> "TxEnv": ...
 
     @property
     def caller(self) -> Optional[str]: ...
     @property
     def gas_limit(self) -> Optional[int]: ...
     @property
@@ -63,14 +74,26 @@
     def value(self) -> Optional[int]: ...
     @property
     def data(self) -> Optional[bytes]: ...
     @property
     def chain_id(self) -> Optional[int]: ...
     @property
     def nonce(self) -> Optional[int]: ...
+    @property
+    def salt(self) -> Optional[int]: ...
+    @property
+    def access_list(self) -> list[tuple[str, list[int]]]: ...
+    @property
+    def blob_hashes(self) -> list[bytes]: ...
+    @property
+    def max_fee_per_blob_gas(self) -> Optional[int]: ...
+    @blob_hashes.setter
+    def blob_hashes(self, value: list[bytes]) -> None: ...
+    @max_fee_per_blob_gas.setter
+    def max_fee_per_blob_gas(self, value: Optional[int]) -> None: ...
 
 class Env:
     def __new__(
         cls: Type["Env"],
         cfg: Optional[CfgEnv] = None,
         block: Optional[BlockEnv] = None,
         tx: Optional[TxEnv] = None,
@@ -288,21 +311,27 @@
     @property
     def journal_state(self: "EVM") -> dict[str, AccountInfo]:
         """ The state in the journal. """
 
     def set_block_env(self: "EVM", block: BlockEnv) -> None:
         """ Set the block environment. """
 
+    def set_tx_env(self: "EVM", block: TxEnv) -> None:
+        """ Set the transaction environment. """
+
     def reset_transient_storage(self: "EVM") -> None:
         """ Reset the transient storage. """
 
 
 class Log:
     @property
     def address(self) -> str: ...
 
     @property
     def topics(self) -> list[str]: ...
 
     @property
     def data(self) -> tuple[list[bytes], bytes]:
         """ :return: A tuple with a list of topics and the log data. """
+
+
+def fake_exponential(factor: int, numerator: int, denominator: int) -> int: ...
```

### Comparing `pyrevm-0.3.1/pytest/contracts/full_math.bin` & `pyrevm-0.3.2/tests/fixtures/full_math.bin`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/pytest/contracts/weth_9.bin` & `pyrevm-0.3.2/tests/fixtures/weth_9.bin`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/pytest/test.py` & `pyrevm-0.3.2/tests/test_evm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 import json
-import os.path
+import os
 
+from pyrevm import EVM, Env, BlockEnv, AccountInfo, TxEnv
+
+from tests.utils import load_contract_bin, encode_uint, encode_address
 import pytest
-from pyrevm import EVM, Env, BlockEnv, AccountInfo
+
 
 address = "0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045"  # vitalik.eth
 address2 = "0xbBbBBBBbbBBBbbbBbbBbbbbBBbBbbbbBbBbbBBbB"
 
-fork_url = "https://mainnet.infura.io/v3/c60b0bb42f8a4c6481ecd229eddaca27"
+# use your own key during development to avoid rate limiting the CI job
+fork_url = os.getenv("FORK_URL") or "https://mainnet.infura.io/v3/c60b0bb42f8a4c6481ecd229eddaca27"
 
 KWARG_CASES = [
     {"fork_url": fork_url},
     {"fork_url": fork_url, "tracing": False, "fork_block": "latest"},
     {},
 ]
 
 
-def load_contract_bin(contract_name: str) -> bytes:
-    with open(
-        f"{os.path.dirname(__file__)}/contracts/{contract_name}", "r"
-    ) as readfile:
-        hexstring = readfile.readline()
-    return bytes.fromhex(hexstring)
-
-
-def encode_uint(num: int) -> str:
-    encoded = hex(num)[2:]
-    return ("0" * (64 - len(encoded))) + encoded
-
-
-def encode_address(address: str) -> str:
-    return f'{"0" * 24}{address[2:]}'
-
-
 def test_revm_fork():
     # set up an evm
     evm = EVM(
         # can fork from a remote node
         fork_url=fork_url,
         # can set tracing to true/false
         tracing=True,
@@ -208,18 +195,22 @@
         to=address,
         value=10000,
         calldata=bytes.fromhex("d0e30db0"),
     )
     assert evm.tracing
     captured = capsys.readouterr()
     traces = [json.loads(i) for i in captured.out.split("\n") if i]
-    assert {'gasUsed': '0xffffffffffff5011',
-            'output': '0x',
-            'pass': True,
-            'stateRoot': '0x0000000000000000000000000000000000000000000000000000000000000000'} == traces[-1]
+    expected = {
+        "fork": "Latest",
+        "gasUsed": "0xafee",
+        "output": "0x",
+        "pass": True,
+        "stateRoot": "0x0000000000000000000000000000000000000000000000000000000000000000",
+    }
+    assert expected == traces[-1]
     assert len(traces) == 128
 
 
 def test_blueprint():
     evm = EVM()
     # bytecode based on vyper `@external def foo() -> uint256: return 123`
     bytecode = load_contract_bin("blueprint.bin")
@@ -230,7 +221,62 @@
 
     # prepend a quick deploy preamble
     deploy_preamble = bytes.fromhex("61" + bytecode_len_hex + "3d81600a3d39f3")
     deploy_bytecode = deploy_preamble + bytecode
 
     deployer_address = evm.deploy(address, deploy_bytecode)
     assert evm.basic(deployer_address).code.hex().rstrip('0') in deploy_bytecode.hex()
+
+
+def test_block_setters():
+    evm = EVM()
+    block_env = evm.env.block
+    block_env.number = 20
+    block_env.timestamp = 100
+    block_env.excess_blob_gas = 200
+    assert block_env.number == 20
+    assert block_env.timestamp == 100
+    assert block_env.excess_blob_gas == 200
+    evm.set_block_env(block_env)
+    assert evm.env.block.number == 20
+
+
+def test_tx_setters():
+    evm = EVM()
+    tx_env = evm.env.tx
+    tx_env.blob_hashes = [b"1" * 32]
+    tx_env.max_fee_per_blob_gas = 100
+    assert tx_env.blob_hashes == [b"1" * 32]
+    assert tx_env.max_fee_per_blob_gas == 100
+    evm.set_tx_env(tx_env)
+    assert evm.env.tx.blob_hashes == [b"1" * 32]
+
+
+@pytest.mark.parametrize("excess_blob_gas,expected_fee", [(0, 1), (10**3, 1), (2**24, 152), (2**26, 537070730)])
+def test_get_blobbasefee(excess_blob_gas, expected_fee):
+    evm = EVM()
+    evm.set_block_env(BlockEnv(excess_blob_gas=excess_blob_gas))
+    bytecode = load_contract_bin("blob_base_fee.bin")
+    deployer_address = evm.deploy(address, bytecode)
+    blobbasefee = evm.message_call(
+        caller=address,
+        to=deployer_address,
+        calldata=bytes.fromhex("5fb0146d"),  # method_id("get_blobbasefee()")
+    )
+    assert int.from_bytes(blobbasefee, "big") == expected_fee
+
+
+@pytest.mark.parametrize("blob_hashes", [[b"1" * 32] * 2, [b"2" * 32] * 6])
+def test_get_blobhashes(blob_hashes):
+    evm = EVM()
+    evm.set_tx_env(TxEnv(blob_hashes=blob_hashes))
+    bytecode = load_contract_bin("blob_hash.bin")
+    deployer_address = evm.deploy(address, bytecode)
+    evm.message_call(
+        caller=address,
+        to=deployer_address,
+        calldata=bytes.fromhex("cc883ac4"),  # method_id("log_blobhashes()")
+    )
+    logged = [log.data[0][1] for log in evm.result.logs]
+
+    # the contract logs 6 blob hashes, so pad with 0s
+    assert logged == blob_hashes + [b"\0" * 32] * (6 - len(blob_hashes))
```

### Comparing `pyrevm-0.3.1/src/database.rs` & `pyrevm-0.3.2/src/database.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/src/empty_db_wrapper.rs` & `pyrevm-0.3.2/src/empty_db_wrapper.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/src/evm.rs` & `pyrevm-0.3.2/src/evm.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-use crate::database::DB;
-use crate::executor::call_evm;
-use crate::types::{PyByteVec, PyDB};
-use crate::{
-    types::{AccountInfo, BlockEnv, Env, ExecutionResult, JournalCheckpoint},
-    utils::{addr, pyerr},
-};
+use std::collections::{HashMap, HashSet};
+use std::fmt::Debug;
+use std::mem::replace;
+
 use pyo3::exceptions::{PyKeyError, PyOverflowError};
 use pyo3::types::PyBytes;
 use pyo3::{pyclass, pymethods, PyObject, PyResult, Python};
 use revm::precompile::{Address, Bytes};
 use revm::primitives::ExecutionResult::Success;
 use revm::primitives::{
     BlockEnv as RevmBlockEnv, CreateScheme, Env as RevmEnv, ExecutionResult as RevmExecutionResult,
-    HandlerCfg, Output, SpecId, TransactTo, TxEnv,
+    HandlerCfg, Output, SpecId, TransactTo, TxEnv as RevmTxEnv,
 };
 use revm::{primitives::U256, Evm, EvmContext, JournalCheckpoint as RevmCheckpoint};
-use std::collections::{HashMap, HashSet};
-use std::fmt::Debug;
-use std::mem::replace;
 use tracing::trace;
 
+use crate::database::DB;
+use crate::executor::call_evm;
+use crate::types::{PyByteVec, PyDB};
+use crate::{
+    types::{AccountInfo, BlockEnv, Env, ExecutionResult, JournalCheckpoint, TxEnv},
+    utils::{addr, pyerr},
+};
+
 #[derive(Debug)]
 #[pyclass]
 pub struct EVM {
     /// Context of execution.
     context: EvmContext<DB>,
 
     /// Handler configuration.
@@ -270,14 +272,18 @@
             .collect()
     }
 
     fn set_block_env(&mut self, block: BlockEnv) {
         self.context.env.block = block.into();
     }
 
+    fn set_tx_env(&mut self, tx: TxEnv) {
+        self.context.env.tx = tx.into();
+    }
+
     fn reset_transient_storage(&mut self) {
         self.context.journaled_state.transient_storage.clear();
     }
 
     fn __str__(&self) -> String {
         format!("{:?}", self)
     }
@@ -303,15 +309,15 @@
             // network conditions - the actual gas price is kept in `evm.block` and is applied by
             // the cheatcode handler if it is enabled
             block: RevmBlockEnv {
                 basefee: U256::ZERO,
                 gas_limit: self.gas_limit,
                 ..self.context.env.block.clone()
             },
-            tx: TxEnv {
+            tx: RevmTxEnv {
                 caller,
                 transact_to,
                 data,
                 value,
                 // As above, we set the gas price to 0.
                 gas_price: gas_price.unwrap_or(U256::ZERO),
                 gas_priority_fee: None,
```

### Comparing `pyrevm-0.3.1/src/executor.rs` & `pyrevm-0.3.2/src/executor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 pub(crate) fn call_evm(
     evm_context: EvmContext<DB>,
     handler_cfg: HandlerCfg,
     tracing: bool,
     is_static: bool,
 ) -> PyResult<(ExecutionResult, EvmContext<DB>)> {
     if tracing {
-        let tracer = TracerEip3155::new(Box::new(crate::pystdout::PySysStdout {}), true);
+        let tracer = TracerEip3155::new(Box::new(crate::pystdout::PySysStdout {}));
         let evm = Evm::builder()
             .with_context_with_handler_cfg(ContextWithHandlerCfg {
                 cfg: handler_cfg,
                 context: Context {
                     evm: evm_context,
                     external: tracer,
                 },
@@ -158,15 +158,15 @@
     context: &mut Context<EXT, DB>,
     result: FrameResult,
     logs: Vec<Log>,
 ) -> PyResult<ExecutionResult> {
     replace(&mut context.evm.error, Ok(())).map_err(pyerr)?;
     // used gas with refund calculated.
     let gas_refunded = result.gas().refunded() as u64;
-    let final_gas_used = result.gas().spend() - gas_refunded;
+    let final_gas_used = result.gas().spent() - gas_refunded;
     let output = result.output();
     let instruction_result = result.into_interpreter_result();
 
     let result = match instruction_result.result.into() {
         SuccessOrHalt::Success(reason) => ExecutionResult::Success {
             reason,
             gas_used: final_gas_used,
```

### Comparing `pyrevm-0.3.1/src/lib.rs` & `pyrevm-0.3.2/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 #![cfg_attr(not(test), warn(unused_crate_dependencies))]
 #![deny(unused_must_use, rust_2018_idioms)]
 #![cfg_attr(docsrs, feature(doc_cfg, doc_auto_cfg))]
 #![allow(clippy::too_many_arguments)]
 
 use pyo3::prelude::*;
 
-mod types;
-pub use types::*;
-
-mod evm;
-pub use evm::EVM;
-
 mod database;
 mod empty_db_wrapper;
+mod evm;
 mod executor;
 mod pystdout;
+mod types;
 mod utils;
 
+pub use evm::EVM;
+pub use types::*;
+pub use utils::fake_exponential;
+
 #[pymodule]
 fn pyrevm(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<EVM>()?;
 
     // Types
     m.add_class::<AccountInfo>()?;
     m.add_class::<Env>()?;
     m.add_class::<CfgEnv>()?;
     m.add_class::<TxEnv>()?;
     m.add_class::<BlockEnv>()?;
     m.add_class::<ExecutionResult>()?;
     m.add_class::<Log>()?;
     m.add_class::<JournalCheckpoint>()?;
+    m.add_function(wrap_pyfunction!(fake_exponential, m)?)?;
 
     Ok(())
 }
```

### Comparing `pyrevm-0.3.1/src/pystdout.rs` & `pyrevm-0.3.2/src/pystdout.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/src/types/evm_env.rs` & `pyrevm-0.3.2/src/types/evm_env.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-use crate::utils::{addr, addr_or_zero};
-use pyo3::{
-    exceptions::PyTypeError, pyclass, pymethods, types::PyBytes, PyObject, PyResult, Python,
-};
+use std::default::Default;
+
+use pyo3::types::PyTuple;
+use pyo3::{pyclass, pymethods, types::PyBytes, PyObject, PyResult, Python};
 use revm::primitives::{
-    BlobExcessGasAndPrice, BlockEnv as RevmBlockEnv, CfgEnv as RevmCfgEnv, CreateScheme,
+    Address, BlobExcessGasAndPrice, BlockEnv as RevmBlockEnv, CfgEnv as RevmCfgEnv, CreateScheme,
     Env as RevmEnv, TransactTo, TxEnv as RevmTxEnv, B256, U256,
 };
 
+use crate::utils::{addr, addr_or_zero, from_pybytes};
+
 #[pyclass]
 #[derive(Clone, Debug, Default)]
 pub struct Env(RevmEnv);
 
 #[pymethods]
 impl Env {
     #[new]
@@ -68,14 +70,17 @@
         gas_priority_fee: Option<U256>,
         to: Option<&str>,
         value: Option<U256>,
         data: Option<Vec<u8>>,
         chain_id: Option<u64>,
         nonce: Option<u64>,
         salt: Option<U256>,
+        access_list: Option<Vec<&PyTuple /*str, list[int]*/>>,
+        blob_hashes: Option<Vec<&PyBytes>>,
+        max_fee_per_blob_gas: Option<U256>,
     ) -> PyResult<Self> {
         Ok(TxEnv(RevmTxEnv {
             caller: addr_or_zero(caller)?,
             gas_limit: gas_limit.unwrap_or(u64::MAX),
             gas_price: gas_price.unwrap_or_default(),
             gas_priority_fee: gas_priority_fee.map(Into::into),
             transact_to: match to {
@@ -84,16 +89,30 @@
                     .map(TransactTo::create2)
                     .unwrap_or_else(TransactTo::create),
             },
             value: value.unwrap_or_default(),
             data: data.unwrap_or_default().into(),
             chain_id,
             nonce,
-            // TODO: Add access list.
-            ..Default::default()
+            access_list: access_list
+                .unwrap_or_default()
+                .iter()
+                .map(|tuple| {
+                    Ok((
+                        addr(tuple.get_item(0)?.extract()?)?,
+                        tuple.get_item(1)?.extract::<Vec<U256>>()?,
+                    ))
+                })
+                .collect::<PyResult<Vec<(Address, Vec<U256>)>>>()?,
+            blob_hashes: blob_hashes
+                .unwrap_or_default()
+                .iter()
+                .map(|b| from_pybytes(b))
+                .collect::<PyResult<Vec<B256>>>()?,
+            max_fee_per_blob_gas,
         }))
     }
 
     #[getter]
     fn caller(&self) -> String {
         self.0.caller.to_string()
     }
@@ -145,14 +164,51 @@
     fn salt(&self) -> Option<U256> {
         if let TransactTo::Create(CreateScheme::Create2 { salt }) = self.0.transact_to {
             return Some(salt);
         }
         None
     }
 
+    #[getter]
+    fn access_list(&self) -> Vec<(String, Vec<U256>)> {
+        self.0
+            .access_list
+            .iter()
+            .map(|(a, b)| (a.to_string(), b.clone()))
+            .collect()
+    }
+
+    #[getter]
+    fn blob_hashes(&self, py: Python<'_>) -> Vec<PyObject> {
+        self.0
+            .blob_hashes
+            .iter()
+            .map(|i| PyBytes::new(py, i.0.as_ref()).into())
+            .collect()
+    }
+
+    #[getter]
+    fn max_fee_per_blob_gas(&self) -> Option<U256> {
+        self.0.max_fee_per_blob_gas
+    }
+
+    #[setter]
+    fn set_blob_hashes(&mut self, blob_hashes: Vec<&PyBytes>) -> PyResult<()> {
+        self.0.blob_hashes = blob_hashes
+            .iter()
+            .map(|b| from_pybytes(b))
+            .collect::<PyResult<Vec<B256>>>()?;
+        Ok(())
+    }
+
+    #[setter]
+    fn set_max_fee_per_blob_gas(&mut self, max_fee_per_blob_gas: Option<U256>) {
+        self.0.max_fee_per_blob_gas = max_fee_per_blob_gas;
+    }
+
     fn __str__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self))
     }
 }
 
 impl From<TxEnv> for RevmTxEnv {
     fn from(env: TxEnv) -> Self {
@@ -179,26 +235,23 @@
         timestamp: Option<U256>,
         difficulty: Option<U256>,
         prevrandao: Option<&PyBytes>,
         basefee: Option<U256>,
         gas_limit: Option<U256>,
         excess_blob_gas: Option<u64>,
     ) -> PyResult<Self> {
-        let prevrandao = match prevrandao {
-            Some(b) => {
-                B256::try_from(b.as_bytes()).map_err(|e| PyTypeError::new_err(e.to_string()))?
-            }
-            None => B256::ZERO,
-        };
         Ok(BlockEnv(RevmBlockEnv {
             number: number.unwrap_or_default(),
             coinbase: addr_or_zero(coinbase)?,
             timestamp: timestamp.unwrap_or(U256::from(1)),
             difficulty: difficulty.unwrap_or_default(),
-            prevrandao: Some(prevrandao),
+            prevrandao: Some(match prevrandao {
+                Some(b) => from_pybytes(b)?,
+                None => B256::ZERO,
+            }),
             basefee: basefee.unwrap_or_default(),
             gas_limit: gas_limit.unwrap_or_else(|| U256::from(u64::MAX)),
             blob_excess_gas_and_price: Some(BlobExcessGasAndPrice::new(
                 excess_blob_gas.unwrap_or(0),
             )),
         }))
     }
@@ -244,14 +297,37 @@
     fn excess_blob_gas(&self) -> Option<u64> {
         self.0
             .blob_excess_gas_and_price
             .clone()
             .map(|i| i.excess_blob_gas)
     }
 
+    #[getter]
+    fn blob_gasprice(&self) -> Option<u128> {
+        self.0
+            .blob_excess_gas_and_price
+            .clone()
+            .map(|i| i.blob_gasprice)
+    }
+
+    #[setter]
+    fn set_number(&mut self, number: U256) {
+        self.0.number = number;
+    }
+
+    #[setter]
+    fn set_timestamp(&mut self, timestamp: U256) {
+        self.0.timestamp = timestamp;
+    }
+
+    #[setter]
+    fn set_excess_blob_gas(&mut self, excess_blob_gas: Option<u64>) {
+        self.0.blob_excess_gas_and_price = excess_blob_gas.map(BlobExcessGasAndPrice::new);
+    }
+
     fn __str__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self))
     }
 }
 
 impl From<BlockEnv> for RevmBlockEnv {
     fn from(env: BlockEnv) -> Self {
```

### Comparing `pyrevm-0.3.1/src/types/execution_result.rs` & `pyrevm-0.3.2/src/types/execution_result.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/src/types/info.rs` & `pyrevm-0.3.2/src/types/info.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.1/Cargo.lock` & `pyrevm-0.3.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "async_io_stream"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6d7b9decdf35d8908a7e3ef02f64c5e9b1695e230154c0e8de3969142d9b94c"
@@ -226,31 +226,31 @@
  "futures",
  "pharos",
  "rustc_version 0.4.0",
 ]
 
 [[package]]
 name = "aurora-engine-modexp"
-version = "1.0.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfacad86e9e138fca0670949eb8ed4ffdf73a55bded8887efe0863cd1a3a6f70"
+checksum = "0aef7712851e524f35fbbb74fa6599c5cd8692056a1c36f9ca0d2001b670e7e5"
 dependencies = [
  "hex",
  "num",
 ]
 
 [[package]]
 name = "auto_impl"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c87f3f15e7794432337fc718554eaa4dc8f04c9677a950ffe366f20a162ae42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -397,29 +397,29 @@
  "hex",
  "libc",
  "serde",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "const-hex"
 version = "1.11.3"
@@ -644,15 +644,15 @@
 name = "enumn"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -892,15 +892,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1492,15 +1492,15 @@
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
  "proc-macro-crate 3.1.0",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
@@ -1643,15 +1643,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -1724,17 +1724,17 @@
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
  "toml_edit 0.21.1",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proptest"
 version = "1.4.0"
@@ -1813,15 +1813,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyrevm"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "ethers-core",
  "ethers-providers",
  "pyo3",
  "revm",
  "revm-interpreter",
  "ruint",
@@ -1965,17 +1965,17 @@
  "web-sys",
  "webpki-roots",
  "winreg",
 ]
 
 [[package]]
 name = "revm"
-version = "7.2.0"
+version = "8.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24fd3ed4b62dc61c647552d8b781811ae25ec74d23309055077e4dfb392444d2"
+checksum = "72a454c1c650b2b2e23f0c461af09e6c31e1d15e1cbebe905a701c46b8a50afc"
 dependencies = [
  "auto_impl",
  "cfg-if",
  "dyn-clone",
  "ethers-core",
  "ethers-providers",
  "revm-interpreter",
@@ -1983,27 +1983,27 @@
  "serde",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "revm-interpreter"
-version = "3.4.0"
+version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f0a1818f8c876b0d71a0714217c34da7df8a42c0462750768779d55680e4554"
+checksum = "d322f2730cd300e99d271a1704a2dfb8973d832428f5aa282aaa40e2473b5eec"
 dependencies = [
  "revm-primitives",
  "serde",
 ]
 
 [[package]]
 name = "revm-precompile"
-version = "5.1.0"
+version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a9645a70f1df1e5bd7fa8718b9ba486fac9c3f0467aa6b58e7f590d5f6fd0f7"
+checksum = "931f692f3f4fc72ec39d5d270f8e9d208c4a6008de7590ee96cf948e3b6d3f8d"
 dependencies = [
  "aurora-engine-modexp",
  "c-kzg",
  "k256",
  "once_cell",
  "revm-primitives",
  "ripemd",
@@ -2163,30 +2163,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver 1.0.22",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
 dependencies = [
  "log",
  "ring 0.17.8",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2340,37 +2340,37 @@
 name = "send_wrapper"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd0b0ec5f1c1ca621c432a25813d8d60c88abe6d3e08a3eb9cf37d97a0fe3d73"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -2518,15 +2518,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "substrate-bn"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b5bbfa79abbae15dd642ea8176a21a635ff3c00059961d1ea27ad04e5b441c"
@@ -2553,17 +2553,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2615,30 +2615,30 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "threadpool"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
@@ -2722,15 +2722,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -2828,15 +2828,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3025,15 +3025,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3059,15 +3059,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3311,15 +3311,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
@@ -3331,9 +3331,9 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
```

### Comparing `pyrevm-0.3.1/pyproject.toml` & `pyrevm-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [tool.poetry]
 name = "pyrevm"
-version = "0.3.1"  # Cargo.toml needs to be updated for releases
+version = "0.3.2"  # Cargo.toml needs to be updated for releases
 description = "Python bindings to rust evm (revm)"
 authors = ["Georgios Konstantopoulos <me@gakonst.com>", "Dani Popes", "Daniel Schiavini", "Charles Cooper"]
 
 [tool.poetry.dependencies]
-python = ">=3.7"
-maturin = ">=1.5,<1.6"
-pytest = "^7.1.3"  # TODO: move this to test dependencies
+python = ">=3.8"
+maturin = "1.5.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8.0"
-mypy = "^0.981"
+black = "24.4.0"
+mypy = "1.9.0"
+pytest = "8.1.1"
 
 [build-system]
 requires = ["maturin>=1.5,<1.6"]
 build-backend = "maturin"
```

### Comparing `pyrevm-0.3.1/PKG-INFO` & `pyrevm-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrevm
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # <h1 align="center"> pyrevm </h1>
@@ -84,15 +84,15 @@
     value=...,
 )
 evm.revert(checkpoint)  # or: evm.commit() to clear all checkpoints
 ```
 
 **Note**: in contrast to the Rust library, the Python library does not automatically commit to database.
 
-See more usage examples in the [pytests](./pytest/test.py).
+See more usage examples in the [pytests](tests/test_evm.py).
 
 ## Develop
 
 We use Poetry for virtual environment management and [Maturin](https://github.com/PyO3/maturin) as our Rust <> Python FFI build system. The Rust bindings are auto-generated from the macros provided by [PyO3](https://pyo3.rs/v0.17.1/).
 
 To build the library, run `make build`. To run the tests, run `make test`.
```

