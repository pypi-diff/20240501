# Comparing `tmp/runit_cli-0.4.0.tar.gz` & `tmp/runit_cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runit_cli-0.4.0.tar", last modified: Sat Apr 13 14:28:36 2024, max compression
+gzip compressed data, was "runit_cli-0.4.1.tar", last modified: Wed May  1 12:06:29 2024, max compression
```

## Comparing `runit_cli-0.4.0.tar` & `runit_cli-0.4.1.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.923806 runit_cli-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-13 14:28:32.000000 runit_cli-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 14:28:36.923806 runit_cli-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-13 14:28:32.000000 runit_cli-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.911805 runit_cli-0.4.0/runit/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/languages/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/php.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/modules/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/plugins/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/php.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/python.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/r.py
--rw-r--r--   0 runner    (1001) docker     (127)    16554 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/runit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/.runitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/templates/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/javascript/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/javascript/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/templates/multi/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/index.php
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/request.php
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/test.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/templates/php/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/php/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/php/index.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/python/application.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/request.php
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/runit.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.911805 runit_cli-0.4.0/runit/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/tools/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/javascript/loader.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/javascript/runner.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/tools/php/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/php/loader.php
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/php/manager.php
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/php/runner.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/tools/python/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/python/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/python/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.923806 runit_cli-0.4.0/runit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:28:36.923806 runit_cli-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-13 14:28:32.000000 runit_cli-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_clone_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_create_new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_create_project_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_generate_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_publish_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_run_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.227735 runit_cli-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 12:06:25.000000 runit_cli-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-01 12:06:29.227735 runit_cli-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-01 12:06:25.000000 runit_cli-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/php.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/modules/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/plugins/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/php.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/r.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/runit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/.runitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/javascript/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/javascript/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/multi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/index.php
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/request.php
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/php/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/php/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/php/index.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/python/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/request.php
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/runit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.215735 runit_cli-0.4.1/runit/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/tools/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/javascript/loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/javascript/runner.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/tools/php/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/php/loader.php
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/php/manager.php
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/php/runner.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/tools/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/python/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/python/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.227735 runit_cli-0.4.1/runit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:06:29.227735 runit_cli-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-01 12:06:25.000000 runit_cli-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.227735 runit_cli-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_clone_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_create_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_create_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_generate_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_publish_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_run_project.py
```

### Comparing `runit_cli-0.4.0/PKG-INFO` & `runit_cli-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-cli
-Version: 0.4.0
+Version: 0.4.1
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit_cli-0.4.0/README.md` & `runit_cli-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/Request.py` & `runit_cli-0.4.1/runit/Request.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/cli.py` & `runit_cli-0.4.1/runit/cli.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/constants.py` & `runit_cli-0.4.1/runit/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.4.0"
+VERSION = "0.4.1"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = Path(os.curdir).resolve()
```

### Comparing `runit_cli-0.4.0/runit/core.py` & `runit_cli-0.4.1/runit/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import asyncio
 import os
+from typing import Optional
 from fastapi import FastAPI, Request
 from fastapi.responses import HTMLResponse
 import json
 import uvicorn
 import sys
 from pathlib import Path
 from dotenv import find_dotenv, dotenv_values, set_key
@@ -42,66 +44,71 @@
         '''
         settings = dotenv_values(find_dotenv())
 
         RunitServerSetup.create_default_env_file()
         RunitServerSetup.update_api_settings(args, settings)
 
         for key, value in settings.items():
-            set_key(find_dotenv(), key, value)
+            set_key(find_dotenv(), key, str(value))
 
 # Example usage:
 # setup = RunitServerSetup()
 # setup.setup_runit(args)
 
 class WebServer:
     def __init__(self, project):
         self.project = project
 
     def create_app(self):
         app = FastAPI()
-        app.secret_key = os.getenv('SECRET_KEY')
         return app
 
     def add_routes(self, app):
         @app.api_route('/', methods=["GET", "POST"])
         @app.api_route('/{func}', methods=["GET", "POST"])
         @app.api_route('/{func}/', methods=["GET", "POST"])
         @app.api_route('/{func}/{output_format}', methods=["GET", "POST"])
         @app.api_route('/{func}/{output_format}/', methods=["GET", "POST"])
-        async def serve(func: str = 'index', output_format: str = 'json', request: Request = None):
+        
+        async def serve(func: str = 'index', output_format: str = 'json', request: Request = None): # type: ignore
             response = self.handle_request(func, output_format, request)
             return self.process_response(output_format, response)
 
     def handle_request(self, func, output_format, request):
-        response = {'status': True, 'data': {}}
+        response = ''
         result = ''
-
         try:
             parameters = self.get_request_parameters(request)
             result = self.project.serve(func, parameters)
             self.check_404(result)
-            response['data'] = self.parse_result(result)
+            response = self.parse_result(result)
         except json.decoder.JSONDecodeError:
-            response['data'] = result
+            response = result
         except Exception:
-            response['status'] = False
-            response['message'] = self.project.notfound(output_format)
+            response = self.project.notfound(output_format)
+        finally:
+            return response
+
+    def get_request_parameters(self, request: Request):
+        data = {}
 
-        return response
+        if request.method.lower() == 'post':
+            data = request._form._dict if request._form else {}
+
+            if request.headers['content-type'] == "application/json":
+                data = asyncio.run(request.json())
+        else:
+            data = request.query_params._dict
 
-    async def get_request_parameters(self, request):
-        parameters = request.query_params._dict
-        if 'content-type' in request.headers.keys() and request.headers['content-type'] == "application/json":
-            data = await request.json()
-            parameters = {**parameters, **data}
-        parameters.pop('output_format', None)
-        return list(parameters.values()) if request else request
+        data.pop('output_format', None)
+        
+        return list(data.values())
 
     def check_404(self, result):
-        if result.startswith('404'):
+        if '404' in result:
             raise RuntimeError('Not Found')
 
     def parse_result(self, result):
         return json.loads(result.replace("'", '"'))
 
     def process_response(self, output_format, response):
         if output_format == 'html':
```

### Comparing `runit_cli-0.4.0/runit/generate.py` & `runit_cli-0.4.1/runit/generate.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/languages/__init__.py` & `runit_cli-0.4.1/runit/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/languages/javascript.py` & `runit_cli-0.4.1/runit/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/languages/multi.py` & `runit_cli-0.4.1/runit/languages/multi.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/languages/php.py` & `runit_cli-0.4.1/runit/languages/php.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/languages/python.py` & `runit_cli-0.4.1/runit/languages/python.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/languages/runtime.py` & `runit_cli-0.4.1/runit/languages/runtime.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/modules/account.py` & `runit_cli-0.4.1/runit/modules/account.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/plugins/base.py` & `runit_cli-0.4.1/runit/plugins/base.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/plugins/languages/javascript.py` & `runit_cli-0.4.1/runit/plugins/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/plugins/languages/language.py` & `runit_cli-0.4.1/runit/plugins/languages/language.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/plugins/languages/php.py` & `runit_cli-0.4.1/runit/plugins/languages/php.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/plugins/languages/python.py` & `runit_cli-0.4.1/runit/plugins/languages/python.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/runit.py` & `runit_cli-0.4.1/runit/runit.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         self.config['private'] = self.private
         self.config['start_file'] = self.start_file
         self.config['author'] = self.author
         json.dump(self.config, config_file, indent=4)
         config_file.close()
     
     def get_exclude_list(self):
-        exclude_list = [self.name + '.zip', 'account.db', '.git', '.venv', 'venv', 'Dockerfile']
+        exclude_list = [self.name + '.zip', '.env', 'account.db', '.git', '.venv', 'venv', 'Dockerfile']
         
         if os.path.exists(DOT_RUNIT_IGNORE):
             with open(DOT_RUNIT_IGNORE, 'rt') as file:
                 exclude_list.extend(os.path.normpath(line.strip()) for line in file if line.strip())
         
         exclude_list = [item for item in exclude_list if item != '.']
         return exclude_list
@@ -409,18 +409,15 @@
         package_details['author'] = self.author
         
         with open('package.json', 'wt') as package_file:
             json.dump(package_details, package_file, indent=4)
         
         try:
             logger.info('[-] Installing node modules...')
-            if RunIt.RUNTIME_ENV == 'client':
-                os.system('npm install')
-            else:
-                os.system('bun install')
+            os.system(f'{self.runtime if self.runtime == 'bun' else 'npm'} install')
         except Exception as e:
             logger.exception(str(e))
             logger.error("[!] Couldn't install modules")
             logger.debug(INSTALL_MODULE_LATER_MESSAGE)
         
 
     def update_and_install_composer_json(self):
```

### Comparing `runit_cli-0.4.0/runit/templates/404.html` & `runit_cli-0.4.1/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/templates/multi/application.py` & `runit_cli-0.4.1/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/templates/python/application.py` & `runit_cli-0.4.1/runit/templates/python/application.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/tools/php/loader.php` & `runit_cli-0.4.1/runit/tools/php/loader.php`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/tools/php/runner.php` & `runit_cli-0.4.1/runit/tools/php/runner.php`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit/tools/python/runner.py` & `runit_cli-0.4.1/runit/tools/python/runner.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/runit_cli.egg-info/PKG-INFO` & `runit_cli-0.4.1/runit_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-cli
-Version: 0.4.0
+Version: 0.4.1
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit_cli-0.4.0/runit_cli.egg-info/SOURCES.txt` & `runit_cli-0.4.1/runit_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 runit/templates/multi/application.py
 runit/templates/multi/composer.json
 runit/templates/multi/index.php
 runit/templates/multi/main.js
 runit/templates/multi/package.json
 runit/templates/multi/request.php
 runit/templates/multi/requirements.txt
-runit/templates/multi/test.php
 runit/templates/php/composer.json
 runit/templates/php/index.php
 runit/templates/python/application.py
 runit/templates/python/requirements.txt
 runit/tools/javascript/loader.js
 runit/tools/javascript/runner.js
 runit/tools/php/loader.php
```

### Comparing `runit_cli-0.4.0/setup.py` & `runit_cli-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='runit-cli',
     version=VERSION,
```

### Comparing `runit_cli-0.4.0/tests/test_clone_project.py` & `runit_cli-0.4.1/tests/test_clone_project.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/tests/test_create_new_project.py` & `runit_cli-0.4.1/tests/test_create_new_project.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/tests/test_create_project_config.py` & `runit_cli-0.4.1/tests/test_create_project_config.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/tests/test_generate_function.py` & `runit_cli-0.4.1/tests/test_generate_function.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/tests/test_publish_project.py` & `runit_cli-0.4.1/tests/test_publish_project.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.0/tests/test_run_project.py` & `runit_cli-0.4.1/tests/test_run_project.py`

 * *Files identical despite different names*

