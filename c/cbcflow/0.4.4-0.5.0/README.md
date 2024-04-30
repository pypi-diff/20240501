# Comparing `tmp/cbcflow-0.4.4.tar.gz` & `tmp/cbcflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.4.4.tar", last modified: Mon Mar 18 17:53:55 2024, max compression
+gzip compressed data, was "cbcflow-0.5.0.tar", last modified: Tue Apr 30 22:05:22 2024, max compression
```

## Comparing `cbcflow-0.4.4.tar` & `cbcflow-0.5.0.tar`

### file list

```diff
@@ -1,139 +1,138 @@
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.155452 cbcflow-0.4.4/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.4.4/.gitattributes
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      229 2024-03-11 14:49:50.000000 cbcflow-0.4.4/.gitignore
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1602 2024-03-15 16:52:35.000000 cbcflow-0.4.4/.gitlab-ci.yml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-12-08 19:49:13.000000 cbcflow-0.4.4/.pre-commit-config.yaml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.4.4/CHANGELOG.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.4.4/LICENSE.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.4.4/MANIFEST.in
--rw-r--r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3652 2024-03-18 17:53:55.155452 cbcflow-0.4.4/PKG-INFO
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2676 2023-08-15 18:08:33.000000 cbcflow-0.4.4/README.md
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:54.962450 cbcflow-0.4.4/docs/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.4.4/docs/Makefile
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/requirements.txt
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.011451 cbcflow-0.4.4/docs/source/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.014451 cbcflow-0.4.4/docs/source/_templates/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.4.4/docs/source/_templates/custom-class-template.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.4.4/docs/source/_templates/custom-module-template.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/actionitems.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/adding-to-the-schema.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/asimov.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.4.4/docs/source/cbcflow-git-merging.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/conf.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/configuration.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/development-setup.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.021451 cbcflow-0.4.4/docs/source/example_mini_schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/example_mini_schema/example.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/example_mini_schema/schema_doc.css
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/example_mini_schema/schema_doc.html
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/example_mini_schema/schema_doc.min.js
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/gwosc.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/index.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.036451 cbcflow-0.4.4/docs/source/libraries_images/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.038451 cbcflow-0.4.4/docs/source/libraries_images/.ipynb_checkpoints/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_1.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_2.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_3.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_4.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_5.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_6.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_7.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/libraries_images/part_8.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/library-index-labelling.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/library-indices.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.4.4/docs/source/library-setup-from-scratch.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/local-library-copy-setup.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/monitor-usage.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/reading-the-schema.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.4.4/docs/source/schema-visualization.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/updating-metadata-from-the-command-line.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2024-03-11 16:28:04.000000 cbcflow-0.4.4/docs/source/updating-metadata-with-the-python-api.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.4.4/docs/source/what-is-metadata.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.061452 cbcflow-0.4.4/examples/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.4.4/examples/initial_example.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      899 2024-03-11 14:49:50.000000 cbcflow-0.4.4/pyproject.toml
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.068452 cbcflow-0.4.4/schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.4.4/schema/cbc-meta-data-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.4.4/schema/cbc-meta-data-v2.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)   134922 2024-03-15 16:44:06.000000 cbcflow-0.4.4/schema/cbc-meta-data-v3.schema
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.4.4/schema/index-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1748 2024-03-18 17:53:55.157452 cbcflow-0.4.4/setup.cfg
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      617 2024-03-11 16:28:27.000000 cbcflow-0.4.4/setup.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:54.943450 cbcflow-0.4.4/src/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.086452 cbcflow-0.4.4/src/cbcflow/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1212 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/__init__.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      411 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow/_version.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      386 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/asimov.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      317 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/cbcflow.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.098452 cbcflow-0.4.4/src/cbcflow/client/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       47 2023-10-04 20:55:03.000000 cbcflow-0.4.4/src/cbcflow/client/__init__.py
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9440 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/client/cbcflow.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1337 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/client/migrate_v2_to_v3.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6450 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/client/monitor.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      324 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/configuration.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.109452 cbcflow-0.4.4/src/cbcflow/core/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       89 2023-10-04 20:55:03.000000 cbcflow-0.4.4/src/cbcflow/core/__init__.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1437 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/core/configuration.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    43542 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/core/database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15693 2023-11-30 19:49:31.000000 cbcflow-0.4.4/src/cbcflow/core/metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9631 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/core/parser.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-09-19 22:38:51.000000 cbcflow-0.4.4/src/cbcflow/core/process.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2798 2024-03-15 16:44:50.000000 cbcflow-0.4.4/src/cbcflow/core/schema.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7763 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/core/utils.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1662 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/core/wrapped.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      314 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      316 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/gracedb.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.114452 cbcflow-0.4.4/src/cbcflow/inputs/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      116 2023-10-04 20:55:03.000000 cbcflow-0.4.4/src/cbcflow/inputs/__init__.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    13145 2023-10-13 16:04:41.000000 cbcflow-0.4.4/src/cbcflow/inputs/asimov.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    30788 2024-03-15 16:44:06.000000 cbcflow-0.4.4/src/cbcflow/inputs/gracedb.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14974 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/inputs/pe_scraper.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      314 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      316 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/monitor.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.116452 cbcflow-0.4.4/src/cbcflow/outputs/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       69 2023-10-04 20:55:03.000000 cbcflow-0.4.4/src/cbcflow/outputs/__init__.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3418 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/outputs/asimov.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      310 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/parser.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      322 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/pe_scraper.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      312 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/process.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.122452 cbcflow-0.4.4/src/cbcflow/schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow/schema/cbc-meta-data-v2.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)   134922 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow/schema/cbc-meta-data-v3.schema
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow/schema/index-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      310 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/schema.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      308 2024-03-11 14:49:50.000000 cbcflow-0.4.4/src/cbcflow/utils.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.153452 cbcflow-0.4.4/src/cbcflow.egg-info/
--rw-r--r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3652 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow.egg-info/PKG-INFO
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3937 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow.egg-info/SOURCES.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow.egg-info/dependency_links.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      625 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow.egg-info/entry_points.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      144 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow.egg-info/requires.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2024-03-18 17:53:54.000000 cbcflow-0.4.4/src/cbcflow.egg-info/top_level.txt
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.127452 cbcflow-0.4.4/tests/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.140452 cbcflow-0.4.4/tests/files_for_testing/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26314 2024-03-15 16:52:25.000000 cbcflow-0.4.4/tests/files_for_testing/cbc-meta-data-example.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.4.4/tests/files_for_testing/merge_test.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.4.4/tests/files_for_testing/test-file-for-linking-1.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.4.4/tests/files_for_testing/test-file-for-linking-2.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.4.4/tests/files_for_testing/test-file-for-linking-3.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.4.4/tests/files_for_testing/update_json_1.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.4.4/tests/files_for_testing/update_json_2.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.4.4/tests/files_for_testing/update_yaml_1.yaml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.4.4/tests/files_for_testing/update_yaml_2.yaml
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-03-18 17:53:55.152452 cbcflow-0.4.4/tests/library_for_testing/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5514 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4444 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4430 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2529 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3487 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5414 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3390 2024-03-15 16:51:51.000000 cbcflow-0.4.4/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.4.4/tests/library_for_testing/library.cfg
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.4.4/tests/library_for_testing/testing-library-index.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3529 2023-09-19 22:38:51.000000 cbcflow-0.4.4/tests/test_database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38506 2023-09-19 22:38:51.000000 cbcflow-0.4.4/tests/test_merging.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    32841 2023-09-19 22:38:51.000000 cbcflow-0.4.4/tests/test_metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      782 2024-03-15 17:08:35.000000 cbcflow-0.4.4/tests/test_schema.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.774399 cbcflow-0.5.0/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.5.0/.gitattributes
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      229 2024-04-10 18:22:08.000000 cbcflow-0.5.0/.gitignore
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1602 2024-04-10 18:22:09.000000 cbcflow-0.5.0/.gitlab-ci.yml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-12-08 19:49:13.000000 cbcflow-0.5.0/.pre-commit-config.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.5.0/CHANGELOG.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.5.0/LICENSE.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.5.0/MANIFEST.in
+-rw-r--r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3652 2024-04-30 22:05:22.771399 cbcflow-0.5.0/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2676 2023-08-15 18:08:33.000000 cbcflow-0.5.0/README.md
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.435396 cbcflow-0.5.0/docs/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.5.0/docs/Makefile
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/requirements.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.491396 cbcflow-0.5.0/docs/source/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.495396 cbcflow-0.5.0/docs/source/_templates/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.5.0/docs/source/_templates/custom-class-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.5.0/docs/source/_templates/custom-module-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/actionitems.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/adding-to-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/asimov.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.5.0/docs/source/cbcflow-git-merging.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/conf.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/configuration.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/development-setup.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.502396 cbcflow-0.5.0/docs/source/example_mini_schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/example_mini_schema/example.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/example_mini_schema/schema_doc.css
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/example_mini_schema/schema_doc.html
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/example_mini_schema/schema_doc.min.js
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/gwosc.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/index.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.612398 cbcflow-0.5.0/docs/source/libraries_images/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.629398 cbcflow-0.5.0/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_1.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_2.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_3.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_4.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_5.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_6.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_7.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/libraries_images/part_8.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/library-index-labelling.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/library-indices.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.5.0/docs/source/library-setup-from-scratch.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/local-library-copy-setup.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/monitor-usage.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/reading-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.5.0/docs/source/schema-visualization.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/updating-metadata-from-the-command-line.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2024-03-11 16:28:04.000000 cbcflow-0.5.0/docs/source/updating-metadata-with-the-python-api.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.5.0/docs/source/what-is-metadata.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.645398 cbcflow-0.5.0/examples/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.5.0/examples/initial_example.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      899 2024-04-10 18:22:09.000000 cbcflow-0.5.0/pyproject.toml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.654398 cbcflow-0.5.0/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.5.0/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.5.0/schema/cbc-meta-data-v2.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)   134922 2024-04-10 18:22:09.000000 cbcflow-0.5.0/schema/cbc-meta-data-v3.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.5.0/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1748 2024-04-30 22:05:22.776399 cbcflow-0.5.0/setup.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      617 2024-04-10 18:22:09.000000 cbcflow-0.5.0/setup.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.399396 cbcflow-0.5.0/src/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.670398 cbcflow-0.5.0/src/cbcflow/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1129 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      411 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow/_version.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      386 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/asimov.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      317 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/cbcflow.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.683398 cbcflow-0.5.0/src/cbcflow/client/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       47 2023-10-04 20:55:03.000000 cbcflow-0.5.0/src/cbcflow/client/__init__.py
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9756 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/client/cbcflow.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1309 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/client/migrate_v2_to_v3.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6133 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/client/monitor.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.695398 cbcflow-0.5.0/src/cbcflow/core/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       89 2023-10-04 20:55:03.000000 cbcflow-0.5.0/src/cbcflow/core/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    48884 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/core/database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15693 2023-11-30 19:49:31.000000 cbcflow-0.5.0/src/cbcflow/core/metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9630 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/core/parser.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-09-19 22:38:51.000000 cbcflow-0.5.0/src/cbcflow/core/process.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3531 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/core/schema.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8332 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/core/utils.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1581 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/core/wrapped.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      314 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      316 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/gracedb.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.700398 cbcflow-0.5.0/src/cbcflow/inputs/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      116 2023-10-04 20:55:03.000000 cbcflow-0.5.0/src/cbcflow/inputs/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    13145 2023-10-13 16:04:41.000000 cbcflow-0.5.0/src/cbcflow/inputs/asimov.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    20026 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/inputs/gracedb.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    19294 2024-04-30 21:57:02.000000 cbcflow-0.5.0/src/cbcflow/inputs/pe_scraper.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      314 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      316 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/monitor.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.703398 cbcflow-0.5.0/src/cbcflow/outputs/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       69 2023-10-04 20:55:03.000000 cbcflow-0.5.0/src/cbcflow/outputs/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3418 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/outputs/asimov.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      310 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/parser.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      322 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/pe_scraper.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      312 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/process.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.711398 cbcflow-0.5.0/src/cbcflow/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)   134922 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow/schema/cbc-meta-data-v3.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      310 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/schema.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      308 2024-03-11 14:49:50.000000 cbcflow-0.5.0/src/cbcflow/utils.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.769399 cbcflow-0.5.0/src/cbcflow.egg-info/
+-rw-r--r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3652 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow.egg-info/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3896 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      625 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow.egg-info/entry_points.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      144 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow.egg-info/requires.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2024-04-30 22:05:22.000000 cbcflow-0.5.0/src/cbcflow.egg-info/top_level.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.718398 cbcflow-0.5.0/tests/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.751399 cbcflow-0.5.0/tests/files_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26314 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/files_for_testing/cbc-meta-data-example.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.5.0/tests/files_for_testing/merge_test.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.5.0/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.5.0/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.5.0/tests/files_for_testing/test-file-for-linking-3.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.5.0/tests/files_for_testing/update_json_1.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.5.0/tests/files_for_testing/update_json_2.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.5.0/tests/files_for_testing/update_yaml_1.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.5.0/tests/files_for_testing/update_yaml_2.yaml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2024-04-30 22:05:22.767399 cbcflow-0.5.0/tests/library_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5514 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4444 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4430 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2529 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3487 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5414 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3390 2024-04-10 18:22:10.000000 cbcflow-0.5.0/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.5.0/tests/library_for_testing/library.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.5.0/tests/library_for_testing/testing-library-index.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3529 2023-09-19 22:38:51.000000 cbcflow-0.5.0/tests/test_database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3865 2024-04-30 21:57:02.000000 cbcflow-0.5.0/tests/test_gracedb.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38506 2023-09-19 22:38:51.000000 cbcflow-0.5.0/tests/test_merging.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    32841 2023-09-19 22:38:51.000000 cbcflow-0.5.0/tests/test_metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      820 2024-04-30 21:57:02.000000 cbcflow-0.5.0/tests/test_schema.py
```

### Comparing `cbcflow-0.4.4/.gitlab-ci.yml` & `cbcflow-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/.pre-commit-config.yaml` & `cbcflow-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/CHANGELOG.md` & `cbcflow-0.5.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/LICENSE.md` & `cbcflow-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/PKG-INFO` & `cbcflow-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.4.4
+Version: 0.5.0
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.4.4/README.md` & `cbcflow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/Makefile` & `cbcflow-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.5.0/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.5.0/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/actionitems.rst` & `cbcflow-0.5.0/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/adding-to-the-schema.rst` & `cbcflow-0.5.0/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/cbcflow-git-merging.rst` & `cbcflow-0.5.0/docs/source/cbcflow-git-merging.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/conf.py` & `cbcflow-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/configuration.rst` & `cbcflow-0.5.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/development-setup.rst` & `cbcflow-0.5.0/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/example_mini_schema/example.schema` & `cbcflow-0.5.0/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.5.0/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.5.0/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.5.0/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/index.rst` & `cbcflow-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries.rst` & `cbcflow-0.5.0/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.5.0/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_1.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_2.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_3.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_4.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_5.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_6.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_7.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/libraries_images/part_8.png` & `cbcflow-0.5.0/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/library-index-labelling.rst` & `cbcflow-0.5.0/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/library-indices.rst` & `cbcflow-0.5.0/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/library-setup-from-scratch.rst` & `cbcflow-0.5.0/docs/source/library-setup-from-scratch.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/local-library-copy-setup.rst` & `cbcflow-0.5.0/docs/source/local-library-copy-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/monitor-usage.rst` & `cbcflow-0.5.0/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/reading-the-schema.rst` & `cbcflow-0.5.0/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.5.0/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.5.0/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/docs/source/what-is-metadata.rst` & `cbcflow-0.5.0/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/examples/initial_example.md` & `cbcflow-0.5.0/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/pyproject.toml` & `cbcflow-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/schema/cbc-meta-data-v1.schema` & `cbcflow-0.5.0/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/schema/cbc-meta-data-v2.schema` & `cbcflow-0.5.0/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/schema/cbc-meta-data-v3.schema` & `cbcflow-0.5.0/schema/cbc-meta-data-v3.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/schema/index-v1.schema` & `cbcflow-0.5.0/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/setup.cfg` & `cbcflow-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/setup.py` & `cbcflow-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/__init__.py` & `cbcflow-0.5.0/src/cbcflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     setup_args_metadata,
     pull,
     print_metadata,
     update,
     validate_library,
     cbcflow_git_merge,
 )
-from .core.configuration import get_cbcflow_config
 from .core.metadata import MetaData
 from .core.database import LocalLibraryDatabase
 from .client.monitor import generate_crondor, generate_crontab, run_monitor
 from .core.parser import get_parser_and_default_data
 from .core.schema import get_schema
 from .core.wrapped import get_superevent
 from .client.migrate_v2_to_v3 import main as migrate_schema_v2_to_v3
@@ -26,15 +25,14 @@
 logger.info(
     "Also including old import paths as well, e.g. `cbcflow.database`\n\
     These will be deprecated at some point in the future."
 )
 
 from .core import database
 from .core import wrapped as cbcflow
-from .core import configuration
 from .inputs import gracedb
 from .core import metadata
 from .client import monitor
 from .core import parser
 from .inputs import pe_scraper
 from .core import process
 from .core import schema
```

### Comparing `cbcflow-0.4.4/src/cbcflow/client/cbcflow.py` & `cbcflow-0.5.0/src/cbcflow/client/cbcflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 
 """Client level methods for cbcflow (i.e. those that use argument parsing)"""
 
 import argparse
 import copy
 import glob
 import json
+import os
 from typing import Tuple
 
-
-from ..core.configuration import config_defaults
 from ..inputs.gracedb import fetch_gracedb_information
 from ..inputs.pe_scraper import add_pe_information
 from ..core.metadata import MetaData
 from ..core.database import LocalLibraryDatabase
 from ..core.parser import get_parser_and_default_data, sname_string
 from ..core.process import process_user_input
-from ..core.schema import get_schema
+from ..core.schema import get_schema, get_schema_from_args
 from ..core.utils import setup_logger
 
 
 def setup_args_metadata() -> Tuple[argparse.Namespace, "MetaData"]:
     """Take in command line arguments, and return a metadata object
 
     Returns
     =======
     argparse.Namespace
         A namespace generated by parsing the input arguments
     MetaData
         A metadata object generated by the parsing of the arguments
     """
-    schema = get_schema()
+    schema = get_schema_from_args()
     parser, default_data = get_parser_and_default_data(schema)
     args = parser.parse_args()
 
     # Set the sname in the default data
     default_data["Sname"] = args.sname
 
     # Instantiate the metadata
@@ -97,21 +96,24 @@
             check_changes=check_changes, branch_name=args.branch_name
         )
 
 
 def print_metadata() -> None:
     """Print the metadata for a given event in a given library, as passed in args"""
     # Read in command line arguments
-    schema = get_schema()
+    schema = get_schema_from_args()
     _, default_data = get_parser_and_default_data(schema)
 
     parser = argparse.ArgumentParser()
     parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     parser.add_argument(
-        "--library", default=config_defaults["library"], help="The library"
+        "--library",
+        default=os.getcwd(),
+        help="The library in which the metadata file in question is stored, defaults to cwd",
+        type=str,
     )
     args = parser.parse_args()
 
     # Set the sname in the default data
     default_data["Sname"] = args.sname
 
     # Instantiate the metadata
@@ -124,40 +126,37 @@
 
     metadata.pretty_print()
 
 
 def from_file() -> None:
     """Given a superevent and an update file, apply the updates"""
     # Read in command line arguments
-    schema = get_schema()
+    schema = get_schema_from_args()
     _, default_data = get_parser_and_default_data(schema)
 
     file_parser = argparse.ArgumentParser()
     file_parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     file_parser.add_argument(
         "update_file",
         help="The file to update from, either a json or a yaml.\
         The type of file will be inferred from the ending .yaml or .json",
     )
     file_parser.add_argument(
+        "--library",
+        default=os.getcwd(),
+        help="The library in which the metadata file in question is stored, defaults to cwd",
+        type=str,
+    )
+    file_parser.add_argument(
         "--removal-file",
         action="store_true",
         help="If passed, this will be treated as a negative image,\
             so array elements will be removed instead of added",
     )
     file_parser.add_argument(
-        "--library", default=config_defaults["library"], help="The library"
-    )
-    file_parser.add_argument("--schema-version", help="The schema version to use")
-    file_parser.add_argument(
-        "--schema-file",
-        help="Explicit path to the schema-file. If None (default) the inbuilt schema is used",
-        default=config_defaults["schema"],
-    )
-    file_parser.add_argument(
         "--no-git-library",
         action="store_true",
         help="If true, do not treat the library as a git repo",
     )
     file_parser.add_argument(
         "--branch-name",
         help="The name of the branch to which commits should be written."
@@ -167,14 +166,26 @@
         default=None,
     )
     file_parser.add_argument(
         "--yes",
         help="Do not ask for confirmation",
         action="store_true",
     )
+    file_parser.add_argument(
+        "--schema-version",
+        help="The schema version to use, defaults to most recent",
+        type=str,
+        default=None,
+    )
+    file_parser.add_argument(
+        "--schema-file",
+        help="Explicit path to the schema-file. If None (default) the inbuilt schema is used",
+        type=str,
+        default=None,
+    )
     args = file_parser.parse_args()
 
     # Set the sname in the default data
     default_data["Sname"] = args.sname
 
     # Instantiate the metadata
     metadata = MetaData(
@@ -215,15 +226,15 @@
 
 
 def validate_library() -> None:
     """Go through the library, validating that all metadata files satisfy the schema"""
     from jsonschema.exceptions import ValidationError
 
     # Read in command line arguments
-    schema = get_schema()
+    schema = get_schema_from_args()
     _, default_data = get_parser_and_default_data(schema)
 
     # Set up argument parser
     parser = argparse.ArgumentParser()
     parser.add_argument("library", help="The library to validate")
     args = parser.parse_args()
 
@@ -260,17 +271,17 @@
         "ourfile", type=str, help="The version of the file on our current branch"
     )
     parser.add_argument(
         "theirfile", type=str, help="The version of the file on the other branch"
     )
     parser.add_argument(
         "--library",
+        default=os.getcwd(),
+        help="The library in which the metadata file in question is stored, defaults to cwd",
         type=str,
-        default=config_defaults["library"],
-        help="The library to operate in",
     )
     args = parser.parse_args()
 
     logger.info(f"Merging file {args.ourfile}")
 
     # Setup the library, necessary to do the merge operation
     local_library = LocalLibraryDatabase(args.library)
```

### Comparing `cbcflow-0.4.4/src/cbcflow/client/migrate_v2_to_v3.py` & `cbcflow-0.5.0/src/cbcflow/client/migrate_v2_to_v3.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("library", help="The library to convert", type=str)
     args = parser.parse_args()
 
-    v2_schema = get_schema(["--schema-version", "v2"])
-    v3_schema = get_schema(["--schema-version", "v3"])
+    v2_schema = get_schema(version="v2")
+    v3_schema = get_schema(version="v3")
 
     library = LocalLibraryDatabase(library_path=args.library, schema=v2_schema)
 
     library.load_library_metadata_dict()
     library.metadata_schema = v3_schema
 
     for superevent, metadata in library.metadata_dict.items():
```

### Comparing `cbcflow-0.4.4/src/cbcflow/client/monitor.py` & `cbcflow-0.5.0/src/cbcflow/client/monitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 import os
 from shutil import which
 
 from glue import pipeline
 from crontab import CronTab
 
 from ..core.utils import setup_logger
-from ..core.configuration import get_cbcflow_config
 from ..core.database import LocalLibraryDatabase
 
 logger = setup_logger()
 
 
 def get_base_parser():
     """Generate the standard monitor parser"""
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        "--config-file",
-        default="~/.cbcflow.cfg",
-        help="The cfg from which to obtain monitor configuration info",
+        "library",
+        help="The library which the monitor will update",
     )
     parser.add_argument(
         "--monitor-interval",
         type=int,
         default=2,
         help="The interval in hours between runs of the monitoring job",
     )
@@ -55,17 +53,17 @@
 
     if args.rundir is None:
         rundir = os.getcwd()
     else:
         rundir = args.rundir
 
     monitor_exe = which("cbcflow_monitor_run")
-    monitor_args = f" {os.path.expanduser(args.config_file)} "
+    monitor_args = f" {os.path.expanduser(args.library)} "
 
-    log_file = f"{rundir}/cbcflow.log"
+    log_file = f"{rundir}/monitor.log"
 
     cron = CronTab(user=args.user_name)
     job = cron.new(command=f"{monitor_exe} {monitor_args} >> {log_file} 2>&1")
     job.hour.every(args.monitor_interval)
     job.minute.on(args.monitor_minute)
     cron.write()
 
@@ -107,15 +105,15 @@
     monitor_job.add_condor_cmd("get_env", "True")
     monitor_job.add_condor_cmd("on_exit_remove", "False")
     # These are the unusual settings - this makes the job repeat every N hours, at the Mth minute
     monitor_job.add_condor_cmd("cron_minute", f"{args.monitor_minute}")
     monitor_job.add_condor_cmd("cron_hour", f"* / {args.monitor_interval}")
     # This tells the job to queue 5 minutes before it's execution time, so it will be ready when the time comes
     monitor_job.add_condor_cmd("cron_prep_time", "300")
-    monitor_args = f" {os.path.expanduser(args.config_file)} "
+    monitor_args = f" {os.path.expanduser(args.library)} "
     monitor_job.add_arg(monitor_args)
     sub_path = os.path.join(rundir, "monitor.sub")
     monitor_job.set_sub_file(sub_path)
     monitor_job.write_sub_file()
 
     os.system(f"condor_submit {sub_path}")
 
@@ -123,43 +121,41 @@
 def run_monitor() -> None:
     """
     Pulls all superevents created within the past 30 days, creates metadata if necessary,
     then pushes back any changes made in this process
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        "cbcflowconfig",
+        "library",
         type=str,
-        help="The .cbcflow.cfg file to use for library and service URL info",
+        help="The path to the library to operate on",
     )
     parser.add_argument(
         "--branch-name",
         type=str,
         default="main",
         help="The branch the monitor should write to - defaults to main",
     )
     args = parser.parse_args()
 
-    config_values = get_cbcflow_config(args.cbcflowconfig)
-    local_library = LocalLibraryDatabase(library_path=config_values["library"])
+    local_library = LocalLibraryDatabase(library_path=args.library)
     logger.info("CBCFlow monitor is beginning sweep")
     logger.info("Attempting to pull from remote")
     # Pull before we potentially checkout a new branch
     local_library.git_pull_from_remote(automated=True)
     # Make sure we switch to main for monitor operations
     local_library.git_checkout_new_branch(branch_name=args.branch_name)
     # Pull again in case the remote already existed and we want to update it
     if local_library.remote_has_merge_conflict:
         logger.info(
             "Could not pull from remote, continuing with standard sync sequence\n\
                     Before these changes can be propagated to the remote, this merge conflict\n\
                     must be resolved manually."
         )
-    logger.info(f"Config values are {config_values}")
-    local_library.initialize_parent(source_path=config_values["gracedb_service_url"])
+    local_library.initialize_parent()
     # Note that we explicitly sync to main instead of any other branch
     local_library.library_parent.sync_library(branch_name=args.branch_name)
     logger.info("Updating index file for library")
     # For now we don't want to do any labelling locally, instead doing it all in gitlab
     # set_working_index... will change LastUpdate and add events
     # but won't touch the labels
     local_library.set_working_index_with_updates_to_file_index()
```

### Comparing `cbcflow-0.4.4/src/cbcflow/core/database.py` & `cbcflow-0.5.0/src/cbcflow/core/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import glob
 import json
 import os
 import ast
 from functools import cached_property
 import sys
 from pprint import pformat
-from typing import Union, Dict, Type, TypeVar, Tuple
+from typing import Union, Dict, Type, TypeVar, Tuple, Optional, List
 from datetime import datetime
 
 import dateutil.parser as dp
 from jsondiff import diff
 import jsonschema
 import git
 import tqdm
@@ -238,14 +238,33 @@
         pe_rota_token_path : str
             The path to the token to use when accessing the PE rota
         """
         super(GraceDbDatabase, self).__init__(source_path=service_url, library=library)
         self.cred = cred
         self.pe_rota_token = pe_rota_token_path
 
+        # Do the setup of the standard query from the library config here
+        self.event_config = self.library.library_config["Events"]
+
+        # annying hack due to gracedb query bug
+        import datetime
+        from gwpy.time import to_gps
+
+        start_gps = to_gps(self.event_config["earliest-library-datetime"])
+        # to_gps understands 'now'
+        end_gps = to_gps(self.event_config["latest-library-datetime"])
+
+        now = datetime.datetime.utcnow()
+
+        logger.info(f"Syncing with GraceDB at {now}")
+        # make query and defaults, query
+        self.library_query = f"gpstime: {start_gps} .. {end_gps} \
+        FAR <= {self.event_config['far-threshold']}"
+        logger.info(f"Constructed query {self.library_query} from library config")
+
     @property
     def cred(self) -> Union[Tuple[str, str], str, None]:
         """Information on the credentials to pass to GraceDb, per
         https://ligo-gracedb.readthedocs.io/en/latest/api.html#ligo.gracedb.rest.GraceDb
         """
         return self._cred
 
@@ -275,34 +294,45 @@
             The sname for the superevent in question
 
         Returns
         =======
         dict
             The GraceDB data for the superevent
         """
-        return fetch_gracedb_information(
-            sname, service_url=self.source_path, cred=self.cred
-        )
+        try:
+            return fetch_gracedb_information(
+                sname, service_url=self.source_path, cred=self.cred
+            )
+        except Exception:
+            logger.warning(
+                f"Failed with exception {Exception} to fetch gracedb information for {sname},\
+                no update will be performed"
+            )
+            return None
 
-    def query_superevents(self, query: str) -> list:
+    def query_superevents(self, query: Optional[str] = None) -> list:
         """Queries superevents in GraceDb, according to a given query
 
         Parameters
         ==========
         query : str
             a GraceDb query string to query for superevents
-            see https://gracedb.ligo.org/documentation/queries.html
+            see https://gracedb.ligo.org/documentation/queries.html.
+            Defaults to the query constructed from the library config.
 
         Returns
         =======
         list
             The superevents which satisfy the query
         """
         from ligo.gracedb.rest import GraceDb
 
+        if query is None:
+            query = self.library_query
+
         queried_superevents = []
         with GraceDb(service_url=self.source_path, cred=self.cred) as gdb:
             superevent_iterator = gdb.superevents(query)
             for superevent in superevent_iterator:
                 queried_superevents.append(superevent["superevent_id"])
         return queried_superevents
 
@@ -312,115 +342,101 @@
         Parameters
         ==========
         branch_name : str, optional
             The name of the branch to write to, as passed to `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`
         """
         from ligo.gracedb.exceptions import HTTPError
 
-        if hasattr(self, "superevents_to_propagate"):
-            for superevent_id in tqdm.tqdm(self.superevents_to_propagate):
-                logger.info(f"Updating superevent {superevent_id}")
-                if superevent_id in self.library.metadata_dict.keys():
-                    metadata = self.library.metadata_dict[superevent_id]
-                else:
-                    metadata = MetaData(
-                        superevent_id,
-                        local_library=self.library,
-                        schema=self.library.metadata_schema,
-                        default_data=self.library.metadata_default_data,
-                    )
-                    assert (
-                        len(self.library.metadata_default_data["Info"]["Notes"]) == 0
-                    ), "Something has gone horribly wrong and modified the defaults"
-                try:
-                    backup_data = copy.deepcopy(metadata.data)
-
-                    # Pull information from GraceDB
-                    gdb_data = self.pull(superevent_id)
-                    for note in metadata["Info"]["Notes"]:
-                        # If a note already marks this as retracted don't add another
-                        if "retracted" in note.lower():
-                            gdb_data.pop("Info")
-                            break
-                    metadata.data.update(gdb_data)
-
-                    try:
-                        # Pull information from PE
-                        add_pe_information(metadata, superevent_id, self.pe_rota_token)
-                    except Exception as e:
-                        logger.warning(
-                            f"Fatal error while scraping PE automatically for superevent {superevent_id}"
-                        )
-                        logger.warning(
-                            "Proceeding automatically to maintain library status as best as possible"
-                        )
-                        logger.warning(f"The exception was {e}")
-
-                    changes = metadata.get_diff()
-                    if "GraceDB" in changes.keys() and len(changes.keys()) == 1:
-                        if len(changes["GraceDB"].keys()) == 1:
-                            continue
-                        # This is a hack to make it not update if the only update would be "LastUpdate"
-                        # It may have to change in further schema versions
-                    logger.info(f"Updates to supervent {superevent_id}")
-                    string_rep_changes = get_dumpable_json_diff(changes)
-                    logger.debug(json.dumps(string_rep_changes, indent=2))
-                    metadata.write_to_library(branch_name=branch_name)
-                except jsonschema.exceptions.ValidationError:
-                    logger.warning(
-                        f"For superevent {superevent_id}, GraceDB generated metadata failed validation\
-                        Writing backup data (either default or pre-loaded) to library instead\n"
-                    )
-                    metadata.update(backup_data)
-                    metadata.write_to_library(branch_name=branch_name)
-                except HTTPError:
-                    logger.warning(
-                        f"For superevent {superevent_id}, failed to obtain data from GraceDB\
-                        Writing backup data (either default or pre-loaded) to library instead\n"
-                    )
-                    metadata.update(backup_data)
-                    metadata.write_to_library(branch_name=branch_name)
-        else:
+        if not hasattr(self, "superevents_to_propagate"):
             logger.info(
                 "This GraceDbDatabase instance has not assigned any superevents to propagate yet\
                  please do so before attempting to pull them."
             )
+            return None
+        for superevent_id in tqdm.tqdm(self.superevents_to_propagate):
+            logger.info(f"Updating superevent {superevent_id}")
+            if superevent_id in self.library.metadata_dict.keys():
+                metadata = self.library.metadata_dict[superevent_id]
+            else:
+                metadata = MetaData(
+                    superevent_id,
+                    local_library=self.library,
+                    schema=self.library.metadata_schema,
+                    default_data=self.library.metadata_default_data,
+                )
+                assert (
+                    len(self.library.metadata_default_data["Info"]["Notes"]) == 0
+                ), "Something has gone horribly wrong and modified the defaults"
+            updated_metadata = copy.deepcopy(metadata)
+
+            # Note - we will *always* clear the g-events from an event before
+            # starting the update loop, even though it's only strictly necessary
+            # in catalog operations. This saves a lot of code duplication.
+            # If something fails in the update loop then
+            # The metadata won't be updated in total, so this should be safe
+            # (the failure mode would be if Gracedb 'successfully' returned 0 events
+            # In which case the issue would be something upstream)
+            updated_metadata["GraceDB"]["Events"] = []
+
+            # Pull information from GraceDB
+            gdb_data = self.pull(superevent_id)
+            for note in metadata["Info"]["Notes"]:
+                # If a note already marks this as retracted don't add another
+                if "retracted" in note.lower() and "Info" in gdb_data:
+                    gdb_data.pop("Info")
+                    break
+            if gdb_data is not None:
+                try:
+                    updated_metadata.update(gdb_data)
+                    metadata = updated_metadata
+                except jsonschema.ValidationError:
+                    logger.warning(
+                        f"For superevent {superevent_id}, GraceDB generated metadata failed validation\n\
+                        No GraceDB information will be updated\n"
+                    )
+
+            try:
+                # Pull information from PE
+                add_pe_information(updated_metadata, superevent_id, self.pe_rota_token)
+                metadata = updated_metadata
+            except Exception as e:
+                logger.warning(
+                    f"Fatal error while scraping PE automatically for superevent {superevent_id}"
+                )
+                logger.warning("No PE information will be updated")
+                logger.warning(f"The exception was {e}")
+
+            changes = metadata.get_diff()
+            if "GraceDB" in changes.keys() and len(changes.keys()) == 1:
+                # This is a hack to make it not update if the only update would be "LastUpdate"
+                # It may have to change in further schema versions
+                if len(changes["GraceDB"].keys()) == 1:
+                    continue
+
+            logger.info(f"Updates to supervent {superevent_id}")
+            string_rep_changes = get_dumpable_json_diff(changes)
+            logger.debug(json.dumps(string_rep_changes, indent=2))
+            metadata.write_to_library(branch_name=branch_name)
 
     def sync_library(self, branch_name: Union[str, None] = None) -> None:
         """Attempts to sync library and GraceDb,
         pulling any new events and changes to GraceDB data.
 
         Parameters
         ==========
         branch_name : str | None, optional
             The branch_name to write commits to, per `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`
         """
         from ligo.gracedb.exceptions import HTTPError
-        from gwpy.time import to_gps
-
-        # setup defaults
-        # monitor_config = local_library.library_config["Monitor"]
-        event_config = self.library.library_config["Events"]
-
-        # annying hack due to gracedb query bug
-        import datetime
-
-        start_gps = to_gps(event_config["earliest-library-datetime"])
-        # to_gps understands 'now'
-        end_gps = to_gps(event_config["latest-library-datetime"])
 
-        now = datetime.datetime.utcnow()
-
-        logger.info(f"Syncing with GraceDB at {now}")
-        # make query and defaults, query
-        query = f"gpstime: {start_gps} .. {end_gps} \
-        FAR <= {event_config['far-threshold']}"
-        logger.info(f"Constructed query {query} from library config")
         try:
-            self.superevents_to_propagate = self.query_superevents(query)
+            self.superevents_to_propagate = self.query_superevents(
+                query=self.library_query
+            )
+            # TODO self.superevents_to_propogate should now include only catalog superevents satsifying the query
         except HTTPError:
             self.superevents_to_propagate = []
             logger.warning(
                 "Query to GraceDB for superevents unsuccessful \
                            - falling back on superevents already in library only"
             )
 
@@ -448,14 +464,123 @@
         self.superevents_to_propagate = list(
             set(self.superevents_to_propagate) - set(specially_excuded_snames)
         )
 
         self.pull_library_updates(branch_name=branch_name)
 
 
+class CatalogGraceDbDatabase(GraceDbDatabase):
+    def __init__(
+        self,
+        service_url: str,
+        library: "LocalLibraryDatabase",
+        cred: Tuple[str, str] | str | None = None,
+        pe_rota_token_path: str | None = None,
+    ) -> None:
+        super().__init__(service_url, library, cred, pe_rota_token_path)
+        self.catalog_number = library.library_config["Catalog"]["number"]
+        self.catalog_query_version = library.library_config["Catalog"]["version"]
+
+    def pull(self, sname: str) -> dict:
+        """Pull information on the superevent with this sname from GraceDB
+
+        Parameters
+        ==========
+        sname : str
+            The sname for the superevent in question
+
+        Returns
+        =======
+        dict
+            The GraceDB data for the superevent
+        """
+        try:
+            return fetch_gracedb_information(
+                sname,
+                service_url=self.source_path,
+                cred=self.cred,
+                catalog_mode=True,
+                catalog_number=self.catalog_number,
+                catalog_version=self.catalog_table_version,
+                gevent_ids=[
+                    x for x in self.catalog_superevents[sname]["pipelines"].values()
+                ],
+                catalog_superevent_far=self.catalog_superevents[sname]["far"],
+                catalog_superevent_pastro=self.catalog_superevents[sname]["pastro"],
+            )
+        except Exception as exception:
+            logger.warning(
+                f"Failed with exception:\n\
+                {exception}\n\
+                to fetch gracedb information for {sname},\
+                no update will be performed"
+            )
+            return None
+
+    @property
+    def catalog_superevents(self) -> Dict[str, List[str]]:
+        """A map of superevents to catalog gevents for superevents which are in the catalog"""
+        return self._catalog_superevents
+
+    @catalog_superevents.setter
+    def catalog_superevents(self, catalog_superevents: Dict[str, List[str]]) -> None:
+        self._catalog_superevents = catalog_superevents
+
+    @property
+    def catalog_query_version(self) -> Union[str, int]:
+        """The version of the catalog table to query - either a number or "latest" """
+        return self._catalog_query_version
+
+    @catalog_query_version.setter
+    def catalog_query_version(self, catalog_query_version: Union[str, int]):
+        self._catalog_query_version = catalog_query_version
+
+    @property
+    def catalog_table_version(self) -> int:
+        """The version of the gwtc catalog table which was obtained from the query."""
+        return self._catalog_table_version
+
+    @catalog_table_version.setter
+    def catalog_table_version(self, catalog_table_version: int):
+        self._catalog_table_version = catalog_table_version
+
+    def query_superevents(self, query: Optional[str] = None) -> list:
+        """Query for superevents in the catalog
+
+        Parameters
+        ==========
+        query : Optional[str]
+            This parameter is included for API compatibililty, but is ignored for Catalog operations
+        """
+        from gwtc.gwtc_gracedb import GWTCGraceDB
+
+        if query is None:
+            query = self.library_query
+
+        # standard query structure: "gpstime: {start_gps} .. {end_gps} \
+        # FAR <= {self.event_config['far-threshold']}"
+        # so split() then take 2 indexes further
+        far_threshold = float(query.split()[query.split().index("FAR") + 2])
+
+        with GWTCGraceDB(service_url=self.source_path, cred=self.cred) as gdb:
+            gwtc_table = gdb.gwtc_get(
+                number=self.catalog_number, version=self.catalog_query_version
+            ).json()
+            catalog_superevents_map = gwtc_table["gwtc_superevents"]
+            catalog_superevents = {
+                k: v
+                for k, v in catalog_superevents_map.items()
+                if v["far"] <= far_threshold
+            }
+            self.catalog_table_version = gwtc_table["version"]
+
+        self.catalog_superevents = catalog_superevents
+        return [k for k in catalog_superevents.keys()]
+
+
 class LocalLibraryDatabase(object):
     """An object reflecting the contents of a local library, and offering methods to interact with it"""
 
     def __init__(
         self,
         library_path: str,
         schema: Union[dict, None] = None,
@@ -496,15 +621,15 @@
 
         Parameters
         ==========
         source_path
             The path (GraceDB url, git url, or filesystem path) to the parent source
         """
         if source_path is None:
-            source_path = self.library_config["Monitor"]["parent"]
+            source_path = self.library_config["Monitor"]["gracedb-service-url"]
             logger.info(
                 f"Initializing parent from configuration, with source path {source_path}"
             )
         if "https://gracedb" in source_path:
             if self.library_config["Monitor"]["cred"] is not None:
                 import re
 
@@ -526,30 +651,43 @@
             if self.library_config["Monitor"]["pe_rota_token"] is not None:
                 if self.library_config["Monitor"]["pe_rota_token"].lower() != "none":
                     pe_rota_token_path = self.library_config["Monitor"]["pe_rota_token"]
                 else:
                     pe_rota_token_path = None
             else:
                 pe_rota_token_path = None
-            self._library_parent = GraceDbDatabase(
-                service_url=source_path,
-                library=self,
-                cred=cred,
-                pe_rota_token_path=pe_rota_token_path,
-            )
+            if self.library_config["Monitor"]["parent"] == "gracedb":
+                self._library_parent = GraceDbDatabase(
+                    service_url=source_path,
+                    library=self,
+                    cred=cred,
+                    pe_rota_token_path=pe_rota_token_path,
+                )
+            elif self.library_config["Monitor"]["parent"] == "gwtc-gracedb":
+                self._library_parent = CatalogGraceDbDatabase(
+                    service_url=source_path,
+                    library=self,
+                    cred=cred,
+                    pe_rota_token_path=pe_rota_token_path,
+                )
+            else:
+                raise ValueError(
+                    f"{self.library_config['Monitor']['parent']} is not a valid parent"
+                )
         elif os.path.exists(source_path):
             # This will be the branch for pulling from a git repo in the local filesystem
             pass
         elif "https" in source_path:
             # This will be the branch for pulling from a non-local git repo on e.g. gitlab
             pass
         else:
             raise ValueError(
                 f"Could not obtain source information from path {source_path}"
             )
+        return self._library_parent
 
     @property
     def filelist(self) -> list:
         """The list of cbc metadata jsons in this library"""
         return glob.glob(os.path.join(self.library, "*cbc-metadata.json"))
 
     @property
@@ -680,17 +818,19 @@
             "earliest-library-datetime": "2022-01-01",
             "latest-library-datetime": "now",
             "snames-to-include": [],
             "snames-to-exclude": [],
         }
         library_defaults["Monitor"] = {
             "parent": "gracedb",
+            "gracedb-service-url": "https://gracedb.ligo.org/api/",
             "cred": None,
             "pe_rota_token": None,
         }
+        library_defaults["Catalog"] = {"number": "4", "version": "latest"}
         if os.path.exists(config_file):
             config.read(config_file)
             for section_key in config.sections():
                 if section_key not in library_defaults.keys():
                     library_defaults[section_key] = dict()
                 section = config[section_key]
                 if (
@@ -940,15 +1080,15 @@
         """The file path to the library's index json"""
         index_file = os.path.join(self.library, self.index_file_name)
         return index_file
 
     @property
     def library_index_schema(self) -> dict:
         """The schema being used for this library's index"""
-        return get_schema(index_schema=True, args=["--schema-version", "v1"])
+        return get_schema(index_schema=True, version="v1")
 
     @cached_property
     def index_from_file(self) -> dict:
         """Fetch the info from the index json as it currently exists"""
         if os.path.exists(self.index_file_path):
             try:
                 with open(self.index_file_path, "r") as f:
```

### Comparing `cbcflow-0.4.4/src/cbcflow/core/metadata.py` & `cbcflow-0.5.0/src/cbcflow/core/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/core/parser.py` & `cbcflow-0.5.0/src/cbcflow/core/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Parsing tools, and tools for generating default data"""
 import argparse
 from typing import Tuple, Union
 import re
+import os
 
 import argcomplete
 
-from .configuration import config_defaults
 from .utils import setup_logger
+from .schema import get_schema
 
 logger = setup_logger()
 
 IGNORE_ARGS = ["info-sname"]
 
 group_shorthands = dict(
     parameter_estimation="parameter_estimation",
@@ -224,33 +225,36 @@
         A parser object, associated with this schema
     dict
         The default data associated with this schema
     """
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     parser.add_argument(
-        "--library", default=config_defaults["library"], help="The library"
+        "--library",
+        default=os.getcwd(),
+        help="The library in which the metadata file in question is stored, defaults to cwd",
+        type=str,
+    )
+    parser.add_argument(
+        "--schema-version",
+        help="The schema version to use, if None (default) the latest version is used",
+        type=str,
+        default=None,
     )
-    parser.add_argument("--schema-version", help="The schema version to use")
     parser.add_argument(
         "--schema-file",
         help="Explicit path to the schema-file. If None (default) the inbuilt schema is used",
-        default=config_defaults["gracedb_service_url"],
+        default=None,
     )
     parser.add_argument(
         "--no-git-library",
         action="store_true",
         help="If true, do not treat the library as a git repo",
     )
     parser.add_argument(
-        "--gracedb-service-url",
-        help="The GraceDb service url",
-        default=config_defaults["gracedb_service_url"],
-    )
-    parser.add_argument(
         "--yes",
         help="Do not ask for confirmation",
         action="store_true",
     )
     parser.add_argument(
         "--branch-name",
         help="The name of the branch to which commits should be written."
```

### Comparing `cbcflow-0.4.4/src/cbcflow/core/process.py` & `cbcflow-0.5.0/src/cbcflow/core/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/core/schema.py` & `cbcflow-0.5.0/src/cbcflow/core/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Methods for fetching schema information"""
 import importlib.resources as importlib_resources
 import json
 import sys
-from typing import Union
+from typing import Union, Optional
 from pathlib import Path
 
-from .configuration import get_cbcflow_config
 from .utils import setup_logger
 
 logger = setup_logger()
 
+CURRENT_CBC_SCHEMA_VERSION = "v3"
+CURRENT_INDEX_SCHEMA_VERSION = "v1"
+
 
 def get_schema_path(version, schema_type_designator="cbc"):
     """Get the path to the schema file
 
     Parameters
     ==========
     version : str
@@ -37,15 +39,54 @@
         return matches[0]
     elif len(matches) == 0:
         raise ValueError(f"No schema file for version {version} found")
     elif len(matches) > 1:
         raise ValueError("Too many matching schema files found")
 
 
-def get_schema(args: Union[list, None] = None, index_schema: bool = False) -> dict:
+def get_schema(
+    schema_path: Optional[str] = None,
+    version: Optional[str] = None,
+    index_schema: bool = False,
+):
+    """Gets the cbc or index schema given a schema path, or a requested version
+
+    Parameters
+    ==========
+    schema_path : Optional[str]
+        If passed, overwrites all defaults to point to given schema file, which will be loaded
+    version : Optional[str]
+        If passed and schema_path is not passed, sets version to read, else up-to-date schema will be used
+    index_schema : bool
+        If set true, loads the index schema, else loads CBC metadata schema by default
+
+    Returns
+    =======
+    dict
+        The json form of the schema
+    """
+    schema_type_designator = "index" if index_schema else "cbc"
+    if version is not None:
+        schema_version = version
+    elif index_schema:
+        schema_version = CURRENT_INDEX_SCHEMA_VERSION
+    else:
+        schema_version = CURRENT_CBC_SCHEMA_VERSION
+    if schema_path is None:
+        schema_path = get_schema_path(
+            version=schema_version, schema_type_designator=schema_type_designator
+        )
+    with Path(schema_path).open("r") as file:
+        schema = json.load(file)
+    return schema
+
+
+def get_schema_from_args(
+    args: Union[list, None] = None, index_schema: bool = False
+) -> dict:
     """Get the schema json
 
     Parameters
     ==========
     args : Union[list, None], optional
         The arguments to use in grabbing the schema. If none are passed defaults to sys.argv
     index_schema : bool, optional
@@ -54,39 +95,26 @@
     Returns
     =======
     dict
         The schema dict loaded from the appropriate file.
     """
     if args is None:
         args = sys.argv
-    VERSION = "v3"
 
     # Set up bootstrap variables
     fileflag = "--schema-file"
     versionflag = "--schema-version"
-    configuration = get_cbcflow_config()
-    if index_schema:
-        config_schema = configuration["index_schema"]
-        schema_type_designator = "index"
-    else:
-        config_schema = configuration["schema"]
-        schema_type_designator = "cbc"
 
-    if config_schema is not None:
-        schema_file = config_schema
-    elif fileflag in args:
+    if fileflag in args:
         schema_file = args[args.index(fileflag) + 1]
+        version = None
     elif versionflag in args:
+        schema_file = None
         version = args[args.index(versionflag) + 1]
-        schema_file = get_schema_path(
-            version, schema_type_designator=schema_type_designator
-        )
     else:
-        schema_file = get_schema_path(
-            VERSION, schema_type_designator=schema_type_designator
-        )
-
-    logger.info(f"Using {schema_type_designator} schema file {schema_file}")
-    with Path(schema_file).open("r") as file:
-        schema = json.load(file)
+        schema_file = None
+        version = None
+    schema = get_schema(
+        schema_path=schema_file, version=version, index_schema=index_schema
+    )
 
     return schema
```

### Comparing `cbcflow-0.4.4/src/cbcflow/core/utils.py` & `cbcflow-0.5.0/src/cbcflow/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,7 +272,25 @@
             raise KeyError(
                 (
                     f"Failed with key error {e}\n"
                     f"Why is there an object without {refId} in this key-tracked array?"
                 )
             )
     return list_of_uids
+
+
+def get_uid_index_for_object_array(
+    uid: str, array: List[Dict], refId: str = "UID"
+) -> int:
+    """Get the index where the object with this uid can be found
+
+    Parameters
+    ==========
+    uid : str
+        The UID corresponding to the object you want to find
+    array : List[Dict]
+        A list of objects each with a unique ID (the refId)
+    refId : str
+        The reference ID which uniquely identifies objects, in normal operation UID
+    """
+    list_of_uids = get_uids_from_object_array(array=array, refId=refId)
+    return list_of_uids.index(uid)
```

### Comparing `cbcflow-0.4.4/src/cbcflow/core/wrapped.py` & `cbcflow-0.5.0/src/cbcflow/core/wrapped.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Convenience wrappers for other lower level functions"""
 from typing import Union
 
 from .schema import get_schema
 from .parser import get_parser_and_default_data
-from .configuration import get_cbcflow_config
 from .metadata import MetaData
 from .database import LocalLibraryDatabase
+import os
 
 
 def get_superevent(
     sname: str,
     library: Union[str, "LocalLibraryDatabase", None] = None,
     no_git_library: bool = False,
 ):
@@ -17,30 +17,29 @@
     A helper method to easily fetch information on a given superevent.
 
     Parameters
     ==========
     sname : str
         The sname of the superevent in question, according to GraceDB
     library : str | `cbcflow.database.LocalLibraryDatabase` | None
-        The library from which to fetch information
+        The library from which to fetch information, defaults to cwd
     no_git_library : bool
         If true, don't attempt to treat this library as a git repository
 
     Returns
     =======
     cbcflow.metadata.MetaData
         The metadata object associated with the superevent in question
     """
 
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
 
     if library is None:
-        config_defaults = get_cbcflow_config()
-        library = config_defaults["library"]
+        library = os.getcwd()
 
     if isinstance(library, LocalLibraryDatabase):
         metadata = MetaData(
             sname,
             local_library=library,
             default_data=default_data,
             schema=schema,
```

### Comparing `cbcflow-0.4.4/src/cbcflow/inputs/asimov.py` & `cbcflow-0.5.0/src/cbcflow/inputs/asimov.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/inputs/pe_scraper.py` & `cbcflow-0.5.0/src/cbcflow/inputs/pe_scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import copy
 from typing import Union, Tuple, Dict
 
 from ..core.utils import (
     setup_logger,
     get_cluster,
     get_url_from_public_html_dir,
+    get_uids_from_object_array,
 )
 from ..core.metadata import MetaData
 
 logger = setup_logger()
 
 
 def scrape_bayeswave_result(path: str):
@@ -265,22 +266,40 @@
 
     # Get existing results, analysts list, reviewers list
     existing_results_dict = {
         res["UID"]: res for res in metadata["ParameterEstimation"]["Results"]
     }
     existing_analysts = metadata["ParameterEstimation"]["Analysts"]
     existing_reviewers = metadata["ParameterEstimation"]["Reviewers"]
+    existing_notes = metadata["ParameterEstimation"]["Notes"]
+    current_status = metadata["ParameterEstimation"]["Status"]
 
     all_analysts = copy.copy(existing_analysts)
     all_reviewers = copy.copy(existing_reviewers)
+    all_notes = copy.copy(existing_notes)
 
     update_dictionary = {"ParameterEstimation": {"Results": []}}
 
+    if current_status == "unstarted" and existing_results_dict != {}:
+        update_dictionary["ParameterEstimation"]["Status"] = "ongoing"
+
     directories = sorted(glob(f"{base_directory}/{sname}/*"))
-    for directory in directories:
+    if "EventInfo.yml" in [x.split("/")[-1] for x in directories]:
+        event_info_yml = os.path.join(base_directory, sname, "EventInfo.yml")
+        event_info = process_event_info_yml(event_info_yml)
+        if "Notes" in event_info:
+            all_notes += event_info["Notes"]
+        if "Status" in event_info:
+            update_dictionary["ParameterEstimation"]["Status"] = event_info["Status"]
+    else:
+        event_info = dict()
+
+    for directory in [
+        directory for directory in directories if os.path.isdir(directory)
+    ]:
         # For each directory under this superevents heading...
         uid = directory.split("/")[-1]
         existing_result = existing_results_dict.get(uid, dict(UID=uid))
 
         # ... generate the update dictionary for the PEResult
         result_update, result_analysts, result_reviewers = generate_result_update(
             directory, existing_result, uid
@@ -293,19 +312,37 @@
         # Add this result update to the full update dictionary
         if len(list(result_update.keys())) > 0:
             update_dictionary["ParameterEstimation"]["Results"].append(result_update)
 
     # Add only reviewers and analysts not yet
     new_analysts = list(set(all_analysts) - set(existing_analysts))
     new_reviewers = list(set(all_reviewers) - set(existing_reviewers))
+    new_notes = list(set(all_notes) - set(existing_notes))
 
+    if "IllustrativeResult" in event_info:
+        update_dictionary["ParameterEstimation"]["IllustrativeResult"] = event_info[
+            "IllustrativeResult"
+        ]
+    if "SkymapReleaseResult" in event_info:
+        update_dictionary["ParameterEstimation"]["SkymapReleaseResult"] = event_info[
+            "SkymapReleaseResult"
+        ]
     update_dictionary["ParameterEstimation"]["Analysts"] = new_analysts
     update_dictionary["ParameterEstimation"]["Reviewers"] = new_reviewers
+    update_dictionary["ParameterEstimation"]["Notes"] = new_notes
 
     metadata.update(update_dict=update_dictionary)
+
+    for pointer_name in ["IllustrativeResult", "SkymapReleaseResult"]:
+        if pointer_name in metadata["ParameterEstimation"]:
+            result_update = regularize_result_pointer_case(
+                metadata, pointer_name=pointer_name
+            )
+            metadata.update(result_update)
+
     return metadata
 
 
 def generate_result_update(
     directory: str, existing_result: dict, uid: str
 ) -> Tuple[dict, list, list]:
     """Process a directory for updates to the corresponding PEResult
@@ -402,35 +439,101 @@
                 run_info_data = yaml.safe_load(file)
             except Exception:
                 logger.warning(f"Yaml file {path_to_run_info} corrupted")
                 return dict()
     else:
         return dict()
 
+    for key in ["Analyst", "Reviewer", "Note"]:
+        # correct when people don't put plurals correctly
+        if key in run_info_data:
+            run_info_data[key + "s"] = run_info_data.pop(key)
+
     # Process information for Analysts, Reviewers, and Notes
     # Each of these may be screwed up in some way by the writer of the RunInfo
     for key in ["Analysts", "Reviewers", "Notes"]:
         if key in run_info_data:
             yaml_content = run_info_data.pop(key)
             yaml_elements = process_ambiguous_yaml_list(yaml_content=yaml_content)
             run_info_data[key] = yaml_elements
 
-    for key in ["ReviewStatus"]:
         # ReviewStatus is an enum, and hence expects specific values, which the PE expert may mess up
         # This drops everything to lowercase, to fix one such failure mode
-        if key in run_info_data:
-            run_info_data[key] = run_info_data[key].lower()
-            if run_info_data[key] in ["passed"]:
-                # Catch a specific case which has gone wrong in the past
-                # We'll add more to this list if people invent new ways to get things wrong
-                run_info_data[key] = "pass"
+    if "ReviewStatus" in run_info_data:
+        if isinstance("ReviewStatus", bool):
+            # If a reviewer says the ReviewStatus is "False" they presumably mean it failed
+            # And if they say it's true they presumably mean it passed
+            # While this is not guaranteed, it's preferable to failing entirely, or softly ignoring it
+            run_info_data["ReviewStatus"] = (
+                "pass" if run_info_data["ReviewStatus"] else "fail"
+            )
+
+        run_info_data["ReviewStatus"] = run_info_data["ReviewStatus"].lower()
+        if run_info_data["ReviewStatus"] in ["passed"]:
+            # Catch a specific case which has gone wrong in the past
+            # We'll add more to this list if people invent new ways to get things wrong
+            run_info_data["ReviewStatus"] = "pass"
+        if run_info_data["ReviewStatus"] in ["not reviewed"]:
+            run_info_data["ReviewStatus"] = "unstarted"
 
     return run_info_data
 
 
+def process_event_info_yml(
+    path_to_event_info_yml: str,
+) -> Dict[str, Union[list, str, bool]]:
+    """Extracts information from an EventInfo.yml file"""
+    if os.path.exists(path_to_event_info_yml):
+        with open(path_to_event_info_yml, "r") as file:
+            try:
+                event_info_data = yaml.safe_load(file)
+            except Exception:
+                logger.warning(f"Yaml file {path_to_event_info_yml} corrupted")
+                return dict()
+    else:
+        return dict()
+
+    for key in ["IllustrativeResult", "Status", "SkymapReleaseResult"]:
+        info_update = event_info_data.get(key, 0)
+        if info_update is None:
+            # The case where the key is present but has no contents
+            event_info_data.pop(key)
+        elif info_update == 0:
+            # The case where the key isn't even present, so nothing to worry about
+            pass
+
+    if "Notes" in event_info_data:
+        yaml_content = event_info_data.pop("Notes")
+        yaml_elements = process_ambiguous_yaml_list(yaml_content=yaml_content)
+        event_info_data["Notes"] = yaml_elements
+
+    return event_info_data
+
+
+def regularize_result_pointer_case(
+    metadata: MetaData, pointer_name="IllustrativeResult"
+) -> dict:
+    illustrative_result = metadata["ParameterEstimation"][pointer_name]
+    pe_result_uids = get_uids_from_object_array(
+        metadata["ParameterEstimation"]["Results"]
+    )
+    if illustrative_result in pe_result_uids:
+        return dict()
+    elif illustrative_result.lower() in [x.lower() for x in pe_result_uids]:
+        correct_uid = pe_result_uids[
+            [x.lower() for x in pe_result_uids].index(illustrative_result.lower())
+        ]
+        return {"ParameterEstimation": {pointer_name: correct_uid}}
+    else:
+        logger.warning(
+            f"{pointer_name} key {illustrative_result} is not in list of UIDs {pe_result_uids}"
+        )
+        return dict()
+
+
 def process_ambiguous_yaml_list(yaml_content: Union[str, list]) -> list:
     """Process heterogeneous yaml contents smoothly
 
     Parameters
     ==========
     yaml_content : Union[str, list]
         The content of the yaml, which should be either a string or a list
```

### Comparing `cbcflow-0.4.4/src/cbcflow/outputs/asimov.py` & `cbcflow-0.5.0/src/cbcflow/outputs/asimov.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.5.0/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.5.0/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/schema/cbc-meta-data-v3.schema` & `cbcflow-0.5.0/src/cbcflow/schema/cbc-meta-data-v3.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.5.0/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.5.0/src/cbcflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.4.4
+Version: 0.5.0
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.4.4/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.5.0/src/cbcflow.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 schema/cbc-meta-data-v2.schema
 schema/cbc-meta-data-v3.schema
 schema/index-v1.schema
 src/cbcflow/__init__.py
 src/cbcflow/_version.py
 src/cbcflow/asimov.py
 src/cbcflow/cbcflow.py
-src/cbcflow/configuration.py
 src/cbcflow/database.py
 src/cbcflow/gracedb.py
 src/cbcflow/metadata.py
 src/cbcflow/monitor.py
 src/cbcflow/parser.py
 src/cbcflow/pe_scraper.py
 src/cbcflow/process.py
@@ -72,15 +71,14 @@
 src/cbcflow.egg-info/requires.txt
 src/cbcflow.egg-info/top_level.txt
 src/cbcflow/client/__init__.py
 src/cbcflow/client/cbcflow.py
 src/cbcflow/client/migrate_v2_to_v3.py
 src/cbcflow/client/monitor.py
 src/cbcflow/core/__init__.py
-src/cbcflow/core/configuration.py
 src/cbcflow/core/database.py
 src/cbcflow/core/metadata.py
 src/cbcflow/core/parser.py
 src/cbcflow/core/process.py
 src/cbcflow/core/schema.py
 src/cbcflow/core/utils.py
 src/cbcflow/core/wrapped.py
@@ -91,14 +89,15 @@
 src/cbcflow/outputs/__init__.py
 src/cbcflow/outputs/asimov.py
 src/cbcflow/schema/cbc-meta-data-v1.schema
 src/cbcflow/schema/cbc-meta-data-v2.schema
 src/cbcflow/schema/cbc-meta-data-v3.schema
 src/cbcflow/schema/index-v1.schema
 tests/test_database.py
+tests/test_gracedb.py
 tests/test_merging.py
 tests/test_metadata.py
 tests/test_schema.py
 tests/files_for_testing/cbc-meta-data-example.json
 tests/files_for_testing/merge_test.json
 tests/files_for_testing/test-file-for-linking-1.txt
 tests/files_for_testing/test-file-for-linking-2.txt
```

### Comparing `cbcflow-0.4.4/src/cbcflow.egg-info/entry_points.txt` & `cbcflow-0.5.0/src/cbcflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.5.0/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/files_for_testing/merge_test.json` & `cbcflow-0.5.0/tests/files_for_testing/merge_test.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/files_for_testing/update_json_1.json` & `cbcflow-0.5.0/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/files_for_testing/update_json_2.json` & `cbcflow-0.5.0/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.5.0/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.5.0/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.5.0/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/test_database.py` & `cbcflow-0.5.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/test_merging.py` & `cbcflow-0.5.0/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.4.4/tests/test_metadata.py` & `cbcflow-0.5.0/tests/test_metadata.py`

 * *Files identical despite different names*

