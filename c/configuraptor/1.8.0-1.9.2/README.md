# Comparing `tmp/configuraptor-1.8.0.tar.gz` & `tmp/configuraptor-1.9.2.tar.gz`

## Comparing `configuraptor-1.8.0.tar` & `configuraptor-1.9.2.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 configuraptor-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.8.0/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.8.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/ages.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dataclass.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dumping.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dumping.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/existing_instance.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/main.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/postponed.py
--rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/readme.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    26392 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   131736 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
--rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/__init__.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/core.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/dump.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/helpers.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/postpone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_about.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_core.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_dumps.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_mypy.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_postponed.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_existing.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.8.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.8.0/README.md
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 configuraptor-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 configuraptor-1.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.9.2/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.9.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/dataclass.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/dumping.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/dumping.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_mapping.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/main.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/postponed.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/readme.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    48825 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   137212 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
+-rw-r--r--   0        0        0    34632 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
+-rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/dump.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/postpone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_about.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_core.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_dumps.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_mypy.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_postponed.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_singleton.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.9.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.9.2/README.md
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 configuraptor-1.9.2/PKG-INFO
```

### Comparing `configuraptor-1.8.0/CHANGELOG.md` & `configuraptor-1.9.2/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.9.2 (2023-06-22)
+### Fix
+* Internal values (_) should be updatable without TypedConfig._update logic ([`ef24673`](https://github.com/trialandsuccess/configuraptor/commit/ef24673f4304fa58d2b51a429efe7dc62ddc84f9))
+
+## v1.9.1 (2023-06-22)
+### Fix
+* Key="" workaround no longer required ([`2c5fcaf`](https://github.com/trialandsuccess/configuraptor/commit/2c5fcaf8471176b82ebf5438d677e8db657018ab))
+* **mapping:** Made mapping immutable, so MutableMapping actually has different behavior ([`a68ef56`](https://github.com/trialandsuccess/configuraptor/commit/a68ef5651a457cc08f0125f01f00b98ceb49c544))
+
+### Documentation
+* **mapping:** Add example for TypedMapping ([`e430f40`](https://github.com/trialandsuccess/configuraptor/commit/e430f4065b5060fb2d2a4a8c134e8c42e9f66b74))
+
+## v1.9.0 (2023-06-22)
+### Feature
+* **mapping:** Add configuraptor.TypedMapping and .TypedMutableMapping to support **unpacking (but not on default TypedConfig) ([`b4c6b9d`](https://github.com/trialandsuccess/configuraptor/commit/b4c6b9dc01cfd6727187310610e750fa6ada3234))
+
 ## v1.8.0 (2023-06-21)
 ### Feature
 * **format:** Allow TypedConfig._format ([`0b46646`](https://github.com/trialandsuccess/configuraptor/commit/0b46646fec153a6bcdfea0c40b872da884aa9146))
 
 ## v1.7.2 (2023-06-20)
 ### Fix
 * **toml:** Tomlkit had own types, move to tomli ([`0b5f0a4`](https://github.com/trialandsuccess/configuraptor/commit/0b5f0a4333f5767fc2329cebb040c6cf4c78eff9))
```

### Comparing `configuraptor-1.8.0/coverage.svg` & `configuraptor-1.9.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_circle.png` & `configuraptor-1.9.2/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_original.jpeg` & `configuraptor-1.9.2/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_round.png` & `configuraptor-1.9.2/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_transparent.png` & `configuraptor-1.9.2/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/dataclass.py` & `configuraptor-1.9.2/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/dumping.py` & `configuraptor-1.9.2/examples/dumping.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/example_from_readme.py` & `configuraptor-1.9.2/examples/example_from_readme.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/main.py` & `configuraptor-1.9.2/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/postponed.py` & `configuraptor-1.9.2/examples/postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/readme.md` & `configuraptor-1.9.2/examples/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 (e.g. `key="tool.some-tool"`). If no key is passed, it will be guessed based on some criteria:
 
 - if there is only one top-level key, it will be used automatically (this happens in the case of `OtherConfig` in
   the `README` example);
 - otherwise, the name of the class is used to guess the key name (this happens in the case of `Config` in
   the `README` example).
 
-If you pass `key=""` (empty string), all data will be loaded from the top-level.
+If you pass `key=""` (empty string), all data will be loaded from the top-level. 
+This will be done automatically too if something goes wrong with the supplied key.
 Example:
 
 ```json
 // somedata.json
 {
   "string": "here",
   "number": 123
@@ -370,8 +371,33 @@
       },
       "second": {
         "name": "dependency 3.2"
       }
     }
   }
 }
-```
+```
+
+## Mappings
+
+To make a class unpackable with `**`, you need to inherit `TypedMapping` or `TypedMutableMapping`.
+Doing this will break compatibility with `Singleton`, so this unpacking feature is not enabled on the
+default `TypedConfig`.
+`TypedMapping` also makes updating the data illegal, whereas this is allowed in `TypedConfig` and `TypedMutableMapping`.
+
+```python
+# example_mapping.py
+import configuraptor
+
+
+class MyConfig(configuraptor.TypedMapping):
+    key: str
+
+
+my_config = MyConfig.load({"key": "something"})
+
+# not allowed, because it's not a Mutable Mapping:
+my_config.update(key="something else")
+
+# this would crash if MyConfig was a TypedConfig:
+"key is {key}".format(**my_config)  # == "key is something"
+```
```

### Comparing `configuraptor-1.8.0/examples/singleton.py` & `configuraptor-1.9.2/examples/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/typedconfig_class.py` & `configuraptor-1.9.2/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/coverage_html.js` & `configuraptor-1.9.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:49 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the module version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.7.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.9.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:49 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  11 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-20 10:44 +0200
+22 13:49 +0200
 _1""" 
 _2This file contains the module version. 
 _3""" 
 _4 
 _5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 _6# 
 _7# SPDX-License-Identifier: MIT 
-_8__version__ = "1.7.2" 
+_8__version__ = "1.9.0" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-20 10:44 +0200
+22 13:49 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,15 +83,15 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Exposes TypedConfig and load_into for this library.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span><span class="op">,</span> <span class="nam">update</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span><span class="op">,</span> <span class="nam">TypedMapping</span><span class="op">,</span> <span class="nam">TypedMutableMapping</span><span class="op">,</span> <span class="nam">update</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">all_annotations</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">check_and_convert_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">convert_config</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">ensure_types</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">load_into</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">load_into_class</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
@@ -100,42 +100,44 @@
     <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">dump</span> <span class="key">import</span> <span class="nam">asdict</span><span class="op">,</span> <span class="nam">asjson</span><span class="op">,</span> <span class="nam">astoml</span><span class="op">,</span> <span class="nam">asyaml</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">postpone</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span><span class="op">,</span> <span class="nam">SingletonMeta</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="com"># cls</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"TypedConfig"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"update"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"TypedMapping"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"TypedMutableMapping"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"update"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,24 +6,24 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 66 ssttaatteemmeennttss ?  66 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-20 10:44 +0200
+22 13:07 +0200
 _1""" 
 _2Exposes TypedConfig and load_into for this library. 
 _3""" 
 _4 
 _5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 _6# 
 _7# SPDX-License-Identifier: MIT 
-_8from .cls import TypedConfig, update 
+_8from .cls import TypedConfig, TypedMapping, TypedMutableMapping, update 
 _9from .core import ( 
 _1_0 all_annotations, 
 _1_1 check_and_convert_data, 
 _1_2 convert_config, 
 _1_3 ensure_types, 
 _1_4 load_into, 
 _1_5 load_into_class, 
@@ -32,29 +32,31 @@
 _1_8from .dump import asdict, asjson, astoml, asyaml 
 _1_9from .postpone import postpone 
 _2_0from .singleton import Singleton, SingletonMeta 
 _2_1 
 _2_2__all__ = [ 
 _2_3 # cls 
 _2_4 "TypedConfig", 
-_2_5 "update", 
-_2_6 # singleton 
-_2_7 "Singleton", 
-_2_8 "SingletonMeta", 
-_2_9 # core 
-_3_0 "all_annotations", 
-_3_1 "check_and_convert_data", 
-_3_2 "convert_config", 
-_3_3 "ensure_types", 
-_3_4 "load_into", 
-_3_5 "load_into_class", 
-_3_6 "load_into_instance", 
-_3_7 # postpone 
-_3_8 "postpone", 
-_3_9 # dump 
-_4_0 "asdict", 
-_4_1 "astoml", 
-_4_2 "asyaml", 
-_4_3 "asjson", 
-_4_4] 
+_2_5 "TypedMapping", 
+_2_6 "TypedMutableMapping", 
+_2_7 "update", 
+_2_8 # singleton 
+_2_9 "Singleton", 
+_3_0 "SingletonMeta", 
+_3_1 # core 
+_3_2 "all_annotations", 
+_3_3 "check_and_convert_data", 
+_3_4 "convert_config", 
+_3_5 "ensure_types", 
+_3_6 "load_into", 
+_3_7 "load_into_class", 
+_3_8 "load_into_instance", 
+_3_9 # postpone 
+_4_0 "postpone", 
+_4_1 # dump 
+_4_2 "asdict", 
+_4_3 "astoml", 
+_4_4 "asyaml", 
+_4_5 "asjson", 
+_4_6] 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-20 10:44 +0200
+22 13:07 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_dump_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/cls.py: 100%</title>
+    <title>Coverage for src/configuraptor/dump.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/cls.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">24 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">24<span class="text"> run</span></button>
+            <span class="text">31 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,100 +77,84 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Logic for the TypedConfig inheritable class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Method to dump classes to other formats.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">all_annotations</span><span class="op">,</span> <span class="nam">check_type</span><span class="op">,</span> <span class="nam">load_into</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">,</span> <span class="nam">ConfigErrorInvalidType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedConfig</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    Can be used instead of load_into.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">load</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        Load a class' config values from the config file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        SomeClass.load(data, ...) = load_into(SomeClass, data, ...).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">def</span> <span class="nam">_update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">        Can be used if .update is overwritten with another value in the config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">values</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">_allow_none</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">instance_of_custom_class</span><span class="op">,</span> <span class="nam">is_custom_class</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_level</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">0</span><span class="op">,</span> <span class="op">/</span><span class="op">,</span> <span class="nam">with_top_level_key</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Dump a config instance to a dictionary (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">cls</span> <span class="op">=</span> <span class="nam">value</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">asdict</span><span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">_</span><span class="op">)</span> <span class="key">else</span> <span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">else</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">data</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">if</span> <span class="nam">_level</span> <span class="op">==</span> <span class="num">0</span> <span class="key">and</span> <span class="nam">with_top_level_key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="com"># top-level: add an extra key indicating the class' name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">cls_name</span> <span class="op">=</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="nam">cls_name</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="key">if</span> <span class="nam">_strict</span> <span class="key">and</span> <span class="nam">key</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">(</span><span class="nam">cls</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">if</span> <span class="nam">_strict</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">)</span> <span class="key">and</span> <span class="key">not</span> <span class="op">(</span><span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">_allow_none</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">expected_type</span><span class="op">=</span><span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">setattr</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    Dump a config instance to toml (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">tomli_w</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">=</span><span class="nam">multiline_strings</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">        Update values on this config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">            _strict: allow wrong types?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">            _allow_none: allow None or skip those entries?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">            **values: key: value pairs in the right types to update.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_update</span><span class="op">(</span><span class="nam">_strict</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">def</span> <span class="nam">_format</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">string</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">        Format the config data into a string template.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">        Replacement for string.format(**config), which is only possible for MutableMappings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">        MutableMapping does not work well with our Singleton Metaclass.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">return</span> <span class="nam">string</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="op">**</span><span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="com"># also expose as separate function:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">instance</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">    Update values on a config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="str">        instance: config instance to update</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        _strict: allow wrong types?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">        _allow_none: allow None or skip those entries?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">        **values: key: value pairs in the right types to update.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedConfig</span><span class="op">.</span><span class="nam">_update</span><span class="op">(</span><span class="nam">instance</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    Dump a config instance to json (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Dump a config instance to yaml (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">output</span> <span class="op">=</span> <span class="nam">yaml</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="com"># output is already a str but mypy doesn't know that</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,101 +1,81 @@
-************ CCoovveerraaggee ffoorr ssrrcc//ccoonnffiigguurraappttoorr//ccllss..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//ccoonnffiigguurraappttoorr//dduummpp..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2244 ssttaatteemmeennttss ?  2244 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 3311 ssttaatteemmeennttss ?  3311 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-21 15:50 +0200
+20 10:44 +0200
 _1""" 
-_2Logic for the TypedConfig inheritable class. 
+_2Method to dump classes to other formats. 
 _3""" 
 _4 
-_5import typing 
-_6 
-_7from .core import T_data, all_annotations, check_type, load_into 
-_8from .errors import ConfigErrorExtraKey, ConfigErrorInvalidType 
-_9 
-_1_0C = typing.TypeVar("C", bound=typing.Any) 
-_1_1 
-_1_2 
-_1_3class TypedConfig: 
-_1_4 """ 
-_1_5 Can be used instead of load_into. 
+_5import json 
+_6import typing 
+_7 
+_8import tomli_w 
+_9import yaml 
+_1_0 
+_1_1from .core import instance_of_custom_class, is_custom_class 
+_1_2from .helpers import camel_to_snake 
+_1_3 
+_1_4 
+_1_5def asdict(inst: typing.Any, _level: int = 0, /, with_top_level_key: bool =
+True) -> dict[str, typing.Any]: 
 _1_6 """ 
-_1_7 
-_1_8 @classmethod 
-_1_9 def load( 
-_2_0 cls: typing.Type[C], data: T_data, key: str = None, init: dict[str,
-typing.Any] = None, strict: bool = True 
-_2_1 ) -> C: 
-_2_2 """ 
-_2_3 Load a class' config values from the config file. 
-_2_4 
-_2_5 SomeClass.load(data, ...) = load_into(SomeClass, data, ...). 
-_2_6 """ 
-_2_7 return load_into(cls, data, key=key, init=init, strict=strict) 
-_2_8 
-_2_9 def _update(self, _strict: bool = True, _allow_none: bool = False, **values:
-typing.Any) -> None: 
-_3_0 """ 
-_3_1 Can be used if .update is overwritten with another value in the config. 
-_3_2 """ 
-_3_3 annotations = all_annotations(self.__class__) 
-_3_4 
-_3_5 for key, value in values.items(): 
-_3_6 if value is None and not _allow_none: 
-_3_7 continue 
+_1_7 Dump a config instance to a dictionary (recursively). 
+_1_8 """ 
+_1_9 data = {} 
+_2_0 
+_2_1 for key, value in inst.__dict__.items(): 
+_2_2 cls = value.__class__ 
+_2_3 if is_custom_class(cls): 
+_2_4 value = asdict(value, _level + 1) 
+_2_5 elif isinstance(value, list): 
+_2_6 value = [asdict(_, _level + 1) if instance_of_custom_class(_) else _ for _
+in value] 
+_2_7 elif isinstance(value, dict): 
+_2_8 value = {k: asdict(v, _level + 1) if instance_of_custom_class(v) else v for
+k, v in value.items()} 
+_2_9 
+_3_0 data[key] = value 
+_3_1 
+_3_2 if _level == 0 and with_top_level_key: 
+_3_3 # top-level: add an extra key indicating the class' name 
+_3_4 cls_name = camel_to_snake(inst.__class__.__name__) 
+_3_5 return {cls_name: data} 
+_3_6 
+_3_7 return data 
 _3_8 
-_3_9 if _strict and key not in annotations: 
-_4_0 raise ConfigErrorExtraKey(cls=self.__class__, key=key, value=value) 
-_4_1 
-_4_2 if _strict and not check_type(value, annotations[key]) and not (value is
-None and _allow_none): 
-_4_3 raise ConfigErrorInvalidType(expected_type=annotations[key], key=key,
-value=value) 
-_4_4 
-_4_5 setattr(self, key, value) 
+_3_9 
+_4_0def astoml(inst: typing.Any, multiline_strings: bool = False) -> str: 
+_4_1 """ 
+_4_2 Dump a config instance to toml (recursively). 
+_4_3 """ 
+_4_4 data = asdict(inst) 
+_4_5 return tomli_w.dumps(data, multiline_strings=multiline_strings) 
 _4_6 
-_4_7 def update(self, _strict: bool = True, _allow_none: bool = False, **values:
-typing.Any) -> None: 
-_4_8 """ 
-_4_9 Update values on this config. 
-_5_0 
-_5_1 Args: 
-_5_2 _strict: allow wrong types? 
-_5_3 _allow_none: allow None or skip those entries? 
-_5_4 **values: key: value pairs in the right types to update. 
-_5_5 """ 
-_5_6 return self._update(_strict, _allow_none, **values) 
-_5_7 
-_5_8 def _format(self, string: str) -> str: 
+_4_7 
+_4_8def asjson(inst: typing.Any, **kw: typing.Any) -> str: 
+_4_9 """ 
+_5_0 Dump a config instance to json (recursively). 
+_5_1 """ 
+_5_2 data = asdict(inst) 
+_5_3 return json.dumps(data, **kw) 
+_5_4 
+_5_5 
+_5_6def asyaml(inst: typing.Any, **kw: typing.Any) -> str: 
+_5_7 """ 
+_5_8 Dump a config instance to yaml (recursively). 
 _5_9 """ 
-_6_0 Format the config data into a string template. 
-_6_1 
-_6_2 Replacement for string.format(**config), which is only possible for
-MutableMappings. 
-_6_3 MutableMapping does not work well with our Singleton Metaclass. 
-_6_4 """ 
-_6_5 return string.format(**self.__dict__) 
-_6_6 
-_6_7 
-_6_8# also expose as separate function: 
-_6_9def update(instance: typing.Any, _strict: bool = True, _allow_none: bool =
-False, **values: typing.Any) -> None: 
-_7_0 """ 
-_7_1 Update values on a config. 
-_7_2 
-_7_3 Args: 
-_7_4 instance: config instance to update 
-_7_5 _strict: allow wrong types? 
-_7_6 _allow_none: allow None or skip those entries? 
-_7_7 **values: key: value pairs in the right types to update. 
-_7_8 """ 
-_7_9 return TypedConfig._update(instance, _strict, _allow_none, **values) 
+_6_0 data = asdict(inst) 
+_6_1 output = yaml.dump(data, encoding=None, **kw) 
+_6_2 # output is already a str but mypy doesn't know that 
+_6_3 return typing.cast(str, output) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-21 15:50 +0200
+20 10:44 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">156 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">156<span class="text"> run</span></button>
+            <span class="text">166 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">166<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">3<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">5<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:38 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -132,15 +132,15 @@
     <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    If no key is manually defined for `load_into`, \</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">    the class' name is converted to snake_case to use as the default key.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">return</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">clsname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">__load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    Tries to load the right data from a filename/path or dict, based on a manual key or a classname.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">    E.g. class Tool will be mapped to key tool.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">    It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -157,430 +157,450 @@
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="com"># try to guess key by grabbing the first one or using the class name</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">elif</span> <span class="nam">classname</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">_guess_key</span><span class="op">(</span><span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="key">return</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="com"># no key found, just return all data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"No data found!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Data is not a dict!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="key">def</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">    Wrapper around __load_data that retries with key="" if anything goes wrong.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">return</span> <span class="nam">__load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="key">if</span> <span class="nam">key</span> <span class="op">!=</span> <span class="str">""</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">            <span class="key">return</span> <span class="nam">__load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="str">""</span><span class="op">,</span> <span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="com"># key already was "", just return data!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">            <span class="com"># (will probably not happen but fallback)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">            <span class="key">return</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="com"># custom object to use instead of None, since typing.Optional can be None!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="com"># cast to T to make mypy happy</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">notfound</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T</span><span class="op">,</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="nam">postponed</span> <span class="op">=</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">notfound</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">notfound</span><span class="op">:</span>  <span class="com"># pragma: nocover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="nam">warnings</span><span class="op">.</span><span class="nam">warn</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="str">"This should not happen since "</span> <span class="str">"`load_recursive` already fills `data` "</span> <span class="str">"based on `annotations`"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">postponed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="com"># don't do anything with this item!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="key">def</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">items</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">    Converts the config dict (from toml) or 'overwrites' dict in two ways.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    1. removes any items where the value is None, since in that case the default should be used;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">    2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config properties.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"-"</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"."</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">items</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t"><span class="nam">Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t"><span class="nam">T_Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Type"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="key">def</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">    Returns whether _type is one of the builtin types.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"__builtin__"</span><span class="op">,</span> <span class="str">"builtins"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="key">def</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="com"># custom object to use instead of None, since typing.Optional can be None!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="com"># cast to T to make mypy happy</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="nam">notfound</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T</span><span class="op">,</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">postponed</span> <span class="op">=</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">notfound</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">notfound</span><span class="op">:</span>  <span class="com"># pragma: nocover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">            <span class="nam">warnings</span><span class="op">.</span><span class="nam">warn</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                <span class="str">"This should not happen since "</span> <span class="str">"`load_recursive` already fills `data` "</span> <span class="str">"based on `annotations`"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">postponed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="com"># don't do anything with this item!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="com"># def is_builtin_class_instance(obj: typing.Any) -> bool:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="com">#     return is_builtin_type(obj.__class__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="key">def</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">items</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">    Converts the config dict (from toml) or 'overwrites' dict in two ways.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="str">    Returns whether _type is one of the stlib typing/types types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">    1. removes any items where the value is None, since in that case the default should be used;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="str">    2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config properties.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"-"</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"."</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">items</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t"><span class="str">    e.g. types.UnionType or typing.Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"types"</span><span class="op">,</span> <span class="str">"typing"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="nam">Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t"><span class="nam">T_Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Type"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="key">def</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">    Besides builtins, toml also supports 'datetime' and 'math' types, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">    so this returns whether _type is a type from these stdlib modules.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"datetime"</span><span class="op">,</span> <span class="str">"math"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">    Returns whether _type is one of the builtin types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"__builtin__"</span><span class="op">,</span> <span class="str">"builtins"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="key">def</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">    Returns whether _type is a parameterized type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="str">        list[str] -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t"><span class="str">        str -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t"><span class="com"># def is_builtin_class_instance(obj: typing.Any) -> bool:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="com">#     return is_builtin_type(obj.__class__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="str">    Returns whether _type is one of the stlib typing/types types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">    e.g. types.UnionType or typing.Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"types"</span><span class="op">,</span> <span class="str">"typing"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="key">def</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">    Tries to guess if _type is a builtin or a custom (user-defined) class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">    Other logic in this module depends on knowing that.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t"><span class="str">    Besides builtins, toml also supports 'datetime' and 'math' types, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">    so this returns whether _type is a type from these stdlib modules.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"datetime"</span><span class="op">,</span> <span class="str">"math"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="key">def</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">    Returns whether _type is a parameterized type.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="key">def</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">    Calls `is_custom_class` on an instance of a (possibly custom) class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">    <span class="key">return</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="str">        list[str] -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t"><span class="str">        str -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="key">def</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span> <span class="op">|</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">    Tries to guess if _type could be optional.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="str">        None -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="str">        NoneType -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">        typing.Union[str, None] -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">        str | None -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">        list[str | None] -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">        list[str] -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="key">if</span> <span class="nam">_type</span> <span class="key">and</span> <span class="op">(</span><span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">dict</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">)</span> <span class="key">or</span> <span class="op">(</span><span class="nam">_type</span> <span class="key">is</span> <span class="nam">math</span><span class="op">.</span><span class="nam">nan</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="com"># e.g. list[str]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="com"># will crash issubclass to test it first here</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">or</span> <span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t"><span class="key">def</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t"><span class="str">    Tries to guess if _type is a builtin or a custom (user-defined) class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t"><span class="str">    Other logic in this module depends on knowing that.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="key">def</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">    Calls `is_custom_class` on an instance of a (possibly custom) class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">return</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="key">def</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span> <span class="op">|</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">    Tries to guess if _type could be optional.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">        None -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        NoneType -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">        typing.Union[str, None] -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">        str | None -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">        list[str | None] -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        list[str] -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="key">if</span> <span class="nam">_type</span> <span class="key">and</span> <span class="op">(</span><span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">dict</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">)</span> <span class="key">or</span> <span class="op">(</span><span class="nam">_type</span> <span class="key">is</span> <span class="nam">math</span><span class="op">.</span><span class="nam">nan</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="com"># e.g. list[str]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="com"># will crash issubclass to test it first here</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">        <span class="key">or</span> <span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="key">def</span> <span class="nam">check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">if</span> <span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="key">def</span> <span class="nam">check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="key">if</span> <span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_instance</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t"><span class="str">    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t"><span class="str">    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t"><span class="str">        strict: enable type checks or allow anything?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">        <span class="com"># would not be supported according to mypy, but you can still load_into(instance)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t">    <span class="com"># _cls = typing.cast(typing.Type[C], cls)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_instance</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t490" href="#t490">490</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t491" href="#t491">491</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t492" href="#t492">492</a></span><span class="t"><span class="str">    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t493" href="#t493">493</a></span><span class="t"><span class="str">    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t494" href="#t494">494</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t495" href="#t495">495</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t496" href="#t496">496</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t497" href="#t497">497</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t498" href="#t498">498</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t499" href="#t499">499</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t500" href="#t500">500</a></span><span class="t"><span class="str">        strict: enable type checks or allow anything?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t501" href="#t501">501</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t502" href="#t502">502</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t503" href="#t503">503</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t504" href="#t504">504</a></span><span class="t">        <span class="com"># would not be supported according to mypy, but you can still load_into(instance)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t505" href="#t505">505</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t506" href="#t506">506</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t507" href="#t507">507</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t508" href="#t508">508</a></span><span class="t">    <span class="com"># _cls = typing.cast(typing.Type[C], cls)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t509" href="#t509">509</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:38 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,17 +4,17 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 115566 ssttaatteemmeennttss ?  115566 rruunn 00 mmiissssiinngg 33 eexxcclluuddeedd **********
+********** 116666 ssttaatteemmeennttss ?  116666 rruunn 00 mmiissssiinngg 55 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-19 17:38 +0200
+22 14:32 +0200
 _1""" 
 _2Contains most of the loading logic. 
 _3""" 
 _4 
 _5import dataclasses as dc 
 _6import math 
 _7import types 
@@ -65,15 +65,15 @@
 _5_0 """ 
 _5_1 If no key is manually defined for `load_into`, \ 
 _5_2 the class' name is converted to snake_case to use as the default key. 
 _5_3 """ 
 _5_4 return camel_to_snake(clsname) 
 _5_5 
 _5_6 
-_5_7def _load_data(data: T_data, key: str = None, classname: str = None) -> dict
+_5_7def __load_data(data: T_data, key: str = None, classname: str = None) -> dict
 [str, typing.Any]: 
 _5_8 """ 
 _5_9 Tries to load the right data from a filename/path or dict, based on a manual
 key or a classname. 
 _6_0 
 _6_1 E.g. class Tool will be mapped to key tool. 
 _6_2 It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}} 
@@ -92,451 +92,472 @@
 _7_5 # try to guess key by grabbing the first one or using the class name 
 _7_6 if len(data) == 1: 
 _7_7 key = list(data.keys())[0] 
 _7_8 elif classname is not None: 
 _7_9 key = _guess_key(classname) 
 _8_0 
 _8_1 if key: 
-_8_2 return _data_for_nested_key(key, data) 
-_8_3 else: 
-_8_4 # no key found, just return all data 
-_8_5 return data 
+_8_2 data = _data_for_nested_key(key, data) 
+_8_3 
+_8_4 if not data: 
+_8_5 raise ValueError("No data found!") 
 _8_6 
-_8_7 
-_8_8def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
-_8_9 """ 
-_9_0 Given a variable, check if it matches 'expected_type' (which can be a Union,
-parameterized generic etc.). 
+_8_7 if not isinstance(data, dict): 
+_8_8 raise ValueError("Data is not a dict!") 
+_8_9 
+_9_0 return data 
 _9_1 
-_9_2 Based on typeguard but this returns a boolean instead of returning the value
-or throwing a TypeCheckError 
-_9_3 """ 
-_9_4 try: 
-_9_5 _check_type(value, expected_type) 
-_9_6 return True 
-_9_7 except TypeCheckError: 
-_9_8 return False 
-_9_9 
-_1_0_0 
-_1_0_1def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
+_9_2 
+_9_3def _load_data(data: T_data, key: str = None, classname: str = None) -> dict
+[str, typing.Any]: 
+_9_4 """ 
+_9_5 Wrapper around __load_data that retries with key="" if anything goes wrong. 
+_9_6 """ 
+_9_7 try: 
+_9_8 return __load_data(data, key, classname) 
+_9_9 except Exception as e: 
+_1_0_0 if key != "": 
+_1_0_1 return __load_data(data, "", classname) 
+_1_0_2 else: # pragma: no cover 
+_1_0_3 # key already was "", just return data! 
+_1_0_4 # (will probably not happen but fallback) 
+_1_0_5 return {} 
+_1_0_6 
+_1_0_7 
+_1_0_8def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
+_1_0_9 """ 
+_1_1_0 Given a variable, check if it matches 'expected_type' (which can be a
+Union, parameterized generic etc.). 
+_1_1_1 
+_1_1_2 Based on typeguard but this returns a boolean instead of returning the
+value or throwing a TypeCheckError 
+_1_1_3 """ 
+_1_1_4 try: 
+_1_1_5 _check_type(value, expected_type) 
+_1_1_6 return True 
+_1_1_7 except TypeCheckError: 
+_1_1_8 return False 
+_1_1_9 
+_1_2_0 
+_1_2_1def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
 [str, T | None]: 
-_1_0_2 """ 
-_1_0_3 Make sure all values in 'data' are in line with the ones stored in
+_1_2_2 """ 
+_1_2_3 Make sure all values in 'data' are in line with the ones stored in
 'annotations'. 
-_1_0_4 
-_1_0_5 If an annotated key in missing from data, it will be filled with None for
+_1_2_4 
+_1_2_5 If an annotated key in missing from data, it will be filled with None for
 convenience. 
-_1_0_6 
-_1_0_7 TODO: python 3.11 exception groups to throw multiple errors at once! 
-_1_0_8 """ 
-_1_0_9 # custom object to use instead of None, since typing.Optional can be None! 
-_1_1_0 # cast to T to make mypy happy 
-_1_1_1 notfound = typing.cast(T, object()) 
-_1_1_2 postponed = Postponed() 
-_1_1_3 
-_1_1_4 final: dict[str, T | None] = {} 
-_1_1_5 for key, _type in annotations.items(): 
-_1_1_6 compare = data.get(key, notfound) 
-_1_1_7 if compare is notfound: # pragma: nocover 
-_1_1_8 warnings.warn( 
-_1_1_9 "This should not happen since " "`load_recursive` already fills `data` "
+_1_2_6 
+_1_2_7 TODO: python 3.11 exception groups to throw multiple errors at once! 
+_1_2_8 """ 
+_1_2_9 # custom object to use instead of None, since typing.Optional can be None! 
+_1_3_0 # cast to T to make mypy happy 
+_1_3_1 notfound = typing.cast(T, object()) 
+_1_3_2 postponed = Postponed() 
+_1_3_3 
+_1_3_4 final: dict[str, T | None] = {} 
+_1_3_5 for key, _type in annotations.items(): 
+_1_3_6 compare = data.get(key, notfound) 
+_1_3_7 if compare is notfound: # pragma: nocover 
+_1_3_8 warnings.warn( 
+_1_3_9 "This should not happen since " "`load_recursive` already fills `data` "
 "based on `annotations`" 
-_1_2_0 ) 
-_1_2_1 # skip! 
-_1_2_2 continue 
-_1_2_3 
-_1_2_4 if compare is postponed: 
-_1_2_5 # don't do anything with this item! 
-_1_2_6 continue 
-_1_2_7 
-_1_2_8 if not check_type(compare, _type): 
-_1_2_9 raise ConfigErrorInvalidType(key, value=compare, expected_type=_type) 
-_1_3_0 
-_1_3_1 final[key] = compare 
-_1_3_2 
-_1_3_3 return final 
-_1_3_4 
-_1_3_5 
-_1_3_6def convert_config(items: dict[str, T]) -> dict[str, T]: 
-_1_3_7 """ 
-_1_3_8 Converts the config dict (from toml) or 'overwrites' dict in two ways. 
-_1_3_9 
-_1_4_0 1. removes any items where the value is None, since in that case the
-default should be used; 
-_1_4_1 2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config
-properties. 
-_1_4_2 """ 
-_1_4_3 return {k.replace("-", "_").replace(".", "_"): v for k, v in items.items()
-if v is not None} 
-_1_4_4 
-_1_4_5 
-_1_4_6Type = typing.Type[typing.Any] 
-_1_4_7T_Type = typing.TypeVar("T_Type", bound=Type) 
-_1_4_8 
-_1_4_9 
-_1_5_0def is_builtin_type(_type: Type) -> bool: 
-_1_5_1 """ 
-_1_5_2 Returns whether _type is one of the builtin types. 
-_1_5_3 """ 
-_1_5_4 return _type.__module__ in ("__builtin__", "builtins") 
+_1_4_0 ) 
+_1_4_1 # skip! 
+_1_4_2 continue 
+_1_4_3 
+_1_4_4 if compare is postponed: 
+_1_4_5 # don't do anything with this item! 
+_1_4_6 continue 
+_1_4_7 
+_1_4_8 if not check_type(compare, _type): 
+_1_4_9 raise ConfigErrorInvalidType(key, value=compare, expected_type=_type) 
+_1_5_0 
+_1_5_1 final[key] = compare 
+_1_5_2 
+_1_5_3 return final 
+_1_5_4 
 _1_5_5 
-_1_5_6 
-_1_5_7# def is_builtin_class_instance(obj: typing.Any) -> bool: 
-_1_5_8# return is_builtin_type(obj.__class__) 
+_1_5_6def convert_config(items: dict[str, T]) -> dict[str, T]: 
+_1_5_7 """ 
+_1_5_8 Converts the config dict (from toml) or 'overwrites' dict in two ways. 
 _1_5_9 
-_1_6_0 
-_1_6_1def is_from_types_or_typing(_type: Type) -> bool: 
+_1_6_0 1. removes any items where the value is None, since in that case the
+default should be used; 
+_1_6_1 2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config
+properties. 
 _1_6_2 """ 
-_1_6_3 Returns whether _type is one of the stlib typing/types types. 
+_1_6_3 return {k.replace("-", "_").replace(".", "_"): v for k, v in items.items()
+if v is not None} 
 _1_6_4 
-_1_6_5 e.g. types.UnionType or typing.Union 
-_1_6_6 """ 
-_1_6_7 return _type.__module__ in ("types", "typing") 
+_1_6_5 
+_1_6_6Type = typing.Type[typing.Any] 
+_1_6_7T_Type = typing.TypeVar("T_Type", bound=Type) 
 _1_6_8 
 _1_6_9 
-_1_7_0def is_from_other_toml_supported_module(_type: Type) -> bool: 
+_1_7_0def is_builtin_type(_type: Type) -> bool: 
 _1_7_1 """ 
-_1_7_2 Besides builtins, toml also supports 'datetime' and 'math' types, \ 
-_1_7_3 so this returns whether _type is a type from these stdlib modules. 
-_1_7_4 """ 
-_1_7_5 return _type.__module__ in ("datetime", "math") 
+_1_7_2 Returns whether _type is one of the builtin types. 
+_1_7_3 """ 
+_1_7_4 return _type.__module__ in ("__builtin__", "builtins") 
+_1_7_5 
 _1_7_6 
-_1_7_7 
-_1_7_8def is_parameterized(_type: Type) -> bool: 
-_1_7_9 """ 
-_1_8_0 Returns whether _type is a parameterized type. 
-_1_8_1 
-_1_8_2 Examples: 
-_1_8_3 list[str] -> True 
-_1_8_4 str -> False 
-_1_8_5 """ 
-_1_8_6 return typing.get_origin(_type) is not None 
-_1_8_7 
+_1_7_7# def is_builtin_class_instance(obj: typing.Any) -> bool: 
+_1_7_8# return is_builtin_type(obj.__class__) 
+_1_7_9 
+_1_8_0 
+_1_8_1def is_from_types_or_typing(_type: Type) -> bool: 
+_1_8_2 """ 
+_1_8_3 Returns whether _type is one of the stlib typing/types types. 
+_1_8_4 
+_1_8_5 e.g. types.UnionType or typing.Union 
+_1_8_6 """ 
+_1_8_7 return _type.__module__ in ("types", "typing") 
 _1_8_8 
-_1_8_9def is_custom_class(_type: Type) -> bool: 
-_1_9_0 """ 
-_1_9_1 Tries to guess if _type is a builtin or a custom (user-defined) class. 
-_1_9_2 
-_1_9_3 Other logic in this module depends on knowing that. 
+_1_8_9 
+_1_9_0def is_from_other_toml_supported_module(_type: Type) -> bool: 
+_1_9_1 """ 
+_1_9_2 Besides builtins, toml also supports 'datetime' and 'math' types, \ 
+_1_9_3 so this returns whether _type is a type from these stdlib modules. 
 _1_9_4 """ 
-_1_9_5 return ( 
-_1_9_6 type(_type) is type 
-_1_9_7 and not is_builtin_type(_type) 
-_1_9_8 and not is_from_other_toml_supported_module(_type) 
-_1_9_9 and not is_from_types_or_typing(_type) 
-_2_0_0 ) 
+_1_9_5 return _type.__module__ in ("datetime", "math") 
+_1_9_6 
+_1_9_7 
+_1_9_8def is_parameterized(_type: Type) -> bool: 
+_1_9_9 """ 
+_2_0_0 Returns whether _type is a parameterized type. 
 _2_0_1 
-_2_0_2 
-_2_0_3def instance_of_custom_class(var: typing.Any) -> bool: 
-_2_0_4 """ 
-_2_0_5 Calls `is_custom_class` on an instance of a (possibly custom) class. 
-_2_0_6 """ 
-_2_0_7 return is_custom_class(var.__class__) 
+_2_0_2 Examples: 
+_2_0_3 list[str] -> True 
+_2_0_4 str -> False 
+_2_0_5 """ 
+_2_0_6 return typing.get_origin(_type) is not None 
+_2_0_7 
 _2_0_8 
-_2_0_9 
-_2_1_0def is_optional(_type: Type | typing.Any) -> bool: 
-_2_1_1 """ 
-_2_1_2 Tries to guess if _type could be optional. 
-_2_1_3 
-_2_1_4 Examples: 
-_2_1_5 None -> True 
-_2_1_6 NoneType -> True 
-_2_1_7 typing.Union[str, None] -> True 
-_2_1_8 str | None -> True 
-_2_1_9 list[str | None] -> False 
-_2_2_0 list[str] -> False 
-_2_2_1 """ 
-_2_2_2 if _type and (is_parameterized(_type) and typing.get_origin(_type) in
-(dict, list)) or (_type is math.nan): 
-_2_2_3 # e.g. list[str] 
-_2_2_4 # will crash issubclass to test it first here 
-_2_2_5 return False 
-_2_2_6 
-_2_2_7 return ( 
-_2_2_8 _type is None 
-_2_2_9 or types.NoneType in typing.get_args(_type) # union with Nonetype 
-_2_3_0 or issubclass(types.NoneType, _type) 
-_2_3_1 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
-_2_3_2 ) 
+_2_0_9def is_custom_class(_type: Type) -> bool: 
+_2_1_0 """ 
+_2_1_1 Tries to guess if _type is a builtin or a custom (user-defined) class. 
+_2_1_2 
+_2_1_3 Other logic in this module depends on knowing that. 
+_2_1_4 """ 
+_2_1_5 return ( 
+_2_1_6 type(_type) is type 
+_2_1_7 and not is_builtin_type(_type) 
+_2_1_8 and not is_from_other_toml_supported_module(_type) 
+_2_1_9 and not is_from_types_or_typing(_type) 
+_2_2_0 ) 
+_2_2_1 
+_2_2_2 
+_2_2_3def instance_of_custom_class(var: typing.Any) -> bool: 
+_2_2_4 """ 
+_2_2_5 Calls `is_custom_class` on an instance of a (possibly custom) class. 
+_2_2_6 """ 
+_2_2_7 return is_custom_class(var.__class__) 
+_2_2_8 
+_2_2_9 
+_2_3_0def is_optional(_type: Type | typing.Any) -> bool: 
+_2_3_1 """ 
+_2_3_2 Tries to guess if _type could be optional. 
 _2_3_3 
-_2_3_4 
-_2_3_5def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
+_2_3_4 Examples: 
+_2_3_5 None -> True 
+_2_3_6 NoneType -> True 
+_2_3_7 typing.Union[str, None] -> True 
+_2_3_8 str | None -> True 
+_2_3_9 list[str | None] -> False 
+_2_4_0 list[str] -> False 
+_2_4_1 """ 
+_2_4_2 if _type and (is_parameterized(_type) and typing.get_origin(_type) in
+(dict, list)) or (_type is math.nan): 
+_2_4_3 # e.g. list[str] 
+_2_4_4 # will crash issubclass to test it first here 
+_2_4_5 return False 
+_2_4_6 
+_2_4_7 return ( 
+_2_4_8 _type is None 
+_2_4_9 or types.NoneType in typing.get_args(_type) # union with Nonetype 
+_2_5_0 or issubclass(types.NoneType, _type) 
+_2_5_1 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
+_2_5_2 ) 
+_2_5_3 
+_2_5_4 
+_2_5_5def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
 [typing.Any]]: 
-_2_3_6 """ 
-_2_3_7 Get Field info for a dataclass cls. 
-_2_3_8 """ 
-_2_3_9 fields = getattr(cls, "__dataclass_fields__", {}) 
-_2_4_0 return fields.get(key) 
-_2_4_1 
-_2_4_2 
-_2_4_3def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
+_2_5_6 """ 
+_2_5_7 Get Field info for a dataclass cls. 
+_2_5_8 """ 
+_2_5_9 fields = getattr(cls, "__dataclass_fields__", {}) 
+_2_6_0 return fields.get(key) 
+_2_6_1 
+_2_6_2 
+_2_6_3def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
 Type]) -> dict[str, T]: 
-_2_4_4 """ 
-_2_4_5 For all annotations (recursively gathered from parents with
+_2_6_4 """ 
+_2_6_5 For all annotations (recursively gathered from parents with
 `all_annotations`), \ 
-_2_4_6 try to resolve the tree of annotations. 
-_2_4_7 
-_2_4_8 Uses `load_into_recurse`, not itself directly. 
-_2_4_9 
-_2_5_0 Example: 
-_2_5_1 class First: 
-_2_5_2 key: str 
-_2_5_3 
-_2_5_4 class Second: 
-_2_5_5 other: First 
-_2_5_6 
-_2_5_7 # step 1 
-_2_5_8 cls = Second 
-_2_5_9 data = {"second": {"other": {"key": "anything"}}} 
-_2_6_0 annotations: {"other": First} 
-_2_6_1 
-_2_6_2 # step 1.5 
-_2_6_3 data = {"other": {"key": "anything"} 
-_2_6_4 annotations: {"other": First} 
-_2_6_5 
-_2_6_6 # step 2 
-_2_6_7 cls = First 
-_2_6_8 data = {"key": "anything"} 
-_2_6_9 annotations: {"key": str} 
-_2_7_0 
-_2_7_1 
-_2_7_2 TODO: python 3.11 exception groups to throw multiple errors at once! 
-_2_7_3 """ 
-_2_7_4 updated = {} 
-_2_7_5 
-_2_7_6 for _key, _type in annotations.items(): 
-_2_7_7 if _key in data: 
-_2_7_8 value: typing.Any = data[_key] # value can change so define it as any
-instead of T 
-_2_7_9 if is_parameterized(_type): 
-_2_8_0 origin = typing.get_origin(_type) 
-_2_8_1 arguments = typing.get_args(_type) 
-_2_8_2 if origin is list and arguments and is_custom_class(arguments[0]): 
-_2_8_3 subtype = arguments[0] 
-_2_8_4 value = [_load_into_recurse(subtype, subvalue) for subvalue in value] 
+_2_6_6 try to resolve the tree of annotations. 
+_2_6_7 
+_2_6_8 Uses `load_into_recurse`, not itself directly. 
+_2_6_9 
+_2_7_0 Example: 
+_2_7_1 class First: 
+_2_7_2 key: str 
+_2_7_3 
+_2_7_4 class Second: 
+_2_7_5 other: First 
+_2_7_6 
+_2_7_7 # step 1 
+_2_7_8 cls = Second 
+_2_7_9 data = {"second": {"other": {"key": "anything"}}} 
+_2_8_0 annotations: {"other": First} 
+_2_8_1 
+_2_8_2 # step 1.5 
+_2_8_3 data = {"other": {"key": "anything"} 
+_2_8_4 annotations: {"other": First} 
 _2_8_5 
-_2_8_6 elif origin is dict and arguments and is_custom_class(arguments[1]): 
-_2_8_7 # e.g. dict[str, Point] 
-_2_8_8 subkeytype, subvaluetype = arguments 
-_2_8_9 # subkey(type) is not a custom class, so don't try to convert it: 
-_2_9_0 value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey,
+_2_8_6 # step 2 
+_2_8_7 cls = First 
+_2_8_8 data = {"key": "anything"} 
+_2_8_9 annotations: {"key": str} 
+_2_9_0 
+_2_9_1 
+_2_9_2 TODO: python 3.11 exception groups to throw multiple errors at once! 
+_2_9_3 """ 
+_2_9_4 updated = {} 
+_2_9_5 
+_2_9_6 for _key, _type in annotations.items(): 
+_2_9_7 if _key in data: 
+_2_9_8 value: typing.Any = data[_key] # value can change so define it as any
+instead of T 
+_2_9_9 if is_parameterized(_type): 
+_3_0_0 origin = typing.get_origin(_type) 
+_3_0_1 arguments = typing.get_args(_type) 
+_3_0_2 if origin is list and arguments and is_custom_class(arguments[0]): 
+_3_0_3 subtype = arguments[0] 
+_3_0_4 value = [_load_into_recurse(subtype, subvalue) for subvalue in value] 
+_3_0_5 
+_3_0_6 elif origin is dict and arguments and is_custom_class(arguments[1]): 
+_3_0_7 # e.g. dict[str, Point] 
+_3_0_8 subkeytype, subvaluetype = arguments 
+_3_0_9 # subkey(type) is not a custom class, so don't try to convert it: 
+_3_1_0 value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey,
 subvalue in value.items()} 
-_2_9_1 # elif origin is dict: 
-_2_9_2 # keep data the same 
-_2_9_3 elif origin is typing.Union and arguments: 
-_2_9_4 for arg in arguments: 
-_2_9_5 if is_custom_class(arg): 
-_2_9_6 value = _load_into_recurse(arg, value) 
-_2_9_7 else: 
-_2_9_8 # print(_type, arg, value) 
-_2_9_9 ... 
-_3_0_0 
-_3_0_1 # todo: other parameterized/unions/typing.Optional 
-_3_0_2 
-_3_0_3 elif is_custom_class(_type): 
-_3_0_4 # type must be C (custom class) at this point 
-_3_0_5 value = _load_into_recurse( 
-_3_0_6 # make mypy and pycharm happy by telling it _type is of type C... 
-_3_0_7 # actually just passing _type as first arg! 
-_3_0_8 typing.cast(Type_C[typing.Any], _type), 
-_3_0_9 value, 
-_3_1_0 ) 
-_3_1_1 
-_3_1_2 elif _key in cls.__dict__: 
-_3_1_3 # property has default, use that instead. 
-_3_1_4 value = cls.__dict__[_key] 
-_3_1_5 elif is_optional(_type): 
-_3_1_6 # type is optional and not found in __dict__ -> default is None 
-_3_1_7 value = None 
-_3_1_8 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
+_3_1_1 # elif origin is dict: 
+_3_1_2 # keep data the same 
+_3_1_3 elif origin is typing.Union and arguments: 
+_3_1_4 for arg in arguments: 
+_3_1_5 if is_custom_class(arg): 
+_3_1_6 value = _load_into_recurse(arg, value) 
+_3_1_7 else: 
+_3_1_8 # print(_type, arg, value) 
+_3_1_9 ... 
+_3_2_0 
+_3_2_1 # todo: other parameterized/unions/typing.Optional 
+_3_2_2 
+_3_2_3 elif is_custom_class(_type): 
+_3_2_4 # type must be C (custom class) at this point 
+_3_2_5 value = _load_into_recurse( 
+_3_2_6 # make mypy and pycharm happy by telling it _type is of type C... 
+_3_2_7 # actually just passing _type as first arg! 
+_3_2_8 typing.cast(Type_C[typing.Any], _type), 
+_3_2_9 value, 
+_3_3_0 ) 
+_3_3_1 
+_3_3_2 elif _key in cls.__dict__: 
+_3_3_3 # property has default, use that instead. 
+_3_3_4 value = cls.__dict__[_key] 
+_3_3_5 elif is_optional(_type): 
+_3_3_6 # type is optional and not found in __dict__ -> default is None 
+_3_3_7 value = None 
+_3_3_8 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
 field.default_factory is not dc.MISSING: 
-_3_1_9 # could have a default factory 
-_3_2_0 # todo: do something with field.default? 
-_3_2_1 value = field.default_factory() 
-_3_2_2 else: 
-_3_2_3 raise ConfigErrorMissingKey(_key, cls, _type) 
-_3_2_4 
-_3_2_5 updated[_key] = value 
-_3_2_6 
-_3_2_7 return updated 
-_3_2_8 
-_3_2_9 
-_3_3_0def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
-_3_3_1 """ 
-_3_3_2 Returns a dictionary-like ChainMap that includes annotations for all \ 
-_3_3_3 attributes defined in cls or inherited from superclasses. 
-_3_3_4 """ 
-_3_3_5 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
-"__annotations__" in c.__dict__)) 
-_3_3_6 
-_3_3_7 
-_3_3_8def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
-[str, Type]: 
-_3_3_9 """ 
-_3_4_0 Wrapper around `_all_annotations` that filters away any keys in _except. 
-_3_4_1 
-_3_4_2 It also flattens the ChainMap to a regular dict. 
-_3_4_3 """ 
-_3_4_4 if _except is None: 
-_3_4_5 _except = set() 
+_3_3_9 # could have a default factory 
+_3_4_0 # todo: do something with field.default? 
+_3_4_1 value = field.default_factory() 
+_3_4_2 else: 
+_3_4_3 raise ConfigErrorMissingKey(_key, cls, _type) 
+_3_4_4 
+_3_4_5 updated[_key] = value 
 _3_4_6 
-_3_4_7 _all = _all_annotations(cls) 
-_3_4_8 return {k: v for k, v in _all.items() if k not in _except} 
+_3_4_7 return updated 
+_3_4_8 
 _3_4_9 
-_3_5_0 
-_3_5_1def check_and_convert_data( 
-_3_5_2 cls: typing.Type[C], 
-_3_5_3 data: dict[str, typing.Any], 
-_3_5_4 _except: typing.Iterable[str], 
-_3_5_5 strict: bool = True, 
-_3_5_6) -> dict[str, typing.Any]: 
-_3_5_7 """ 
-_3_5_8 Based on class annotations, this prepares the data for
+_3_5_0def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
+_3_5_1 """ 
+_3_5_2 Returns a dictionary-like ChainMap that includes annotations for all \ 
+_3_5_3 attributes defined in cls or inherited from superclasses. 
+_3_5_4 """ 
+_3_5_5 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+"__annotations__" in c.__dict__)) 
+_3_5_6 
+_3_5_7 
+_3_5_8def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
+[str, Type]: 
+_3_5_9 """ 
+_3_6_0 Wrapper around `_all_annotations` that filters away any keys in _except. 
+_3_6_1 
+_3_6_2 It also flattens the ChainMap to a regular dict. 
+_3_6_3 """ 
+_3_6_4 if _except is None: 
+_3_6_5 _except = set() 
+_3_6_6 
+_3_6_7 _all = _all_annotations(cls) 
+_3_6_8 return {k: v for k, v in _all.items() if k not in _except} 
+_3_6_9 
+_3_7_0 
+_3_7_1def check_and_convert_data( 
+_3_7_2 cls: typing.Type[C], 
+_3_7_3 data: dict[str, typing.Any], 
+_3_7_4 _except: typing.Iterable[str], 
+_3_7_5 strict: bool = True, 
+_3_7_6) -> dict[str, typing.Any]: 
+_3_7_7 """ 
+_3_7_8 Based on class annotations, this prepares the data for
 `load_into_recurse`. 
-_3_5_9 
-_3_6_0 1. convert config-keys to python compatible config_keys 
-_3_6_1 2. loads custom class type annotations with the same logic (see also
+_3_7_9 
+_3_8_0 1. convert config-keys to python compatible config_keys 
+_3_8_1 2. loads custom class type annotations with the same logic (see also
 `load_recursive`) 
-_3_6_2 3. ensures the annotated types match the actual types after loading the
+_3_8_2 3. ensures the annotated types match the actual types after loading the
 config file. 
-_3_6_3 """ 
-_3_6_4 annotations = all_annotations(cls, _except=_except) 
-_3_6_5 
-_3_6_6 to_load = convert_config(data) 
-_3_6_7 to_load = load_recursive(cls, to_load, annotations) 
-_3_6_8 if strict: 
-_3_6_9 to_load = ensure_types(to_load, annotations) 
-_3_7_0 
-_3_7_1 return to_load 
-_3_7_2 
-_3_7_3 
-_3_7_4def _load_into_recurse( 
-_3_7_5 cls: typing.Type[C], 
-_3_7_6 data: dict[str, typing.Any], 
-_3_7_7 init: dict[str, typing.Any] = None, 
-_3_7_8 strict: bool = True, 
-_3_7_9) -> C: 
-_3_8_0 """ 
-_3_8_1 Loads an instance of `cls` filled with `data`. 
-_3_8_2 
-_3_8_3 Uses `load_recursive` to load any fillable annotated properties (see that
+_3_8_3 """ 
+_3_8_4 annotations = all_annotations(cls, _except=_except) 
+_3_8_5 
+_3_8_6 to_load = convert_config(data) 
+_3_8_7 to_load = load_recursive(cls, to_load, annotations) 
+_3_8_8 if strict: 
+_3_8_9 to_load = ensure_types(to_load, annotations) 
+_3_9_0 
+_3_9_1 return to_load 
+_3_9_2 
+_3_9_3 
+_3_9_4def _load_into_recurse( 
+_3_9_5 cls: typing.Type[C], 
+_3_9_6 data: dict[str, typing.Any], 
+_3_9_7 init: dict[str, typing.Any] = None, 
+_3_9_8 strict: bool = True, 
+_3_9_9) -> C: 
+_4_0_0 """ 
+_4_0_1 Loads an instance of `cls` filled with `data`. 
+_4_0_2 
+_4_0_3 Uses `load_recursive` to load any fillable annotated properties (see that
 method for an example). 
-_3_8_4 `init` can be used to optionally pass extra __init__ arguments. \ 
-_3_8_5 NOTE: This will overwrite a config key with the same name! 
-_3_8_6 """ 
-_3_8_7 if init is None: 
-_3_8_8 init = {} 
-_3_8_9 
-_3_9_0 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
-_3_9_1 
-_3_9_2 if dc.is_dataclass(cls): 
-_3_9_3 to_load = check_and_convert_data(cls, data, init.keys(), strict=strict) 
-_3_9_4 to_load |= init # add extra init variables (should not happen for a
+_4_0_4 `init` can be used to optionally pass extra __init__ arguments. \ 
+_4_0_5 NOTE: This will overwrite a config key with the same name! 
+_4_0_6 """ 
+_4_0_7 if init is None: 
+_4_0_8 init = {} 
+_4_0_9 
+_4_1_0 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
+_4_1_1 
+_4_1_2 if dc.is_dataclass(cls): 
+_4_1_3 to_load = check_and_convert_data(cls, data, init.keys(), strict=strict) 
+_4_1_4 to_load |= init # add extra init variables (should not happen for a
 dataclass but whatev) 
-_3_9_5 
-_3_9_6 # ensure mypy inst is an instance of the cls type (and not a fictuous
+_4_1_5 
+_4_1_6 # ensure mypy inst is an instance of the cls type (and not a fictuous
 `DataclassInstance`) 
-_3_9_7 inst = typing.cast(C, cls(**to_load)) 
-_3_9_8 else: 
-_3_9_9 inst = cls(**init) 
-_4_0_0 to_load = check_and_convert_data(cls, data, inst.__dict__.keys(),
+_4_1_7 inst = typing.cast(C, cls(**to_load)) 
+_4_1_8 else: 
+_4_1_9 inst = cls(**init) 
+_4_2_0 to_load = check_and_convert_data(cls, data, inst.__dict__.keys(),
 strict=strict) 
-_4_0_1 inst.__dict__.update(**to_load) 
-_4_0_2 
-_4_0_3 return inst 
-_4_0_4 
-_4_0_5 
-_4_0_6def _load_into_instance( 
-_4_0_7 inst: C, 
-_4_0_8 cls: typing.Type[C], 
-_4_0_9 data: dict[str, typing.Any], 
-_4_1_0 init: dict[str, typing.Any] = None, 
-_4_1_1 strict: bool = True, 
-_4_1_2) -> C: 
-_4_1_3 """ 
-_4_1_4 Similar to `load_into_recurse` but uses an existing instance of a class (so
-after __init__) \ 
-_4_1_5 and thus does not support init. 
-_4_1_6 
-_4_1_7 """ 
-_4_1_8 if init is not None: 
-_4_1_9 raise ValueError("Can not init an existing instance!") 
-_4_2_0 
-_4_2_1 existing_data = inst.__dict__ 
+_4_2_1 inst.__dict__.update(**to_load) 
 _4_2_2 
-_4_2_3 to_load = check_and_convert_data(cls, data, _except=existing_data.keys(),
-strict=strict) 
+_4_2_3 return inst 
 _4_2_4 
-_4_2_5 inst.__dict__.update(**to_load) 
-_4_2_6 
-_4_2_7 return inst 
-_4_2_8 
-_4_2_9 
-_4_3_0def load_into_class( 
-_4_3_1 cls: typing.Type[C], 
-_4_3_2 data: T_data, 
-_4_3_3 /, 
-_4_3_4 key: str = None, 
-_4_3_5 init: dict[str, typing.Any] = None, 
-_4_3_6 strict: bool = True, 
-_4_3_7) -> C: 
-_4_3_8 """ 
-_4_3_9 Shortcut for _load_data + load_into_recurse. 
-_4_4_0 """ 
-_4_4_1 to_load = _load_data(data, key, cls.__name__) 
-_4_4_2 return _load_into_recurse(cls, to_load, init=init, strict=strict) 
-_4_4_3 
+_4_2_5 
+_4_2_6def _load_into_instance( 
+_4_2_7 inst: C, 
+_4_2_8 cls: typing.Type[C], 
+_4_2_9 data: dict[str, typing.Any], 
+_4_3_0 init: dict[str, typing.Any] = None, 
+_4_3_1 strict: bool = True, 
+_4_3_2) -> C: 
+_4_3_3 """ 
+_4_3_4 Similar to `load_into_recurse` but uses an existing instance of a class (so
+after __init__) \ 
+_4_3_5 and thus does not support init. 
+_4_3_6 
+_4_3_7 """ 
+_4_3_8 if init is not None: 
+_4_3_9 raise ValueError("Can not init an existing instance!") 
+_4_4_0 
+_4_4_1 existing_data = inst.__dict__ 
+_4_4_2 
+_4_4_3 to_load = check_and_convert_data(cls, data, _except=existing_data.keys(),
+strict=strict) 
 _4_4_4 
-_4_4_5def load_into_instance( 
-_4_4_6 inst: C, 
-_4_4_7 data: T_data, 
-_4_4_8 /, 
-_4_4_9 key: str = None, 
-_4_5_0 init: dict[str, typing.Any] = None, 
-_4_5_1 strict: bool = True, 
-_4_5_2) -> C: 
-_4_5_3 """ 
-_4_5_4 Shortcut for _load_data + load_into_existing. 
-_4_5_5 """ 
-_4_5_6 cls = inst.__class__ 
-_4_5_7 to_load = _load_data(data, key, cls.__name__) 
-_4_5_8 return _load_into_instance(inst, cls, to_load, init=init, strict=strict) 
-_4_5_9 
-_4_6_0 
-_4_6_1def load_into( 
-_4_6_2 cls: typing.Type[C], 
-_4_6_3 data: T_data, 
-_4_6_4 /, 
-_4_6_5 key: str = None, 
-_4_6_6 init: dict[str, typing.Any] = None, 
-_4_6_7 strict: bool = True, 
-_4_6_8) -> C: 
-_4_6_9 """ 
-_4_7_0 Load your config into a class (instance). 
-_4_7_1 
-_4_7_2 Supports both a class or an instance as first argument, but that's hard to
+_4_4_5 inst.__dict__.update(**to_load) 
+_4_4_6 
+_4_4_7 return inst 
+_4_4_8 
+_4_4_9 
+_4_5_0def load_into_class( 
+_4_5_1 cls: typing.Type[C], 
+_4_5_2 data: T_data, 
+_4_5_3 /, 
+_4_5_4 key: str = None, 
+_4_5_5 init: dict[str, typing.Any] = None, 
+_4_5_6 strict: bool = True, 
+_4_5_7) -> C: 
+_4_5_8 """ 
+_4_5_9 Shortcut for _load_data + load_into_recurse. 
+_4_6_0 """ 
+_4_6_1 to_load = _load_data(data, key, cls.__name__) 
+_4_6_2 return _load_into_recurse(cls, to_load, init=init, strict=strict) 
+_4_6_3 
+_4_6_4 
+_4_6_5def load_into_instance( 
+_4_6_6 inst: C, 
+_4_6_7 data: T_data, 
+_4_6_8 /, 
+_4_6_9 key: str = None, 
+_4_7_0 init: dict[str, typing.Any] = None, 
+_4_7_1 strict: bool = True, 
+_4_7_2) -> C: 
+_4_7_3 """ 
+_4_7_4 Shortcut for _load_data + load_into_existing. 
+_4_7_5 """ 
+_4_7_6 cls = inst.__class__ 
+_4_7_7 to_load = _load_data(data, key, cls.__name__) 
+_4_7_8 return _load_into_instance(inst, cls, to_load, init=init, strict=strict) 
+_4_7_9 
+_4_8_0 
+_4_8_1def load_into( 
+_4_8_2 cls: typing.Type[C], 
+_4_8_3 data: T_data, 
+_4_8_4 /, 
+_4_8_5 key: str = None, 
+_4_8_6 init: dict[str, typing.Any] = None, 
+_4_8_7 strict: bool = True, 
+_4_8_8) -> C: 
+_4_8_9 """ 
+_4_9_0 Load your config into a class (instance). 
+_4_9_1 
+_4_9_2 Supports both a class or an instance as first argument, but that's hard to
 explain to mypy, so officially only 
-_4_7_3 classes are supported, and if you want to `load_into` an instance, you
+_4_9_3 classes are supported, and if you want to `load_into` an instance, you
 should use `load_into_instance`. 
-_4_7_4 
-_4_7_5 Args: 
-_4_7_6 cls: either a class or an existing instance of that class. 
-_4_7_7 data: can be a dictionary or a path to a file to load (as pathlib.Path or
+_4_9_4 
+_4_9_5 Args: 
+_4_9_6 cls: either a class or an existing instance of that class. 
+_4_9_7 data: can be a dictionary or a path to a file to load (as pathlib.Path or
 str) 
-_4_7_8 key: optional (nested) dictionary key to load data from (e.g.
+_4_9_8 key: optional (nested) dictionary key to load data from (e.g.
 'tool.su6.specific') 
-_4_7_9 init: optional data to pass to your cls' __init__ method (only if cls is
+_4_9_9 init: optional data to pass to your cls' __init__ method (only if cls is
 not an instance already) 
-_4_8_0 strict: enable type checks or allow anything? 
-_4_8_1 
-_4_8_2 """ 
-_4_8_3 if not isinstance(cls, type): 
-_4_8_4 # would not be supported according to mypy, but you can still load_into
+_5_0_0 strict: enable type checks or allow anything? 
+_5_0_1 
+_5_0_2 """ 
+_5_0_3 if not isinstance(cls, type): 
+_5_0_4 # would not be supported according to mypy, but you can still load_into
 (instance) 
-_4_8_5 return load_into_instance(cls, data, key=key, init=init, strict=strict) 
-_4_8_6 
-_4_8_7 # make mypy and pycharm happy by telling it cls is of type C and not just
+_5_0_5 return load_into_instance(cls, data, key=key, init=init, strict=strict) 
+_5_0_6 
+_5_0_7 # make mypy and pycharm happy by telling it cls is of type C and not just
 'type' 
-_4_8_8 # _cls = typing.cast(typing.Type[C], cls) 
-_4_8_9 return load_into_class(cls, data, key=key, init=init, strict=strict) 
+_5_0_8 # _cls = typing.cast(typing.Type[C], cls) 
+_5_0_9 return load_into_class(cls, data, key=key, init=init, strict=strict) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-19 17:38 +0200
+22 14:32 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/dump.py: 100%</title>
+    <title>Coverage for src/configuraptor/errors.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/errors.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">31 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
+            <span class="text">46 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">46<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:50 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,84 +77,163 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Method to dump classes to other formats.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains module-specific custom errors.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">dataclasses</span> <span class="key">import</span> <span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">instance_of_custom_class</span><span class="op">,</span> <span class="nam">is_custom_class</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Base exception class for this module.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_level</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">0</span><span class="op">,</span> <span class="op">/</span><span class="op">,</span> <span class="nam">with_top_level_key</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Dump a config instance to a dictionary (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">cls</span> <span class="op">=</span> <span class="nam">value</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">asdict</span><span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">_</span><span class="op">)</span> <span class="key">else</span> <span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">else</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">data</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">if</span> <span class="nam">_level</span> <span class="op">==</span> <span class="num">0</span> <span class="key">and</span> <span class="nam">with_top_level_key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="com"># top-level: add an extra key indicating the class' name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">cls_name</span> <span class="op">=</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="nam">cls_name</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    Dump a config instance to toml (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">tomli_w</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">=</span><span class="nam">multiline_strings</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    Dump a config instance to json (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># class ConfigErrorGroup(ConfigError, ExceptionGroup):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="com">#     Base Exception class for this module, but for exception groups (3.11+)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="com">#     def __init__(self, _type: str, errors: list[Exception]):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com">#         more = len(errors) > 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="com">#         cnt = "Multiple" if more else "One"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="com">#         s = "s" if more else ""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="com">#         message = f"{cnt} {_type}{s} in config!"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="com">#         super().__init__(message, errors)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="com">#         if not errors:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="com">#             raise ValueError("Error group raised without any errors?")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    Exception for when the config file is missing a required key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">annotated_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        Automatically filles in the names of annotated type and cls for printing from __str__.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_annotated_type</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="str">f"Config key '{self.key}' (type `{self._annotated_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="str">f"of class `{self._cls}` was not found in the config, "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="str">f"but is required as a default value is not specified."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Dump a config instance to yaml (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">output</span> <span class="op">=</span> <span class="nam">yaml</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="com"># output is already a str but mypy doesn't know that</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    Exception for when the config file is missing a required key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        Automatically filles in the names of annotated type and cls for printing from __str__.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="str">f"Config key '{self.key}' (value: `{self.value}` type `{self._type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="str">f"does not exist on class `{self._cls}`, but was attempted to be updated. "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="str">f"Use strict = False to allow this behavior."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">    Exception for when the config file contains a key with an unexpected type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">        Store the actual type of the config variable.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">actual_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">max_len</span> <span class="op">=</span> <span class="num">50</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_value</span><span class="op">)</span> <span class="op">></span> <span class="nam">max_len</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="str">f"{self._value[:max_len]}..."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">            <span class="str">f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">            <span class="str">f"that was not expected: `{self.expected_type}` is the required type."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorImmutable</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="str">    Raised when an immutable Mapping is attempted to be updated.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">        Store the class name.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">        Custom error message.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="key">return</span> <span class="str">f"{self._cls} is Immutable!"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="key">class</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="str">    Error thrown when you try to access a 'postponed' property without filling its value first.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"This postponed property has not been filled yet!"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:50 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,81 +1,162 @@
-************ CCoovveerraaggee ffoorr ssrrcc//ccoonnffiigguurraappttoorr//dduummpp..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//ccoonnffiigguurraappttoorr//eerrrroorrss..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3311 ssttaatteemmeennttss ?  3311 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 4466 ssttaatteemmeennttss ?  4466 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-20 10:44 +0200
+22 13:50 +0200
 _1""" 
-_2Method to dump classes to other formats. 
+_2Contains module-specific custom errors. 
 _3""" 
-_4 
-_5import json 
-_6import typing 
+_4import typing 
+_5from dataclasses import dataclass 
+_6 
 _7 
-_8import tomli_w 
-_9import yaml 
-_1_0 
-_1_1from .core import instance_of_custom_class, is_custom_class 
-_1_2from .helpers import camel_to_snake 
+_8class ConfigError(Exception): 
+_9 """ 
+_1_0 Base exception class for this module. 
+_1_1 """ 
+_1_2 
 _1_3 
-_1_4 
-_1_5def asdict(inst: typing.Any, _level: int = 0, /, with_top_level_key: bool =
-True) -> dict[str, typing.Any]: 
-_1_6 """ 
-_1_7 Dump a config instance to a dictionary (recursively). 
-_1_8 """ 
-_1_9 data = {} 
-_2_0 
-_2_1 for key, value in inst.__dict__.items(): 
-_2_2 cls = value.__class__ 
-_2_3 if is_custom_class(cls): 
-_2_4 value = asdict(value, _level + 1) 
-_2_5 elif isinstance(value, list): 
-_2_6 value = [asdict(_, _level + 1) if instance_of_custom_class(_) else _ for _
-in value] 
-_2_7 elif isinstance(value, dict): 
-_2_8 value = {k: asdict(v, _level + 1) if instance_of_custom_class(v) else v for
-k, v in value.items()} 
-_2_9 
-_3_0 data[key] = value 
-_3_1 
-_3_2 if _level == 0 and with_top_level_key: 
-_3_3 # top-level: add an extra key indicating the class' name 
-_3_4 cls_name = camel_to_snake(inst.__class__.__name__) 
-_3_5 return {cls_name: data} 
-_3_6 
-_3_7 return data 
-_3_8 
-_3_9 
-_4_0def astoml(inst: typing.Any, multiline_strings: bool = False) -> str: 
+_1_4# class ConfigErrorGroup(ConfigError, ExceptionGroup): 
+_1_5# """ 
+_1_6# Base Exception class for this module, but for exception groups (3.11+) 
+_1_7# """ 
+_1_8# def __init__(self, _type: str, errors: list[Exception]): 
+_1_9# more = len(errors) > 1 
+_2_0# cnt = "Multiple" if more else "One" 
+_2_1# s = "s" if more else "" 
+_2_2# message = f"{cnt} {_type}{s} in config!" 
+_2_3# super().__init__(message, errors) 
+_2_4# if not errors: 
+_2_5# raise ValueError("Error group raised without any errors?") 
+_2_6 
+_2_7 
+_2_8@dataclass 
+_2_9class ConfigErrorMissingKey(ConfigError): 
+_3_0 """ 
+_3_1 Exception for when the config file is missing a required key. 
+_3_2 """ 
+_3_3 
+_3_4 key: str 
+_3_5 cls: type 
+_3_6 annotated_type: type 
+_3_7 
+_3_8 def __post_init__(self) -> None: 
+_3_9 """ 
+_4_0 Automatically filles in the names of annotated type and cls for printing
+from __str__. 
 _4_1 """ 
-_4_2 Dump a config instance to toml (recursively). 
-_4_3 """ 
-_4_4 data = asdict(inst) 
-_4_5 return tomli_w.dumps(data, multiline_strings=multiline_strings) 
-_4_6 
-_4_7 
-_4_8def asjson(inst: typing.Any, **kw: typing.Any) -> str: 
-_4_9 """ 
-_5_0 Dump a config instance to json (recursively). 
-_5_1 """ 
-_5_2 data = asdict(inst) 
-_5_3 return json.dumps(data, **kw) 
+_4_2 self._annotated_type = getattr(self.annotated_type, "__name__", str
+(self.annotated_type)) 
+_4_3 self._cls = self.cls.__name__ 
+_4_4 
+_4_5 def __str__(self) -> str: 
+_4_6 """ 
+_4_7 Custom error message based on dataclass values and calculated actual type. 
+_4_8 """ 
+_4_9 return ( 
+_5_0 f"Config key '{self.key}' (type `{self._annotated_type}`) " 
+_5_1 f"of class `{self._cls}` was not found in the config, " 
+_5_2 f"but is required as a default value is not specified." 
+_5_3 ) 
 _5_4 
 _5_5 
-_5_6def asyaml(inst: typing.Any, **kw: typing.Any) -> str: 
-_5_7 """ 
-_5_8 Dump a config instance to yaml (recursively). 
-_5_9 """ 
-_6_0 data = asdict(inst) 
-_6_1 output = yaml.dump(data, encoding=None, **kw) 
-_6_2 # output is already a str but mypy doesn't know that 
-_6_3 return typing.cast(str, output) 
+_5_6@dataclass 
+_5_7class ConfigErrorExtraKey(ConfigError): 
+_5_8 """ 
+_5_9 Exception for when the config file is missing a required key. 
+_6_0 """ 
+_6_1 
+_6_2 key: str 
+_6_3 value: str 
+_6_4 cls: type 
+_6_5 
+_6_6 def __post_init__(self) -> None: 
+_6_7 """ 
+_6_8 Automatically filles in the names of annotated type and cls for printing
+from __str__. 
+_6_9 """ 
+_7_0 self._cls = self.cls.__name__ 
+_7_1 self._type = type(self.value) 
+_7_2 
+_7_3 def __str__(self) -> str: 
+_7_4 """ 
+_7_5 Custom error message based on dataclass values and calculated actual type. 
+_7_6 """ 
+_7_7 return ( 
+_7_8 f"Config key '{self.key}' (value: `{self.value}` type `{self._type}`) " 
+_7_9 f"does not exist on class `{self._cls}`, but was attempted to be updated. " 
+_8_0 f"Use strict = False to allow this behavior." 
+_8_1 ) 
+_8_2 
+_8_3 
+_8_4@dataclass 
+_8_5class ConfigErrorInvalidType(ConfigError): 
+_8_6 """ 
+_8_7 Exception for when the config file contains a key with an unexpected type. 
+_8_8 """ 
+_8_9 
+_9_0 key: str 
+_9_1 value: typing.Any 
+_9_2 expected_type: type 
+_9_3 
+_9_4 def __post_init__(self) -> None: 
+_9_5 """ 
+_9_6 Store the actual type of the config variable. 
+_9_7 """ 
+_9_8 self.actual_type = type(self.value) 
+_9_9 
+_1_0_0 max_len = 50 
+_1_0_1 self._value = str(self.value) 
+_1_0_2 if len(self._value) > max_len: 
+_1_0_3 self._value = f"{self._value[:max_len]}..." 
+_1_0_4 
+_1_0_5 def __str__(self) -> str: 
+_1_0_6 """ 
+_1_0_7 Custom error message based on dataclass values and calculated actual type. 
+_1_0_8 """ 
+_1_0_9 return ( 
+_1_1_0 f"Config key '{self.key}' had a value (`{self._value}`) with a type (`
+{self.actual_type}`) " 
+_1_1_1 f"that was not expected: `{self.expected_type}` is the required type." 
+_1_1_2 ) 
+_1_1_3 
+_1_1_4 
+_1_1_5@dataclass 
+_1_1_6class ConfigErrorImmutable(ConfigError): 
+_1_1_7 """ 
+_1_1_8 Raised when an immutable Mapping is attempted to be updated. 
+_1_1_9 """ 
+_1_2_0 
+_1_2_1 cls: type 
+_1_2_2 
+_1_2_3 def __post_init__(self) -> None: 
+_1_2_4 """ 
+_1_2_5 Store the class name. 
+_1_2_6 """ 
+_1_2_7 self._cls = self.cls.__name__ 
+_1_2_8 
+_1_2_9 def __str__(self) -> str: 
+_1_3_0 """ 
+_1_3_1 Custom error message. 
+_1_3_2 """ 
+_1_3_3 return f"{self._cls} is Immutable!" 
+_1_3_4 
+_1_3_5 
+_1_3_6@dataclass 
+_1_3_7class IsPostponedError(ConfigError): 
+_1_3_8 """ 
+_1_3_9 Error thrown when you try to access a 'postponed' property without filling
+its value first. 
+_1_4_0 """ 
+_1_4_1 
+_1_4_2 message: str = "This postponed property has not been filled yet!" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-20 10:44 +0200
+22 13:50 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">13 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">13<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -94,15 +94,15 @@
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    Can be used as a metaclass:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">        class AbstractConfig(metaclass=Singleton):</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Source: https://stackoverflow.com/questions/6760685/creating-a-singleton-in-python</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">_instances</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">_instances</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">ClassVar</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        When a class is instantiated (e.g. `AbstractConfig()`), __call__ is called. This overrides the default behavior.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_instances</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_instances</span><span class="op">[</span><span class="nam">self</span><span class="op">]</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="nam">SingletonMeta</span><span class="op">,</span> <span class="nam">self</span><span class="op">)</span><span class="op">.</span><span class="nam">__call__</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
@@ -126,18 +126,18 @@
     <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    Mixin to make a class a singleton.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1133 ssttaatteemmeennttss ?  1133 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-14 11:42 +0200
+22 13:07 +0200
 _1""" 
 _2Singleton mixin/metaclass. 
 _3""" 
 _4 
 _5import typing 
 _6 
 _7 
@@ -26,15 +26,16 @@
 _1_3 Example: 
 _1_4 class AbstractConfig(metaclass=Singleton): 
 _1_5 
 _1_6 Source: https://stackoverflow.com/questions/6760685/creating-a-singleton-in-
 python 
 _1_7 """ 
 _1_8 
-_1_9 _instances: dict[typing.Type[typing.Any], typing.Type[typing.Any]] = {} 
+_1_9 _instances: typing.ClassVar[dict[typing.Type[typing.Any], typing.Type
+[typing.Any]]] = {} 
 _2_0 
 _2_1 def __call__(self, *args: typing.Any, **kwargs: typing.Any) -> typing.Type
 [typing.Any]: 
 _2_2 """ 
 _2_3 When a class is instantiated (e.g. `AbstractConfig()`), __call__ is called.
 This overrides the default behavior. 
 _2_4 """ 
@@ -58,8 +59,8 @@
 _4_1 
 _4_2 
 _4_3class Singleton(metaclass=SingletonMeta): 
 _4_4 """ 
 _4_5 Mixin to make a class a singleton. 
 _4_6 """ 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-
-14 11:42 +0200
+22 13:07 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/favicon_32.png` & `configuraptor-1.9.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/index.html` & `configuraptor-1.9.2/htmlcov/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,39 +73,39 @@
                 <td>6</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_cls_py.html">src/configuraptor/cls.py</a></td>
-                <td>24</td>
+                <td>51</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="24 24">100%</td>
+                <td class="right" data-ratio="51 51">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_core_py.html">src/configuraptor/core.py</a></td>
-                <td>156</td>
+                <td>166</td>
                 <td>0</td>
-                <td>3</td>
-                <td class="right" data-ratio="156 156">100%</td>
+                <td>5</td>
+                <td class="right" data-ratio="166 166">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_dump_py.html">src/configuraptor/dump.py</a></td>
                 <td>31</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="31 31">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_errors_py.html">src/configuraptor/errors.py</a></td>
-                <td>39</td>
+                <td>46</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="39 39">100%</td>
+                <td class="right" data-ratio="46 46">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_helpers_py.html">src/configuraptor/helpers.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
@@ -145,30 +145,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>310</td>
+                <td>354</td>
                 <td>0</td>
-                <td>3</td>
-                <td class="right" data-ratio="310 310">100%</td>
+                <td>5</td>
+                <td class="right" data-ratio="354 354">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html"/>
         <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 ************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-21 15:50 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-22 14:32 +0200
 MMoodduullee                                ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_____a_b_o_u_t_____._p_y        1          0       0        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_____i_n_i_t_____._p_y         6          0       0        100%
-_s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_c_l_s_._p_y              24         0       0        100%
-_s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_c_o_r_e_._p_y             156        0       3        100%
+_s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_c_l_s_._p_y              51         0       0        100%
+_s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_c_o_r_e_._p_y             166        0       5        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_d_u_m_p_._p_y             31         0       0        100%
-_s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_e_r_r_o_r_s_._p_y           39         0       0        100%
+_s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_e_r_r_o_r_s_._p_y           46         0       0        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_h_e_l_p_e_r_s_._p_y          2          0       0        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_l_o_a_d_e_r_s_/_____i_n_i_t_____._p_y 11         0       0        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_l_o_a_d_e_r_s_/___t_y_p_e_s_._p_y   4          0       0        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_l_o_a_d_e_r_s_/            14         0       0        100%
 _l_o_a_d_e_r_s___s_h_a_r_e_d_._p_y
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_p_o_s_t_p_o_n_e_._p_y         9          0       0        100%
 _s_r_c_/_c_o_n_f_i_g_u_r_a_p_t_o_r_/_s_i_n_g_l_e_t_o_n_._p_y        13         0       0        100%
-Total                                 310        0       3        100%
+Total                                 354        0       5        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-21 15:50 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._7, created at 2023-06-22 14:32 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/keybd_closed.png` & `configuraptor-1.9.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/keybd_open.png` & `configuraptor-1.9.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/status.json` & `configuraptor-1.9.2/htmlcov/status.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996162037037037%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': 'f3d6090fee225db883989217e2a740bf'}, "*

 * *            "'d_eb75b6cf8f5eab40___init___py': {'hash': 'fcf8563f24b1586e1a72722455863f60'}, "*

 * *            "'d_eb75b6cf8f5eab40_cls_py': {'hash': '4eb0bef0088cbc7c1cd0ac424bf43b42', 'index': "*

 * *            "{'nums': {insert: [(2, 51)], delete: [2]}}}, 'd_eb75b6cf8f5eab40_core_py': {'hash': "*

 * *            "'1980a48acff8d9458e8ee05729ad82cd', 'index': {'nums': {insert: [(2, 166), (3, 5)], "*

 * *            "delete: [3,  […]*

```diff
@@ -269,15 +269,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
             }
         },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "3e93cb54154f78c6f81f6feef3376f69",
+            "hash": "f3d6090fee225db883989217e2a740bf",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -286,15 +286,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__about__.py"
             }
         },
         "d_eb75b6cf8f5eab40___init___py": {
-            "hash": "d5c1f5ac693aae2044dffde7eccaae57",
+            "hash": "fcf8563f24b1586e1a72722455863f60",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___init___py.html",
                 "nums": [
                     0,
                     1,
                     6,
                     0,
@@ -303,39 +303,39 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__init__.py"
             }
         },
         "d_eb75b6cf8f5eab40_cls_py": {
-            "hash": "b1f068469f7f94c16e9d267b087e8806",
+            "hash": "4eb0bef0088cbc7c1cd0ac424bf43b42",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_cls_py.html",
                 "nums": [
                     0,
                     1,
-                    24,
+                    51,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
             }
         },
         "d_eb75b6cf8f5eab40_core_py": {
-            "hash": "000fc824ee5ffb18202f5e36ed1843ec",
+            "hash": "1980a48acff8d9458e8ee05729ad82cd",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_core_py.html",
                 "nums": [
                     0,
                     1,
-                    156,
-                    3,
+                    166,
+                    5,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
             }
@@ -354,21 +354,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/dump.py"
             }
         },
         "d_eb75b6cf8f5eab40_errors_py": {
-            "hash": "f59126ae493adc32aa6331d7fc163d94",
+            "hash": "c246b517d164adf3fa3f9a012132c89f",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_errors_py.html",
                 "nums": [
                     0,
                     1,
-                    39,
+                    46,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/errors.py"
@@ -405,15 +405,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/postpone.py"
             }
         },
         "d_eb75b6cf8f5eab40_singleton_py": {
-            "hash": "0e6e4db931998b4489d5c07b70fcbef5",
+            "hash": "b7f8b3ec8c29f6bec4d56f56dee1396c",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_singleton_py.html",
                 "nums": [
                     0,
                     1,
                     13,
                     0,
```

### Comparing `configuraptor-1.8.0/htmlcov/style.css` & `configuraptor-1.9.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/pytest_examples/some.toml` & `configuraptor-1.9.2/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/__init__.py` & `configuraptor-1.9.2/src/configuraptor/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Exposes TypedConfig and load_into for this library.
 """
 
 # SPDX-FileCopyrightText: 2023-present Robin van der Noord <robinvandernoord@gmail.com>
 #
 # SPDX-License-Identifier: MIT
-from .cls import TypedConfig, update
+from .cls import TypedConfig, TypedMapping, TypedMutableMapping, update
 from .core import (
     all_annotations,
     check_and_convert_data,
     convert_config,
     ensure_types,
     load_into,
     load_into_class,
@@ -18,14 +18,16 @@
 from .dump import asdict, asjson, astoml, asyaml
 from .postpone import postpone
 from .singleton import Singleton, SingletonMeta
 
 __all__ = [
     # cls
     "TypedConfig",
+    "TypedMapping",
+    "TypedMutableMapping",
     "update",
     # singleton
     "Singleton",
     "SingletonMeta",
     # core
     "all_annotations",
     "check_and_convert_data",
```

### Comparing `configuraptor-1.8.0/src/configuraptor/core.py` & `configuraptor-1.9.2/src/configuraptor/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """
     If no key is manually defined for `load_into`, \
     the class' name is converted to snake_case to use as the default key.
     """
     return camel_to_snake(clsname)
 
 
-def _load_data(data: T_data, key: str = None, classname: str = None) -> dict[str, typing.Any]:
+def __load_data(data: T_data, key: str = None, classname: str = None) -> dict[str, typing.Any]:
     """
     Tries to load the right data from a filename/path or dict, based on a manual key or a classname.
 
     E.g. class Tool will be mapped to key tool.
     It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}
     """
     if isinstance(data, str):
@@ -75,18 +75,39 @@
         # try to guess key by grabbing the first one or using the class name
         if len(data) == 1:
             key = list(data.keys())[0]
         elif classname is not None:
             key = _guess_key(classname)
 
     if key:
-        return _data_for_nested_key(key, data)
-    else:
-        # no key found, just return all data
-        return data
+        data = _data_for_nested_key(key, data)
+
+    if not data:
+        raise ValueError("No data found!")
+
+    if not isinstance(data, dict):
+        raise ValueError("Data is not a dict!")
+
+    return data
+
+
+def _load_data(data: T_data, key: str = None, classname: str = None) -> dict[str, typing.Any]:
+    """
+    Wrapper around __load_data that retries with key="" if anything goes wrong.
+    """
+    try:
+        return __load_data(data, key, classname)
+    except Exception as e:
+        if key != "":
+            return __load_data(data, "", classname)
+        else:  # pragma: no cover
+            warnings.warn(f"Data could not be loaded: {e}", source=e)
+            # key already was "", just return data!
+            # (will probably not happen but fallback)
+            return {}
 
 
 def check_type(value: typing.Any, expected_type: T_typelike) -> bool:
     """
     Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).
 
     Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError
```

### Comparing `configuraptor-1.8.0/src/configuraptor/dump.py` & `configuraptor-1.9.2/src/configuraptor/dump.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/errors.py` & `configuraptor-1.9.2/src/configuraptor/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,13 +109,34 @@
         return (
             f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "
             f"that was not expected: `{self.expected_type}` is the required type."
         )
 
 
 @dataclass
+class ConfigErrorImmutable(ConfigError):
+    """
+    Raised when an immutable Mapping is attempted to be updated.
+    """
+
+    cls: type
+
+    def __post_init__(self) -> None:
+        """
+        Store the class name.
+        """
+        self._cls = self.cls.__name__
+
+    def __str__(self) -> str:
+        """
+        Custom error message.
+        """
+        return f"{self._cls} is Immutable!"
+
+
+@dataclass
 class IsPostponedError(ConfigError):
     """
     Error thrown when you try to access a 'postponed' property without filling its value first.
     """
 
     message: str = "This postponed property has not been filled yet!"
```

### Comparing `configuraptor-1.8.0/src/configuraptor/postpone.py` & `configuraptor-1.9.2/src/configuraptor/postpone.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/singleton.py` & `configuraptor-1.9.2/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/loaders/__init__.py` & `configuraptor-1.9.2/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/loaders/loaders_shared.py` & `configuraptor-1.9.2/src/configuraptor/loaders/loaders_shared.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_core.py` & `configuraptor-1.9.2/tests/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,31 +5,51 @@
 
 import pytest
 
 from src.configuraptor import all_annotations
 from src.configuraptor.core import is_optional
 from tests.constants import EXAMPLE_FILE
 
+
 def test_invalid_extension():
     from src.configuraptor.loaders import get
 
     with pytest.raises(ValueError):
         get(".doesntexist")
 
 
 def test_is_optional_with_weird_inputs():
     assert is_optional(math.nan) is False
     assert is_optional(typing.Optional[dict[str, typing.Optional[str]]]) is True
 
+
 class Base:
     has: int
 
 
 class Sub(Base):
     has_also: int
 
 
 def test_all_annotations():
     # without except:
     assert set(all_annotations(Sub).keys()) == {"has", "has_also"}
     # with except:
     assert set(all_annotations(Sub, {"has_also"}).keys()) == {"has"}
+
+
+def test_no_data():
+    from src import configuraptor
+
+    # data must be a dict:
+    with pytest.raises(ValueError):
+        configuraptor.core._load_data(42, key=None)
+    with pytest.raises(ValueError):
+        configuraptor.core._load_data(["joe"], key=None)
+
+    # but other than that, it should be fine:
+    configuraptor.core._load_data({}, key="")
+    configuraptor.core._load_data({}, key=None)
+    configuraptor.core._load_data({"-": 0, "+": None}, key="joe", classname="-.+")
+    configuraptor.core._load_data({"-": 0, "+": None}, key="+", classname="-.+")
+    configuraptor.core._load_data({"-": 0, "+": None}, key="", classname="-.+")
+    configuraptor.core._load_data({"-": 0, "+": None}, key=None, classname="-.+")
```

### Comparing `configuraptor-1.8.0/tests/test_dumps.py` & `configuraptor-1.9.2/tests/test_dumps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import typing
 
 import tomli_w
 import yaml
 
 from src.configuraptor import TypedConfig
-from src.configuraptor.dump import asdict, asyaml, asjson, astoml
+from src.configuraptor.dump import asdict, asjson, astoml, asyaml
 
 
 class Simple(TypedConfig):
     key: str
     num: int
```

### Comparing `configuraptor-1.8.0/tests/test_json_yaml.py` & `configuraptor-1.9.2/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_postponed.py` & `configuraptor-1.9.2/tests/test_postponed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pytest
 
-from src.configuraptor import TypedConfig, Singleton, postpone
+from src.configuraptor import Singleton, TypedConfig, postpone
 from src.configuraptor.errors import IsPostponedError
 
 
 class Later(TypedConfig, Singleton):
     field: str  # instant
     other_field: str = postpone()
 
     def update(self):
         self.other_field = "usable"
 
 
-later = Later.load({"field": "instant"}, key="")
+later = Later.load({"field": "instant"})
 
 
 def test_postponed_can_be_filled_later():
     # later should be able to exist
     assert later
     assert later.field
     print(later, later.field)
```

### Comparing `configuraptor-1.8.0/tests/test_singleton.py` & `configuraptor-1.9.2/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_toml_basic.py` & `configuraptor-1.9.2/tests/test_toml_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     relevant = configuraptor.load_into(Relevant, file)
     assert relevant and relevant.key == "this one!"
 
 
 def test_guess_key_no_match():
     file = str(PYTEST_EXAMPLES / "with_multiple_toplevel_keys.toml")
     # no key and no match by class name:
-    relevant = configuraptor.load_into(Irrelevant, file, key="")
+    relevant = configuraptor.load_into(Irrelevant, file)
     assert relevant and relevant.key["value"] == "fallback"
 
 
 class TooLong:
     type: str
 
 
@@ -195,8 +195,8 @@
     not_required: typing.Optional[list[str]]
 
 
 def test_missing_required_parameterized():
     # should go through is_optional -> is_parameterized -> typing.get_origin(_type) in (dict, list) -> False -> Error
     data = {"not_required": ["list", "of", "string"]}
     with pytest.raises(ConfigErrorMissingKey):
-        configuraptor.load_into(ShouldHaveListOfString, data, key="")  # empty key to indicate data exists top-level
+        configuraptor.load_into(ShouldHaveListOfString, data)
```

### Comparing `configuraptor-1.8.0/tests/test_toml_dataclass.py` & `configuraptor-1.9.2/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_toml_existing.py` & `configuraptor-1.9.2/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/LICENSE.txt` & `configuraptor-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/README.md` & `configuraptor-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/pyproject.toml` & `configuraptor-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 upload_to_release = false
 build_command = "hatch build"
 
 [tool.su6]
 directory = "src"
 include = []
 exclude = []
-stop-after-first-failure = false
+stop-after-first-failure = true
 coverage = 100
 badge = true
 
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
```

### Comparing `configuraptor-1.8.0/PKG-INFO` & `configuraptor-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.8.0
+Version: 1.9.2
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

