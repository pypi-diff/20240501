# Comparing `tmp/safety-3.0.1.tar.gz` & `tmp/safety-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safety-3.0.1.tar", last modified: Sat Jan 20 03:08:22 2024, max compression
+gzip compressed data, was "safety-3.1.0.tar", last modified: Tue Mar 26 03:11:08 2024, max compression
```

## Comparing `safety-3.0.1.tar` & `safety-3.1.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    24035 2024-01-20 03:08:13.000000 safety-3.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-20 03:08:13.000000 safety-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-20 03:08:13.000000 safety-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-01-20 03:08:22.493777 safety-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-01-20 03:08:13.000000 safety-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-20 03:08:13.000000 safety-3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.477777 safety-3.0.1/safety/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-20 03:08:13.000000 safety-3.0.1/safety/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-20 03:08:13.000000 safety-3.0.1/safety/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-20 03:08:13.000000 safety-3.0.1/safety/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.481777 safety-3.0.1/safety/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-01-20 03:08:13.000000 safety-3.0.1/safety/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-01-20 03:08:13.000000 safety-3.0.1/safety/alerts/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-01-20 03:08:13.000000 safety-3.0.1/safety/alerts/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.481777 safety-3.0.1/safety/alerts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-01-20 03:08:13.000000 safety-3.0.1/safety/alerts/templates/issue.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-01-20 03:08:13.000000 safety-3.0.1/safety/alerts/templates/pr.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-01-20 03:08:13.000000 safety-3.0.1/safety/alerts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.481777 safety-3.0.1/safety/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-01-20 03:08:13.000000 safety-3.0.1/safety/auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32425 2024-01-20 03:08:13.000000 safety-3.0.1/safety/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    22376 2024-01-20 03:08:13.000000 safety-3.0.1/safety/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/safety/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-01-20 03:08:13.000000 safety-3.0.1/safety/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-01-20 03:08:13.000000 safety-3.0.1/safety/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-01-20 03:08:13.000000 safety-3.0.1/safety/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.481777 safety-3.0.1/safety/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/bare.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.481777 safety-3.0.1/safety/formatters/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/schemas/v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/schemas/v3_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/schemas/zero_five.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-01-20 03:08:13.000000 safety-3.0.1/safety/formatters/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-01-20 03:08:13.000000 safety-3.0.1/safety/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    37313 2024-01-20 03:08:13.000000 safety-3.0.1/safety/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-01-20 03:08:13.000000 safety-3.0.1/safety/safety-policy-template.yml
--rw-r--r--   0 runner    (1001) docker     (127)    45148 2024-01-20 03:08:13.000000 safety-3.0.1/safety/safety.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.485777 safety-3.0.1/safety/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33310 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.485777 safety-3.0.1/safety/scan/ecosystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/ecosystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/ecosystems/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.485777 safety-3.0.1/safety/scan/ecosystems/python/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/ecosystems/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/ecosystems/python/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15450 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/ecosystems/python/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/ecosystems/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.485777 safety-3.0.1/safety/scan/finder/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/finder/file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/finder/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    21287 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-01-20 03:08:13.000000 safety-3.0.1/safety/scan/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.485777 safety-3.0.1/safety/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-01-20 03:08:13.000000 safety-3.0.1/safety/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-01-20 03:08:13.000000 safety-3.0.1/safety/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/safety.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-20 03:08:22.000000 safety-3.0.1/safety.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-20 03:08:22.497777 safety-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-20 03:08:13.000000 safety-3.0.1/tests/.policy_full.yml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-20 03:08:13.000000 safety-3.0.1/tests/.policy_with_ignores.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-20 03:08:13.000000 safety-3.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/action/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/Pipfile.lock-insecure
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/Pipfile.lock-secure
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/action/docker-insecure/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/docker-insecure/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/action/docker-secure/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/docker-secure/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/poetry.lock-insecure
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/poetry.lock-secure
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/pyproject.toml-insecure
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/pyproject.toml-secure
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/requirements.txt-insecure
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-20 03:08:13.000000 safety-3.0.1/tests/action/requirements.txt-secure
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-01-20 03:08:13.000000 safety-3.0.1/tests/alerts/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/auth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/auth/test_assets/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-20 03:08:13.000000 safety-3.0.1/tests/auth/test_assets/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-20 03:08:13.000000 safety-3.0.1/tests/auth/test_assets/config_empty.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 03:08:13.000000 safety-3.0.1/tests/auth/test_assets/config_no_id.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-20 03:08:13.000000 safety-3.0.1/tests/auth/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-01-20 03:08:13.000000 safety-3.0.1/tests/auth/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.489777 safety-3.0.1/tests/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/tests/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/tests/formatters/test_bare.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-01-20 03:08:13.000000 safety-3.0.1/tests/formatters/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/tests/formatters/test_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:13.000000 safety-3.0.1/tests/formatters/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_pinned.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_pinned_affected.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_pinned_and_unpinned.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-20 03:08:13.000000 safety-3.0.1/tests/reqs_unpinned.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-01-20 03:08:13.000000 safety-3.0.1/tests/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/tests/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-20 03:08:13.000000 safety-3.0.1/tests/scan/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-01-20 03:08:13.000000 safety-3.0.1/tests/scan/test_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-01-20 03:08:13.000000 safety-3.0.1/tests/scan/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    23850 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/tests/test_db/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/insecure.json
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/insecure_full.json
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/insecure_full_affected_versions.json
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/report.json
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/report_invalid_decode_error.json
--rw-r--r--   0 runner    (1001) docker     (127)   176374 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_db/report_with_recommended_fix.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.473777 safety-3.0.1/tests/test_fix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/tests/test_fix/basic/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_fix/basic/no_recommended_remediation_report.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_fix/basic/reqs_simple.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/tests/test_policy_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_policy_file/default_policy_file.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_policy_file/default_policy_file_using_invalid_keyword.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_policy_file/default_policy_file_using_invalid_typo_keyword.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 03:08:22.493777 safety-3.0.1/tests/test_policy_file/v3_0/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_policy_file/v3_0/default_policy_file.yml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_policy_file/v3_0/default_policy_file_using_invalid_keyword.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_safety.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-01-20 03:08:13.000000 safety-3.0.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.497420 safety-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    24250 2024-03-26 03:11:03.000000 safety-3.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-26 03:11:03.000000 safety-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-26 03:11:03.000000 safety-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-03-26 03:11:08.497420 safety-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-03-26 03:11:03.000000 safety-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-26 03:11:03.000000 safety-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.481420 safety-3.1.0/safety/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 03:11:03.000000 safety-3.1.0/safety/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 03:11:03.000000 safety-3.1.0/safety/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 03:11:03.000000 safety-3.1.0/safety/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.485420 safety-3.1.0/safety/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-26 03:11:03.000000 safety-3.1.0/safety/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-03-26 03:11:03.000000 safety-3.1.0/safety/alerts/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-03-26 03:11:03.000000 safety-3.1.0/safety/alerts/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.485420 safety-3.1.0/safety/alerts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-26 03:11:03.000000 safety-3.1.0/safety/alerts/templates/issue.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-26 03:11:03.000000 safety-3.1.0/safety/alerts/templates/pr.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-03-26 03:11:03.000000 safety-3.1.0/safety/alerts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.485420 safety-3.1.0/safety/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-03-26 03:11:03.000000 safety-3.1.0/safety/auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32425 2024-03-26 03:11:03.000000 safety-3.1.0/safety/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22376 2024-03-26 03:11:03.000000 safety-3.1.0/safety/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/safety/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-26 03:11:03.000000 safety-3.1.0/safety/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-03-26 03:11:03.000000 safety-3.1.0/safety/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-26 03:11:03.000000 safety-3.1.0/safety/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.485420 safety-3.1.0/safety/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/bare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.485420 safety-3.1.0/safety/formatters/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/schemas/v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/schemas/v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/schemas/zero_five.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-26 03:11:03.000000 safety-3.1.0/safety/formatters/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-03-26 03:11:03.000000 safety-3.1.0/safety/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37313 2024-03-26 03:11:03.000000 safety-3.1.0/safety/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-03-26 03:11:03.000000 safety-3.1.0/safety/safety-policy-template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    45148 2024-03-26 03:11:03.000000 safety-3.1.0/safety/safety.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.489420 safety-3.1.0/safety/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33310 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.489420 safety-3.1.0/safety/scan/ecosystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/ecosystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/ecosystems/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.489420 safety-3.1.0/safety/scan/ecosystems/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/ecosystems/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/ecosystems/python/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15450 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/ecosystems/python/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/ecosystems/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.489420 safety-3.1.0/safety/scan/finder/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/finder/file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/finder/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21287 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-26 03:11:03.000000 safety-3.1.0/safety/scan/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.489420 safety-3.1.0/safety/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-03-26 03:11:03.000000 safety-3.1.0/safety/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-03-26 03:11:03.000000 safety-3.1.0/safety/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.497420 safety-3.1.0/safety.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 03:11:08.000000 safety-3.1.0/safety.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-26 03:11:08.497420 safety-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-26 03:11:03.000000 safety-3.1.0/tests/.policy_full.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-26 03:11:03.000000 safety-3.1.0/tests/.policy_with_ignores.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 03:11:03.000000 safety-3.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/action/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/Pipfile.lock-insecure
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/Pipfile.lock-secure
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/action/docker-insecure/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/docker-insecure/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/action/docker-secure/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/docker-secure/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/poetry.lock-insecure
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/poetry.lock-secure
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/pyproject.toml-insecure
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/pyproject.toml-secure
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/requirements.txt-insecure
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 03:11:03.000000 safety-3.1.0/tests/action/requirements.txt-secure
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-03-26 03:11:03.000000 safety-3.1.0/tests/alerts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/auth/test_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 03:11:03.000000 safety-3.1.0/tests/auth/test_assets/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 03:11:03.000000 safety-3.1.0/tests/auth/test_assets/config_empty.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 03:11:03.000000 safety-3.1.0/tests/auth/test_assets/config_no_id.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-26 03:11:03.000000 safety-3.1.0/tests/auth/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-26 03:11:03.000000 safety-3.1.0/tests/auth/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/tests/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/tests/formatters/test_bare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-03-26 03:11:03.000000 safety-3.1.0/tests/formatters/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/tests/formatters/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:03.000000 safety-3.1.0/tests/formatters/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_pinned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_pinned_affected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_pinned_and_unpinned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 03:11:03.000000 safety-3.1.0/tests/reqs_unpinned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-03-26 03:11:03.000000 safety-3.1.0/tests/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.493420 safety-3.1.0/tests/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-26 03:11:03.000000 safety-3.1.0/tests/scan/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-26 03:11:03.000000 safety-3.1.0/tests/scan/test_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-26 03:11:03.000000 safety-3.1.0/tests/scan/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.497420 safety-3.1.0/tests/test_db/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/insecure.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/insecure_full.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/insecure_full_affected_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/report.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/report_invalid_decode_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)   176374 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_db/report_with_recommended_fix.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.477420 safety-3.1.0/tests/test_fix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.497420 safety-3.1.0/tests/test_fix/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_fix/basic/no_recommended_remediation_report.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_fix/basic/reqs_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.497420 safety-3.1.0/tests/test_policy_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_policy_file/default_policy_file.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_policy_file/default_policy_file_using_invalid_keyword.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_policy_file/default_policy_file_using_invalid_typo_keyword.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:11:08.497420 safety-3.1.0/tests/test_policy_file/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_policy_file/v3_0/default_policy_file.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_policy_file/v3_0/default_policy_file_using_invalid_keyword.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29816 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-03-26 03:11:03.000000 safety-3.1.0/tests/test_util.py
```

### Comparing `safety-3.0.1/CHANGELOG.md` & `safety-3.1.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is partly based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) and [PEP 440](https://peps.python.org/pep-0440/)
 
+## [3.1.0] - 2024-03-25
+- fix: ensure compatibility with Pydantic version 2.0 (#509)
+- feat: introduce --headless flag to enable an alternative login mechanism that bypasses the need for a local web server. (#508)
+
 ## [3.0.1] - 2024-01-19
 - fix: add back the license legacy cmd (#498)
 - perf: unpin authlib and remove jwt
 
 ## [3.0.0] - 2024-01-17
 
 ### Safety 3.0.0 major version release!
```

### Comparing `safety-3.0.1/LICENSE` & `safety-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/PKG-INFO` & `safety-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safety
-Version: 3.0.1
+Version: 3.1.0
 Summary: Checks installed dependencies for known vulnerabilities and licenses.
 Home-page: https://github.com/pyupio/safety
 Author: safetycli.com
 Author-email: support@safetycli.com
 License: MIT license
 Project-URL: Bug Tracker, https://github.com/pyupio/safety/issues
 Project-URL: Source, https://github.com/pyupio/safety/
@@ -35,16 +35,16 @@
 Requires-Dist: dparse>=0.6.4b0
 Requires-Dist: ruamel.yaml>=0.17.21
 Requires-Dist: jinja2>=3.1.0
 Requires-Dist: marshmallow>=3.15.0
 Requires-Dist: Authlib>=1.2.0
 Requires-Dist: rich
 Requires-Dist: typer
-Requires-Dist: pydantic<2.0,>=1.10.12
-Requires-Dist: safety_schemas>=0.0.1
+Requires-Dist: pydantic>=1.10.12
+Requires-Dist: safety_schemas>=0.0.2
 Requires-Dist: typing-extensions>=4.7.1
 Provides-Extra: github
 Requires-Dist: pygithub>=1.43.3; extra == "github"
 Provides-Extra: gitlab
 Requires-Dist: python-gitlab>=1.3.0; extra == "gitlab"
 Provides-Extra: spdx
 Requires-Dist: spdx-tools>=0.8.2; extra == "spdx"
@@ -173,14 +173,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is partly based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) and [PEP 440](https://peps.python.org/pep-0440/)
 
+## [3.1.0] - 2024-03-25
+- fix: ensure compatibility with Pydantic version 2.0 (#509)
+- feat: introduce --headless flag to enable an alternative login mechanism that bypasses the need for a local web server. (#508)
+
 ## [3.0.1] - 2024-01-19
 - fix: add back the license legacy cmd (#498)
 - perf: unpin authlib and remove jwt
 
 ## [3.0.0] - 2024-01-17
 
 ### Safety 3.0.0 major version release!
```

### Comparing `safety-3.0.1/README.md` & `safety-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/alerts/__init__.py` & `safety-3.1.0/safety/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/alerts/github.py` & `safety-3.1.0/safety/alerts/github.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/alerts/requirements.py` & `safety-3.1.0/safety/alerts/requirements.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/alerts/templates/issue.jinja2` & `safety-3.1.0/safety/alerts/templates/issue.jinja2`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/alerts/templates/pr.jinja2` & `safety-3.1.0/safety/alerts/templates/pr.jinja2`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/alerts/utils.py` & `safety-3.1.0/safety/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/auth/cli.py` & `safety-3.1.0/safety/auth/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,46 +92,55 @@
                         f"{organization}[green]")
 
     for msg in details:
         console.print(Padding(msg, (0, 0, 0, 1)), emoji=True)    
 
 
 @auth_app.command(name=CMD_LOGIN_NAME, help=CLI_AUTH_LOGIN_HELP)
-def login(ctx: typer.Context):
+def login(ctx: typer.Context, headless: bool = False):
     """
     Authenticate Safety CLI with your safetycli.com account using your default browser.
     """
     LOG.info('login started')
 
     fail_if_authenticated(ctx, with_msg=MSG_FAIL_LOGIN_AUTHED)
 
     console.print()
-    brief_msg: str = "Redirecting your browser to log in; once authenticated, " \
-          "return here to start using Safety"    
     
-    uri, initial_state = get_authorization_data(client=ctx.obj.auth.client,
-                                                code_verifier=ctx.obj.auth.code_verifier,
-                                                organization=ctx.obj.auth.org)
+    info = None
     
-    if ctx.obj.auth.org:
+    brief_msg: str = "Redirecting your browser to log in; once authenticated, " \
+            "return here to start using Safety"
+        
+    if ctx.obj.auth.org:        
         console.print(f"Logging into [bold]{ctx.obj.auth.org.name}[/bold] " \
                       "organization.")
-    
+        
+    if headless:
+        brief_msg = "Running in headless mode. Please copy and open the following URL in a browser"
+
+
+    uri, initial_state = get_authorization_data(client=ctx.obj.auth.client,
+                                                code_verifier=ctx.obj.auth.code_verifier,
+                                                organization=ctx.obj.auth.org, headless=headless)
     click.secho(brief_msg)
     click.echo()
 
-    info = process_browser_callback(uri, 
-                                    initial_state=initial_state, ctx=ctx)
+    info = process_browser_callback(uri, initial_state=initial_state, ctx=ctx, headless=headless)
+        
 
     if info:
         if info.get("email", None):
             organization = None
             if ctx.obj.auth.org and ctx.obj.auth.org.name:
                 organization = ctx.obj.auth.org.name
             ctx.obj.auth.refresh_from(info)
+            if headless:
+                console.print()
+
             render_successful_login(ctx.obj.auth, organization=organization)
 
             console.print()
             if ctx.obj.auth.org or ctx.obj.auth.email_verified:
                 console.print(
                     "[tip]Tip[/tip]: now try [bold]`safety scan`[/bold] in your project’s root " \
                     "folder to run a project scan or [bold]`safety -–help`[/bold] to learn more.")
@@ -145,15 +154,15 @@
         msg = ":stop_sign: [red]"
         if ctx.obj.auth.org:
             msg += f"Error logging into {ctx.obj.auth.org.name} organization " \
                 f"with auth ID: {ctx.obj.auth.org.id}."
         else:
             msg += "Error logging into Safety."
 
-        msg += " Please try again, or use [bold]`safety auth –help`[/bold] " \
+        msg += " Please try again, or use [bold]`safety auth -–help`[/bold] " \
             "for more information[/red]"
         
         console.print(msg, emoji=True)
 
 @auth_app.command(name=CMD_LOGOUT_NAME, help=CLI_AUTH_LOGOUT_HELP)
 def logout(ctx: typer.Context):
     """
```

### Comparing `safety-3.0.1/safety/auth/cli_utils.py` & `safety-3.1.0/safety/auth/cli_utils.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/auth/constants.py` & `safety-3.1.0/safety/auth/constants.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/auth/main.py` & `safety-3.1.0/safety/auth/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import configparser
 import json
 
 from typing import Any, Dict, Optional, Tuple, Union
+from urllib.parse import urlencode
 
 from authlib.oidc.core import CodeIDToken
 from authlib.jose import jwt
 from authlib.jose.errors import ExpiredTokenError
 
 from safety.auth.models import Organization
 from safety.auth.constants import AUTH_SERVER_URL, CLI_AUTH_LOGOUT, CLI_CALLBACK, AUTH_CONFIG_USER, CLI_AUTH
@@ -13,17 +14,17 @@
 from safety.errors import NotVerifiedEmailError
 from safety.scan.util import Stage
 from safety.util import get_proxy_dict
 
 
 def get_authorization_data(client, code_verifier: str,
                            organization: Optional[Organization] = None, 
-                           sign_up: bool = False, ensure_auth: bool = False) -> Tuple[str, str]:
+                           sign_up: bool = False, ensure_auth: bool = False, headless: bool = False) -> Tuple[str, str]:
     
-    kwargs = {'sign_up': sign_up, 'locale': 'en', 'ensure_auth': ensure_auth}
+    kwargs = {'sign_up': sign_up, 'locale': 'en', 'ensure_auth': ensure_auth, 'headless': headless}
     if organization:
         kwargs['organization'] = organization.id
 
     return client.create_authorization_url(CLI_AUTH,
                                            code_verifier=code_verifier,
                                            **kwargs)
```

### Comparing `safety-3.0.1/safety/auth/models.py` & `safety-3.1.0/safety/auth/models.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/auth/server.py` & `safety-3.1.0/safety/auth/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import http.server
+import json
 import logging
 import socket
 import sys
 import time
 from typing import Any, Optional
 import urllib.parse
 import threading
 import click
 from safety.auth.cli_utils import load_auth_session
 
 from safety.console import main_console as console
 
 from safety.auth.constants import AUTH_SERVER_URL, CLI_AUTH_SUCCESS, CLI_LOGOUT_SUCCESS, HOST
 from safety.auth.main import save_auth_config
+from authlib.integrations.base_client.errors import OAuthError
+from rich.prompt import Prompt
 
 LOG = logging.getLogger(__name__)
 
 
 def find_available_port():
     """Find an available port on localhost"""
     # Dynamic ports IANA
@@ -29,48 +32,57 @@
                 # If the connect succeeds, the port is already in use
             except socket.error as e:
                 # If the connect fails, the port is available
                 return port
 
     return None
 
+def auth_process(code: str, state: str, initial_state: str, code_verifier, client):
+    err = None
+
+    if initial_state is None or initial_state != state:
+        err = "The state parameter value provided does not match the expected " \
+                "value. The state parameter is used to protect against Cross-Site " \
+                "Request Forgery (CSRF) attacks. For security reasons, the " \
+                "authorization process cannot proceed with an invalid state " \
+                "parameter value. Please try again, ensuring that the state " \
+                "parameter value provided in the authorization request matches " \
+                "the value returned in the callback."
+
+    if err:
+        click.secho(f'Error: {err}', fg='red')
+        sys.exit(1)
+    
+    try:
+        tokens = client.fetch_token(url=f'{AUTH_SERVER_URL}/oauth/token',
+                                        code_verifier=code_verifier,
+                                        client_id=client.client_id,
+                                        grant_type='authorization_code', code=code)
+
+        save_auth_config(access_token=tokens['access_token'], 
+                            id_token=tokens['id_token'], 
+                            refresh_token=tokens['refresh_token'])
+        return client.fetch_user_info()
+
+    except Exception as e:
+        LOG.exception(e)
+        sys.exit(1)
 
 class CallbackHandler(http.server.BaseHTTPRequestHandler):
     def auth(self, code: str, state: str, err, error_description):
         initial_state = self.server.initial_state
         ctx = self.server.ctx
 
-        if initial_state is None or initial_state != state:
-            err = "The state parameter value provided does not match the expected" \
-                    "value. The state parameter is used to protect against Cross-Site " \
-                    "Request Forgery (CSRF) attacks. For security reasons, the " \
-                    "authorization process cannot proceed with an invalid state " \
-                    "parameter value. Please try again, ensuring that the state " \
-                    "parameter value provided in the authorization request matches " \
-                    "the value returned in the callback."
-
-        if err:
-            click.secho(f'Error: {err}', fg='red')
-            sys.exit(1)
+        result = auth_process(code=code, 
+                              state=state, 
+                              initial_state=initial_state, 
+                              code_verifier=ctx.obj.auth.code_verifier,
+                              client=ctx.obj.auth.client)
         
-        try:
-            tokens = ctx.obj.auth.client.fetch_token(url=f'{AUTH_SERVER_URL}/oauth/token',
-                                            code_verifier=ctx.obj.auth.code_verifier,
-                                            client_id=ctx.obj.auth.client.client_id,
-                                            grant_type='authorization_code', code=code)
-
-            save_auth_config(access_token=tokens['access_token'], 
-                             id_token=tokens['id_token'], 
-                             refresh_token=tokens['refresh_token'])
-            self.server.callback = ctx.obj.auth.client.fetch_user_info()
-
-        except Exception as e:
-            LOG.exception(e)
-            sys.exit(1)
-
+        self.server.callback = result
         self.do_redirect(location=CLI_AUTH_SUCCESS, params={})
 
     def logout(self):
         ctx = self.server.ctx
         uri = CLI_LOGOUT_SUCCESS
 
         if ctx.obj.auth.org:
@@ -128,35 +140,60 @@
     PORT = find_available_port()
 
     if not PORT:
         click.secho("No available ports.")
         sys.exit(1)
     
     try:
-        server = ThreadedHTTPServer((HOST, PORT), CallbackHandler)
-        server.initial_state = kwargs.get("initial_state", None)
-        server.timeout = kwargs.get("timeout", 600)
-        # timeout = kwargs.get("timeout", None)
-        # timeout = float(timeout) if timeout else None
-        server.ctx = kwargs.get("ctx", None)
-        server_thread = threading.Thread(target=server.handle_request)
-        server_thread.start()
-
-        target = f"{uri}&port={PORT}"
-        console.print(f"If the browser does not automatically open in 5 seconds, " \
-                      "copy and paste this url into your browser: " \
-                      f"[link={target}]{target}[/link]")
-        click.echo()
-
-        wait_msg = "waiting for browser authentication"
-        
-        with console.status(wait_msg, spinner="bouncingBar"):
-            time.sleep(2)
-            click.launch(target)
-            server_thread.join()
+        headless = kwargs.get("headless", False)
+        initial_state = kwargs.get("initial_state", None)
+        ctx = kwargs.get("ctx", None)
+
+        message = "Copy and paste this url into your browser:"
+
+
+        if not headless:
+            server = ThreadedHTTPServer((HOST, PORT), CallbackHandler)
+            server.initial_state = initial_state
+            server.timeout = kwargs.get("timeout", 600)
+            server.ctx = ctx
+            server_thread = threading.Thread(target=server.handle_request)
+            server_thread.start()
+            message = f"If the browser does not automatically open in 5 seconds, " \
+                        "copy and paste this url into your browser:"            
+
+        target = uri if headless else f"{uri}&port={PORT}"
+        console.print(f"{message} [link={target}]{target}[/link]")
+        console.print()
+
+        if headless:
+            
+            exchange_data = None
+            while not exchange_data:
+                auth_code_text = Prompt.ask("Paste the response here", default=None, console=console)
+                try:
+                    exchange_data = json.loads(auth_code_text)
+                    state = exchange_data["state"]
+                    code = exchange_data["code"]
+                except Exception as e:
+                    code = state = None             
+
+            return auth_process(code=code, 
+                                        state=state, 
+                                        initial_state=initial_state, 
+                                        code_verifier=ctx.obj.auth.code_verifier,
+                                        client=ctx.obj.auth.client)
+        else:
+
+            wait_msg = "waiting for browser authentication"
+            
+            with console.status(wait_msg, spinner="bouncingBar"):
+                time.sleep(2)
+                click.launch(target)
+                server_thread.join()
 
     except OSError as e:
         if e.errno == socket.errno.EADDRINUSE:
             reason = f"The port {HOST}:{PORT} is currently being used by another" \
                        "application or process. Please choose a different port or " \
                        "terminate the conflicting application/process to free up " \
                         "the port."
```

### Comparing `safety-3.0.1/safety/auth/utils.py` & `safety-3.1.0/safety/auth/utils.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/cli.py` & `safety-3.1.0/safety/cli.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/cli_util.py` & `safety-3.1.0/safety/cli_util.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/console.py` & `safety-3.1.0/safety/console.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/constants.py` & `safety-3.1.0/safety/constants.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/errors.py` & `safety-3.1.0/safety/errors.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatter.py` & `safety-3.1.0/safety/formatter.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/bare.py` & `safety-3.1.0/safety/formatters/bare.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/html.py` & `safety-3.1.0/safety/formatters/html.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/json.py` & `safety-3.1.0/safety/formatters/json.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/schemas/common.py` & `safety-3.1.0/safety/formatters/schemas/common.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/schemas/v3_0.py` & `safety-3.1.0/safety/formatters/schemas/v3_0.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/schemas/zero_five.py` & `safety-3.1.0/safety/formatters/schemas/zero_five.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/screen.py` & `safety-3.1.0/safety/formatters/screen.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/formatters/text.py` & `safety-3.1.0/safety/formatters/text.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/models.py` & `safety-3.1.0/safety/models.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/output_utils.py` & `safety-3.1.0/safety/output_utils.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/safety-policy-template.yml` & `safety-3.1.0/safety/safety-policy-template.yml`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/safety.py` & `safety-3.1.0/safety/safety.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/command.py` & `safety-3.1.0/safety/scan/command.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/constants.py` & `safety-3.1.0/safety/scan/constants.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/decorators.py` & `safety-3.1.0/safety/scan/decorators.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/ecosystems/base.py` & `safety-3.1.0/safety/scan/ecosystems/base.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/ecosystems/python/dependencies.py` & `safety-3.1.0/safety/scan/ecosystems/python/dependencies.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/ecosystems/python/main.py` & `safety-3.1.0/safety/scan/ecosystems/python/main.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/ecosystems/target.py` & `safety-3.1.0/safety/scan/ecosystems/target.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/finder/file_finder.py` & `safety-3.1.0/safety/scan/finder/file_finder.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/finder/handlers.py` & `safety-3.1.0/safety/scan/finder/handlers.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/main.py` & `safety-3.1.0/safety/scan/main.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/models.py` & `safety-3.1.0/safety/scan/models.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/render.py` & `safety-3.1.0/safety/scan/render.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/util.py` & `safety-3.1.0/safety/scan/util.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/scan/validators.py` & `safety-3.1.0/safety/scan/validators.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/templates/index.html` & `safety-3.1.0/safety/templates/index.html`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety/util.py` & `safety-3.1.0/safety/util.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/safety.egg-info/PKG-INFO` & `safety-3.1.0/safety.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safety
-Version: 3.0.1
+Version: 3.1.0
 Summary: Checks installed dependencies for known vulnerabilities and licenses.
 Home-page: https://github.com/pyupio/safety
 Author: safetycli.com
 Author-email: support@safetycli.com
 License: MIT license
 Project-URL: Bug Tracker, https://github.com/pyupio/safety/issues
 Project-URL: Source, https://github.com/pyupio/safety/
@@ -35,16 +35,16 @@
 Requires-Dist: dparse>=0.6.4b0
 Requires-Dist: ruamel.yaml>=0.17.21
 Requires-Dist: jinja2>=3.1.0
 Requires-Dist: marshmallow>=3.15.0
 Requires-Dist: Authlib>=1.2.0
 Requires-Dist: rich
 Requires-Dist: typer
-Requires-Dist: pydantic<2.0,>=1.10.12
-Requires-Dist: safety_schemas>=0.0.1
+Requires-Dist: pydantic>=1.10.12
+Requires-Dist: safety_schemas>=0.0.2
 Requires-Dist: typing-extensions>=4.7.1
 Provides-Extra: github
 Requires-Dist: pygithub>=1.43.3; extra == "github"
 Provides-Extra: gitlab
 Requires-Dist: python-gitlab>=1.3.0; extra == "gitlab"
 Provides-Extra: spdx
 Requires-Dist: spdx-tools>=0.8.2; extra == "spdx"
@@ -173,14 +173,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is partly based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) and [PEP 440](https://peps.python.org/pep-0440/)
 
+## [3.1.0] - 2024-03-25
+- fix: ensure compatibility with Pydantic version 2.0 (#509)
+- feat: introduce --headless flag to enable an alternative login mechanism that bypasses the need for a local web server. (#508)
+
 ## [3.0.1] - 2024-01-19
 - fix: add back the license legacy cmd (#498)
 - perf: unpin authlib and remove jwt
 
 ## [3.0.0] - 2024-01-17
 
 ### Safety 3.0.0 major version release!
```

### Comparing `safety-3.0.1/safety.egg-info/SOURCES.txt` & `safety-3.1.0/safety.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/setup.cfg` & `safety-3.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 	dparse>=0.6.4b0
 	ruamel.yaml>=0.17.21
 	jinja2>=3.1.0
 	marshmallow>=3.15.0
 	Authlib>=1.2.0
 	rich
 	typer
-	pydantic>=1.10.12,<2.0
-	safety_schemas>=0.0.1
+	pydantic>=1.10.12
+	safety_schemas>=0.0.2
 	typing-extensions>=4.7.1
 
 [options.entry_points]
 console_scripts = 
 	safety = safety.cli:cli
 
 [options.extras_require]
```

### Comparing `safety-3.0.1/tests/action/Pipfile.lock-insecure` & `safety-3.1.0/tests/action/Pipfile.lock-insecure`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/action/Pipfile.lock-secure` & `safety-3.1.0/tests/action/Pipfile.lock-secure`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/action/poetry.lock-insecure` & `safety-3.1.0/tests/action/poetry.lock-insecure`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/action/poetry.lock-secure` & `safety-3.1.0/tests/action/poetry.lock-secure`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/alerts/test_utils.py` & `safety-3.1.0/tests/alerts/test_utils.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/auth/test_cli.py` & `safety-3.1.0/tests/auth/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         process_browser_callback.return_value = {"email": "user@safetycli.com", "name": "Safety User"}
         result = self.runner.invoke(cli, ['auth'])
 
         fail_if_authenticated.assert_called_once()
         get_authorization_data.assert_called_once()
         process_browser_callback.assert_called_once_with(auth_data[0], 
                                                          initial_state=auth_data[1], 
-                                                         ctx=ANY)
+                                                         ctx=ANY, headless=False)
         
         expected = [
             "",
             "Redirecting your browser to log in; once authenticated, return here to start using Safety",
             "",
             "You're authenticated",
             " Account: Safety User, user@safetycli.com (email verification required)",
```

### Comparing `safety-3.0.1/tests/auth/test_main.py` & `safety-3.1.0/tests/auth/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,29 @@
         client.create_authorization_url = Mock()
         _ = get_authorization_data(client, code_verifier, organization)
 
         kwargs = {
              "sign_up": False,
              "locale": "en",
              "ensure_auth": False,
-             "organization": org_id
+             "organization": org_id,
+             "headless": False
         }
 
         client.create_authorization_url.assert_called_once_with(
              CLI_AUTH, code_verifier=code_verifier, **kwargs)
         
         client.create_authorization_url = Mock()
         _ = get_authorization_data(client, code_verifier, organization=None)
 
         kwargs = {
              "sign_up": False,
              "locale": "en",
-             "ensure_auth":False
+             "ensure_auth":False,
+             "headless": False             
         }
 
         client.create_authorization_url.assert_called_once_with(
              CLI_AUTH, code_verifier=code_verifier, **kwargs)        
 
     def get_logout_url(self, id_token):
         return f'{CLI_AUTH_LOGOUT}?id_token={id_token}'
```

### Comparing `safety-3.0.1/tests/formatters/test_json.py` & `safety-3.1.0/tests/formatters/test_json.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/resources.py` & `safety-3.1.0/tests/resources.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/scan/test_command.py` & `safety-3.1.0/tests/scan/test_command.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/scan/test_file_finder.py` & `safety-3.1.0/tests/scan/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/scan/test_render.py` & `safety-3.1.0/tests/scan/test_render.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_cli.py` & `safety-3.1.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,16 +200,15 @@
         self.assertEqual(msg + parsed, cleaned_stdout)
         self.assertEqual(result.exit_code, 0)
 
         path = os.path.join(dirname, "test_policy_file", "v3_0", "default_policy_file.yml")
         result = self.runner.invoke(cli.cli, ['validate', 'policy_file', '3.0', '--path', path])
         cleaned_stdout = click.unstyle(result.stdout)
         msg = 'The Safety policy (3.0) file (Used for scan and system-scan commands) was successfully parsed with the following values:\n'
-        parsed = json.dumps(
-            {
+        parsed = {
             "version": "3.0",
             "scan": {
                 "max_depth": 6,
                 "exclude": [],
                 "include_files": [],
                 "system": {
                 "targets": []
@@ -226,42 +225,51 @@
                     "vulnerabilities": None,
                     "cvss_severity": []
                 }
                 }
             },
             "fail_scan": {
                 "dependency_vulnerabilities": {
-                "enabled": True,
-                "fail_on_any_of": {
-                    "cvss_severity": [
-                    "critical",
-                    "high",
-                    "medium"
-                    ],
-                    "exploitability": [
-                    "critical",
-                    "high",
-                    "medium"
-                    ]
-                }
+                    "enabled": True,
+                    "fail_on_any_of": {
+                        "cvss_severity": [
+                            "critical",
+                            "high",
+                            "medium",                    
+                        ],
+                        "exploitability": [
+                            "critical",
+                            "high",
+                            "medium",
+                        ]
+                    }
                 }
             },
             "security_updates": {
                 "dependency_vulnerabilities": {
                 "auto_security_updates_limit": [
                     "patch"
                 ]
                 }
             }
-            },
-            indent=2
-        ) + '\n'
+            }
 
-        self.assertEqual(msg + parsed, cleaned_stdout)
-        self.assertEqual(result.exit_code, 0)        
+        msg_stdout, parsed_policy = cleaned_stdout.split('\n', 1)
+        msg_stdout += '\n'
+        parsed_policy = json.loads(parsed_policy.replace('\n', ''))
+
+        fail_scan = parsed_policy.get("fail_scan", None)
+        self.assertIsNotNone(fail_scan)
+        fail_of_any = fail_scan["dependency_vulnerabilities"]["fail_on_any_of"]
+        fail_of_any["cvss_severity"] = sorted(fail_of_any["cvss_severity"])
+        fail_of_any["exploitability"] = sorted(fail_of_any["exploitability"])
+
+        self.assertEqual(msg, msg_stdout)
+        self.assertEqual(parsed, parsed_policy)
+        self.assertEqual(result.exit_code, 0)
 
 
     def test_validate_with_policy_file_using_invalid_keyword(self):
         dirname = os.path.dirname(__file__)
         filename = 'default_policy_file_using_invalid_keyword.yml'
         path = os.path.join(dirname, "test_policy_file", filename)
         result = self.runner.invoke(cli.cli, ['validate', 'policy_file', '2.0', '--path', path])
@@ -273,19 +281,17 @@
 
         self.assertEqual(msg, cleaned_stdout)
         self.assertEqual(result.exit_code, 1)
 
         path = os.path.join(dirname, "test_policy_file", "v3_0", filename)
         result = self.runner.invoke(cli.cli, ['validate', 'policy_file', '3.0', '--path', path])
         cleaned_stdout = click.unstyle(result.stderr)
-        msg_hint = 'report -> dependency-vulnerabilities -> transitive\n' \
-                   '  extra fields not permitted (type=value_error.extra)\n'
-        msg = f'Unable to load the Safety Policy file ("{path}"), this command only supports version 3.0, details: 1 validation error for Config\n{msg_hint}'
+        msg = f'Unable to load the Safety Policy file ("{path}"), this command only supports version 3.0, details: 1 validation error for Config'
 
-        self.assertEqual(msg, cleaned_stdout)
+        self.assertIn(msg, cleaned_stdout)
         self.assertEqual(result.exit_code, 1)
 
 
     def test_validate_with_policy_file_using_invalid_typo_keyword(self):
         dirname = os.path.dirname(__file__)
         filename = 'default_policy_file_using_invalid_typo_keyword.yml'
         path = os.path.join(dirname, "test_policy_file", filename)
```

### Comparing `safety-3.0.1/tests/test_db/insecure_full.json` & `safety-3.1.0/tests/test_db/insecure_full.json`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_db/insecure_full_affected_versions.json` & `safety-3.1.0/tests/test_db/insecure_full_affected_versions.json`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_db/report.json` & `safety-3.1.0/tests/test_db/report.json`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_db/report_invalid_decode_error.json` & `safety-3.1.0/tests/test_db/report_invalid_decode_error.json`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_db/report_with_recommended_fix.json` & `safety-3.1.0/tests/test_db/report_with_recommended_fix.json`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_fix/basic/no_recommended_remediation_report.json` & `safety-3.1.0/tests/test_fix/basic/no_recommended_remediation_report.json`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_models.py` & `safety-3.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_output_utils.py` & `safety-3.1.0/tests/test_output_utils.py`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_policy_file/default_policy_file.yml` & `safety-3.1.0/tests/test_policy_file/default_policy_file.yml`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_policy_file/default_policy_file_using_invalid_keyword.yml` & `safety-3.1.0/tests/test_policy_file/default_policy_file_using_invalid_keyword.yml`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_policy_file/default_policy_file_using_invalid_typo_keyword.yml` & `safety-3.1.0/tests/test_policy_file/default_policy_file_using_invalid_typo_keyword.yml`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_policy_file/v3_0/default_policy_file.yml` & `safety-3.1.0/tests/test_policy_file/v3_0/default_policy_file.yml`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_policy_file/v3_0/default_policy_file_using_invalid_keyword.yml` & `safety-3.1.0/tests/test_policy_file/v3_0/default_policy_file_using_invalid_keyword.yml`

 * *Files identical despite different names*

### Comparing `safety-3.0.1/tests/test_safety.py` & `safety-3.1.0/tests/test_safety.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,14 +462,15 @@
             session.get.return_value = mock          
 
             self.assertEqual(get_announcements(session), [])
 
     @patch("safety.util.get_used_options")
     @patch.object(click, 'get_current_context', Mock(command=Mock(name=Mock(return_value='check'))))
     def test_get_announcements_http_ok(self, get_used_options):
+        get_used_options.return_value = {}
 
         announcements = {
             "announcements": [{
                 "type": "notice",
                 "message": "You are using an outdated version of  Please upgrade to Safety version 1.2.3"
                 },
                 {
@@ -490,14 +491,16 @@
         session.post.return_value = mock
 
         self.assertEqual(get_announcements(session), expected)
 
     @patch("safety.util.get_used_options")
     @patch.object(click, 'get_current_context', Mock(command=Mock(name=Mock(return_value='check'))))
     def test_get_announcements_wrong_json_response_handling(self, get_used_options):
+        get_used_options.return_value = {}
+
         # wrong JSON structure
         announcements = {
                 "type": "notice",
                 "message": "You are using an outdated version of  Please upgrade to Safety version 1.2.3"
         }
 
         mock = Mock()
```

### Comparing `safety-3.0.1/tests/test_util.py` & `safety-3.1.0/tests/test_util.py`

 * *Files identical despite different names*

