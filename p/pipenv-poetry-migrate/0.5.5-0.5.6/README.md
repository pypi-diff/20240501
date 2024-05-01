# Comparing `tmp/pipenv_poetry_migrate-0.5.5.tar.gz` & `tmp/pipenv_poetry_migrate-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipenv_poetry_migrate-0.5.5.tar", max compression
+gzip compressed data, was "pipenv_poetry_migrate-0.5.6.tar", max compression
```

## Comparing `pipenv_poetry_migrate-0.5.5.tar` & `pipenv_poetry_migrate-0.5.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/LICENSE
--rw-r--r--   0        0        0     4243 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/README.md
--rw-r--r--   0        0        0      100 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/__init__.py
--rw-r--r--   0        0        0     2360 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/cli.py
--rw-r--r--   0        0        0      702 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/loader.py
--rw-r--r--   0        0        0     5701 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/migrate.py
--rw-r--r--   0        0        0      425 2024-04-01 09:21:38.589063 pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/translator.py
--rw-r--r--   0        0        0     2241 2024-04-01 09:21:57.064965 pipenv_poetry_migrate-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 pipenv_poetry_migrate-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-03-30 14:07:21.424255 pipenv_poetry_migrate-0.5.6/LICENSE
+-rw-r--r--   0        0        0     4243 2024-04-01 09:14:13.834526 pipenv_poetry_migrate-0.5.6/README.md
+-rw-r--r--   0        0        0      100 2021-04-19 07:17:13.649654 pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/__init__.py
+-rw-r--r--   0        0        0     2360 2023-11-07 17:11:02.621797 pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/cli.py
+-rw-r--r--   0        0        0      702 2023-05-09 14:29:09.368905 pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/loader.py
+-rw-r--r--   0        0        0     5701 2023-10-31 14:58:39.373678 pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/migrate.py
+-rw-r--r--   0        0        0      425 2023-12-06 14:58:08.453347 pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/translator.py
+-rw-r--r--   0        0        0     2324 2024-05-01 00:28:08.743198 pipenv_poetry_migrate-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 pipenv_poetry_migrate-0.5.6/PKG-INFO
```

### Comparing `pipenv_poetry_migrate-0.5.5/LICENSE` & `pipenv_poetry_migrate-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipenv_poetry_migrate-0.5.5/README.md` & `pipenv_poetry_migrate-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/cli.py` & `pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/loader.py` & `pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/loader.py`

 * *Files identical despite different names*

### Comparing `pipenv_poetry_migrate-0.5.5/pipenv_poetry_migrate/migrate.py` & `pipenv_poetry_migrate-0.5.6/pipenv_poetry_migrate/migrate.py`

 * *Files identical despite different names*

### Comparing `pipenv_poetry_migrate-0.5.5/pyproject.toml` & `pipenv_poetry_migrate-0.5.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipenv-poetry-migrate"
-version = "0.5.5"
+version = "0.5.6"
 description = "simple migration script, migrate pipenv to poetry"
 authors = ["Yoshiyuki HINO <yhinoz@gmail.com>"]
 license = "Apache-2.0"
 repository = 'https://github.com/yhino/pipenv-poetry-migrate'
 homepage = 'https://github.com/yhino/pipenv-poetry-migrate'
 readme = 'README.md'
 
@@ -13,17 +13,17 @@
 tomlkit = "^0.12.1"
 typer = ">=0.9,<0.13"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
 pytest-cov = ">=4.1,<6.0"
 mypy = "^1.6.1"
-python-semantic-release = "^7.15.3"
+python-semantic-release = "^9.4.1"
 types-setuptools = ">=68.2,<70.0"
-ruff = ">=0.1.3,<0.4.0"
+ruff = ">=0.1.3,<0.5.0"
 
 [tool.poetry.scripts]
 pipenv-poetry-migrate = "pipenv_poetry_migrate.cli:app"
 
 [tool.isort]
 py_version = 38
 profile = "black"
@@ -59,18 +59,22 @@
 
 [tool.mypy]
 python_version = 3.8
 strict = true
 ignore_missing_imports = true
 
 [tool.semantic_release]
-branch = "main"
-version_toml = "pyproject.toml:tool.poetry.version"
-commit_parser = "semantic_release.history.emoji_parser"
-major_emoji = ":boom:"
-minor_emoji = ":sparkles:,:children_crossing:,:lipstick:,:iphone:,:egg:,:chart_with_upwards_trend:"
-patch_emoji = ":ambulance:,:lock:,:arrow_up:,:bug:,:zap:,:goal_net:,:alien:,:wheelchair:,:speech_balloon:,:mag:,:apple:,:penguin:,:checkered_flag:,:robot:,:green_apple:"
-build_command = "poetry build"
+version_toml = ["pyproject.toml:tool.poetry.version"]
+commit_parser = "emoji"
+
+[tool.semantic_release.branches.main]
+match = "main"
+prerelease = false
+
+[tool.semantic_release.commit_parser_options]
+major_tags = [":boom:"]
+minor_tags = [":sparkles:",":children_crossing:",":lipstick:",":iphone:",":egg:",":chart_with_upwards_trend:"]
+patch_tags = [":ambulance:",":lock:",":arrow_up:",":bug:",":zap:",":goal_net:",":alien:",":wheelchair:",":speech_balloon:",":mag:",":apple:",":penguin:",":checkered_flag:",":robot:",":green_apple:"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pipenv_poetry_migrate-0.5.5/PKG-INFO` & `pipenv_poetry_migrate-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipenv-poetry-migrate
-Version: 0.5.5
+Version: 0.5.6
 Summary: simple migration script, migrate pipenv to poetry
 Home-page: https://github.com/yhino/pipenv-poetry-migrate
 License: Apache-2.0
 Author: Yoshiyuki HINO
 Author-email: yhinoz@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipenv-poetry-migrate Version: 0.5.5 Summary:
+Metadata-Version: 2.1 Name: pipenv-poetry-migrate Version: 0.5.6 Summary:
 simple migration script, migrate pipenv to poetry Home-page: https://
 github.com/yhino/pipenv-poetry-migrate License: Apache-2.0 Author: Yoshiyuki
 HINO Author-email: yhinoz@gmail.com Requires-Python: >=3.8.1,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

