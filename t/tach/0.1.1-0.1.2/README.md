# Comparing `tmp/tach-0.1.1.tar.gz` & `tmp/tach-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.1.1.tar", last modified: Tue Apr 30 07:28:32 2024, max compression
+gzip compressed data, was "tach-0.1.2.tar", last modified: Wed May  1 17:02:41 2024, max compression
```

## Comparing `tach-0.1.1.tar` & `tach-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.496687 tach-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 07:28:28.000000 tach-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-30 07:28:32.496687 tach-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-30 07:28:28.000000 tach-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 07:28:28.000000 tach-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:28:32.496687 tach-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.488687 tach-0.1.1/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:28.000000 tach-0.1.1/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-30 07:28:28.000000 tach-0.1.1/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-30 07:28:28.000000 tach-0.1.1/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-30 07:28:28.000000 tach-0.1.1/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.488687 tach-0.1.1/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 07:28:28.000000 tach-0.1.1/tach/colors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 07:28:28.000000 tach-0.1.1/tach/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-30 07:28:28.000000 tach-0.1.1/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-30 07:28:28.000000 tach-0.1.1/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-30 07:28:28.000000 tach-0.1.1/tach/core/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 07:28:28.000000 tach-0.1.1/tach/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 07:28:28.000000 tach-0.1.1/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 07:28:28.000000 tach-0.1.1/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 07:28:28.000000 tach-0.1.1/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-30 07:28:28.000000 tach-0.1.1/tach/filesystem/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-30 07:28:28.000000 tach-0.1.1/tach/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-30 07:28:28.000000 tach-0.1.1/tach/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-30 07:28:28.000000 tach-0.1.1/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 07:28:28.000000 tach-0.1.1/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 07:28:28.000000 tach-0.1.1/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-30 07:28:28.000000 tach-0.1.1/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 07:28:28.000000 tach-0.1.1/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 07:28:28.000000 tach-0.1.1/tach/parsing/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-30 07:28:32.000000 tach-0.1.1/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 07:28:32.000000 tach-0.1.1/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:28:32.000000 tach-0.1.1/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 07:28:32.000000 tach-0.1.1/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 07:28:32.000000 tach-0.1.1/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 07:28:32.000000 tach-0.1.1/tach.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:28:32.492687 tach-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_module_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:28:28.000000 tach-0.1.1/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.178931 tach-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.182931 tach-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 17:02:36.000000 tach-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-01 17:02:36.000000 tach-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 17:02:36.000000 tach-0.1.2/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-01 17:02:36.000000 tach-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 17:02:36.000000 tach-0.1.2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 17:02:36.000000 tach-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-01 17:02:41.198931 tach-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-01 17:02:36.000000 tach-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 17:02:36.000000 tach-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-01 17:02:36.000000 tach-0.1.2/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 17:02:36.000000 tach-0.1.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-01 17:02:36.000000 tach-0.1.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 17:02:36.000000 tach-0.1.2/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 17:02:36.000000 tach-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-01 17:02:36.000000 tach-0.1.2/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-01 17:02:36.000000 tach-0.1.2/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-01 17:02:36.000000 tach-0.1.2/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-01 17:02:36.000000 tach-0.1.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-01 17:02:36.000000 tach-0.1.2/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-01 17:02:36.000000 tach-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-01 17:02:36.000000 tach-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:02:41.198931 tach-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-01 17:02:36.000000 tach-0.1.2/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-05-01 17:02:36.000000 tach-0.1.2/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-01 17:02:36.000000 tach-0.1.2/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-01 17:02:36.000000 tach-0.1.2/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 17:02:36.000000 tach-0.1.2/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 17:02:36.000000 tach-0.1.2/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 17:02:36.000000 tach-0.1.2/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 17:02:36.000000 tach-0.1.2/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 17:02:36.000000 tach-0.1.2/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-01 17:02:36.000000 tach-0.1.2/tach/hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-01 17:02:36.000000 tach-0.1.2/tach/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 17:02:36.000000 tach-0.1.2/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 17:02:36.000000 tach-0.1.2/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-01 17:02:36.000000 tach-0.1.2/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_module_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_show.py
```

### Comparing `tach-0.1.1/LICENSE` & `tach-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/PKG-INFO` & `tach-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.1.1/README.md` & `tach-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/pyproject.toml` & `tach-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -39,12 +39,12 @@
 
 [tool.pyright]
 include = ["tach"]
 exclude = ["**/__pycache__", ".venv"]
 strict = ["tach"]
 
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "setuptools-scm>=8.0"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 tach = "tach.cli:main"
```

### Comparing `tach-0.1.1/tach/add.py` & `tach-0.1.2/tach/add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/check.py` & `tach-0.1.2/tach/check.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/cli.py` & `tach-0.1.2/tach/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import argparse
 import sys
+from enum import Enum
 from typing import Optional
 
 from tach.add import add_packages
 from tach.check import check, ErrorInfo
 from tach import filesystem as fs
 from tach.constants import CONFIG_FILE_NAME
+from tach.filesystem import install_pre_commit
 from tach.init import init_project
 from tach.loading import stop_spinner, start_spinner
 from tach.parsing import parse_project_config
 from tach.colors import BCOLORS
 
 
 def print_errors(error_list: list[ErrorInfo]) -> None:
@@ -83,14 +85,33 @@
         "--tags",
         required=False,
         type=str,
         metavar="tag,...",
         help="The tag for the module to be initialized with."
         "Use a comma-separated list for multiple.",
     )
+    install_parser = subparsers.add_parser(
+        "install",
+        prog="tach install",
+        help="Install tach into your workflow (e.g. as a pre-commit hook)",
+        description="Install tach into your workflow (e.g. as a pre-commit hook)",
+    )
+    install_parser.add_argument(
+        "target",
+        choices=InstallTarget.choices(),
+        help="What kind of installation to perform (e.g. pre-commit)",
+    )
+    install_parser.add_argument(
+        "-p",
+        "--path",
+        required=False,
+        type=str,
+        default=".",
+        help="The path where this installation should occur (default '.')",
+    )
     return parser
 
 
 def parse_arguments(
     args: list[str],
 ) -> tuple[argparse.Namespace, argparse.ArgumentParser]:
     parser = build_parser()
@@ -159,27 +180,64 @@
     if len(paths) > 1:
         print(f"✅ {BCOLORS.OKGREEN}Packages added.{BCOLORS.ENDC}")
     else:
         print(f"✅ {BCOLORS.OKGREEN}Package added.{BCOLORS.ENDC}")
     sys.exit(0)
 
 
+class InstallTarget(Enum):
+    PRE_COMMIT = "pre-commit"
+
+    @classmethod
+    def choices(cls) -> list[str]:
+        return [item.value for item in cls]
+
+
+def tach_install(path: str, target: InstallTarget) -> None:
+    try:
+        if target == InstallTarget.PRE_COMMIT:
+            installed, warning = install_pre_commit(path=path)
+        else:
+            raise NotImplementedError(f"Target {target} is not supported by 'install'.")
+    except Exception as e:
+        print(str(e))
+        sys.exit(1)
+
+    if installed:
+        print(
+            f"✅ {BCOLORS.OKGREEN}Pre-commit hook installed to '.git/hooks/pre-commit'.{BCOLORS.ENDC}"
+        )
+        sys.exit(0)
+    else:
+        print(
+            f"{BCOLORS.WARNING}Pre-commit hook could not be installed: {warning} {BCOLORS.ENDC}"
+        )
+        sys.exit(1)
+
+
 def main() -> None:
     args, parser = parse_arguments(sys.argv[1:])
     if args.command == "add":
         paths = set(args.path.split(","))
         tags = set(args.tags.split(",")) if args.tags else None
         tach_add(paths=paths, tags=tags)
         return
-    exclude_paths = args.exclude.split(",") if args.exclude else None
+    exclude_paths = args.exclude.split(",") if getattr(args, "exclude", None) else None
     if args.command == "init":
         tach_init(depth=args.depth, exclude_paths=exclude_paths)
     elif args.command == "check":
         start_spinner("Scanning...")
         tach_check(exclude_paths=exclude_paths)
+    elif args.command == "install":
+        try:
+            install_target = InstallTarget(args.target)
+        except ValueError:
+            print(f"{args.target} is not a valid installation target.")
+            sys.exit(1)
+        tach_install(path=args.path, target=install_target)
     else:
         print("Unrecognized command")
         parser.print_help()
         exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `tach-0.1.1/tach/core/config.py` & `tach-0.1.2/tach/core/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/core/package.py` & `tach-0.1.2/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/filesystem/__init__.py` & `tach-0.1.2/tach/filesystem/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     validate_project_config_path,
     print_no_config_yml,
     find_project_config_root,
 )
 from tach.filesystem.package import (
     validate_package_config,
 )
+from tach.filesystem.install import install_pre_commit
 
 __all__ = [
     "get_cwd",
     "chdir",
     "canonical",
     "read_file",
     "write_file",
@@ -36,8 +37,9 @@
     "module_to_file_path",
     "is_project_import",
     "get_project_config_path",
     "validate_project_config_path",
     "print_no_config_yml",
     "validate_package_config",
     "find_project_config_root",
+    "install_pre_commit",
 ]
```

### Comparing `tach-0.1.1/tach/filesystem/project.py` & `tach-0.1.2/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/filesystem/service.py` & `tach-0.1.2/tach/filesystem/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import ast
 import re
+import stat
 import sys
 import threading
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
 from typing import Optional, Generator
@@ -103,14 +104,21 @@
     if cached_file:
         cached_file.content = content
         cached_file.ast = None
     else:
         _set_cached_file(path, FileInfo(path=path, content=content))
 
 
+def mark_executable(path: str):
+    file_path = Path(path)
+    file_path.chmod(
+        file_path.stat().st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH
+    )
+
+
 def parse_ast(path: str) -> ast.AST:
     cached_file = _cached_file(path)
     if cached_file and cached_file.ast:
         return cached_file.ast
 
     if cached_file and cached_file.content:
         content = cached_file.content
```

### Comparing `tach-0.1.1/tach/init.py` & `tach-0.1.2/tach/init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/loading.py` & `tach-0.1.2/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/parsing/config.py` & `tach-0.1.2/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/parsing/imports.py` & `tach-0.1.2/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/parsing/interface.py` & `tach-0.1.2/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach/parsing/packages.py` & `tach-0.1.2/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tach.egg-info/PKG-INFO` & `tach-0.1.2/tach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.1.1/tests/test_add.py` & `tach-0.1.2/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tests/test_check.py` & `tach-0.1.2/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tests/test_cli.py` & `tach-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tests/test_init.py` & `tach-0.1.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tests/test_module_trie.py` & `tach-0.1.2/tests/test_module_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.1/tests/test_parsing.py` & `tach-0.1.2/tests/test_parsing.py`

 * *Files identical despite different names*

