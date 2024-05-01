# Comparing `tmp/pydal2sql_core-0.3.6.tar.gz` & `tmp/pydal2sql_core-0.3.7.tar.gz`

## Comparing `pydal2sql_core-0.3.6.tar` & `pydal2sql_core-0.3.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/coverage.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/.github/workflows/su6.yml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/alter.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/examples.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/magic.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/settings_in_code.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    66916 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html
--rw-r--r--   0        0        0    71509 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0   104236 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html
--rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    27846 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0    93519 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
--rw-r--r--   0        0        0    96080 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___about___py.html
--rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___init___py.html
--rw-r--r--   0        0        0   271713 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_cli_support_py.html
--rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_core_py.html
--rw-r--r--   0        0        0    33315 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_helpers_py.html
--rw-r--r--   0        0        0    93963 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_magic_py.html
--rw-r--r--   0        0        0    31174 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/htmlcov/style.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/common.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_post.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_pre.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_with_function.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/magic_with_import.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/pydal_before.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/some_config.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pytest_examples/typedal_after.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/__about__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/__init__.py
--rw-r--r--   0        0        0    37107 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/cli_support.py
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/core.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/py.typed
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/src/pydal2sql_core/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/mock_git.py
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/test_cli_support.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/test_core.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/tests/test_helpers.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/README.md
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/coverage.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/examples/alter.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/examples/examples.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/examples/magic.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/examples/settings_in_code.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    66916 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html
+-rw-r--r--   0        0        0    71509 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0   104236 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html
+-rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    27846 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0    93519 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
+-rw-r--r--   0        0        0    96080 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660___about___py.html
+-rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660___init___py.html
+-rw-r--r--   0        0        0   271713 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_cli_support_py.html
+-rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_core_py.html
+-rw-r--r--   0        0        0    33315 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_helpers_py.html
+-rw-r--r--   0        0        0    93963 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_magic_py.html
+-rw-r--r--   0        0        0    31174 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/htmlcov/style.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/common.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/magic_post.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/magic_pre.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/magic_with_function.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/magic_with_import.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/pydal_before.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/some_config.toml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pytest_examples/typedal_after.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/__about__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/__init__.py
+-rw-r--r--   0        0        0    38335 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/cli_support.py
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/core.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/py.typed
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/src/pydal2sql_core/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/tests/mock_git.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/tests/test_cli_support.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/tests/test_core.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/tests/test_helpers.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/README.md
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 pydal2sql_core-0.3.7/PKG-INFO
```

### Comparing `pydal2sql_core-0.3.6/CHANGELOG.md` & `pydal2sql_core-0.3.7/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.7 (2024-05-01)
+
+### Fix
+
+* Allow indented blocks if magic ✨ is enabled ([`98d1955`](https://github.com/robinvandernoord/pydal2sql-core/commit/98d1955e29c9f457fec68c0b4c20de4f7d458ca5))
+
 ## v0.3.6 (2024-04-17)
 
 ### Fix
 
 * If 'default=' is a callable, it's result is NOT stored in the CREATE statement ([`3548347`](https://github.com/robinvandernoord/pydal2sql-core/commit/35483479c63986110e69dfd61a7d75ede15262be))
 
 ## v0.3.5 (2024-03-20)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydal2sql_core-0.3.6/coverage.svg` & `pydal2sql_core-0.3.7/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/examples/alter.py` & `pydal2sql_core-0.3.7/examples/alter.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/coverage_html.js` & `pydal2sql_core-0.3.7/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_cli_old_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_cli_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_typer_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___about___py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660___init___py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_cli_support_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_cli_support_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_core_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_helpers_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_magic_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_magic_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/d_ed2881eaa6b25660_types_py.html` & `pydal2sql_core-0.3.7/htmlcov/d_ed2881eaa6b25660_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/favicon_32.png` & `pydal2sql_core-0.3.7/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/index.html` & `pydal2sql_core-0.3.7/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/keybd_closed.png` & `pydal2sql_core-0.3.7/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/keybd_open.png` & `pydal2sql_core-0.3.7/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/status.json` & `pydal2sql_core-0.3.7/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/htmlcov/style.css` & `pydal2sql_core-0.3.7/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/pytest_examples/pydal_before.py` & `pydal2sql_core-0.3.7/pytest_examples/pydal_before.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/pytest_examples/typedal_after.py` & `pydal2sql_core-0.3.7/pytest_examples/typedal_after.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/src/pydal2sql_core/__init__.py` & `pydal2sql_core-0.3.7/src/pydal2sql_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/src/pydal2sql_core/cli_support.py` & `pydal2sql_core-0.3.7/src/pydal2sql_core/cli_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 CLI-Agnostic support.
 """
 
+import ast
 import contextlib
 import io
 import os
 import re
 import select
 import string
 import sys
@@ -343,16 +344,50 @@
     else:
         exists = False
         absolute_path = ""
 
     return exists, absolute_path
 
 
+def check_indentation(code: str, fix: bool = False) -> str:
+    """
+    Check the indentation of the given code.
+
+    This function attempts to parse the code using Python's built-in `ast.parse` function.
+    If the code is correctly indented, it is returned as is. If the code is incorrectly indented,
+    an `IndentationError` is raised. If the `fix` parameter is set to `True`, the function will
+    attempt to fix the indentation using `textwrap.dedent` before returning it.
+
+    Args:
+        code (str): The code to check.
+        fix (bool): Whether to fix the indentation if it is incorrect. Defaults to False.
+
+    Returns:
+        str: The original code if it is correctly indented,
+                or the fixed code if `fix` is True and the code was incorrectly indented.
+
+    Raises:
+        IndentationError: If the code is incorrectly indented and `fix` is False.
+    """
+    if not code:
+        # no code? perfect indentation!
+        return code
+
+    try:
+        ast.parse(code)
+        return code
+    except IndentationError as e:
+        if fix:
+            return textwrap.dedent(code)
+        else:
+            raise e
+
+
 def ensure_no_migrate_on_real_db(
-    code: str, db_names: typing.Iterable[str] = ("db", "database"), fix: typing.Optional[bool] = False
+    code: str, db_names: typing.Iterable[str] = ("db", "database"), fix: bool = False
 ) -> str:
     """
     Ensure that the code does not contain actual migrations on a real database.
 
     It does this by removing definitions of 'db' and database. This can be changed by customizing `db_names`.
     It also removes local imports to prevent irrelevant code being executed.
 
@@ -659,17 +694,17 @@
 
 
 def handle_cli(
     code_before: str,
     code_after: str,
     db_type: Optional[str] = None,
     tables: Optional[list[str] | list[list[str]]] = None,
-    verbose: Optional[bool] = False,
-    noop: Optional[bool] = False,
-    magic: Optional[bool] = False,
+    verbose: bool = False,
+    noop: bool = False,
+    magic: bool = False,
     function_name: Optional[str | tuple[str, ...]] = "define_tables",
     use_typedal: bool | typing.Literal["auto"] = "auto",
     output_format: SUPPORTED_OUTPUT_FORMATS = DEFAULT_OUTPUT_FORMAT,
     output_file: Optional[str | Path | io.StringIO] = None,
 ) -> bool:
     """
     Handle user input for generating SQL migration statements based on before and after code.
@@ -701,16 +736,20 @@
     else:
         define_table_functions = set()
 
     template = TEMPLATE_TYPEDAL if use_typedal else TEMPLATE_PYDAL
 
     to_execute = string.Template(textwrap.dedent(template))
 
+    code_before = check_indentation(code_before, fix=magic)
     code_before = ensure_no_migrate_on_real_db(code_before, fix=magic)
+
+    code_after = check_indentation(code_after, fix=magic)
     code_after = ensure_no_migrate_on_real_db(code_after, fix=magic)
+
     extra_code = ""
 
     generated_code = to_execute.substitute(
         {
             "tables": flatten(tables or []),
             "db_type": db_type or "",
             "code_before": textwrap.dedent(code_before),
```

### Comparing `pydal2sql_core-0.3.6/src/pydal2sql_core/core.py` & `pydal2sql_core-0.3.7/src/pydal2sql_core/core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/src/pydal2sql_core/helpers.py` & `pydal2sql_core-0.3.7/src/pydal2sql_core/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/src/pydal2sql_core/types.py` & `pydal2sql_core-0.3.7/src/pydal2sql_core/types.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/tests/mock_git.py` & `pydal2sql_core-0.3.7/tests/mock_git.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/tests/test_cli_support.py` & `pydal2sql_core-0.3.7/tests/test_cli_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import contextlib
 import io
 import os
 import shutil
+import sys
 import tempfile
 import textwrap
 from pathlib import Path
 
 import pytest
 from contextlib_chdir import chdir
 
@@ -466,7 +468,36 @@
     )
     buffer.seek(0)
 
     contents = buffer.read()
 
     assert "CREATE" not in contents
     assert "ALTER" in contents
+
+
+@contextlib.contextmanager
+def fake_stdin(data: str):
+    _stdin = sys.stdin
+    try:
+        with tempfile.NamedTemporaryFile(mode='w+t') as tmp:
+            tmp.write(data)
+            tmp.seek(0)
+            sys.stdin = tmp
+            yield
+    finally:
+        sys.stdin = _stdin
+
+
+def test_indent():
+    with fake_stdin("    raise ValueError('')"):
+        with pytest.raises(IndentationError):
+            core_create()
+
+    with fake_stdin("    raise ValueError('')"):
+        assert not core_create(magic=True)
+
+    with fake_stdin("""
+        
+                        db.define_table("empty")
+        
+                    """):
+        assert core_create(magic=True, db_type="sqlite")
```

### Comparing `pydal2sql_core-0.3.6/tests/test_core.py` & `pydal2sql_core-0.3.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/tests/test_helpers.py` & `pydal2sql_core-0.3.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/LICENSE.txt` & `pydal2sql_core-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/README.md` & `pydal2sql_core-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pydal2sql_core-0.3.6/pyproject.toml` & `pydal2sql_core-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,17 @@
 # check_untyped_defs = True
 
 exclude = ["venv", ".bak"]
 
 [tool.ruff]
 target-version = "py310"
 line-length = 120
+extend-exclude = ["*.bak/", "venv*/"]
 
+[tool.ruff.lint]
 select = [
     "F", # pyflake error
     "E", # pycodestyle error
     "W", # pycodestyle warning
     "Q", # quotes
     "A", # builtins
     # "C4", # comprehensions - NO: doesn't allow dict()
@@ -149,15 +151,14 @@
     "F401",
 ]
 extend-ignore = [
     # db.field == None should NOT be fixed to db.field is None
     "E711",
 ]
 
-extend-exclude = ["*.bak/", "venv*/"]
 
 ignore = [
     "RUF013", # implicit optional
     "RUF012",  # ClassVar
 ]
 
 [tool.bandit]
```

### Comparing `pydal2sql_core-0.3.6/PKG-INFO` & `pydal2sql_core-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql-core
-Version: 0.3.6
+Version: 0.3.7
 Summary: CLI-agnostic pydal2sql code; Convert pydal define_tables to SQL using pydal's CREATE TABLE logic.
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql-core#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql-core/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql-core
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

