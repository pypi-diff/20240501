# Comparing `tmp/rython_calc-0.4.8.tar.gz` & `tmp/rython_calc-0.4.9.tar.gz`

## Comparing `rython_calc-0.4.8.tar` & `rython_calc-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 rython_calc-0.4.8/Cargo.toml
--rw-r--r--   0     1001      127      367 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.github/dependabot.yml
--rw-r--r--   0     1001      127     4975 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.gitignore
--rw-r--r--   0     1001      127      949 2024-04-13 16:13:25.000000 rython_calc-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1075 2024-04-13 16:13:25.000000 rython_calc-0.4.8/LICENSE
--rw-r--r--   0     1001      127      603 2024-04-13 16:13:25.000000 rython_calc-0.4.8/README.md
--rw-r--r--   0     1001      127    29590 2024-04-13 16:13:25.000000 rython_calc-0.4.8/poetry.lock
--rw-r--r--   0     1001      127        0 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/cli/__init__.py
--rw-r--r--   0     1001      127     1744 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/cli/main.py
--rw-r--r--   0     1001      127      443 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/cli/performance.txt
--rw-r--r--   0     1001      127        0 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/rython/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/rython/py.typed
--rw-r--r--   0     1001      127      694 2024-04-13 16:13:25.000000 rython_calc-0.4.8/python/rython/rython_calc.pyi
--rw-r--r--   0     1001      127     3030 2024-04-13 16:13:25.000000 rython_calc-0.4.8/src/lib.rs
--rw-r--r--   0     1001      127      350 2024-04-13 16:13:25.000000 rython_calc-0.4.8/test/rython/test_rython_calc.py
--rw-r--r--   0     1001      127    12301 2024-04-13 16:13:25.000000 rython_calc-0.4.8/Cargo.lock
--rw-r--r--   0     1001      127     1685 2024-04-13 16:13:25.000000 rython_calc-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 rython_calc-0.4.9/Cargo.toml
+-rw-r--r--   0     1001      127      367 2024-05-01 19:29:01.000000 rython_calc-0.4.9/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4975 2024-05-01 19:29:01.000000 rython_calc-0.4.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-01 19:29:01.000000 rython_calc-0.4.9/.gitignore
+-rw-r--r--   0     1001      127      949 2024-05-01 19:29:01.000000 rython_calc-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1075 2024-05-01 19:29:01.000000 rython_calc-0.4.9/LICENSE
+-rw-r--r--   0     1001      127      603 2024-05-01 19:29:01.000000 rython_calc-0.4.9/README.md
+-rw-r--r--   0     1001      127    29642 2024-05-01 19:29:01.000000 rython_calc-0.4.9/poetry.lock
+-rw-r--r--   0     1001      127        0 2024-05-01 19:29:01.000000 rython_calc-0.4.9/python/cli/__init__.py
+-rw-r--r--   0     1001      127     1744 2024-05-01 19:29:01.000000 rython_calc-0.4.9/python/cli/main.py
+-rw-r--r--   0     1001      127      443 2024-05-01 19:29:01.000000 rython_calc-0.4.9/python/cli/performance.txt
+-rw-r--r--   0     1001      127        0 2024-05-01 19:29:01.000000 rython_calc-0.4.9/python/rython/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-01 19:29:01.000000 rython_calc-0.4.9/python/rython/py.typed
+-rw-r--r--   0     1001      127      694 2024-05-01 19:29:01.000000 rython_calc-0.4.9/python/rython/rython_calc.pyi
+-rw-r--r--   0     1001      127     3030 2024-05-01 19:29:01.000000 rython_calc-0.4.9/src/lib.rs
+-rw-r--r--   0     1001      127      350 2024-05-01 19:29:01.000000 rython_calc-0.4.9/test/rython/test_rython_calc.py
+-rw-r--r--   0     1001      127    12301 2024-05-01 19:29:01.000000 rython_calc-0.4.9/Cargo.lock
+-rw-r--r--   0     1001      127     1686 2024-05-01 19:29:01.000000 rython_calc-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.9/PKG-INFO
```

### Comparing `rython_calc-0.4.8/.github/workflows/CI.yml` & `rython_calc-0.4.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/.gitignore` & `rython_calc-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/.pre-commit-config.yaml` & `rython_calc-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/LICENSE` & `rython_calc-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/README.md` & `rython_calc-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/poetry.lock` & `rython_calc-0.4.9/poetry.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "black"
-version = "24.4.0"
+version = "24.4.2"
 description = "The uncompromising code formatter."
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "black-24.4.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436"},
-    {file = "black-24.4.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf"},
-    {file = "black-24.4.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad"},
-    {file = "black-24.4.0-cp310-cp310-win_amd64.whl", hash = "sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb"},
-    {file = "black-24.4.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8"},
-    {file = "black-24.4.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745"},
-    {file = "black-24.4.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070"},
-    {file = "black-24.4.0-cp311-cp311-win_amd64.whl", hash = "sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397"},
-    {file = "black-24.4.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2"},
-    {file = "black-24.4.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33"},
-    {file = "black-24.4.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965"},
-    {file = "black-24.4.0-cp312-cp312-win_amd64.whl", hash = "sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd"},
-    {file = "black-24.4.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1"},
-    {file = "black-24.4.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8"},
-    {file = "black-24.4.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d"},
-    {file = "black-24.4.0-cp38-cp38-win_amd64.whl", hash = "sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3"},
-    {file = "black-24.4.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665"},
-    {file = "black-24.4.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6"},
-    {file = "black-24.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e"},
-    {file = "black-24.4.0-cp39-cp39-win_amd64.whl", hash = "sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702"},
-    {file = "black-24.4.0-py3-none-any.whl", hash = "sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e"},
-    {file = "black-24.4.0.tar.gz", hash = "sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641"},
+    {file = "black-24.4.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:dd1b5a14e417189db4c7b64a6540f31730713d173f0b63e55fabd52d61d8fdce"},
+    {file = "black-24.4.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8e537d281831ad0e71007dcdcbe50a71470b978c453fa41ce77186bbe0ed6021"},
+    {file = "black-24.4.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eaea3008c281f1038edb473c1aa8ed8143a5535ff18f978a318f10302b254063"},
+    {file = "black-24.4.2-cp310-cp310-win_amd64.whl", hash = "sha256:7768a0dbf16a39aa5e9a3ded568bb545c8c2727396d063bbaf847df05b08cd96"},
+    {file = "black-24.4.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:257d724c2c9b1660f353b36c802ccece186a30accc7742c176d29c146df6e474"},
+    {file = "black-24.4.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:bdde6f877a18f24844e381d45e9947a49e97933573ac9d4345399be37621e26c"},
+    {file = "black-24.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e151054aa00bad1f4e1f04919542885f89f5f7d086b8a59e5000e6c616896ffb"},
+    {file = "black-24.4.2-cp311-cp311-win_amd64.whl", hash = "sha256:7e122b1c4fb252fd85df3ca93578732b4749d9be076593076ef4d07a0233c3e1"},
+    {file = "black-24.4.2-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:accf49e151c8ed2c0cdc528691838afd217c50412534e876a19270fea1e28e2d"},
+    {file = "black-24.4.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:88c57dc656038f1ab9f92b3eb5335ee9b021412feaa46330d5eba4e51fe49b04"},
+    {file = "black-24.4.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be8bef99eb46d5021bf053114442914baeb3649a89dc5f3a555c88737e5e98fc"},
+    {file = "black-24.4.2-cp312-cp312-win_amd64.whl", hash = "sha256:415e686e87dbbe6f4cd5ef0fbf764af7b89f9057b97c908742b6008cc554b9c0"},
+    {file = "black-24.4.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bf10f7310db693bb62692609b397e8d67257c55f949abde4c67f9cc574492cc7"},
+    {file = "black-24.4.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:98e123f1d5cfd42f886624d84464f7756f60ff6eab89ae845210631714f6db94"},
+    {file = "black-24.4.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:48a85f2cb5e6799a9ef05347b476cce6c182d6c71ee36925a6c194d074336ef8"},
+    {file = "black-24.4.2-cp38-cp38-win_amd64.whl", hash = "sha256:b1530ae42e9d6d5b670a34db49a94115a64596bc77710b1d05e9801e62ca0a7c"},
+    {file = "black-24.4.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:37aae07b029fa0174d39daf02748b379399b909652a806e5708199bd93899da1"},
+    {file = "black-24.4.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:da33a1a5e49c4122ccdfd56cd021ff1ebc4a1ec4e2d01594fef9b6f267a9e741"},
+    {file = "black-24.4.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef703f83fc32e131e9bcc0a5094cfe85599e7109f896fe8bc96cc402f3eb4b6e"},
+    {file = "black-24.4.2-cp39-cp39-win_amd64.whl", hash = "sha256:b9176b9832e84308818a99a561e90aa479e73c523b3f77afd07913380ae2eab7"},
+    {file = "black-24.4.2-py3-none-any.whl", hash = "sha256:d36ed1124bb81b32f8614555b34cc4259c3fbc7eec17870e8ff8ded335b58d8c"},
+    {file = "black-24.4.2.tar.gz", hash = "sha256:c872b53057f000085da66a19c55d68f6f8ddcac2642392ad3a355878406fbd4d"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
 packaging = ">=22.0"
 pathspec = ">=0.9.0"
@@ -89,37 +89,37 @@
 files = [
     {file = "distlib-0.3.8-py2.py3-none-any.whl", hash = "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784"},
     {file = "distlib-0.3.8.tar.gz", hash = "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"},
 ]
 
 [[package]]
 name = "filelock"
-version = "3.13.4"
+version = "3.14.0"
 description = "A platform independent file lock."
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "filelock-3.13.4-py3-none-any.whl", hash = "sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f"},
-    {file = "filelock-3.13.4.tar.gz", hash = "sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4"},
+    {file = "filelock-3.14.0-py3-none-any.whl", hash = "sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f"},
+    {file = "filelock-3.14.0.tar.gz", hash = "sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.9.10)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.25.2)"]
 testing = ["covdefaults (>=2.3)", "coverage (>=7.3.2)", "diff-cover (>=8.0.1)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)", "pytest-timeout (>=2.2)"]
 typing = ["typing-extensions (>=4.8)"]
 
 [[package]]
 name = "identify"
-version = "2.5.35"
+version = "2.5.36"
 description = "File identification library for Python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "identify-2.5.35-py2.py3-none-any.whl", hash = "sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e"},
-    {file = "identify-2.5.35.tar.gz", hash = "sha256:10a7ca245cfcd756a554a7288159f72ff105ad233c7c4b9c6f0f4d108f5f6791"},
+    {file = "identify-2.5.36-py2.py3-none-any.whl", hash = "sha256:37d93f380f4de590500d9dba7db359d0d3da95ffe7f9de1753faa159e71e7dfa"},
+    {file = "identify-2.5.36.tar.gz", hash = "sha256:e5e00f54165f9047fbebeb4a560f9acfb8af4c88232be60a488e9b68d122745d"},
 ]
 
 [package.extras]
 license = ["ukkonen"]
 
 [[package]]
 name = "iniconfig"
@@ -170,46 +170,46 @@
 
 [package.extras]
 patchelf = ["patchelf"]
 zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
 name = "mypy"
-version = "1.9.0"
+version = "1.10.0"
 description = "Optional static typing for Python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "mypy-1.9.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f"},
-    {file = "mypy-1.9.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed"},
-    {file = "mypy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150"},
-    {file = "mypy-1.9.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374"},
-    {file = "mypy-1.9.0-cp310-cp310-win_amd64.whl", hash = "sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03"},
-    {file = "mypy-1.9.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3"},
-    {file = "mypy-1.9.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc"},
-    {file = "mypy-1.9.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129"},
-    {file = "mypy-1.9.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612"},
-    {file = "mypy-1.9.0-cp311-cp311-win_amd64.whl", hash = "sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3"},
-    {file = "mypy-1.9.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd"},
-    {file = "mypy-1.9.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6"},
-    {file = "mypy-1.9.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185"},
-    {file = "mypy-1.9.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913"},
-    {file = "mypy-1.9.0-cp312-cp312-win_amd64.whl", hash = "sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6"},
-    {file = "mypy-1.9.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b"},
-    {file = "mypy-1.9.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2"},
-    {file = "mypy-1.9.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e"},
-    {file = "mypy-1.9.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04"},
-    {file = "mypy-1.9.0-cp38-cp38-win_amd64.whl", hash = "sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89"},
-    {file = "mypy-1.9.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02"},
-    {file = "mypy-1.9.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4"},
-    {file = "mypy-1.9.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d"},
-    {file = "mypy-1.9.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf"},
-    {file = "mypy-1.9.0-cp39-cp39-win_amd64.whl", hash = "sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9"},
-    {file = "mypy-1.9.0-py3-none-any.whl", hash = "sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e"},
-    {file = "mypy-1.9.0.tar.gz", hash = "sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99"},
+    {file = "mypy-1.10.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2"},
+    {file = "mypy-1.10.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9"},
+    {file = "mypy-1.10.0-cp310-cp310-win_amd64.whl", hash = "sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee"},
+    {file = "mypy-1.10.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de"},
+    {file = "mypy-1.10.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7"},
+    {file = "mypy-1.10.0-cp311-cp311-win_amd64.whl", hash = "sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30"},
+    {file = "mypy-1.10.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e"},
+    {file = "mypy-1.10.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5"},
+    {file = "mypy-1.10.0-cp312-cp312-win_amd64.whl", hash = "sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727"},
+    {file = "mypy-1.10.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4"},
+    {file = "mypy-1.10.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061"},
+    {file = "mypy-1.10.0-cp38-cp38-win_amd64.whl", hash = "sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec"},
+    {file = "mypy-1.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821"},
+    {file = "mypy-1.10.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746"},
+    {file = "mypy-1.10.0-cp39-cp39-win_amd64.whl", hash = "sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a"},
+    {file = "mypy-1.10.0-py3-none-any.whl", hash = "sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee"},
+    {file = "mypy-1.10.0.tar.gz", hash = "sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131"},
 ]
 
 [package.dependencies]
 mypy-extensions = ">=1.0.0"
 typing-extensions = ">=4.1.0"
 
 [package.extras]
@@ -263,36 +263,37 @@
 files = [
     {file = "pathspec-0.12.1-py3-none-any.whl", hash = "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08"},
     {file = "pathspec-0.12.1.tar.gz", hash = "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "4.2.0"
-description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
+version = "4.2.1"
+description = "A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`."
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "platformdirs-4.2.0-py3-none-any.whl", hash = "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068"},
-    {file = "platformdirs-4.2.0.tar.gz", hash = "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"},
+    {file = "platformdirs-4.2.1-py3-none-any.whl", hash = "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"},
+    {file = "platformdirs-4.2.1.tar.gz", hash = "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.9.10)", "proselint (>=0.13)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.25.2)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)"]
+type = ["mypy (>=1.8)"]
 
 [[package]]
 name = "pluggy"
-version = "1.4.0"
+version = "1.5.0"
 description = "plugin and hook calling mechanisms for python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "pluggy-1.4.0-py3-none-any.whl", hash = "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981"},
-    {file = "pluggy-1.4.0.tar.gz", hash = "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
@@ -311,31 +312,31 @@
 identify = ">=1.0.0"
 nodeenv = ">=0.11.1"
 pyyaml = ">=5.1"
 virtualenv = ">=20.10.0"
 
 [[package]]
 name = "pytest"
-version = "8.1.1"
+version = "8.2.0"
 description = "pytest: simple powerful testing with Python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "pytest-8.1.1-py3-none-any.whl", hash = "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7"},
-    {file = "pytest-8.1.1.tar.gz", hash = "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"},
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 iniconfig = "*"
 packaging = "*"
-pluggy = ">=1.4,<2.0"
+pluggy = ">=1.5,<2.0"
 
 [package.extras]
-testing = ["argcomplete", "attrs (>=19.2)", "hypothesis (>=3.56)", "mock", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
+dev = ["argcomplete", "attrs (>=19.2)", "hypothesis (>=3.56)", "mock", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "pyyaml"
 version = "6.0.1"
 description = "YAML parser and emitter for Python"
 optional = false
 python-versions = ">=3.6"
@@ -391,21 +392,21 @@
     {file = "PyYAML-6.0.1-cp39-cp39-win32.whl", hash = "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c"},
     {file = "PyYAML-6.0.1-cp39-cp39-win_amd64.whl", hash = "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486"},
     {file = "PyYAML-6.0.1.tar.gz", hash = "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43"},
 ]
 
 [[package]]
 name = "setuptools"
-version = "69.5.0"
+version = "69.5.1"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "setuptools-69.5.0-py3-none-any.whl", hash = "sha256:3b2dbd8f63dcc6b7c327d0243c2d7dc8c96cc507c016f09221f3787e6e528719"},
-    {file = "setuptools-69.5.0.tar.gz", hash = "sha256:8d881f842bfc0e29e93bc98a2e650e8845609adff4d2989ba6c748e67b09d5be"},
+    {file = "setuptools-69.5.1-py3-none-any.whl", hash = "sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32"},
+    {file = "setuptools-69.5.1.tar.gz", hash = "sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9.3)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (>=1,<2)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
 testing = ["build[virtualenv]", "filelock (>=3.4.0)", "importlib-metadata", "ini2toml[lite] (>=0.9)", "jaraco.develop (>=7.21)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "mypy (==1.9)", "packaging (>=23.2)", "pip (>=19.1)", "pytest (>=6,!=8.1.1)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=2.2)", "pytest-home (>=0.5)", "pytest-mypy", "pytest-perf", "pytest-ruff (>=0.2.1)", "pytest-timeout", "pytest-xdist (>=3)", "tomli", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv] (>=1.0.3)", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "packaging (>=23.2)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
@@ -418,29 +419,29 @@
 files = [
     {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
     {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "virtualenv"
-version = "20.25.1"
+version = "20.26.1"
 description = "Virtual Python Environment builder"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "virtualenv-20.25.1-py3-none-any.whl", hash = "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a"},
-    {file = "virtualenv-20.25.1.tar.gz", hash = "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"},
+    {file = "virtualenv-20.26.1-py3-none-any.whl", hash = "sha256:7aa9982a728ae5892558bff6a2839c00b9ed145523ece2274fad6f414690ae75"},
+    {file = "virtualenv-20.26.1.tar.gz", hash = "sha256:604bfdceaeece392802e6ae48e69cec49168b9c5f4a44e483963f9242eb0e78b"},
 ]
 
 [package.dependencies]
 distlib = ">=0.3.7,<1"
 filelock = ">=3.12.2,<4"
 platformdirs = ">=3.9.1,<5"
 
 [package.extras]
-docs = ["furo (>=2023.7.26)", "proselint (>=0.13)", "sphinx (>=7.1.2)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
+docs = ["furo (>=2023.7.26)", "proselint (>=0.13)", "sphinx (>=7.1.2,!=7.3)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
 test = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23.1)", "pytest (>=7.4)", "pytest-env (>=0.8.2)", "pytest-freezer (>=0.4.8)", "pytest-mock (>=3.11.1)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)", "setuptools (>=68)", "time-machine (>=2.10)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.12"
-content-hash = "b5fbd43e96e2a6795ff41b5f852fb1aada5d1f2d2412048c22946fd6ef86ac17"
+content-hash = "a2a058fc4c3408f467b47c016d0c7c6d08dedd6492b46b8e0390310e1395b9b5"
```

### Comparing `rython_calc-0.4.8/python/cli/main.py` & `rython_calc-0.4.9/python/cli/main.py`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/python/rython/rython_calc.pyi` & `rython_calc-0.4.9/python/rython/rython_calc.pyi`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/src/lib.rs` & `rython_calc-0.4.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.8/Cargo.lock` & `rython_calc-0.4.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
  "blake2b_simd",
  "constant_time_eq",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "rython"
-version = "0.4.8"
+version = "0.4.9"
 dependencies = [
  "check",
  "clippy",
  "fmt",
  "pyo3",
 ]
```

### Comparing `rython_calc-0.4.8/pyproject.toml` & `rython_calc-0.4.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rython_calc"
 requires-python = ">=3.12"
-version = "0.4.8"
+version = "0.4.9"
 description = "Small project developed by me to learn PyO3 library."
 authors = [
     {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
 ]
 maintainers = [
     {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
 ]
@@ -31,15 +31,15 @@
 python-source = "python"
 bindings = "pyo3"
 module-name = "rython.rython_calc"
 strip = true
 
 [tool.poetry]
 name = "rython_calc"
-version = "0.4.8"
+version = "0.4.9"
 description = "Small project developed by me to learn PyO3 library."
 authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 maintainers = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -49,15 +49,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.group.dev.dependencies]
 maturin = "^1.5.1"
-pytest = "^8.1.1"
-mypy = "^1.9.0"
+pytest = "^8.2.0"
+mypy = "^1.10.0"
 isort = "^5.13.2"
-black = "^24.4.0"
+black = "^24.4.2"
 pre-commit = "^3.7.0"
 
 [tool.isort]
 profile = "black"
```

### Comparing `rython_calc-0.4.8/PKG-INFO` & `rython_calc-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rython_calc
-Version: 0.4.8
+Version: 0.4.9
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Small project developed by me to learn PyO3 library.
 Author-email: Krystian Krakowski <kkrakowski22@gmail.com>
```

