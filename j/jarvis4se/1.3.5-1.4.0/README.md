# Comparing `tmp/jarvis4se-1.3.5.tar.gz` & `tmp/jarvis4se-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis4se-1.3.5.tar", last modified: Sun May 21 16:51:56 2023, max compression
+gzip compressed data, was "jarvis4se-1.4.0.tar", last modified: Wed May  1 11:47:45 2024, max compression
```

## Comparing `jarvis4se-1.3.5.tar` & `jarvis4se-1.4.0.tar`

### file list

```diff
@@ -1,60 +1,78 @@
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1105 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/LICENSE
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2497 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/PKG-INFO
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1783 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/README.md
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      188 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/pyproject.toml
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      793 2023-05-21 16:51:56.878998 jarvis4se-1.3.5/setup.cfg
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1100 2023-05-21 16:49:17.000000 jarvis4se-1.3.5/setup.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.865665 jarvis4se-1.3.5/src/
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.868998 jarvis4se-1.3.5/src/datamodel/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      900 2023-02-21 11:54:41.000000 jarvis4se-1.3.5/src/datamodel/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    30237 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/datamodel/datamodel.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      235 2023-02-21 11:54:41.000000 jarvis4se-1.3.5/src/datamodel/setup.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1494 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/datamodel/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.868998 jarvis4se-1.3.5/src/jarvis/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      684 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12938 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/command_parser.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.868998 jarvis4se-1.3.5/src/jarvis/diagram/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      229 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    38387 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     4862 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_chain.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     5869 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_fana.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    10784 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_farch.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    19998 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/util.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     4433 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/jarvis.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.872332 jarvis4se-1.3.5/src/jarvis/orchestrator/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      109 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    33057 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/functional_orchestrator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    60025 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/shared_orchestrator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12291 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/viewpoint_orchestrator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    34208 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/jarvis/question_answer.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1721 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.872332 jarvis4se-1.3.5/src/jarvis4se.egg-info/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2497 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/PKG-INFO
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1368 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/SOURCES.txt
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)        1 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/dependency_links.txt
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)       74 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/requires.txt
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)       52 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/top_level.txt
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.872332 jarvis4se-1.3.5/src/plantuml_adapter/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1433 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/plantuml_adapter/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    47455 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/plantuml_adapter/plantuml_adapter.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      206 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/src/plantuml_adapter/setup.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    20036 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/plantuml_adapter/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/src/tools/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      551 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/tools/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     3071 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/config.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2708 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/console.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     3014 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/logger.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1575 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/magic_tools.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      362 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/src/xml_adapter/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      142 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/xml_adapter/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      191 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/src/xml_adapter/setup.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    25934 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/xml_adapter/xml_parser.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    32240 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/xml_adapter/xml_writer.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/tests/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     9338 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_input_cell.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      911 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_lib.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2669 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_magic_tools.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      227 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_question_answer.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12564 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_xml_file.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.237947 jarvis4se-1.4.0/
+-rw-rw-rw-   0        0        0     1127 2022-04-09 16:21:43.000000 jarvis4se-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2768 2024-05-01 11:47:45.236948 jarvis4se-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1814 2022-06-06 16:16:21.000000 jarvis4se-1.4.0/README.md
+-rw-rw-rw-   0        0        0      198 2022-04-09 16:21:43.000000 jarvis4se-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      831 2024-05-01 11:47:45.238934 jarvis4se-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2024-05-01 11:46:38.000000 jarvis4se-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.095123 jarvis4se-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.110132 jarvis4se-1.4.0/src/csv_adapter/
+-rw-rw-rw-   0        0        0      147 2024-03-17 20:34:42.000000 jarvis4se-1.4.0/src/csv_adapter/__init__.py
+-rw-rw-rw-   0        0        0    40928 2024-05-01 11:37:59.000000 jarvis4se-1.4.0/src/csv_adapter/csv_parser.py
+-rw-rw-rw-   0        0        0    30797 2024-04-14 20:29:42.000000 jarvis4se-1.4.0/src/csv_adapter/csv_writer.py
+-rw-rw-rw-   0        0        0      259 2024-03-17 16:24:30.000000 jarvis4se-1.4.0/src/csv_adapter/setup.py
+-rw-rw-rw-   0        0        0     3741 2024-05-01 11:37:59.000000 jarvis4se-1.4.0/src/csv_adapter/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.118126 jarvis4se-1.4.0/src/datamodel/
+-rw-rw-rw-   0        0        0     1372 2024-02-12 18:53:23.000000 jarvis4se-1.4.0/src/datamodel/__init__.py
+-rw-rw-rw-   0        0        0    48062 2024-04-14 20:11:42.000000 jarvis4se-1.4.0/src/datamodel/datamodel.py
+-rw-rw-rw-   0        0        0      248 2024-03-17 16:24:30.000000 jarvis4se-1.4.0/src/datamodel/setup.py
+-rw-rw-rw-   0        0        0     3808 2024-04-14 18:02:21.000000 jarvis4se-1.4.0/src/datamodel/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.146513 jarvis4se-1.4.0/src/jarvis/
+-rw-rw-rw-   0        0        0      706 2023-05-04 13:55:14.000000 jarvis4se-1.4.0/src/jarvis/__init__.py
+-rw-rw-rw-   0        0        0    12034 2024-05-01 11:37:59.000000 jarvis4se-1.4.0/src/jarvis/command_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.165274 jarvis4se-1.4.0/src/jarvis/diagram/
+-rw-rw-rw-   0        0        0      236 2023-05-08 19:29:58.000000 jarvis4se-1.4.0/src/jarvis/diagram/__init__.py
+-rw-rw-rw-   0        0        0    40767 2024-03-02 18:12:03.000000 jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator.py
+-rw-rw-rw-   0        0        0     5133 2024-01-28 21:48:19.000000 jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator_chain.py
+-rw-rw-rw-   0        0        0     5979 2024-01-27 19:35:06.000000 jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator_fana.py
+-rw-rw-rw-   0        0        0    11266 2024-04-14 18:04:03.000000 jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator_farch.py
+-rw-rw-rw-   0        0        0    20696 2024-01-28 21:50:59.000000 jarvis4se-1.4.0/src/jarvis/diagram/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.168273 jarvis4se-1.4.0/src/jarvis/handler/
+-rw-rw-rw-   0        0        0       30 2023-09-05 21:20:18.000000 jarvis4se-1.4.0/src/jarvis/handler/__init__.py
+-rw-rw-rw-   0        0        0     6794 2023-09-26 20:53:28.000000 jarvis4se-1.4.0/src/jarvis/handler/handler_question.py
+-rw-rw-rw-   0        0        0     4550 2023-09-05 21:35:27.000000 jarvis4se-1.4.0/src/jarvis/jarvis.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.190778 jarvis4se-1.4.0/src/jarvis/orchestrator/
+-rw-rw-rw-   0        0        0      327 2024-03-17 21:47:07.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/__init__.py
+-rw-rw-rw-   0        0        0     3816 2024-04-15 18:39:41.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_dictionary.py
+-rw-rw-rw-   0        0        0    36055 2024-02-13 10:41:58.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_functional.py
+-rw-rw-rw-   0        0        0    16103 2024-03-11 21:38:44.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_object.py
+-rw-rw-rw-   0        0        0    64265 2024-03-02 18:37:00.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_shared.py
+-rw-rw-rw-   0        0        0     4994 2024-03-17 21:41:43.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_viewpoint.py
+-rw-rw-rw-   0        0        0     7035 2024-03-17 21:30:21.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_viewpoint_attribute.py
+-rw-rw-rw-   0        0        0    21535 2024-03-11 21:04:21.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_viewpoint_requirement.py
+-rw-rw-rw-   0        0        0     2657 2024-03-17 21:43:33.000000 jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_viewpoint_type.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.195760 jarvis4se-1.4.0/src/jarvis/query/
+-rw-rw-rw-   0        0        0       64 2023-09-05 17:01:24.000000 jarvis4se-1.4.0/src/jarvis/query/__init__.py
+-rw-rw-rw-   0        0        0    13784 2024-03-02 18:45:45.000000 jarvis4se-1.4.0/src/jarvis/query/query_object_list.py
+-rw-rw-rw-   0        0        0    18971 2024-05-01 11:30:44.000000 jarvis4se-1.4.0/src/jarvis/query/question_answer.py
+-rw-rw-rw-   0        0        0     3147 2023-08-09 20:49:48.000000 jarvis4se-1.4.0/src/jarvis/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.235964 jarvis4se-1.4.0/src/jarvis4se.egg-info/
+-rw-rw-rw-   0        0        0     2768 2024-05-01 11:47:45.000000 jarvis4se-1.4.0/src/jarvis4se.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2024-05-01 11:47:45.000000 jarvis4se-1.4.0/src/jarvis4se.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:47:45.000000 jarvis4se-1.4.0/src/jarvis4se.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:47:45.000000 jarvis4se-1.4.0/src/jarvis4se.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       64 2024-05-01 11:47:45.000000 jarvis4se-1.4.0/src/jarvis4se.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.205593 jarvis4se-1.4.0/src/plantuml_adapter/
+-rw-rw-rw-   0        0        0     1459 2023-03-04 16:52:21.000000 jarvis4se-1.4.0/src/plantuml_adapter/__init__.py
+-rw-rw-rw-   0        0        0    49747 2024-01-28 22:52:03.000000 jarvis4se-1.4.0/src/plantuml_adapter/plantuml_adapter.py
+-rw-rw-rw-   0        0        0      269 2024-03-17 16:24:30.000000 jarvis4se-1.4.0/src/plantuml_adapter/setup.py
+-rw-rw-rw-   0        0        0    21801 2024-02-12 13:52:05.000000 jarvis4se-1.4.0/src/plantuml_adapter/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.215747 jarvis4se-1.4.0/src/tools/
+-rw-rw-rw-   0        0        0      569 2023-03-05 16:49:04.000000 jarvis4se-1.4.0/src/tools/__init__.py
+-rw-rw-rw-   0        0        0     3143 2023-05-04 14:43:11.000000 jarvis4se-1.4.0/src/tools/config.py
+-rw-rw-rw-   0        0        0     2847 2023-09-05 21:39:04.000000 jarvis4se-1.4.0/src/tools/console.py
+-rw-rw-rw-   0        0        0     3111 2023-05-04 14:43:11.000000 jarvis4se-1.4.0/src/tools/logger.py
+-rw-rw-rw-   0        0        0     1630 2023-05-04 14:43:11.000000 jarvis4se-1.4.0/src/tools/magic_tools.py
+-rw-rw-rw-   0        0        0      381 2023-05-04 14:43:11.000000 jarvis4se-1.4.0/src/tools/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.223759 jarvis4se-1.4.0/src/xml_adapter/
+-rw-rw-rw-   0        0        0      147 2023-04-21 10:34:50.000000 jarvis4se-1.4.0/src/xml_adapter/__init__.py
+-rw-rw-rw-   0        0        0      254 2024-03-17 16:24:30.000000 jarvis4se-1.4.0/src/xml_adapter/setup.py
+-rw-rw-rw-   0        0        0    35717 2024-04-14 20:24:58.000000 jarvis4se-1.4.0/src/xml_adapter/xml_parser.py
+-rw-rw-rw-   0        0        0    45860 2024-04-15 17:51:45.000000 jarvis4se-1.4.0/src/xml_adapter/xml_writer.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:47:45.234947 jarvis4se-1.4.0/tests/
+-rw-rw-rw-   0        0        0    12575 2024-04-14 18:32:00.000000 jarvis4se-1.4.0/tests/test_csv_file.py
+-rw-rw-rw-   0        0        0     2665 2023-09-27 18:00:45.000000 jarvis4se-1.4.0/tests/test_handler_question.py
+-rw-rw-rw-   0        0        0     9591 2023-05-16 15:57:12.000000 jarvis4se-1.4.0/tests/test_input_cell.py
+-rw-rw-rw-   0        0        0     1214 2024-04-14 16:13:29.000000 jarvis4se-1.4.0/tests/test_lib.py
+-rw-rw-rw-   0        0        0     2735 2023-04-19 10:49:08.000000 jarvis4se-1.4.0/tests/test_magic_tools.py
+-rw-rw-rw-   0        0        0    12952 2023-09-27 19:15:44.000000 jarvis4se-1.4.0/tests/test_xml_file.py
```

### Comparing `jarvis4se-1.3.5/LICENSE` & `jarvis4se-1.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2022 Regis Casteran
-Copyright (c) 2022 Justin Ancelot
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Regis Casteran
+Copyright (c) 2022 Justin Ancelot
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `jarvis4se-1.3.5/PKG-INFO` & `jarvis4se-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,57 @@
-Metadata-Version: 2.1
-Name: jarvis4se
-Version: 1.3.5
-Summary: Jarvis 4 Systems Engineers
-Home-page: https://github.com/rcasteran/jarvis4se
-Author: Justin ANCELOT
-Author-email: not2behere@gmx.fr
-License: MIT
-Project-URL: Bug Tracker, https://github.com/rcasteran/jarvis4se/issues
-Project-URL: Gitbook, https://regis-casteran.gitbook.io/jarvis4se/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Just Another Rather Very Intelligent System (JARVIS) for Systems Engineers (SE)
-
-Latest stable release: ![GitHub release (latest by date)](https://img.shields.io/github/v/release/rcasteran/jarvis4se)
-
-Current CI status: [![CircleCI](https://circleci.com/gh/rcasteran/jarvis4se/tree/main.svg?style=svg)](https://circleci.com/gh/rcasteran/jarvis4se/tree/main)
-
-Playground (with latest stable release) : [![Binder](https://mybinder.org/badge\_logo.svg)](https://mybinder.org/v2/gh/Not2behere/PlayJarvis4se/HEAD)
-
-## Introduction
-
-JARVIS4SE allows systems engineers to build the single source of truth of the knowledge they develop about the system of interest they want to master, preventing this knowledge from being:
-
-* Distorted by any graphical representation considerations
-* Splitted accross different domain languages
-* Expressed only in a machine readable medium
-
-### Free from graphical representation considerations
-
-The core of JARVIS4SE is independent from any graphical representation considerations: it is based on a set of basic [engineering concepts](docs/engineering-concepts/definitions.md) adapted from different domain languages, without taking into account concepts like coordinates, rendering...
-
-To be able to visualize the knowledge of the system of interest with diagrams, the core of JARVIS4SE can be interfaced with the API of any modeling tool through a dedicated adapter.
-
-Today the following adapters are available:
-
-* [PlantUML](https://plantuml.com/en/)
-
-### Based on natural language
-
-The core of JARVIS4SE is based on a subset of the english language that has been mapped to the set of basic [engineering concepts](docs/engineering-concepts/definitions.md).
-
-This allows systems engineers to interact with JARVIS4SE via voice or a textual interface.
+Metadata-Version: 2.1
+Name: jarvis4se
+Version: 1.4.0
+Summary: Jarvis 4 Systems Engineers
+Home-page: https://github.com/rcasteran/jarvis4se
+Author: Regis CASTERAN
+Author-email: casteranregis@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/rcasteran/jarvis4se/issues
+Project-URL: Gitbook, https://regis-casteran.gitbook.io/jarvis4se/
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython>=7.27.0
+Requires-Dist: lxml>=4.6.3
+Requires-Dist: notebook>=6.4.3
+Requires-Dist: plantuml==0.3.0
+Requires-Dist: pandas~=1.4.1
+Requires-Dist: requests>=2.31.0
+Requires-Dist: nltk~=3.8.1
+
+# Just Another Rather Very Intelligent System (JARVIS) for Systems Engineers (SE)
+
+Latest stable release: ![GitHub release (latest by date)](https://img.shields.io/github/v/release/rcasteran/jarvis4se)
+
+Current CI status: [![CircleCI](https://circleci.com/gh/rcasteran/jarvis4se/tree/main.svg?style=svg)](https://circleci.com/gh/rcasteran/jarvis4se/tree/main)
+
+Playground (with latest stable release) : [![Binder](https://mybinder.org/badge\_logo.svg)](https://mybinder.org/v2/gh/Not2behere/PlayJarvis4se/HEAD)
+
+## Introduction
+
+JARVIS4SE allows systems engineers to build the single source of truth of the knowledge they develop about the system of interest they want to master, preventing this knowledge from being:
+
+* Distorted by any graphical representation considerations
+* Splitted accross different domain languages
+* Expressed only in a machine readable medium
+
+### Free from graphical representation considerations
+
+The core of JARVIS4SE is independent from any graphical representation considerations: it is based on a set of basic [engineering concepts](docs/engineering-concepts/definitions.md) adapted from different domain languages, without taking into account concepts like coordinates, rendering...
+
+To be able to visualize the knowledge of the system of interest with diagrams, the core of JARVIS4SE can be interfaced with the API of any modeling tool through a dedicated adapter.
+
+Today the following adapters are available:
+
+* [PlantUML](https://plantuml.com/en/)
+
+### Based on natural language
+
+The core of JARVIS4SE is based on a subset of the english language that has been mapped to the set of basic [engineering concepts](docs/engineering-concepts/definitions.md).
+
+This allows systems engineers to interact with JARVIS4SE via voice or a textual interface.
```

### Comparing `jarvis4se-1.3.5/README.md` & `jarvis4se-1.4.0/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Just Another Rather Very Intelligent System (JARVIS) for Systems Engineers (SE)
-
-Latest stable release: ![GitHub release (latest by date)](https://img.shields.io/github/v/release/rcasteran/jarvis4se)
-
-Current CI status: [![CircleCI](https://circleci.com/gh/rcasteran/jarvis4se/tree/main.svg?style=svg)](https://circleci.com/gh/rcasteran/jarvis4se/tree/main)
-
-Playground (with latest stable release) : [![Binder](https://mybinder.org/badge\_logo.svg)](https://mybinder.org/v2/gh/Not2behere/PlayJarvis4se/HEAD)
-
-## Introduction
-
-JARVIS4SE allows systems engineers to build the single source of truth of the knowledge they develop about the system of interest they want to master, preventing this knowledge from being:
-
-* Distorted by any graphical representation considerations
-* Splitted accross different domain languages
-* Expressed only in a machine readable medium
-
-### Free from graphical representation considerations
-
-The core of JARVIS4SE is independent from any graphical representation considerations: it is based on a set of basic [engineering concepts](docs/engineering-concepts/definitions.md) adapted from different domain languages, without taking into account concepts like coordinates, rendering...
-
-To be able to visualize the knowledge of the system of interest with diagrams, the core of JARVIS4SE can be interfaced with the API of any modeling tool through a dedicated adapter.
-
-Today the following adapters are available:
-
-* [PlantUML](https://plantuml.com/en/)
-
-### Based on natural language
-
-The core of JARVIS4SE is based on a subset of the english language that has been mapped to the set of basic [engineering concepts](docs/engineering-concepts/definitions.md).
-
-This allows systems engineers to interact with JARVIS4SE via voice or a textual interface.
+# Just Another Rather Very Intelligent System (JARVIS) for Systems Engineers (SE)
+
+Latest stable release: ![GitHub release (latest by date)](https://img.shields.io/github/v/release/rcasteran/jarvis4se)
+
+Current CI status: [![CircleCI](https://circleci.com/gh/rcasteran/jarvis4se/tree/main.svg?style=svg)](https://circleci.com/gh/rcasteran/jarvis4se/tree/main)
+
+Playground (with latest stable release) : [![Binder](https://mybinder.org/badge\_logo.svg)](https://mybinder.org/v2/gh/Not2behere/PlayJarvis4se/HEAD)
+
+## Introduction
+
+JARVIS4SE allows systems engineers to build the single source of truth of the knowledge they develop about the system of interest they want to master, preventing this knowledge from being:
+
+* Distorted by any graphical representation considerations
+* Splitted accross different domain languages
+* Expressed only in a machine readable medium
+
+### Free from graphical representation considerations
+
+The core of JARVIS4SE is independent from any graphical representation considerations: it is based on a set of basic [engineering concepts](docs/engineering-concepts/definitions.md) adapted from different domain languages, without taking into account concepts like coordinates, rendering...
+
+To be able to visualize the knowledge of the system of interest with diagrams, the core of JARVIS4SE can be interfaced with the API of any modeling tool through a dedicated adapter.
+
+Today the following adapters are available:
+
+* [PlantUML](https://plantuml.com/en/)
+
+### Based on natural language
+
+The core of JARVIS4SE is based on a subset of the english language that has been mapped to the set of basic [engineering concepts](docs/engineering-concepts/definitions.md).
+
+This allows systems engineers to interact with JARVIS4SE via voice or a textual interface.
```

### Comparing `jarvis4se-1.3.5/setup.cfg` & `jarvis4se-1.4.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6a61 7276 6973 3473 650a 7665 7273  = jarvis4se.vers
-00000020: 696f 6e20 3d20 312e 332e 350a 6175 7468  ion = 1.3.5.auth
-00000030: 6f72 203d 204a 7573 7469 6e20 414e 4345  or = Justin ANCE
-00000040: 4c4f 540a 6175 7468 6f72 5f65 6d61 696c  LOT.author_email
-00000050: 203d 206e 6f74 3262 6568 6572 6540 676d   = not2behere@gm
-00000060: 782e 6672 0a64 6573 6372 6970 7469 6f6e  x.fr.description
-00000070: 203d 204a 6172 7669 7320 3420 5379 7374   = Jarvis 4 Syst
-00000080: 656d 7320 456e 6769 6e65 6572 730a 6c6f  ems Engineers.lo
-00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-000000a0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
-000000b0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000c0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-000000d0: 2074 6578 742f 6d61 726b 646f 776e 0a75   text/markdown.u
-000000e0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-000000f0: 6875 622e 636f 6d2f 7263 6173 7465 7261  hub.com/rcastera
-00000100: 6e2f 6a61 7276 6973 3473 650a 7072 6f6a  n/jarvis4se.proj
-00000110: 6563 745f 7572 6c73 203d 200a 0942 7567  ect_urls = ..Bug
-00000120: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
-00000130: 3a2f 2f67 6974 6875 622e 636f 6d2f 7263  ://github.com/rc
-00000140: 6173 7465 7261 6e2f 6a61 7276 6973 3473  asteran/jarvis4s
-00000150: 652f 6973 7375 6573 0a09 4769 7462 6f6f  e/issues..Gitboo
-00000160: 6b20 3d20 6874 7470 733a 2f2f 7265 6769  k = https://regi
-00000170: 732d 6361 7374 6572 616e 2e67 6974 626f  s-casteran.gitbo
-00000180: 6f6b 2e69 6f2f 6a61 7276 6973 3473 652f  ok.io/jarvis4se/
-00000190: 0a63 6c61 7373 6966 6965 7273 203d 200a  .classifiers = .
-000001a0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001c0: 3a3a 2033 2e38 0a09 4c69 6365 6e73 6520  :: 3.8..License 
-000001d0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001e0: 3a3a 204d 4954 204c 6963 656e 7365 0a09  :: MIT License..
-000001f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000200: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000210: 6e74 0a09 546f 7069 6320 3a3a 2053 6369  nt..Topic :: Sci
-00000220: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-00000230: 696e 6720 3a3a 2056 6973 7561 6c69 7a61  ing :: Visualiza
-00000240: 7469 6f6e 0a09 546f 7069 6320 3a3a 2053  tion..Topic :: S
-00000250: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00000260: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-00000270: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
-00000280: 6573 0a0a 5b6f 7074 696f 6e73 5d0a 7061  es..[options].pa
-00000290: 636b 6167 655f 6469 7220 3d20 0a09 3d20  ckage_dir = ..= 
-000002a0: 7372 630a 7061 636b 6167 6573 203d 2066  src.packages = f
-000002b0: 696e 643a 0a70 7974 686f 6e5f 7265 7175  ind:.python_requ
-000002c0: 6972 6573 203d 203e 3d33 2e38 0a0a 5b6f  ires = >=3.8..[o
-000002d0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000002e0: 6669 6e64 5d0a 7768 6572 6520 3d20 7372  find].where = sr
-000002f0: 630a 0a5b 6567 675f 696e 666f 5d0a 7461  c..[egg_info].ta
-00000300: 675f 6275 696c 6420 3d20 0a74 6167 5f64  g_build = .tag_d
-00000310: 6174 6520 3d20 300a 0a                   ate = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206a 6172 7669 7334 7365 0d0a 7665   = jarvis4se..ve
+00000020: 7273 696f 6e20 3d20 312e 342e 300d 0a61  rsion = 1.4.0..a
+00000030: 7574 686f 7220 3d20 5265 6769 7320 4341  uthor = Regis CA
+00000040: 5354 4552 414e 0d0a 6175 7468 6f72 5f65  STERAN..author_e
+00000050: 6d61 696c 203d 2063 6173 7465 7261 6e72  mail = casteranr
+00000060: 6567 6973 4067 6d61 696c 2e63 6f6d 0d0a  egis@gmail.com..
+00000070: 6465 7363 7269 7074 696f 6e20 3d20 4a61  description = Ja
+00000080: 7276 6973 2034 2053 7973 7465 6d73 2045  rvis 4 Systems E
+00000090: 6e67 696e 6565 7273 0d0a 6c6f 6e67 5f64  ngineers..long_d
+000000a0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000b0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+000000c0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000d0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+000000e0: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
+000000f0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000100: 622e 636f 6d2f 7263 6173 7465 7261 6e2f  b.com/rcasteran/
+00000110: 6a61 7276 6973 3473 650d 0a70 726f 6a65  jarvis4se..proje
+00000120: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
+00000130: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+00000140: 3a2f 2f67 6974 6875 622e 636f 6d2f 7263  ://github.com/rc
+00000150: 6173 7465 7261 6e2f 6a61 7276 6973 3473  asteran/jarvis4s
+00000160: 652f 6973 7375 6573 0d0a 0947 6974 626f  e/issues...Gitbo
+00000170: 6f6b 203d 2068 7474 7073 3a2f 2f72 6567  ok = https://reg
+00000180: 6973 2d63 6173 7465 7261 6e2e 6769 7462  is-casteran.gitb
+00000190: 6f6f 6b2e 696f 2f6a 6172 7669 7334 7365  ook.io/jarvis4se
+000001a0: 2f0d 0a63 6c61 7373 6966 6965 7273 203d  /..classifiers =
+000001b0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+000001c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001d0: 6f6e 203a 3a20 332e 380d 0a09 4c69 6365  on :: 3.8...Lice
+000001e0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001f0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000200: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+00000210: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000220: 7065 6e64 656e 740d 0a09 546f 7069 6320  pendent...Topic 
+00000230: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+00000240: 6769 6e65 6572 696e 6720 3a3a 2056 6973  gineering :: Vis
+00000250: 7561 6c69 7a61 7469 6f6e 0d0a 0954 6f70  ualization...Top
+00000260: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+00000270: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+00000280: 6272 6172 6965 7320 3a3a 2050 7974 686f  braries :: Pytho
+00000290: 6e20 4d6f 6475 6c65 730d 0a0d 0a5b 6f70  n Modules....[op
+000002a0: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
+000002b0: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
+000002c0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+000002d0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+000002e0: 7320 3d20 3e3d 332e 380d 0a0d 0a5b 6f70  s = >=3.8....[op
+000002f0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000300: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000310: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
+00000320: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000330: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator.py` & `jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,723 +1,765 @@
-"""@defgroup diagram
-Jarvis diagram module
-"""
-# Libraries
-import re
-
-# Modules
-import plantuml_adapter
-from datamodel import FunctionalElement
-from jarvis import question_answer
-from jarvis.orchestrator import shared_orchestrator
-from jarvis import util as jarvis_util
-from . import diagram_generator_chain
-from . import diagram_generator_farch
-from . import diagram_generator_fana
-from . import util
-from tools import Logger
-
-
-def filter_show_command(diagram_name_str, **kwargs):
-    """Entry point for all diagrams (i.e. 'show' command) from command_parser.py"""
-    plantuml_string = None
-    wanted_diagram_str = diagram_name_str[0].strip()
-    regex = r"(decomposition|context|chain|sequence|state|function|state sequence)\s(.*)"
-    specific_diagram_str = re.search(regex, wanted_diagram_str, re.MULTILINE)
-    if specific_diagram_str:
-        if 'sequence' not in specific_diagram_str.group(2):
-            diagram_type_str = specific_diagram_str.group(1)
-            diagram_object_str = specific_diagram_str.group(2)
-        else:
-            diagram_type_str = specific_diagram_str.group(1) + ' sequence'
-            diagram_object_str = specific_diagram_str.group(2).replace("sequence ", "")
-
-        plantuml_string = switch_show_filter(diagram_type_str=diagram_type_str,
-                                             diagram_object_str=diagram_object_str,
-                                             **kwargs)
-    else:
-        Logger.set_warning(__name__,
-                           f"Jarvis does not understand the command {wanted_diagram_str}")
-
-    return plantuml_string
-
-
-def switch_show_filter(**kwargs):
-    """Switch case between diagram types"""
-    switch = {
-        "function": case_function_diagram,
-        "context": case_context_diagram,
-        "decomposition": case_decomposition_diagram,
-        "chain": case_chain_diagram,
-        "sequence": case_sequence_diagram,
-        "state": case_state_diagram,
-        "state sequence": case_state_sequence_diagram
-    }
-    get_diagram = switch.get(kwargs['diagram_type_str'], case_no_diagram)
-    return get_diagram(**kwargs)
-
-
-def case_function_diagram(**kwargs):
-    """Case for 'show function <functional_element>'"""
-    plantuml_string = None
-
-    if kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_fun_elem_list']):
-        plantuml_string = diagram_generator_farch.show_fun_elem_function(kwargs['diagram_object_str'],
-                                                                         kwargs['xml_fun_elem_list'],
-                                                                         kwargs['xml_function_list'],
-                                                                         kwargs['xml_consumer_function_list'],
-                                                                         kwargs['xml_producer_function_list'],
-                                                                         kwargs['xml_attribute_list'])
-
-    else:
-        Logger.set_warning(__name__,
-                           f"Jarvis does not know the functional Element {kwargs['diagram_object_str']}")
-
-    return plantuml_string
-
-
-def case_context_diagram(**kwargs):
-    """Case for 'show context <functional_element>/<function>'"""
-    plantuml_string = None
-
-    if kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_function_list']):
-        child_inheritance = shared_orchestrator.childs_inheritance(kwargs['xml_function_list'])
-        attribute_inheritance = shared_orchestrator.attribute_inheritance(kwargs['xml_attribute_list'],
-                                                                          kwargs['xml_function_list'])
-
-        plantuml_string = diagram_generator_fana.show_function_context(kwargs['diagram_object_str'],
-                                                                       kwargs['xml_function_list'],
-                                                                       kwargs['xml_consumer_function_list'],
-                                                                       kwargs['xml_producer_function_list'],
-                                                                       kwargs['xml_data_list'],
-                                                                       kwargs['xml_attribute_list'],
-                                                                       kwargs['xml_type_list'])
-
-        shared_orchestrator.reset_childs_inheritance(kwargs['xml_function_list'], derived_child_id=child_inheritance[2])
-        shared_orchestrator.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
-
-    elif kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_state_list']):
-        plantuml_string = show_states_chain([kwargs['diagram_object_str']],
-                                            kwargs['xml_state_list'],
-                                            kwargs['xml_transition_list'])
-
-    elif kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_fun_elem_list']):
-        child_inheritance = shared_orchestrator.childs_inheritance(kwargs['xml_function_list'],
-                                                                   kwargs['xml_fun_elem_list'],
-                                                                   level=None)
-        attribute_inheritance = shared_orchestrator.attribute_inheritance(kwargs['xml_attribute_list'],
-                                                                          kwargs['xml_function_list'],
-                                                                          kwargs['xml_fun_elem_list'],
-                                                                          kwargs['xml_fun_inter_list'])
-        func_alloc_inheritance = shared_orchestrator.allocation_inheritance(kwargs['xml_fun_elem_list'],
-                                                                            kwargs['xml_function_list'])
-        fun_inter_alloc_inheritance = shared_orchestrator.allocation_inheritance(kwargs['xml_fun_inter_list'],
-                                                                                 kwargs['xml_data_list'])
-
-        plantuml_string = diagram_generator_farch.show_fun_elem_context(kwargs['diagram_object_str'],
-                                                                        kwargs['xml_fun_elem_list'],
-                                                                        kwargs['xml_function_list'],
-                                                                        kwargs['xml_consumer_function_list'],
-                                                                        kwargs['xml_producer_function_list'],
-                                                                        kwargs['xml_attribute_list'],
-                                                                        kwargs['xml_fun_inter_list'],
-                                                                        kwargs['xml_data_list'])
-
-        shared_orchestrator.reset_childs_inheritance(kwargs['xml_function_list'],
-                                                     kwargs['xml_fun_elem_list'],
-                                                     derived_child_id=child_inheritance[2])
-        shared_orchestrator.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
-        shared_orchestrator.reset_alloc_inheritance(func_alloc_inheritance)
-        shared_orchestrator.reset_alloc_inheritance(fun_inter_alloc_inheritance)
-    else:
-        Logger.set_warning(__name__,
-                           f"Jarvis does not know the function {kwargs['diagram_object_str']} or "
-                           f"{kwargs['diagram_object_str']} is not a valid "
-                           f"Function/State/Functional Element name/alias")
-
-    return plantuml_string
-
-
-def case_decomposition_diagram(**kwargs):
-    """Case for 'show decomposition <functional_element>/<function>'"""
-    plantuml_string = None
-
-    if ' at level ' in kwargs['diagram_object_str']:
-        splitted_str = re.split(" at level ", kwargs['diagram_object_str'])
-        diagram_object_str = splitted_str[0]
-        try:
-            diagram_level = int(splitted_str[1])
-            if diagram_level == 0:
-                Logger.set_error(__name__,
-                                 "Invalid level, please choose a valid level >= 1")
-                return plantuml_string
-        except ValueError:
-            Logger.set_error(__name__,
-                             "Invalid level, please choose a valid level >= 1")
-            return plantuml_string
-    else:
-        diagram_object_str = kwargs['diagram_object_str']
-        diagram_level = None
-
-    v_inheritance = shared_orchestrator.view_inheritance(kwargs['xml_view_list'],
-                                                         kwargs['xml_function_list'],
-                                                         kwargs['xml_fun_elem_list'])
-
-    # Check view if activated and filter allocated item
-    function_list = util.get_object_list_from_view(diagram_object_str,
-                                                   kwargs['xml_function_list'],
-                                                   kwargs['xml_view_list'])
-
-    if len(function_list) > 0:
-        _, consumer_list, producer_list = \
-            util.get_cons_prod_from_view_allocated_data(kwargs['xml_data_list'],
-                                                        kwargs['xml_view_list'],
-                                                        kwargs['xml_consumer_function_list'],
-                                                        kwargs['xml_producer_function_list'],
-                                                        function_list)
-
-        if diagram_object_str in question_answer.get_objects_names(kwargs['xml_function_list']):
-            child_inheritance = shared_orchestrator.childs_inheritance(function_list, level=diagram_level)
-            attribute_inheritance = shared_orchestrator.attribute_inheritance(kwargs['xml_attribute_list'],
-                                                                              function_list)
-
-            plantuml_string = diagram_generator_fana.show_function_decomposition(diagram_object_str,
-                                                                                 function_list,
-                                                                                 consumer_list,
-                                                                                 producer_list,
-                                                                                 kwargs['xml_attribute_list'],
-                                                                                 kwargs['xml_type_list'],
-                                                                                 diagram_level=diagram_level)
-
-            shared_orchestrator.reset_childs_inheritance(function_list, derived_child_id=child_inheritance[2])
-            shared_orchestrator.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
-        elif diagram_object_str in question_answer.get_objects_names(kwargs['xml_fun_elem_list']):
-            fun_elem_list = util.get_object_list_from_view(diagram_object_str,
-                                                           kwargs['xml_fun_elem_list'],
-                                                           kwargs['xml_view_list'])
-
-            if len(fun_elem_list) > 0:
-                child_inheritance = shared_orchestrator.childs_inheritance(function_list, fun_elem_list,
-                                                                           level=diagram_level)
-                attribute_inheritance = shared_orchestrator.attribute_inheritance(kwargs['xml_attribute_list'],
-                                                                                  function_list,
-                                                                                  fun_elem_list,
-                                                                                  kwargs['xml_fun_inter_list'])
-                func_alloc_inheritance = shared_orchestrator.allocation_inheritance(fun_elem_list, function_list)
-                fun_inter_alloc_inheritance = shared_orchestrator.allocation_inheritance(kwargs['xml_fun_inter_list'],
-                                                                                         kwargs['xml_data_list'])
-
-                plantuml_string = diagram_generator_farch.show_fun_elem_decomposition(diagram_object_str,
-                                                                                      function_list,
-                                                                                      consumer_list,
-                                                                                      producer_list,
-                                                                                      fun_elem_list,
-                                                                                      kwargs['xml_attribute_list'],
-                                                                                      kwargs['xml_data_list'],
-                                                                                      kwargs['xml_fun_inter_list'],
-                                                                                      diagram_level)
-
-                shared_orchestrator.reset_childs_inheritance(function_list,
-                                                             fun_elem_list,
-                                                             derived_child_id=child_inheritance[2])
-                shared_orchestrator.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
-                shared_orchestrator.reset_alloc_inheritance(func_alloc_inheritance)
-                shared_orchestrator.reset_alloc_inheritance(fun_inter_alloc_inheritance)
-        else:
-            Logger.set_warning(__name__,
-                               f"Jarvis does not know the object {diagram_object_str}"
-                               f"(i.e. it is not a function, nor a functional element)")
-
-    shared_orchestrator.reset_view_inheritance(kwargs['xml_view_list'], v_inheritance)
-
-    return plantuml_string
-
-
-def case_chain_diagram(**kwargs):
-    """Case for 'show chain <states>/<functions>'"""
-    plantuml_string = None
-
-    object_list_str = jarvis_util.cut_string(kwargs['diagram_object_str'])
-
-    if len(object_list_str) > 0:
-        xml_function_name_list = question_answer.get_objects_names(kwargs['xml_function_list'])
-        result_function = all(t in xml_function_name_list for t in object_list_str)
-
-        xml_state_name_list = question_answer.get_objects_names(kwargs['xml_state_list'])
-        result_state = all(t in xml_state_name_list for t in object_list_str)
-
-        xml_fun_elem_name_list = question_answer.get_objects_names(kwargs['xml_fun_elem_list'])
-        result_fun_elem = all(t in xml_fun_elem_name_list for t in object_list_str)
-
-        if result_function:
-            function_list = util.get_object_list_from_view(object_list_str,
-                                                           kwargs['xml_function_list'],
-                                                           kwargs['xml_view_list'])
-
-            if len(function_list) > 0:
-                _, consumer_list, producer_list = \
-                    util.get_cons_prod_from_view_allocated_data(kwargs['xml_data_list'],
-                                                                kwargs['xml_view_list'],
-                                                                kwargs[
-                                                                    'xml_consumer_function_list'],
-                                                                kwargs[
-                                                                    'xml_producer_function_list'],
-                                                                function_list)
-
-                plantuml_string = diagram_generator_chain.show_function_chain(object_list_str,
-                                                                              function_list,
-                                                                              consumer_list,
-                                                                              producer_list,
-                                                                              kwargs['xml_type_list'],
-                                                                              kwargs['xml_attribute_list'])
-            else:
-                Logger.set_warning(__name__,
-                                   f"Nothing to display for the selected view")
-        elif result_fun_elem:
-            fun_elem_list_from_view = util.get_object_list_from_view(object_list_str,
-                                                                     kwargs['xml_fun_elem_list'],
-                                                                     kwargs['xml_view_list'])
-
-            if len(fun_elem_list_from_view) > 0:
-                fun_elem_list = set()
-                function_list = set()
-
-                function_list_from_view = util.get_object_list_from_view(object_list_str,
-                                                                         kwargs['xml_function_list'],
-                                                                         kwargs['xml_view_list'])
-                for i in object_list_str:
-                    for fun_elem in fun_elem_list_from_view:
-                        if i == fun_elem.name or i == fun_elem.alias:
-                            fun_elem_list.add(fun_elem)
-
-                            if len(fun_elem.allocated_function_list) > 0:
-                                for allocated_function_id in fun_elem.allocated_function_list:
-                                    for function in kwargs['xml_function_list']:
-                                        if function.id == allocated_function_id and function in function_list_from_view:
-                                            util.get_fun_elem_function_list(function, function_list, fun_elem)
-                            else:
-                                Logger.set_info(__name__,
-                                                f"No function allocated to {fun_elem.name} (no display)")
-
-                new_function_list, consumer_list, producer_list = \
-                    util.get_cons_prod_from_view_allocated_data(kwargs['xml_data_list'],
-                                                                kwargs['xml_view_list'],
-                                                                kwargs[
-                                                                    'xml_consumer_function_list'],
-                                                                kwargs[
-                                                                    'xml_producer_function_list'],
-                                                                function_list)
-
-                plantuml_string = diagram_generator_chain.show_fun_elem_chain(object_list_str,
-                                                                              new_function_list,
-                                                                              consumer_list,
-                                                                              producer_list,
-                                                                              fun_elem_list,
-                                                                              kwargs['xml_type_list'],
-                                                                              kwargs['xml_attribute_list'])
-            else:
-                Logger.set_warning(__name__,
-                                   f"Nothing to display for the selected view")
-        elif result_state:
-            state_list = util.get_object_list_from_view(object_list_str,
-                                                        kwargs['xml_state_list'],
-                                                        kwargs['xml_view_list'])
-
-            if len(state_list) > 0:
-                transition_list = util.filter_allocated_item_from_view(kwargs['xml_transition_list'],
-                                                                       kwargs['xml_view_list'])
-
-                plantuml_string = show_states_chain(object_list_str, state_list, transition_list)
-            else:
-                Logger.set_warning(__name__,
-                                   f"Nothing to display for the selected view")
-        else:
-            Logger.set_warning(__name__,
-                               f"Jarvis does not know the object(s): {kwargs['diagram_object_str']}"
-                               f"(i.e. it is not a function, nor a functional element, nor a state)")
-    else:
-        Logger.set_error(__name__,
-                         f"{kwargs['diagram_object_str']} is not a valid chain")
-
-    return plantuml_string
-
-
-def case_sequence_diagram(**kwargs):
-    """Case for 'show sequence <functional_elements>/<functions>/<functional_interface>'"""
-    plantuml_string = None
-    object_list_str = re.split(r',(?![^[]*\])', kwargs['diagram_object_str'].replace(", ", ","))
-    object_list_str = [s.rstrip() for s in object_list_str]
-    if object_list_str:
-        if len(object_list_str) == 1 and \
-                any(s == object_list_str[0] for s in question_answer.get_objects_names(kwargs['xml_fun_inter_list'])):
-            plantuml_string = get_fun_inter_sequence_diagram(object_list_str.pop(), **kwargs)
-        elif len(object_list_str) >= 1:
-            # Check view if activated and filter allocated item,
-            # if not activated then no item filtered
-            # if not any item under view return string
-            xml_data_list = util.filter_allocated_item_from_view(kwargs['xml_data_list'],
-                                                                 kwargs['xml_view_list'])
-
-            if len(xml_data_list) > 0:
-                if all(i in question_answer.get_objects_names(kwargs['xml_function_list']) for i in object_list_str):
-
-                    if len(xml_data_list) != len(kwargs['xml_data_list']):
-                        xml_cons = [i for i in kwargs['xml_consumer_function_list']
-                                    if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                        xml_prod = [i for i in kwargs['xml_producer_function_list']
-                                    if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                    else:
-                        xml_cons = kwargs['xml_consumer_function_list']
-                        xml_prod = kwargs['xml_producer_function_list']
-                    plantuml_string = show_functions_sequence(object_list_str,
-                                                              kwargs['xml_function_list'],
-                                                              xml_cons,
-                                                              xml_prod,
-                                                              xml_data_list)
-
-                elif all(i in question_answer.get_objects_names(kwargs['xml_fun_elem_list']) for i in object_list_str):
-                    if len(xml_data_list) != len(kwargs['xml_data_list']):
-                        kwargs['xml_consumer_function_list'] = \
-                            [i for i in kwargs['xml_consumer_function_list']
-                             if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                        kwargs['xml_producer_function_list'] = \
-                            [i for i in kwargs['xml_producer_function_list']
-                             if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                    kwargs['xml_data_list'] = xml_data_list
-                    plantuml_string = get_fun_elem_sequence_diagram(object_list_str, **kwargs)
-
-                else:
-                    Logger.set_error(__name__,
-                                     f"{kwargs['diagram_object_str']} is not a valid sequence, available sequences "
-                                     f"are:\n"
-                                     f"- show sequence Function_A, Function_B, ...\n"
-                                     f"- show sequence Functional_element_A, Functional_element_B, ...\n"
-                                     f"- show sequence Functional_interface\n")
-
-    return plantuml_string
-
-
-def case_state_diagram(**kwargs):
-    """Case for 'show state <functional_element>'"""
-    plantuml_string = None
-    xml_fun_elem_name_list = question_answer.get_objects_names(kwargs['xml_fun_elem_list'])
-    if kwargs['diagram_object_str'] in xml_fun_elem_name_list:
-        plantuml_string = show_fun_elem_state_machine(kwargs['diagram_object_str'],
-                                                      kwargs['xml_state_list'],
-                                                      kwargs['xml_transition_list'],
-                                                      kwargs['xml_fun_elem_list'])
-    else:
-        Logger.set_error(__name__,
-                         f"Jarvis does not know the functional Element {kwargs['diagram_object_str']}")
-
-    return plantuml_string
-
-
-def case_state_sequence_diagram(**kwargs):
-    """Case for 'show state sequence <state>'"""
-    plantuml_string = None
-    xml_state_name_list = question_answer.get_objects_names(kwargs['xml_state_list'])
-    if kwargs['diagram_object_str'] in xml_state_name_list:
-        plantuml_string = show_state_allocated_function(kwargs['diagram_object_str'],
-                                                        kwargs['xml_state_list'],
-                                                        kwargs['xml_function_list'],
-                                                        kwargs['xml_consumer_function_list'],
-                                                        kwargs['xml_producer_function_list'],
-                                                        kwargs['xml_data_list'])
-    else:
-        Logger.set_error(__name__,
-                         f"Jarvis does not know the State {kwargs['diagram_object_str']}")
-
-    return plantuml_string
-
-
-def case_no_diagram(**kwargs):
-    """Default Case when no command has been found"""
-    Logger.set_warning(__name__,
-                       f"Jarvis does not understand the command {kwargs['diagram_type_str']}")
-
-
-def show_state_allocated_function(state_str, state_list, function_list, xml_consumer_function_list,
-                                  xml_producer_function_list, xml_data_list):
-    """Creates lists with desired objects for <state> function's allocation, send them to
-    plantuml_adapter.py then returns plantuml_text"""
-    allocated_function_id_list = set()
-    state_name = ''
-    for state in state_list:
-        if state_str in (state.name, state.alias):
-            if not state.allocated_function_list:
-                Logger.set_info(__name__,
-                                f"No function allocated to {state.name} (no display)")
-                return None
-
-            state_name = state.name
-            for fun_id in state.allocated_function_list:
-                allocated_function_id_list.add(fun_id)
-
-    for function in function_list:
-        if function.id in allocated_function_id_list.copy():
-            allocated_function_id_list.remove(function.id)
-            allocated_function_id_list.add(function.name)
-
-    diagram_str = show_functions_sequence(allocated_function_id_list, function_list,
-                                          xml_consumer_function_list, xml_producer_function_list,
-                                          xml_data_list, True)
-
-    diagram_str = f'box "{state_name}"\n{diagram_str}end box\n'
-
-    Logger.set_info(__name__,
-                    f"Function Sequence Diagram for {state_str} generated")
-
-    return diagram_str
-
-
-def show_fun_elem_state_machine(fun_elem_str, xml_state_list, xml_transition_list,
-                                xml_fun_elem_list):
-    """Creates lists with desired objects for <functional_element> state, send them to
-    plantuml_adapter.py then returns plantuml_text"""
-    new_fun_elem_list = set()
-
-    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        # TODO error message
-        return None
-
-    if not main_fun_elem.allocated_state_list:
-        Logger.set_error(__name__,
-                         f"No state allocated to {main_fun_elem.name} (no display)")
-        return None
-
-    new_fun_elem_list.add(main_fun_elem)
-
-    new_state_list = {s for s in xml_state_list if s.id in main_fun_elem.allocated_state_list}
-
-    new_transition_list = get_transitions(new_state_list, xml_transition_list)
-
-    plantuml_text = plantuml_adapter.get_state_machine_diagram(new_state_list,
-                                                               new_transition_list,
-                                                               xml_fun_elem_list)
-
-    Logger.set_info(__name__,
-                    f"State Machine Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def get_transitions(state_list, xml_transition_list):
-    """Get transitions if state(s) from state_list are source/destination"""
-    new_transition_list = set()
-    for new_state in state_list:
-        for transition in xml_transition_list:
-            if new_state.id == transition.source:
-                new_transition_list.add(transition)
-            if new_state.id == transition.destination:
-                new_transition_list.add(transition)
-
-    return new_transition_list
-
-
-def show_states_chain(state_list_str, xml_state_list, xml_transition_list):
-    """Creates lists with desired objects for <states> chain, send them to plantuml_adapter.py
-    then returns plantuml_text"""
-    new_state_list = set()
-    for state_str in state_list_str:
-        for state in xml_state_list:
-            if state_str in (state.name, state.alias):
-                state.child_list.clear()
-                state.set_parent(None)
-                new_state_list.add(state)
-
-    new_transition_list = get_transitions(new_state_list, xml_transition_list)
-
-    plantuml_text = plantuml_adapter.get_state_machine_diagram(new_state_list,
-                                                               new_transition_list)
-    spaced_state_list = ", ".join(state_list_str)
-    if len(state_list_str) == 1:
-        Logger.set_info(__name__,
-                        f"Context Diagram {str(spaced_state_list)} generated")
-    else:
-        Logger.set_info(__name__,
-                        f"Chain Diagram {str(spaced_state_list)} generated")
-
-    return plantuml_text
-
-
-def show_functions_sequence(function_list_str, xml_function_list, xml_consumer_function_list,
-                            xml_producer_function_list, xml_data_list, str_out=False):
-    """Creates lists with desired objects for <functions> sequence, send them to plantuml_adapter.py
-    then returns plantuml_text"""
-    new_function_list = set()
-
-    for i in function_list_str:
-        fun = question_answer.check_get_object(i, **{'xml_function_list': xml_function_list})
-        if not fun:
-            continue
-        fun.child_list.clear()
-        new_function_list.add(fun)
-
-    new_consumer_list = util.get_cons_or_prod_paired(new_function_list,
-                                                     xml_consumer_function_list,
-                                                     xml_producer_function_list)
-
-    new_producer_list = util.get_cons_or_prod_paired(new_function_list,
-                                                     xml_producer_function_list,
-                                                     xml_consumer_function_list)
-    # (Re)Filter data_list with only produced(same data in consumed since paired) and functions
-    # asked for sequence i.e. new_function_list used in get_cons_or_prod_paired()
-    # => TBC/TBT
-    new_data_list = {s for s in xml_data_list if any(s.name in j for j in new_producer_list)}
-
-    for new_data in new_data_list:
-        for pred in new_data.predecessor_list.copy():
-            if pred not in new_data_list:
-                new_data.predecessor_list.remove(pred)
-
-    plantuml_text = plantuml_adapter.get_sequence_diagram(new_function_list,
-                                                          new_consumer_list,
-                                                          new_producer_list,
-                                                          {},
-                                                          new_data_list, str_out)
-    if not str_out:
-        Logger.set_info(__name__,
-                        "Sequence Diagram " + str(", ".join(function_list_str)) + " generated")
-
-    return plantuml_text
-
-
-def get_fun_inter_sequence_diagram(fun_inter_str, **kwargs):
-    """
-    Check and get all "show sequence Fun_inter" strings, find Fun_inter obj and then get/filter
-    needed lists for plantuml_adapter.
-    Args:
-        fun_inter_str: functional interface name/alias from input cell
-        **kwargs: whole lists
-
-    Returns:
-        plantuml_text (str) : plantuml text
-    """
-    new_consumer_list = []
-    new_producer_list = []
-    new_fun_elem_list = set()
-    fun_inter = question_answer.check_get_object(
-        fun_inter_str, **{'xml_fun_inter_list': kwargs['xml_fun_inter_list']})
-
-    if fun_inter:
-        data_list_fun_inter = question_answer.switch_data(fun_inter, None, **kwargs)['data']
-        for elem in data_list_fun_inter:
-            fun_elem_cons = question_answer.check_get_object(
-                elem['Last consumer Functional element(s)'].pop(),
-                **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
-            fun_elem_prod = question_answer.check_get_object(
-                elem['Last producer Functional element(s)'].pop(),
-                **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
-            if fun_elem_cons and fun_elem_prod:
-                new_consumer_list.append([elem['Data'], fun_elem_cons])
-                new_producer_list.append([elem['Data'], fun_elem_prod])
-                new_fun_elem_list.add(fun_elem_cons)
-                new_fun_elem_list.add(fun_elem_prod)
-
-    if new_consumer_list and new_producer_list:
-        plantuml_text = plantuml_adapter.get_sequence_diagram(new_fun_elem_list,
-                                                              new_consumer_list,
-                                                              new_producer_list,
-                                                              {},
-                                                              kwargs['xml_data_list'])
-
-        return plantuml_text
-
-    else:
-        Logger.set_warning(__name__,
-                           f"No data found for {fun_inter.name}")
-
-
-def get_fun_elem_sequence_diagram(fun_elem_str, **kwargs):
-    """
-    Check and get all "show sequence Fun_elem_A, Fun_elem_B, ..." strings, find objects and
-    then get/filter needed lists for plantuml_adapter.
-    Args:
-        fun_elem_str: functional elements name/alias from input cell
-        **kwargs: dict with whole lists/sets
-
-    Returns:
-        plantuml_text (str) : plantuml_text
-    """
-    new_consumer_list = []
-    new_producer_list = []
-
-    new_fun_elem_list = {
-        question_answer.check_get_object(i, **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
-        for i in fun_elem_str
-    }
-
-    for fun_elem in new_fun_elem_list:
-        temp_fun_set = question_answer.get_allocation_object(
-            fun_elem,
-            kwargs['xml_function_list']
-        )
-
-        if isinstance(fun_elem.derived, FunctionalElement):
-            get_derived_if_in_view = util.filter_allocated_item_from_view(
-                {fun_elem.derived}, kwargs['xml_view_list']
-            )
-            # If type(list) has been returned from activated View()
-            # then add it's allocated func
-
-            # TODO not used in the code
-            if isinstance(get_derived_if_in_view, list):
-                alloc_derived_func_set = question_answer.get_allocation_object(
-                    fun_elem.derived,
-                    kwargs['xml_function_list']
-                )
-                # if alloc_derived_func_set is not None and temp_fun_set is not None:
-                # allocated_fun_set.update(alloc_derived_func_set)
-
-        if temp_fun_set is not None:
-            for fun in temp_fun_set:
-                new_consumer_list.extend(
-                    get_fun_elem_for_cons_prod_lists(
-                        fun_elem, fun, kwargs['xml_consumer_function_list']
-                    )
-                )
-                new_producer_list.extend(
-                    get_fun_elem_for_cons_prod_lists(
-                        fun_elem, fun, kwargs['xml_producer_function_list']
-                    )
-                )
-
-        fun_elem.child_list.clear()
-        fun_elem.parent = None
-
-    if new_consumer_list and new_producer_list:
-
-        for i in new_consumer_list:
-            if not any(i[0] in s for s in new_producer_list):
-                new_consumer_list.remove(i)
-
-        for j in new_producer_list:
-            if not any(j[0] in s for s in new_consumer_list):
-                new_producer_list.remove(j)
-
-    if new_consumer_list and new_producer_list:
-        plantuml_text = plantuml_adapter.get_sequence_diagram(new_fun_elem_list,
-                                                              new_consumer_list,
-                                                              new_producer_list,
-                                                              {},
-                                                              kwargs['xml_data_list'])
-
-        return plantuml_text
-
-    else:
-        Logger.set_warning(__name__,
-                           f"Not any data allocated to interfaces exposed by {', '.join(fun_elem_str)}")
-
-
-def get_fun_elem_for_cons_prod_lists(fun_elem, func_obj, cons_or_prod_list):
-    """
-    From cons or prod list [[data_1, function_1_str], [data_2, function_2_str], ...]
-    returns [[data_1, Function(1)], [data_2, Function(2)], ...]
-    """
-    output = []
-    for cons_or_prod in cons_or_prod_list:
-        if cons_or_prod[1] == func_obj:
-            output.append([cons_or_prod[0], fun_elem])
-
-    return output
+"""@defgroup diagram
+Jarvis diagram module
+"""
+# Libraries
+import re
+
+# Modules
+import plantuml_adapter
+from datamodel import FunctionalElement
+from jarvis.query import question_answer, query_object_list
+from jarvis.orchestrator import orchestrator_shared
+from jarvis import util as jarvis_util
+from . import diagram_generator_chain
+from . import diagram_generator_farch
+from . import diagram_generator_fana
+from . import util
+from tools import Logger
+
+
+def filter_show_command(diagram_name_str, **kwargs):
+    """Entry point for all diagrams (i.e. 'show' command) from command_parser.py"""
+    plantuml_string = None
+    wanted_diagram_str = diagram_name_str[0].strip()
+    regex = r"(decomposition|context|chain|sequence|state|function|state sequence)\s(.*)"
+    specific_diagram_str = re.search(regex, wanted_diagram_str, re.MULTILINE)
+    if specific_diagram_str:
+        if 'sequence' not in specific_diagram_str.group(2):
+            diagram_type_str = specific_diagram_str.group(1)
+            diagram_object_str = specific_diagram_str.group(2)
+        else:
+            diagram_type_str = specific_diagram_str.group(1) + ' sequence'
+            diagram_object_str = specific_diagram_str.group(2).replace("sequence ", "")
+
+        plantuml_string = switch_show_filter(diagram_type_str=diagram_type_str,
+                                             diagram_object_str=diagram_object_str,
+                                             **kwargs)
+    else:
+        Logger.set_warning(__name__,
+                           f"Jarvis does not understand the command {wanted_diagram_str}")
+
+    return plantuml_string
+
+
+def switch_show_filter(**kwargs):
+    """Switch case between diagram types"""
+    switch = {
+        "function": case_function_diagram,
+        "context": case_context_diagram,
+        "decomposition": case_decomposition_diagram,
+        "chain": case_chain_diagram,
+        "sequence": case_sequence_diagram,
+        "state": case_state_diagram,
+        "state sequence": case_state_sequence_diagram
+    }
+    get_diagram = switch.get(kwargs['diagram_type_str'], case_no_diagram)
+    return get_diagram(**kwargs)
+
+
+def case_function_diagram(**kwargs):
+    """Case for 'show function <functional_element>'"""
+    plantuml_string = None
+
+    if kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_fun_elem_list']):
+        plantuml_string = diagram_generator_farch.show_fun_elem_function(kwargs['diagram_object_str'],
+                                                                         kwargs['xml_fun_elem_list'],
+                                                                         kwargs['xml_function_list'],
+                                                                         kwargs['xml_consumer_function_list'],
+                                                                         kwargs['xml_producer_function_list'],
+                                                                         kwargs['xml_attribute_list'])
+
+    else:
+        Logger.set_warning(__name__,
+                           f"Jarvis does not know the functional Element {kwargs['diagram_object_str']}")
+
+    return plantuml_string
+
+
+def case_context_diagram(**kwargs):
+    """Case for 'show context <functional_element>/<function>'"""
+    plantuml_string = None
+
+    if kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_function_list']):
+        child_inheritance = orchestrator_shared.childs_inheritance(kwargs['xml_function_list'])
+        attribute_inheritance = orchestrator_shared.attribute_inheritance(kwargs['xml_attribute_list'],
+                                                                          kwargs['xml_function_list'])
+
+        plantuml_string = diagram_generator_fana.show_function_context(kwargs['diagram_object_str'],
+                                                                       kwargs['xml_function_list'],
+                                                                       kwargs['xml_consumer_function_list'],
+                                                                       kwargs['xml_producer_function_list'],
+                                                                       kwargs['xml_data_list'],
+                                                                       kwargs['xml_attribute_list'],
+                                                                       kwargs['xml_type_list'])
+
+        orchestrator_shared.reset_childs_inheritance(kwargs['xml_function_list'], derived_child_id=child_inheritance[2])
+        orchestrator_shared.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
+
+    elif kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_state_list']):
+        plantuml_string = show_states_chain([kwargs['diagram_object_str']],
+                                            kwargs['xml_state_list'],
+                                            kwargs['xml_transition_list'])
+
+    elif kwargs['diagram_object_str'] in question_answer.get_objects_names(kwargs['xml_fun_elem_list']):
+        child_inheritance = orchestrator_shared.childs_inheritance(kwargs['xml_function_list'],
+                                                                   kwargs['xml_fun_elem_list'],
+                                                                   level=None)
+        attribute_inheritance = orchestrator_shared.attribute_inheritance(kwargs['xml_attribute_list'],
+                                                                          kwargs['xml_function_list'],
+                                                                          kwargs['xml_fun_elem_list'],
+                                                                          kwargs['xml_fun_inter_list'])
+        func_alloc_inheritance = orchestrator_shared.allocation_inheritance(kwargs['xml_fun_elem_list'],
+                                                                            kwargs['xml_function_list'])
+        fun_inter_alloc_inheritance = orchestrator_shared.allocation_inheritance(kwargs['xml_fun_inter_list'],
+                                                                                 kwargs['xml_data_list'])
+
+        plantuml_string = diagram_generator_farch.show_fun_elem_context(kwargs['diagram_object_str'],
+                                                                        kwargs['xml_fun_elem_list'],
+                                                                        kwargs['xml_function_list'],
+                                                                        kwargs['xml_consumer_function_list'],
+                                                                        kwargs['xml_producer_function_list'],
+                                                                        kwargs['xml_attribute_list'],
+                                                                        kwargs['xml_fun_inter_list'],
+                                                                        kwargs['xml_data_list'])
+
+        orchestrator_shared.reset_childs_inheritance(kwargs['xml_function_list'],
+                                                     kwargs['xml_fun_elem_list'],
+                                                     derived_child_id=child_inheritance[2])
+        orchestrator_shared.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
+        orchestrator_shared.reset_alloc_inheritance(func_alloc_inheritance)
+        orchestrator_shared.reset_alloc_inheritance(fun_inter_alloc_inheritance)
+    else:
+        Logger.set_warning(__name__,
+                           f"Jarvis does not know the function {kwargs['diagram_object_str']} or "
+                           f"{kwargs['diagram_object_str']} is not a valid "
+                           f"Function/State/Functional Element name/alias")
+
+    return plantuml_string
+
+
+def case_decomposition_diagram(**kwargs):
+    """Case for 'show decomposition <functional_element>/<function>'"""
+    plantuml_string = None
+
+    if ' at level ' in kwargs['diagram_object_str']:
+        splitted_str = re.split(" at level ", kwargs['diagram_object_str'])
+        diagram_object_str = splitted_str[0]
+        try:
+            diagram_level = int(splitted_str[1])
+            if diagram_level == 0:
+                Logger.set_error(__name__,
+                                 "Invalid level, please choose a valid level >= 1")
+                return plantuml_string
+        except ValueError:
+            Logger.set_error(__name__,
+                             "Invalid level, please choose a valid level >= 1")
+            return plantuml_string
+    else:
+        diagram_object_str = kwargs['diagram_object_str']
+        diagram_level = None
+
+    v_inheritance = orchestrator_shared.view_inheritance(kwargs['xml_view_list'],
+                                                         kwargs['xml_function_list'],
+                                                         kwargs['xml_fun_elem_list'])
+
+    # Check view if activated and filter allocated item
+    function_list = util.get_object_list_from_view(diagram_object_str,
+                                                   kwargs['xml_function_list'],
+                                                   kwargs['xml_view_list'])
+
+    if len(function_list) > 0:
+        _, consumer_list, producer_list = \
+            util.get_cons_prod_from_view_allocated_data(kwargs['xml_data_list'],
+                                                        kwargs['xml_view_list'],
+                                                        kwargs['xml_consumer_function_list'],
+                                                        kwargs['xml_producer_function_list'],
+                                                        function_list)
+    else:
+        consumer_list = []
+        producer_list = []
+
+    if diagram_object_str in question_answer.get_objects_names(kwargs['xml_function_list']):
+        child_inheritance = orchestrator_shared.childs_inheritance(function_list, level=diagram_level)
+        attribute_inheritance = orchestrator_shared.attribute_inheritance(kwargs['xml_attribute_list'],
+                                                                          function_list)
+
+        plantuml_string = diagram_generator_fana.show_function_decomposition(diagram_object_str,
+                                                                             function_list,
+                                                                             consumer_list,
+                                                                             producer_list,
+                                                                             kwargs['xml_attribute_list'],
+                                                                             kwargs['xml_type_list'],
+                                                                             diagram_level=diagram_level)
+
+        orchestrator_shared.reset_childs_inheritance(function_list, derived_child_id=child_inheritance[2])
+        orchestrator_shared.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
+    elif diagram_object_str in question_answer.get_objects_names(kwargs['xml_fun_elem_list']):
+        fun_elem_list = util.get_object_list_from_view(diagram_object_str,
+                                                       kwargs['xml_fun_elem_list'],
+                                                       kwargs['xml_view_list'])
+
+        if len(fun_elem_list) > 0:
+            child_inheritance = orchestrator_shared.childs_inheritance(function_list, fun_elem_list,
+                                                                       level=diagram_level)
+            attribute_inheritance = orchestrator_shared.attribute_inheritance(kwargs['xml_attribute_list'],
+                                                                              function_list,
+                                                                              fun_elem_list,
+                                                                              kwargs['xml_fun_inter_list'])
+            func_alloc_inheritance = orchestrator_shared.allocation_inheritance(fun_elem_list, function_list)
+            fun_inter_alloc_inheritance = orchestrator_shared.allocation_inheritance(kwargs['xml_fun_inter_list'],
+                                                                                     kwargs['xml_data_list'])
+
+            plantuml_string = diagram_generator_farch.show_fun_elem_decomposition(diagram_object_str,
+                                                                                  function_list,
+                                                                                  consumer_list,
+                                                                                  producer_list,
+                                                                                  fun_elem_list,
+                                                                                  kwargs['xml_attribute_list'],
+                                                                                  kwargs['xml_data_list'],
+                                                                                  kwargs['xml_fun_inter_list'],
+                                                                                  diagram_level)
+
+            orchestrator_shared.reset_childs_inheritance(function_list,
+                                                         fun_elem_list,
+                                                         derived_child_id=child_inheritance[2])
+            orchestrator_shared.reset_attribute_inheritance(kwargs['xml_attribute_list'], attribute_inheritance)
+            orchestrator_shared.reset_alloc_inheritance(func_alloc_inheritance)
+            orchestrator_shared.reset_alloc_inheritance(fun_inter_alloc_inheritance)
+    else:
+        Logger.set_warning(__name__,
+                           f"Jarvis does not know the object {diagram_object_str}"
+                           f"(i.e. it is not a function, nor a functional element)")
+
+    orchestrator_shared.reset_view_inheritance(kwargs['xml_view_list'], v_inheritance)
+
+    return plantuml_string
+
+
+def case_chain_diagram(**kwargs):
+    """Case for 'show chain <states>/<functions>'"""
+    plantuml_string = None
+
+    object_list_str = jarvis_util.cut_string(kwargs['diagram_object_str'])
+
+    if len(object_list_str) > 0:
+        xml_function_name_list = question_answer.get_objects_names(kwargs['xml_function_list'])
+        result_function = all(t in xml_function_name_list for t in object_list_str)
+
+        xml_state_name_list = question_answer.get_objects_names(kwargs['xml_state_list'])
+        result_state = all(t in xml_state_name_list for t in object_list_str)
+
+        xml_fun_elem_name_list = question_answer.get_objects_names(kwargs['xml_fun_elem_list'])
+        result_fun_elem = all(t in xml_fun_elem_name_list for t in object_list_str)
+
+        if result_function:
+            function_list = util.get_object_list_from_view(object_list_str,
+                                                           kwargs['xml_function_list'],
+                                                           kwargs['xml_view_list'])
+
+            if len(function_list) > 0:
+                _, consumer_list, producer_list = \
+                    util.get_cons_prod_from_view_allocated_data(kwargs['xml_data_list'],
+                                                                kwargs['xml_view_list'],
+                                                                kwargs[
+                                                                    'xml_consumer_function_list'],
+                                                                kwargs[
+                                                                    'xml_producer_function_list'],
+                                                                function_list)
+
+                plantuml_string = diagram_generator_chain.show_function_chain(object_list_str,
+                                                                              function_list,
+                                                                              consumer_list,
+                                                                              producer_list,
+                                                                              kwargs['xml_type_list'],
+                                                                              kwargs['xml_attribute_list'])
+            else:
+                Logger.set_warning(__name__,
+                                   f"Nothing to display for the selected view")
+        elif result_fun_elem:
+            fun_elem_list_from_view = util.get_object_list_from_view(object_list_str,
+                                                                     kwargs['xml_fun_elem_list'],
+                                                                     kwargs['xml_view_list'])
+
+            if len(fun_elem_list_from_view) > 0:
+                fun_elem_list = set()
+                function_list = set()
+
+                function_list_from_view = util.get_object_list_from_view(object_list_str,
+                                                                         kwargs['xml_function_list'],
+                                                                         kwargs['xml_view_list'])
+
+                for i in object_list_str:
+                    for fun_elem in fun_elem_list_from_view:
+                        if i == fun_elem.name or i == fun_elem.alias:
+                            fun_elem_list.add(fun_elem)
+
+                            if len(fun_elem.allocated_function_list) > 0:
+                                for allocated_function_id in fun_elem.allocated_function_list:
+                                    for function in kwargs['xml_function_list']:
+                                        if function.id == allocated_function_id and function in function_list_from_view:
+                                            util.get_fun_elem_function_list(function, function_list, fun_elem)
+                            else:
+                                Logger.set_info(__name__,
+                                                f"No function allocated to {fun_elem.name} (no display)")
+
+                new_function_list, consumer_list, producer_list = \
+                    util.get_cons_prod_from_view_allocated_data(kwargs['xml_data_list'],
+                                                                kwargs['xml_view_list'],
+                                                                kwargs[
+                                                                    'xml_consumer_function_list'],
+                                                                kwargs[
+                                                                    'xml_producer_function_list'],
+                                                                function_list)
+
+                plantuml_string = diagram_generator_chain.show_fun_elem_chain(object_list_str,
+                                                                              new_function_list,
+                                                                              consumer_list,
+                                                                              producer_list,
+                                                                              fun_elem_list,
+                                                                              kwargs['xml_type_list'],
+                                                                              kwargs['xml_attribute_list'])
+            else:
+                Logger.set_warning(__name__,
+                                   f"Nothing to display for the selected view")
+        elif result_state:
+            state_list = util.get_object_list_from_view(object_list_str,
+                                                        kwargs['xml_state_list'],
+                                                        kwargs['xml_view_list'])
+
+            if len(state_list) > 0:
+                transition_list = util.filter_allocated_item_from_view(kwargs['xml_transition_list'],
+                                                                       kwargs['xml_view_list'])
+
+                plantuml_string = show_states_chain(object_list_str, state_list, transition_list)
+            else:
+                Logger.set_warning(__name__,
+                                   f"Nothing to display for the selected view")
+        else:
+            Logger.set_warning(__name__,
+                               f"Jarvis does not know the object(s): {kwargs['diagram_object_str']}"
+                               f"(i.e. it is not a function, nor a functional element, nor a state)")
+    else:
+        Logger.set_error(__name__,
+                         f"{kwargs['diagram_object_str']} is not a valid chain")
+
+    return plantuml_string
+
+
+def case_sequence_diagram(**kwargs):
+    """Case for 'show sequence <functional_elements>/<functions>/<functional_interface>'"""
+    plantuml_string = None
+    object_list_str = re.split(r',(?![^[]*\])', kwargs['diagram_object_str'].replace(", ", ","))
+    object_list_str = [s.rstrip() for s in object_list_str]
+    if object_list_str:
+        if len(object_list_str) == 1 and \
+                any(s == object_list_str[0] for s in question_answer.get_objects_names(kwargs['xml_fun_inter_list'])):
+            plantuml_string = get_fun_inter_sequence_diagram(object_list_str.pop(), **kwargs)
+        elif len(object_list_str) >= 1:
+            # Check view if activated and filter allocated item,
+            # if not activated then no item filtered
+            # if not any item under view return string
+            xml_data_list = util.filter_allocated_item_from_view(kwargs['xml_data_list'],
+                                                                 kwargs['xml_view_list'])
+
+            if len(xml_data_list) > 0:
+                if all(i in question_answer.get_objects_names(kwargs['xml_function_list']) for i in object_list_str):
+
+                    if len(xml_data_list) != len(kwargs['xml_data_list']):
+                        xml_cons = [i for i in kwargs['xml_consumer_function_list']
+                                    if any(a == i[0] for a in [d.name for d in xml_data_list])]
+                        xml_prod = [i for i in kwargs['xml_producer_function_list']
+                                    if any(a == i[0] for a in [d.name for d in xml_data_list])]
+                    else:
+                        xml_cons = kwargs['xml_consumer_function_list']
+                        xml_prod = kwargs['xml_producer_function_list']
+                    plantuml_string = show_functions_sequence(object_list_str,
+                                                              kwargs['xml_function_list'],
+                                                              xml_cons,
+                                                              xml_prod,
+                                                              xml_data_list)
+
+                elif all(i in question_answer.get_objects_names(kwargs['xml_fun_elem_list']) for i in object_list_str):
+                    if len(xml_data_list) != len(kwargs['xml_data_list']):
+                        kwargs['xml_consumer_function_list'] = \
+                            [i for i in kwargs['xml_consumer_function_list']
+                             if any(a == i[0] for a in [d.name for d in xml_data_list])]
+                        kwargs['xml_producer_function_list'] = \
+                            [i for i in kwargs['xml_producer_function_list']
+                             if any(a == i[0] for a in [d.name for d in xml_data_list])]
+                    kwargs['xml_data_list'] = xml_data_list
+                    plantuml_string = get_fun_elem_sequence_diagram(object_list_str, **kwargs)
+
+                else:
+                    Logger.set_error(__name__,
+                                     f"{kwargs['diagram_object_str']} is not a valid sequence, available sequences "
+                                     f"are:\n"
+                                     f"- show sequence Function_A, Function_B, ...\n"
+                                     f"- show sequence Functional_element_A, Functional_element_B, ...\n"
+                                     f"- show sequence Functional_interface\n")
+
+    return plantuml_string
+
+
+def case_state_diagram(**kwargs):
+    """Case for 'show state <functional_element>'"""
+    plantuml_string = None
+    xml_fun_elem_name_list = question_answer.get_objects_names(kwargs['xml_fun_elem_list'])
+    if kwargs['diagram_object_str'] in xml_fun_elem_name_list:
+        plantuml_string = show_fun_elem_state_machine(kwargs['diagram_object_str'],
+                                                      kwargs['xml_state_list'],
+                                                      kwargs['xml_transition_list'],
+                                                      kwargs['xml_fun_elem_list'])
+    else:
+        Logger.set_error(__name__,
+                         f"Jarvis does not know the functional Element {kwargs['diagram_object_str']}")
+
+    return plantuml_string
+
+
+def case_state_sequence_diagram(**kwargs):
+    """Case for 'show state sequence <state>'"""
+    plantuml_string = None
+    xml_state_name_list = question_answer.get_objects_names(kwargs['xml_state_list'])
+    if kwargs['diagram_object_str'] in xml_state_name_list:
+        plantuml_string = show_state_allocated_function(kwargs['diagram_object_str'],
+                                                        kwargs['xml_state_list'],
+                                                        kwargs['xml_function_list'],
+                                                        kwargs['xml_consumer_function_list'],
+                                                        kwargs['xml_producer_function_list'],
+                                                        kwargs['xml_data_list'])
+    else:
+        Logger.set_error(__name__,
+                         f"Jarvis does not know the State {kwargs['diagram_object_str']}")
+
+    return plantuml_string
+
+
+def case_no_diagram(**kwargs):
+    """Default Case when no command has been found"""
+    Logger.set_warning(__name__,
+                       f"Jarvis does not understand the command {kwargs['diagram_type_str']}")
+
+
+def show_state_allocated_function(state_str, state_list, function_list, xml_consumer_function_list,
+                                  xml_producer_function_list, xml_data_list):
+    """Creates lists with desired objects for <state> function's allocation, send them to
+    plantuml_adapter.py then returns plantuml_text"""
+    allocated_function_id_list = set()
+    state_name = ''
+    for state in state_list:
+        if state_str in (state.name, state.alias):
+            if not state.allocated_function_list:
+                Logger.set_info(__name__,
+                                f"No function allocated to {state.name} (no display)")
+                return None
+
+            state_name = state.name
+            for fun_id in state.allocated_function_list:
+                allocated_function_id_list.add(fun_id)
+
+    for function in function_list:
+        if function.id in allocated_function_id_list.copy():
+            allocated_function_id_list.remove(function.id)
+            allocated_function_id_list.add(function.name)
+
+    diagram_str = show_functions_sequence(allocated_function_id_list, function_list,
+                                          xml_consumer_function_list, xml_producer_function_list,
+                                          xml_data_list, True)
+
+    diagram_str = f'box "{state_name}"\n{diagram_str}end box\n'
+
+    Logger.set_info(__name__,
+                    f"Function Sequence Diagram for {state_str} generated")
+
+    return diagram_str
+
+
+def show_fun_elem_state_machine(fun_elem_str, xml_state_list, xml_transition_list,
+                                xml_fun_elem_list):
+    """Creates lists with desired objects for <functional_element> state, send them to
+    plantuml_adapter.py then returns plantuml_text"""
+    new_fun_elem_list = set()
+
+    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
+    if not main_fun_elem:
+        # TODO error message
+        return None
+
+    if not main_fun_elem.allocated_state_list:
+        Logger.set_error(__name__,
+                         f"No state allocated to {main_fun_elem.name} (no display)")
+        return None
+
+    new_fun_elem_list.add(main_fun_elem)
+
+    new_state_list = {s for s in xml_state_list if s.id in main_fun_elem.allocated_state_list}
+
+    new_transition_list = get_transitions(new_state_list, xml_transition_list)
+
+    plantuml_text = plantuml_adapter.get_state_machine_diagram(new_state_list,
+                                                               new_transition_list,
+                                                               xml_fun_elem_list)
+
+    Logger.set_info(__name__,
+                    f"State Machine Diagram for {fun_elem_str} generated")
+
+    return plantuml_text
+
+
+def get_transitions(state_list, xml_transition_list):
+    """Get transitions if state(s) from state_list are source/destination"""
+    new_transition_list = set()
+    for new_state in state_list:
+        for transition in xml_transition_list:
+            if new_state.id == transition.source:
+                new_transition_list.add(transition)
+            if new_state.id == transition.destination:
+                new_transition_list.add(transition)
+
+    return new_transition_list
+
+
+def show_states_chain(state_list_str, xml_state_list, xml_transition_list):
+    """Creates lists with desired objects for <states> chain, send them to plantuml_adapter.py
+    then returns plantuml_text"""
+    new_state_list = set()
+    new_transition_list = set()
+    context_state_list = set()
+    spaced_state_list = ", ".join(state_list_str)
+
+    for state_str in state_list_str:
+        for state in xml_state_list:
+            if state_str in (state.name, state.alias):
+                state.child_list.clear()
+                state.set_parent(None)
+                new_state_list.add(state)
+            else:
+                context_state_list.add(state)
+
+    if len(state_list_str) > 1:
+        # In case of chain diagram, discard the context
+        context_state_list = new_state_list
+    # Else do nothing
+
+    for state in new_state_list.copy():
+        # State list depends on transition reachable from the state
+        for transition in xml_transition_list:
+            if transition.source == state.id:
+                for context_state in context_state_list:
+                    if transition.destination == context_state.id:
+                        context_state.child_list.clear()
+                        context_state.set_parent(None)
+                        new_state_list.add(context_state)
+                        new_transition_list.add(transition)
+            # Else do nothing
+            if transition.destination == state.id:
+                for context_state in context_state_list:
+                    if transition.source == context_state.id:
+                        context_state.child_list.clear()
+                        context_state.set_parent(None)
+                        new_state_list.add(context_state)
+                        new_transition_list.add(transition)
+            # Else do nothing
+
+    plantuml_text = plantuml_adapter.get_state_machine_diagram(sorted(new_state_list, key=lambda x: x.name,
+                                                                      reverse=False),
+                                                               sorted(new_transition_list, key=lambda x: x.name,
+                                                                      reverse=False))
+    if len(state_list_str) == 1:
+        Logger.set_info(__name__,
+                        f"Context Diagram {str(spaced_state_list)} generated")
+    else:
+        Logger.set_info(__name__,
+                        f"Chain Diagram {str(spaced_state_list)} generated")
+
+    return plantuml_text
+
+
+def show_functions_sequence(function_list_str, xml_function_list, xml_consumer_function_list,
+                            xml_producer_function_list, xml_data_list, str_out=False):
+    """Creates lists with desired objects for <functions> sequence, send them to plantuml_adapter.py
+    then returns plantuml_text"""
+    new_function_list = set()
+
+    for i in function_list_str:
+        fun = question_answer.check_get_object(i, **{'xml_function_list': xml_function_list})
+        if not fun:
+            continue
+        fun.child_list.clear()
+        new_function_list.add(fun)
+
+    new_consumer_list = util.get_cons_or_prod_paired(new_function_list,
+                                                     xml_consumer_function_list,
+                                                     xml_producer_function_list)
+
+    new_producer_list = util.get_cons_or_prod_paired(new_function_list,
+                                                     xml_producer_function_list,
+                                                     xml_consumer_function_list)
+    # (Re)Filter data_list with only produced(same data in consumed since paired) and functions
+    # asked for sequence i.e. new_function_list used in get_cons_or_prod_paired()
+    # => TBC/TBT
+    new_data_list = {s for s in xml_data_list if any(s.name in j for j in new_producer_list)}
+
+    for new_data in new_data_list:
+        for pred in new_data.predecessor_list.copy():
+            if pred not in new_data_list:
+                new_data.predecessor_list.remove(pred)
+
+    plantuml_text = plantuml_adapter.get_sequence_diagram(new_function_list,
+                                                          new_consumer_list,
+                                                          new_producer_list,
+                                                          {},
+                                                          new_data_list, str_out)
+    if not str_out:
+        Logger.set_info(__name__,
+                        "Sequence Diagram " + str(", ".join(function_list_str)) + " generated")
+
+    return plantuml_text
+
+
+def get_fun_inter_sequence_diagram(fun_inter_str, **kwargs):
+    """
+    Check and get all "show sequence Fun_inter" strings, find Fun_inter obj and then get/filter
+    needed lists for plantuml_adapter.
+    Args:
+        fun_inter_str: functional interface name/alias from input cell
+        **kwargs: whole lists
+
+    Returns:
+        plantuml_text (str) : plantuml text
+    """
+    new_consumer_list = []
+    new_producer_list = []
+    new_fun_elem_list = set()
+    fun_inter = question_answer.check_get_object(
+        fun_inter_str, **{'xml_fun_inter_list': kwargs['xml_fun_inter_list']})
+
+    if fun_inter:
+        data_list_fun_inter = query_object_list.get_fun_intf_data(fun_inter, None, **kwargs)['data']
+        for elem in data_list_fun_inter:
+            if elem['Last consumer Functional element(s)']:
+                fun_elem_cons = question_answer.check_get_object(
+                    elem['Last consumer Functional element(s)'].pop(),
+                    **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
+            else:
+                fun_elem_cons = []
+
+            if elem['Last producer Functional element(s)']:
+                fun_elem_prod = question_answer.check_get_object(
+                    elem['Last producer Functional element(s)'].pop(),
+                    **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
+            else:
+                fun_elem_prod = []
+
+            if fun_elem_cons and fun_elem_prod:
+                new_consumer_list.append([elem['Data'], fun_elem_cons])
+                new_producer_list.append([elem['Data'], fun_elem_prod])
+                new_fun_elem_list.add(fun_elem_cons)
+                new_fun_elem_list.add(fun_elem_prod)
+
+    if new_consumer_list and new_producer_list:
+        plantuml_text = plantuml_adapter.get_sequence_diagram(new_fun_elem_list,
+                                                              new_consumer_list,
+                                                              new_producer_list,
+                                                              {},
+                                                              kwargs['xml_data_list'])
+
+        return plantuml_text
+
+    else:
+        Logger.set_warning(__name__,
+                           f"No data found for {fun_inter.name}")
+
+
+def get_fun_elem_sequence_diagram(fun_elem_str, **kwargs):
+    """
+    Check and get all "show sequence Fun_elem_A, Fun_elem_B, ..." strings, find objects and
+    then get/filter needed lists for plantuml_adapter.
+    Args:
+        fun_elem_str: functional elements name/alias from input cell
+        **kwargs: dict with whole lists/sets
+
+    Returns:
+        plantuml_text (str) : plantuml_text
+    """
+    new_consumer_list = []
+    new_producer_list = []
+
+    new_fun_elem_list = {
+        question_answer.check_get_object(i, **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
+        for i in fun_elem_str
+    }
+
+    for fun_elem in new_fun_elem_list:
+        temp_fun_set = question_answer.get_allocation_object(
+            fun_elem,
+            kwargs['xml_function_list']
+        )
+
+        if isinstance(fun_elem.derived, FunctionalElement):
+            get_derived_if_in_view = util.filter_allocated_item_from_view(
+                {fun_elem.derived}, kwargs['xml_view_list']
+            )
+            # If type(list) has been returned from activated View()
+            # then add it's allocated func
+
+            # TODO not used in the code
+            if isinstance(get_derived_if_in_view, list):
+                alloc_derived_func_set = question_answer.get_allocation_object(
+                    fun_elem.derived,
+                    kwargs['xml_function_list']
+                )
+                # if alloc_derived_func_set is not None and temp_fun_set is not None:
+                # allocated_fun_set.update(alloc_derived_func_set)
+
+        if temp_fun_set is not None:
+            for fun in temp_fun_set:
+                new_consumer_list.extend(
+                    get_fun_elem_for_cons_prod_lists(
+                        fun_elem, fun, kwargs['xml_consumer_function_list']
+                    )
+                )
+                new_producer_list.extend(
+                    get_fun_elem_for_cons_prod_lists(
+                        fun_elem, fun, kwargs['xml_producer_function_list']
+                    )
+                )
+
+        fun_elem.child_list.clear()
+        fun_elem.parent = None
+
+    if new_consumer_list and new_producer_list:
+
+        for i in new_consumer_list:
+            if not any(i[0] in s for s in new_producer_list):
+                new_consumer_list.remove(i)
+
+        for j in new_producer_list:
+            if not any(j[0] in s for s in new_consumer_list):
+                new_producer_list.remove(j)
+
+    if new_consumer_list and new_producer_list:
+        plantuml_text = plantuml_adapter.get_sequence_diagram(new_fun_elem_list,
+                                                              new_consumer_list,
+                                                              new_producer_list,
+                                                              {},
+                                                              kwargs['xml_data_list'])
+
+        return plantuml_text
+
+    else:
+        Logger.set_warning(__name__,
+                           f"Not any data allocated to interfaces exposed by {', '.join(fun_elem_str)}")
+
+
+def get_fun_elem_for_cons_prod_lists(fun_elem, func_obj, cons_or_prod_list):
+    """
+    From cons or prod list [[data_1, function_1_str], [data_2, function_2_str], ...]
+    returns [[data_1, Function(1)], [data_2, Function(2)], ...]
+    """
+    output = []
+    for cons_or_prod in cons_or_prod_list:
+        if cons_or_prod[1] == func_obj:
+            output.append([cons_or_prod[0], fun_elem])
+
+    return output
```

### Comparing `jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_chain.py` & `jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-"""@defgroup diagram
-Jarvis diagram module
-"""
-# Libraries
-
-# Modules
-import plantuml_adapter
-from . import util
-from tools import Logger
-
-
-def show_function_chain(function_list_str, xml_function_list, xml_consumer_function_list,
-                        xml_producer_function_list, xml_type_list, xml_attribute_list):
-    new_function_list = set()
-    new_parent_dict = {}
-    new_producer_list = []
-    new_consumer_list = []
-
-    for i in function_list_str:
-        for fun in xml_function_list:
-            if i == fun.name or i == fun.alias:
-                new_function_list.add(fun)
-
-                util.get_parent_dict(fun, new_function_list, new_parent_dict)
-
-                for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
-                    if fun == xml_consumer:
-                        fun.child_list.clear()
-                        if [xml_consumer_flow, fun] not in new_consumer_list and \
-                                [xml_consumer_flow, fun] not in xml_producer_function_list:
-                            new_consumer_list.append([xml_consumer_flow, fun])
-
-                for xml_producer_flow, xml_producer in xml_producer_function_list:
-                    if fun == xml_producer:
-                        fun.child_list.clear()
-                        if [xml_producer_flow, fun] not in new_producer_list and \
-                                [xml_producer_flow, fun] not in xml_consumer_function_list:
-                            new_producer_list.append([xml_producer_flow, fun])
-
-    Logger.set_debug(__name__, f"function list: {new_function_list}")
-    Logger.set_debug(__name__, f"consumer function list: {new_consumer_list}")
-    Logger.set_debug(__name__, f"producer function list: {new_producer_list}")
-    Logger.set_debug(__name__, f"parent list: {new_parent_dict}")
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
-                                                           fun_elem_list=None,
-                                                           consumer_function_list=new_consumer_list,
-                                                           producer_function_list=new_producer_list,
-                                                           parent_child_dict=new_parent_dict,
-                                                           data_list=None,
-                                                           xml_type_list=xml_type_list,
-                                                           xml_attribute_list=xml_attribute_list)
-
-    Logger.set_info(__name__,
-                    f'Chain Diagram {str(", ".join(function_list_str))} generated')
-
-    return plantuml_text
-
-
-def show_fun_elem_chain(fun_elem_list_str, xml_function_list, xml_consumer_function_list, xml_producer_function_list,
-                        xml_fun_elem_list, xml_type_list, xml_attribute_list):
-    parent_child_dict = {}
-
-    for i in fun_elem_list_str:
-        for fun_elem in xml_fun_elem_list:
-            if i == fun_elem.name or i == fun_elem.alias:
-                if len(fun_elem.allocated_function_list) > 0:
-                    for allocated_function_id in fun_elem.allocated_function_list:
-                        parent_child_dict[allocated_function_id] = fun_elem.id
-
-    external_function_list, new_consumer_list, new_producer_list = \
-        util.get_cons_prod_from_allocated_functions(xml_function_list,
-                                                    xml_producer_function_list,
-                                                    xml_consumer_function_list,
-                                                    False)
-
-    Logger.set_debug(__name__, f'list of allocated functions to element: {xml_function_list}')
-    Logger.set_debug(__name__, f'list of external functions to element: {external_function_list}')
-    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
-    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=xml_function_list,
-                                                           fun_elem_list=xml_fun_elem_list,
-                                                           consumer_function_list=new_consumer_list,
-                                                           producer_function_list=new_producer_list,
-                                                           parent_child_dict=parent_child_dict,
-                                                           data_list=None,
-                                                           xml_type_list=None,
-                                                           xml_attribute_list=xml_attribute_list)
-
-    Logger.set_info(__name__,
-                    f'Chain Diagram {str(", ".join(fun_elem_list_str))} generated')
-
-    return plantuml_text
+"""@defgroup diagram
+Jarvis diagram module
+"""
+# Libraries
+
+# Modules
+import plantuml_adapter
+from . import util
+from tools import Logger
+
+
+def show_function_chain(function_list_str, xml_function_list, xml_consumer_function_list,
+                        xml_producer_function_list, xml_type_list, xml_attribute_list):
+    new_function_list = set()
+    new_parent_dict = {}
+    new_producer_list = []
+    new_consumer_list = []
+
+    for i in function_list_str:
+        for fun in xml_function_list:
+            if i == fun.name or i == fun.alias:
+                new_function_list.add(fun)
+
+                util.get_parent_dict(fun, new_function_list, new_parent_dict)
+
+                for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
+                    if fun == xml_consumer:
+                        fun.child_list.clear()
+                        if [xml_consumer_flow, fun] not in new_consumer_list and \
+                                [xml_consumer_flow, fun] not in xml_producer_function_list:
+                            new_consumer_list.append([xml_consumer_flow, fun])
+
+                for xml_producer_flow, xml_producer in xml_producer_function_list:
+                    if fun == xml_producer:
+                        fun.child_list.clear()
+                        if [xml_producer_flow, fun] not in new_producer_list and \
+                                [xml_producer_flow, fun] not in xml_consumer_function_list:
+                            new_producer_list.append([xml_producer_flow, fun])
+
+    Logger.set_debug(__name__, f"function list: {new_function_list}")
+    Logger.set_debug(__name__, f"consumer function list: {new_consumer_list}")
+    Logger.set_debug(__name__, f"producer function list: {new_producer_list}")
+    Logger.set_debug(__name__, f"parent list: {new_parent_dict}")
+
+    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
+                                                           fun_elem_list=None,
+                                                           consumer_function_list=new_consumer_list,
+                                                           producer_function_list=new_producer_list,
+                                                           parent_child_dict=new_parent_dict,
+                                                           data_list=None,
+                                                           xml_type_list=xml_type_list,
+                                                           xml_attribute_list=xml_attribute_list)
+
+    Logger.set_info(__name__,
+                    f'Chain Diagram {str(", ".join(function_list_str))} generated')
+
+    return plantuml_text
+
+
+def show_fun_elem_chain(fun_elem_list_str, xml_function_list, xml_consumer_function_list, xml_producer_function_list,
+                        xml_fun_elem_list, xml_type_list, xml_attribute_list):
+    parent_child_dict = {}
+
+    for i in fun_elem_list_str:
+        for fun_elem in xml_fun_elem_list.copy():
+            if i == fun_elem.name or i == fun_elem.alias:
+                if fun_elem.parent:
+                    xml_fun_elem_list.add(fun_elem.parent)
+                    parent_child_dict[fun_elem.id] = fun_elem.parent.id
+                if len(fun_elem.allocated_function_list) > 0:
+                    for allocated_function_id in fun_elem.allocated_function_list:
+                        parent_child_dict[allocated_function_id] = fun_elem.id
+
+    external_function_list, new_consumer_list, new_producer_list = \
+        util.get_cons_prod_from_allocated_functions(xml_function_list,
+                                                    xml_producer_function_list,
+                                                    xml_consumer_function_list,
+                                                    False)
+
+    Logger.set_debug(__name__, f'list of allocated functions to element: {xml_function_list}')
+    Logger.set_debug(__name__, f'list of external functions to element: {external_function_list}')
+    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
+    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
+
+    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=xml_function_list,
+                                                           fun_elem_list=xml_fun_elem_list,
+                                                           consumer_function_list=new_consumer_list,
+                                                           producer_function_list=new_producer_list,
+                                                           parent_child_dict=parent_child_dict,
+                                                           data_list=None,
+                                                           xml_type_list=None,
+                                                           xml_attribute_list=xml_attribute_list)
+
+    Logger.set_info(__name__,
+                    f'Chain Diagram {str(", ".join(fun_elem_list_str))} generated')
+
+    return plantuml_text
```

### Comparing `jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_fana.py` & `jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator_fana.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""@defgroup diagram
-Jarvis diagram module
-"""
-# Libraries
-
-# Modules
-import plantuml_adapter
-from jarvis import question_answer
-from . import util
-from tools import Logger
-
-
-def show_function_context(diagram_function_str, xml_function_list, xml_consumer_function_list,
-                          xml_producer_function_list, xml_data_list, xml_attribute_list,
-                          xml_type_list):
-
-    new_function_list, new_consumer_list, new_producer_list = util.get_function_context_lists(
-        diagram_function_str,
-        xml_function_list,
-        xml_consumer_function_list,
-        xml_producer_function_list)
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
-                                                           fun_elem_list=None,
-                                                           consumer_function_list=new_consumer_list,
-                                                           producer_function_list=new_producer_list,
-                                                           parent_child_dict={},
-                                                           data_list=xml_data_list,
-                                                           xml_type_list=xml_type_list,
-                                                           xml_attribute_list=xml_attribute_list)
-
-    Logger.set_info(__name__,
-                    f"Context Diagram {diagram_function_str} generated")
-
-    return plantuml_text
-
-
-# TODO: Clean-up once inheritance has been validated (Create method for Function and others
-#  objects?)
-def show_function_decomposition(diagram_function_str, xml_function_list, xml_consumer_function_list,
-                                xml_producer_function_list, xml_attribute_list, xml_type_list,
-                                diagram_level=None):
-    """Create necessary lists then returns plantuml text for decomposition of function"""
-    main_fun = question_answer.check_get_object(diagram_function_str, **{'xml_function_list': xml_function_list})
-
-    if not main_fun:
-        return
-
-    main_parent = main_fun.parent
-
-    if diagram_level:
-        full_fun_list, _ = question_answer.get_children(main_fun)
-        main_function_list, main_parent_dict = question_answer.get_children(main_fun, level=diagram_level)
-        # derived = childs_inheritance(main_fun, level=diagram_level)
-        # if derived:
-        #     main_function_list = main_function_list.union(derived[0])
-        #     main_parent_dict.update(derived[1])
-
-        # Remove functions and flows that are not in the diagram level
-        for k in full_fun_list.symmetric_difference(main_function_list):
-            Logger.set_debug(__name__, f"{k.name} not in diagram level {diagram_level}")
-            for cons in xml_consumer_function_list.copy():
-                if k in cons:
-                    xml_consumer_function_list.remove([cons[0], k])
-                    Logger.set_debug(__name__, f"[{cons[0]}, {k.name} removed]")
-
-            for prod in xml_producer_function_list.copy():
-                if k in prod:
-                    xml_producer_function_list.remove([prod[0], k])
-                    Logger.set_debug(__name__, f"[{prod[0]}, {k.name} removed]")
-    else:
-        main_function_list, main_parent_dict = question_answer.get_children(main_fun)
-        # derived = childs_inheritance(main_fun)
-        # if derived:
-        #     main_function_list = main_function_list.union(derived[0])
-        #     main_parent_dict.update(derived[1])
-
-    Logger.set_debug(__name__, f"main function list: {main_function_list}")
-    Logger.set_debug(__name__, f"consumer function list: {xml_consumer_function_list}")
-    Logger.set_debug(__name__, f"producer function list: {xml_producer_function_list}")
-
-    main_consumer_list = util.check_get_child_flows(main_function_list, xml_consumer_function_list)
-    main_producer_list = util.check_get_child_flows(main_function_list, xml_producer_function_list)
-
-    ext_prod_fun_list, ext_producer_list, ext_prod_parent_dict = util.get_external_flow_with_level(
-        main_consumer_list, main_function_list, main_fun, xml_producer_function_list, diagram_level)
-
-    ext_cons_fun_list, ext_consumer_list, ext_cons_parent_dict = util.get_external_flow_with_level(
-        main_producer_list, main_function_list, main_fun, xml_consumer_function_list, diagram_level)
-
-    new_function_list = main_function_list.union(ext_prod_fun_list).union(ext_cons_fun_list)
-    new_consumer_list = main_consumer_list + ext_consumer_list
-    new_producer_list = main_producer_list + ext_producer_list
-    new_parent_dict = {**main_parent_dict, **ext_cons_parent_dict, **ext_prod_parent_dict}
-
-    for function in new_function_list:
-        if main_parent and function.parent is main_parent:
-            function.parent = None
-        if function.child_list:
-            for j in function.child_list.copy():
-                if j not in new_function_list:
-                    function.child_list.remove(j)
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
-                                                           fun_elem_list=None,
-                                                           consumer_function_list=new_consumer_list,
-                                                           producer_function_list=new_producer_list,
-                                                           parent_child_dict=new_parent_dict,
-                                                           data_list=None,
-                                                           xml_type_list=xml_type_list,
-                                                           xml_attribute_list=xml_attribute_list)
-
-    Logger.set_info(__name__,
-                    f"Decomposition Diagram {diagram_function_str} generated")
-
-    return plantuml_text
+"""@defgroup diagram
+Jarvis diagram module
+"""
+# Libraries
+
+# Modules
+import plantuml_adapter
+from jarvis.query import question_answer
+from . import util
+from tools import Logger
+
+
+def show_function_context(diagram_function_str, xml_function_list, xml_consumer_function_list,
+                          xml_producer_function_list, xml_data_list, xml_attribute_list,
+                          xml_type_list):
+
+    new_function_list, new_consumer_list, new_producer_list = util.get_function_context_lists(
+        diagram_function_str,
+        xml_function_list,
+        xml_consumer_function_list,
+        xml_producer_function_list)
+
+    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
+                                                           fun_elem_list=None,
+                                                           consumer_function_list=new_consumer_list,
+                                                           producer_function_list=new_producer_list,
+                                                           parent_child_dict={},
+                                                           data_list=xml_data_list,
+                                                           xml_type_list=xml_type_list,
+                                                           xml_attribute_list=xml_attribute_list)
+
+    Logger.set_info(__name__,
+                    f"Context Diagram {diagram_function_str} generated")
+
+    return plantuml_text
+
+
+# TODO: Clean-up once inheritance has been validated (Create method for Function and others
+#  objects?)
+def show_function_decomposition(diagram_function_str, xml_function_list, xml_consumer_function_list,
+                                xml_producer_function_list, xml_attribute_list, xml_type_list,
+                                diagram_level=None):
+    """Create necessary lists then returns plantuml text for decomposition of function"""
+    main_fun = question_answer.check_get_object(diagram_function_str, **{'xml_function_list': xml_function_list})
+
+    if not main_fun:
+        return
+
+    main_parent = main_fun.parent
+
+    if diagram_level:
+        full_fun_list, _ = question_answer.get_children(main_fun)
+        main_function_list, main_parent_dict = question_answer.get_children(main_fun, level=diagram_level)
+        # derived = childs_inheritance(main_fun, level=diagram_level)
+        # if derived:
+        #     main_function_list = main_function_list.union(derived[0])
+        #     main_parent_dict.update(derived[1])
+
+        # Remove functions and flows that are not in the diagram level
+        for k in full_fun_list.symmetric_difference(main_function_list):
+            Logger.set_debug(__name__, f"{k.name} not in diagram level {diagram_level}")
+            for cons in xml_consumer_function_list.copy():
+                if k in cons:
+                    xml_consumer_function_list.remove([cons[0], k])
+                    Logger.set_debug(__name__, f"[{cons[0]}, {k.name} removed]")
+
+            for prod in xml_producer_function_list.copy():
+                if k in prod:
+                    xml_producer_function_list.remove([prod[0], k])
+                    Logger.set_debug(__name__, f"[{prod[0]}, {k.name} removed]")
+    else:
+        main_function_list, main_parent_dict = question_answer.get_children(main_fun)
+        # derived = childs_inheritance(main_fun)
+        # if derived:
+        #     main_function_list = main_function_list.union(derived[0])
+        #     main_parent_dict.update(derived[1])
+
+    Logger.set_debug(__name__, f"main function list: {main_function_list}")
+    Logger.set_debug(__name__, f"consumer function list: {xml_consumer_function_list}")
+    Logger.set_debug(__name__, f"producer function list: {xml_producer_function_list}")
+
+    main_consumer_list = util.check_get_flows(main_function_list, xml_consumer_function_list)
+    main_producer_list = util.check_get_flows(main_function_list, xml_producer_function_list)
+
+    ext_prod_fun_list, ext_producer_list, ext_prod_parent_dict = util.get_external_flow_with_level(
+        main_consumer_list, main_function_list, main_fun, xml_producer_function_list, diagram_level)
+
+    ext_cons_fun_list, ext_consumer_list, ext_cons_parent_dict = util.get_external_flow_with_level(
+        main_producer_list, main_function_list, main_fun, xml_consumer_function_list, diagram_level)
+
+    new_function_list = main_function_list.union(ext_prod_fun_list).union(ext_cons_fun_list)
+    new_consumer_list = main_consumer_list + ext_consumer_list
+    new_producer_list = main_producer_list + ext_producer_list
+    new_parent_dict = {**main_parent_dict, **ext_cons_parent_dict, **ext_prod_parent_dict}
+
+    for function in new_function_list:
+        if main_parent and function.parent is main_parent:
+            function.parent = None
+        if function.child_list:
+            for j in function.child_list.copy():
+                if j not in new_function_list:
+                    function.child_list.remove(j)
+
+    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
+                                                           fun_elem_list=None,
+                                                           consumer_function_list=new_consumer_list,
+                                                           producer_function_list=new_producer_list,
+                                                           parent_child_dict=new_parent_dict,
+                                                           data_list=None,
+                                                           xml_type_list=xml_type_list,
+                                                           xml_attribute_list=xml_attribute_list)
+
+    Logger.set_info(__name__,
+                    f"Decomposition Diagram {diagram_function_str} generated")
+
+    return plantuml_text
```

### Comparing `jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_farch.py` & `jarvis4se-1.4.0/src/jarvis/diagram/diagram_generator_farch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,216 +1,222 @@
-"""@defgroup diagram
-Jarvis diagram module
-"""
-# Libraries
-
-# Modules
-import plantuml_adapter
-from jarvis import question_answer
-from . import util
-from tools import Logger
-
-
-def show_fun_elem_function(fun_elem_str, xml_fun_elem_list, xml_function_list,
-                           xml_consumer_function_list, xml_producer_function_list, xml_attribute_list):
-    """@ingroup diagram
-    @anchor show_fun_elem_function
-    Creates lists with desired objects for functional element functions allocation, send them to plantuml_adapter.py
-    and returns plantuml text
-    @param[in] fun_elem_str: name of the functional element
-    @param[in] xml_fun_elem_list: list of all functional elements
-    @param[in] xml_function_list: list of all functions
-    @param[in] xml_consumer_function_list: list of [[flow name, consumer function]]
-    @param[in] xml_producer_function_list: list of [[flow name, producer function]]
-    @param[in] xml_attribute_list: list of all attributes
-    @return plantuml text
-    """
-    plantuml_text = None
-
-    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        return plantuml_text
-
-    if not main_fun_elem.allocated_function_list:
-        Logger.set_info(__name__,
-                        f"No function allocated to {main_fun_elem.name} (no display)")
-        return plantuml_text
-
-    main_fun_elem.parent = None
-    main_fun_elem.child_list.clear()
-
-    # Get allocated main function to main_fun_elem
-    new_function_list = {f for f in xml_function_list
-                         if f.id in main_fun_elem.allocated_function_list and f.parent is None}
-
-    if not new_function_list:
-        Logger.set_info(__name__,
-                        f"No main function allocated to {main_fun_elem.name} (no display)")
-        return plantuml_text
-
-    external_function_list, new_consumer_list, new_producer_list = \
-        util.get_cons_prod_from_allocated_functions(new_function_list,
-                                                    xml_producer_function_list,
-                                                    xml_consumer_function_list,
-                                                    False)
-
-    Logger.set_debug(__name__, f'list of allocated functions to element: {new_function_list}')
-    Logger.set_debug(__name__, f'list of external functions to element: {external_function_list}')
-    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
-    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
-                                                           fun_elem_list=None,
-                                                           consumer_function_list=new_consumer_list,
-                                                           producer_function_list=new_producer_list,
-                                                           parent_child_dict={},
-                                                           data_list=None,
-                                                           xml_type_list=None,
-                                                           xml_attribute_list=xml_attribute_list)
-
-    Logger.set_info(__name__,
-                    f"Function Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def show_fun_elem_context(fun_elem_str, xml_fun_elem_list, xml_function_list,
-                          xml_consumer_function_list, xml_producer_function_list,
-                          xml_attribute_list, xml_fun_inter_list, xml_data_list):
-    """@ingroup diagram
-    @anchor show_fun_elem_context
-    Creates lists with desired objects for functional element context, send them to plantuml_adapter.py
-    and returns plantuml text
-    @param[in] fun_elem_str: name of the functional element
-    @param[in] xml_fun_elem_list: list of all functional elements
-    @param[in] xml_function_list: list of all functions
-    @param[in] xml_consumer_function_list: list of [[flow name, consumer function]]
-    @param[in] xml_producer_function_list: list of [[flow name, producer function]]
-    @param[in] xml_attribute_list: list of all attributes
-    @param[in] xml_fun_inter_list: list of all functional interfaces
-    @param[in] xml_data_list: list of all data
-    @return plantuml text
-    """
-    plantuml_text = None
-
-    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        return plantuml_text
-
-    # Get allocated main function to main_fun_elem
-    allocated_function_list = {f for f in xml_function_list
-                               if f.id in main_fun_elem.allocated_function_list and f.parent is None}
-
-    new_function_list, new_consumer_list, new_producer_list = util.get_allocated_function_context_lists(
-        allocated_function_list,
-        xml_consumer_function_list,
-        xml_producer_function_list)
-
-    Logger.set_debug(__name__, f'list of functions: {new_function_list}')
-    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
-    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
-
-    # TODO : fun_elem_inter_list to be removed (not used anymore)
-    fun_elem_list, interface_list, fun_elem_inter_list = util.get_fun_inter_for_fun_elem_context(
-        main_fun_elem, xml_fun_inter_list, xml_fun_elem_list)
-
-    Logger.set_debug(__name__, f'list of functional element: {fun_elem_list}')
-    Logger.set_debug(__name__, f'list of functional interfaces: {interface_list}')
-
-    for fun in new_function_list:
-        for elem in xml_fun_elem_list:
-            if any(z == fun.id for z in elem.allocated_function_list) and elem not in fun_elem_list:
-                fun_elem_list.add(elem)
-
-    for elem in fun_elem_list.copy():
-        for str_id in elem.allocated_function_list.copy():
-            if str_id not in [i.id for i in new_function_list]:
-                elem.allocated_function_list.remove(str_id)
-        if any(a == elem for a in main_fun_elem.child_list):
-            fun_elem_list.remove(elem)
-
-    # Remove parent for main functional element : we do not care about it in context diagram
-    if main_fun_elem.parent:
-        fun_elem_list.remove(main_fun_elem.parent)
-
-    plantuml_text = plantuml_adapter.get_fun_elem_context_diagram(new_function_list,
-                                                                  new_consumer_list,
-                                                                  new_producer_list,
-                                                                  xml_data_list,
-                                                                  xml_attribute_list,
-                                                                  fun_elem_list,
-                                                                  interface_list)
-
-    Logger.set_info(__name__,
-                    f"Context Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def show_fun_elem_decomposition(fun_elem_str, xml_function_list, xml_consumer_function_list,
-                                xml_producer_function_list, xml_fun_elem_list, xml_attribute_list,
-                                xml_data_list, xml_fun_inter_list, diagram_level=None):
-    """@ingroup diagram
-    @anchor show_fun_elem_context
-    Creates lists with desired objects for functional element decomposition, send them to plantuml_adapter.py
-    and returns plantuml text
-    @param[in] fun_elem_str: name of the functional element
-    @param[in] xml_fun_elem_list: list of all functional elements
-    @param[in] xml_function_list: list of all functions
-    @param[in] xml_consumer_function_list: list of [[flow name, consumer function]]
-    @param[in] xml_producer_function_list: list of [[flow name, producer function]]
-    @param[in] xml_attribute_list: list of all attributes
-    @param[in] xml_fun_inter_list: list of all functional interfaces
-    @param[in] xml_data_list: list of all data
-    @return plantuml text
-    """
-    plantuml_text = None
-
-    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        return plantuml_text
-
-    main_fun_elem.parent = None
-
-    if diagram_level:
-        xml_function_list, xml_fun_elem_list = util.filter_fun_elem_with_level(main_fun_elem,
-                                                                               diagram_level,
-                                                                               xml_function_list,
-                                                                               xml_fun_elem_list)
-
-    allocated_function_list = set()
-    if main_fun_elem.child_list != set():
-        util.get_level_0_function(main_fun_elem, xml_function_list, allocated_function_list)
-
-    if allocated_function_list != set():
-        external_function_list, new_consumer_list, new_producer_list = \
-            util.get_cons_prod_from_allocated_functions(
-                allocated_function_list,
-                xml_producer_function_list,
-                xml_consumer_function_list)
-
-        for fun in external_function_list:
-            for child in fun.child_list.copy():
-                if not any(t == child for t in external_function_list):
-                    fun.child_list.remove(child)
-    else:
-        external_function_list, xml_fun_elem_list = set(), set()
-        new_consumer_list, new_producer_list = [], []
-
-    Logger.set_debug(__name__, f'list of allocated functions: {allocated_function_list}')
-    Logger.set_debug(__name__, f'list of external functions: {external_function_list}')
-    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
-    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
-    Logger.set_debug(__name__, f'list of functional interfaces: {xml_fun_inter_list}')
-
-    plantuml_text = plantuml_adapter.get_fun_elem_decomposition(main_fun_elem, xml_fun_elem_list,
-                                                                allocated_function_list,
-                                                                new_consumer_list,
-                                                                new_producer_list,
-                                                                external_function_list,
-                                                                xml_attribute_list,
-                                                                xml_data_list,
-                                                                xml_fun_inter_list)
-    Logger.set_info(__name__,
-                    f"Decomposition Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
+"""@defgroup diagram
+Jarvis diagram module
+"""
+# Libraries
+
+# Modules
+import plantuml_adapter
+from jarvis.query import question_answer
+from . import util
+from tools import Logger
+
+
+def show_fun_elem_function(fun_elem_str, xml_fun_elem_list, xml_function_list,
+                           xml_consumer_function_list, xml_producer_function_list, xml_attribute_list):
+    """@ingroup diagram
+    @anchor show_fun_elem_function
+    Creates lists with desired objects for functional element functions allocation, send them to plantuml_adapter.py
+    and returns plantuml text
+    @param[in] fun_elem_str: name of the functional element
+    @param[in] xml_fun_elem_list: list of all functional elements
+    @param[in] xml_function_list: list of all functions
+    @param[in] xml_consumer_function_list: list of [[flow name, consumer function]]
+    @param[in] xml_producer_function_list: list of [[flow name, producer function]]
+    @param[in] xml_attribute_list: list of all attributes
+    @return plantuml text
+    """
+    plantuml_text = None
+
+    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
+    if not main_fun_elem:
+        return plantuml_text
+
+    if not main_fun_elem.allocated_function_list:
+        Logger.set_info(__name__,
+                        f"No function allocated to {main_fun_elem.name} (no display)")
+        return plantuml_text
+
+    main_fun_elem.parent = None
+    main_fun_elem.child_list.clear()
+
+    # Get allocated main function to main_fun_elem
+    new_function_list = {f for f in xml_function_list
+                         if f.id in main_fun_elem.allocated_function_list and f.parent is None}
+
+    if not new_function_list:
+        Logger.set_info(__name__,
+                        f"No main function allocated to {main_fun_elem.name} (no display)")
+        return plantuml_text
+
+    external_function_list, new_consumer_list, new_producer_list = \
+        util.get_cons_prod_from_allocated_functions(new_function_list,
+                                                    xml_producer_function_list,
+                                                    xml_consumer_function_list,
+                                                    False)
+
+    Logger.set_debug(__name__, f'list of allocated functions to element: {new_function_list}')
+    Logger.set_debug(__name__, f'list of external functions to element: {external_function_list}')
+    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
+    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
+
+    plantuml_text = plantuml_adapter.get_function_diagrams(function_list=new_function_list,
+                                                           fun_elem_list=None,
+                                                           consumer_function_list=new_consumer_list,
+                                                           producer_function_list=new_producer_list,
+                                                           parent_child_dict={},
+                                                           data_list=None,
+                                                           xml_type_list=None,
+                                                           xml_attribute_list=xml_attribute_list)
+
+    Logger.set_info(__name__,
+                    f"Function Diagram for {fun_elem_str} generated")
+
+    return plantuml_text
+
+
+def show_fun_elem_context(fun_elem_str, xml_fun_elem_list, xml_function_list,
+                          xml_consumer_function_list, xml_producer_function_list,
+                          xml_attribute_list, xml_fun_inter_list, xml_data_list):
+    """@ingroup diagram
+    @anchor show_fun_elem_context
+    Creates lists with desired objects for functional element context, send them to plantuml_adapter.py
+    and returns plantuml text
+    @param[in] fun_elem_str: name of the functional element
+    @param[in] xml_fun_elem_list: list of all functional elements
+    @param[in] xml_function_list: list of all functions
+    @param[in] xml_consumer_function_list: list of [[flow name, consumer function]]
+    @param[in] xml_producer_function_list: list of [[flow name, producer function]]
+    @param[in] xml_attribute_list: list of all attributes
+    @param[in] xml_fun_inter_list: list of all functional interfaces
+    @param[in] xml_data_list: list of all data
+    @return plantuml text
+    """
+    plantuml_text = None
+
+    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
+    if not main_fun_elem:
+        return plantuml_text
+
+    # Get allocated main function to main_fun_elem
+    allocated_function_list = {f for f in xml_function_list
+                               if f.id in main_fun_elem.allocated_function_list and f.parent is None}
+
+    new_function_list, new_consumer_list, new_producer_list = util.get_allocated_function_context_lists(
+        allocated_function_list,
+        xml_consumer_function_list,
+        xml_producer_function_list)
+
+    Logger.set_debug(__name__, f'list of functions: {new_function_list}')
+    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
+    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
+
+    # TODO : fun_elem_inter_list to be removed (not used anymore)
+    fun_elem_list, interface_list, fun_elem_inter_list = util.get_fun_inter_for_fun_elem_context(
+        main_fun_elem, xml_fun_inter_list, xml_fun_elem_list)
+
+    Logger.set_debug(__name__, f'list of functional element: {fun_elem_list}')
+    Logger.set_debug(__name__, f'list of functional interfaces: {interface_list}')
+
+    for fun in new_function_list:
+        for elem in xml_fun_elem_list:
+            if any(z == fun.id for z in elem.allocated_function_list) and elem not in fun_elem_list:
+                fun_elem_list.add(elem)
+
+    for elem in fun_elem_list.copy():
+        for str_id in elem.allocated_function_list.copy():
+            if str_id not in [i.id for i in new_function_list]:
+                elem.allocated_function_list.remove(str_id)
+        if any(a == elem for a in main_fun_elem.child_list):
+            fun_elem_list.remove(elem)
+
+    # Remove parent for main functional element : we do not care about it in context diagram
+    if main_fun_elem.parent:
+        fun_elem_list.remove(main_fun_elem.parent)
+
+    plantuml_text = plantuml_adapter.get_fun_elem_context_diagram(new_function_list,
+                                                                  new_consumer_list,
+                                                                  new_producer_list,
+                                                                  xml_data_list,
+                                                                  xml_attribute_list,
+                                                                  fun_elem_list,
+                                                                  interface_list)
+
+    Logger.set_info(__name__,
+                    f"Context Diagram for {fun_elem_str} generated")
+
+    return plantuml_text
+
+
+def show_fun_elem_decomposition(fun_elem_str, xml_function_list, xml_consumer_function_list,
+                                xml_producer_function_list, xml_fun_elem_list, xml_attribute_list,
+                                xml_data_list, xml_fun_inter_list, diagram_level=None):
+    """@ingroup diagram
+    @anchor show_fun_elem_decomposition
+    Creates lists with desired objects for functional element decomposition, send them to plantuml_adapter.py
+    and returns plantuml text
+    @param[in] fun_elem_str: name of the functional element
+    @param[in] xml_fun_elem_list: list of all functional elements
+    @param[in] xml_function_list: list of all functions
+    @param[in] xml_consumer_function_list: list of [[flow name, consumer function]]
+    @param[in] xml_producer_function_list: list of [[flow name, producer function]]
+    @param[in] xml_attribute_list: list of all attributes
+    @param[in] xml_fun_inter_list: list of all functional interfaces
+    @param[in] xml_data_list: list of all data
+    @return plantuml text
+    """
+    plantuml_text = None
+
+    main_fun_elem = question_answer.check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
+    if not main_fun_elem:
+        return plantuml_text
+
+    main_fun_elem.parent = None
+
+    if diagram_level:
+        xml_function_list, xml_fun_elem_list = util.filter_fun_elem_with_level(main_fun_elem,
+                                                                               diagram_level,
+                                                                               xml_function_list,
+                                                                               xml_fun_elem_list)
+
+    allocated_function_list = set()
+    if main_fun_elem.child_list != set():
+        util.get_level_0_function(main_fun_elem, xml_function_list, allocated_function_list)
+
+    if allocated_function_list != set():
+        external_function_list, new_consumer_list, new_producer_list = \
+            util.get_cons_prod_from_allocated_functions(
+                allocated_function_list,
+                xml_producer_function_list,
+                xml_consumer_function_list)
+
+        if external_function_list:
+            for fun in external_function_list:
+                for child in fun.child_list.copy():
+                    if not any(t == child for t in external_function_list):
+                        fun.child_list.remove(child)
+        else:
+            xml_fun_elem_list = set()
+            xml_fun_elem_list.add(main_fun_elem)
+            for child in main_fun_elem.child_list:
+                xml_fun_elem_list.add(child)
+    else:
+        external_function_list, xml_fun_elem_list = set(), set()
+        new_consumer_list, new_producer_list = [], []
+
+    Logger.set_debug(__name__, f'list of allocated functions: {allocated_function_list}')
+    Logger.set_debug(__name__, f'list of external functions: {external_function_list}')
+    Logger.set_debug(__name__, f'list of consumer list: {new_consumer_list}')
+    Logger.set_debug(__name__, f'list of producer list: {new_producer_list}')
+    Logger.set_debug(__name__, f'list of functional interfaces: {xml_fun_inter_list}')
+
+    plantuml_text = plantuml_adapter.get_fun_elem_decomposition(main_fun_elem, xml_fun_elem_list,
+                                                                allocated_function_list,
+                                                                new_consumer_list,
+                                                                new_producer_list,
+                                                                external_function_list,
+                                                                xml_attribute_list,
+                                                                xml_data_list,
+                                                                xml_fun_inter_list)
+    Logger.set_info(__name__,
+                    f"Decomposition Diagram for {fun_elem_str} generated")
+
+    return plantuml_text
```

### Comparing `jarvis4se-1.3.5/src/jarvis/diagram/util.py` & `jarvis4se-1.4.0/src/jarvis/diagram/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,439 +1,445 @@
-"""@defgroup diagram
-Jarvis diagram module
-"""
-# Modules
-from jarvis import question_answer
-from tools import Logger
-
-
-def get_cons_or_prod_paired(function_list, xml_flow_list, xml_opposite_flow_list):
-    """Get flow list if opposite flow is existing: e.g. if flow A is consumed and produced by
-    function within function_list => Add it"""
-    new_flow_list = []
-
-    for func in function_list:
-        # Flow = [Data_name, Function]
-        for flow in xml_flow_list:
-            if func in flow and flow not in new_flow_list:
-                # Oppo = [Data_name, Function]
-                for oppo in xml_opposite_flow_list:
-                    if oppo[0] == flow[0] and oppo[1] in function_list:
-                        new_flow_list.append(flow)
-                        break
-
-    return new_flow_list
-
-
-def get_cons_prod_from_allocated_functions(allocated_function_list,
-                                           xml_producer_function_list,
-                                           xml_consumer_function_list,
-                                           with_external_functions=True):
-    """Get consumers/producers from function's allocated to main_fun_elem (and its descendant)"""
-    new_producer_list = []
-    new_consumer_list = []
-    for allocated_function in allocated_function_list:
-        allocated_function.child_list.clear()
-        allocated_function.parent = None
-        for elem in xml_producer_function_list:
-            if allocated_function in elem:
-                new_producer_list.append(elem)
-        for elem in xml_consumer_function_list:
-            if allocated_function in elem:
-                new_consumer_list.append(elem)
-
-    if with_external_functions:
-        external_function_list, new_consumer_list, new_producer_list = get_ext_cons_prod(
-            new_producer_list,
-            new_consumer_list,
-            xml_producer_function_list,
-            xml_consumer_function_list)
-    else:
-        external_function_list = None
-
-    return external_function_list, new_consumer_list, new_producer_list
-
-
-def get_ext_cons_prod(producer_list, consumer_list, xml_producer_function_list,
-                      xml_consumer_function_list):
-    """Get external cons/prod associated to main_fun_elem allocated functions"""
-    external_function_list = set()
-    for elem in consumer_list:
-        if not any(elem[0] in s for s in producer_list):
-            for prod in xml_producer_function_list:
-                if prod[0] == elem[0] and prod[1].parent is None:
-                    external_function_list.add(prod[1])
-                    if prod not in producer_list:
-                        producer_list.append(prod)
-
-    for elem in producer_list:
-        if not any(elem[0] in s for s in consumer_list):
-            for cons in xml_consumer_function_list:
-                if cons[0] == elem[0] and cons[1].parent is None:
-                    external_function_list.add(cons[1])
-                    if cons not in consumer_list:
-                        consumer_list.append(cons)
-
-    return external_function_list, consumer_list, producer_list
-
-
-def get_allocated_function_context_lists(allocated_function_list,
-                                         xml_consumer_function_list,
-                                         xml_producer_function_list):
-    """For each function within allocated_function_list, asks the context of the function then
-    adds returned list from show_function_context() to current lists"""
-    new_function_list = set()
-    new_consumer_list = []
-    new_producer_list = []
-
-    for fun in allocated_function_list:
-        fun_function_list, fun_consumer_list, fun_producer_list = get_function_context_lists(
-            fun.name,
-            allocated_function_list,
-            xml_consumer_function_list,
-            xml_producer_function_list)
-
-        for fun_function in fun_function_list:
-            new_function_list.add(fun_function)
-
-        for fun_consumer in fun_consumer_list:
-            if fun_consumer not in new_consumer_list:
-                new_consumer_list.append(fun_consumer)
-
-        for fun_producer in fun_producer_list:
-            if fun_producer not in new_producer_list:
-                new_producer_list.append(fun_producer)
-
-    return new_function_list, new_consumer_list, new_producer_list
-
-
-def get_function_context_lists(diagram_function_str, xml_function_list, xml_consumer_function_list,
-                               xml_producer_function_list):
-    """Create necessary lists then returns plantuml text for context of function"""
-    new_function_list = set()
-    new_producer_list = []
-    new_consumer_list = []
-    main_function = None
-
-    for fun in xml_function_list:
-        if diagram_function_str in (fun.name, fun.alias):
-            new_function_list.add(fun)
-            main_function = fun
-            for xml_producer_flow, xml_producer in xml_producer_function_list:
-                if fun == xml_producer:
-                    check = False
-                    for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
-                        if xml_producer_flow == xml_consumer_flow:
-                            if xml_consumer.parent is None:
-                                current_func, current_dict = question_answer.get_children(fun)
-                                parent_check = question_answer.check_parentality(xml_consumer, main_function)
-                                if xml_consumer not in current_func and parent_check is False:
-                                    new_consumer_list.append([xml_producer_flow, xml_consumer])
-                                    new_function_list.add(xml_consumer)
-                                    check = True
-                            elif main_function.parent == xml_consumer.parent and xml_consumer != main_function:
-                                new_consumer_list.append([xml_consumer_flow, xml_consumer])
-                                new_function_list.add(xml_consumer)
-                                check = True
-                    if check:
-                        if [xml_producer_flow, xml_producer] not in new_producer_list:
-                            new_producer_list.append([xml_producer_flow, xml_producer])
-
-                    if not any(xml_producer_flow in s for s in xml_consumer_function_list):
-                        if [xml_producer_flow, xml_producer] not in new_producer_list:
-                            new_producer_list.append([xml_producer_flow, xml_producer])
-
-    if main_function is not None:
-        for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
-            if xml_consumer == main_function:
-                check = False
-                for xml_producer_flow, producer in xml_producer_function_list:
-                    if xml_producer_flow == xml_consumer_flow:
-                        if producer.parent is None:
-                            current_func, current_dict = question_answer.get_children(producer)
-                            if main_function not in current_func:
-                                new_producer_list.append([xml_producer_flow, producer])
-                                new_function_list.add(producer)
-                                check = True
-                        elif main_function.parent == producer.parent and producer != main_function:
-                            new_producer_list.append([xml_producer_flow, producer])
-                            new_function_list.add(producer)
-                            check = True
-                if check:
-                    if [xml_consumer_flow, xml_consumer] not in new_consumer_list:
-                        new_consumer_list.append([xml_consumer_flow, xml_consumer])
-
-                if not any(xml_consumer_flow in s for s in xml_producer_function_list):
-                    if [xml_consumer_flow, xml_consumer] not in new_consumer_list:
-                        new_consumer_list.append([xml_consumer_flow, xml_consumer])
-
-    for f in new_function_list:
-        f.child_list.clear()
-
-    return new_function_list, new_consumer_list, new_producer_list
-
-
-def get_fun_inter_for_fun_elem_context(main_fun_elem, xml_fun_inter_list, xml_fun_elem_list):
-    """Get functional interfaces and associated functional elements"""
-    fun_elem_list = set()
-    interface_list = set()
-    fun_elem_inter_list = []
-
-    # Add main_fun_elem to filtered fun_elem_list and remove it from xml_fun_elem_list
-    fun_elem_list.add(main_fun_elem)
-    xml_fun_elem_list.remove(main_fun_elem)
-
-    # Get exposed interfaces of fun_elem
-    for interface in xml_fun_inter_list:
-        if any(i == interface.id for i in main_fun_elem.exposed_interface_list):
-            interface_list.add(interface)
-
-    # Get fun_elem pair for fun_inter
-    for fun_inter in interface_list:
-        for fun_elem in xml_fun_elem_list:
-            if any(i == fun_inter.id for i in fun_elem.exposed_interface_list):
-                if get_highest_fun_elem_exposing_fun_inter(fun_inter, fun_elem) and \
-                        question_answer.check_not_family(main_fun_elem, fun_elem):
-                    fun_elem_list.add(fun_elem)
-                    if [main_fun_elem, fun_elem, fun_inter] not in fun_elem_inter_list:
-                        fun_elem_inter_list.append([main_fun_elem, fun_elem, fun_inter])
-
-    return fun_elem_list, interface_list, fun_elem_inter_list
-
-
-def get_highest_fun_elem_exposing_fun_inter(fun_inter, fun_elem):
-    """Returns True if it's highest fun_elem exposing fun_inter"""
-    check = False
-    if not fun_elem.parent:
-        check = True
-    elif not any(a == fun_inter.id for a in fun_elem.parent.exposed_interface_list):
-        check = True
-
-    return check
-
-
-def filter_fun_elem_with_level(main_fun_elem, diagram_level, xml_function_list, xml_fun_elem_list):
-    """Clean unwanted fun_elem and functions from xml_lists then returns them"""
-    main_fun_elem_list, _ = question_answer.get_children(main_fun_elem, level=diagram_level)
-    # Remove (child) elements from xml lists that are below the level asked
-    for unwanted_fun_elem in xml_fun_elem_list.symmetric_difference(main_fun_elem_list):
-        if not question_answer.check_not_family(unwanted_fun_elem, main_fun_elem):
-            for fun in xml_function_list.copy():
-                if fun.id in unwanted_fun_elem.allocated_function_list:
-                    xml_function_list.remove(fun)
-            xml_fun_elem_list.remove(unwanted_fun_elem)
-    # Remove (child) elements from external fun_elem (main_fun_elem point of view)
-    for unwanted_fun_elem in xml_fun_elem_list.symmetric_difference(main_fun_elem_list):
-        if question_answer.check_not_family(unwanted_fun_elem, main_fun_elem) and \
-                unwanted_fun_elem.parent is None:
-            curr_fun_elem_list, _ = question_answer.get_children(unwanted_fun_elem, level=diagram_level)
-            for un_fun_elem in xml_fun_elem_list.symmetric_difference(curr_fun_elem_list):
-                if not question_answer.check_not_family(unwanted_fun_elem, un_fun_elem):
-                    xml_fun_elem_list.remove(un_fun_elem)
-
-    return xml_function_list, xml_fun_elem_list
-
-
-def get_level_0_function(fun_elem, function_list, level_0_function_list):
-    """Recursively get functions allocated to main_fun_elem and its descendant"""
-    for function_id in fun_elem.allocated_function_list:
-        for function in function_list:
-            if function.id == function_id and function not in level_0_function_list:
-                if fun_elem.child_list == set() is True:
-                    level_0_function_list.add(function)
-                else:
-                    # Check if any function child is allocated to any element child
-                    function_child_id_list = [elem.id for elem in function.child_list]
-                    allocated_function_id_list = []
-                    for fun_elem_child in fun_elem.child_list:
-                        for allocated_function_id in fun_elem_child.allocated_function_list:
-                            allocated_function_id_list.append(allocated_function_id)
-
-                    if not any(fid in function_child_id_list for fid in allocated_function_id_list):
-                        # Check function parent
-                        if function.parent is None:
-                            level_0_function_list.add(function)
-                        else:
-                            if function.parent.id not in fun_elem.allocated_function_list:
-                                level_0_function_list.add(function)
-
-    for child in fun_elem.child_list:
-        get_level_0_function(child, function_list, level_0_function_list)
-
-
-def get_object_list_from_view(obj_str, xml_obj_list, xml_view_list):
-    """Returns current object's list by checking view"""
-    filtered_item_list = filter_allocated_item_from_view(xml_obj_list, xml_view_list)
-
-    if len(xml_obj_list) == len(filtered_item_list):
-        return xml_obj_list
-
-    if isinstance(obj_str, str):
-        for obj in xml_obj_list:
-            if obj_str in (obj.name, obj.alias) and not any(item == obj for item in filtered_item_list):
-                filtered_item_list.append(obj)
-    elif isinstance(obj_str, list):
-        for object_name in obj_str:
-            for obj in xml_obj_list:
-                if object_name in (obj.name, obj.alias) and \
-                        not any(item == obj for item in filtered_item_list):
-                    filtered_item_list.append(obj)
-
-    for new_obj in filtered_item_list:
-        child_list = set()
-        for child in new_obj.child_list:
-            if child in filtered_item_list:
-                child_list.add(child)
-        new_obj.child_list.clear()
-        new_obj.child_list = child_list
-
-    return filtered_item_list
-
-
-def filter_allocated_item_from_view(xml_item_list, xml_view_list):
-    """For a type of item from xml, check if a View is activated and if the item is in its
-    allocated item's list"""
-    if not any(j.activated for j in xml_view_list):
-        return xml_item_list
-
-    filtered_item_list = []
-    activated_view = ''
-    for view in xml_view_list:
-        if view.activated:
-            activated_view = view.name
-            for item in xml_item_list:
-                if item.id in view.allocated_item_list:
-                    filtered_item_list.append(item)
-
-    if not filtered_item_list:
-        Logger.set_debug(__name__,
-                         f"The requested elements are not allocated to the view {activated_view}")
-
-    return filtered_item_list
-
-
-def check_get_child_flows(function_list, xml_flow_list):
-    """Get flow_list associated with function_list and xml_flow_list"""
-    new_flow_list = []
-
-    for f in function_list:
-        for xml_flow, xml_function in xml_flow_list:
-            if f == xml_function:
-                if not xml_function.child_list:
-                    if [xml_flow, xml_function] not in new_flow_list:
-                        new_flow_list.append([xml_flow, xml_function])
-
-    return new_flow_list
-
-
-def get_external_flow_with_level(main_flow_list, main_function_list, main_fun, xml_flow_list,
-                                 level):
-    """Returns external functions list, flow lists and parent dict"""
-    ext_flow_fun_list = set()
-    ext_flow_list = []
-    ext_flow_parent_dict = {}
-    for flow, _ in main_flow_list:
-        for xml_flow, xml_fun in xml_flow_list:
-            if flow == xml_flow and xml_fun.parent == main_fun.parent:
-                ext_flow_fun_list.add(xml_fun)
-            elif flow == xml_flow and question_answer.check_not_family(main_fun, xml_fun) and \
-                    xml_fun.parent is None:
-                ext_flow_fun_list.add(xml_fun)
-            elif flow == xml_flow and not question_answer.check_parentality(xml_fun, main_fun) and \
-                    [xml_flow, xml_fun.parent] not in xml_flow_list:
-                ext_flow_fun_list.add(xml_fun)
-
-    for fun in ext_flow_fun_list.copy():
-        if fun.child_list:
-            function_list_dict = question_answer.get_children(fun, level=level)
-            ext_flow_fun_list.update(function_list_dict[0])
-            ext_flow_parent_dict.update(function_list_dict[1])
-
-    for flow, _ in main_flow_list:
-        for xml_flow, xml_fun in xml_flow_list:
-            if flow == xml_flow and xml_fun in ext_flow_fun_list and \
-                    xml_fun not in main_function_list:
-                # ext_flow_list.append([xml_flow, xml_fun])
-                if not xml_fun.child_list:
-                    if [xml_flow, xml_fun] not in ext_flow_list:
-                        ext_flow_list.append([xml_flow, xml_fun])
-                else:
-                    temp = []
-                    for k in xml_fun.child_list:
-                        temp.append([xml_flow, k])
-                    if not any(t in temp for t in xml_flow_list):
-                        if [xml_flow, xml_fun] not in ext_flow_list:
-                            ext_flow_list.append([xml_flow, xml_fun])
-
-    for fun in ext_flow_fun_list.copy():
-        if not any(a == fun for a in [i[1] for i in ext_flow_list]) and not fun.child_list:
-            ext_flow_fun_list.remove(fun)
-
-    for fun in ext_flow_fun_list.copy():
-        if not any(a == fun for a in [i[1] for i in ext_flow_list]) and \
-                not any(i in fun.child_list for i in ext_flow_fun_list) and \
-                fun != main_fun:
-            ext_flow_fun_list.remove(fun)
-
-    return ext_flow_fun_list, ext_flow_list, ext_flow_parent_dict
-
-
-def get_cons_prod_from_view_allocated_data(xml_data_list, xml_view_list, xml_consumer_function_list,
-                                           xml_producer_function_list, function_list):
-    """If a view is activated, returns filtered consumer/producer lists"""
-    new_function_list = []
-    new_consumer_list = []
-    new_producer_list = []
-    new_data_list = filter_allocated_item_from_view(xml_data_list, xml_view_list)
-
-    if len(new_data_list) == len(xml_data_list):
-        for prod in xml_producer_function_list:
-            if any(item == prod[1] for item in function_list):
-                new_producer_list.append(prod)
-                if prod[1] not in new_function_list:
-                    new_function_list.append(prod[1])
-
-        for cons in xml_consumer_function_list:
-            if any(item == cons[1] for item in function_list):
-                new_consumer_list.append(cons)
-                if cons[1] not in new_function_list:
-                    new_function_list.append(cons[1])
-
-    else:
-        for cons in xml_consumer_function_list:
-            if any(item.name == cons[0] for item in new_data_list) and \
-                    any(item == cons[1] for item in function_list):
-                new_consumer_list.append(cons)
-                if cons[1] not in new_function_list:
-                    new_function_list.append(cons[1])
-
-        for prod in xml_producer_function_list:
-            if any(item.name == prod[0] for item in new_data_list) and \
-                    any(item == prod[1] for item in function_list):
-                new_producer_list.append(prod)
-                if prod[1] not in new_function_list:
-                    new_function_list.append(prod[1])
-
-    return new_function_list, new_consumer_list, new_producer_list
-
-
-def get_parent_dict(element, element_list, parent_dict):
-    if element.parent:
-        parent_dict[element.id] = element.parent.id
-
-        if element.parent not in element_list:
-            element_list.add(element.parent)
-            element.parent.child_list.clear()
-
-        element.parent.add_child(element)
-
-        get_parent_dict(element.parent, element_list, parent_dict)
-
-
-def get_fun_elem_function_list(function, function_list, fun_elem):
-    if function.parent:
-        if function.parent.id in fun_elem.allocated_function_list:
-            get_fun_elem_function_list(function.parent, function_list, fun_elem)
-        else:
-            function_list.add(function)
-    else:
-        function_list.add(function)
+"""@defgroup diagram
+Jarvis diagram module
+"""
+# Modules
+from jarvis.query import question_answer
+from tools import Logger
+
+
+def get_cons_or_prod_paired(function_list, xml_flow_list, xml_opposite_flow_list):
+    """Get flow list if opposite flow is existing: e.g. if flow A is consumed and produced by
+    function within function_list => Add it"""
+    new_flow_list = []
+
+    for func in function_list:
+        # Flow = [Data_name, Function]
+        for flow in xml_flow_list:
+            if func in flow and flow not in new_flow_list:
+                # Oppo = [Data_name, Function]
+                for oppo in xml_opposite_flow_list:
+                    if oppo[0] == flow[0] and oppo[1] in function_list:
+                        new_flow_list.append(flow)
+                        break
+
+    return new_flow_list
+
+
+def get_cons_prod_from_allocated_functions(allocated_function_list,
+                                           xml_producer_function_list,
+                                           xml_consumer_function_list,
+                                           with_external_functions=True):
+    """Get consumers/producers from function's allocated to main_fun_elem (and its descendant)"""
+    new_producer_list = []
+    new_consumer_list = []
+    for allocated_function in allocated_function_list:
+        allocated_function.child_list.clear()
+        allocated_function.parent = None
+        for elem in xml_producer_function_list:
+            if allocated_function in elem:
+                new_producer_list.append(elem)
+        for elem in xml_consumer_function_list:
+            if allocated_function in elem:
+                new_consumer_list.append(elem)
+
+    if with_external_functions:
+        external_function_list, new_consumer_list, new_producer_list = get_ext_cons_prod(
+            new_producer_list,
+            new_consumer_list,
+            xml_producer_function_list,
+            xml_consumer_function_list)
+    else:
+        external_function_list = None
+
+    return external_function_list, new_consumer_list, new_producer_list
+
+
+def get_ext_cons_prod(producer_list, consumer_list, xml_producer_function_list,
+                      xml_consumer_function_list):
+    """Get external cons/prod associated to main_fun_elem allocated functions"""
+    external_function_list = set()
+    for elem in consumer_list:
+        if not any(elem[0] in s for s in producer_list):
+            for prod in xml_producer_function_list:
+                if prod[0] == elem[0] and prod[1].parent is None:
+                    external_function_list.add(prod[1])
+                    if prod not in producer_list:
+                        producer_list.append(prod)
+
+    for elem in producer_list:
+        if not any(elem[0] in s for s in consumer_list):
+            for cons in xml_consumer_function_list:
+                if cons[0] == elem[0] and cons[1].parent is None:
+                    external_function_list.add(cons[1])
+                    if cons not in consumer_list:
+                        consumer_list.append(cons)
+
+    return external_function_list, consumer_list, producer_list
+
+
+def get_allocated_function_context_lists(allocated_function_list,
+                                         xml_consumer_function_list,
+                                         xml_producer_function_list):
+    """For each function within allocated_function_list, asks the context of the function then
+    adds returned list from show_function_context() to current lists"""
+    new_function_list = set()
+    new_consumer_list = []
+    new_producer_list = []
+
+    for fun in allocated_function_list:
+        fun_function_list, fun_consumer_list, fun_producer_list = get_function_context_lists(
+            fun.name,
+            allocated_function_list,
+            xml_consumer_function_list,
+            xml_producer_function_list)
+
+        for fun_function in fun_function_list:
+            new_function_list.add(fun_function)
+
+        for fun_consumer in fun_consumer_list:
+            if fun_consumer not in new_consumer_list:
+                new_consumer_list.append(fun_consumer)
+
+        for fun_producer in fun_producer_list:
+            if fun_producer not in new_producer_list:
+                new_producer_list.append(fun_producer)
+
+    return new_function_list, new_consumer_list, new_producer_list
+
+
+def get_function_context_lists(diagram_function_str, xml_function_list, xml_consumer_function_list,
+                               xml_producer_function_list):
+    """Create necessary lists then returns plantuml text for context of function"""
+    new_function_list = set()
+    new_producer_list = []
+    new_consumer_list = []
+    main_function = None
+
+    for fun in xml_function_list:
+        if diagram_function_str in (fun.name, fun.alias):
+            new_function_list.add(fun)
+            main_function = fun
+            for xml_producer_flow, xml_producer in xml_producer_function_list:
+                if fun == xml_producer:
+                    check = False
+                    for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
+                        if xml_producer_flow == xml_consumer_flow:
+                            if xml_consumer.parent is None:
+                                current_func, current_dict = question_answer.get_children(fun)
+                                parent_check = question_answer.check_parentality(xml_consumer, main_function)
+                                if xml_consumer not in current_func and parent_check is False:
+                                    new_consumer_list.append([xml_producer_flow, xml_consumer])
+                                    new_function_list.add(xml_consumer)
+                                    check = True
+                            elif main_function.parent == xml_consumer.parent and xml_consumer != main_function:
+                                new_consumer_list.append([xml_consumer_flow, xml_consumer])
+                                new_function_list.add(xml_consumer)
+                                check = True
+                    if check:
+                        if [xml_producer_flow, xml_producer] not in new_producer_list:
+                            new_producer_list.append([xml_producer_flow, xml_producer])
+
+                    if not any(xml_producer_flow in s for s in xml_consumer_function_list):
+                        if [xml_producer_flow, xml_producer] not in new_producer_list:
+                            new_producer_list.append([xml_producer_flow, xml_producer])
+
+    if main_function is not None:
+        for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
+            if xml_consumer == main_function:
+                check = False
+                for xml_producer_flow, producer in xml_producer_function_list:
+                    if xml_producer_flow == xml_consumer_flow:
+                        if producer.parent is None:
+                            current_func, current_dict = question_answer.get_children(producer)
+                            if main_function not in current_func:
+                                new_producer_list.append([xml_producer_flow, producer])
+                                new_function_list.add(producer)
+                                check = True
+                        elif main_function.parent == producer.parent and producer != main_function:
+                            new_producer_list.append([xml_producer_flow, producer])
+                            new_function_list.add(producer)
+                            check = True
+                if check:
+                    if [xml_consumer_flow, xml_consumer] not in new_consumer_list:
+                        new_consumer_list.append([xml_consumer_flow, xml_consumer])
+
+                if not any(xml_consumer_flow in s for s in xml_producer_function_list):
+                    if [xml_consumer_flow, xml_consumer] not in new_consumer_list:
+                        new_consumer_list.append([xml_consumer_flow, xml_consumer])
+
+    for f in new_function_list:
+        f.child_list.clear()
+
+    return new_function_list, new_consumer_list, new_producer_list
+
+
+def get_fun_inter_for_fun_elem_context(main_fun_elem, xml_fun_inter_list, xml_fun_elem_list):
+    """Get functional interfaces and associated functional elements"""
+    fun_elem_list = set()
+    interface_list = set()
+    fun_elem_inter_list = []
+
+    # Add main_fun_elem to filtered fun_elem_list and remove it from xml_fun_elem_list
+    fun_elem_list.add(main_fun_elem)
+    xml_fun_elem_list.remove(main_fun_elem)
+
+    # Get exposed interfaces of fun_elem
+    for interface in xml_fun_inter_list:
+        if any(i == interface.id for i in main_fun_elem.exposed_interface_list):
+            interface_list.add(interface)
+
+    # Get fun_elem pair for fun_inter
+    for fun_inter in interface_list:
+        for fun_elem in xml_fun_elem_list:
+            if any(i == fun_inter.id for i in fun_elem.exposed_interface_list):
+                if get_highest_fun_elem_exposing_fun_inter(fun_inter, fun_elem) and \
+                        question_answer.check_not_family(main_fun_elem, fun_elem):
+                    fun_elem_list.add(fun_elem)
+                    if [main_fun_elem, fun_elem, fun_inter] not in fun_elem_inter_list:
+                        fun_elem_inter_list.append([main_fun_elem, fun_elem, fun_inter])
+
+    return fun_elem_list, interface_list, fun_elem_inter_list
+
+
+def get_highest_fun_elem_exposing_fun_inter(fun_inter, fun_elem):
+    """Returns True if it's highest fun_elem exposing fun_inter"""
+    check = False
+    if not fun_elem.parent:
+        check = True
+    elif not any(a == fun_inter.id for a in fun_elem.parent.exposed_interface_list):
+        check = True
+
+    return check
+
+
+def filter_fun_elem_with_level(main_fun_elem, diagram_level, xml_function_list, xml_fun_elem_list):
+    """Clean unwanted fun_elem and functions from xml_lists then returns them"""
+    main_fun_elem_list, _ = question_answer.get_children(main_fun_elem, level=diagram_level)
+    # Remove (child) elements from xml lists that are below the level asked
+    for unwanted_fun_elem in xml_fun_elem_list.symmetric_difference(main_fun_elem_list):
+        if not question_answer.check_not_family(unwanted_fun_elem, main_fun_elem):
+            for fun in xml_function_list.copy():
+                if fun.id in unwanted_fun_elem.allocated_function_list:
+                    xml_function_list.remove(fun)
+            xml_fun_elem_list.remove(unwanted_fun_elem)
+    # Remove (child) elements from external fun_elem (main_fun_elem point of view)
+    for unwanted_fun_elem in xml_fun_elem_list.symmetric_difference(main_fun_elem_list):
+        if question_answer.check_not_family(unwanted_fun_elem, main_fun_elem) and \
+                unwanted_fun_elem.parent is None:
+            curr_fun_elem_list, _ = question_answer.get_children(unwanted_fun_elem, level=diagram_level)
+            for un_fun_elem in xml_fun_elem_list.symmetric_difference(curr_fun_elem_list):
+                if not question_answer.check_not_family(unwanted_fun_elem, un_fun_elem):
+                    xml_fun_elem_list.remove(un_fun_elem)
+
+    return xml_function_list, xml_fun_elem_list
+
+
+def get_level_0_function(fun_elem, function_list, level_0_function_list):
+    """Recursively get functions allocated to main_fun_elem and its descendant"""
+    for function_id in fun_elem.allocated_function_list:
+        for function in function_list:
+            if function.id == function_id and function not in level_0_function_list:
+                if fun_elem.child_list == set() is True:
+                    level_0_function_list.add(function)
+                else:
+                    # Check if any function child is allocated to any element child
+                    function_child_id_list = [elem.id for elem in function.child_list]
+                    allocated_function_id_list = []
+                    for fun_elem_child in fun_elem.child_list:
+                        for allocated_function_id in fun_elem_child.allocated_function_list:
+                            allocated_function_id_list.append(allocated_function_id)
+
+                    if not any(fid in function_child_id_list for fid in allocated_function_id_list):
+                        # Check function parent
+                        if function.parent is None:
+                            level_0_function_list.add(function)
+                        else:
+                            if function.parent.id not in fun_elem.allocated_function_list:
+                                level_0_function_list.add(function)
+
+    for child in fun_elem.child_list:
+        get_level_0_function(child, function_list, level_0_function_list)
+
+
+def get_object_list_from_view(obj_str, xml_obj_list, xml_view_list):
+    """Returns current object's list by checking view"""
+    filtered_item_list = filter_allocated_item_from_view(xml_obj_list, xml_view_list)
+
+    if len(xml_obj_list) == len(filtered_item_list):
+        return xml_obj_list
+
+    if isinstance(obj_str, str):
+        for obj in xml_obj_list:
+            if obj_str in (obj.name, obj.alias) and not any(item == obj for item in filtered_item_list):
+                filtered_item_list.append(obj)
+    elif isinstance(obj_str, list):
+        for object_name in obj_str:
+            for obj in xml_obj_list:
+                if object_name in (obj.name, obj.alias) and \
+                        not any(item == obj for item in filtered_item_list):
+                    filtered_item_list.append(obj)
+
+    for new_obj in filtered_item_list:
+        child_list = set()
+        for child in new_obj.child_list:
+            if child in filtered_item_list:
+                child_list.add(child)
+        new_obj.child_list.clear()
+        new_obj.child_list = child_list
+
+    return filtered_item_list
+
+
+def filter_allocated_item_from_view(xml_item_list, xml_view_list):
+    """For a type of item from xml, check if a View is activated and if the item is in its
+    allocated item's list"""
+    if not any(j.activated for j in xml_view_list):
+        return xml_item_list
+
+    filtered_item_list = []
+    activated_view = ''
+    for view in xml_view_list:
+        if view.activated:
+            activated_view = view.name
+            for item in xml_item_list:
+                if item.id in view.allocated_item_list:
+                    filtered_item_list.append(item)
+
+    if not filtered_item_list:
+        Logger.set_debug(__name__,
+                         f"The requested elements are not allocated to the view {activated_view}")
+
+    return filtered_item_list
+
+
+def check_get_flows(function_list, xml_flow_list):
+    """Get flow_list associated with function_list and xml_flow_list"""
+    new_flow_list = []
+
+    for function in function_list:
+        for xml_flow, xml_function in xml_flow_list:
+            if function == xml_function:
+                if [xml_flow, xml_function] not in new_flow_list:
+                    new_flow_list.append([xml_flow, xml_function])
+
+    for xml_flow, xml_function in new_flow_list.copy():
+        if [xml_flow, xml_function.parent] in new_flow_list:
+            new_flow_list.remove([xml_flow, xml_function.parent])
+
+    return new_flow_list
+
+
+def get_external_flow_with_level(main_flow_list, main_function_list, main_fun, xml_flow_list,
+                                 level):
+    """Returns external functions list, flow lists and parent dict"""
+    ext_flow_fun_list = set()
+    ext_flow_list = []
+    ext_flow_parent_dict = {}
+    for flow, _ in main_flow_list:
+        for xml_flow, xml_fun in xml_flow_list:
+            if flow == xml_flow and xml_fun.parent == main_fun.parent:
+                ext_flow_fun_list.add(xml_fun)
+            elif flow == xml_flow and question_answer.check_not_family(main_fun, xml_fun) and \
+                    xml_fun.parent is None:
+                ext_flow_fun_list.add(xml_fun)
+            elif flow == xml_flow and not question_answer.check_parentality(xml_fun, main_fun) and \
+                    [xml_flow, xml_fun.parent] not in xml_flow_list:
+                ext_flow_fun_list.add(xml_fun)
+
+    for fun in ext_flow_fun_list.copy():
+        if fun.child_list:
+            function_list_dict = question_answer.get_children(fun, level=level)
+            ext_flow_fun_list.update(function_list_dict[0])
+            ext_flow_parent_dict.update(function_list_dict[1])
+
+    for flow, _ in main_flow_list:
+        for xml_flow, xml_fun in xml_flow_list:
+            if flow == xml_flow and xml_fun in ext_flow_fun_list and \
+                    xml_fun not in main_function_list:
+                # ext_flow_list.append([xml_flow, xml_fun])
+                if not xml_fun.child_list:
+                    if [xml_flow, xml_fun] not in ext_flow_list:
+                        ext_flow_list.append([xml_flow, xml_fun])
+                else:
+                    temp = []
+                    for k in xml_fun.child_list:
+                        temp.append([xml_flow, k])
+                    if not any(t in temp for t in xml_flow_list):
+                        if [xml_flow, xml_fun] not in ext_flow_list:
+                            ext_flow_list.append([xml_flow, xml_fun])
+
+    for fun in ext_flow_fun_list.copy():
+        if not any(a == fun for a in [i[1] for i in ext_flow_list]) and not fun.child_list:
+            ext_flow_fun_list.remove(fun)
+
+    for fun in ext_flow_fun_list.copy():
+        if not any(a == fun for a in [i[1] for i in ext_flow_list]) and \
+                not any(i in fun.child_list for i in ext_flow_fun_list) and \
+                fun != main_fun:
+            ext_flow_fun_list.remove(fun)
+
+    return ext_flow_fun_list, ext_flow_list, ext_flow_parent_dict
+
+
+def get_cons_prod_from_view_allocated_data(xml_data_list, xml_view_list, xml_consumer_function_list,
+                                           xml_producer_function_list, function_list):
+    """If a view is activated, returns filtered consumer/producer lists"""
+    new_function_list = []
+    new_consumer_list = []
+    new_producer_list = []
+    new_data_list = filter_allocated_item_from_view(xml_data_list, xml_view_list)
+
+    if len(new_data_list) == len(xml_data_list):
+        for prod in xml_producer_function_list:
+            if any(item == prod[1] for item in function_list):
+                new_producer_list.append(prod)
+                if prod[1] not in new_function_list:
+                    new_function_list.append(prod[1])
+
+        for cons in xml_consumer_function_list:
+            if any(item == cons[1] for item in function_list):
+                new_consumer_list.append(cons)
+                if cons[1] not in new_function_list:
+                    new_function_list.append(cons[1])
+
+    else:
+        for cons in xml_consumer_function_list:
+            if any(item.name == cons[0] for item in new_data_list) and \
+                    any(item == cons[1] for item in function_list):
+                new_consumer_list.append(cons)
+                if cons[1] not in new_function_list:
+                    new_function_list.append(cons[1])
+
+        for prod in xml_producer_function_list:
+            if any(item.name == prod[0] for item in new_data_list) and \
+                    any(item == prod[1] for item in function_list):
+                new_producer_list.append(prod)
+                if prod[1] not in new_function_list:
+                    new_function_list.append(prod[1])
+
+    if len(new_consumer_list) == 0 and len(new_producer_list) == 0:
+        new_function_list = function_list
+
+    return new_function_list, new_consumer_list, new_producer_list
+
+
+def get_parent_dict(element, element_list, parent_dict):
+    if element.parent:
+        parent_dict[element.id] = element.parent.id
+
+        if element.parent not in element_list:
+            element_list.add(element.parent)
+            element.parent.child_list.clear()
+
+        element.parent.add_child(element)
+
+        get_parent_dict(element.parent, element_list, parent_dict)
+
+
+def get_fun_elem_function_list(function, function_list, fun_elem):
+    if function.parent:
+        if function.parent.id in fun_elem.allocated_function_list:
+            get_fun_elem_function_list(function.parent, function_list, fun_elem)
+        else:
+            function_list.add(function)
+    else:
+        function_list.add(function)
```

### Comparing `jarvis4se-1.3.5/src/jarvis/jarvis.py` & `jarvis4se-1.4.0/src/jarvis/jarvis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-"""@defgroup jarvis
-Jarvis module
-"""
-# Libraries
-import re
-import os
-import getpass
-import shutil
-from datetime import datetime
-from io import StringIO
-from IPython.core.magic import (Magics, magics_class, cell_magic)
-
-# Modules
-from xml_adapter import XmlWriter3SE, XmlParser3SE
-from tools import Logger
-
-
-# The class MUST call this class decorator at creation time
-@magics_class
-class MagicJarvis(Magics):
-    """Magic iPython class"""
-    def __init__(self, shell, parser):
-        # You must call the parent constructor
-        super().__init__(shell)
-        self.parser = parser
-
-    @cell_magic
-    def jarvis(self, _, cell):
-        """Entry point for jarvi4se"""
-        # Initialize xml_parser i.e. empty obj_dict that will contain objet's lists
-        xml_parser = XmlParser3SE()
-        obj_dict = xml_parser.xml_dict
-        # We create a string buffer containing the
-        # contents of the cell.
-        sio = StringIO(cell)
-        # Take the value within the buffer
-        input_str = sio.getvalue()
-        # Delete the '"' from input string, to avoid xml to plantuml errors.
-        input_str = input_str.replace('"', "")
-        # Delete extra whitespaces
-        input_str = re.sub(' +', ' ', input_str)
-        # Get model's declaration, need a space after "with" otherwise print a message
-        xml_name_str = re.match(r"^with (.*)(?=.|\n)", input_str, re.MULTILINE)
-        if xml_name_str:
-            xml_name = xml_name_str.group(1)
-            # If the model(i.e. file) already exists, parse it to extract lists
-            if os.path.isfile(f"{xml_name}.xml"):
-                obj_dict = xml_parser.parse_xml(f"{xml_name}.xml")
-                Logger.set_info(__name__,
-                                f"{xml_name}.xml parsed")
-                output_xml = XmlWriter3SE(f"{xml_name}.xml")
-            # Else create an empty xml_lists
-            # or will be named by default "Outpout"
-            else:
-                if len(xml_name) > 1:
-                    Logger.set_info(__name__,
-                                    f"Creating {xml_name}.xml !")
-
-                    output_xml = XmlWriter3SE(f"{xml_name}.xml")
-                else:
-                    Logger.set_info(__name__,
-                                    "Xml's file does not exists, creating it ('output.xml' by default) !")
-                    output_xml = XmlWriter3SE("")
-                output_xml.write()
-
-            obj_dict['output_xml'] = output_xml
-            update = self.parser.lookup_table(input_str, **obj_dict)
-
-            if not update:
-                return
-
-            if 1 in update:
-                Logger.set_info(__name__,
-                                f"{output_xml.file} updated")
-            else:
-                Logger.set_info(__name__,
-                                f"No update for {output_xml.file}")
-        else:
-            Logger.set_error(__name__,
-                             "Bad model's declaration, model's name should be written or add a ' '(blank space) "
-                             "after 'with' command to create default 'Output.xml'")
-
-
-def greet_user():
-    """Greets the user according to the time thanks to :
-    https://ireadblog.com/posts/141/how-to-build-your-personal-ai-assistant-using-python"""
-    hour = datetime.now().hour
-    # Use getpass() because available on Unix/Windows
-    user_name = getpass.getuser()
-
-    # Single display (not related to logging)
-    if 6 <= hour < 12:
-        print(f"Good morning {user_name}")
-    elif 12 <= hour < 16:
-        print(f"Good afternoon {user_name}")
-    elif 16 <= hour < 19:
-        print(f"Good evening {user_name}")
-    else:
-        print(f"Hello {user_name}")
-
-    print("I am Jarvis. How may I assist you?")
-
-
-def clean_folders():
-    """ Clean Jarvis folder
-    @return None
-    """
-    for folder in ["./diagrams", "./log"]:
-        if os.path.isdir(folder):
-            for filename in os.listdir(folder):
-                file_path = os.path.join(folder, filename)
-                try:
-                    if os.path.isfile(file_path) or os.path.islink(file_path):
-                        os.remove(file_path)
-                    elif os.path.isdir(file_path):
-                        shutil.rmtree(file_path)
-                except Exception as ex:
-                    # function called before Logger initialization.
-                    print('[ERROR] Failed to delete %s. Reason: %s' % (file_path, ex))
+"""@defgroup jarvis
+Jarvis module
+"""
+# Libraries
+import re
+import os
+import getpass
+import shutil
+from datetime import datetime
+from io import StringIO
+from IPython.core.magic import (Magics, magics_class, cell_magic)
+
+# Modules
+from xml_adapter import XmlWriter3SE, XmlParser3SE
+from tools import Logger
+
+
+# The class MUST call this class decorator at creation time
+@magics_class
+class MagicJarvis(Magics):
+    """Magic iPython class"""
+    def __init__(self, shell, parser):
+        # You must call the parent constructor
+        super().__init__(shell)
+        self.parser = parser
+
+    @cell_magic
+    def jarvis(self, _, cell):
+        """Entry point for jarvi4se"""
+        # Initialize xml_parser i.e. empty obj_dict that will contain objet's lists
+        xml_parser = XmlParser3SE()
+        obj_dict = xml_parser.xml_dict
+        # We create a string buffer containing the
+        # contents of the cell.
+        sio = StringIO(cell)
+        # Take the value within the buffer
+        input_str = sio.getvalue()
+        # Delete the '"' from input string, to avoid xml to plantuml errors.
+        input_str = input_str.replace('"', "")
+        # Delete extra whitespaces
+        input_str = re.sub(' +', ' ', input_str)
+        # Get model's declaration, need a space after "with" otherwise print a message
+        xml_name_str = re.match(r"^with (.*)(?=.|\n)", input_str, re.MULTILINE)
+        if xml_name_str:
+            xml_name = xml_name_str.group(1)
+            # If the model(i.e. file) already exists, parse it to extract lists
+            if os.path.isfile(f"{xml_name}.xml"):
+                obj_dict = xml_parser.parse_xml(f"{xml_name}.xml")
+                Logger.set_info(__name__,
+                                f"{xml_name}.xml parsed")
+                output_xml = XmlWriter3SE(f"{xml_name}.xml")
+            # Else create an empty xml_lists
+            # or will be named by default "Output"
+            else:
+                if len(xml_name) > 1:
+                    Logger.set_info(__name__,
+                                    f"Creating {xml_name}.xml !")
+
+                    output_xml = XmlWriter3SE(f"{xml_name}.xml")
+                else:
+                    Logger.set_info(__name__,
+                                    "Xml's file does not exist, creating it ('output.xml' by default) !")
+                    output_xml = XmlWriter3SE("")
+                output_xml.write()
+
+            obj_dict['output_xml'] = output_xml
+            update = self.parser.lookup_table(input_str, **obj_dict)
+
+            if not update:
+                return
+
+            if 1 in update:
+                Logger.set_info(__name__,
+                                f"{output_xml.file} updated")
+            else:
+                Logger.set_info(__name__,
+                                f"No update for {output_xml.file}")
+        else:
+            Logger.set_error(__name__,
+                             "Bad model's declaration, model's name should be written or add a ' '(blank space) "
+                             "after 'with' command to create default 'Output.xml'")
+
+
+def greet_user():
+    """Greets the user according to the time thanks to :
+    https://ireadblog.com/posts/141/how-to-build-your-personal-ai-assistant-using-python"""
+    hour = datetime.now().hour
+    # Use getpass() because available on Unix/Windows
+    user_name = getpass.getuser()
+
+    # Single display (not related to logging)
+    if 6 <= hour < 12:
+        print(f"Good morning {user_name}")
+    elif 12 <= hour < 16:
+        print(f"Good afternoon {user_name}")
+    elif 16 <= hour < 19:
+        print(f"Good evening {user_name}")
+    else:
+        print(f"Hello {user_name}")
+
+    print("I am Jarvis. How may I assist you?")
+
+
+def clean_folders():
+    """ Clean Jarvis folder
+    @return None
+    """
+    for folder in ["./diagrams", "./log"]:
+        if os.path.isdir(folder):
+            for filename in os.listdir(folder):
+                file_path = os.path.join(folder, filename)
+                try:
+                    if os.path.isfile(file_path) or os.path.islink(file_path):
+                        os.remove(file_path)
+                    elif os.path.isdir(file_path):
+                        shutil.rmtree(file_path)
+                except Exception as ex:
+                    # function called before Logger initialization.
+                    print('[ERROR] Failed to delete %s. Reason: %s' % (file_path, ex))
```

### Comparing `jarvis4se-1.3.5/src/jarvis/orchestrator/functional_orchestrator.py` & `jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_functional.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,707 +1,751 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Module with methods relative to Functional section"""
-# Libraries
-
-# Modules
-import datamodel
-from . import shared_orchestrator
-from jarvis import question_answer
-from jarvis import util
-from tools import Logger
-
-
-def check_add_predecessor(data_predecessor_str_set, xml_data_list, xml_view_list, output_xml):
-    """
-    Check if each string in data_predecessor_str_set is corresponding to an actual Data object,
-    create new [Data, predecessor] objects lists for object's type : Data.
-    Send lists to add_predecessor() to write them within xml and then returns update_list from it.
-
-        Parameters:
-            data_predecessor_str_set ([str]) : Lists of string from jarvis cell
-            xml_data_list ([Data]) : Data list from xml parsing
-            xml_view_list ([View]) : View list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    data_predecessor_list = []
-
-    allocated_item_list = []
-    # Filter input string
-    data_predecessor_str_list = util.cut_tuple_list(data_predecessor_str_set)
-
-    # Create data names list already in xml
-    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
-
-    for elem in data_predecessor_str_list:
-        is_elem_found = True
-        if elem[0] not in xml_data_name_list:
-            is_elem_found = False
-            if elem[1] not in xml_data_name_list:
-                Logger.set_error(__name__,
-                                 f"{elem[0]} and {elem[1]} do not exist")
-            else:
-                Logger.set_error(__name__,
-                                 f"{elem[0]} does not exist")
-
-        if elem[0] in xml_data_name_list:
-            if elem[1] not in xml_data_name_list:
-                is_elem_found = False
-                Logger.set_error(__name__,
-                                 f"{elem[1]} does not exist")
-
-        if is_elem_found:
-            predecessor = None
-            selected_data = None
-            existing_predecessor_id_list = []
-            for data in xml_data_list:
-                if elem[0] == data.name:
-                    selected_data = data
-                    for existing_predecessor in data.predecessor_list:
-                        existing_predecessor_id_list.append(existing_predecessor.id)
-            for da in xml_data_list:
-                if elem[1] == da.name and da.id not in existing_predecessor_id_list:
-                    predecessor = da
-            if predecessor is not None and selected_data is not None:
-                data_predecessor_list.append([selected_data, predecessor])
-
-            allocation_chain_1 = shared_orchestrator.check_add_allocated_item(elem[0],
-                                                                              xml_data_list,
-                                                                              xml_view_list)
-            if allocation_chain_1:
-                allocated_item_list.append(allocation_chain_1)
-
-            allocation_chain_2 = shared_orchestrator.check_add_allocated_item(elem[1],
-                                                                              xml_data_list,
-                                                                              xml_view_list)
-            if allocation_chain_2:
-                allocated_item_list.append(allocation_chain_2)
-
-    update = add_predecessor(data_predecessor_list, xml_data_list, output_xml)
-    shared_orchestrator.add_allocation({5: allocated_item_list}, output_xml)
-
-    return update
-
-
-def add_predecessor(predecessor_list, xml_data_list, output_xml):
-    """
-    Check if input lists is not empty, write in xml for each list and return update list if some
-    updates has been made
-
-        Parameters:
-            predecessor_list ([Data, Data(predecessor)]) : Data object to set new predessor and
-            predecessor Data
-            xml_data_list ([Data]) : Data list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-
-    if not predecessor_list:
-        return 0
-
-    output_xml.write_data_predecessor(predecessor_list)
-
-    for data_predecessor in predecessor_list:
-        for d in xml_data_list:
-            if data_predecessor[0].id == d.id:
-                d.add_predecessor(data_predecessor[1])
-
-        Logger.set_info(__name__,
-                        f"{data_predecessor[1].name} predecessor for "
-                        f"{data_predecessor[0].name}")
-
-    return 1
-
-
-def check_add_consumer_function(consumer_str_list, xml_consumer_function_list,
-                                xml_producer_function_list, xml_function_list, xml_data_list,
-                                output_xml):
-    """
-    Check if each string in consumer_str_list are corresponding to an actual object, create new
-    [data, consumer] objects list for object's type : Function.
-    Send lists to add_consumer_function() to write them within xml and then returns update_list
-    from it.
-
-        Parameters:
-            consumer_str_list ([str]) : Lists of string from jarvis cell
-            xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
-            function list from xml
-            xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
-            function list from xml
-            xml_function_list ([Function]) : Function list from xml parsing
-            xml_data_list ([Data]) : Data list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    new_consumer_list = []
-    # Create object names/aliases list and data's name
-    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
-    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
-    # Loop to filter consumer and create a new list
-    for elem in consumer_str_list:
-        is_elem_found = True
-        if not any(item == elem[1] for item in xml_function_name_list) and \
-                not any(item == elem[0] for item in xml_data_name_list):
-            is_elem_found = False
-            Logger.set_error(__name__,
-                             f"{elem[1]} and {elem[0]} do not exist")
-        elif not any(item == elem[1] for item in xml_function_name_list) or \
-                not any(item == elem[0] for item in xml_data_name_list):
-            is_elem_found = False
-            if any(item == elem[1] for item in xml_function_name_list) and \
-                    not any(item == elem[0] for item in xml_data_name_list):
-                Logger.set_error(__name__,
-                                 f"{elem[0]} does not exist")
-            elif any(item == elem[0] for item in xml_data_name_list) and \
-                    not any(item == elem[1] for item in xml_function_name_list):
-                Logger.set_error(__name__,
-                                 f"{elem[1]} does not exist")
-
-        if is_elem_found:
-            Logger.set_debug(__name__, f"[{elem[0]}, {elem[1]}] check")
-            # Loop to filter consumer and create a new list
-            for function in xml_function_list:
-                if elem[1] == function.name or elem[1] == function.alias:
-                    if [elem[0], function] not in xml_consumer_function_list:
-                        add_producer_consumer_flow_recursively(elem[0],
-                                                               function,
-                                                               xml_consumer_function_list,
-                                                               xml_producer_function_list,
-                                                               new_consumer_list,
-                                                               output_xml,
-                                                               "consumer")
-                    break
-
-    Logger.set_debug(__name__, f"{consumer_str_list}: {new_consumer_list}")
-    update = add_consumer_function(new_consumer_list, xml_consumer_function_list, output_xml)
-
-    return update
-
-
-def add_consumer_function(new_consumer_list, xml_consumer_function_list, output_xml):
-    """
-    Check if input list is not empty, write in xml for each element and return update list if some
-    updates has been made
-
-        Parameters:
-            new_consumer_list ([Data_name_str, Function]) : Data's name and consumer's function list
-            xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
-            function list from xml
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-
-    if not new_consumer_list:
-        return 0
-
-    # TODO : new_producer_list to be [data, function] and not [data_name, function]
-    output_xml.write_data_consumer(new_consumer_list)
-
-    # Warn the user once added within xml
-    for consumer in new_consumer_list:
-        xml_consumer_function_list.append(consumer)
-        Logger.set_info(__name__,
-                        f"{consumer[1].name} consumes {consumer[0]}")
-
-    return 1
-
-
-def add_producer_consumer_flow_recursively(flow, function, current_list, opposite_list, new_list, output_xml,
-                                           relationship_str):
-    """
-    Recursive method to add producer / consumer function for a flow.
-        Parameters:
-            flow (Data_name_str) : Data's name
-            function (Function) : Current function's parent
-            current_list ([Data_name_str, function_name_str]) : 'Current' list (producer/consumer)
-            opposite_list ([Data_name_str, function_name_str]) : Opposite list from current
-            new_list ([Data_name_str, Function]) : Data's name and consumer/producer's function list
-            output_xml (XmlWriter3SE object) : XML's file object
-            relationship_str (str) : "consumer" or "producer"
-            out (bool) : List for recursivity
-        Returns:
-            elem ([data, Function]) : Return parent
-
-    """
-    # Prevent function.parent to be added twice
-    if [flow, function] not in new_list and [flow, function] not in current_list:
-        new_list.append([flow, function])
-        Logger.set_debug(__name__, f"[{flow}, {function.name}] added")
-
-        # Check that parent opposite flow is present (if any)
-        is_opposite = False
-        for [opposite_flow, opposite_function] in opposite_list:
-            if opposite_flow == flow:
-                is_opposite = True
-                if opposite_function.parent is not None and opposite_function.parent != function and \
-                        opposite_function.parent != function.parent:
-                    if [opposite_flow, opposite_function.parent] not in opposite_list:
-                        add_producer_consumer_opposite(flow, opposite_function.parent, opposite_list, output_xml,
-                                                       relationship_str)
-
-        if not is_opposite:
-            if relationship_str == "consumer":
-                Logger.set_warning(__name__, f"No producer found for {flow}")
-            elif relationship_str == "producer":
-                Logger.set_warning(__name__, f"No consumer found for {flow}")
-            else:
-                Logger.set_error(__name__, f"Unsupported data relationship type: {relationship_str}")
-
-    if function.parent is not None:
-        parent_child_list, parent_child_dict = question_answer.get_children(function.parent)
-
-        if not any([flow, parent_child] in opposite_list for parent_child in parent_child_list):
-            add_producer_consumer_flow_recursively(flow, function.parent, current_list, opposite_list, new_list,
-                                                   output_xml,
-                                                   relationship_str)
-        elif [flow, function.parent] in opposite_list:
-            # Check that no other function needs the flow before removing it
-            ext_function_list = []
-            for [current_flow, current_function] in current_list:
-                if current_flow == flow:
-                    Logger.set_debug(__name__, f"[{current_flow}, {current_function.name}] "
-                                               f"added in external function list")
-                    ext_function_list.append([current_flow, current_function])
-
-            for parent_child in parent_child_list:
-                if [flow, parent_child] in ext_function_list:
-                    ext_function_list.remove([flow, parent_child])
-
-            if len(ext_function_list) == 0:
-                remove_producer_consumer_opposite(flow, function.parent, opposite_list, output_xml, relationship_str)
-            else:
-                Logger.set_debug(__name__, f"[{flow}, {function.parent.name}] still needed")
-
-
-def add_producer_consumer_opposite(flow, function, flow_function_list, output_xml, relationship_type):
-    """
-    Add specific consumer/producer relationship within xml's file.
-
-        Parameters:
-            flow (Data_name_str) : Data's name
-            function (Function) : Current Function object
-            flow_function_list : list of [flow, function]
-            output_xml (XmlWriter3SE object) : XML's file object
-            relationship_type (str) : Type of relationship (i.e. consumer or producer)
-        Returns:
-            None
-    """
-    flow_function_list.append([flow, function])
-
-    if relationship_type == "producer":
-        output_xml.write_data_relationship([flow, function],
-                                           "consumer")
-        Logger.set_info(__name__,
-                        f"{function.name} consumes {flow} due to one of its children")
-    elif relationship_type == "consumer":
-
-        output_xml.write_data_relationship([flow, function],
-                                           "producer")
-        Logger.set_info(__name__,
-                        f"{function.name} produces {flow} due to one of its children")
-
-    if function.parent:
-        add_producer_consumer_opposite(flow, function.parent, flow_function_list, output_xml, relationship_type)
-
-
-def remove_producer_consumer_opposite(flow, function, flow_function_list, output_xml, relationship_type):
-    """
-    Delete specific consumer/producer relationship within xml's file.
-
-        Parameters:
-            flow (Data_name_str) : Data's name
-            function (Function) : Current Function object
-            flow_function_list : list of [flow, function]
-            output_xml (XmlWriter3SE object) : XML's file object
-            relationship_type (str) : Type of relationship (i.e. consumer or producer)
-        Returns:
-            None
-    """
-    flow_function_list.remove([flow, function])
-
-    if relationship_type == "producer":
-        output_xml.delete_data_relationship([flow, function],
-                                            "consumer")
-        Logger.set_info(__name__,
-                        f"{function.name} does not consume {flow} anymore")
-    elif relationship_type == "consumer":
-
-        output_xml.delete_data_relationship([flow, function],
-                                            "producer")
-        Logger.set_info(__name__,
-                        f"{function.name} does not produce {flow} anymore")
-
-    if function.parent and [flow, function.parent] in flow_function_list:
-        remove_producer_consumer_opposite(flow, function.parent, flow_function_list, output_xml, relationship_type)
-
-
-def check_add_producer_function(producer_str_list, xml_consumer_function_list,
-                                xml_producer_function_list, xml_function_list, xml_data_list,
-                                output_xml):
-    """
-    Check if each string in consumer_str_list are corresponding to an actual object, create new
-    [data, producer] objects list for object's type : Function.
-    Send list to add_producer_function() to write them within xml and then returns update.
-
-        Parameters:
-            producer_str_list ([str]) : List of string from jarvis cell
-            xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
-            function list from xml
-            xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
-            function list from xml
-            xml_function_list ([Function]) : Function list from xml parsing
-            xml_data_list ([Data]) : Data list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    new_producer_list = []
-    # Create object names/aliases list
-    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
-    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
-    # Loop to filter producer and create a new list
-    for elem in producer_str_list:
-        is_elem_found = True
-        if not any(item == elem[1] for item in xml_function_name_list) and \
-                not any(item == elem[0] for item in xml_data_name_list):
-            is_elem_found = False
-            Logger.set_error(__name__,
-                             f"{elem[1]} and {elem[0]} do not exist")
-        elif not any(item == elem[1] for item in xml_function_name_list) or \
-                not any(item == elem[0] for item in xml_data_name_list):
-            is_elem_found = False
-            if any(item == elem[1] for item in xml_function_name_list) and \
-                    not any(item == elem[0] for item in xml_data_name_list):
-                Logger.set_error(__name__,
-                                 f"{elem[0]} does not exist")
-            elif any(item == elem[0] for item in xml_data_name_list) and \
-                    not any(item == elem[1] for item in xml_function_name_list):
-                Logger.set_error(__name__,
-                                 f"{elem[1]} does not exist")
-
-        if is_elem_found:
-            Logger.set_debug(__name__, f"[{elem[0]}, {elem[1]}] check")
-            # Loop to filter consumer and create a new list
-            for function in xml_function_list:
-                if elem[1] == function.name or elem[1] == function.alias:
-                    if [elem[0], function] not in xml_producer_function_list:
-                        add_producer_consumer_flow_recursively(elem[0],
-                                                               function,
-                                                               xml_producer_function_list,
-                                                               xml_consumer_function_list,
-                                                               new_producer_list,
-                                                               output_xml,
-                                                               "producer")
-                    break
-
-    Logger.set_debug(__name__, f"{producer_str_list}: {new_producer_list}")
-    update = add_producer_function(new_producer_list, xml_producer_function_list, output_xml)
-
-    return update
-
-
-def add_producer_function(new_producer_list, xml_producer_function_list, output_xml):
-    """
-    Check if input list is not empty, write in xml for each element and return update list if some
-    updates has been made
-
-        Parameters:
-            new_producer_list ([Data_name_str, Function]) : Data's name and producer's function list
-            xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
-            function list from xml
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    if not new_producer_list:
-        return 0
-
-    # TODO : new_producer_list to be [data, function] and not [data_name, function]
-    output_xml.write_data_producer(new_producer_list)
-    # Warn the user once added within xml
-    for producer in new_producer_list:
-        xml_producer_function_list.append(producer)
-        Logger.set_info(__name__,
-                        f"{producer[1].name} produces {producer[0]}")
-    return 1
-
-
-# TODO: Check condition_str on data and (add LogicalType, ArithmeticType in datamodel.py)
-def check_add_transition_condition(trans_condition_str_list, xml_transition_list, output_xml):
-    """
-    Check if each string in trans_condition_str_list is corresponding to an actual Transition
-    object, create new [Transition, condition_str] objects lists for object's type : Transition.
-    Send lists to add_transition_condition() to write them within xml and then returns update_list
-    from it.
-
-        Parameters:
-            trans_condition_str_list ([str]) : Lists of string from jarvis cell
-            xml_transition_list ([Transition]) : Transition list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    condition_list = []
-    # Create a list with all transition names/aliases already in the xml
-    xml_transition_name_list = question_answer.get_objects_names(xml_transition_list)
-    for transition_str, condition_str in trans_condition_str_list:
-        is_elem_found = True
-        if not any(transition_str in s for s in xml_transition_name_list):
-            is_elem_found = False
-            Logger.set_error(__name__,
-                             f"The transition {transition_str} does not exist")
-
-        if is_elem_found:
-            for transition in xml_transition_list:
-                if transition_str == transition.name or transition_str == transition.alias:
-                    if not condition_str.lstrip(' ') in transition.condition_list:
-                        condition_list.append([transition, condition_str.lstrip(' ')])
-
-    update = add_transition_condition(condition_list, output_xml)
-
-    return update
-
-
-def add_transition_condition(condition_list, output_xml):
-    """
-    Check if input list is not empty, write in xml for each list and return update list if some
-    updates has been made
-
-        Parameters:
-            condition_list ([Transition, condition_str]) : Transition object and conditions as str
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    if not condition_list:
-        return 0
-
-    output_xml.write_transition_condition(condition_list)
-    for elem in condition_list:
-        elem[0].add_condition(elem[1])
-        Logger.set_info(__name__,
-                        f"Condition for {elem[0].name} : {elem[1]}")
-    return 1
-
-
-def check_add_src_dest(src_dest_str, xml_transition_list, xml_state_list, output_xml):
-    """
-    Check if each string in src_dest_str is corresponding to an actual Transition and State object,
-    create new [Transition, State] objects lists.
-    Send lists to add_src_dest() to write them within xml and then returns update_list from it.
-
-        Parameters:
-            src_dest_str ([str]) : Lists of string from jarvis cell
-            xml_transition_list ([Transition]) : Transition list from xml parsing
-            xml_state_list ([State]) : State list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    new_src_list = []
-    new_dest_list = []
-    # Create lists with all object names/aliases already in the xml
-    xml_transition_name_list = question_answer.get_objects_names(xml_transition_list)
-    xml_state_name_list = question_answer.get_objects_names(xml_state_list)
-
-    concatenated_lists = [*xml_transition_name_list, *xml_state_name_list]
-
-    # elem = [source/destination, transition_name, state_name]
-    for elem in src_dest_str:
-        is_elem_found = True
-        if not all(t in concatenated_lists for t in [elem[1], elem[2]]):
-            is_elem_found = False
-            if any(elem[1] in s for s in xml_transition_name_list) and not any(
-                    elem[2] in j for j in xml_state_name_list):
-                Logger.set_error(__name__,
-                                 f"{elem[2]} state does not exist")
-            elif any(elem[2] in s for s in xml_state_name_list) and not any(
-                    elem[1] in j for j in xml_transition_name_list):
-                Logger.set_error(__name__,
-                                 f"{elem[1]} transition does not exist")
-            else:
-                Logger.set_error(__name__,
-                                 f"{elem[1]} transition and {elem[2]} state do not exist")
-
-        if is_elem_found:
-            if elem[0] == "source":
-                for transition in xml_transition_list:
-                    if elem[1] == transition.name or elem[1] == transition.alias:
-                        for state in xml_state_list:
-                            if elem[2] == state.name or elem[2] == state.alias:
-                                if not isinstance(state.type, datamodel.BaseType):
-                                    if 'EXIT' in state.type.name:
-                                        Logger.set_error(__name__,
-                                                         f"{elem[2]} is typed as EXIT state, "
-                                                         f"it cannot be put as source's transition (not added)")
-                                else:
-                                    if transition.source != state.id:
-                                        new_src_list.append([transition, state])
-
-            elif elem[0] == "destination":
-                for transition in xml_transition_list:
-                    if elem[1] == transition.name or elem[1] == transition.alias:
-                        for state in xml_state_list:
-                            if elem[2] == state.name or elem[2] == state.alias:
-                                if not isinstance(state.type, datamodel.BaseType):
-                                    if 'ENTRY' in state.type.name:
-                                        Logger.set_error(__name__,
-                                                         f"{elem[2]} is typed as ENTRY state, it cannot be "
-                                                         f"put as destination's transition (not added)")
-                                else:
-                                    if transition.destination != state.id:
-                                        new_dest_list.append([transition, state])
-
-    src_dest_lists = [new_src_list, new_dest_list]
-    update = add_src_dest(src_dest_lists, output_xml)
-
-    return update
-
-
-def add_src_dest(src_dest_lists, output_xml):
-    """
-    Check if input lists are not empty, write in xml for each list and return update list if some
-    updates has been made
-
-        Parameters:
-            src_dest_lists ([Transition, State(Source)],[Transition, State(Destination)]) :
-            Transition object and Source/Destination
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    if any(src_dest_lists):
-        new_src_list = src_dest_lists[0]
-        new_dest_list = src_dest_lists[1]
-        if new_src_list:
-            output_xml.write_transition_source(new_src_list)
-            # Warn the user once writtent and added within xml
-            for source in new_src_list:
-                source[0].set_source(source[1].id)
-                Logger.set_info(__name__,
-                                f"{source[1].name} source for {source[0].name}")
-
-        if new_dest_list:
-            output_xml.write_transition_destination(new_dest_list)
-            # Warn the user once writtent and added within xml
-            for destination in new_dest_list:
-                destination[0].set_destination(destination[1].id)
-                Logger.set_info(__name__,
-                                f"{destination[1].name} destination for {destination[0].name}")
-        return 1
-
-    return 0
-
-
-def check_add_exposes(exposes_str_list, xml_fun_elem_list, xml_fun_inter_list, xml_data_list,
-                      output_xml):
-    """
-    Check and get all "Fun_elem exposes Fun_inter" strings, if Fun_inter is not exposed yet
-    (or parentality relationship) => add it to Fun_elem object and as exposedInterface within xml.
-    Args:
-        exposes_str_list ([strings]): list of strings
-        xml_fun_elem_list ([Fun Elem]) : Functional Element list from xml parsing
-        xml_fun_inter_list ([FunctionalInterface]) : FunctionalInterface list from xml parsing
-        xml_data_list ([Data]) : Data list from xml parsing
-        output_xml (XmlWriter3SE object) : XML's file object
-
-    Returns:
-        [0/1] : if update has been made
-    """
-    # TODO : add physical interface support (see write_element_exposed_interface())
-    output = False
-    cleaned_exposes_str_list = util.cut_tuple_list(exposes_str_list)
-    for exposes_str in cleaned_exposes_str_list:
-        fun_elem = question_answer.check_get_object(exposes_str[0], **{'xml_fun_elem_list': xml_fun_elem_list})
-        fun_inter = question_answer.check_get_object(exposes_str[1], **{'xml_fun_inter_list': xml_fun_inter_list})
-
-        check_print_wrong_pair_object((exposes_str[0], fun_elem, 'Functional Element'),
-                                      (exposes_str[1], fun_inter, 'Functional Interface'),
-                                      'exposes')
-        if fun_elem and fun_inter:
-            check_rule = check_fun_elem_inter_families(fun_elem, fun_inter, xml_fun_elem_list)
-            if fun_inter.id not in fun_elem.exposed_interface_list and check_rule:
-                output = True
-                fun_elem.add_exposed_interface(fun_inter.id)
-                output_xml.write_element_exposed_interface([[fun_elem, fun_inter]])
-                Logger.set_info(__name__,
-                                f"{fun_elem.name} exposes {fun_inter.name}")
-
-    if output:
-        return 1
-
-    return 0
-
-
-def check_fun_elem_inter_families(fun_elem, fun_inter, xml_fun_elem_list):
-    """A fun elem can expose an interface if already allocated to a parent/child and
-    an interface can only be exposed by 2 families of fun_elem"""
-    check = True
-    exposed_fun_elem_list = set()
-    for xml_fun_elem in xml_fun_elem_list:
-        if any(s == fun_inter.id for s in xml_fun_elem.exposed_interface_list) and \
-                xml_fun_elem != fun_elem:
-            exposed_fun_elem_list.add(xml_fun_elem)
-
-    if not exposed_fun_elem_list:
-        return check
-
-    opposite_fun_elem_list = []
-    for elem in exposed_fun_elem_list:
-        if question_answer.check_parentality(elem, fun_elem) or \
-                question_answer.check_parentality(fun_elem, elem):
-            return check
-        else:
-            opposite_fun_elem_list.append(elem)
-
-    for idx in range(0, len(opposite_fun_elem_list) - 1):
-        if not question_answer.check_parentality(
-                opposite_fun_elem_list[idx], opposite_fun_elem_list[idx + 1]) and \
-                not question_answer.check_parentality(opposite_fun_elem_list[idx + 1], opposite_fun_elem_list[idx]):
-            check = False
-            return check
-
-    return check
-
-
-def check_print_wrong_pair_object(object_a, object_b, relationship_type):
-    """
-    Prints specific user messages for wrong object(s) pair (Object_a, Object_b) relationship
-
-    Args:
-        object_a: (input_string, object_or_none, object_type_string)
-        e.g. (exposes_str[0], fun_elem, 'Functional Element')
-        object_b: (exposes_str[1], fun_inter, 'Functional Interface')
-        relationship_type: e.g. 'exposes'
-
-    """
-    if object_a[1] == object_b[1] is None:
-        Logger.set_error(__name__,
-                         f"{object_a[0]} and {object_b[0]} do not exist, choose valid names/aliases for: "
-                         f"'{object_a[2]}' {relationship_type} "
-                         f"'{object_b[2]}'")
-    elif object_a[1] is None or object_b[1] is None:
-        if object_a[1] is None and object_b[1]:
-            Logger.set_error(__name__,
-                             f"{object_a[0]} does not exist, choose a valid name/alias for: "
-                             f"'{object_a[2]}' {relationship_type} "
-                             f"{object_b[1].name}")
-        elif object_b[1] is None and object_a[1]:
-            Logger.set_error(__name__,
-                             f"{object_b[0]} does not exist, choose a valid name/alias for: "
-                             f"{object_a[1].name} {relationship_type} "
-                             f"'{object_b[2]}'")
+"""@defgroup jarvis
+Jarvis module
+"""
+# Libraries
+
+# Modules
+import datamodel
+from . import orchestrator_shared
+from jarvis.query import question_answer
+from jarvis import util
+from tools import Logger
+
+
+def check_add_predecessor(data_predecessor_str_set, **kwargs):
+    """
+    Check if each string in data_predecessor_str_set is corresponding to an actual Data object,
+    create new [Data, predecessor] objects lists for object's type : Data.
+    Send lists to add_predecessor() to write them within xml and then returns update_list from it.
+
+        Parameters:
+            data_predecessor_str_set ([str]) : Lists of string from jarvis cell
+            xml_data_list ([Data]) : Data list from xml parsing
+            xml_view_list ([View]) : View list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+    xml_data_list = kwargs['xml_data_list']
+    xml_view_list = kwargs['xml_view_list']
+    output_xml = kwargs['output_xml']
+
+    data_predecessor_list = []
+
+    allocated_item_list = []
+    # Filter input string
+    data_predecessor_str_list = util.cut_tuple_list(data_predecessor_str_set)
+
+    # Create data names list already in xml
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
+
+    for elem in data_predecessor_str_list:
+        is_elem_found = True
+        if elem[0] not in xml_data_name_list:
+            is_elem_found = False
+            if elem[1] not in xml_data_name_list:
+                Logger.set_error(__name__,
+                                 f"{elem[0]} and {elem[1]} do not exist")
+            else:
+                Logger.set_error(__name__,
+                                 f"{elem[0]} does not exist")
+
+        if elem[0] in xml_data_name_list:
+            if elem[1] not in xml_data_name_list:
+                is_elem_found = False
+                Logger.set_error(__name__,
+                                 f"{elem[1]} does not exist")
+
+        if is_elem_found:
+            predecessor = None
+            selected_data = None
+            existing_predecessor_id_list = []
+            for data in xml_data_list:
+                if elem[0] == data.name:
+                    selected_data = data
+                    for existing_predecessor in data.predecessor_list:
+                        existing_predecessor_id_list.append(existing_predecessor.id)
+            for da in xml_data_list:
+                if elem[1] == da.name and da.id not in existing_predecessor_id_list:
+                    predecessor = da
+            if predecessor is not None and selected_data is not None:
+                data_predecessor_list.append([selected_data, predecessor])
+
+            allocation_chain_1 = orchestrator_shared.check_add_allocated_item(elem[0],
+                                                                              xml_data_list,
+                                                                              xml_view_list)
+            if allocation_chain_1:
+                allocated_item_list.append(allocation_chain_1)
+
+            allocation_chain_2 = orchestrator_shared.check_add_allocated_item(elem[1],
+                                                                              xml_data_list,
+                                                                              xml_view_list)
+            if allocation_chain_2:
+                allocated_item_list.append(allocation_chain_2)
+
+    update = add_predecessor(data_predecessor_list, xml_data_list, output_xml)
+    orchestrator_shared.add_allocation({5: allocated_item_list}, **kwargs)
+
+    return update
+
+
+def add_predecessor(predecessor_list, xml_data_list, output_xml):
+    """
+    Check if input lists is not empty, write in xml for each list and return update list if some
+    updates has been made
+
+        Parameters:
+            predecessor_list ([Data, Data(predecessor)]) : Data object to set new predessor and
+            predecessor Data
+            xml_data_list ([Data]) : Data list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+
+    if not predecessor_list:
+        return 0
+
+    output_xml.write_data_predecessor(predecessor_list)
+
+    for data_predecessor in predecessor_list:
+        for d in xml_data_list:
+            if data_predecessor[0].id == d.id:
+                d.add_predecessor(data_predecessor[1])
+
+        Logger.set_info(__name__,
+                        f"{data_predecessor[1].name} predecessor for "
+                        f"{data_predecessor[0].name}")
+
+    return 1
+
+
+def check_add_consumer_function(consumer_str_list, **kwargs):
+    """
+    Check if each string in consumer_str_list are corresponding to an actual object, create new
+    [data, consumer] objects list for object's type : Function.
+    Send lists to add_consumer_function() to write them within xml and then returns update_list
+    from it.
+
+        Parameters:
+            consumer_str_list ([str]) : Lists of string from jarvis cell
+            xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
+            function list from xml
+            xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
+            function list from xml
+            xml_function_list ([Function]) : Function list from xml parsing
+            xml_data_list ([Data]) : Data list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    xml_consumer_function_list = kwargs['xml_consumer_function_list']
+    xml_producer_function_list = kwargs['xml_producer_function_list']
+    xml_function_list = kwargs['xml_function_list']
+    xml_data_list = kwargs['xml_data_list']
+    output_xml = kwargs['output_xml']
+
+    new_consumer_list = []
+    # Create object names/aliases list and data's name
+    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
+    # Loop to filter consumer and create a new list
+    for elem in consumer_str_list:
+        is_elem_found = True
+        if not any(item == elem[1] for item in xml_function_name_list) and \
+                not any(item == elem[0] for item in xml_data_name_list):
+            is_elem_found = False
+            Logger.set_error(__name__,
+                             f"{elem[1]} and {elem[0]} do not exist")
+        elif not any(item == elem[1] for item in xml_function_name_list) or \
+                not any(item == elem[0] for item in xml_data_name_list):
+            is_elem_found = False
+            if any(item == elem[1] for item in xml_function_name_list) and \
+                    not any(item == elem[0] for item in xml_data_name_list):
+                Logger.set_error(__name__,
+                                 f"{elem[0]} does not exist")
+            elif any(item == elem[0] for item in xml_data_name_list) and \
+                    not any(item == elem[1] for item in xml_function_name_list):
+                Logger.set_error(__name__,
+                                 f"{elem[1]} does not exist")
+
+        if is_elem_found:
+            Logger.set_debug(__name__, f"[{elem[0]}, {elem[1]}] check")
+            # Loop to filter consumer and create a new list
+            for function in xml_function_list:
+                if elem[1] == function.name or elem[1] == function.alias:
+                    if [elem[0], function] not in xml_consumer_function_list:
+                        add_producer_consumer_flow_recursively(elem[0],
+                                                               function,
+                                                               xml_consumer_function_list,
+                                                               xml_producer_function_list,
+                                                               new_consumer_list,
+                                                               output_xml,
+                                                               "consumer")
+                    break
+
+    Logger.set_debug(__name__, f"{consumer_str_list}: {new_consumer_list}")
+    update = add_consumer_function(new_consumer_list, xml_consumer_function_list, output_xml)
+
+    return update
+
+
+def add_consumer_function(new_consumer_list, xml_consumer_function_list, output_xml):
+    """
+    Check if input list is not empty, write in xml for each element and return update list if some
+    updates has been made
+
+        Parameters:
+            new_consumer_list ([Data_name_str, Function]) : Data's name and consumer's function list
+            xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
+            function list from xml
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+
+    if not new_consumer_list:
+        return 0
+
+    # TODO : new_producer_list to be [data, function] and not [data_name, function]
+    output_xml.write_data_consumer(new_consumer_list)
+
+    # Warn the user once added within xml
+    for consumer in new_consumer_list:
+        xml_consumer_function_list.append(consumer)
+        Logger.set_info(__name__,
+                        f"{consumer[1].name} consumes {consumer[0]}")
+
+    return 1
+
+
+def add_producer_consumer_flow_recursively(flow, function, current_list, opposite_list, new_list, output_xml,
+                                           relationship_str):
+    """
+    Recursive method to add producer / consumer function for a flow.
+        Parameters:
+            flow (Data_name_str) : Data's name
+            function (Function) : Current function's parent
+            current_list ([Data_name_str, function_name_str]) : 'Current' list (producer/consumer)
+            opposite_list ([Data_name_str, function_name_str]) : Opposite list from current
+            new_list ([Data_name_str, Function]) : Data's name and consumer/producer's function list
+            output_xml (XmlWriter3SE object) : XML's file object
+            relationship_str (str) : "consumer" or "producer"
+            out (bool) : List for recursivity
+        Returns:
+            elem ([data, Function]) : Return parent
+
+    """
+    # Prevent function.parent to be added twice
+    if [flow, function] not in new_list and [flow, function] not in current_list:
+        new_list.append([flow, function])
+        Logger.set_debug(__name__, f"[{flow}, {function.name}] added")
+
+        # Check that parent opposite flow is present (if any)
+        is_opposite = False
+        for [opposite_flow, opposite_function] in opposite_list:
+            if opposite_flow == flow:
+                is_opposite = True
+                if opposite_function.parent is not None and opposite_function.parent != function and \
+                        opposite_function.parent != function.parent:
+                    if [opposite_flow, opposite_function.parent] not in opposite_list:
+                        add_producer_consumer_opposite(flow, opposite_function.parent, opposite_list, output_xml,
+                                                       relationship_str)
+
+        if not is_opposite:
+            if relationship_str == "consumer":
+                Logger.set_warning(__name__, f"No producer found for {flow}")
+            elif relationship_str == "producer":
+                Logger.set_warning(__name__, f"No consumer found for {flow}")
+            else:
+                Logger.set_error(__name__, f"Unsupported data relationship type: {relationship_str}")
+
+    if function.parent is not None:
+        parent_child_list, parent_child_dict = question_answer.get_children(function.parent)
+
+        if not any([flow, parent_child] in opposite_list for parent_child in parent_child_list):
+            add_producer_consumer_flow_recursively(flow, function.parent, current_list, opposite_list, new_list,
+                                                   output_xml,
+                                                   relationship_str)
+        elif [flow, function.parent] in opposite_list:
+            # Check that no other function needs the flow before removing it
+            ext_function_list = []
+            for [current_flow, current_function] in current_list:
+                if current_flow == flow:
+                    Logger.set_debug(__name__, f"[{current_flow}, {current_function.name}] "
+                                               f"added in external function list")
+                    ext_function_list.append([current_flow, current_function])
+
+            for parent_child in parent_child_list:
+                if [flow, parent_child] in ext_function_list:
+                    ext_function_list.remove([flow, parent_child])
+
+            if len(ext_function_list) == 0:
+                remove_producer_consumer_opposite(flow, function.parent, opposite_list, output_xml, relationship_str)
+            else:
+                Logger.set_debug(__name__, f"[{flow}, {function.parent.name}] still needed")
+
+
+def add_producer_consumer_opposite(flow, function, flow_function_list, output_xml, relationship_type):
+    """
+    Add specific consumer/producer relationship within xml's file.
+
+        Parameters:
+            flow (Data_name_str) : Data's name
+            function (Function) : Current Function object
+            flow_function_list : list of [flow, function]
+            output_xml (XmlWriter3SE object) : XML's file object
+            relationship_type (str) : Type of relationship (i.e. consumer or producer)
+        Returns:
+            None
+    """
+    flow_function_list.append([flow, function])
+
+    if relationship_type == "producer":
+        output_xml.write_data_relationship([flow, function],
+                                           "consumer")
+        Logger.set_info(__name__,
+                        f"{function.name} consumes {flow} due to one of its children")
+    elif relationship_type == "consumer":
+
+        output_xml.write_data_relationship([flow, function],
+                                           "producer")
+        Logger.set_info(__name__,
+                        f"{function.name} produces {flow} due to one of its children")
+
+    if function.parent:
+        add_producer_consumer_opposite(flow, function.parent, flow_function_list, output_xml, relationship_type)
+
+
+def remove_producer_consumer_opposite(flow, function, flow_function_list, output_xml, relationship_type):
+    """
+    Delete specific consumer/producer relationship within xml's file.
+
+        Parameters:
+            flow (Data_name_str) : Data's name
+            function (Function) : Current Function object
+            flow_function_list : list of [flow, function]
+            output_xml (XmlWriter3SE object) : XML's file object
+            relationship_type (str) : Type of relationship (i.e. consumer or producer)
+        Returns:
+            None
+    """
+    flow_function_list.remove([flow, function])
+
+    if relationship_type == "producer":
+        output_xml.delete_data_relationship([flow, function],
+                                            "consumer")
+        Logger.set_info(__name__,
+                        f"{function.name} does not consume {flow} anymore")
+    elif relationship_type == "consumer":
+
+        output_xml.delete_data_relationship([flow, function],
+                                            "producer")
+        Logger.set_info(__name__,
+                        f"{function.name} does not produce {flow} anymore")
+
+    if function.parent and [flow, function.parent] in flow_function_list:
+        remove_producer_consumer_opposite(flow, function.parent, flow_function_list, output_xml, relationship_type)
+
+
+def check_add_producer_function(producer_str_list, **kwargs):
+    """
+    Check if each string in consumer_str_list are corresponding to an actual object, create new
+    [data, producer] objects list for object's type : Function.
+    Send list to add_producer_function() to write them within xml and then returns update.
+
+        Parameters:
+            producer_str_list ([str]) : List of string from jarvis cell
+            xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
+            function list from xml
+            xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
+            function list from xml
+            xml_function_list ([Function]) : Function list from xml parsing
+            xml_data_list ([Data]) : Data list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    xml_consumer_function_list = kwargs['xml_consumer_function_list']
+    xml_producer_function_list = kwargs['xml_producer_function_list']
+    xml_function_list = kwargs['xml_function_list']
+    xml_data_list = kwargs['xml_data_list']
+    output_xml = kwargs['output_xml']
+
+    new_producer_list = []
+    # Create object names/aliases list
+    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
+    # Loop to filter producer and create a new list
+    for elem in producer_str_list:
+        is_elem_found = True
+        if not any(item == elem[1] for item in xml_function_name_list) and \
+                not any(item == elem[0] for item in xml_data_name_list):
+            is_elem_found = False
+            Logger.set_error(__name__,
+                             f"{elem[1]} and {elem[0]} do not exist")
+        elif not any(item == elem[1] for item in xml_function_name_list) or \
+                not any(item == elem[0] for item in xml_data_name_list):
+            is_elem_found = False
+            if any(item == elem[1] for item in xml_function_name_list) and \
+                    not any(item == elem[0] for item in xml_data_name_list):
+                Logger.set_error(__name__,
+                                 f"{elem[0]} does not exist")
+            elif any(item == elem[0] for item in xml_data_name_list) and \
+                    not any(item == elem[1] for item in xml_function_name_list):
+                Logger.set_error(__name__,
+                                 f"{elem[1]} does not exist")
+
+        if is_elem_found:
+            Logger.set_debug(__name__, f"[{elem[0]}, {elem[1]}] check")
+            # Loop to filter consumer and create a new list
+            for function in xml_function_list:
+                if elem[1] == function.name or elem[1] == function.alias:
+                    if [elem[0], function] not in xml_producer_function_list:
+                        add_producer_consumer_flow_recursively(elem[0],
+                                                               function,
+                                                               xml_producer_function_list,
+                                                               xml_consumer_function_list,
+                                                               new_producer_list,
+                                                               output_xml,
+                                                               "producer")
+                    break
+
+    Logger.set_debug(__name__, f"{producer_str_list}: {new_producer_list}")
+    update = add_producer_function(new_producer_list, xml_producer_function_list, output_xml)
+
+    return update
+
+
+def add_producer_function(new_producer_list, xml_producer_function_list, output_xml):
+    """
+    Check if input list is not empty, write in xml for each element and return update list if some
+    updates has been made
+
+        Parameters:
+            new_producer_list ([Data_name_str, Function]) : Data's name and producer's function list
+            xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
+            function list from xml
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    if not new_producer_list:
+        return 0
+
+    # TODO : new_producer_list to be [data, function] and not [data_name, function]
+    output_xml.write_data_producer(new_producer_list)
+    # Warn the user once added within xml
+    for producer in new_producer_list:
+        xml_producer_function_list.append(producer)
+        Logger.set_info(__name__,
+                        f"{producer[1].name} produces {producer[0]}")
+    return 1
+
+
+# TODO: Check condition_str on data and (add LogicalType, ArithmeticType in datamodel.py)
+def check_add_transition_condition(trans_condition_str_list, **kwargs):
+    """
+    Check if each string in trans_condition_str_list is corresponding to an actual Transition
+    object, create new [Transition, condition_str] objects lists for object's type : Transition.
+    Send lists to add_transition_condition() to write them within xml and then returns update_list
+    from it.
+
+        Parameters:
+            trans_condition_str_list ([str]) : Lists of string from jarvis cell
+            xml_transition_list ([Transition]) : Transition list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    xml_transition_list = kwargs['xml_transition_list']
+    output_xml = kwargs['output_xml']
+
+    condition_list = []
+    # Create a list with all transition names/aliases already in the xml
+    xml_transition_name_list = question_answer.get_objects_names(xml_transition_list)
+    for transition_str, condition_str in trans_condition_str_list:
+        is_elem_found = True
+        if not any(transition_str in s for s in xml_transition_name_list):
+            is_elem_found = False
+            Logger.set_error(__name__,
+                             f"The transition {transition_str} does not exist")
+
+        if is_elem_found:
+            for transition in xml_transition_list:
+                if transition_str == transition.name or transition_str == transition.alias:
+                    if not condition_str.lstrip(' ') in transition.condition_list:
+                        condition_list.append([transition, condition_str.lstrip(' ')])
+                    else:
+                        Logger.set_info(__name__,
+                                        f'Condition "{condition_str.lstrip(" ")}" already exists '
+                                        f'for transition {transition_str}')
+
+    update = add_transition_condition(condition_list, output_xml)
+
+    return update
+
+
+def add_transition_condition(condition_list, output_xml):
+    """
+    Check if input list is not empty, write in xml for each list and return update list if some
+    updates has been made
+
+        Parameters:
+            condition_list ([Transition, condition_str]) : Transition object and conditions as str
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    if not condition_list:
+        return 0
+
+    output_xml.write_transition_condition(condition_list)
+    for elem in condition_list:
+        elem[0].add_condition(elem[1])
+        Logger.set_info(__name__,
+                        f"Condition for {elem[0].name} : {elem[1]}")
+    return 1
+
+
+def check_add_src_dest(src_dest_str, **kwargs):
+    """
+    Check if each string in src_dest_str is corresponding to an actual Transition and State object,
+    create new [Transition, State] objects lists.
+    Send lists to add_src_dest() to write them within xml and then returns update_list from it.
+
+        Parameters:
+            src_dest_str ([str]) : Lists of string from jarvis cell
+            xml_transition_list ([Transition]) : Transition list from xml parsing
+            xml_state_list ([State]) : State list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    xml_transition_list = kwargs['xml_transition_list']
+    xml_state_list = kwargs['xml_state_list']
+    output_xml = kwargs['output_xml']
+
+    new_src_list = []
+    new_dest_list = []
+    # Create lists with all object names/aliases already in the xml
+    xml_transition_name_list = question_answer.get_objects_names(xml_transition_list)
+    xml_state_name_list = question_answer.get_objects_names(xml_state_list)
+
+    concatenated_lists = [*xml_transition_name_list, *xml_state_name_list]
+
+    # elem = [source/destination, transition_name, state_name]
+    for elem in src_dest_str:
+        is_elem_found = True
+        if not all(t in concatenated_lists for t in [elem[1], elem[2]]):
+            is_elem_found = False
+            if any(elem[1] in s for s in xml_transition_name_list) and not any(
+                    elem[2] in j for j in xml_state_name_list):
+                Logger.set_error(__name__,
+                                 f"{elem[2]} state does not exist")
+            elif any(elem[2] in s for s in xml_state_name_list) and not any(
+                    elem[1] in j for j in xml_transition_name_list):
+                Logger.set_error(__name__,
+                                 f"{elem[1]} transition does not exist")
+            else:
+                Logger.set_error(__name__,
+                                 f"{elem[1]} transition and {elem[2]} state do not exist")
+
+        if is_elem_found:
+            if elem[0] == "source":
+                for transition in xml_transition_list:
+                    if elem[1] == transition.name or elem[1] == transition.alias:
+                        for state in xml_state_list:
+                            if elem[2] == state.name or elem[2] == state.alias:
+                                if not isinstance(state.type, datamodel.BaseType):
+                                    if datamodel.ExitStateLabel in state.type.name.lower():
+                                        Logger.set_error(__name__,
+                                                         f"{elem[2]} is typed as EXIT state, "
+                                                         f"it cannot be put as source's transition (not added)")
+                                    elif datamodel.EntryStateLabel in state.type.name.lower():
+                                        new_src_list.append([transition, state])
+                                    else:
+                                        Logger.set_error(__name__,
+                                                         f"{elem[2]} is not typed as state, "
+                                                         f"it cannot be put as source's transition (not added)")
+                                else:
+                                    if transition.source != state.id:
+                                        new_src_list.append([transition, state])
+                                    else:
+                                        Logger.set_info(__name__,
+                                                        f'{elem[2]} already the source of transition {elem[1]}')
+
+            elif elem[0] == "destination":
+                for transition in xml_transition_list:
+                    if elem[1] == transition.name or elem[1] == transition.alias:
+                        for state in xml_state_list:
+                            if elem[2] == state.name or elem[2] == state.alias:
+                                if not isinstance(state.type, datamodel.BaseType):
+                                    if datamodel.EntryStateLabel in state.type.name.lower():
+                                        Logger.set_error(__name__,
+                                                         f"{elem[2]} is typed as ENTRY state, it cannot be "
+                                                         f"put as destination's transition (not added)")
+                                    elif datamodel.ExitStateLabel in state.type.name.lower():
+                                        new_dest_list.append([transition, state])
+                                    else:
+                                        Logger.set_error(__name__,
+                                                         f"{elem[2]} is not typed as state, "
+                                                         f"it cannot be put as source's transition (not added)")
+                                else:
+                                    if transition.destination != state.id:
+                                        new_dest_list.append([transition, state])
+                                    else:
+                                        Logger.set_info(__name__,
+                                                        f'{elem[2]} already the destination of transition {elem[1]}')
+
+    src_dest_lists = [new_src_list, new_dest_list]
+    update = add_src_dest(src_dest_lists, output_xml)
+
+    return update
+
+
+def add_src_dest(src_dest_lists, output_xml):
+    """
+    Check if input lists are not empty, write in xml for each list and return update list if some
+    updates has been made
+
+        Parameters:
+            src_dest_lists ([Transition, State(Source)],[Transition, State(Destination)]) :
+            Transition object and Source/Destination
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    if any(src_dest_lists):
+        new_src_list = src_dest_lists[0]
+        new_dest_list = src_dest_lists[1]
+        if new_src_list:
+            output_xml.write_transition_source(new_src_list)
+            # Warn the user once writtent and added within xml
+            for source in new_src_list:
+                source[0].set_source(source[1].id)
+                Logger.set_info(__name__,
+                                f"{source[1].name} source for {source[0].name}")
+
+        if new_dest_list:
+            output_xml.write_transition_destination(new_dest_list)
+            # Warn the user once writtent and added within xml
+            for destination in new_dest_list:
+                destination[0].set_destination(destination[1].id)
+                Logger.set_info(__name__,
+                                f"{destination[1].name} destination for {destination[0].name}")
+        return 1
+
+    return 0
+
+
+def check_add_exposes(exposes_str_list, **kwargs):
+    """
+    Check and get all "Fun_elem exposes Fun_inter" strings, if Fun_inter is not exposed yet
+    (or parentality relationship) => add it to Fun_elem object and as exposedInterface within xml.
+    Args:
+        exposes_str_list ([strings]): list of strings
+        xml_fun_elem_list ([Fun Elem]) : Functional Element list from xml parsing
+        xml_fun_inter_list ([FunctionalInterface]) : FunctionalInterface list from xml parsing
+        xml_data_list ([Data]) : Data list from xml parsing
+        output_xml (XmlWriter3SE object) : XML's file object
+
+    Returns:
+        [0/1] : if update has been made
+    """
+    # TODO : add physical interface support (see write_element_exposed_interface())
+    xml_fun_elem_list = kwargs['xml_fun_elem_list']
+    xml_fun_inter_list = kwargs['xml_fun_inter_list']
+    output_xml = kwargs['output_xml']
+
+    output = False
+    cleaned_exposes_str_list = util.cut_tuple_list(exposes_str_list)
+    for exposes_str in cleaned_exposes_str_list:
+        fun_elem = question_answer.check_get_object(exposes_str[0], **{'xml_fun_elem_list': xml_fun_elem_list})
+        fun_inter = question_answer.check_get_object(exposes_str[1], **{'xml_fun_inter_list': xml_fun_inter_list})
+
+        check_print_wrong_pair_object((exposes_str[0], fun_elem, 'Functional Element'),
+                                      (exposes_str[1], fun_inter, 'Functional Interface'),
+                                      'exposes')
+        if fun_elem and fun_inter:
+            check_rule = check_fun_elem_inter_families(fun_elem, fun_inter, xml_fun_elem_list)
+            if fun_inter.id not in fun_elem.exposed_interface_list and check_rule:
+                output = True
+                fun_elem.add_exposed_interface(fun_inter.id)
+                output_xml.write_element_exposed_interface([[fun_elem, fun_inter]])
+                Logger.set_info(__name__,
+                                f"{fun_elem.name} exposes {fun_inter.name}")
+
+    if output:
+        return 1
+
+    return 0
+
+
+def check_fun_elem_inter_families(fun_elem, fun_inter, xml_fun_elem_list):
+    """A fun elem can expose an interface if already allocated to a parent/child and
+    an interface can only be exposed by 2 families of fun_elem"""
+    check = True
+    exposed_fun_elem_list = set()
+    for xml_fun_elem in xml_fun_elem_list:
+        if any(s == fun_inter.id for s in xml_fun_elem.exposed_interface_list) and \
+                xml_fun_elem != fun_elem:
+            exposed_fun_elem_list.add(xml_fun_elem)
+
+    if not exposed_fun_elem_list:
+        return check
+
+    opposite_fun_elem_list = []
+    for elem in exposed_fun_elem_list:
+        if question_answer.check_parentality(elem, fun_elem) or \
+                question_answer.check_parentality(fun_elem, elem):
+            return check
+        else:
+            opposite_fun_elem_list.append(elem)
+
+    for idx in range(0, len(opposite_fun_elem_list) - 1):
+        if not question_answer.check_parentality(
+                opposite_fun_elem_list[idx], opposite_fun_elem_list[idx + 1]) and \
+                not question_answer.check_parentality(opposite_fun_elem_list[idx + 1], opposite_fun_elem_list[idx]):
+            check = False
+            return check
+
+    return check
+
+
+def check_print_wrong_pair_object(object_a, object_b, relationship_type):
+    """
+    Prints specific user messages for wrong object(s) pair (Object_a, Object_b) relationship
+
+    Args:
+        object_a: (input_string, object_or_none, object_type_string)
+        e.g. (exposes_str[0], fun_elem, 'Functional Element')
+        object_b: (exposes_str[1], fun_inter, 'Functional Interface')
+        relationship_type: e.g. 'exposes'
+
+    """
+    if object_a[1] == object_b[1] is None:
+        Logger.set_error(__name__,
+                         f"{object_a[0]} and {object_b[0]} do not exist, choose valid names/aliases for: "
+                         f"'{object_a[2]}' {relationship_type} "
+                         f"'{object_b[2]}'")
+    elif object_a[1] is None or object_b[1] is None:
+        if object_a[1] is None and object_b[1]:
+            Logger.set_error(__name__,
+                             f"{object_a[0]} does not exist, choose a valid name/alias for: "
+                             f"'{object_a[2]}' {relationship_type} "
+                             f"{object_b[1].name}")
+        elif object_b[1] is None and object_a[1]:
+            Logger.set_error(__name__,
+                             f"{object_b[0]} does not exist, choose a valid name/alias for: "
+                             f"{object_a[1].name} {relationship_type} "
+                             f"'{object_b[2]}'")
```

### Comparing `jarvis4se-1.3.5/src/jarvis/orchestrator/shared_orchestrator.py` & `jarvis4se-1.4.0/src/jarvis/orchestrator/orchestrator_shared.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1483 +1,1445 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Module containing methods shared between objects/orchestrator"""
-# Libraries
-import re
-import uuid
-
-# Modules
-import datamodel
-from jarvis import question_answer
-from jarvis import util
-from tools import Logger
-
-
-def check_add_child(parent_child_name_str_list, **kwargs):
-    """
-    Check if each string in parent_child_name_str_list are corresponding to an actual object,
-    create new [parent, child] objects lists for object's type : State/Function/FunctionalElement.
-    Send lists to add_child() to write them within xml and then returns update_list from it.
-
-        Parameters:
-            parent_child_name_str_list ([str]) : Lists of string from jarvis cell
-            kwargs (dict) : 4 xml lists(see matched_composition() within command_parser.py)
-            + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-
-    parent_child_lists = [[] for _ in range(4)]
-    available_objects = (datamodel.Function, datamodel.State,
-                         datamodel.FunctionalElement, datamodel.PhysicalElement)
-
-    cleaned_parent_child_list_str = util.cut_tuple_list(parent_child_name_str_list)
-    for elem in cleaned_parent_child_list_str:
-        parent_object = question_answer.check_get_object(elem[0], **kwargs)
-        child_object = question_answer.check_get_object(elem[1], **kwargs)
-        if parent_object is None:
-            if child_object is None:
-                Logger.set_error(__name__,
-                                 f"{elem[0]} and {elem[1]} are not Function/State/FunctionalElement"
-                                 f"/PhysicalElement or the object does not exist")
-            else:
-                Logger.set_error(__name__,
-                                 f"{elem[0]} is not Function/State/FunctionalElement"
-                                 f"/PhysicalElement or the object does not exist")
-            continue
-        if child_object is None:
-            Logger.set_error(__name__,
-                             f"{elem[1]} is not Function/State/FunctionalElement"
-                             f"/PhysicalElement or the object does not exist")
-            continue
-        check_pair = None
-        for idx, obj_type in enumerate(available_objects):
-            if isinstance(parent_object, obj_type) and isinstance(child_object, obj_type):
-                check_pair = idx
-                break
-        if isinstance(check_pair, int):
-            if child_object.parent is None:
-                parent_object.add_child(child_object)
-                child_object.set_parent(parent_object)
-                parent_child_lists[check_pair].append([parent_object, child_object])
-        else:
-            # Single display (not related to logging)
-            print(f"Please choose a valid pair of element(Function/State/FunctionalElement"
-                  f"/PhysicalElement) for {parent_object.name} and {child_object.name}")
-
-    update = add_child(parent_child_lists, kwargs['xml_fun_elem_list'], kwargs['output_xml'])
-
-    return update
-
-
-def add_child(parent_child_lists, xml_fun_elem_list, output_xml):
-    """
-    Check if input lists are not empty, write in xml for each list and return update list if some
-    updates has been made
-
-        Parameters:
-            parent_child_lists ([Parent, Child]) : [[Function],[State],[FunctionalElement],
-            [PhysicalElement]]
-            xml_fun_elem_list ([FunctionalElement]) : functional element list from xml parsing
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
-    """
-    if any(parent_child_lists):
-        for i in range(4):
-            if parent_child_lists[i]:
-                output_xml.write_object_child(parent_child_lists[i])
-                for k in parent_child_lists[i]:
-                    Logger.set_info(__name__,
-                                    f"{k[0].name} is composed of {k[1].name}")
-                    if i in (0, 1):
-                        for fun_elem in xml_fun_elem_list:
-                            if k[0].id in fun_elem.allocated_function_list:
-                                recursive_allocation([fun_elem, k[1]], output_xml)
-        return 1
-
-    return 0
-
-
-def check_add_allocated_item(item, xml_item_list, xml_view_list):
-    """
-    Checks if a view is already activated, if yes check if item isn't already
-    allocated and returns corresponding [View, Object].
-    Args:
-        item (string): Object's name/alias from user's input
-        xml_item_list ([Object]): List of xml's item (same type as item)
-        xml_view_list ([View]) : View list from xml parsing
-
-    Returns:
-        [View, Object]
-    """
-    if not any(s.activated for s in xml_view_list):
-        return None
-
-    activated_view = None
-    for view in xml_view_list:
-        if view.activated:
-            activated_view = view
-            break
-    if activated_view:
-        for i in xml_item_list:
-            if item == i.name:
-                if i.id not in activated_view.allocated_item_list:
-                    activated_view.add_allocated_item(i.id)
-                    return [activated_view, i]
-            # To avoid errors for i.alias when i is Data (no such attriute)
-            try:
-                if item == i.alias:
-                    if i.id not in activated_view.allocated_item_list:
-                        activated_view.add_allocated_item(i.id)
-                        return [activated_view, i]
-            except AttributeError:
-                pass
-
-
-def check_and_delete_object(delete_str_list, **kwargs):
-    """
-    Check if each string in delete_str_list are corresponding to an actual object, create new
-    objects list for objects to delete.
-    Send lists to delete_objects() to delete them within xml and then returns update from it.
-
-        Parameters:
-            delete_str_list ([str]) : List of string from jarvis cell
-            kwargs (dict) : whole xml lists + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    to_be_deleted_obj_lists = [[] for _ in range(10)]
-    # Check if the wanted to delete object exists and can be deleted
-    for obj_str in delete_str_list:
-        object_to_del = question_answer.check_get_object(obj_str, **kwargs)
-        if object_to_del is None:
-            Logger.set_error(__name__,
-                             f"{obj_str} does not exist")
-            continue
-
-        check, list_idx = check_relationship_before_delete(object_to_del, **kwargs)
-        if check:
-            to_be_deleted_obj_lists[list_idx].append(object_to_del)
-        else:
-            Logger.set_error(__name__,
-                             f"{object_to_del.name} can not be deleted")
-
-    update = delete_objects(to_be_deleted_obj_lists, kwargs['output_xml'])
-
-    return update
-
-
-def check_relationship_before_delete(object_to_del, **kwargs):
-    """Switch to trigger differents methods depend object's type"""
-    _, idx = get_basetype_and_idx(object_to_del)
-    switch_check = {
-        0: check_data,
-        1: check_function,
-        2: check_fun_elem,
-        3: check_fun_inter,
-        4: check_phy_elem,
-        5: check_phy_inter,
-        6: check_state,
-        7: check_transition,
-        8: check_attribute,
-        9: check_chain,
-    }
-    check_obj = switch_check.get(idx, "Object can not be deleted")
-    check = check_obj(object_to_del, **kwargs)
-    return check, idx
-
-
-def check_object_not_in_prod_cons(object_to_check, consumer_list, producer_list):
-    """Check if object/data_name not in producer or consumer lists"""
-    check = False
-    if not any(object_to_check in o for o in consumer_list + producer_list):
-        check = True
-    return check
-
-
-def check_object_no_parent_and_child(object_to_check):
-    """Check if an object has not parent and not child"""
-    check = False
-    if not object_to_check.child_list and object_to_check.parent is None:
-        check = True
-
-    return check
-
-
-def check_object_not_allocated(object_to_check, allocated_to_object_list):
-    """Check if object in allocated_list of allocated objects"""
-    check = False
-    if not allocated_to_object_list:
-        check = True
-        return check
-
-    converted_list = list(allocated_to_object_list)
-    if isinstance(object_to_check, datamodel.Function):
-        if isinstance(converted_list[0], (datamodel.State, datamodel.FunctionalElement)):
-            if not any(object_to_check.id in obj.allocated_function_list for obj
-                       in converted_list):
-                check = True
-        if isinstance(converted_list[0], datamodel.View):
-            if not any(object_to_check.id in obj.allocated_item_list for obj
-                       in converted_list):
-                check = True
-    if isinstance(object_to_check, datamodel.Data):
-        if isinstance(converted_list[0], datamodel.View):
-            if not any(object_to_check.id in obj.allocated_item_list for obj
-                       in converted_list):
-                check = True
-        if isinstance(converted_list[0], datamodel.FunctionalInterface):
-            if not any(object_to_check.id in obj.allocated_data_list for obj
-                       in converted_list):
-                check = True
-    if isinstance(object_to_check, datamodel.State):
-        if isinstance(converted_list[0], datamodel.FunctionalElement):
-            if not any(object_to_check.id in obj.allocated_state_list for obj
-                       in converted_list):
-                check = True
-    if isinstance(object_to_check, datamodel.FunctionalElement):
-        if isinstance(converted_list[0], datamodel.PhysicalElement):
-            if not any(object_to_check.id in obj.allocated_fun_elem_list for obj
-                       in converted_list):
-                check = True
-    if isinstance(object_to_check, datamodel.FunctionalInterface):
-        if isinstance(converted_list[0], datamodel.FunctionalElement):
-            if not any(object_to_check.id in obj.exposed_interface_list for obj
-                       in converted_list):
-                check = True
-        if isinstance(converted_list[0], datamodel.PhysicalInterface):
-            if not any(object_to_check.id in obj.allocated_fun_inter_list for obj
-                       in converted_list):
-                check = True
-    if isinstance(object_to_check, datamodel.PhysicalInterface):
-        if isinstance(converted_list[0], datamodel.PhysicalElement):
-            if not any(object_to_check.id in obj.exposed_interface_list for obj
-                       in converted_list):
-                check = True
-    return check
-
-
-def check_object_no_attribute(object_to_check, attribute_list):
-    """Check that object has not attribute set"""
-    check = False
-    described_item_list = [obj.described_item_list for obj in attribute_list]
-    if not any(object_to_check.id in obj for obj in described_item_list):
-        check = True
-    return check
-
-
-def check_function(object_to_del, **kwargs):
-    """Checks for Function's object"""
-    check = False
-    check_list = [False] * 6
-    check_list[0] = check_object_no_parent_and_child(object_to_del)
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has composition relationship(s)")
-
-    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_state_list'])
-    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
-    if not check_list[1] or not check_list[2]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    check_list[3] = check_object_not_in_prod_cons(object_to_del,
-                                                  kwargs['xml_consumer_function_list'],
-                                                  kwargs['xml_producer_function_list'])
-    if not check_list[3]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has production/consumption relationship(s)")
-
-    check_list[4] = check_object_no_attribute(object_to_del, kwargs['xml_attribute_list'])
-    if not check_list[4]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has attribute(s) set")
-
-    check_list[5] = check_object_not_allocated(object_to_del, kwargs['xml_view_list'])
-    if not check_list[5]:
-        Logger.set_info(__name__, f"{object_to_del.name} has chain relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_function_list'].remove(object_to_del)
-    return check
-
-
-def check_data(object_to_del, **kwargs):
-    """Checks for Data's object"""
-    check = False
-    check_list = [False] * 3
-    check_list[0] = check_object_not_in_prod_cons(object_to_del.name,
-                                                  kwargs['xml_consumer_function_list'],
-                                                  kwargs['xml_producer_function_list'])
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has production/consumption relationship(s)")
-
-    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_view_list'])
-    if not check_list[1]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has chain relationship(s)")
-
-    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_inter_list'])
-    if not check_list[2]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_data_list'].remove(object_to_del)
-    return check
-
-
-def check_state(object_to_del, **kwargs):
-    """Checks for State's object"""
-    check = False
-    check_list = [False] * 4
-
-    check_list[0] = check_object_no_parent_and_child(object_to_del)
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has composition relationship(s)")
-
-    check_list[1] = not object_to_del.allocated_function_list
-    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
-    if not check_list[1] or not check_list[2]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    check_list[3] = not any(object_to_del.id in (trans.source, trans.destination)
-                            for trans in kwargs['xml_transition_list'])
-    if not check_list[3]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has transition relationship(s)")
-    if all(check_list):
-        check = True
-        kwargs['xml_state_list'].remove(object_to_del)
-    return check
-
-
-def check_transition(object_to_del, **kwargs):
-    """Checks for State's object"""
-    check = False
-    check_list = [False] * 1
-
-    check_list[0] = object_to_del.source is None and object_to_del.destination is None
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has source/destination relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_transition_list'].remove(object_to_del)
-    return check
-
-
-def check_fun_elem(object_to_del, **kwargs):
-    """Checks for Functional Element's object"""
-    check = False
-    check_list = [False] * 4
-
-    check_list[0] = check_object_no_parent_and_child(object_to_del)
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has composition relationship(s)")
-
-    check_list[1] = (not object_to_del.allocated_function_list and
-                     not object_to_del.allocated_state_list)
-    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_phy_elem_list'])
-    if not check_list[1] or not check_list[2]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    check_list[3] = not object_to_del.exposed_interface_list
-    if not check_list[3]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has interface relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_fun_elem_list'].remove(object_to_del)
-
-    return check
-
-
-def check_chain(object_to_del, **kwargs):
-    """Checks for View's object"""
-    check = False
-    check_list = [False] * 1
-
-    check_list[0] = not object_to_del.allocated_item_list
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_view_list'].remove(object_to_del)
-
-    return check
-
-
-def check_attribute(object_to_del, **kwargs):
-    """Checks for Attribute's object"""
-    check = False
-    check_list = [False] * 1
-
-    check_list[0] = not object_to_del.described_item_list
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has attribute relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_attribute_list'].remove(object_to_del)
-
-    return check
-
-
-def check_fun_inter(object_to_del, **kwargs):
-    """Checks for Functional Interface's object"""
-    check = False
-    check_list = [False] * 3
-
-    check_list[0] = not object_to_del.allocated_data_list
-    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
-    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_phy_inter_list'])
-    if not check_list[0] or not check_list[1] or not check_list[2]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_fun_inter_list'].remove(object_to_del)
-
-    return check
-
-
-def check_phy_elem(object_to_del, **kwargs):
-    """Checks for Physical Element's object"""
-    check = False
-    check_list = [False] * 3
-
-    check_list[0] = check_object_no_parent_and_child(object_to_del)
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has composition relationship(s)")
-
-    check_list[1] = not object_to_del.allocated_fun_elem_list
-    if not check_list[1]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    check_list[2] = not object_to_del.exposed_interface_list
-    if not check_list[2]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has interface relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_phy_elem_list'].remove(object_to_del)
-
-    return check
-
-
-def check_phy_inter(object_to_del, **kwargs):
-    """Checks for Physical Interface's object"""
-    check = False
-    check_list = [False] * 2
-
-    check_list[0] = not object_to_del.allocated_fun_inter_list
-    if not check_list[0]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has allocation relationship(s)")
-
-    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_phy_elem_list'])
-    if not check_list[1]:
-        Logger.set_info(__name__,
-                        f"{object_to_del.name} has interface relationship(s)")
-
-    if all(check_list):
-        check = True
-        kwargs['xml_phy_inter_list'].remove(object_to_del)
-
-    return check
-
-
-def delete_objects(object_lists, output_xml):
-    """
-    Check if input lists are not empty, write in xml for each list and return update list if some
-    updates has been made
-
-        Parameters:
-            object_lists : see order in get_basetype_and_idx()
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            1 if update, else 0
-    """
-    if any(object_lists):
-        for i in range(10):
-            if object_lists[i]:
-                output_xml.delete_object(object_lists[i])
-                for object_type in object_lists[i]:
-                    Logger.set_info(__name__,
-                                    f"{object_type.name} deleted")
-        return 1
-    return 0
-
-
-def check_set_object_type(type_str_list, **kwargs):
-    """
-    Check if each string in type_str_list are corresponding to an actual object's name/alias, create
-    [objects] ordered lists(as BaseType(Enum)) for:
-    [[Data], [Function],[FunctionalElement], [FuncitonalInterface],[PhysicalElement],
-    [PhysicalInterface], [State],[Transition],[Attribute],[View]]
-    Send lists to set_object_type() to write them within xml and then returns update from it.
-
-        Parameters:
-            type_str_list ([str]) : Lists of string from jarvis cell
-            kwargs (dict) : whole xml lists + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    object_type_lists = [[] for _ in range(10)]
-    # Check if the wanted object exists and the type can be set
-    for object_str, type_name in type_str_list:
-        object_to_set = question_answer.check_get_object(object_str, **kwargs)
-        if object_to_set is None:
-            Logger.set_error(__name__,
-                             f"{object_str} does not exist")
-            continue
-        if object_to_set.type == type_name:
-            continue
-        check, basetype_idx = check_new_type(object_to_set, type_name, kwargs['xml_type_list'])
-        if check:
-            object_type_lists[basetype_idx].append(object_to_set)
-
-    update = set_object_type(object_type_lists, kwargs['output_xml'])
-
-    return update
-
-
-def check_new_type(object_to_set, type_name, xml_type_list):
-    """Check if type in specity object's type list and if changed"""
-    check = False
-    basetype_idx = None
-    obj_base_type = get_basetype_and_idx(object_to_set)
-    # print(specific_obj_type_list, list_idx)
-    if obj_base_type and type_name != object_to_set.type:
-        if type_name.capitalize().replace("_", " ") in [str(i) for i in datamodel.BaseType]:
-            basetype_idx = obj_base_type.value
-            check = True
-            object_to_set.set_type(obj_base_type)
-        elif any(t == type_name for t in question_answer.get_objects_names(xml_type_list)):
-            obj_type = question_answer.check_get_object(type_name, **{'xml_type_list': xml_type_list})
-            check = check_type_recursively(obj_type)
-            if not check:
-                Logger.set_info(__name__,
-                                f"{obj_type.name} is not base type: "
-                                f"{str(obj_base_type)}")
-            else:
-                basetype_idx = obj_base_type.value
-                object_to_set.set_type(obj_type)
-        else:
-            Logger.set_error(__name__,
-                             f"The type {type_name} does not exist, available types are "
-                             f": {', '.join([str(i) for i in datamodel.BaseType])}.")
-
-    return check, basetype_idx
-
-
-def check_type_recursively(obj_type):
-    """Checks type.base recursively if it within specific_obj_type_list"""
-    check = False
-    if isinstance(obj_type.base, (datamodel.BaseType, str)):
-        check = True
-        return check
-    elif isinstance(obj_type.base, datamodel.Type):
-        return check_type_recursively(obj_type.base)
-    return check
-
-
-def get_basetype_and_idx(object_to_set):
-    """Return BaseType according to object's type"""
-    # Tuple order is same as datamodel.BaseType(Enum)
-    class_obj_tuple = (datamodel.Data, datamodel.Function, datamodel.FunctionalElement,
-                       datamodel.FunctionalInterface, datamodel.PhysicalElement, datamodel.PhysicalInterface,
-                       datamodel.State, datamodel.Transition, datamodel.Attribute, datamodel.View)
-
-    for idx, i in enumerate(class_obj_tuple):
-        if isinstance(object_to_set, i):
-            return datamodel.BaseType(idx)
-
-    return None
-
-
-def set_object_type(object_lists, output_xml):
-    """
-    Check if input lists are not empty, write in xml for each list and return update list if some
-    updates has been made
-
-        Parameters:
-            object_lists : see order in get_basetype_and_idx()
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            1 if update, else 0
-    """
-    if any(object_lists):
-        for i in range(10):
-            if object_lists[i]:
-                output_xml.write_object_type(object_lists[i])
-                for object_type in object_lists[i]:
-                    if isinstance(object_type.type, datamodel.BaseType):
-                        type_name = str(object_type.type)
-                    else:
-                        type_name = object_type.type.name
-                    Logger.set_info(__name__,
-                                    f"The type of {object_type.name} is {type_name}")
-        return 1
-    return 0
-
-
-def check_set_object_alias(alias_str_list, **kwargs):
-    """
-    Check if each string in alias_str_list are corresponding to an actual object's name/alias,
-    create [objects] ordered lists for:
-    [[Function],[State],[Transition],[FunctionalElement],[Attribute],
-    [FuncitonalInterface],[PhysicalElement],[PhysicalInterface]]
-    Send lists to set_object_type() to write them within xml and then returns update from it.
-
-        Parameters:
-            alias_str_list ([str]) : Lists of string from jarvis cell
-            kwargs (dict) : whole xml lists + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    object_lists = [[] for _ in range(9)]
-    # Check if the wanted to object exists and the type can be set
-    for object_to_set_alias, alias_str in alias_str_list:
-        object_to_set = question_answer.check_get_object(object_to_set_alias, **kwargs)
-        if object_to_set is None:
-            Logger.set_error(__name__,
-                             f"{object_to_set_alias} does not exist")
-            continue
-
-        idx = check_new_alias(object_to_set, alias_str)
-        if isinstance(idx, int):
-            object_lists[idx].append(object_to_set)
-
-    update = set_object_alias(object_lists, kwargs['output_xml'])
-
-    return update
-
-
-def check_new_alias(object_to_set, alias_str):
-    """Check that alias is new and object has en alias attribute, then returns corresponding
-    object's type index"""
-    check = None
-    try:
-        if object_to_set.alias == alias_str:
-            return check
-    except AttributeError:
-        print(f"{object_to_set.name} object does not have alias attribute")
-        return check
-    if isinstance(object_to_set, datamodel.Type):
-        object_to_set.set_alias(alias_str)
-        return 0
-
-    base_type = get_base_type_recursively(object_to_set.type)
-    if isinstance(base_type, datamodel.BaseType):
-        # Data() and View() do not have aliases attributes
-        if base_type.value not in (0, 9):
-            object_to_set.set_alias(alias_str)
-            return base_type.value
-
-    return check
-
-
-def set_object_alias(object_lists, output_xml):
-    """
-    Check if input lists are not empty, write in xml for each list and return update if some
-    updates has been made.
-        Parameters:
-            object_lists ([Object]) : object with new alias
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            1 if update, else 0
-    """
-    if any(object_lists):
-        for i in range(9):
-            if object_lists[i]:
-                output_xml.write_object_alias(object_lists[i])
-                for object_alias in object_lists[i]:
-                    Logger.set_info(__name__,
-                                    f"The alias for {object_alias.name} is {object_alias.alias}")
-
-        return 1
-
-    return 0
-
-
-def check_add_allocation(allocation_str_list, **kwargs):
-    """
-    Check if each string in allocation_str_list are corresponding to an actual object's name/alias,
-    create lists for:
-    [[FunctionalElement, Function/State], [FunctionalInterface, Data],[State, Function],
-    [PhysicalElement, FunctionalElement], [PhysicalInterface, FunctionalInterface]]
-    Send lists to add_allocation() to write them within xml and then returns update from it.
-
-        Parameters:
-            allocation_str_list ([str]) : Lists of string from jarvis cell
-            kwargs (dict) : whole xml lists + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    new_allocation = {
-        0: [],  # [FunctionalElement, Function/State]
-        1: [],  # [State, Function]
-        2: [],  # [FunctionalInterface, Data]
-        3: [],  # [PhysicalElement, FunctionalElement]
-        4: [],  # [PhysicalInterface, FunctionalInterface]
-        # 5: [],  [View, Object] in other modules or [Fun_elem_Parent, Function/State] in
-        # check_parent_allocation() it's just a key with no recursivety
-    }
-    for elem in allocation_str_list:
-        alloc_obj = question_answer.check_get_object(elem[0],
-                                                     **{'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                                        'xml_state_list': kwargs['xml_state_list'],
-                                                        'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                                        'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
-                                                        'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
-                                                        })
-        obj_to_alloc = question_answer.check_get_object(elem[1],
-                                                        **{'xml_function_list': kwargs['xml_function_list'],
-                                                           'xml_state_list': kwargs['xml_state_list'],
-                                                           'xml_data_list': kwargs['xml_data_list'],
-                                                           'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                                           'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                                           })
-        check_obj = check_allocation_objects_types(alloc_obj, obj_to_alloc, elem)
-        if not check_obj:
-            continue
-        check_rule, alloc = check_allocation_rules(alloc_obj, obj_to_alloc, **kwargs)
-        if check_rule and alloc:
-            new_allocation[alloc[0]].append(alloc[1])
-
-    update = add_allocation(new_allocation, kwargs['output_xml'])
-
-    return update
-
-
-def check_allocation_objects_types(alloc_obj, obj_to_alloc, elem):
-    """Check that alloc_obj within is FunctionalElement or FunctionalInterface or State or
-    PhysicalElement or PhysicalInterface AND obj_to_alloc is Function/State or Data or
-    FunctionalElement or FunctionalInterface"""
-    check = True
-    if alloc_obj is None and obj_to_alloc is None:
-        print_wrong_obj_allocation(elem)
-        check = False
-    elif alloc_obj is None or obj_to_alloc is None:
-        if alloc_obj is None:
-            print_wrong_obj_allocation(elem[0])
-            check = False
-        elif obj_to_alloc is None:
-            print_wrong_obj_allocation(elem[1])
-            check = False
-
-    return check
-
-
-def print_wrong_obj_allocation(obj_str):
-    """Print relative message to wrong pair allocations"""
-    if isinstance(obj_str, tuple):
-        name_str = f"Objects {obj_str[0]} and {obj_str[1]}"
-    else:
-        name_str = f"Object {obj_str}"
-
-    Logger.set_error(__name__,
-                     name_str + " not found or can not be allocated, "
-                                "available allocations are: \n"
-                                "(Functional Element allocates State/Function) OR \n"
-                                "(State allocates Function) OR \n"
-                                "(Functional Interface allocates Data) OR \n"
-                                "(Physical Element allocates Functional Element) OR \n"
-                                "(Physical Interface allocates Functional Interface)\n")
-
-
-def check_allocation_rules(alloc_obj, obj_to_alloc, **kwargs):
-    """Check "good" combinations, trigger specific check and then return check and new tuple
-    allocation"""
-    check = False
-    new_alloc = None
-    if isinstance(alloc_obj, datamodel.FunctionalElement):
-        if isinstance(obj_to_alloc, (datamodel.Function, datamodel.State)):
-            check = True
-            pair = check_fun_elem_allocation(alloc_obj, obj_to_alloc, kwargs['xml_fun_elem_list'])
-            if pair:
-                new_alloc = [0, pair]
-        else:
-            print_wrong_obj_allocation(obj_to_alloc.name)
-    elif isinstance(alloc_obj, datamodel.State):
-        if isinstance(obj_to_alloc, datamodel.Function):
-            check = True
-            pair = check_state_allocation(alloc_obj, obj_to_alloc, kwargs['xml_state_list'])
-            if pair:
-                new_alloc = [1, pair]
-        else:
-            print_wrong_obj_allocation(obj_to_alloc.name)
-    elif isinstance(alloc_obj, datamodel.FunctionalInterface):
-        if isinstance(obj_to_alloc, datamodel.Data):
-            check = True
-            pair = check_fun_inter_allocation(alloc_obj, obj_to_alloc, **kwargs)
-            if pair:
-                new_alloc = [2, pair]
-        else:
-            print_wrong_obj_allocation(obj_to_alloc.name)
-    elif isinstance(alloc_obj, datamodel.PhysicalElement):
-        if isinstance(obj_to_alloc, datamodel.FunctionalElement):
-            check = True
-        else:
-            print_wrong_obj_allocation(obj_to_alloc.name)
-    elif isinstance(alloc_obj, datamodel.PhysicalInterface):
-        if isinstance(obj_to_alloc, datamodel.FunctionalInterface):
-            check = True
-        else:
-            print_wrong_obj_allocation(obj_to_alloc.name)
-
-    return check, new_alloc
-
-
-def check_fun_elem_allocation(fun_elem, obj_to_alloc, fun_elem_list):
-    """Check allocation rules for fun_elem then returns objects if check"""
-    count = None
-    out = None
-    check_allocation = question_answer.get_allocation_object(obj_to_alloc, fun_elem_list)
-    if check_allocation is not None:
-        count = len(check_allocation)
-        for item in check_allocation:
-            # Checks if they are in the same family
-            if not question_answer.check_not_family(item, fun_elem) and item != fun_elem:
-                count -= 1
-
-    if count in (None, 0):
-        if isinstance(obj_to_alloc, datamodel.State):
-            fun_elem.add_allocated_state(obj_to_alloc.id)
-        else:
-            fun_elem.add_allocated_function(obj_to_alloc.id)
-        out = [fun_elem, obj_to_alloc]
-
-    return out
-
-
-def check_state_allocation(state, function, state_list):
-    """Check allocation rules for state then returns objects if check"""
-    out = None
-    check_allocation = question_answer.get_allocation_object(function, state_list)
-    if check_allocation is None:
-        state.add_allocated_function(function.id)
-        out = [state, function]
-    else:
-        if state not in check_allocation:
-            state.add_allocated_function(function.id)
-            out = [state, function]
-
-    return out
-
-
-def check_fun_inter_allocation(fun_inter, data, **kwargs):
-    """Check allocation rules for fun_inter then returns objects if check"""
-    out = None
-    check_allocation_fun_inter = question_answer.get_allocation_object(data, kwargs['xml_fun_inter_list'])
-    if check_allocation_fun_inter is None:
-        check_fe = check_fun_elem_data_consumption(
-            data, fun_inter,
-            kwargs['xml_fun_elem_list'],
-            kwargs['xml_function_list'],
-            kwargs['xml_consumer_function_list'],
-            kwargs['xml_producer_function_list'])
-        if all(i for i in check_fe):
-            out = [fun_inter, data]
-            fun_inter.add_allocated_data(data.id)
-        elif True in check_fe:
-            if check_fe[0] is True:
-                Logger.set_error(__name__,
-                                 f"Data {data.name} has only consumer(s) "
-                                 f"allocated to a functional element exposing "
-                                 f"{fun_inter.name}, {data.name} not "
-                                 f"allocated to {fun_inter.name}")
-            elif check_fe[1] is True:
-                Logger.set_error(__name__,
-                                 f"Data {data.name} has only producer(s) "
-                                 f"allocated to a functional element exposing "
-                                 f"{fun_inter.name}, {data.name} not "
-                                 f"allocated to {fun_inter.name}")
-        else:
-            Logger.set_error(__name__,
-                             f"Data {data.name} has no producer(s) nor "
-                             f"consumer(s) allocated to functional elements "
-                             f"exposing {fun_inter.name}, {data.name} not "
-                             f"allocated to {fun_inter.name}")
-
-    return out
-
-
-def check_fun_elem_data_consumption(data, fun_inter, fun_elem_list, function_list,
-                                    xml_consumer_function_list, xml_producer_function_list):
-    """Check if for a fun_inter, the fun_elem exposing it has allocated functions producing and
-    consuming that data"""
-    fun_elem_exposes = set()
-    for fun_elem in fun_elem_list:
-        if any(a == fun_inter.id for a in fun_elem.exposed_interface_list):
-            fun_elem_exposes.add(fun_elem)
-
-    cons_list = False
-    prod_list = False
-    for function in function_list:
-        for fun_elem in fun_elem_exposes:
-            if any(a == function.id for a in fun_elem.allocated_function_list):
-                fun_data = [data.name, function]
-                if any(a == fun_data for a in xml_consumer_function_list):
-                    cons_list = True
-                if any(a == fun_data for a in xml_producer_function_list):
-                    prod_list = True
-
-    return [cons_list, prod_list]
-
-
-def add_allocation(allocation_dict, output_xml):
-    """
-    Check if allocation_lists is not empty, write in xml for each list and return 0/1
-    if some update has been made.
-
-        Parameters:
-            allocation_dict : Containing all allocation to write within xml
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            1 if update, else 0
-    """
-    if any(allocation_dict.values()):
-        for _, k in enumerate(allocation_dict):
-            if allocation_dict[k]:
-                output_xml.write_object_allocation(allocation_dict[k])
-                # Warn the user once added within xml
-                for elem in allocation_dict[k]:
-                    Logger.set_info(__name__,
-                                    f"{elem[1].__class__.__name__} {elem[1].name} is allocated to "
-                                    f"{elem[0].__class__.__name__} {elem[0].name}")
-                    # Check the dict length, if this method is called from viewpoint_orchestrator
-                    # or functional_orchestrator for View => Only key[0] and no recursion wanted
-                    if k in (0, 1):
-                        recursive_allocation(elem, output_xml)
-        return 1
-    return 0
-
-
-def check_parent_allocation(elem, output_xml):
-    """Check if parent's Function/Sate are allocated to parent's Fucntional Element:
-    if not print message to user asking if he wants to, if yes write it in xml then continue
-    with parents"""
-    if elem[0].parent is not None and elem[1].parent is not None:
-        fun_elem_parent = elem[0].parent
-        object_parent = elem[1].parent
-        check = False
-        if isinstance(elem[1], datamodel.State):
-            if object_parent.id in fun_elem_parent.allocated_state_list:
-                check = True
-        elif isinstance(elem[1], datamodel.Function):
-            if object_parent.id in fun_elem_parent.allocated_function_list:
-                check = True
-        if not check:
-            answer = input(f"Do you also want to allocate parents(i.e. {object_parent.name} "
-                           f"to {fun_elem_parent.name}) ?(Y/N)")
-            if answer.lower() == "y":
-                if isinstance(elem[1], datamodel.State):
-                    fun_elem_parent.add_allocated_state(object_parent.id)
-                else:
-                    fun_elem_parent.add_allocated_function(object_parent.id)
-
-                add_allocation({5: [[fun_elem_parent, object_parent]]}, output_xml)
-                check_parent_allocation([fun_elem_parent, object_parent], output_xml)
-            else:
-                Logger.set_error(__name__,
-                                 f"{object_parent.name} is not allocated despite at least one "
-                                 f"of its child is")
-
-
-def recursive_allocation(elem, output_xml):
-    """Recursive allocation for childs of State/Function"""
-    check_parent_allocation(elem, output_xml)
-    object_type = question_answer.get_object_type(elem[1])
-    if elem[1].child_list:
-        for i in elem[1].child_list:
-            parent_child = [elem[1], i]
-            allocated_child_list = get_allocated_child(parent_child, [elem[0]])
-            if allocated_child_list:
-                for item in allocated_child_list:
-                    if isinstance(elem[1], datamodel.State):
-                        item[0].add_allocated_state(item[1].id)
-                    else:
-                        item[0].add_allocated_function(item[1].id)
-                # We want recursivety so it trigger for (0, 1) keys in the dict
-                add_allocation({0: allocated_child_list}, output_xml)
-    else:
-        # TBT/TBC
-        if object_type == "state" and elem[1].id not in elem[0].allocated_state_list:
-            elem[0].add_allocated_state(elem[1].id)
-            Logger.set_info(__name__,
-                            f"State {elem[1].name} is allocated to functional "
-                            f"element {elem[0].name}")
-        elif object_type == "function" and elem[1].id not in elem[0].allocated_function_list:
-            elem[0].add_allocated_function(elem[1].id)
-            Logger.set_info(__name__,
-                            f"Function {elem[1].name} is allocated to functional "
-                            f"element {elem[0].name}")
-
-
-def get_allocated_child(elem, xml_fun_elem_list):
-    """
-    Check if the parent state/function is already allocated to a fun elem and create list to add
-    its child also (if not already allocated)
-
-        Parameters:
-            elem ([State/Function]) : parent object, child object
-            xml_fun_elem_list ([FunctionalElement]) : functional element list from xml parsing
-
-        Returns:
-            output_list ([FunctionalElement, State/Function]) : Allocation Relationships that need
-            to be added
-    """
-    output_list = []
-    for fun_elem in xml_fun_elem_list:
-        if isinstance(elem[0], datamodel.State):
-            # To avoid "RuntimeError: Set changed size during iteration" copy()
-            allocated_list = fun_elem.allocated_state_list.copy()
-        else:
-            allocated_list = fun_elem.allocated_function_list.copy()
-        if allocated_list:
-            for allocated_object in allocated_list:
-                if allocated_object == elem[0].id:
-                    if elem[1].id not in allocated_list:
-                        if isinstance(elem[0], datamodel.State):
-                            fun_elem.add_allocated_state(elem[1].id)
-                        else:
-                            fun_elem.add_allocated_function(elem[1].id)
-                        output_list.append([fun_elem, elem[1]])
-
-    return output_list
-
-
-def check_add_inheritance(inherit_str_list, **kwargs):
-    """
-    Check if each string in allocation_str_list are corresponding to an actual object's name/alias,
-    set_derive, create lists of objets.
-    Send lists to add_derived() to write them within xml and then returns update from it.
-
-        Parameters:
-            inherit_str_list ([str]) : Lists of string from jarvis cell
-            kwargs (dict) : whole xml lists + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    new_list = []
-    for elem in inherit_str_list:
-        # elem_0: inheriting object
-        elem_0 = question_answer.check_get_object(elem[0],
-                                                  **{'xml_function_list': kwargs['xml_function_list'],
-                                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
-                                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
-                                                     })
-        # elem_1: object to inherit from
-        elem_1 = question_answer.check_get_object(elem[1],
-                                                  **{'xml_function_list': kwargs['xml_function_list'],
-                                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
-                                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
-                                                     })
-        if not elem_0 or not elem_1:
-            if not elem_0 and not elem_1:
-                print_wrong_object_inheritance(elem[0], elem[1])
-            elif not elem_0:
-                print_wrong_object_inheritance(elem[0])
-            else:
-                print_wrong_object_inheritance(elem[1])
-            continue
-        if elem_0 == elem_1:
-            Logger.set_warning(__name__,
-                               f"Same object {elem_0.name}")
-            continue
-        if elem_0.derived == elem_1:
-            continue
-
-        check_obj = check_inheritance(elem_0, elem_1)
-        if not check_obj:
-            continue
-        new_list.append(elem_0)
-
-    if not new_list:
-        return 0
-
-    add_derived(new_list, kwargs['output_xml'])
-    return 1
-
-
-def print_wrong_object_inheritance(*obj):
-    """Prints wrong object(s) message for inheritance from input string"""
-    if len(obj) == 2:
-        user_message = f"{obj[0]} and {obj[1]}"
-    else:
-        user_message = f"{obj[0]}"
-
-    Logger.set_error(__name__,
-                     f"{user_message} not found, available objects for inheritance are:\n"
-                     "- Function\n"
-                     "- Functional element\n"
-                     "- Functional interface\n"
-                     "- Physical element\n"
-                     "- Physical element\n")
-
-
-def check_inheritance(elem_0, elem_1):
-    """Returns check if pair are compatible and object list have been updated"""
-    inheritance_type_list = [datamodel.Function, datamodel.FunctionalElement,
-                             datamodel.FunctionalInterface, datamodel.PhysicalElement,
-                             datamodel.PhysicalInterface]
-
-    type_found = None
-    for idx, inheritance_type in enumerate(inheritance_type_list):
-        if isinstance(elem_0, inheritance_type) and isinstance(elem_1, inheritance_type):
-            type_found = idx
-            break
-
-    if type_found is None:
-        Logger.set_error(__name__,
-                         f"{elem_0.__class__.__name__} and {elem_1.__class__.__name__} "
-                         f"are not of the same type")
-        return False
-
-    elem_0.set_derived(elem_1)
-    return True
-
-
-def add_derived(object_list, output_xml):
-    """
-    Check if input lists are not empty, write in xml for each list and return update if some
-    updates has been made.
-        Parameters:
-            object_list ([Object]) : object with new derived
-            output_xml (XmlWriter3SE object) : XML's file object
-
-        Returns:
-            1 if update, else 0
-    """
-    if any(object_list):
-        output_xml.write_object_derived(object_list)
-        for obj in object_list:
-            Logger.set_info(__name__,
-                            f"{obj.name} inherited from {obj.derived.name}")
-        return 1
-    return 0
-
-
-class CreateObjInstance:
-    def __init__(self, obj_str, base_type, specific_obj_type=None, **kwargs):
-        self.specific_obj_type = specific_obj_type
-        self.base_type = base_type
-        self.base_type_idx = datamodel.BaseType.get_enum(
-            str(self.base_type)).value
-        self.new_obj = self.create_obj(obj_str)
-        # Data() and View() do not have aliases
-        if not isinstance(self.new_obj, (datamodel.Data, datamodel.View)):
-            self.create_alias(obj_str)
-        self.add_obj_to_xml_set(**kwargs)
-
-    def create_obj(self, obj_str):
-        self.base_type_idx = datamodel.BaseType.get_enum(
-            str(self.base_type)).value
-        switch_obj_list = {
-            0: datamodel.Data,
-            1: datamodel.Function,
-            2: datamodel.FunctionalElement,
-            3: datamodel.FunctionalInterface,
-            4: datamodel.PhysicalElement,
-            5: datamodel.PhysicalInterface,
-            6: datamodel.State,
-            7: datamodel.Transition,
-        }
-        call = switch_obj_list.get(self.base_type_idx)
-        if self.specific_obj_type is None:
-            return call(p_name=obj_str, p_id=get_unique_id())
-        return call(p_name=obj_str, p_id=get_unique_id(), p_type=self.specific_obj_type)
-
-    def create_alias(self, obj_str):
-        alias_str = re.search(r"(.*)\s[-]\s", obj_str, re.MULTILINE)
-        if alias_str:
-            self.new_obj.set_alias(alias_str.group(1))
-
-    def add_obj_to_xml_set(self, **kwargs):
-        switch_obj_list = {
-            0: kwargs['xml_data_list'].add,
-            1: kwargs['xml_function_list'].add,
-            2: kwargs['xml_fun_elem_list'].add,
-            3: kwargs['xml_fun_inter_list'].add,
-            4: kwargs['xml_phy_elem_list'].add,
-            5: kwargs['xml_phy_inter_list'].add,
-            6: kwargs['xml_state_list'].add,
-            7: kwargs['xml_transition_list'].add,
-        }
-        call = switch_obj_list.get(self.base_type_idx)
-        return call(self.new_obj)
-
-    def return_obj(self):
-        return self.new_obj, self.base_type_idx
-
-
-xml_str_lists = ['xml_function_list', 'xml_data_list', 'xml_state_list', 'xml_fun_elem_list',
-                 'xml_transition_list', 'xml_fun_inter_list', 'xml_phy_elem_list',
-                 'xml_phy_inter_list', 'xml_attribute_list', 'xml_view_list', 'xml_type_list']
-
-
-def check_add_specific_obj_by_type(obj_type_str_list, **kwargs):
-    """
-    Check if each string in obj_type_str_list are corresponding to an actual object's name/alias,
-    set_derive, create object_lists with list per obj. Send lists to add_obj_to_xml()
-    write them within xml and then returns update from it.
-
-        Parameters:
-            obj_type_str_list ([str]) : Lists of string from jarvis cell
-            kwargs (dict) : whole xml lists + xml's file object
-
-        Returns:
-            update ([0/1]) : 1 if update, else 0
-    """
-    object_lists = [[] for _ in range(8)]
-    for elem in obj_type_str_list:
-        spec_obj_type = None
-        base_type = None
-        if elem[1].capitalize() in [str(i) for i in datamodel.BaseType]:
-            base_type = next((i for i in [str(i) for i in datamodel.BaseType]
-                              if i == elem[1].capitalize()))
-        else:
-            spec_obj_type = question_answer.check_get_object(elem[1],
-                                                             **{'xml_type_list': kwargs['xml_type_list']})
-            if not spec_obj_type:
-                Logger.set_error(__name__,
-                                 f"No valid type found for {elem[1]}")
-                continue
-            base_type = get_base_type_recursively(spec_obj_type)
-        if base_type is None:
-            Logger.set_error(__name__,
-                             f"No valid base type found for {elem[1]}")
-            continue
-
-        xml_names_list = question_answer.get_objects_name_lists(
-            **{key: value for (key, value) in kwargs.items() if key in xml_str_lists})
-        flat_names_list = [item for sublist in xml_names_list for item in sublist]
-        if any(n == elem[0] for n in flat_names_list):
-            # Maybe we can warn user
-            continue
-        new_obj, base_type_idx = CreateObjInstance(
-            elem[0],
-            base_type,
-            spec_obj_type,
-            **kwargs
-        ).return_obj()
-        if isinstance(new_obj.type, datamodel.BaseType):
-            type_name = str(new_obj.type)
-        else:
-            type_name = new_obj.type.name
-
-        Logger.set_info(__name__,
-                        f"{new_obj.name} is a {type_name}")
-
-        object_lists[base_type_idx].append(new_obj)
-
-    if any(object_lists):
-        return add_obj_to_xml(object_lists, kwargs['output_xml'])
-    return 0
-
-
-def get_base_type_recursively(obj_type):
-    """Checks type: if it's a BaseType or its base else recursively return """
-    if isinstance(obj_type, datamodel.BaseType):
-        return obj_type
-    elif obj_type.base in [str(i) for i in datamodel.BaseType]:
-        return obj_type.base
-    return get_base_type_recursively(obj_type.base)
-
-
-def get_unique_id():
-    """Generate and set unique identifier of length 10 integers"""
-    identifier = uuid.uuid4()
-    return str(identifier.int)[:10]
-
-
-def add_obj_to_xml(object_lists, output_xml):
-    """Send lists object to respective methods of XmlWriter3SE, returns 1 if at least one obj has
-    been written"""
-    switch_write_obj = {
-        0: output_xml.write_data,
-        1: output_xml.write_function,
-        2: output_xml.write_functional_element,
-        3: output_xml.write_functional_interface,
-        4: output_xml.write_physical_element,
-        5: output_xml.write_physical_interface,
-        6: output_xml.write_state,
-        7: output_xml.write_transition,
-    }
-    check = 0
-    for idx, sub in enumerate(object_lists):
-        if sub:
-            switch_write_obj.get(idx)(sub)
-            check = 1
-    return check
-
-
-# Inheritance start here - Should be moved/refactored after validation
-def childs_inheritance(*xml_obj_set, level=None):
-    """Check if object from xml_obj_set is derived, if yes:
-    - call derived_childs()
-    - returns derived_parent_dict of derived objects id, derived_child_set of derived objects and
-    derived_child_id_list
-    Parameter:
-    - obj: set() of objects
-    - level: diagram level"""
-    derived_child_set = set()
-    derived_parent_dict = {}
-    derived_child_id_list = set()
-
-    for xml_set in xml_obj_set:
-        for elem in xml_set:
-            if elem.derived:
-                partial_child_set, partial_par_dict, partial_child_id_set = derived_childs(elem,
-                                                                                           level)
-                derived_child_set = derived_child_set.union(partial_child_set)
-                derived_parent_dict.update(partial_par_dict)
-                derived_child_id_list = derived_child_id_list.union(partial_child_id_set)
-
-    return derived_child_set, derived_parent_dict, derived_child_id_list
-
-
-def derived_childs(obj, level):
-    """Add derived object childs to object and set derived parent to object"""
-    derived_parent_dict = {}
-
-    [obj.add_child(c) for c in obj.derived.child_list
-     if c.parent == obj.derived]
-    [c.set_parent(obj) for c in obj.derived.child_list
-     if c.parent == obj.derived]
-    for child in obj.derived.child_list:
-        derived_parent_dict[str(child.id)] = str(obj.id)
-    derived_child_set = question_answer.get_children(obj.derived, level=level)[0]
-    derived_child_id_list = {c.id for c in obj.derived.child_list}
-    obj.derived.child_list.clear()
-    derived_child_set.remove(obj.derived)
-
-    return derived_child_set, derived_parent_dict, derived_child_id_list
-
-
-def reset_childs_inheritance(*xml_obj_set, derived_child_id=None):
-    """Check if there is first level derived child id list, if yes reset original child/parent
-    relationships"""
-    if derived_child_id:
-        for xml_set in xml_obj_set:
-            for elem in xml_set:
-                if elem.derived:
-                    child_pop = [c for c in elem.child_list
-                                 if c.id in [f for f in derived_child_id]]
-                    [elem.derived.add_child(c) for c in child_pop]
-                    [c.set_parent(elem.derived) for c in child_pop]
-
-
-def attribute_inheritance(xml_attribute_set, *xml_object_set):
-    """Attribute inheritance"""
-    modified_attrib_set = set()
-    derived_elem = set()
-
-    for xml_set in xml_object_set:
-        [derived_elem.add(e) for e in xml_set if e.derived]
-
-    for attribute in xml_attribute_set:
-        for obj_id, value in attribute.described_item_list.copy():
-            for der_obj in derived_elem:
-                if obj_id == der_obj.derived.id:
-                    attribute.add_described_item((der_obj.id, value))
-                    modified_attrib_set.add((attribute.id, der_obj.id, value))
-
-    return modified_attrib_set
-
-
-def reset_attribute_inheritance(xml_attribute_set, to_be_reset_id_set):
-    """Reset attributes"""
-    for attribute in xml_attribute_set:
-        [attribute.described_item_list.remove((e[1], e[2])) for e in to_be_reset_id_set
-         if e[0] == attribute.id]
-
-
-def view_inheritance(xml_view_set, *xml_obj_set):
-    """View inheritance"""
-    temp_view_set = set()
-    derived_elem_set = set()
-
-    for xml_set in xml_obj_set:
-        [derived_elem_set.add(e) for e in xml_set if e.derived]
-
-    for view in xml_view_set:
-        for item_id in view.allocated_item_list.copy():
-            for obj in derived_elem_set:
-                if item_id == obj.derived.id:
-                    temp_view_set.add((view.id, obj.id))
-                    view.add_allocated_item(obj.id)
-
-    return temp_view_set
-
-
-def reset_view_inheritance(xml_view_set, to_be_removed_id):
-    """Reset views"""
-    for view in xml_view_set:
-        for ids in to_be_removed_id:
-            if view.id == ids[0]:
-                view.allocated_item_list.remove(ids[1])
-
-
-def allocation_inheritance(xml_obj_set, xml_allocated_obj_set):
-    """Allocation Inheritance"""
-    alloc_to_reset = []
-    for elem in xml_obj_set:
-        if elem.derived:
-            if isinstance(elem, datamodel.FunctionalElement):
-                pair = [elem, {i for i in elem.derived.allocated_function_list
-                               if i not in elem.allocated_function_list}]
-                elem.allocated_function_list = elem.allocated_function_list.union(
-                    elem.derived.allocated_function_list)
-                alloc_to_reset.append(pair)
-            if isinstance(elem, datamodel.FunctionalInterface):
-                pair = [elem, {i for i in elem.derived.allocated_data_list
-                               if i not in elem.allocated_data_list}]
-                elem.allocated_data_list = elem.allocated_data_list.union(
-                    elem.derived.allocated_data_list)
-                alloc_to_reset.append(pair)
-
-    return alloc_to_reset
-
-
-def reset_alloc_inheritance(pairs_to_reset):
-    """Reset Allocation Inheritance"""
-    for pair in pairs_to_reset:
-        if isinstance(pair[0], datamodel.FunctionalElement):
-            [pair[0].allocated_function_list.remove(fun_id) for fun_id in pair[1]]
-        if isinstance(pair[0], datamodel.FunctionalInterface):
-            [pair[0].allocated_data_list.remove(data_id) for data_id in pair[1]]
+"""@defgroup jarvis
+Jarvis module
+"""
+# Libraries
+
+# Modules
+import datamodel
+from . import orchestrator_object
+from jarvis.query import question_answer
+from jarvis import util
+from tools import Logger
+
+
+def check_add_child(parent_child_name_str_list, **kwargs):
+    """
+    Check if each string in parent_child_name_str_list are corresponding to an actual object,
+    create new [parent, child] objects lists for object's type : State/Function/FunctionalElement.
+    Send lists to add_child() to write them within xml and then returns update_list from it.
+
+        Parameters:
+            parent_child_name_str_list ([str]) : Lists of string from jarvis cell
+            kwargs (dict) : 4 xml lists(see matched_composition() within command_parser.py)
+            + xml's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+
+    parent_child_lists = [[] for _ in range(len(datamodel.TypeWithChildList))]
+
+    cleaned_parent_child_list_str = util.cut_tuple_list(parent_child_name_str_list)
+    for elem in cleaned_parent_child_list_str:
+        parent_object = question_answer.check_get_object(elem[0], **kwargs)
+        child_object = question_answer.check_get_object(elem[1], **kwargs)
+        if parent_object is not None and child_object is not None:
+            check_pair = None
+            for idx, obj_type in enumerate(datamodel.TypeWithChildList):
+                if isinstance(parent_object, obj_type) and isinstance(child_object, obj_type):
+                    check_pair = idx
+                    break
+            if isinstance(check_pair, int):
+                if child_object.parent is None:
+                    parent_object.add_child(child_object)
+                    child_object.set_parent(parent_object)
+                    parent_child_lists[check_pair].append([parent_object, child_object])
+                elif child_object.parent.id != parent_object.id:
+                    Logger.set_warning(__name__, f"{elem[1]} has already a parent: {child_object.parent.name}")
+            else:
+                # Single display (not related to logging)
+                print(f"Please choose a valid pair of element(Function/State/FunctionalElement"
+                      f"/PhysicalElement) for {parent_object.name} and {child_object.name}")
+        elif parent_object is None:
+            Logger.set_error(__name__, f"{elem[0]} does not exist")
+        else:
+            Logger.set_error(__name__, f"{elem[1]} does not exist")
+
+    update = add_child(parent_child_lists, **kwargs)
+
+    return update
+
+
+def add_child(parent_child_lists, **kwargs):
+    """
+    Check if input lists are not empty, write in xml for each list and return update list if some
+    updates has been made
+
+        Parameters:
+            parent_child_lists ([Parent, Child]) : [[Function],[State],[FunctionalElement],
+            [PhysicalElement]]
+            xml_fun_elem_list ([FunctionalElement]) : functional element list from xml parsing
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
+    """
+    update = 0
+    if any(parent_child_lists):
+        xml_fun_elem_list = kwargs['xml_fun_elem_list']
+        output_xml = kwargs['output_xml']
+        for object_type in range(len(datamodel.TypeWithChildList)):
+            if parent_child_lists[object_type]:
+                output_xml.write_object_child(parent_child_lists[object_type])
+                update = 1
+
+                for obj in parent_child_lists[object_type]:
+                    Logger.set_info(__name__,
+                                    f"{obj[0].name} is composed of {obj[1].name}")
+                    if object_type in (datamodel.TypeWithChildListFunctionIndex, datamodel.TypeWithChildListStateIndex):
+                        # Considering function and state allocation to a functional element
+                        for fun_elem in xml_fun_elem_list:
+                            if obj[0].id in fun_elem.allocated_function_list:
+                                allocate_all_children_in_element([fun_elem, obj[1]], **kwargs)
+
+                        if object_type == datamodel.TypeWithChildListFunctionIndex:
+                            # Considering function allocation
+                            xml_consumer_function_list = kwargs['xml_consumer_function_list']
+                            xml_producer_function_list = kwargs['xml_producer_function_list']
+
+                            for (flow, function) in xml_consumer_function_list:
+                                if obj[1].id == function.id and [flow, obj[0]] not in xml_consumer_function_list:
+                                    if [flow, obj[0]] not in xml_producer_function_list:
+                                        output_xml.write_data_consumer([[flow, obj[0]]])
+                                        xml_consumer_function_list.append([flow, obj[0]])
+
+                                        Logger.set_info(__name__, f"{obj[0].name} produces {flow}")
+                                    else:
+                                        # Case of a parent child is producing the data
+                                        output_xml.delete_data_relationship([flow, obj[0]], "producer")
+                                        xml_producer_function_list.remove([flow, obj[0]])
+
+                                        Logger.set_info(__name__, f"{obj[0].name} does not produce {flow} anymore")
+
+                            for (flow, function) in xml_producer_function_list:
+                                if obj[1].id == function.id and [flow, obj[0]] not in xml_producer_function_list:
+                                    if [flow, obj[0]] not in xml_consumer_function_list:
+                                        output_xml.write_data_producer([[flow, obj[0]]])
+                                        xml_producer_function_list.append([flow, obj[0]])
+
+                                        Logger.set_info(__name__, f"{obj[0].name} consumes {flow}")
+                                    else:
+                                        # Case of a parent child is consuming the data
+                                        output_xml.delete_data_relationship([flow, obj[0]], "consumer")
+                                        xml_consumer_function_list.remove([flow, obj[0]])
+
+                                        Logger.set_info(__name__, f"{obj[0].name} does not consume {flow} anymore")
+
+    return update
+
+
+def check_add_allocated_item(item, xml_item_list, xml_view_list):
+    """
+    Checks if a view is already activated, if yes check if item isn't already
+    allocated and returns corresponding [View, Object].
+    Args:
+        item (string): Object's name/alias from user's input
+        xml_item_list ([Object]): List of xml's item (same type as item)
+        xml_view_list ([View]) : View list from xml parsing
+
+    Returns:
+        [View, Object]
+    """
+    if not any(s.activated for s in xml_view_list):
+        return None
+
+    activated_view = None
+    for view in xml_view_list:
+        if view.activated:
+            activated_view = view
+            break
+    if activated_view:
+        for i in xml_item_list:
+            if item == i.name:
+                if i.id not in activated_view.allocated_item_list:
+                    activated_view.add_allocated_item(i.id)
+                    return [activated_view, i]
+            # To avoid errors for i.alias when i is Data (no such attriute)
+            try:
+                if item == i.alias:
+                    if i.id not in activated_view.allocated_item_list:
+                        activated_view.add_allocated_item(i.id)
+                        return [activated_view, i]
+            except AttributeError:
+                pass
+
+
+def check_and_delete_object(delete_str_list, **kwargs):
+    """
+    Check if each string in delete_str_list are corresponding to an actual object, create new
+    objects list for objects to delete.
+    Send lists to delete_objects() to delete them within xml and then returns update from it.
+
+        Parameters:
+            delete_str_list ([str]) : List of string from jarvis cell
+            kwargs (dict) : whole xml lists + xml's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+    to_be_deleted_obj_lists = [[] for _ in range(10)]
+    # Check if the wanted to delete object exists and can be deleted
+    for obj_str in delete_str_list:
+        object_to_del = question_answer.check_get_object(obj_str, **kwargs)
+        if object_to_del is None:
+            Logger.set_error(__name__,
+                             f"{obj_str} does not exist")
+            continue
+
+        check, list_idx = check_relationship_before_delete(object_to_del, **kwargs)
+        if check:
+            to_be_deleted_obj_lists[list_idx].append(object_to_del)
+        else:
+            Logger.set_error(__name__,
+                             f"{object_to_del.name} can not be deleted")
+
+    update = delete_objects(to_be_deleted_obj_lists, kwargs['output_xml'])
+
+    return update
+
+
+def check_relationship_before_delete(object_to_del, **kwargs):
+    """Switch to trigger differents methods depend object's type"""
+    _, idx = get_basetype_and_idx(object_to_del)
+    switch_check = {
+        0: check_data,
+        1: check_function,
+        2: check_fun_elem,
+        3: check_fun_inter,
+        4: check_phy_elem,
+        5: check_phy_inter,
+        6: check_state,
+        7: check_transition,
+        8: check_attribute,
+        9: check_chain,
+    }
+    check_obj = switch_check.get(idx, "Object can not be deleted")
+    check = check_obj(object_to_del, **kwargs)
+    return check, idx
+
+
+def check_object_not_in_prod_cons(object_to_check, consumer_list, producer_list):
+    """Check if object/data_name not in producer or consumer lists"""
+    check = False
+    if not any(object_to_check in o for o in consumer_list + producer_list):
+        check = True
+    return check
+
+
+def check_object_no_parent_and_child(object_to_check):
+    """Check if an object has not parent and not child"""
+    check = False
+    if not object_to_check.child_list and object_to_check.parent is None:
+        check = True
+
+    return check
+
+
+def check_object_not_allocated(object_to_check, allocated_to_object_list):
+    """Check if object in allocated_list of allocated objects"""
+    check = False
+    if not allocated_to_object_list:
+        check = True
+        return check
+
+    converted_list = list(allocated_to_object_list)
+    if isinstance(object_to_check, datamodel.Function):
+        if isinstance(converted_list[0], (datamodel.State, datamodel.FunctionalElement)):
+            if not any(object_to_check.id in obj.allocated_function_list for obj
+                       in converted_list):
+                check = True
+        if isinstance(converted_list[0], datamodel.View):
+            if not any(object_to_check.id in obj.allocated_item_list for obj
+                       in converted_list):
+                check = True
+    if isinstance(object_to_check, datamodel.Data):
+        if isinstance(converted_list[0], datamodel.View):
+            if not any(object_to_check.id in obj.allocated_item_list for obj
+                       in converted_list):
+                check = True
+        if isinstance(converted_list[0], datamodel.FunctionalInterface):
+            if not any(object_to_check.id in obj.allocated_data_list for obj
+                       in converted_list):
+                check = True
+    if isinstance(object_to_check, datamodel.State):
+        if isinstance(converted_list[0], datamodel.FunctionalElement):
+            if not any(object_to_check.id in obj.allocated_state_list for obj
+                       in converted_list):
+                check = True
+    if isinstance(object_to_check, datamodel.FunctionalElement):
+        if isinstance(converted_list[0], datamodel.PhysicalElement):
+            if not any(object_to_check.id in obj.allocated_fun_elem_list for obj
+                       in converted_list):
+                check = True
+    if isinstance(object_to_check, datamodel.FunctionalInterface):
+        if isinstance(converted_list[0], datamodel.FunctionalElement):
+            if not any(object_to_check.id in obj.exposed_interface_list for obj
+                       in converted_list):
+                check = True
+        if isinstance(converted_list[0], datamodel.PhysicalInterface):
+            if not any(object_to_check.id in obj.allocated_fun_inter_list for obj
+                       in converted_list):
+                check = True
+    if isinstance(object_to_check, datamodel.PhysicalInterface):
+        if isinstance(converted_list[0], datamodel.PhysicalElement):
+            if not any(object_to_check.id in obj.exposed_interface_list for obj
+                       in converted_list):
+                check = True
+    return check
+
+
+def check_object_no_attribute(object_to_check, attribute_list):
+    """Check that object has not attribute set"""
+    check = False
+    described_item_list = [obj.described_item_list for obj in attribute_list]
+    if not any(object_to_check.id in obj for obj in described_item_list):
+        check = True
+    return check
+
+
+def check_function(object_to_del, **kwargs):
+    """Checks for Function's object"""
+    check = False
+    check_list = [False] * 6
+    check_list[0] = check_object_no_parent_and_child(object_to_del)
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has composition relationship(s)")
+
+    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_state_list'])
+    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
+    if not check_list[1] or not check_list[2]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    check_list[3] = check_object_not_in_prod_cons(object_to_del,
+                                                  kwargs['xml_consumer_function_list'],
+                                                  kwargs['xml_producer_function_list'])
+    if not check_list[3]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has production/consumption relationship(s)")
+
+    check_list[4] = check_object_no_attribute(object_to_del, kwargs['xml_attribute_list'])
+    if not check_list[4]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has attribute(s) set")
+
+    check_list[5] = check_object_not_allocated(object_to_del, kwargs['xml_view_list'])
+    if not check_list[5]:
+        Logger.set_info(__name__, f"{object_to_del.name} has chain relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_function_list'].remove(object_to_del)
+    return check
+
+
+def check_data(object_to_del, **kwargs):
+    """Checks for Data's object"""
+    check = False
+    check_list = [False] * 3
+    check_list[0] = check_object_not_in_prod_cons(object_to_del.name,
+                                                  kwargs['xml_consumer_function_list'],
+                                                  kwargs['xml_producer_function_list'])
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has production/consumption relationship(s)")
+
+    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_view_list'])
+    if not check_list[1]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has chain relationship(s)")
+
+    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_inter_list'])
+    if not check_list[2]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_data_list'].remove(object_to_del)
+    return check
+
+
+def check_state(object_to_del, **kwargs):
+    """Checks for State's object"""
+    check = False
+    check_list = [False] * 4
+
+    check_list[0] = check_object_no_parent_and_child(object_to_del)
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has composition relationship(s)")
+
+    check_list[1] = not object_to_del.allocated_function_list
+    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
+    if not check_list[1] or not check_list[2]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    check_list[3] = not any(object_to_del.id in (trans.source, trans.destination)
+                            for trans in kwargs['xml_transition_list'])
+    if not check_list[3]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has transition relationship(s)")
+    if all(check_list):
+        check = True
+        kwargs['xml_state_list'].remove(object_to_del)
+    return check
+
+
+def check_transition(object_to_del, **kwargs):
+    """Checks for State's object"""
+    check = False
+    check_list = [False] * 1
+
+    check_list[0] = object_to_del.source is None and object_to_del.destination is None
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has source/destination relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_transition_list'].remove(object_to_del)
+    return check
+
+
+def check_fun_elem(object_to_del, **kwargs):
+    """Checks for Functional Element's object"""
+    check = False
+    check_list = [False] * 4
+
+    check_list[0] = check_object_no_parent_and_child(object_to_del)
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has composition relationship(s)")
+
+    check_list[1] = (not object_to_del.allocated_function_list and
+                     not object_to_del.allocated_state_list)
+    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_phy_elem_list'])
+    if not check_list[1] or not check_list[2]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    check_list[3] = not object_to_del.exposed_interface_list
+    if not check_list[3]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has interface relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_fun_elem_list'].remove(object_to_del)
+
+    return check
+
+
+def check_chain(object_to_del, **kwargs):
+    """Checks for View's object"""
+    check = False
+    check_list = [False] * 1
+
+    check_list[0] = not object_to_del.allocated_item_list
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_view_list'].remove(object_to_del)
+
+    return check
+
+
+def check_attribute(object_to_del, **kwargs):
+    """Checks for Attribute's object"""
+    check = False
+    check_list = [False] * 1
+
+    check_list[0] = not object_to_del.described_item_list
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has attribute relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_attribute_list'].remove(object_to_del)
+
+    return check
+
+
+def check_fun_inter(object_to_del, **kwargs):
+    """Checks for Functional Interface's object"""
+    check = False
+    check_list = [False] * 3
+
+    check_list[0] = not object_to_del.allocated_data_list
+    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
+    check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_phy_inter_list'])
+    if not check_list[0] or not check_list[1] or not check_list[2]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_fun_inter_list'].remove(object_to_del)
+
+    return check
+
+
+def check_phy_elem(object_to_del, **kwargs):
+    """Checks for Physical Element's object"""
+    check = False
+    check_list = [False] * 3
+
+    check_list[0] = check_object_no_parent_and_child(object_to_del)
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has composition relationship(s)")
+
+    check_list[1] = not object_to_del.allocated_fun_elem_list
+    if not check_list[1]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    check_list[2] = not object_to_del.exposed_interface_list
+    if not check_list[2]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has interface relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_phy_elem_list'].remove(object_to_del)
+
+    return check
+
+
+def check_phy_inter(object_to_del, **kwargs):
+    """Checks for Physical Interface's object"""
+    check = False
+    check_list = [False] * 2
+
+    check_list[0] = not object_to_del.allocated_fun_inter_list
+    if not check_list[0]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has allocation relationship(s)")
+
+    check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_phy_elem_list'])
+    if not check_list[1]:
+        Logger.set_info(__name__,
+                        f"{object_to_del.name} has interface relationship(s)")
+
+    if all(check_list):
+        check = True
+        kwargs['xml_phy_inter_list'].remove(object_to_del)
+
+    return check
+
+
+def delete_objects(object_lists, output_xml):
+    """
+    Check if input lists are not empty, write in xml for each list and return update list if some
+    updates has been made
+
+        Parameters:
+            object_lists : see order in get_basetype_and_idx()
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            1 if update, else 0
+    """
+    if any(object_lists):
+        for i in range(10):
+            if object_lists[i]:
+                output_xml.delete_object(object_lists[i])
+                for object_type in object_lists[i]:
+                    Logger.set_info(__name__,
+                                    f"{object_type.name} deleted")
+        return 1
+    return 0
+
+
+def check_set_object_type(type_str_list, **kwargs):
+    """
+    Check if each string in type_str_list are corresponding to an actual object's name/alias, create
+    [objects] ordered lists(as BaseType(Enum)) for:
+    [[Data], [Function],[FunctionalElement], [FuncitonalInterface],[PhysicalElement],
+    [PhysicalInterface], [State],[Transition],[Attribute],[View]]
+    Send lists to set_object_type() to write them within xml and then returns update from it.
+
+        Parameters:
+            type_str_list ([str]) : Lists of string from jarvis cell
+            kwargs (dict) : whole xml lists + xml's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+    object_type_lists = [[] for _ in range(10)]
+    # Check if the wanted object exists and the type can be set
+    for object_str, type_name in type_str_list:
+        object_to_set = question_answer.check_get_object(object_str, **kwargs)
+        if object_to_set is None:
+            Logger.set_error(__name__,
+                             f"{object_str} does not exist")
+            continue
+        if object_to_set.type == type_name:
+            continue
+        check, basetype_idx = check_new_type(object_to_set, type_name, kwargs['xml_type_list'])
+        if check:
+            object_type_lists[basetype_idx].append(object_to_set)
+
+    update = set_object_type(object_type_lists, kwargs['output_xml'])
+
+    return update
+
+
+def check_new_type(object_to_set, type_name, xml_type_list):
+    """Check if type in specity object's type list and if changed"""
+    check = False
+    basetype_idx = None
+    obj_base_type = get_basetype_and_idx(object_to_set)
+    # print(specific_obj_type_list, list_idx)
+    if obj_base_type and type_name != object_to_set.type:
+        if type_name.capitalize().replace("_", " ") in [str(i) for i in datamodel.BaseType]:
+            basetype_idx = obj_base_type.value
+            check = True
+            object_to_set.set_type(obj_base_type)
+        elif any(t == type_name for t in question_answer.get_objects_names(xml_type_list)):
+            obj_type = question_answer.check_get_object(type_name, **{'xml_type_list': xml_type_list})
+            check = check_type_recursively(obj_type)
+            if not check:
+                Logger.set_info(__name__,
+                                f"{obj_type.name} is not base type: "
+                                f"{str(obj_base_type)}")
+            else:
+                basetype_idx = obj_base_type.value
+                object_to_set.set_type(obj_type)
+        else:
+            Logger.set_error(__name__,
+                             f"The type {type_name} does not exist, available types are "
+                             f": {', '.join([str(i) for i in datamodel.BaseType])}.")
+
+    return check, basetype_idx
+
+
+def check_type_recursively(obj_type):
+    """Checks type.base recursively if it within specific_obj_type_list"""
+    check = False
+    if isinstance(obj_type.base, (datamodel.BaseType, str)):
+        check = True
+        return check
+    elif isinstance(obj_type.base, datamodel.Type):
+        return check_type_recursively(obj_type.base)
+    return check
+
+
+def get_basetype_and_idx(object_to_set):
+    """Return BaseType according to object's type"""
+    # Tuple order is same as datamodel.BaseType(Enum)
+    class_obj_tuple = (datamodel.Data, datamodel.Function, datamodel.FunctionalElement,
+                       datamodel.FunctionalInterface, datamodel.PhysicalElement, datamodel.PhysicalInterface,
+                       datamodel.State, datamodel.Transition, datamodel.Attribute, datamodel.View)
+
+    for idx, i in enumerate(class_obj_tuple):
+        if isinstance(object_to_set, i):
+            return datamodel.BaseType(idx)
+
+    return None
+
+
+def set_object_type(object_lists, output_xml):
+    """
+    Check if input lists are not empty, write in xml for each list and return update list if some
+    updates has been made
+
+        Parameters:
+            object_lists : see order in get_basetype_and_idx()
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            1 if update, else 0
+    """
+    if any(object_lists):
+        for i in range(10):
+            if object_lists[i]:
+                output_xml.write_object_type(object_lists[i])
+                for object_type in object_lists[i]:
+                    if isinstance(object_type.type, datamodel.BaseType):
+                        type_name = str(object_type.type)
+                    else:
+                        type_name = object_type.type.name
+                    Logger.set_info(__name__,
+                                    f"The type of {object_type.name} is {type_name}")
+        return 1
+    return 0
+
+
+def check_set_object_alias(alias_str_list, **kwargs):
+    """
+    Check if each string in alias_str_list are corresponding to an actual object's name/alias,
+    create [objects] ordered lists for:
+    [[Function],[State],[Transition],[FunctionalElement],[Attribute],
+    [FuncitonalInterface],[PhysicalElement],[PhysicalInterface]]
+    Send lists to set_object_type() to write them within xml and then returns update from it.
+
+        Parameters:
+            alias_str_list ([str]) : Lists of string from jarvis cell
+            kwargs (dict) : whole xml lists + xml's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+    object_lists = [[] for _ in range(9)]
+    # Check if the wanted to object exists and the type can be set
+    for object_to_set_alias, alias_str in alias_str_list:
+        object_to_set = question_answer.check_get_object(object_to_set_alias, **kwargs)
+        if object_to_set is None:
+            Logger.set_error(__name__,
+                             f"{object_to_set_alias} does not exist")
+            continue
+
+        idx = check_new_alias(object_to_set, alias_str)
+        if isinstance(idx, int):
+            object_lists[idx].append(object_to_set)
+
+    update = set_object_alias(object_lists, kwargs['output_xml'])
+
+    return update
+
+
+def check_new_alias(object_to_set, alias_str):
+    """Check that alias is new and object has en alias attribute, then returns corresponding
+    object's type index"""
+    check = None
+    try:
+        if object_to_set.alias == alias_str:
+            return check
+    except AttributeError:
+        print(f"{object_to_set.name} object does not have alias attribute")
+        return check
+    if isinstance(object_to_set, datamodel.Type):
+        object_to_set.set_alias(alias_str)
+        return 0
+
+    base_type = orchestrator_object.get_base_type_recursively(object_to_set.type)
+    if isinstance(base_type, datamodel.BaseType):
+        # Data() and View() do not have aliases attributes
+        if base_type.value not in (0, 9):
+            object_to_set.set_alias(alias_str)
+            return base_type.value
+
+    return check
+
+
+def set_object_alias(object_lists, output_xml):
+    """
+    Check if input lists are not empty, write in xml for each list and return update if some
+    updates has been made.
+        Parameters:
+            object_lists ([Object]) : object with new alias
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            1 if update, else 0
+    """
+    if any(object_lists):
+        for i in range(9):
+            if object_lists[i]:
+                output_xml.write_object_alias(object_lists[i])
+                for object_alias in object_lists[i]:
+                    Logger.set_info(__name__,
+                                    f"The alias for {object_alias.name} is {object_alias.alias}")
+
+        return 1
+
+    return 0
+
+
+def check_add_allocation(allocation_str_list, **kwargs):
+    """
+    Check if each string in allocation_str_list are corresponding to an actual object's name/alias,
+    create lists for:
+    [[FunctionalElement, Function/State], [FunctionalInterface, Data],[State, Function],
+    [PhysicalElement, FunctionalElement], [PhysicalInterface, FunctionalInterface]]
+    Send lists to add_allocation() to write them within xml and then returns update from it.
+
+        Parameters:
+            allocation_str_list ([str]) : Lists of string from jarvis cell
+            kwargs (dict) : whole xml lists + xml's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+    new_allocation = {
+        0: [],  # [FunctionalElement, Function/State]
+        1: [],  # [State, Function]
+        2: [],  # [FunctionalInterface, Data]
+        3: [],  # [PhysicalElement, FunctionalElement]
+        4: [],  # [PhysicalInterface, FunctionalInterface]
+        # 5: [],  [View, Object] in other modules or [Fun_elem_Parent, Function/State] in
+        # check_parent_allocation() it's just a key with no recursivety
+    }
+    cleaned_allocation_str_list = util.cut_tuple_list(allocation_str_list)
+    for elem in cleaned_allocation_str_list:
+        alloc_obj = question_answer.check_get_object(elem[0],
+                                                     **{'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                        'xml_state_list': kwargs['xml_state_list'],
+                                                        'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                        'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
+                                                        'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
+                                                        })
+        obj_to_alloc = question_answer.check_get_object(elem[1],
+                                                        **{'xml_function_list': kwargs['xml_function_list'],
+                                                           'xml_state_list': kwargs['xml_state_list'],
+                                                           'xml_data_list': kwargs['xml_data_list'],
+                                                           'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                           'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                           })
+        check_obj = check_allocation_objects_types(alloc_obj, obj_to_alloc, elem)
+        if not check_obj:
+            continue
+        check_rule, alloc = check_allocation_rules(alloc_obj, obj_to_alloc, **kwargs)
+        if check_rule and alloc:
+            new_allocation[alloc[0]].append(alloc[1])
+
+    update = add_allocation(new_allocation, **kwargs)
+
+    return update
+
+
+def check_allocation_objects_types(alloc_obj, obj_to_alloc, elem):
+    """Check that alloc_obj within is FunctionalElement or FunctionalInterface or State or
+    PhysicalElement or PhysicalInterface AND obj_to_alloc is Function/State or Data or
+    FunctionalElement or FunctionalInterface"""
+    check = True
+    if alloc_obj is None and obj_to_alloc is None:
+        print_wrong_obj_allocation(elem)
+        check = False
+    elif alloc_obj is None or obj_to_alloc is None:
+        if alloc_obj is None:
+            print_wrong_obj_allocation(elem[0])
+            check = False
+        elif obj_to_alloc is None:
+            print_wrong_obj_allocation(elem[1])
+            check = False
+
+    return check
+
+
+def print_wrong_obj_allocation(obj_str):
+    """Print relative message to wrong pair allocations"""
+    if isinstance(obj_str, tuple):
+        name_str = f"Objects {obj_str[0]} and {obj_str[1]}"
+    else:
+        name_str = f"Object {obj_str}"
+
+    Logger.set_error(__name__,
+                     name_str + " not found or can not be allocated, "
+                                "available allocations are: \n"
+                                "(Functional Element allocates State/Function) OR \n"
+                                "(State allocates Function) OR \n"
+                                "(Functional Interface allocates Data) OR \n"
+                                "(Physical Element allocates Functional Element) OR \n"
+                                "(Physical Interface allocates Functional Interface)")
+
+
+def check_allocation_rules(alloc_obj, obj_to_alloc, **kwargs):
+    """Check "good" combinations, trigger specific check and then return check and new tuple
+    allocation"""
+    check = False
+    new_alloc = None
+    if isinstance(alloc_obj, datamodel.FunctionalElement):
+        if isinstance(obj_to_alloc, (datamodel.Function, datamodel.State)):
+            check = True
+            pair = check_fun_elem_allocation(alloc_obj, obj_to_alloc, kwargs['xml_fun_elem_list'])
+            if pair:
+                new_alloc = [0, pair]
+        else:
+            print_wrong_obj_allocation(obj_to_alloc.name)
+    elif isinstance(alloc_obj, datamodel.State):
+        if isinstance(obj_to_alloc, datamodel.Function):
+            check = True
+            pair = check_state_allocation(alloc_obj, obj_to_alloc, kwargs['xml_state_list'])
+            if pair:
+                new_alloc = [1, pair]
+        else:
+            print_wrong_obj_allocation(obj_to_alloc.name)
+    elif isinstance(alloc_obj, datamodel.FunctionalInterface):
+        if isinstance(obj_to_alloc, datamodel.Data):
+            check = True
+            pair = check_fun_inter_allocation(alloc_obj, obj_to_alloc, **kwargs)
+            if pair:
+                new_alloc = [2, pair]
+        else:
+            print_wrong_obj_allocation(obj_to_alloc.name)
+    elif isinstance(alloc_obj, datamodel.PhysicalElement):
+        if isinstance(obj_to_alloc, datamodel.FunctionalElement):
+            check = True
+        else:
+            print_wrong_obj_allocation(obj_to_alloc.name)
+    elif isinstance(alloc_obj, datamodel.PhysicalInterface):
+        if isinstance(obj_to_alloc, datamodel.FunctionalInterface):
+            check = True
+        else:
+            print_wrong_obj_allocation(obj_to_alloc.name)
+
+    return check, new_alloc
+
+
+def check_fun_elem_allocation(fun_elem, obj_to_alloc, fun_elem_list):
+    """Check allocation rules for fun_elem then returns objects if check"""
+    count = None
+    out = None
+    check_allocation = question_answer.get_allocation_object(obj_to_alloc, fun_elem_list)
+    if check_allocation is not None:
+        count = len(check_allocation)
+        for item in check_allocation:
+            # Checks if they are in the same family
+            if not question_answer.check_not_family(item, fun_elem) and item != fun_elem:
+                count -= 1
+
+    if count in (None, 0):
+        if isinstance(obj_to_alloc, datamodel.State):
+            fun_elem.add_allocated_state(obj_to_alloc.id)
+        else:
+            fun_elem.add_allocated_function(obj_to_alloc.id)
+        out = [fun_elem, obj_to_alloc]
+
+    return out
+
+
+def check_state_allocation(state, function, state_list):
+    """Check allocation rules for state then returns objects if check"""
+    out = None
+    check_allocation = question_answer.get_allocation_object(function, state_list)
+    if check_allocation is None:
+        state.add_allocated_function(function.id)
+        out = [state, function]
+    else:
+        if state not in check_allocation:
+            state.add_allocated_function(function.id)
+            out = [state, function]
+
+    return out
+
+
+def check_fun_inter_allocation(fun_inter, data, **kwargs):
+    """Check allocation rules for fun_inter then returns objects if check"""
+    out = None
+    check_allocation_fun_inter = question_answer.get_allocation_object(data, kwargs['xml_fun_inter_list'])
+    if check_allocation_fun_inter is None:
+        check_fe = check_fun_elem_data_consumption(
+            data, fun_inter,
+            kwargs['xml_fun_elem_list'],
+            kwargs['xml_function_list'],
+            kwargs['xml_consumer_function_list'],
+            kwargs['xml_producer_function_list'])
+        if all(i for i in check_fe):
+            out = [fun_inter, data]
+            fun_inter.add_allocated_data(data.id)
+        elif True in check_fe:
+            if check_fe[0] is True:
+                Logger.set_error(__name__,
+                                 f"Data {data.name} has only consumer(s) "
+                                 f"allocated to a functional element exposing "
+                                 f"{fun_inter.name}, {data.name} not "
+                                 f"allocated to {fun_inter.name}")
+            elif check_fe[1] is True:
+                Logger.set_error(__name__,
+                                 f"Data {data.name} has only producer(s) "
+                                 f"allocated to a functional element exposing "
+                                 f"{fun_inter.name}, {data.name} not "
+                                 f"allocated to {fun_inter.name}")
+        else:
+            Logger.set_error(__name__,
+                             f"Data {data.name} has no producer(s) nor "
+                             f"consumer(s) allocated to functional elements "
+                             f"exposing {fun_inter.name}, {data.name} not "
+                             f"allocated to {fun_inter.name}")
+
+    return out
+
+
+def check_fun_elem_data_consumption(data, fun_inter, fun_elem_list, function_list,
+                                    xml_consumer_function_list, xml_producer_function_list):
+    """Check if for a fun_inter, the fun_elem exposing it has allocated functions producing and
+    consuming that data"""
+    fun_elem_exposes = set()
+    for fun_elem in fun_elem_list:
+        if any(a == fun_inter.id for a in fun_elem.exposed_interface_list):
+            fun_elem_exposes.add(fun_elem)
+
+    is_consumer = False
+    is_producer = False
+    for function in function_list:
+        for fun_elem in fun_elem_exposes:
+            if any(a == function.id for a in fun_elem.allocated_function_list):
+                fun_data = [data.name, function]
+                if any(a == fun_data for a in xml_consumer_function_list):
+                    is_consumer = True
+                if any(a == fun_data for a in xml_producer_function_list):
+                    is_producer = True
+                if is_consumer or is_producer:
+                    for child in fun_elem.child_list:
+                        if child in fun_elem_exposes and \
+                                not any(a == function.id for a in child.allocated_function_list):
+                            Logger.set_warning(__name__,
+                                               f'Child {child.name} of Functional element {fun_elem.name} exposes also '
+                                               f'the Functional interface {fun_inter.name}. Please consider to '
+                                               f'allocate the Function {function.name} to it.')
+
+    return [is_consumer, is_producer]
+
+
+def add_allocation(allocation_dict, **kwargs):
+    """
+    Check if allocation_lists is not empty, write in xml for each list and return 0/1
+    if some update has been made.
+
+        Parameters:
+            allocation_dict : Containing all allocation to write within xml
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            1 if update, else 0
+    """
+    if any(allocation_dict.values()):
+        for _, k in enumerate(allocation_dict):
+            if allocation_dict[k]:
+                output_xml = kwargs['output_xml']
+                output_xml.write_object_allocation(allocation_dict[k])
+                # Warn the user once added within xml
+                for elem in allocation_dict[k]:
+                    Logger.set_info(__name__,
+                                    f"{elem[1].__class__.__name__} {elem[1].name} is allocated to "
+                                    f"{elem[0].__class__.__name__} {elem[0].name}")
+                    if k == 1:
+                        # Allocation of [State, Function]
+                        # Need to remove previous allocation if any
+                        xml_fun_elem_list = kwargs['xml_fun_elem_list']
+                        xml_state_list = kwargs['xml_state_list']
+                        for xml_state in xml_state_list:
+                            if xml_state.id != elem[0].id:
+                                if elem[1].id in xml_state.allocated_function_list:
+                                    is_fun_elem = False
+                                    for xml_fun_elem in xml_fun_elem_list:
+                                        if xml_state.id in xml_fun_elem.allocated_state_list:
+                                            is_fun_elem = True
+                                            if elem[0].id not in xml_fun_elem.allocated_state_list:
+                                                xml_state.remove_allocated_function(elem[1].id)
+                                                output_xml.delete_object_allocation([[xml_state, elem[1]]])
+                                                Logger.set_info(__name__,
+                                                                f"Function {elem[1].name} is not allocated to "
+                                                                f"State {xml_state.name} anymore")
+                                                xml_fun_elem.remove_allocated_function(elem[1].id)
+                                                output_xml.delete_object_allocation([[xml_fun_elem, elem[1]]])
+                                                Logger.set_info(__name__,
+                                                                f"Function {elem[1].name} is not allocated to "
+                                                                f"Functional element {xml_fun_elem.name} anymore")
+
+                                            else:
+                                                Logger.set_info(__name__,
+                                                                f"Function {elem[1].name} is still allocated to "
+                                                                f"State {xml_state.name}")
+                                                Logger.set_info(__name__,
+                                                                f"Function {elem[1].name} is still allocated to "
+                                                                f"Functional element {xml_fun_elem.name}")
+                                        # Else do nothing
+
+                                    if not is_fun_elem:
+                                        xml_state.remove_allocated_function(elem[1].id)
+                                        output_xml.delete_object_allocation([[xml_state, elem[1]]])
+                                        Logger.set_info(__name__,
+                                                        f"Function {elem[1].name} is not allocated to "
+                                                        f"State {xml_state.name} anymore")
+                                # Else do nothing
+                            # Else do nothing
+
+                        # Finalize allocation
+                        for xml_fun_elem in xml_fun_elem_list:
+                            # Check if state is allocated to functional element to allocate function to
+                            # functional element
+                            if elem[0].id in xml_fun_elem.allocated_state_list and elem[1].id not in \
+                                    xml_fun_elem.allocated_function_list:
+                                xml_fun_elem.add_allocated_function(elem[1].id)
+                                output_xml.write_object_allocation([[xml_fun_elem, elem[1]]])
+                                Logger.set_info(__name__,
+                                                f"{elem[1].__class__.__name__} {elem[1].name} is allocated to "
+                                                f"{xml_fun_elem.__class__.__name__} {xml_fun_elem.name}")
+                            # Check if state is not allocated to functional element to allocate state to
+                            # functional element
+                            elif elem[0].id not in xml_fun_elem.allocated_state_list and \
+                                    elem[1].id in elem[0].allocated_function_list and \
+                                    elem[1].id in xml_fun_elem.allocated_function_list:
+                                xml_fun_elem.add_allocated_state(elem[0].id)
+                                output_xml.write_object_allocation([[xml_fun_elem, elem[0]]])
+                                Logger.set_info(__name__,
+                                                f"{elem[0].__class__.__name__} {elem[0].name} is allocated to "
+                                                f"{xml_fun_elem.__class__.__name__} {xml_fun_elem.name}")
+                            # Else do nothing
+
+                    if k in (0, 1):
+                        allocate_all_children_in_element(elem, **kwargs)
+        return 1
+    return 0
+
+
+def check_parent_allocation(elem, **kwargs):
+    """Check if parent's Function/Sate are allocated to parent's Fucntional Element:
+    if not print message to user asking if he wants to, if yes write it in xml then continue
+    with parents"""
+    if elem[0].parent is not None and elem[1].parent is not None:
+        fun_elem_parent = elem[0].parent
+        object_parent = elem[1].parent
+        check = False
+        if isinstance(elem[1], datamodel.State):
+            if object_parent.id in fun_elem_parent.allocated_state_list:
+                check = True
+        elif isinstance(elem[1], datamodel.Function):
+            if object_parent.id in fun_elem_parent.allocated_function_list:
+                check = True
+        if not check:
+            answer = input(f"Do you also want to allocate parents(i.e. {object_parent.name} "
+                           f"to {fun_elem_parent.name}) ?(Y/N)")
+            if answer.lower() == "y":
+                if isinstance(elem[1], datamodel.State):
+                    fun_elem_parent.add_allocated_state(object_parent.id)
+                else:
+                    fun_elem_parent.add_allocated_function(object_parent.id)
+
+                add_allocation({5: [[fun_elem_parent, object_parent]]}, **kwargs)
+                check_parent_allocation([fun_elem_parent, object_parent], **kwargs)
+            else:
+                Logger.set_error(__name__,
+                                 f"{object_parent.name} is not allocated despite at least one "
+                                 f"of its child is")
+
+
+def allocate_all_children_in_element(elem, **kwargs):
+    """Recursive allocation for children of State/Function"""
+    output_xml = kwargs['output_xml']
+    check_parent_allocation(elem, **kwargs)
+    object_type = question_answer.get_object_type(elem[1])
+    if elem[1].child_list:
+        for i in elem[1].child_list:
+            parent_child = [elem[1], i]
+            allocated_child_list = get_allocated_child(parent_child, [elem[0]])
+            if allocated_child_list:
+                for item in allocated_child_list:
+                    if isinstance(elem[1], datamodel.State):
+                        item[0].add_allocated_state(item[1].id)
+                    else:
+                        item[0].add_allocated_function(item[1].id)
+                # We want recursivety so it trigger for (0, 1) keys in the dict
+                add_allocation({0: allocated_child_list}, **kwargs)
+    else:
+        if object_type == "state" and elem[1].id not in elem[0].allocated_state_list:
+            # Remove previous allocation if any
+            xml_fun_elem_list = kwargs['xml_fun_elem_list']
+            for xml_fun_elem in xml_fun_elem_list:
+                if elem[1].id in xml_fun_elem.allocated_state_list:
+                    xml_fun_elem.remove_allocated_state(elem[1].id)
+                    output_xml.delete_object_allocation([[xml_fun_elem, elem[1]]])
+                    Logger.set_info(__name__,
+                                    f"State {elem[1].name} is not allocated to Functional element "
+                                    f"{xml_fun_elem.name} anymore")
+
+            elem[0].add_allocated_state(elem[1].id)
+            add_allocation({5: [elem]}, **kwargs)
+        elif object_type == "function" and elem[1].id not in elem[0].allocated_function_list:
+            # Remove previous allocation if any
+            xml_fun_elem_list = kwargs['xml_fun_elem_list']
+            for xml_fun_elem in xml_fun_elem_list:
+                if elem[1].id in xml_fun_elem.allocated_function_list:
+                    xml_fun_elem.remove_allocated_function(elem[1].id)
+                    output_xml.delete_object_allocation([[xml_fun_elem, elem[1]]])
+                    Logger.set_info(__name__,
+                                    f"Function {elem[1].name} is not allocated to Functional element "
+                                    f"{xml_fun_elem.name} anymore")
+
+            elem[0].add_allocated_function(elem[1].id)
+            add_allocation({5: [elem]}, **kwargs)
+
+
+def get_allocated_child(elem, xml_fun_elem_list):
+    """
+    Check if the parent state/function is already allocated to a fun elem and create list to add
+    its child also (if not already allocated)
+
+        Parameters:
+            elem ([State/Function]) : parent object, child object
+            xml_fun_elem_list ([FunctionalElement]) : functional element list from xml parsing
+
+        Returns:
+            output_list ([FunctionalElement, State/Function]) : Allocation Relationships that need
+            to be added
+    """
+    output_list = []
+    for fun_elem in xml_fun_elem_list:
+        if isinstance(elem[0], datamodel.State):
+            # To avoid "RuntimeError: Set changed size during iteration" copy()
+            allocated_list = fun_elem.allocated_state_list.copy()
+        else:
+            allocated_list = fun_elem.allocated_function_list.copy()
+        if allocated_list:
+            for allocated_object in allocated_list:
+                if allocated_object == elem[0].id:
+                    if elem[1].id not in allocated_list:
+                        if isinstance(elem[0], datamodel.State):
+                            fun_elem.add_allocated_state(elem[1].id)
+                        else:
+                            fun_elem.add_allocated_function(elem[1].id)
+                        output_list.append([fun_elem, elem[1]])
+
+    return output_list
+
+
+def check_add_inheritance(inherit_str_list, **kwargs):
+    """
+    Check if each string in allocation_str_list are corresponding to an actual object's name/alias,
+    set_derive, create lists of objets.
+    Send lists to add_derived() to write them within xml and then returns update from it.
+
+        Parameters:
+            inherit_str_list ([str]) : Lists of string from jarvis cell
+            kwargs (dict) : whole xml lists + xml's file object
+
+        Returns:
+            update ([0/1]) : 1 if update, else 0
+    """
+    new_list = []
+    for elem in inherit_str_list:
+        # elem_0: inheriting object
+        elem_0 = question_answer.check_get_object(elem[0],
+                                                  **{'xml_function_list': kwargs['xml_function_list'],
+                                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
+                                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
+                                                     })
+        # elem_1: object to inherit from
+        elem_1 = question_answer.check_get_object(elem[1],
+                                                  **{'xml_function_list': kwargs['xml_function_list'],
+                                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
+                                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
+                                                     })
+        if not elem_0 or not elem_1:
+            if not elem_0 and not elem_1:
+                print_wrong_object_inheritance(elem[0], elem[1])
+            elif not elem_0:
+                print_wrong_object_inheritance(elem[0])
+            else:
+                print_wrong_object_inheritance(elem[1])
+            continue
+        if elem_0 == elem_1:
+            Logger.set_warning(__name__,
+                               f"Same object {elem_0.name}")
+            continue
+        if elem_0.derived == elem_1:
+            continue
+
+        check_obj = check_inheritance(elem_0, elem_1)
+        if not check_obj:
+            continue
+        new_list.append(elem_0)
+
+    if not new_list:
+        return 0
+
+    add_derived(new_list, kwargs['output_xml'])
+    return 1
+
+
+def print_wrong_object_inheritance(*obj):
+    """Prints wrong object(s) message for inheritance from input string"""
+    if len(obj) == 2:
+        user_message = f"{obj[0]} and {obj[1]}"
+    else:
+        user_message = f"{obj[0]}"
+
+    Logger.set_error(__name__,
+                     f"{user_message} not found, available objects for inheritance are:\n"
+                     "- Function\n"
+                     "- Functional element\n"
+                     "- Functional interface\n"
+                     "- Physical element\n"
+                     "- Physical element\n")
+
+
+def check_inheritance(elem_0, elem_1):
+    """Returns check if pair are compatible and object list have been updated"""
+    inheritance_type_list = [datamodel.Function, datamodel.FunctionalElement,
+                             datamodel.FunctionalInterface, datamodel.PhysicalElement,
+                             datamodel.PhysicalInterface]
+
+    type_found = None
+    for idx, inheritance_type in enumerate(inheritance_type_list):
+        if isinstance(elem_0, inheritance_type) and isinstance(elem_1, inheritance_type):
+            type_found = idx
+            break
+
+    if type_found is None:
+        Logger.set_error(__name__,
+                         f"{elem_0.__class__.__name__} and {elem_1.__class__.__name__} "
+                         f"are not of the same type")
+        return False
+
+    elem_0.set_derived(elem_1)
+    return True
+
+
+def add_derived(object_list, output_xml):
+    """
+    Check if input lists are not empty, write in xml for each list and return update if some
+    updates has been made.
+        Parameters:
+            object_list ([Object]) : object with new derived
+            output_xml (XmlWriter3SE object) : XML's file object
+
+        Returns:
+            1 if update, else 0
+    """
+    if any(object_list):
+        output_xml.write_object_derived(object_list)
+        for obj in object_list:
+            Logger.set_info(__name__,
+                            f"{obj.name} inherited from {obj.derived.name}")
+        return 1
+    return 0
+
+
+# Inheritance start here - Should be moved/refactored after validation
+def childs_inheritance(*xml_obj_set, level=None):
+    """Check if object from xml_obj_set is derived, if yes:
+    - call derived_childs()
+    - returns derived_parent_dict of derived objects id, derived_child_set of derived objects and
+    derived_child_id_list
+    Parameter:
+    - obj: set() of objects
+    - level: diagram level"""
+    derived_child_set = set()
+    derived_parent_dict = {}
+    derived_child_id_list = set()
+
+    for xml_set in xml_obj_set:
+        for elem in xml_set:
+            if elem.derived:
+                partial_child_set, partial_par_dict, partial_child_id_set = derived_childs(elem,
+                                                                                           level)
+                derived_child_set = derived_child_set.union(partial_child_set)
+                derived_parent_dict.update(partial_par_dict)
+                derived_child_id_list = derived_child_id_list.union(partial_child_id_set)
+
+    return derived_child_set, derived_parent_dict, derived_child_id_list
+
+
+def derived_childs(obj, level):
+    """Add derived object childs to object and set derived parent to object"""
+    derived_parent_dict = {}
+
+    [obj.add_child(c) for c in obj.derived.child_list
+     if c.parent == obj.derived]
+    [c.set_parent(obj) for c in obj.derived.child_list
+     if c.parent == obj.derived]
+    for child in obj.derived.child_list:
+        derived_parent_dict[str(child.id)] = str(obj.id)
+    derived_child_set = question_answer.get_children(obj.derived, level=level)[0]
+    derived_child_id_list = {c.id for c in obj.derived.child_list}
+    obj.derived.child_list.clear()
+    derived_child_set.remove(obj.derived)
+
+    return derived_child_set, derived_parent_dict, derived_child_id_list
+
+
+def reset_childs_inheritance(*xml_obj_set, derived_child_id=None):
+    """Check if there is first level derived child id list, if yes reset original child/parent
+    relationships"""
+    if derived_child_id:
+        for xml_set in xml_obj_set:
+            for elem in xml_set:
+                if elem.derived:
+                    child_pop = [c for c in elem.child_list
+                                 if c.id in [f for f in derived_child_id]]
+                    [elem.derived.add_child(c) for c in child_pop]
+                    [c.set_parent(elem.derived) for c in child_pop]
+
+
+def attribute_inheritance(xml_attribute_set, *xml_object_set):
+    """Attribute inheritance"""
+    modified_attrib_set = set()
+    derived_elem = set()
+
+    for xml_set in xml_object_set:
+        [derived_elem.add(e) for e in xml_set if e.derived]
+
+    for attribute in xml_attribute_set:
+        for obj_id, value in attribute.described_item_list.copy():
+            for der_obj in derived_elem:
+                if obj_id == der_obj.derived.id:
+                    attribute.add_described_item((der_obj.id, value))
+                    modified_attrib_set.add((attribute.id, der_obj.id, value))
+
+    return modified_attrib_set
+
+
+def reset_attribute_inheritance(xml_attribute_set, to_be_reset_id_set):
+    """Reset attributes"""
+    for attribute in xml_attribute_set:
+        [attribute.described_item_list.remove((e[1], e[2])) for e in to_be_reset_id_set
+         if e[0] == attribute.id]
+
+
+def view_inheritance(xml_view_set, *xml_obj_set):
+    """View inheritance"""
+    temp_view_set = set()
+    derived_elem_set = set()
+
+    for xml_set in xml_obj_set:
+        [derived_elem_set.add(e) for e in xml_set if e.derived]
+
+    for view in xml_view_set:
+        for item_id in view.allocated_item_list.copy():
+            for obj in derived_elem_set:
+                if item_id == obj.derived.id:
+                    temp_view_set.add((view.id, obj.id))
+                    view.add_allocated_item(obj.id)
+
+    return temp_view_set
+
+
+def reset_view_inheritance(xml_view_set, to_be_removed_id):
+    """Reset views"""
+    for view in xml_view_set:
+        for ids in to_be_removed_id:
+            if view.id == ids[0]:
+                view.allocated_item_list.remove(ids[1])
+
+
+def allocation_inheritance(xml_obj_set, xml_allocated_obj_set):
+    """Allocation Inheritance"""
+    alloc_to_reset = []
+    for elem in xml_obj_set:
+        if elem.derived:
+            if isinstance(elem, datamodel.FunctionalElement):
+                pair = [elem, {i for i in elem.derived.allocated_function_list
+                               if i not in elem.allocated_function_list}]
+                elem.allocated_function_list = elem.allocated_function_list.union(
+                    elem.derived.allocated_function_list)
+                alloc_to_reset.append(pair)
+            if isinstance(elem, datamodel.FunctionalInterface):
+                pair = [elem, {i for i in elem.derived.allocated_data_list
+                               if i not in elem.allocated_data_list}]
+                elem.allocated_data_list = elem.allocated_data_list.union(
+                    elem.derived.allocated_data_list)
+                alloc_to_reset.append(pair)
+
+    return alloc_to_reset
+
+
+def reset_alloc_inheritance(pairs_to_reset):
+    """Reset Allocation Inheritance"""
+    for pair in pairs_to_reset:
+        if isinstance(pair[0], datamodel.FunctionalElement):
+            [pair[0].allocated_function_list.remove(fun_id) for fun_id in pair[1]]
+        if isinstance(pair[0], datamodel.FunctionalInterface):
+            [pair[0].allocated_data_list.remove(data_id) for data_id in pair[1]]
```

### Comparing `jarvis4se-1.3.5/src/jarvis/util.py` & `jarvis4se-1.4.0/src/jarvis/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,108 @@
-"""@defgroup jarvis
-Jarvis module
-"""
-
-# Libraries
-import re
-
-# Modules
-from tools import Logger
-
-
-def cut_tuple_list(string_tuple_list):
-    """@ingroup jarvis
-    @anchor cut_tuple_list
-    From a list of input strings containing {(element_A, [element_B, element_C])} or {([element_B, element_C],
-    element_A)}, returns a list of combined strings containing {(element_A, element_B), (element_A, element_C)}.
-
-    Allows to handle such Jarvis command as "F1, F2, F3 compose F"
-
-    @param[in] string_tuple_list ([(str, str), ...]) : list of input string
-    @return list of combined strings
-    """
-    Logger.set_debug(__name__, f'Input: {string_tuple_list}')
-
-    output_list = []
-    for parent, child in string_tuple_list:
-        if "," in child:
-            child_list_str = cut_string(child)
-            for elem in child_list_str:
-                output_list.append((parent, elem))
-        elif "," in parent:
-            parent_list_str = cut_string(parent)
-            for elem in parent_list_str:
-                output_list.append((elem, child))
-        else:
-            output_list.append((parent, child))
-
-    Logger.set_debug(__name__, f'Output: {output_list}')
-
-    return output_list
-
-
-def cut_string(input_string):
-    """@ingroup jarvis
-    @anchor cut_string_list
-    From an string containing "element_A, element_B, element_C...", returns a list of strings containing
-    [[element_A], [element_B], [element_C], ...]
-
-    @param[in] input_string : input string
-    @return list of strings
-    """
-    splitted_string = re.split(r',(?![^[]*\])', input_string)
-
-    i = 0
-    for elem in splitted_string.copy():
-        splitted_string[i] = elem.strip()
-        i = i+1
-
-    return splitted_string
+"""@defgroup jarvis
+Jarvis module
+"""
+
+# Libraries
+import re
+import uuid
+
+# Modules
+from tools import Logger
+
+
+def cut_tuple_list(string_tuple_list):
+    """@ingroup jarvis
+    @anchor cut_tuple_list
+    From a list of input strings containing {(element_A, [element_B, element_C])} or {([element_B, element_C],
+    element_A)}, returns a list of combined strings containing {(element_A, element_B), (element_A, element_C)}.
+
+    Allows to handle such Jarvis command as "F1, F2, F3 compose F"
+
+    @param[in] string_tuple_list ([(str, str), ...]) : list of input string
+    @return list of combined strings
+    """
+    Logger.set_debug(__name__, f'Input: {string_tuple_list}')
+
+    output_list = []
+    for parent, child in string_tuple_list:
+        if "," in child:
+            child_list_str = cut_string(child)
+            for elem in child_list_str:
+                output_list.append((parent, elem))
+        elif "," in parent:
+            parent_list_str = cut_string(parent)
+            for elem in parent_list_str:
+                output_list.append((elem, child))
+        else:
+            output_list.append((parent, child))
+
+    Logger.set_debug(__name__, f'Output: {output_list}')
+
+    return output_list
+
+
+def reverse_tuple_list(string_tuple_list):
+    """@ingroup jarvis
+    @anchor reverse_tuple_list
+    Reverse a list of input strings
+
+    @param[in] string_tuple_list ([(str, str), ...]) : list of input string
+    @return list of reversed input strings
+    """
+    sorted_list = []
+    for string_tuple in string_tuple_list:
+        reversed_string_tuple = ()
+        for k in reversed(string_tuple):
+            reversed_string_tuple = reversed_string_tuple + (k,)
+        sorted_list.append(reversed_string_tuple)
+
+    return sorted_list
+
+
+def cut_chain_from_string_list(input_string_list):
+    """@ingroup jarvis
+    @anchor cut_chain_from_string_list
+    Creates flatten list : from ["A", "B, C, D"] to ["A", "B", "C", "D"]
+
+    @param[in] input_string_list : input string list
+    @return list of strings
+    """
+    output_list = []
+    for input_string in input_string_list:
+        if "," in input_string:
+            for split_string in cut_string(input_string):
+                output_list.append(split_string)
+        else:
+            output_list.append(input_string)
+
+    return output_list
+
+
+def cut_string(input_string):
+    """@ingroup jarvis
+    @anchor cut_string
+    From an string containing "element_A, element_B, element_C...", returns a list of strings containing
+    [[element_A], [element_B], [element_C], ...]
+
+    @param[in] input_string : input string
+    @return list of strings
+    """
+    split_string = re.split(r',(?![^[]*\])', input_string)
+
+    i = 0
+    for elem in split_string.copy():
+        split_string[i] = elem.strip()
+        i = i+1
+
+    return split_string
+
+
+def get_unique_id():
+    """@ingroup jarvis
+    @anchor get_unique_id
+    Generate unique identifier of length 10 integers
+
+    @return uuid
+    """
+    identifier = uuid.uuid4()
+    return str(identifier.int)[:10]
```

### Comparing `jarvis4se-1.3.5/src/jarvis4se.egg-info/PKG-INFO` & `jarvis4se-1.4.0/src/jarvis4se.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,57 @@
-Metadata-Version: 2.1
-Name: jarvis4se
-Version: 1.3.5
-Summary: Jarvis 4 Systems Engineers
-Home-page: https://github.com/rcasteran/jarvis4se
-Author: Justin ANCELOT
-Author-email: not2behere@gmx.fr
-License: MIT
-Project-URL: Bug Tracker, https://github.com/rcasteran/jarvis4se/issues
-Project-URL: Gitbook, https://regis-casteran.gitbook.io/jarvis4se/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Just Another Rather Very Intelligent System (JARVIS) for Systems Engineers (SE)
-
-Latest stable release: ![GitHub release (latest by date)](https://img.shields.io/github/v/release/rcasteran/jarvis4se)
-
-Current CI status: [![CircleCI](https://circleci.com/gh/rcasteran/jarvis4se/tree/main.svg?style=svg)](https://circleci.com/gh/rcasteran/jarvis4se/tree/main)
-
-Playground (with latest stable release) : [![Binder](https://mybinder.org/badge\_logo.svg)](https://mybinder.org/v2/gh/Not2behere/PlayJarvis4se/HEAD)
-
-## Introduction
-
-JARVIS4SE allows systems engineers to build the single source of truth of the knowledge they develop about the system of interest they want to master, preventing this knowledge from being:
-
-* Distorted by any graphical representation considerations
-* Splitted accross different domain languages
-* Expressed only in a machine readable medium
-
-### Free from graphical representation considerations
-
-The core of JARVIS4SE is independent from any graphical representation considerations: it is based on a set of basic [engineering concepts](docs/engineering-concepts/definitions.md) adapted from different domain languages, without taking into account concepts like coordinates, rendering...
-
-To be able to visualize the knowledge of the system of interest with diagrams, the core of JARVIS4SE can be interfaced with the API of any modeling tool through a dedicated adapter.
-
-Today the following adapters are available:
-
-* [PlantUML](https://plantuml.com/en/)
-
-### Based on natural language
-
-The core of JARVIS4SE is based on a subset of the english language that has been mapped to the set of basic [engineering concepts](docs/engineering-concepts/definitions.md).
-
-This allows systems engineers to interact with JARVIS4SE via voice or a textual interface.
+Metadata-Version: 2.1
+Name: jarvis4se
+Version: 1.4.0
+Summary: Jarvis 4 Systems Engineers
+Home-page: https://github.com/rcasteran/jarvis4se
+Author: Regis CASTERAN
+Author-email: casteranregis@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/rcasteran/jarvis4se/issues
+Project-URL: Gitbook, https://regis-casteran.gitbook.io/jarvis4se/
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython>=7.27.0
+Requires-Dist: lxml>=4.6.3
+Requires-Dist: notebook>=6.4.3
+Requires-Dist: plantuml==0.3.0
+Requires-Dist: pandas~=1.4.1
+Requires-Dist: requests>=2.31.0
+Requires-Dist: nltk~=3.8.1
+
+# Just Another Rather Very Intelligent System (JARVIS) for Systems Engineers (SE)
+
+Latest stable release: ![GitHub release (latest by date)](https://img.shields.io/github/v/release/rcasteran/jarvis4se)
+
+Current CI status: [![CircleCI](https://circleci.com/gh/rcasteran/jarvis4se/tree/main.svg?style=svg)](https://circleci.com/gh/rcasteran/jarvis4se/tree/main)
+
+Playground (with latest stable release) : [![Binder](https://mybinder.org/badge\_logo.svg)](https://mybinder.org/v2/gh/Not2behere/PlayJarvis4se/HEAD)
+
+## Introduction
+
+JARVIS4SE allows systems engineers to build the single source of truth of the knowledge they develop about the system of interest they want to master, preventing this knowledge from being:
+
+* Distorted by any graphical representation considerations
+* Splitted accross different domain languages
+* Expressed only in a machine readable medium
+
+### Free from graphical representation considerations
+
+The core of JARVIS4SE is independent from any graphical representation considerations: it is based on a set of basic [engineering concepts](docs/engineering-concepts/definitions.md) adapted from different domain languages, without taking into account concepts like coordinates, rendering...
+
+To be able to visualize the knowledge of the system of interest with diagrams, the core of JARVIS4SE can be interfaced with the API of any modeling tool through a dedicated adapter.
+
+Today the following adapters are available:
+
+* [PlantUML](https://plantuml.com/en/)
+
+### Based on natural language
+
+The core of JARVIS4SE is based on a subset of the english language that has been mapped to the set of basic [engineering concepts](docs/engineering-concepts/definitions.md).
+
+This allows systems engineers to interact with JARVIS4SE via voice or a textual interface.
```

### Comparing `jarvis4se-1.3.5/src/jarvis4se.egg-info/SOURCES.txt` & `jarvis4se-1.4.0/src/jarvis4se.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+src/csv_adapter/__init__.py
+src/csv_adapter/csv_parser.py
+src/csv_adapter/csv_writer.py
+src/csv_adapter/setup.py
+src/csv_adapter/util.py
 src/datamodel/__init__.py
 src/datamodel/datamodel.py
 src/datamodel/setup.py
 src/datamodel/util.py
 src/jarvis/__init__.py
 src/jarvis/command_parser.py
 src/jarvis/jarvis.py
-src/jarvis/question_answer.py
 src/jarvis/util.py
+src/jarvis4se.egg-info/PKG-INFO
+src/jarvis4se.egg-info/SOURCES.txt
+src/jarvis4se.egg-info/dependency_links.txt
+src/jarvis4se.egg-info/requires.txt
+src/jarvis4se.egg-info/top_level.txt
 src/jarvis/diagram/__init__.py
 src/jarvis/diagram/diagram_generator.py
 src/jarvis/diagram/diagram_generator_chain.py
 src/jarvis/diagram/diagram_generator_fana.py
 src/jarvis/diagram/diagram_generator_farch.py
 src/jarvis/diagram/util.py
+src/jarvis/handler/__init__.py
+src/jarvis/handler/handler_question.py
 src/jarvis/orchestrator/__init__.py
-src/jarvis/orchestrator/functional_orchestrator.py
-src/jarvis/orchestrator/shared_orchestrator.py
-src/jarvis/orchestrator/viewpoint_orchestrator.py
-src/jarvis4se.egg-info/PKG-INFO
-src/jarvis4se.egg-info/SOURCES.txt
-src/jarvis4se.egg-info/dependency_links.txt
-src/jarvis4se.egg-info/requires.txt
-src/jarvis4se.egg-info/top_level.txt
+src/jarvis/orchestrator/orchestrator_dictionary.py
+src/jarvis/orchestrator/orchestrator_functional.py
+src/jarvis/orchestrator/orchestrator_object.py
+src/jarvis/orchestrator/orchestrator_shared.py
+src/jarvis/orchestrator/orchestrator_viewpoint.py
+src/jarvis/orchestrator/orchestrator_viewpoint_attribute.py
+src/jarvis/orchestrator/orchestrator_viewpoint_requirement.py
+src/jarvis/orchestrator/orchestrator_viewpoint_type.py
+src/jarvis/query/__init__.py
+src/jarvis/query/query_object_list.py
+src/jarvis/query/question_answer.py
 src/plantuml_adapter/__init__.py
 src/plantuml_adapter/plantuml_adapter.py
 src/plantuml_adapter/setup.py
 src/plantuml_adapter/util.py
 src/tools/__init__.py
 src/tools/config.py
 src/tools/console.py
 src/tools/logger.py
 src/tools/magic_tools.py
 src/tools/util.py
 src/xml_adapter/__init__.py
 src/xml_adapter/setup.py
 src/xml_adapter/xml_parser.py
 src/xml_adapter/xml_writer.py
+tests/test_csv_file.py
+tests/test_handler_question.py
 tests/test_input_cell.py
 tests/test_lib.py
 tests/test_magic_tools.py
-tests/test_question_answer.py
 tests/test_xml_file.py
```

### Comparing `jarvis4se-1.3.5/src/plantuml_adapter/__init__.py` & `jarvis4se-1.4.0/src/plantuml_adapter/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-""" @package plantuml_adapter
-Plantuml adapter module
-
-Defines the different functions and classes used by Jarvis to call Plantuml as a diagram generator:
-- function to construct the PlantUml text and url for the functions diagram: @ref get_function_diagrams
-- function to construct the PlantUml text for the sequence diagrams: @ref get_sequence_diagram
-- function to construct the PlantUml text and url for state machine diagrams:
-@ref get_state_machine_diagram
-- function to construct the PlantUml text for the functional element decomposition diagram:
-@ref get_fun_elem_decomposition
-- function to construct the PlantUml text and url for the context diagram for functional elements:
-@ref get_fun_elem_context_diagram
-- class to handle local PlantUml PicoWeb Server: @ref PlantUmlPicoServer
-- class to encode PlantUml text and get server url as .svg : @ref PlantUmlGen
-- class to encode PlantUml text for state diagram : @ref StateDiagram
-- class to encode PlantUml text for sequence diagram : @ref SequenceDiagram
-- class to encode PlantUml text for object diagram : @ref ObjDiagram
-"""
-
-from .plantuml_adapter import get_function_diagrams
-from .plantuml_adapter import get_sequence_diagram
-from .plantuml_adapter import get_state_machine_diagram
-from .plantuml_adapter import get_fun_elem_decomposition
-from .plantuml_adapter import get_fun_elem_context_diagram
-from .util import PlantUmlPicoServer
-from .util import PlantUmlGen
+""" @package plantuml_adapter
+Plantuml adapter module
+
+Defines the different functions and classes used by Jarvis to call Plantuml as a diagram generator:
+- function to construct the PlantUml text and url for the functions diagram: @ref get_function_diagrams
+- function to construct the PlantUml text for the sequence diagrams: @ref get_sequence_diagram
+- function to construct the PlantUml text and url for state machine diagrams:
+@ref get_state_machine_diagram
+- function to construct the PlantUml text for the functional element decomposition diagram:
+@ref get_fun_elem_decomposition
+- function to construct the PlantUml text and url for the context diagram for functional elements:
+@ref get_fun_elem_context_diagram
+- class to handle local PlantUml PicoWeb Server: @ref PlantUmlPicoServer
+- class to encode PlantUml text and get server url as .svg : @ref PlantUmlGen
+- class to encode PlantUml text for state diagram : @ref StateDiagram
+- class to encode PlantUml text for sequence diagram : @ref SequenceDiagram
+- class to encode PlantUml text for object diagram : @ref ObjDiagram
+"""
+
+from .plantuml_adapter import get_function_diagrams
+from .plantuml_adapter import get_sequence_diagram
+from .plantuml_adapter import get_state_machine_diagram
+from .plantuml_adapter import get_fun_elem_decomposition
+from .plantuml_adapter import get_fun_elem_context_diagram
+from .util import PlantUmlPicoServer
+from .util import PlantUmlGen
```

### Comparing `jarvis4se-1.3.5/src/plantuml_adapter/plantuml_adapter.py` & `jarvis4se-1.4.0/src/plantuml_adapter/plantuml_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1142 +1,1134 @@
-"""@defgroup plantuml_adapter
-Plantuml adapter module
-"""
-
-# Modules
-import datamodel
-from .util import ObjDiagram, StateDiagram, SequenceDiagram
-from tools import Logger
-
-
-def write_function_child(string_obj, function, input_flow_list, output_flow_list,
-                         xml_attribute_list):
-    """@ingroup plantuml_adapter
-    Construct PlantUml text recursively
-    @param[in,out] string_obj current PlantUml text
-    @param[in] function
-    @param[in] input_flow_list
-    @param[in] output_flow_list
-    @param[in] xml_attribute_list
-    @return None
-    """
-
-    function_input_port = []
-    function_output_port = []
-    external_input_port = []
-    external_output_port = []
-    parent_function_port = []
-    count = 1
-    nb_component = count_composed_component(function, count)
-
-    # TODO: Create get_port_lists() and optimize
-    for p in input_flow_list:
-        if p[0][0] == function.name.lower():
-            function_input_port.append(p)
-        if p[0][0] is None and function.parent is None:
-            external_input_port.append(p)
-            if p[0][1] == function.name.lower():
-                parent_function_port.append(p)
-
-    for q in output_flow_list:
-        if q[0][0] == function.name.lower():
-            function_output_port.append(q)
-        if q[0][0] is None and function.parent is None:
-            external_output_port.append(q)
-            if q[0][1] == function.name.lower():
-                parent_function_port.append(q)
-
-    Logger.set_debug(__name__, f"Function name: {function.name}")
-    Logger.set_debug(__name__, f"Input port list: {function_input_port}")
-    Logger.set_debug(__name__, f"Output port list: {function_input_port}")
-    Logger.set_debug(__name__, f"Parent function port list: {parent_function_port}")
-    Logger.set_debug(__name__, f"External input port list: {external_input_port}")
-    Logger.set_debug(__name__, f"External output port list: {external_output_port}")
-
-    string_obj.create_port(function_input_port, "in")
-    string_obj.create_port(function_output_port, "out")
-    string_obj.create_port(parent_function_port, 'None')
-
-    child_with_no_child_list = []
-    child_with_child_list = []
-    # Create a child list for each parent function
-    for child_function in function.child_list:
-        Logger.set_debug(__name__, f"{child_function.name} check as child of {function.name}")
-        if child_function.child_list:
-            child_with_child_list.append(child_function)
-        else:
-            child_with_no_child_list.append(child_function)
-
-    # For child that has no child: create object
-    for fun in child_with_no_child_list:
-        string_obj.create_object(fun, xml_attribute_list)
-
-    for child in child_with_child_list:
-        string_obj.create_component(child)
-        write_function_child(string_obj, child, input_flow_list, output_flow_list,
-                             xml_attribute_list)
-        nb_component -= 1
-
-    # Close all the brackets depending on the number of component within highest parent
-    for i in range(nb_component):
-        string_obj.append_string('}\n')
-
-    for component in child_with_child_list:
-        string_obj.create_component_attribute(component, xml_attribute_list)
-
-    whole_child_list = child_with_child_list + child_with_no_child_list
-    for fun in whole_child_list:
-        for i in input_flow_list:
-            if i[0][0] == fun.name.lower():
-                string_obj.create_port(input_flow_list, "in")
-        for j in output_flow_list:
-            if j[0][0] == fun.name.lower():
-                string_obj.create_port(output_flow_list, "out")
-
-    string_obj.create_port(external_input_port, "in")
-    string_obj.create_port(external_output_port, "out")
-
-
-def count_composed_component(function, count):
-    """@ingroup plantuml_adapter
-    Count the number of composed function within the higher function
-    @param[in] function function to check
-    @param[in] count number of component
-    @return number of component
-    """
-
-    for elem in function.child_list:
-        if elem.child_list:
-            count += 1
-            count_composed_component(elem, count)
-            continue
-    return count
-
-
-def write_function_object(string_obj, function, input_flow_list, output_flow_list, check,
-                          xml_attribute_list, component_obj=None, compo_diagram=False):
-    """@ingroup plantuml_adapter
-    Construct the PlantUml text for a function object with associated ports for flow lists.
-    @param[in,out] string_obj current PlantUml text
-    @param[in] function
-    @param[in] input_flow_list
-    @param[in] output_flow_list
-    @param[in] check
-    @param[in] xml_attribute_list
-    @param[in] component_obj
-    @param[in] compo_diagram
-    @return PlantUml text for the function object
-    """
-
-    string_obj.create_object(function, xml_attribute_list)
-
-    if check:
-        string_obj.append_string('}\n')
-        if component_obj:
-            string_obj.create_component_attribute(component_obj, xml_attribute_list)
-
-    for p in input_flow_list:
-        if compo_diagram:
-            if p[0][0] == function.name.lower():
-                string_obj.create_port(input_flow_list, "in")
-        else:
-            if p[0][0] == function.name.lower() or p[0][1] == function.name.lower():
-                string_obj.create_port(input_flow_list, "in")
-    for q in output_flow_list:
-        if compo_diagram:
-            if q[0][0] == function.name.lower():
-                string_obj.create_port(output_flow_list, "out")
-        else:
-            if q[0][0] == function.name.lower() or q[0][1] == function.name.lower():
-                string_obj.create_port(output_flow_list, "out")
-
-
-def get_function_diagrams(function_list, fun_elem_list, consumer_function_list, producer_function_list,
-                          parent_child_dict, data_list, xml_type_list, xml_attribute_list):
-    """@ingroup plantuml_adapter
-    @anchor get_function_diagrams
-    Construct the PlantUml text and url for the requested diagram between one of the following:
-    - context of function
-    - decomposition of function
-    - chain of function
-    @param[in] function_list
-    @param[in] consumer_function_list
-    @param[in] producer_function_list
-    @param[in] parent_child_dict
-    @param[in] data_list
-    @param[in] xml_type_list
-    @param[in] xml_attribute_list
-    @return PlantUml text and url of the diagram
-    """
-
-    string_obj = ObjDiagram()
-    # Filter output flows
-    output_flow_list = get_output_flows(consumer_function_list, producer_function_list,
-                                        concatenate=True)
-    # Filter input flows
-    input_flow_list = get_input_flows(consumer_function_list, producer_function_list,
-                                      concatenate=True)
-
-    # Filter consumers and producers list in order to create data flow
-    data_flow_list = get_exchanged_flows(consumer_function_list, producer_function_list,
-                                         parent_child_dict, concatenate=True)
-
-    Logger.set_debug(__name__, f"Output flows list: {output_flow_list}")
-    Logger.set_debug(__name__, f"Input flows list: {input_flow_list}")
-    Logger.set_debug(__name__, f'Exchanged flows list: {data_flow_list}')
-
-    if data_list:
-        per_message_data_flow_list = get_exchanged_flows(consumer_function_list,
-                                                         producer_function_list,
-                                                         parent_child_dict)
-        if len(data_list) == len(per_message_data_flow_list):
-            ordered_function_list, ordered_message_list = order_list(per_message_data_flow_list,
-                                                                     data_list)
-            if per_message_data_flow_list != ordered_message_list:
-                for idx, i in enumerate(ordered_message_list):
-                    for j in data_flow_list:
-                        for k in j[1]:
-                            if i[2] == k and i[3]:
-                                new = str(idx + 1) + ":" + k
-                                j[1].remove(k)
-                                j[1].append(new)
-
-    # Loop in order to filter functions and write in output's file, see write_function_child()
-    if parent_child_dict:
-        if fun_elem_list:
-            for fun_elem in fun_elem_list:
-                string_obj.create_component(fun_elem)
-                check_function = False
-                for f in function_list:
-                    if any(a == f.id for a in fun_elem.allocated_function_list):
-                        if len(fun_elem.allocated_function_list) > 1:
-                            check_function = False
-                        else:
-                            check_function = True
-                        write_function_object(string_obj, f, input_flow_list, output_flow_list,
-                                              check_function, xml_attribute_list, component_obj=fun_elem)
-                if not check_function:
-                    string_obj.append_string('}\n')
-                    string_obj.create_component_attribute(fun_elem, xml_attribute_list)
-        else:
-            for function in function_list:
-                if function.id not in parent_child_dict.keys():
-                    if function.id in parent_child_dict.values():
-                        # Function is a parent
-                        string_obj.create_component(function)
-                        write_function_child(string_obj, function, input_flow_list, output_flow_list,
-                                             xml_attribute_list)
-                    else:
-                        # Function is not a parent:
-                        write_function_object(string_obj, function, input_flow_list, output_flow_list,
-                                              False, xml_attribute_list, compo_diagram=True)
-                # Else do nothing : done as children of function parent
-    else:
-        for function in function_list:
-            write_function_object(string_obj, function, input_flow_list, output_flow_list, False,
-                                  xml_attribute_list)
-
-    string_obj.create_input_flow(input_flow_list)
-    string_obj.create_output_flow(output_flow_list)
-    string_obj.create_data_flow(data_flow_list)
-
-    return string_obj.string
-
-
-def get_fun_elem_context_diagram(function_list, consumer_function_list, producer_function_list,
-                                 data_list, xml_attribute_list, fun_elem_list, fun_inter_list):
-    """@ingroup plantuml_adapter
-    @anchor get_fun_elem_context_diagram
-    Construct the PlantUml text and url for the context diagram for functional elements
-    @param[in] function_list TBD
-    @param[in] consumer_function_list TBD
-    @param[in] producer_function_list TBD
-    @param[in] data_list TBD
-    @param[in] xml_attribute_list TBD
-    @param[in] fun_elem_list TBD
-    @param[in] fun_inter_list TBD
-    @return PlantUml text and url of the diagram
-    """
-
-    string_obj = ObjDiagram()
-    interface_list = None
-
-    if fun_inter_list:
-
-        unmerged_data_list = get_exchanged_flows(consumer_function_list, producer_function_list, {})
-        interface_list, data_flow_list = get_interface_list(fun_inter_list,
-                                                            data_list,
-                                                            unmerged_data_list,
-                                                            function_list,
-                                                            fun_elem_list,
-                                                            is_decomposition=False)
-
-        data_flow_list = concatenate_flows(data_flow_list)
-
-    else:
-
-        # Filter consumers and producers list in order to create data flow
-        data_flow_list = get_exchanged_flows(consumer_function_list, producer_function_list,
-                                             {}, concatenate=True)
-
-    # Filter output flows
-    output_flow_list = get_output_flows(consumer_function_list, producer_function_list,
-                                        concatenate=True)
-    # Filter input flows
-    input_flow_list = get_input_flows(consumer_function_list, producer_function_list,
-                                      concatenate=True)
-
-    # Write external functions
-    external_function_list = []
-    for function in function_list:
-        is_external = True
-        for fun_elem in fun_elem_list:
-            if any(a == function.id for a in fun_elem.allocated_function_list):
-                is_external = False
-
-        if is_external:
-            external_function_list.append(function)
-
-    for function in external_function_list:
-        string_obj.create_object(function, xml_attribute_list)
-
-    for fun_elem in fun_elem_list:
-        string_obj.create_component(fun_elem)
-        check_function = False
-        for f in function_list:
-            if any(a == f.id for a in fun_elem.allocated_function_list):
-                if len(fun_elem.allocated_function_list) > 1:
-                    check_function = False
-                else:
-                    check_function = True
-                write_function_object(string_obj, f, input_flow_list, output_flow_list,
-                                      check_function, xml_attribute_list, component_obj=fun_elem)
-        if not check_function:
-            string_obj.append_string('}\n')
-            string_obj.create_component_attribute(fun_elem, xml_attribute_list)
-
-    string_obj.create_input_flow(input_flow_list)
-    string_obj.create_output_flow(output_flow_list)
-    string_obj.create_data_flow(data_flow_list)
-
-    if interface_list:
-        string_obj.create_interface(interface_list)
-
-    return string_obj.string
-
-
-def get_interface_list(fun_inter_list, data_list, data_flow_list, function_list, fun_elem_list,
-                       is_decomposition=True):
-    """@ingroup plantuml_adapter
-    Get list of functional interfaces with the functional elements exposing them.
-    Functional interface is returned only when specifed data is allocated to it
-    @param[in] fun_inter_list TBD
-    @param[in] data_list TBD
-    @param[in] data_flow_list TBD
-    @param[in] function_list TBD
-    @param[in] fun_elem_list TBD
-    @param[in] is_decomposition indicates if decomposition is required (True) or not (False)
-    @return functional interfaces list
-    """
-
-    interface_list = []
-    removed_data_flow_list = []
-    initial_data = list(data_flow_list)
-    idx = 0
-    # Get all fun_inter with allocated data within data_flow_list and create interface list
-    # [[producer, consumer, fun_inter]...]
-    for fun_inter in fun_inter_list:
-        Logger.set_debug(__name__, f"Interface {fun_inter.name}, allocated data {fun_inter.allocated_data_list}")
-        if fun_inter.allocated_data_list:
-            for data_id in fun_inter.allocated_data_list:
-                for data in data_list:
-                    if data_id == data.id:
-                        for data_flow in data_flow_list.copy():
-                            if data.name == data_flow[2]:
-                                first_fun = None
-                                second_fun = None
-                                for fun in function_list:
-                                    if data_flow[0] == fun.name.lower():
-                                        first_fun = fun
-                                    if data_flow[1] == fun.name.lower():
-                                        second_fun = fun
-
-                                if first_fun or second_fun:
-                                    # Need to check consistency between [elem1, elem2, fun_inter] and [fun1, fun2, data]
-                                    # before adding to the list
-                                    is_first_fun_elem = False
-                                    is_second_fun_elem = False
-                                    for fun_elem in fun_elem_list:
-                                        if any(exposed_fun_inter_id == fun_inter.id for exposed_fun_inter_id in
-                                               fun_elem.exposed_interface_list):
-                                            if first_fun and not is_first_fun_elem:
-                                                is_first_fun_elem = any(allocated_fun_id ==
-                                                                        first_fun.id for allocated_fun_id
-                                                                        in fun_elem.allocated_function_list)
-                                            if second_fun and not is_second_fun_elem:
-                                                is_second_fun_elem = any(allocated_fun_id ==
-                                                                         second_fun.id for allocated_fun_id
-                                                                         in fun_elem.allocated_function_list)
-
-                                    if (first_fun and is_first_fun_elem and not second_fun) or \
-                                            (second_fun and is_second_fun_elem and not first_fun) or \
-                                            (first_fun and is_first_fun_elem and second_fun and is_second_fun_elem):
-                                        Logger.set_debug(__name__, f"[{first_fun}, {second_fun}, {fun_inter}] added")
-                                        interface_list.insert(idx, [first_fun, second_fun, fun_inter])
-                                        removed_data_flow_list.insert(idx, data_flow)
-                                        data_flow_list.remove(data_flow)
-                                        idx += 1
-                                        break
-        else:
-            Logger.set_info(__name__, f"{fun_inter.name} does not have any allocated data (no display)")
-
-    output_list, interface_list = get_fun_elem_from_fun_inter(interface_list, fun_elem_list, is_decomposition)
-
-    if not output_list:
-        return None, initial_data
-
-    # (re)Add [producer, consumer, data_name] to data_flow_list if no interface exposed
-    if any(isinstance(s, list) for s in interface_list):
-        for idx, rest_inter in enumerate(interface_list):
-            if isinstance(rest_inter, list):
-                data_flow_list.append(removed_data_flow_list[idx])
-
-    return output_list, data_flow_list
-
-
-def get_fun_elem_from_fun_inter(interface_list, fun_elem_list, is_decomposition=True):
-    """@ingroup plantuml_adapter
-    Get list of functional interfaces with the functional elements exposing them from interface_list =
-    [[producer, consumer, fun_inter]...] and put value to False if (first, second, interface)
-    have been added to output_list (i.e. fun_elem_1/fun_elem_2 have been found for a fun_inter)
-    @param[in] interface_list TBD
-    @param[in] fun_elem_list TBD
-    @param[in] is_decomposition indicates if decomposition is required (True) or not (False)
-    @return functional interfaces list
-    """
-
-    output_list = []
-    for ix, (first, second, interface) in enumerate(interface_list):
-        fun_elem_1 = None
-        fun_elem_2 = None
-        if first:
-            for elem_1 in fun_elem_list:
-                if any(s == interface.id for s in elem_1.exposed_interface_list):
-                    if is_decomposition:
-                        if not elem_1.child_list:
-                            fun_elem_1 = elem_1
-                        else:
-                            check = True
-                            for child in elem_1.child_list:
-                                if any(s == interface.id for s in child.exposed_interface_list):
-                                    check = False
-                            if check:
-                                fun_elem_1 = elem_1
-                    else:
-                        fun_elem_1 = elem_1
-
-        if second:
-            for elem_2 in fun_elem_list:
-                if not first:
-                    if is_decomposition:
-                        if any(s == interface.id for s in elem_2.exposed_interface_list):
-                            if not elem_2.child_list:
-                                fun_elem_2 = elem_2
-                            else:
-                                check = True
-                                for child in elem_2.child_list:
-                                    if any(s == interface.id for s in child.exposed_interface_list):
-                                        check = False
-                                if check:
-                                    fun_elem_2 = elem_2
-                    else:
-                        fun_elem_2 = elem_2
-                else:
-                    if any(s == interface.id for s in elem_2.exposed_interface_list) and \
-                            elem_2 != fun_elem_1:
-                        if is_decomposition:
-                            if not elem_2.child_list:
-                                fun_elem_2 = elem_2
-                            else:
-                                check = True
-                                for child in elem_2.child_list:
-                                    if any(s == interface.id for s in child.exposed_interface_list):
-                                        check = False
-
-                                if check:
-                                    fun_elem_2 = elem_2
-                        else:
-                            fun_elem_2 = elem_2
-
-        if not (not fun_elem_1 and not fun_elem_2):
-            if [fun_elem_1, fun_elem_2, interface] not in output_list:
-                output_list.append([fun_elem_1, fun_elem_2, interface])
-            interface_list[ix] = False
-
-    return output_list, interface_list
-
-
-def check_child_allocation(string_obj, fun_elem, function_list, xml_attribute_list):
-    """@ingroup plantuml_adapter
-    Check for each function allocated to a functional element if not allocated to any
-    functional element child: in that case => write function object string.
-    @param[in,out] string_obj current PlantUml text
-    @param[in] fun_elem functional element to check
-    @param[in] function_list list of functions
-    @param[in] xml_attribute_list xml list of attributes
-    @return None
-    """
-
-    for function in function_list:
-        if function.id in fun_elem.allocated_function_list:
-            fun_elem_child_allocated_function_list = []
-            for c in fun_elem.child_list:
-                for j in c.allocated_function_list:
-                    fun_elem_child_allocated_function_list.append(j)
-
-            if not any(s == function.id for s in fun_elem_child_allocated_function_list):
-                write_function_object(string_obj, function, [], [], False, xml_attribute_list)
-
-
-def recursive_decomposition(string_obj, main_fun_elem, function_list, xml_attribute_list,
-                            first_iter=False):
-    """@ingroup plantuml_adapter
-    Create PlantUml text for functional elements recursively
-    @param[in,out] string_obj current PlantUml text
-    @param[in] main_fun_elem
-    @param[in] function_list list of functions
-    @param[in] xml_attribute_list xml list of attributes
-    @param[in] first_iter
-    @return None
-    """
-
-    if first_iter is True:
-        string_obj.create_component(main_fun_elem)
-        check_child_allocation(string_obj, main_fun_elem, function_list, xml_attribute_list)
-        if main_fun_elem.child_list:
-            recursive_decomposition(string_obj, main_fun_elem, function_list, xml_attribute_list)
-    else:
-        for c in main_fun_elem.child_list:
-            string_obj.create_component(c)
-            check_child_allocation(string_obj, c, function_list, xml_attribute_list)
-            if c.child_list:
-                recursive_decomposition(string_obj, c, function_list, xml_attribute_list)
-            string_obj.append_string('}\n')
-            string_obj.create_component_attribute(c, xml_attribute_list)
-        string_obj.create_component_attribute(main_fun_elem, xml_attribute_list)
-
-
-def get_fun_elem_decomposition(main_fun_elem, fun_elem_list, allocated_function_list, consumer_list,
-                               producer_list, external_function_list, xml_attribute_list,
-                               data_list, fun_inter_list):
-    """@ingroup plantuml_adapter
-    @anchor get_fun_elem_decomposition
-    Construct the PlantUml text for the functional element decomposition diagram
-    @param[in] main_fun_elem main functional element
-    @param[in] fun_elem_list functional element list
-    @param[in] allocated_function_list list of allocated functions to main functional element
-    @param[in] consumer_list filtered consumers list
-    @param[in] producer_list filtered producers list
-    @param[in] external_function_list filtered external functions list
-    @param[in] xml_attribute_list xml list of attributes
-    @param[in] data_list data list
-    @param[in] fun_inter_list functional interface list
-    @return PlantUml text of the diagram
-    """
-
-    string_obj = ObjDiagram()
-    interface_list = None
-
-    if fun_inter_list:
-        unmerged_data_list = get_exchanged_flows(consumer_list, producer_list, {})
-        interface_list, data_flow_list = get_interface_list(fun_inter_list,
-                                                            data_list,
-                                                            unmerged_data_list,
-                                                            allocated_function_list.
-                                                            union(external_function_list),
-                                                            fun_elem_list,
-                                                            is_decomposition=True)
-
-        data_flow_list = concatenate_flows(data_flow_list)
-
-    else:
-        # Filter consumers and producers list in order to create data flow
-        data_flow_list = get_exchanged_flows(consumer_list, producer_list, {}, concatenate=True)
-
-    # Write external functions that are not already allocated to external components
-    external_function_not_allocated_list = []
-    for function in external_function_list:
-        is_external = True
-        for fun_elem in fun_elem_list:
-            if any(a == function.id for a in fun_elem.allocated_function_list):
-                is_external = False
-
-        if is_external:
-            external_function_not_allocated_list.append(function)
-
-    for function in external_function_not_allocated_list:
-        string_obj.create_object(function, xml_attribute_list)
-
-    # Write functional element decompo recursively and add allocated functions
-    recursive_decomposition(string_obj, main_fun_elem, allocated_function_list, xml_attribute_list,
-                            first_iter=True)
-    string_obj.append_string('}\n')
-    string_obj.create_component_attribute(main_fun_elem, xml_attribute_list)
-    # Write external fun_elem
-    for elem in fun_elem_list:
-        if elem != main_fun_elem and elem.parent is None:
-            recursive_decomposition(string_obj, elem, external_function_list, xml_attribute_list,
-                                    first_iter=True)
-            string_obj.append_string('}\n')
-            string_obj.create_component_attribute(elem, xml_attribute_list)
-
-    # Write data flows
-    string_obj.create_data_flow(data_flow_list)
-    if interface_list:
-        string_obj.create_interface(interface_list)
-
-    return string_obj.string
-
-
-def get_sequence_diagram(function_list, consumer_function_list, producer_function_list,
-                         parent_child_dict, data_list, str_out=False):
-    """@ingroup plantuml_adapter
-    @anchor get_sequence_diagram
-    Construct the PlantUml text for the sequence diagrams
-    @param[in] function_list TBD
-    @param[in] consumer_function_list TBD
-    @param[in] producer_function_list TBD
-    @param[in] parent_child_dict TBD
-    @param[in] data_list TBD
-    @return PlantUml text of the diagram
-    """
-
-    seq_obj_string = SequenceDiagram()
-
-    message_list = get_exchanged_flows(consumer_function_list, producer_function_list,
-                                       parent_child_dict)
-    ordered_function_list, ordered_message_list = order_list(message_list, data_list)
-
-    if ordered_function_list:
-        for fun_name in ordered_function_list:
-            for f in function_list:
-                if fun_name == f.name.lower():
-                    seq_obj_string.create_participant(f)
-    else:
-        for f in function_list:
-            seq_obj_string.create_participant(f)
-
-    seq_obj_string.create_sequence_message(ordered_message_list)
-
-    return seq_obj_string.string
-
-
-def get_predecessor_list(data):
-    """@ingroup plantuml_adapter
-    Get the predecessor's list for a Data object
-    @param[in] data data object
-    @return predecessor list
-    """
-
-    predecessor_list = set()
-    if data.predecessor_list:
-        for predecessor in data.predecessor_list:
-            predecessor_list.add(predecessor)
-
-    return predecessor_list
-
-
-def check_sequence(predecessor_list, sequence):
-    """@ingroup plantuml_adapter
-    Check if predecessors of a data are in a sequence
-    @param[in] predecessor_list predecessor list
-    @param[in] sequence sequence
-    @return TRUE (predecessors are in the sequence) or FALSE
-    """
-
-    check = False
-    if predecessor_list == set():
-        check = None
-        return check
-
-    pred_set = set()
-    seq_set = set()
-    for pred in predecessor_list:
-        pred_set.add(pred.name)
-    for elem in sequence:
-        seq_set.add(elem[2].name)
-
-    if pred_set.issubset(seq_set):
-        check = True
-        return check
-
-    return check
-
-
-def clean_predecessor_list(message_object_list):
-    """@ingroup plantuml_adapter
-    Delete predecessor if not in the message's list
-    @param[in] message_object_list TBD
-    @return updated message list
-    """
-
-    for message in message_object_list:
-        pred_list = get_predecessor_list(message[2])
-        for pred in pred_list:
-            if not any(pred in s for s in message_object_list):
-                message[2].predecessor_list.remove(pred)
-
-    return message_object_list
-
-
-def get_sequence(message, message_object_list, sequence_list, sequence=None, index=None):
-    """@ingroup plantuml_adapter
-    Return a sequence for a given message
-    @param[in] message TBD
-    @param[in] message_object_list TBD
-    @param[in] sequence_list TBD
-    @param[in] sequence TBD
-    @param[in] index TBD
-    @return sequence
-    """
-    if not sequence:
-        sequence = []
-        index = 0
-    if message not in sequence and not any(message in s for s in sequence_list) is True:
-        message[3] = True
-        sequence.insert(index, message)
-        index += 1
-        for mess in message_object_list:
-            if message[2] in mess[2].predecessor_list:
-                get_sequence(mess, message_object_list, sequence_list, sequence, index)
-
-    return sequence
-
-
-def get_sequences(message_object_list):
-    """@ingroup plantuml_adapter
-    Group all sequences into a sequence list
-    @param[in] message_object_list
-    @return sequence list
-    """
-
-    sequence_list = []
-    for message in message_object_list:
-        if not message[2].predecessor_list:
-            sequence = get_sequence(message, message_object_list, sequence_list)
-            sequence_list.append(sequence)
-
-    return sequence_list
-
-
-def post_check_sequence(sequence_list):
-    """@ingroup plantuml_adapter
-    Check if message isn't missing in sequence, insert it at the good place and loop if not
-    well ordered (predecessor after each one)
-    @param[in] sequence_list TBD
-    @return sequence list ordered
-    """
-
-    for (idx, i) in enumerate(sequence_list):
-        pred = i[2].predecessor_list
-        if check_sequence(pred, sequence_list[:idx]) is True:
-            pass
-        elif check_sequence(pred, sequence_list[:idx]) is False:
-            for (index, elem) in enumerate(sequence_list.copy()):
-                curr_pred = elem[2].predecessor_list
-                if check_sequence(curr_pred, sequence_list[:index]) is True:
-                    sequence_list.remove(i)
-                    sequence_list.insert(index + 1, i)
-                    index += 1
-                else:
-                    continue
-        elif check_sequence(pred, sequence_list[:idx]) is None:
-            pass
-        idx += 1
-
-    for (new_idx, message) in enumerate(sequence_list):
-        new_pred = message[2].predecessor_list
-        if check_sequence(new_pred, sequence_list[:new_idx]) is False:
-            post_check_sequence(sequence_list)
-
-    return sequence_list
-
-
-def get_sequence_list(message_object_list):
-    """@ingroup plantuml_adapter
-    Call for sequences then clean_up and post_check
-    @param[in] message_object_list TBD
-    @return sequence list
-    """
-    sequence_list = get_sequences(message_object_list)
-
-    sequence_list = sorted(sequence_list, key=lambda x: len(x), reverse=True)
-    # Could be possible to implement this part within post_check_sequence()
-    for (index, i) in enumerate(sequence_list):
-        main_list = sequence_list[0]
-        if index > 0:
-            start = 0
-            for j in i.copy():
-                if not j[2].predecessor_list:
-                    i.remove(j)
-                    main_list.insert(start, j)
-                    start += 1
-
-    sequence_list = [item for sub in sequence_list for item in sub]
-    sequence_list = post_check_sequence(sequence_list)
-
-    return sequence_list
-
-
-def order_list(message_list, data_list):
-    """@ingroup plantuml_adapter
-    Order functions and messages
-    @param[in] message_list TBD
-    @param[in] data_list TBD
-    @return ordered message list and ordered function list
-    """
-
-    ordered_message_list = []
-    ordered_function_list = []
-    message_object_list = []
-
-    for i in message_list:
-        for data in data_list:
-            if i[2] == data.name:
-                message_object_list.append([i[0], i[1], data, False])
-
-    message_object_list = clean_predecessor_list(message_object_list)
-    ordored_message_object_list = get_sequence_list(message_object_list)
-
-    # Add index for each item within the list
-    for idx, t in enumerate(ordored_message_object_list):
-        ordered_message_list.insert(idx, [t[0], t[1], t[2].name, t[3]])
-
-    # Create the ordered(from ordered message list) function's list
-    # Starting with producers
-    for idx, m in enumerate(ordered_message_list):
-        if m[0] not in ordered_function_list:
-            ordered_function_list.insert(idx, m[0])
-    # Finishing with consumers
-    for j in message_list:
-        if j[1] not in ordered_function_list:
-            ordered_function_list.append(j[1])
-
-    return ordered_function_list, ordered_message_list
-
-
-def get_exchanged_flows(consumer_function_list, producer_function_list, parent_child_dict,
-                        concatenate=False):
-    """@ingroup plantuml_adapter
-    Return list of exchanged flows [[producer, consumer, data]], i.e. data that have
-    producer and consumer
-    @param[in] consumer_function_list TBD
-    @param[in] producer_function_list TBD
-    @param[in] parent_child_dict TBD
-    @param[in] concatenate TBD
-    @return list of exchanged flows
-    """
-
-    output_list = []
-
-    for producer_flow, producer_function in producer_function_list:
-        Logger.set_debug(__name__, f'Producer flow: {producer_flow}; '
-                                   f'function: {producer_function.id}, {producer_function.name}')
-        if not producer_function.child_list or not parent_child_dict:
-            for cons_flow, consumer_function in consumer_function_list:
-                Logger.set_debug(__name__, f'Consumer flow: {cons_flow}; '
-                                           f'function: {consumer_function.id}, {consumer_function.name}')
-                if (not consumer_function.child_list or not parent_child_dict) and cons_flow == producer_flow:
-                    output_list.append(
-                        [producer_function.name.lower(), consumer_function.name.lower(),
-                         producer_flow])
-
-    if concatenate:
-        output_list = concatenate_flows(output_list)
-
-    return output_list
-
-
-def get_output_flows(consumer_function_list, producer_function_list, concatenate=False):
-    """@ingroup plantuml_adapter
-    Return list of output flows [[None/parent_name, producer, data]], i.e. data that
-    have only producer
-    @param[in] consumer_function_list TBD
-    @param[in] producer_function_list TBD
-    @param[in] concatenate TBD
-    @return list of output flows
-    """
-    flow_consumer_name_list = []
-    flow_child_consumer_list = []
-    temp_input_list = []
-    output_list = []
-
-    for flow, cons in consumer_function_list:
-        flow_consumer_name_list.append([flow, cons.name.lower()])
-        if cons.child_list is not None:
-            for child in cons.child_list:
-                flow_child = [flow, child.name.lower()]
-                if [flow, child] in consumer_function_list:
-                    flow_child_consumer_list.append(flow_child)
-
-    for consumer_flow, consumer_function in consumer_function_list:
-        if len(consumer_function.child_list) > 0:
-            if len(flow_child_consumer_list) > 0:
-                if not any(consumer_flow in sublist for sublist in flow_child_consumer_list):
-                    temp_input_list.append([consumer_function.name.lower(), consumer_flow])
-            if len(flow_child_consumer_list) == 0:
-                temp_input_list.append([consumer_function.name.lower(), consumer_flow])
-
-    for producer_flow, producer_function in producer_function_list:
-        # TODO to be checked because returns flow with both producer and consumer (same output as get_exchanged_flows)
-        # for name, flow in temp_input_list:
-        #     if producer_flow == flow:
-        #         flow_child_consumer_list = [name, producer_function.name.lower(), producer_flow]
-        #         output_list.append(flow_child_consumer_list)
-
-        # Looking for outputs (i.e. flow with only producer's function)
-        if not any(producer_flow in sublist for sublist in flow_consumer_name_list):
-            if not any(producer_flow in sub for sub in output_list):
-                output_list.append([None, producer_function.name.lower(), producer_flow])
-
-    if concatenate:
-        output_list = concatenate_flows(output_list)
-
-    return output_list
-
-
-def get_input_flows(consumer_function_list, producer_function_list, concatenate=False):
-    """@ingroup plantuml_adapter
-    Return list of input flow [[None/parent_name, consumer, data]], i.e. data that
-    have only consumer
-    @param[in] consumer_function_list TBD
-    @param[in] producer_function_list TBD
-    @param[in] concatenate TBD
-    @return list of input flows
-    """
-
-    flow_producer_name_list = []
-    flow_child_producer_list = []
-    temp_input_list = []
-    output_list = []
-
-    for flow, prod in producer_function_list:
-        flow_producer_name_list.append([flow, prod.name.lower()])
-        if prod.child_list is not None:
-            for child in prod.child_list:
-                flow_child = [flow, child.name.lower()]
-                if [flow, child] in producer_function_list:
-                    flow_child_producer_list.append(flow_child)
-
-    for producer_flow, producer_function in producer_function_list:
-        if len(producer_function.child_list) > 0:
-            if len(flow_child_producer_list) > 0:
-                if not any(producer_flow in sublist for sublist in flow_child_producer_list):
-                    temp_input_list.append([producer_function.name.lower(), producer_flow])
-            if len(flow_child_producer_list) == 0:
-                temp_input_list.append([producer_function.name.lower(), producer_flow])
-
-    for cons_flow, consumer_fun in consumer_function_list:
-        # TODO to be checked because returns flow with both producer and consumer (same output as get_exchanged_flows)
-        # for name, flow in temp_input_list:
-        #     if cons_flow == flow:
-        #         flow_child_producer_list = [name, consumer_fun.name.lower(), cons_flow]
-        #         output_list.append(flow_child_producer_list)
-
-        if not any(cons_flow in sublist for sublist in flow_producer_name_list):
-            if not any(cons_flow in sublist for sublist in output_list):
-                output_list.append([None, consumer_fun.name.lower(), cons_flow])
-
-    if concatenate:
-        output_list = concatenate_flows(output_list)
-    return output_list
-
-
-def concatenate_flows(input_list):
-    """@ingroup plantuml_adapter
-    Concatenate the flows with same consumer and producer: from [[cons=A, prod=B, flow_1],
-    [cons=A, prod=B, flow_2]] to [[cons=A, prod=B, [flow_1, flow_2]].
-    Adaptation for flow notation in PlantUml
-    @param[in] input_list
-    @return list of output flows
-    """
-
-    output_list = []
-    per_function_name_filtered_list = set(map(lambda x: (x[0], x[1]), input_list))
-    per_flow_filtered_list = [[y[2] for y in input_list if y[0] == x and y[1] == z] for x, z in
-                              per_function_name_filtered_list]
-    for idx, function in enumerate(per_function_name_filtered_list):
-        output_list.append([function, per_flow_filtered_list[idx]])
-
-    return output_list
-
-
-def get_state_machine_diagram(xml_state_list, xml_transition_list, fun_elem_list=None):
-    """@ingroup plantuml_adapter
-    @anchor get_state_machine_diagram
-    Construct  the PlantUml text and url for state machine diagrams
-    @param[in] xml_state_list TBD
-    @param[in] xml_transition_list TBD
-    @param[in] fun_elem_list TBD
-    @return PlantUml text and url diagram for state machine diagram
-    """
-
-    state_obj_string = StateDiagram()
-    objects_conditions_list = get_objects_conditions_list(xml_state_list, xml_transition_list)
-    already_added_state_id_list = []
-    for state in xml_state_list:
-        if not state.parent and state.child_list:
-            check = False
-            if fun_elem_list:
-                for fun_elem in fun_elem_list:
-                    if state.id in fun_elem.allocated_state_list:
-                        if fun_elem.parent is None:
-                            check = True
-                            state_obj_string.create_state(fun_elem, True)
-
-            write_composed_state(state_obj_string, state, already_added_state_id_list,
-                                 objects_conditions_list)
-            if check:
-                state_obj_string.append_string('}\n')
-
-    for s in xml_state_list:
-        if s.id not in already_added_state_id_list:
-            check = False
-            if fun_elem_list:
-                for fun_elem in fun_elem_list:
-                    if s.id in fun_elem.allocated_state_list:
-                        if fun_elem.parent is None:
-                            check = True
-                            state_obj_string.create_state(fun_elem, True)
-            write_state(state_obj_string, s, already_added_state_id_list, objects_conditions_list)
-            if check:
-                state_obj_string.append_string('}\n')
-
-    for p in objects_conditions_list.copy():
-        if (p[0].id and not p[1].id) or (not p[0].id and p[1].id):
-            state_obj_string.create_transition([p])
-            objects_conditions_list.remove(p)
-
-    return state_obj_string.string
-
-
-def get_objects_conditions_list(xml_state_list, xml_transition_list):
-    """@ingroup plantuml_adapter
-    Return all conditions associated to a list of state within a list of transition
-    @param[in] xml_state_list TBD
-    @param[in] xml_transition_list TBD
-    @return conditions list
-    """
-
-    objects_conditions_list = []
-    formatted_transition_list = []
-    # Create transition's list [src_id, dest_id, [conditions]]
-    for i in xml_transition_list:
-        formatted_transition_list.append([i.source, i.destination, i.condition_list])
-
-    # Create transition's list [src_state_obj, dest_state_obj, [conditions]]
-    for j in formatted_transition_list:
-        result = match_transition_states(j, xml_state_list)
-        if result:
-            objects_conditions_list.append(result)
-
-    return objects_conditions_list
-
-
-def write_state(state_obj_string, state, new, objects_conditions_list):
-    """@ingroup plantuml_adapter
-    Returns simple state string for PlantUml text
-    @param[in, out] state_obj_string TBD
-    @param[in] state TBD
-    @param[in] new TBD
-    @param[in, out] objects_conditions_list TBD
-    @return None
-    """
-
-    if not state.parent and not state.child_list:
-        state_obj_string.create_state(state)
-        new.append(state.id)
-
-    for j in objects_conditions_list:
-        if all(x in new for x in [j[0].id, j[1].id]):
-            state_obj_string.create_transition([j])
-            objects_conditions_list.remove(j)
-
-
-def write_composed_state(state_obj_string, state, new, objects_conditions_list, output_str='',
-                         count=0):
-    """@ingroup plantuml_adapter
-    Returns composed state string for PlantUml text
-    @param[in, out] state_obj_string TBD
-    @param[in] state TBD
-    @param[in] new TBD
-    @param[in, out] objects_conditions_list TBD
-    @param[in] output_str TBD
-    @param[in] count TBD
-    @return None
-    """
-
-    state_obj_string.create_state(state, parent=True)
-    new.insert(count, state.id)
-    count += 1
-    for i in state.child_list:
-        if not i.child_list:
-            state_obj_string.create_state(i)
-            new.insert(count + 1, i.id)
-        else:
-            write_composed_state(state_obj_string, i, new, objects_conditions_list, output_str,
-                                 count)
-
-    for j in objects_conditions_list:
-        if all(x in new for x in [j[0].id, j[1].id]):
-            state_obj_string.create_transition([j])
-            objects_conditions_list.remove(j)
-
-    state_obj_string.append_string("}\n" * count)
-
-
-def match_transition_states(transition, xml_state_list):
-    """@ingroup plantuml_adapter
-    Return transition with associated state.
-    If not, create default ENTRY or EXIT if one is missing
-    @param[in] transition TBD
-    @param[in] xml_state_list TBD
-    @return transition
-    """
-    out = None
-    source_state, destination_state = get_source_and_dest(transition, xml_state_list)
-
-    if source_state is not None and destination_state is not None:
-        out = [source_state, destination_state, transition[2]]
-    elif source_state is not None and destination_state is None:
-        n = datamodel.State()
-        n.set_name('EXIT')
-        xml_state_list.add(n)
-        out = [source_state, n, transition[2]]
-    elif source_state is None and destination_state is not None:
-        n = datamodel.State()
-        n.set_name('ENTRY')
-        xml_state_list.add(n)
-        out = [n, destination_state, transition[2]]
-
-    return out
-
-
-def get_source_and_dest(transition, xml_state_list):
-    """@ingroup plantuml_adapter
-    Iterate over states id to get source and destination objects
-    @param[in] transition TBD
-    @param[in] xml_state_list TBD
-    @return source and destination objects
-    """
-    source_state = None
-    destination_state = None
-
-    for a, b in zip(xml_state_list, xml_state_list):
-        if transition[0] == a.id:
-            source_state = a
-        if transition[1] == b.id:
-            destination_state = b
-        if destination_state and source_state:
-            return source_state, destination_state
-
-    return source_state, destination_state
+"""@defgroup plantuml_adapter
+Plantuml adapter module
+"""
+
+# Modules
+import datamodel
+from .util import ObjDiagram, StateDiagram, SequenceDiagram
+from tools import Logger
+
+
+def write_function_child(string_obj, function, input_flow_list, output_flow_list,
+                         xml_attribute_list):
+    """@ingroup plantuml_adapter
+    Construct PlantUml text recursively
+    @param[in,out] string_obj current PlantUml text
+    @param[in] function
+    @param[in] input_flow_list
+    @param[in] output_flow_list
+    @param[in] xml_attribute_list
+    @return None
+    """
+
+    function_input_port = []
+    function_output_port = []
+    external_input_port = []
+    external_output_port = []
+    parent_function_port = []
+    count = 1
+    parent_function_port_count = 1
+    nb_component = count_composed_component(function, count)
+
+    # TODO: Create get_port_lists() and optimize
+    for p in input_flow_list.copy():
+        if p[0][0] == function.name.lower():
+            function_input_port.append(p)
+        if p[0][0] is None and function.parent is None:
+            external_input_port.append(p)
+            if p[0][1] == function.name.lower():
+                p_new = [(p[0][0], function.name.lower() + "_" + str(parent_function_port_count)), p[1]]
+                parent_function_port.append(p_new)
+                parent_function_port_count = parent_function_port_count + 1
+                input_flow_list.remove(p)
+                input_flow_list.append(p_new)
+
+    for q in output_flow_list.copy():
+        if q[0][0] == function.name.lower():
+            function_output_port.append(q)
+        if q[0][0] is None and function.parent is None:
+            external_output_port.append(q)
+            if q[0][1] == function.name.lower():
+                q_new = [(q[0][0], function.name.lower() + "_" + str(parent_function_port_count)), q[1]]
+                parent_function_port.append(q_new)
+                parent_function_port_count = parent_function_port_count + 1
+                output_flow_list.remove(q)
+                output_flow_list.append(q_new)
+
+    Logger.set_debug(__name__, f"Function name: {function.name}")
+    Logger.set_debug(__name__, f"Input port list: {function_input_port}")
+    Logger.set_debug(__name__, f"Output port list: {function_input_port}")
+    Logger.set_debug(__name__, f"Parent function port list: {parent_function_port}")
+    Logger.set_debug(__name__, f"External input port list: {external_input_port}")
+    Logger.set_debug(__name__, f"External output port list: {external_output_port}")
+
+    string_obj.create_port(function_input_port, "in")
+    string_obj.create_port(function_output_port, "out")
+    string_obj.create_port(parent_function_port, 'None')
+
+    child_with_no_child_list = []
+    child_with_child_list = []
+    # Create a child list for each parent function
+    for child_function in function.child_list:
+        Logger.set_debug(__name__, f"{child_function.name} check as child of {function.name}")
+        if child_function.child_list:
+            child_with_child_list.append(child_function)
+        else:
+            child_with_no_child_list.append(child_function)
+
+    # For child that has no child: create object
+    for fun in child_with_no_child_list:
+        string_obj.create_object(fun, xml_attribute_list)
+
+    for child in child_with_child_list:
+        string_obj.create_component(child)
+        write_function_child(string_obj, child, input_flow_list, output_flow_list,
+                             xml_attribute_list)
+        nb_component -= 1
+
+    # Close all the brackets depending on the number of component within highest parent
+    for i in range(nb_component):
+        string_obj.append_string('}\n')
+
+    for component in child_with_child_list:
+        string_obj.create_component_attribute(component, xml_attribute_list)
+
+    whole_child_list = child_with_child_list + child_with_no_child_list
+    for fun in whole_child_list:
+        for i in input_flow_list:
+            if i[0][0] == fun.name.lower():
+                string_obj.create_port(input_flow_list, "in")
+        for j in output_flow_list:
+            if j[0][0] == fun.name.lower():
+                string_obj.create_port(output_flow_list, "out")
+
+    string_obj.create_port(external_input_port, "in")
+    string_obj.create_port(external_output_port, "out")
+
+
+def count_composed_component(function, count):
+    """@ingroup plantuml_adapter
+    Count the number of composed function within the higher function
+    @param[in] function function to check
+    @param[in] count number of component
+    @return number of component
+    """
+
+    for elem in function.child_list:
+        if elem.child_list:
+            count += 1
+            count_composed_component(elem, count)
+            continue
+    return count
+
+
+def write_function_object(string_obj, function, input_flow_list, output_flow_list, check,
+                          xml_attribute_list, component_obj=None, compo_diagram=False):
+    """@ingroup plantuml_adapter
+    Construct the PlantUml text for a function object with associated ports for flow lists.
+    @param[in,out] string_obj current PlantUml text
+    @param[in] function
+    @param[in] input_flow_list
+    @param[in] output_flow_list
+    @param[in] check
+    @param[in] xml_attribute_list
+    @param[in] component_obj
+    @param[in] compo_diagram
+    @return PlantUml text for the function object
+    """
+
+    string_obj.create_object(function, xml_attribute_list)
+
+    if check:
+        string_obj.append_string('}\n')
+        if component_obj:
+            string_obj.create_component_attribute(component_obj, xml_attribute_list)
+
+    for p in input_flow_list:
+        if compo_diagram:
+            if p[0][0] == function.name.lower():
+                string_obj.create_port(input_flow_list, "in")
+        else:
+            if p[0][0] == function.name.lower() or p[0][1] == function.name.lower():
+                string_obj.create_port(input_flow_list, "in")
+    for q in output_flow_list:
+        if compo_diagram:
+            if q[0][0] == function.name.lower():
+                string_obj.create_port(output_flow_list, "out")
+        else:
+            if q[0][0] == function.name.lower() or q[0][1] == function.name.lower():
+                string_obj.create_port(output_flow_list, "out")
+
+
+def get_function_diagrams(function_list, fun_elem_list, consumer_function_list, producer_function_list,
+                          parent_child_dict, data_list, xml_type_list, xml_attribute_list):
+    """@ingroup plantuml_adapter
+    @anchor get_function_diagrams
+    Construct the PlantUml text and url for the requested diagram between one of the following:
+    - context of function
+    - decomposition of function
+    - chain of function
+    @param[in] function_list
+    @param[in] consumer_function_list
+    @param[in] producer_function_list
+    @param[in] parent_child_dict
+    @param[in] data_list
+    @param[in] xml_type_list
+    @param[in] xml_attribute_list
+    @return PlantUml text and url of the diagram
+    """
+
+    string_obj = ObjDiagram()
+    # Filter output flows
+    output_flow_list = get_output_flows(consumer_function_list, producer_function_list,
+                                        concatenate=True)
+    # Filter input flows
+    input_flow_list = get_input_flows(consumer_function_list, producer_function_list,
+                                      concatenate=True)
+
+    # Filter consumers and producers list in order to create data flow
+    data_flow_list = get_exchanged_flows(consumer_function_list, producer_function_list,
+                                         parent_child_dict, concatenate=True)
+
+    Logger.set_debug(__name__, f"Output flows list: {output_flow_list}")
+    Logger.set_debug(__name__, f"Input flows list: {input_flow_list}")
+    Logger.set_debug(__name__, f'Exchanged flows list: {data_flow_list}')
+
+    if data_list:
+        per_message_data_flow_list = get_exchanged_flows(consumer_function_list,
+                                                         producer_function_list,
+                                                         parent_child_dict)
+        if len(data_list) == len(per_message_data_flow_list):
+            ordered_function_list, ordered_message_list = order_list(per_message_data_flow_list,
+                                                                     data_list)
+            if per_message_data_flow_list != ordered_message_list:
+                for idx, i in enumerate(ordered_message_list):
+                    for j in data_flow_list:
+                        for k in j[1]:
+                            if i[2] == k and i[3]:
+                                new = str(idx + 1) + ":" + k
+                                j[1].remove(k)
+                                j[1].append(new)
+
+    # Loop in order to filter functions and write in output's file, see write_function_child()
+    if parent_child_dict:
+        if fun_elem_list:
+            for fun_elem in fun_elem_list:
+                if fun_elem.id not in parent_child_dict.keys():
+                    if fun_elem.id in parent_child_dict.values():
+                        # Fun elem is a parent
+                        string_obj.create_component(fun_elem)
+                        check_function = False
+                        for key, value in parent_child_dict.items():
+                            if value == fun_elem.id:
+                                is_fun_elem_child = False
+                                for fun_elem_child in fun_elem_list:
+                                    if fun_elem_child.id == key:
+                                        is_fun_elem_child = True
+                                        string_obj.create_component(fun_elem_child)
+                                        check_function = False
+                                        for f in function_list:
+                                            if any(a == f.id for a in fun_elem_child.allocated_function_list):
+                                                if len(fun_elem.allocated_function_list) > 1:
+                                                    check_function = False
+                                                else:
+                                                    check_function = True
+                                                write_function_object(string_obj, f, input_flow_list, output_flow_list,
+                                                                      check_function, xml_attribute_list,
+                                                                      component_obj=fun_elem_child)
+
+                                        if not check_function:
+                                            string_obj.append_string('}\n')
+                                            string_obj.create_component_attribute(fun_elem_child, xml_attribute_list)
+
+                                check_function = False
+                                if not is_fun_elem_child:
+                                    for f in function_list:
+                                        if any(a == f.id for a in fun_elem.allocated_function_list):
+                                            if f.id == key:
+                                                if len(fun_elem.allocated_function_list) > 1:
+                                                    check_function = False
+                                                else:
+                                                    check_function = True
+                                                write_function_object(string_obj, f, input_flow_list, output_flow_list,
+                                                                      check_function,
+                                                                      xml_attribute_list,
+                                                                      component_obj=fun_elem)
+
+                        if not check_function:
+                            string_obj.append_string('}\n')
+                        string_obj.create_component_attribute(fun_elem, xml_attribute_list)
+                    # Else do nothing : done as children of fun elem parent
+                # Else do nothing : done as children of fun elem parent
+        else:
+            for function in function_list:
+                if function.id not in parent_child_dict.keys():
+                    if function.id in parent_child_dict.values():
+                        # Function is a parent
+                        string_obj.create_component(function)
+                        write_function_child(string_obj, function, input_flow_list, output_flow_list,
+                                             xml_attribute_list)
+                        string_obj.create_component_attribute(function, xml_attribute_list)
+                    else:
+                        # Function is not a parent:
+                        write_function_object(string_obj, function, input_flow_list, output_flow_list,
+                                              False, xml_attribute_list, compo_diagram=True)
+                # Else do nothing : done as children of function parent
+    else:
+        for function in function_list:
+            write_function_object(string_obj, function, input_flow_list, output_flow_list, False,
+                                  xml_attribute_list)
+
+    string_obj.create_input_flow(input_flow_list)
+    string_obj.create_output_flow(output_flow_list)
+    string_obj.create_data_flow(data_flow_list)
+
+    return string_obj.string
+
+
+def get_fun_elem_context_diagram(function_list, consumer_function_list, producer_function_list,
+                                 data_list, xml_attribute_list, fun_elem_list, fun_inter_list):
+    """@ingroup plantuml_adapter
+    @anchor get_fun_elem_context_diagram
+    Construct the PlantUml text and url for the context diagram for functional elements
+    @param[in] function_list TBD
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] data_list TBD
+    @param[in] xml_attribute_list TBD
+    @param[in] fun_elem_list TBD
+    @param[in] fun_inter_list TBD
+    @return PlantUml text and url of the diagram
+    """
+
+    string_obj = ObjDiagram()
+    interface_list = None
+
+    if fun_inter_list:
+
+        unmerged_data_list = get_exchanged_flows(consumer_function_list, producer_function_list, {})
+        interface_list, data_flow_list = get_interface_list(fun_inter_list,
+                                                            data_list,
+                                                            unmerged_data_list,
+                                                            function_list,
+                                                            fun_elem_list,
+                                                            is_decomposition=False)
+
+        data_flow_list = concatenate_flows(data_flow_list)
+
+    else:
+
+        # Filter consumers and producers list in order to create data flow
+        data_flow_list = get_exchanged_flows(consumer_function_list, producer_function_list,
+                                             {}, concatenate=True)
+
+    # Filter output flows
+    output_flow_list = get_output_flows(consumer_function_list, producer_function_list,
+                                        concatenate=True)
+    # Filter input flows
+    input_flow_list = get_input_flows(consumer_function_list, producer_function_list,
+                                      concatenate=True)
+
+    # Write external functions
+    external_function_list = []
+    for function in function_list:
+        is_external = True
+        for fun_elem in fun_elem_list:
+            if any(a == function.id for a in fun_elem.allocated_function_list):
+                is_external = False
+
+        if is_external:
+            external_function_list.append(function)
+
+    for function in external_function_list:
+        string_obj.create_object(function, xml_attribute_list)
+
+    for fun_elem in fun_elem_list:
+        string_obj.create_component(fun_elem)
+        check_function = False
+        for f in function_list:
+            if any(a == f.id for a in fun_elem.allocated_function_list):
+                if len(fun_elem.allocated_function_list) > 1:
+                    check_function = False
+                else:
+                    check_function = True
+                write_function_object(string_obj, f, input_flow_list, output_flow_list,
+                                      check_function, xml_attribute_list, component_obj=fun_elem)
+        if not check_function:
+            string_obj.append_string('}\n')
+            string_obj.create_component_attribute(fun_elem, xml_attribute_list)
+
+    string_obj.create_input_flow(input_flow_list)
+    string_obj.create_output_flow(output_flow_list)
+    string_obj.create_data_flow(data_flow_list)
+
+    if interface_list:
+        string_obj.create_interface(interface_list)
+
+    return string_obj.string
+
+
+def get_interface_list(fun_inter_list, data_list, data_flow_list, function_list, fun_elem_list,
+                       is_decomposition=True):
+    """@ingroup plantuml_adapter
+    Get list of functional interfaces with the functional elements exposing them.
+    Functional interface is returned only when specifed data is allocated to it
+    @param[in] fun_inter_list TBD
+    @param[in] data_list TBD
+    @param[in] data_flow_list TBD
+    @param[in] function_list TBD
+    @param[in] fun_elem_list TBD
+    @param[in] is_decomposition indicates if decomposition is required (True) or not (False)
+    @return functional interfaces list
+    """
+
+    interface_list = []
+    removed_data_flow_list = []
+    initial_data = list(data_flow_list)
+    idx = 0
+    # Get all fun_inter with allocated data within data_flow_list and create interface list
+    # [[producer, consumer, fun_inter]...]
+    for fun_inter in fun_inter_list:
+        Logger.set_debug(__name__, f"Interface {fun_inter.name}, allocated data {fun_inter.allocated_data_list}")
+        if fun_inter.allocated_data_list:
+            for data_id in fun_inter.allocated_data_list:
+                for data in data_list:
+                    if data_id == data.id:
+                        for data_flow in data_flow_list.copy():
+                            if data.name == data_flow[2]:
+                                first_fun = None
+                                second_fun = None
+                                for fun in function_list:
+                                    if data_flow[0] == fun.name.lower():
+                                        first_fun = fun
+                                    if data_flow[1] == fun.name.lower():
+                                        second_fun = fun
+
+                                if first_fun or second_fun:
+                                    # Need to check consistency between [elem1, elem2, fun_inter] and [fun1, fun2, data]
+                                    # before adding to the list
+                                    is_first_fun_elem = False
+                                    is_second_fun_elem = False
+                                    for fun_elem in fun_elem_list:
+                                        if any(exposed_fun_inter_id == fun_inter.id for exposed_fun_inter_id in
+                                               fun_elem.exposed_interface_list):
+                                            if first_fun and not is_first_fun_elem:
+                                                is_first_fun_elem = any(allocated_fun_id ==
+                                                                        first_fun.id for allocated_fun_id
+                                                                        in fun_elem.allocated_function_list)
+                                            if second_fun and not is_second_fun_elem:
+                                                is_second_fun_elem = any(allocated_fun_id ==
+                                                                         second_fun.id for allocated_fun_id
+                                                                         in fun_elem.allocated_function_list)
+
+                                    if (first_fun and is_first_fun_elem and not second_fun) or \
+                                            (second_fun and is_second_fun_elem and not first_fun) or \
+                                            (first_fun and is_first_fun_elem and second_fun and is_second_fun_elem):
+                                        Logger.set_debug(__name__, f"[{first_fun}, {second_fun}, {fun_inter}] added")
+                                        interface_list.insert(idx, [first_fun, second_fun, fun_inter])
+                                        removed_data_flow_list.insert(idx, data_flow)
+                                        data_flow_list.remove(data_flow)
+                                        idx += 1
+                                        break
+        else:
+            Logger.set_info(__name__, f"{fun_inter.name} does not have any allocated data (no display)")
+
+    output_list, interface_list = get_fun_elem_from_fun_inter(interface_list, fun_elem_list, is_decomposition)
+
+    if not output_list:
+        return None, initial_data
+
+    # (re)Add [producer, consumer, data_name] to data_flow_list if no interface exposed
+    if any(isinstance(s, list) for s in interface_list):
+        for idx, rest_inter in enumerate(interface_list):
+            if isinstance(rest_inter, list):
+                data_flow_list.append(removed_data_flow_list[idx])
+
+    return output_list, data_flow_list
+
+
+def get_fun_elem_from_fun_inter(interface_list, fun_elem_list, is_decomposition=True):
+    """@ingroup plantuml_adapter
+    Get list of functional interfaces with the functional elements exposing them from interface_list =
+    [[producer, consumer, fun_inter]...] and put value to False if (first, second, interface)
+    have been added to output_list (i.e. fun_elem_1/fun_elem_2 have been found for a fun_inter)
+    @param[in] interface_list TBD
+    @param[in] fun_elem_list TBD
+    @param[in] is_decomposition indicates if decomposition is required (True) or not (False)
+    @return functional interfaces list
+    """
+
+    output_list = []
+    for ix, (first, second, interface) in enumerate(interface_list):
+        fun_elem_1 = None
+        fun_elem_2 = None
+        if first:
+            for elem_1 in fun_elem_list:
+                if any(s == interface.id for s in elem_1.exposed_interface_list):
+                    if is_decomposition:
+                        if not elem_1.child_list:
+                            fun_elem_1 = elem_1
+                        else:
+                            check = True
+                            for child in elem_1.child_list:
+                                if any(s == interface.id for s in child.exposed_interface_list):
+                                    check = False
+                            if check:
+                                fun_elem_1 = elem_1
+                    else:
+                        fun_elem_1 = elem_1
+
+        if second:
+            for elem_2 in fun_elem_list:
+                if not first:
+                    if is_decomposition:
+                        if any(s == interface.id for s in elem_2.exposed_interface_list):
+                            if not elem_2.child_list:
+                                fun_elem_2 = elem_2
+                            else:
+                                check = True
+                                for child in elem_2.child_list:
+                                    if any(s == interface.id for s in child.exposed_interface_list):
+                                        check = False
+                                if check:
+                                    fun_elem_2 = elem_2
+                    else:
+                        fun_elem_2 = elem_2
+                else:
+                    if any(s == interface.id for s in elem_2.exposed_interface_list) and \
+                            elem_2 != fun_elem_1:
+                        if is_decomposition:
+                            if not elem_2.child_list:
+                                fun_elem_2 = elem_2
+                            else:
+                                check = True
+                                for child in elem_2.child_list:
+                                    if any(s == interface.id for s in child.exposed_interface_list):
+                                        check = False
+
+                                if check:
+                                    fun_elem_2 = elem_2
+                        else:
+                            fun_elem_2 = elem_2
+
+        if not (not fun_elem_1 and not fun_elem_2):
+            if [fun_elem_1, fun_elem_2, interface] not in output_list:
+                output_list.append([fun_elem_1, fun_elem_2, interface])
+            interface_list[ix] = False
+
+    return output_list, interface_list
+
+
+def check_child_allocation(string_obj, fun_elem, function_list, xml_attribute_list):
+    """@ingroup plantuml_adapter
+    Check for each function allocated to a functional element if not allocated to any
+    functional element child: in that case => write function object string.
+    @param[in,out] string_obj current PlantUml text
+    @param[in] fun_elem functional element to check
+    @param[in] function_list list of functions
+    @param[in] xml_attribute_list xml list of attributes
+    @return None
+    """
+
+    for function in function_list:
+        if function.id in fun_elem.allocated_function_list:
+            fun_elem_child_allocated_function_list = []
+            for c in fun_elem.child_list:
+                for j in c.allocated_function_list:
+                    fun_elem_child_allocated_function_list.append(j)
+
+            if not any(s == function.id for s in fun_elem_child_allocated_function_list):
+                write_function_object(string_obj, function, [], [], False, xml_attribute_list)
+
+
+def recursive_decomposition(string_obj, main_fun_elem, function_list, xml_attribute_list,
+                            first_iter=False):
+    """@ingroup plantuml_adapter
+    Create PlantUml text for functional elements recursively
+    @param[in,out] string_obj current PlantUml text
+    @param[in] main_fun_elem
+    @param[in] function_list list of functions
+    @param[in] xml_attribute_list xml list of attributes
+    @param[in] first_iter
+    @return None
+    """
+
+    if first_iter is True:
+        string_obj.create_component(main_fun_elem)
+        check_child_allocation(string_obj, main_fun_elem, function_list, xml_attribute_list)
+        if main_fun_elem.child_list:
+            recursive_decomposition(string_obj, main_fun_elem, function_list, xml_attribute_list)
+    else:
+        for c in main_fun_elem.child_list:
+            string_obj.create_component(c)
+            check_child_allocation(string_obj, c, function_list, xml_attribute_list)
+            if c.child_list:
+                recursive_decomposition(string_obj, c, function_list, xml_attribute_list)
+            string_obj.append_string('}\n')
+            string_obj.create_component_attribute(c, xml_attribute_list)
+
+
+def get_fun_elem_decomposition(main_fun_elem, fun_elem_list, allocated_function_list, consumer_list,
+                               producer_list, external_function_list, xml_attribute_list,
+                               data_list, fun_inter_list):
+    """@ingroup plantuml_adapter
+    @anchor get_fun_elem_decomposition
+    Construct the PlantUml text for the functional element decomposition diagram
+    @param[in] main_fun_elem main functional element
+    @param[in] fun_elem_list functional element list
+    @param[in] allocated_function_list list of allocated functions to main functional element
+    @param[in] consumer_list filtered consumers list
+    @param[in] producer_list filtered producers list
+    @param[in] external_function_list filtered external functions list
+    @param[in] xml_attribute_list xml list of attributes
+    @param[in] data_list data list
+    @param[in] fun_inter_list functional interface list
+    @return PlantUml text of the diagram
+    """
+
+    string_obj = ObjDiagram()
+    interface_list = None
+
+    if fun_inter_list:
+        unmerged_data_list = get_exchanged_flows(consumer_list, producer_list, {})
+        interface_list, data_flow_list = get_interface_list(fun_inter_list,
+                                                            data_list,
+                                                            unmerged_data_list,
+                                                            allocated_function_list.
+                                                            union(external_function_list),
+                                                            fun_elem_list,
+                                                            is_decomposition=True)
+
+        data_flow_list = concatenate_flows(data_flow_list)
+
+    else:
+        # Filter consumers and producers list in order to create data flow
+        data_flow_list = get_exchanged_flows(consumer_list, producer_list, {}, concatenate=True)
+
+    # Write external functions that are not already allocated to external components
+    external_function_not_allocated_list = []
+    for function in external_function_list:
+        is_external = True
+        for fun_elem in fun_elem_list:
+            if any(a == function.id for a in fun_elem.allocated_function_list):
+                is_external = False
+
+        if is_external:
+            external_function_not_allocated_list.append(function)
+
+    for function in external_function_not_allocated_list:
+        string_obj.create_object(function, xml_attribute_list)
+
+    # Write functional element decompo recursively and add allocated functions
+    recursive_decomposition(string_obj, main_fun_elem, allocated_function_list, xml_attribute_list,
+                            first_iter=True)
+    string_obj.append_string('}\n')
+    string_obj.create_component_attribute(main_fun_elem, xml_attribute_list)
+    # Write external fun_elem
+    for elem in fun_elem_list:
+        if elem != main_fun_elem and elem.parent is None:
+            recursive_decomposition(string_obj, elem, external_function_list, xml_attribute_list,
+                                    first_iter=True)
+            string_obj.append_string('}\n')
+            string_obj.create_component_attribute(elem, xml_attribute_list)
+
+    # Write data flows
+    string_obj.create_data_flow(data_flow_list)
+    if interface_list:
+        string_obj.create_interface(interface_list)
+
+    return string_obj.string
+
+
+def get_sequence_diagram(function_list, consumer_function_list, producer_function_list,
+                         parent_child_dict, data_list, str_out=False):
+    """@ingroup plantuml_adapter
+    @anchor get_sequence_diagram
+    Construct the PlantUml text for the sequence diagrams
+    @param[in] function_list TBD
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] parent_child_dict TBD
+    @param[in] data_list TBD
+    @return PlantUml text of the diagram
+    """
+
+    seq_obj_string = SequenceDiagram()
+
+    message_list = get_exchanged_flows(consumer_function_list, producer_function_list,
+                                       parent_child_dict)
+    ordered_function_list, ordered_message_list = order_list(message_list, data_list)
+
+    if ordered_function_list:
+        for fun_name in ordered_function_list:
+            for f in function_list:
+                if fun_name == f.name.lower():
+                    seq_obj_string.create_participant(f)
+    else:
+        for f in function_list:
+            seq_obj_string.create_participant(f)
+
+    seq_obj_string.create_sequence_message(ordered_message_list)
+
+    return seq_obj_string.string
+
+
+def get_predecessor_list(data):
+    """@ingroup plantuml_adapter
+    Get the predecessor's list for a Data object
+    @param[in] data data object
+    @return predecessor list
+    """
+
+    predecessor_list = set()
+    if data.predecessor_list:
+        for predecessor in data.predecessor_list:
+            predecessor_list.add(predecessor)
+
+    return predecessor_list
+
+
+def check_sequence(predecessor_list, sequence):
+    """@ingroup plantuml_adapter
+    Check if predecessors of a data are in a sequence
+    @param[in] predecessor_list predecessor list
+    @param[in] sequence sequence
+    @return TRUE (predecessors are in the sequence) or FALSE
+    """
+
+    check = False
+    if predecessor_list == set():
+        check = None
+        return check
+
+    pred_set = set()
+    seq_set = set()
+    for pred in predecessor_list:
+        pred_set.add(pred.name)
+    for elem in sequence:
+        seq_set.add(elem[2].name)
+
+    if pred_set.issubset(seq_set):
+        check = True
+        return check
+
+    return check
+
+
+def clean_predecessor_list(message_object_list):
+    """@ingroup plantuml_adapter
+    Delete predecessor if not in the message's list
+    @param[in] message_object_list TBD
+    @return updated message list
+    """
+
+    for message in message_object_list:
+        pred_list = get_predecessor_list(message[2])
+        for pred in pred_list:
+            if not any(pred in s for s in message_object_list):
+                message[2].predecessor_list.remove(pred)
+
+    return message_object_list
+
+
+def get_sequence(message, message_object_list, sequence_list, sequence=None, index=None):
+    """@ingroup plantuml_adapter
+    Return a sequence for a given message
+    @param[in] message TBD
+    @param[in] message_object_list TBD
+    @param[in] sequence_list TBD
+    @param[in] sequence TBD
+    @param[in] index TBD
+    @return sequence
+    """
+    if not sequence:
+        sequence = []
+        index = 0
+    if message not in sequence and not any(message in s for s in sequence_list) is True:
+        message[3] = True
+        sequence.insert(index, message)
+        index += 1
+        for mess in message_object_list:
+            if message[2] in mess[2].predecessor_list:
+                get_sequence(mess, message_object_list, sequence_list, sequence, index)
+
+    return sequence
+
+
+def get_sequences(message_object_list):
+    """@ingroup plantuml_adapter
+    Group all sequences into a sequence list
+    @param[in] message_object_list
+    @return sequence list
+    """
+
+    sequence_list = []
+    for message in message_object_list:
+        if not message[2].predecessor_list:
+            sequence = get_sequence(message, message_object_list, sequence_list)
+            sequence_list.append(sequence)
+
+    return sequence_list
+
+
+def post_check_sequence(sequence_list):
+    """@ingroup plantuml_adapter
+    Check if message isn't missing in sequence, insert it at the good place and loop if not
+    well ordered (predecessor after each one)
+    @param[in] sequence_list TBD
+    @return sequence list ordered
+    """
+
+    for (idx, i) in enumerate(sequence_list):
+        pred = i[2].predecessor_list
+        if check_sequence(pred, sequence_list[:idx]) is True:
+            pass
+        elif check_sequence(pred, sequence_list[:idx]) is False:
+            for (index, elem) in enumerate(sequence_list.copy()):
+                curr_pred = elem[2].predecessor_list
+                if check_sequence(curr_pred, sequence_list[:index]) is True:
+                    sequence_list.remove(i)
+                    sequence_list.insert(index + 1, i)
+                    index += 1
+                else:
+                    continue
+        elif check_sequence(pred, sequence_list[:idx]) is None:
+            pass
+        idx += 1
+
+    for (new_idx, message) in enumerate(sequence_list):
+        new_pred = message[2].predecessor_list
+        if check_sequence(new_pred, sequence_list[:new_idx]) is False:
+            post_check_sequence(sequence_list)
+
+    return sequence_list
+
+
+def get_sequence_list(message_object_list):
+    """@ingroup plantuml_adapter
+    Call for sequences then clean_up and post_check
+    @param[in] message_object_list TBD
+    @return sequence list
+    """
+    sequence_list = get_sequences(message_object_list)
+
+    sequence_list = sorted(sequence_list, key=lambda x: len(x), reverse=True)
+    # Could be possible to implement this part within post_check_sequence()
+    for (index, i) in enumerate(sequence_list):
+        main_list = sequence_list[0]
+        if index > 0:
+            start = 0
+            for j in i.copy():
+                if not j[2].predecessor_list:
+                    i.remove(j)
+                    main_list.insert(start, j)
+                    start += 1
+
+    sequence_list = [item for sub in sequence_list for item in sub]
+    sequence_list = post_check_sequence(sequence_list)
+
+    return sequence_list
+
+
+def order_list(message_list, data_list):
+    """@ingroup plantuml_adapter
+    Order functions and messages
+    @param[in] message_list TBD
+    @param[in] data_list TBD
+    @return ordered message list and ordered function list
+    """
+
+    ordered_message_list = []
+    ordered_function_list = []
+    message_object_list = []
+
+    for i in message_list:
+        for data in data_list:
+            if i[2] == data.name:
+                message_object_list.append([i[0], i[1], data, False])
+
+    message_object_list = clean_predecessor_list(message_object_list)
+    ordored_message_object_list = get_sequence_list(message_object_list)
+
+    # Add index for each item within the list
+    for idx, t in enumerate(ordored_message_object_list):
+        ordered_message_list.insert(idx, [t[0], t[1], t[2].name, t[3]])
+
+    # Create the ordered(from ordered message list) function's list
+    # Starting with producers
+    for idx, m in enumerate(ordered_message_list):
+        if m[0] not in ordered_function_list:
+            ordered_function_list.insert(idx, m[0])
+    # Finishing with consumers
+    for j in message_list:
+        if j[1] not in ordered_function_list:
+            ordered_function_list.append(j[1])
+
+    return ordered_function_list, ordered_message_list
+
+
+def get_exchanged_flows(consumer_function_list, producer_function_list, parent_child_dict,
+                        concatenate=False):
+    """@ingroup plantuml_adapter
+    Return list of exchanged flows [[producer, consumer, data]], i.e. data that have
+    producer and consumer
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] parent_child_dict TBD
+    @param[in] concatenate TBD
+    @return list of exchanged flows
+    """
+
+    output_list = []
+
+    for producer_flow, producer_function in producer_function_list:
+        Logger.set_debug(__name__, f'Producer flow: {producer_flow}; '
+                                   f'function: {producer_function.id}, {producer_function.name}')
+        if not producer_function.child_list or not parent_child_dict:
+            for cons_flow, consumer_function in consumer_function_list:
+                Logger.set_debug(__name__, f'Consumer flow: {cons_flow}; '
+                                           f'function: {consumer_function.id}, {consumer_function.name}')
+                if (not consumer_function.child_list or not parent_child_dict) and cons_flow == producer_flow:
+                    output_list.append(
+                        [producer_function.name.lower(), consumer_function.name.lower(),
+                         producer_flow])
+
+    if concatenate:
+        output_list = concatenate_flows(output_list)
+
+    return output_list
+
+
+def get_output_flows(consumer_function_list, producer_function_list, concatenate=False):
+    """@ingroup plantuml_adapter
+    Return list of output flows [[None/parent_name, producer, data]], i.e. data that
+    have only producer
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] concatenate TBD
+    @return list of output flows
+    """
+    flow_consumer_name_list = []
+    flow_child_consumer_list = []
+    temp_input_list = []
+    output_list = []
+
+    for flow, cons in consumer_function_list:
+        flow_consumer_name_list.append([flow, cons.name.lower()])
+        if cons.child_list is not None:
+            for child in cons.child_list:
+                flow_child = [flow, child.name.lower()]
+                if [flow, child] in consumer_function_list:
+                    flow_child_consumer_list.append(flow_child)
+
+    for consumer_flow, consumer_function in consumer_function_list:
+        if len(consumer_function.child_list) > 0:
+            if len(flow_child_consumer_list) > 0:
+                if not any(consumer_flow in sublist for sublist in flow_child_consumer_list):
+                    temp_input_list.append([consumer_function.name.lower(), consumer_flow])
+            if len(flow_child_consumer_list) == 0:
+                temp_input_list.append([consumer_function.name.lower(), consumer_flow])
+
+    for producer_flow, producer_function in producer_function_list:
+        if not any(producer_flow in sublist for sublist in flow_consumer_name_list):
+            output_list.append([None, producer_function.name.lower(), producer_flow])
+
+    if concatenate:
+        output_list = concatenate_flows(output_list)
+
+    return output_list
+
+
+def get_input_flows(consumer_function_list, producer_function_list, concatenate=False):
+    """@ingroup plantuml_adapter
+    Return list of input flow [[None/parent_name, consumer, data]], i.e. data that
+    have only consumer
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] concatenate TBD
+    @return list of input flows
+    """
+
+    flow_producer_name_list = []
+    flow_child_producer_list = []
+    temp_input_list = []
+    output_list = []
+
+    for flow, prod in producer_function_list:
+        flow_producer_name_list.append([flow, prod.name.lower()])
+        if prod.child_list is not None:
+            for child in prod.child_list:
+                flow_child = [flow, child.name.lower()]
+                if [flow, child] in producer_function_list:
+                    flow_child_producer_list.append(flow_child)
+
+    for producer_flow, producer_function in producer_function_list:
+        if len(producer_function.child_list) > 0:
+            if len(flow_child_producer_list) > 0:
+                if not any(producer_flow in sublist for sublist in flow_child_producer_list):
+                    temp_input_list.append([producer_function.name.lower(), producer_flow])
+            if len(flow_child_producer_list) == 0:
+                temp_input_list.append([producer_function.name.lower(), producer_flow])
+
+    for cons_flow, consumer_fun in consumer_function_list:
+        if not any(cons_flow in sublist for sublist in flow_producer_name_list):
+            output_list.append([None, consumer_fun.name.lower(), cons_flow])
+
+    if concatenate:
+        output_list = concatenate_flows(output_list)
+    return output_list
+
+
+def concatenate_flows(input_list):
+    """@ingroup plantuml_adapter
+    Concatenate the flows with same consumer and producer: from [[cons=A, prod=B, flow_1],
+    [cons=A, prod=B, flow_2]] to [[cons=A, prod=B, [flow_1, flow_2]].
+    Adaptation for flow notation in PlantUml
+    @param[in] input_list
+    @return list of output flows
+    """
+
+    output_list = []
+    per_function_name_filtered_list = set(map(lambda x: (x[0], x[1]), input_list))
+    per_flow_filtered_list = [[y[2] for y in input_list if y[0] == x and y[1] == z] for x, z in
+                              per_function_name_filtered_list]
+    for idx, function in enumerate(per_function_name_filtered_list):
+        output_list.append([function, per_flow_filtered_list[idx]])
+
+    return output_list
+
+
+def get_state_machine_diagram(xml_state_list, xml_transition_list, fun_elem_list=None):
+    """@ingroup plantuml_adapter
+    @anchor get_state_machine_diagram
+    Construct  the PlantUml text and url for state machine diagrams
+    @param[in] xml_state_list TBD
+    @param[in] xml_transition_list TBD
+    @param[in] fun_elem_list TBD
+    @return PlantUml text and url diagram for state machine diagram
+    """
+
+    state_obj_string = StateDiagram()
+    objects_conditions_list = get_objects_conditions_list(xml_state_list, xml_transition_list)
+    already_added_state_id_list = []
+    for state in xml_state_list:
+        if not state.parent and state.child_list:
+            check = False
+            if fun_elem_list:
+                for fun_elem in fun_elem_list:
+                    if state.id in fun_elem.allocated_state_list:
+                        if fun_elem.parent is None:
+                            check = True
+                            state_obj_string.create_state(fun_elem, True)
+
+            write_composed_state(state_obj_string, state, already_added_state_id_list)
+            if check:
+                state_obj_string.append_string('}\n')
+
+    for state in xml_state_list:
+        if state.id not in already_added_state_id_list:
+            check = False
+            if fun_elem_list:
+                for fun_elem in fun_elem_list:
+                    if state.id in fun_elem.allocated_state_list:
+                        if fun_elem.parent is None:
+                            check = True
+                            state_obj_string.create_state(fun_elem, True)
+            write_state(state_obj_string, state, already_added_state_id_list)
+            if check:
+                state_obj_string.append_string('}\n')
+
+    for state in xml_state_list:
+        write_transition(state_obj_string, state, objects_conditions_list)
+
+    return state_obj_string.string
+
+
+def get_objects_conditions_list(xml_state_list, xml_transition_list):
+    """@ingroup plantuml_adapter
+    Return all conditions associated to a list of state within a list of transition
+    @param[in] xml_state_list TBD
+    @param[in] xml_transition_list TBD
+    @return conditions list
+    """
+
+    objects_conditions_list = []
+    formatted_transition_list = []
+    # Create transition's list [name, src_id, dest_id, [conditions]]
+    for transition in xml_transition_list:
+        formatted_transition_list.append([transition.name, transition.source, transition.destination,
+                                          transition.condition_list])
+
+    # Create transition's list [src_state_obj, dest_state_obj, [conditions]]
+    for formatted_transition in formatted_transition_list:
+        src_state_obj = None
+        dest_state_obj = None
+        for state in xml_state_list:
+            if formatted_transition[1] == state.id:
+                src_state_obj = state
+            # Else do nothing
+
+            if formatted_transition[2] == state.id:
+                dest_state_obj = state
+            # Else do nothing
+
+        if src_state_obj is not None and dest_state_obj is not None:
+            objects_conditions_list.append([src_state_obj, dest_state_obj, formatted_transition[3]])
+        elif src_state_obj is None:
+            Logger.set_warning(__name__,
+                               f'{formatted_transition[0]} is not displayed because it has an unknown source state')
+        else:
+            Logger.set_warning(__name__,
+                               f'{formatted_transition[0]} is not displayed because it has unknown destination state')
+
+    return objects_conditions_list
+
+
+def write_state(state_obj_string, state, new):
+    """@ingroup plantuml_adapter
+    Returns simple state string for PlantUml text
+    @param[in, out] state_obj_string TBD
+    @param[in] state TBD
+    @param[in] new TBD
+    @return None
+    """
+
+    if not state.parent and not state.child_list:
+        state_obj_string.create_state(state)
+        new.append(state.id)
+
+
+def write_composed_state(state_obj_string, state, new, count=0):
+    """@ingroup plantuml_adapter
+    Returns composed state string for PlantUml text
+    @param[in, out] state_obj_string TBD
+    @param[in] state TBD
+    @param[in] new TBD
+    @param[in] count TBD
+    @return None
+    """
+    state_obj_string.create_state(state, parent=True)
+    new.insert(count, state.id)
+    count += 1
+    for state_child in state.child_list:
+        if not state_child.child_list:
+            state_obj_string.create_state(state_child)
+            new.insert(count + 1, state_child.id)
+        else:
+            write_composed_state(state_obj_string, state_child, new, count)
+
+    state_obj_string.append_string("}\n" * count)
+
+
+def write_transition(state_obj_string, state, objects_conditions_list):
+    """@ingroup plantuml_adapter
+    Returns simple transition string for PlantUml text
+    @param[in, out] state_obj_string TBD
+    @param[in] state TBD
+    @param[in] new TBD
+    @param[in, out] objects_conditions_list TBD
+    @return None
+    """
+    for object_conditions in objects_conditions_list.copy():
+        if object_conditions[0].id == state.id:
+            state_obj_string.create_transition([object_conditions])
+            objects_conditions_list.remove(object_conditions)
```

### Comparing `jarvis4se-1.3.5/src/plantuml_adapter/util.py` & `jarvis4se-1.4.0/src/plantuml_adapter/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,512 +1,538 @@
-"""@defgroup plantuml_adapter
-Plantuml adapter module
-"""
-# Libraries
-import os
-import re
-import inspect
-import pathlib
-import subprocess
-
-from urllib.request import urlopen
-from urllib.error import URLError, HTTPError
-from plantuml import PlantUML
-
-# Modules
-import datamodel
-from tools import Logger
-
-
-class PlantUmlPicoServer:
-    """@ingroup plantuml_adapter
-    @anchor PlantUmlPicoServer
-    Class that looks for .jar file in root, check version and handle local PlantUml PicoWeb
-    Server (https://plantuml.com/en/picoweb)
-
-    If . jar, get it, check if PicoWeb is running, if not start new process else default url
-    to online PlantUml server
-    """
-    def __init__(self):
-        """
-        @var plantuml_jar_path
-        Filepath to the PlantUml jar
-
-        @var url
-        URL for the local PlantUml PicoWeb Server
-
-        @var version_cmd
-        JAVA command to retrieve the PlantUml jar file version
-        """
-
-        self.plantuml_jar_path = None
-
-        jar_file = self.get_jar()
-        if not jar_file:
-            self.url = 'http://www.plantuml.com/plantuml/svg/'
-        else:
-            self.plantuml_jar_path = str(pathlib.Path(f'./{jar_file}'))
-            self.version_cmd = ['java', '-jar', self.plantuml_jar_path, '-version']
-            pico_cmd = ['java', '-DPLANTUML_LIMIT_SIZE=20000', '-jar', self.plantuml_jar_path,
-                        '-picoweb']
-
-            self.check_version()
-            # Default localhost pico server
-            self.url = "http://127.0.0.1:8080/plantuml/svg/"
-            # Check if pico is running
-            check_pico = False
-            try:
-                with urlopen(f"{self.url}"):
-                    pass
-            except HTTPError:
-                pass
-            except URLError:
-                pass
-            else:
-                check_pico = True
-
-            if not check_pico:
-                self.process = subprocess.Popen(pico_cmd)
-
-    @classmethod
-    def get_jar(cls):
-        """Return first jar filepath with 'plantuml' in filename
-
-        @return jar filepath
-        """
-
-        end_message = ", large diagrams will not be displayed.\n" \
-                      "See: " \
-                      "https://github.com/rcasteran/jarvis4se/blob/main/docs/installation.md"
-
-        list_dir = os.listdir('.')
-        if not any('.jar' in f for f in list_dir):
-            Logger.set_warning(__name__,
-                              f"Not any .jar found for plantuml in root{end_message}")
-            return None
-
-        jar_list = [f.string for f in [re.search("plantuml.*jar", i) for i in list_dir] if f]
-        if not jar_list:
-            Logger.set_warning(__name__,
-                              f"Not any .jar found with 'plantuml' in its name{end_message}")
-            return None
-
-        # Return first filename with plantuml in it
-        return jar_list.pop(0)
-
-    def check_version(self):
-        """ Get .jar version and check with latest release
-
-        @return None
-        """
-
-        jar_version = subprocess.run(
-            self.version_cmd, capture_output=True, encoding="utf-8").stdout[17:26].strip()
-        github_url = "https://github.com/plantuml/plantuml/releases/latest"
-
-        try:
-            with urlopen(f"{github_url}") as rep:
-                release_ver = str(rep.geturl())[51:]
-
-            if int(release_ver[0]) > int(jar_version[0]) or \
-                    int(release_ver[2:6]) > int(jar_version[2:6]) or \
-                    int(release_ver[7:len(release_ver)]) > int(jar_version[7:len(jar_version)]):
-                Logger.set_info(__name__,
-                           f"plantUml.jar is not up-to-date, see latest release {github_url}")
-        except:
-            Logger.set_info(__name__,
-                           "Not able to check plantuml.jar version.")
-
-
-class PlantUmlGen(PlantUmlPicoServer):
-    """@ingroup plantuml_adapter
-    @anchor PlantUmlGen
-    Class to encode PlantUml text and get server url as .svg
-    """
-    def __init__(self):
-        """
-        @var server
-        PlantUml server
-        """
-
-        # Init PicoWeb server from PlantUMLPicoServer
-        # If .jar found or default online PlantUml, send it to PlantUml for encoding and HTTP handling
-        super().__init__()
-        # PlantUml has encoding and handling errors
-        self.server = PlantUML(url=self.url,
-                               basic_auth={},
-                               form_auth={}, http_opts={}, request_opts={})
-
-    def get_diagram_url(self, string, from_diagram_cell=False):
-        """ Generate .svg from PlantUml text using PlantUml default server or PlantUml .jar PicoWeb
-        @param[in] string PlantUml text
-        @param[in] from_diagram_cell indicates if PlantUml text is coming from a notebook diagram cell
-        (TRUE) or not (FALSE)
-        @return diagram url
-        """
-        if not from_diagram_cell:
-            full_string = "@startuml\nskin rose\nskinparam NoteBackgroundColor PapayaWhip\n" \
-                          + string + "@enduml"
-        else:
-            full_string = string
-
-        if len(string) > 15000 and self.plantuml_jar_path is None:
-            Logger.set_warning(__name__,
-                              f"Diagram is too large to be display with PlantUml Online Server, "
-                              f"please consider download .jar at https://plantuml.com/fr/download")
-            return None
-
-        return self.server.get_url(full_string)
-
-
-class StateDiagram:
-    """@ingroup plantuml_adapter
-    @anchor StateDiagram
-    Class to encode PlantUml text for state diagram
-    """
-
-    def __init__(self):
-        """
-        @var string
-        PlantUml text
-        """
-
-        # Initialize PlantUml text
-        self.string = inspect.cleandoc("""skinparam useBetaStyle true
-                                            hide empty description
-                                            <style>
-                                                 .Entry{
-                                                    FontColor white
-                                                    BackgroundColor black
-                                                 }
-                                                 .Exit{
-                                                    FontColor white
-                                                    BackgroundColor black
-                                                 }
-                                            </style>""") + "\n"
-
-    def append_string(self, *string_list):
-        """Append *string_list to PlantUml text
-        @param[in] *string_list string list
-        @return None
-        """
-        self.string = "".join([self.string, *string_list])
-
-    def create_state(self, state, parent=False):
-        """Update the PlantUml text for a state
-        @param[in] state state element
-        @param[in] parent indicates if the state is a parent (TRUE) or not (FALSE)
-        @return None
-        """
-        if parent:
-            open_bracket_str = ' {'
-        else:
-            open_bracket_str = ''
-        if state.alias:
-            state_alias = state.alias
-        else:
-            state_alias = state.name.lower().replace(" ", "_").replace("-", "")
-
-        if isinstance(state.type, datamodel.BaseType):
-            state_type_str = str(state.type).capitalize().replace("_", " ")
-        elif 'EXIT' in state.type.name:
-            state_type_str = 'EXIT'
-        elif 'ENTRY' in state.type.name:
-            state_type_str = 'ENTRY'
-        else:
-            state_type_str = state.type.name
-        self.append_string("'id: ", state.id, '\nstate "', state.name, '"', ' as ', state_alias,
-                           ' <<', state_type_str, '>>', open_bracket_str, '\n')
-
-    def create_transition(self, transition_list):
-        """Update the PlantUml text for a list of transitions
-        @param[in] transition_list list of transitions
-        @return None
-        """
-        for transition in transition_list:
-            if transition[0].alias:
-                source_alias = transition[0].alias
-            else:
-                source_alias = transition[0].name.lower().replace(" ", "_").replace("-", "")
-
-            if transition[1].alias:
-                destination_alias = transition[1].alias
-            else:
-                destination_alias = transition[1].name.lower().replace(" ", "_").replace("-", "")
-
-            self.append_string(str(source_alias), " --> ", str(destination_alias), " : ")
-            conditions_str = ""
-            last = len(transition[2]) - 1
-            if not transition[2]:
-                conditions_str += "No Condition Yet\n"
-            else:
-                for idx, trans in enumerate(transition[2]):
-                    condition = trans.strip("{''}")
-                    if idx < last:
-                        conditions_str += condition + ' \\n '
-                        idx += 1
-                    elif idx == last:
-                        conditions_str += condition + "\n"
-            self.string += conditions_str
-
-
-class SequenceDiagram:
-    """@ingroup plantuml_adapter
-    @anchor SequenceDiagram
-    Class to encode PlantUml text for sequence diagram
-    """
-
-    def __init__(self):
-        """
-        @var string
-        PlantUml text
-        """
-
-        # Allow plantuml option to put duration between 2 messages (not used yet)
-        self.string = "!pragma teoz true\n"
-
-    def append_string(self, *string_list):
-        """Append *string_list to PlantUml text
-        @param[in] *string_list string list
-        @return None
-        """
-        self.string = "".join([self.string, *string_list])
-
-    def create_sequence_message(self, message_list):
-        """Update the PlantUml text for a list of message
-        @param[in] message_list message list
-        @return None
-        """
-        activate_list = []
-        deactivate_list = []
-        for idx, val in enumerate(message_list):
-            for i in range(2):
-                if val[i] not in activate_list:
-                    activate_list.append(val[i])
-                    self.append_string("activate ", val[i].replace(" ", "_").replace("-", ""), "\n")
-
-            relationship_str = val[0].replace(" ", "_").replace("-", "") + ' -> ' \
-                               + val[1].replace(" ", "_").replace("-", "")
-            if val[3]:
-                seq_number = str(idx + 1) + "- "
-            else:
-                seq_number = ""
-            self.append_string(relationship_str, ' : ', seq_number + val[2], '\n')
-            for i in range(2):
-                if val[i] in activate_list and \
-                        not any(val[i] in sub for sub in message_list[idx + 1:]):
-                    deactivate_list.append(val[i])
-                    self.append_string("deactivate ", val[i].replace(" ", "_").replace("-", ""),
-                                       "\n")
-
-    def create_participant(self, function):
-        """Update the PlantUml text for a function
-        @param[in] function function
-        @return None
-        """
-        # If the string is not formatted like this, plantuml raises error
-        function_name = function.name.lower().replace(" ", "_").replace("-", "")
-        if isinstance(function.type, datamodel.BaseType):
-            function_type_str = str(function.type).capitalize().replace("_", " ")
-        else:
-            function_type_str = function.type.name
-        self.append_string("participant ", function_name, ' <<', function_type_str, '>>', "\n")
-
-
-class ObjDiagram:
-    """@ingroup plantuml_adapter
-    @anchor ObjDiagram
-    Class to encode PlantUml text for object diagram
-    """
-
-    def __init__(self):
-        """
-        @var string
-        PlantUml text
-        """
-
-        self.string = ""
-
-    def append_string(self, *string_list):
-        """Append *string_list to PlantUml text
-        @param[in] *string_list string list
-        @return None
-        """
-        self.string = "".join([self.string, *string_list])
-
-    def create_object(self, function, attribute_list):
-        """Update the PlantUml text for a function
-        @param[in] function function
-        @param[in] attribute_list function attribute list
-        @return None
-        """
-
-        # If the string is not formatted like this, plantuml raises error
-        operand_str = ''
-        function_name = function.name.lower().replace(" ", "_").replace("-", "")
-        if isinstance(function.type, datamodel.BaseType):
-            function_type_str = str(function.type).capitalize().replace("_", " ")
-        else:
-            function_type_str = function.type.name
-        self.append_string(
-            "'id: ", str(function.id), '\nobject "', function.name, '" as ', function_name,
-            ' <<', function_type_str, '>>')
-
-        if function.operand:
-            operand_str = str(function.operand) + ' : ' + str(function.input_role) + '\n'
-        attribute_str = self.create_object_attributes(function, attribute_list)
-
-        if len(attribute_str) > 1 or len(operand_str) > 1:
-            self.append_string(" {\n", operand_str, attribute_str, "}\n")
-        else:
-            self.append_string("\n")
-
-    def create_component_attribute(self, component, attribute_list):
-        """Update the PlantUml text for a component attribute list
-        @param[in] component component
-        @param[in] attribute_list component attribute list
-        @return None
-        """
-        attribute_str = self.create_object_attributes(component, attribute_list)
-        if attribute_str:
-            component_name = component.name.lower().replace(" ", "_").replace("-", "")
-            self.append_string('note bottom of ', component_name, '\n', attribute_str, 'end note\n')
-
-    def create_port(self, flow_list, flow_direction):
-        """Update the PlantUml text for a port (circle)
-        @param[in] flow_list flow list
-        @param[in] flow_direction flow direction
-        @return None
-        """
-        for i in flow_list:
-            end = ""
-            if flow_direction == "in":
-                end = '_i\n'
-            elif flow_direction == "out":
-                end = '_o\n'
-            elif flow_direction == "None":
-                end = '\n'
-            self.append_string('circle ', i[0][1].replace(" ", "_").replace("-", ""), end)
-
-    def create_component(self, component):
-        """Update the PlantUml text for a component
-        @param[in] component component
-        @return None
-        """
-
-        # If the string is not formatted like this, plantuml raises error
-        component_name = component.name.lower().replace(" ", "_").replace("-", "")
-        if isinstance(component.type, datamodel.BaseType):
-            component_type_str = str(component.type).capitalize().replace("_", " ")
-        else:
-            component_type_str = component.type.name
-        self.append_string("'id: ", component.id, '\ncomponent "', component.name, '" ', 'as ',
-                           component_name, ' <<', component_type_str, '>>{\n')
-
-    def create_output_flow(self, output_flow_list):
-        """Update the PlantUml text for output flows list
-        @param[in] output_flow_list output flows list
-        @return None
-        """
-        output_flow_str = ""
-        for i in output_flow_list:
-            name = i[0][1].replace(" ", "_").replace("-", "")
-            middle_arrow = ''
-            if i[0][0] is not None:
-                middle_arrow = ' #--> '
-            if i[0][0] is None:
-                middle_arrow = ' --> '
-            relationship_str = name + middle_arrow + name + '_o '
-            if len(i[1]) > 1:
-                self.string += self.create_multiple_arrow(relationship_str, output_flow_str, i)
-            else:
-                self.append_string(relationship_str, ' : ', i[1][0], '\n')
-
-    def create_input_flow(self, input_flow_list):
-        """Update the PlantUml text for input flows list
-        @param[in] input_flow_list input flows list
-        @return None
-        """
-        input_flow_str = ""
-        for i in input_flow_list:
-            relationship_str = "".join([i[0][1].replace(" ", "_").replace("-", ""), '_i', ' --> ',
-                                        i[0][1].replace(" ", "_").replace("-", "")])
-            if len(i[1]) > 1:
-                self.string += self.create_multiple_arrow(relationship_str, input_flow_str, i)
-            else:
-                self.append_string(relationship_str, ' : ', i[1][0], '\n')
-
-    def create_data_flow(self, data_flow_list):
-        """Update the PlantUml text for data flows list
-        @param[in] data_flow_list data flows list
-        @return None
-        """
-        flow_str = ""
-        for i in data_flow_list:
-            relationship_str = "".join([i[0][0].replace(" ", "_").replace("-", ""), ' #--> ',
-                                        i[0][1].replace(" ", "_").replace("-", "")])
-            if len(i[1]) > 1:
-                self.string += self.create_multiple_arrow(relationship_str, flow_str, i)
-            else:
-                self.append_string(relationship_str, ' : ', i[1][0], '\n')
-
-    def create_interface(self, interface_list):
-        """Update the PlantUml text for interface list
-        @param[in] interface_list interface list
-        @return None
-        """
-        for i in interface_list:
-            relationship_str = ""
-            if i[0] and i[1]:
-                relationship_str = i[0].name.lower().replace(" ", "_").replace("-", "") + ' -- ' \
-                                   + i[1].name.lower().replace(" ", "_").replace("-", "")
-            elif not i[0] and i[1]:
-                circle_name = i[1].name.lower().replace(" ", "_").replace("-", "") + '_o'
-                relationship_str = 'circle ' + circle_name + '\n'
-                relationship_str += i[1].name.lower().replace(" ", "_").replace("-", "") \
-                                    + ' -- ' + circle_name
-            elif i[0] and not i[1]:
-                circle_name = i[0].name.lower().replace(" ", "_").replace("-", "") + '_o'
-                relationship_str = 'circle ' + circle_name + '\n'
-                relationship_str += circle_name + ' -- ' +\
-                                    i[0].name.lower().replace(" ", "_").replace("-", "")
-
-            self.append_string(relationship_str, ' : ',
-                               i[2].name.lower().replace(" ", "_").replace("-", ""), '\n')
-
-    @classmethod
-    def create_object_attributes(cls, wanted_object, attribute_list):
-        """Update the PlantUml text for object attribute list
-        @param[in] wanted_object object
-        @param[in] attribute_list object attribute list
-        @return None
-        """
-        attribute_str = ''
-        if attribute_list:
-            for attribute in attribute_list:
-                for described_item in attribute.described_item_list:
-                    if described_item[0] == wanted_object.id:
-                        attribute_str += attribute.name + " = " + described_item[1] + "\n"
-        return attribute_str
-
-    @classmethod
-    def create_multiple_arrow(cls, relationship_str, flow_str, flow_list):
-        """Create multiples arrow, to split data names across for visualization improvements"""
-        extended_flow_list = []
-        new_prod_cons_flow_list = []
-        producer_consumer_name = (flow_list[0][0], flow_list[0][1])
-        flow_list = flow_list[1]
-        flow_str += relationship_str + ' : ' + flow_list[0]
-        count = 0
-        for k, p in enumerate(flow_list):
-            if k < len(flow_list) and k - 1 >= 0:
-                count += len(p)
-                if count < 350:
-                    flow_str += '\\n' + flow_list[k]
-                else:
-                    extended_flow_list.append(p)
-        flow_str += '\n'
-        if len(extended_flow_list) > 0:
-            rest = producer_consumer_name, extended_flow_list
-            new_prod_cons_flow_list += rest
-            return cls.create_multiple_arrow(relationship_str, flow_str, new_prod_cons_flow_list)
-        return flow_str
+"""@defgroup plantuml_adapter
+Plantuml adapter module
+"""
+# Libraries
+import os
+import re
+import inspect
+import pathlib
+import subprocess
+
+from urllib.request import urlopen
+from urllib.error import URLError, HTTPError
+from plantuml import PlantUML
+
+# Modules
+import datamodel
+from tools import Logger
+
+
+class PlantUmlPicoServer:
+    """@ingroup plantuml_adapter
+    @anchor PlantUmlPicoServer
+    Class that looks for .jar file in root, check version and handle local PlantUml PicoWeb
+    Server (https://plantuml.com/en/picoweb)
+
+    If . jar, get it, check if PicoWeb is running, if not start new process else default url
+    to online PlantUml server
+    """
+    def __init__(self):
+        """
+        @var plantuml_jar_path
+        Filepath to the PlantUml jar
+
+        @var url
+        URL for the local PlantUml PicoWeb Server
+
+        @var version_cmd
+        JAVA command to retrieve the PlantUml jar file version
+        """
+
+        self.plantuml_jar_path = None
+
+        jar_file = self.get_jar()
+        if not jar_file:
+            self.url = 'http://www.plantuml.com/plantuml/svg/'
+        else:
+            self.plantuml_jar_path = str(pathlib.Path(f'./{jar_file}'))
+            self.version_cmd = ['java', '-jar', self.plantuml_jar_path, '-version']
+            pico_cmd = ['java', '-DPLANTUML_LIMIT_SIZE=20000', '-jar', self.plantuml_jar_path,
+                        '-picoweb']
+
+            self.check_version()
+            # Default localhost pico server
+            self.url = "http://127.0.0.1:8080/plantuml/svg/"
+            # Check if pico is running
+            check_pico = False
+            try:
+                with urlopen(f"{self.url}"):
+                    pass
+            except HTTPError:
+                pass
+            except URLError:
+                pass
+            else:
+                check_pico = True
+
+            if not check_pico:
+                self.process = subprocess.Popen(pico_cmd)
+
+    @classmethod
+    def get_jar(cls):
+        """Return first jar filepath with 'plantuml' in filename
+
+        @return jar filepath
+        """
+
+        end_message = ", large diagrams will not be displayed.\n" \
+                      "See: " \
+                      "https://github.com/rcasteran/jarvis4se/blob/main/docs/installation.md"
+
+        list_dir = os.listdir('.')
+        if not any('.jar' in f for f in list_dir):
+            Logger.set_warning(__name__,
+                              f"Not any .jar found for plantuml in root{end_message}")
+            return None
+
+        jar_list = [f.string for f in [re.search("plantuml.*jar", i) for i in list_dir] if f]
+        if not jar_list:
+            Logger.set_warning(__name__,
+                              f"Not any .jar found with 'plantuml' in its name{end_message}")
+            return None
+
+        # Return first filename with plantuml in it
+        return jar_list.pop(0)
+
+    def check_version(self):
+        """ Get .jar version and check with latest release
+
+        @return None
+        """
+
+        jar_version = subprocess.run(
+            self.version_cmd, capture_output=True, encoding="utf-8").stdout[17:26].strip()
+        github_url = "https://github.com/plantuml/plantuml/releases/latest"
+
+        try:
+            with urlopen(f"{github_url}") as rep:
+                release_ver = str(rep.geturl())[51:]
+
+            if int(release_ver[0]) > int(jar_version[0]) or \
+                    int(release_ver[2:6]) > int(jar_version[2:6]) or \
+                    int(release_ver[7:len(release_ver)]) > int(jar_version[7:len(jar_version)]):
+                Logger.set_info(__name__,
+                           f"plantUml.jar is not up-to-date, see latest release {github_url}")
+        except:
+            Logger.set_info(__name__,
+                           "Not able to check plantuml.jar version.")
+
+
+class PlantUmlGen(PlantUmlPicoServer):
+    """@ingroup plantuml_adapter
+    @anchor PlantUmlGen
+    Class to encode PlantUml text and get server url as .svg
+    """
+    def __init__(self):
+        """
+        @var server
+        PlantUml server
+        """
+
+        # Init PicoWeb server from PlantUMLPicoServer
+        # If .jar found or default online PlantUml, send it to PlantUml for encoding and HTTP handling
+        super().__init__()
+        # PlantUml has encoding and handling errors
+        self.server = PlantUML(url=self.url,
+                               basic_auth={},
+                               form_auth={}, http_opts={}, request_opts={})
+
+    def get_diagram_url(self, string, from_diagram_cell=False):
+        """ Generate .svg from PlantUml text using PlantUml default server or PlantUml .jar PicoWeb
+        @param[in] string PlantUml text
+        @param[in] from_diagram_cell indicates if PlantUml text is coming from a notebook diagram cell
+        (TRUE) or not (FALSE)
+        @return diagram url
+        """
+        if not from_diagram_cell:
+            full_string = "@startuml\nskin rose\nskinparam NoteBackgroundColor PapayaWhip\n" \
+                          + string + "@enduml"
+        else:
+            full_string = string
+
+        if len(string) > 15000 and self.plantuml_jar_path is None:
+            Logger.set_warning(__name__,
+                              f"Diagram is too large to be display with PlantUml Online Server, "
+                              f"please consider download .jar at https://plantuml.com/fr/download")
+            return None
+
+        return self.server.get_url(full_string)
+
+
+class StateDiagram:
+    """@ingroup plantuml_adapter
+    @anchor StateDiagram
+    Class to encode PlantUml text for state diagram
+    """
+
+    def __init__(self):
+        """
+        @var string
+        PlantUml text
+        """
+
+        # Initialize PlantUml text
+        self.string = inspect.cleandoc("""skinparam useBetaStyle true
+                                            hide empty description
+                                            <style>
+                                                 .Entry{
+                                                    FontColor white
+                                                    BackgroundColor black
+                                                 }
+                                                 .Exit{
+                                                    FontColor white
+                                                    BackgroundColor black
+                                                 }
+                                            </style>""") + "\n"
+
+    def append_string(self, *string_list):
+        """Append *string_list to PlantUml text
+        @param[in] *string_list string list
+        @return None
+        """
+        self.string = "".join([self.string, *string_list])
+
+    def create_state(self, state, parent=False):
+        """Update the PlantUml text for a state
+        @param[in] state state element
+        @param[in] parent indicates if the state is a parent (TRUE) or not (FALSE)
+        @return None
+        """
+        if parent:
+            open_bracket_str = ' {'
+        else:
+            open_bracket_str = ''
+        if state.alias:
+            state_alias = state.alias
+        else:
+            state_alias = state.name.lower().replace(" ", "_").replace("-", "")
+
+        if isinstance(state.type, datamodel.BaseType):
+            state_type_str = str(state.type).capitalize().replace("_", " ")
+        elif datamodel.ExitStateLabel in state.type.name.lower():
+            state_type_str = 'EXIT'
+        elif datamodel.EntryStateLabel in state.type.name.lower():
+            state_type_str = 'ENTRY'
+        else:
+            state_type_str = state.type.name
+        self.append_string("'id: ", state.id, '\nstate "', state.name, '"', ' as ', state_alias,
+                           ' <<', state_type_str, '>>', open_bracket_str, '\n')
+
+    def create_transition(self, transition_list):
+        """Update the PlantUml text for a list of transitions
+        @param[in] transition_list list of transitions
+        @return None
+        """
+        for transition in transition_list:
+            if transition[0].alias:
+                source_alias = transition[0].alias
+            else:
+                source_alias = transition[0].name.lower().replace(" ", "_").replace("-", "")
+
+            if transition[1].alias:
+                destination_alias = transition[1].alias
+            else:
+                destination_alias = transition[1].name.lower().replace(" ", "_").replace("-", "")
+
+            self.append_string(str(source_alias), " --> ", str(destination_alias), " : ")
+            conditions_str = ""
+            last = len(transition[2]) - 1
+            if not transition[2]:
+                conditions_str += "No Condition Yet\n"
+            else:
+                for idx, trans in enumerate(transition[2]):
+                    condition = trans.strip("{''}")
+                    if idx < last:
+                        conditions_str += condition + ' \\n '
+                        idx += 1
+                    elif idx == last:
+                        conditions_str += condition + "\n"
+            self.string += conditions_str
+
+
+class SequenceDiagram:
+    """@ingroup plantuml_adapter
+    @anchor SequenceDiagram
+    Class to encode PlantUml text for sequence diagram
+    """
+
+    def __init__(self):
+        """
+        @var string
+        PlantUml text
+        """
+
+        # Allow plantuml option to put duration between 2 messages (not used yet)
+        self.string = "!pragma teoz true\n"
+
+    def append_string(self, *string_list):
+        """Append *string_list to PlantUml text
+        @param[in] *string_list string list
+        @return None
+        """
+        self.string = "".join([self.string, *string_list])
+
+    def create_sequence_message(self, message_list):
+        """Update the PlantUml text for a list of message
+        @param[in] message_list message list
+        @return None
+        """
+        activate_list = []
+        deactivate_list = []
+        for idx, val in enumerate(message_list):
+            for i in range(2):
+                if val[i] not in activate_list:
+                    activate_list.append(val[i])
+                    self.append_string("activate ", val[i].replace(" ", "_").replace("-", ""), "\n")
+
+            relationship_str = val[0].replace(" ", "_").replace("-", "") + ' -> ' \
+                               + val[1].replace(" ", "_").replace("-", "")
+            if val[3]:
+                seq_number = str(idx + 1) + "- "
+            else:
+                seq_number = ""
+            self.append_string(relationship_str, ' : ', seq_number + val[2], '\n')
+            for i in range(2):
+                if val[i] in activate_list and \
+                        not any(val[i] in sub for sub in message_list[idx + 1:]):
+                    deactivate_list.append(val[i])
+                    self.append_string("deactivate ", val[i].replace(" ", "_").replace("-", ""),
+                                       "\n")
+
+    def create_participant(self, function):
+        """Update the PlantUml text for a function
+        @param[in] function function
+        @return None
+        """
+        # If the string is not formatted like this, plantuml raises error
+        function_name = function.name.lower().replace(" ", "_").replace("-", "")
+        if isinstance(function.type, datamodel.BaseType):
+            function_type_str = str(function.type).capitalize().replace("_", " ")
+        else:
+            function_type_str = function.type.name
+        self.append_string("participant ", function_name, ' <<', function_type_str, '>>', "\n")
+
+
+class ObjDiagram:
+    """@ingroup plantuml_adapter
+    @anchor ObjDiagram
+    Class to encode PlantUml text for object diagram
+    """
+
+    def __init__(self):
+        """
+        @var string
+        PlantUml text
+        """
+
+        self.string = ""
+
+    def append_string(self, *string_list):
+        """Append *string_list to PlantUml text
+        @param[in] *string_list string list
+        @return None
+        """
+        self.string = "".join([self.string, *string_list])
+
+    def create_object(self, function, attribute_list):
+        """Update the PlantUml text for a function
+        @param[in] function function
+        @param[in] attribute_list function attribute list
+        @return None
+        """
+
+        # If the string is not formatted like this, plantuml raises error
+        operand_str = ''
+        function_name = function.name.lower().replace(" ", "_").replace("-", "")
+        if isinstance(function.type, datamodel.BaseType):
+            function_type_str = str(function.type).capitalize().replace("_", " ")
+        else:
+            function_type_str = function.type.name
+        self.append_string(
+            "'id: ", str(function.id), '\nobject "', function.name, '" as ', function_name,
+            ' <<', function_type_str, '>>')
+
+        if function.operand:
+            operand_str = str(function.operand) + ' : ' + str(function.input_role) + '\n'
+        attribute_str = self.create_object_attributes(function, attribute_list)
+
+        if len(attribute_str) > 1 or len(operand_str) > 1:
+            self.append_string(" {\n", operand_str, attribute_str, "}\n")
+        else:
+            self.append_string("\n")
+
+    def create_component_attribute(self, component, attribute_list):
+        """Update the PlantUml text for a component attribute list
+        @param[in] component component
+        @param[in] attribute_list component attribute list
+        @return None
+        """
+        attribute_str = self.create_object_attributes(component, attribute_list)
+        if attribute_str:
+            component_name = component.name.lower().replace(" ", "_").replace("-", "")
+            self.append_string('note bottom of ', component_name, '\n', attribute_str, 'end note\n')
+
+    def create_port(self, flow_list, flow_direction):
+        """Update the PlantUml text for a port (circle)
+        @param[in] flow_list flow list
+        @param[in] flow_direction flow direction
+        @return None
+        """
+        for i in flow_list:
+            end = ""
+            if flow_direction == "in":
+                end = '_i\n'
+            elif flow_direction == "out":
+                end = '_o\n'
+            elif flow_direction == "None":
+                end = '\n'
+            self.append_string('circle ', i[0][1].replace(" ", "_").replace("-", ""), end)
+
+    def create_component(self, component):
+        """Update the PlantUml text for a component
+        @param[in] component component
+        @return None
+        """
+
+        # If the string is not formatted like this, plantuml raises error
+        component_name = component.name.lower().replace(" ", "_").replace("-", "")
+        if isinstance(component.type, datamodel.BaseType):
+            component_type_str = str(component.type).capitalize().replace("_", " ")
+        else:
+            component_type_str = component.type.name
+        self.append_string("'id: ", component.id, '\ncomponent "', component.name, '" ', 'as ',
+                           component_name, ' <<', component_type_str, '>>{\n')
+
+    def create_output_flow(self, output_flow_list):
+        """Update the PlantUml text for output flows list
+        @param[in] output_flow_list output flows list
+        @return None
+        """
+        output_flow_str = ""
+        for i in output_flow_list:
+            if i[0][0] is not None:
+                middle_arrow = ' #--> '
+            else:
+                middle_arrow = ' --> '
+
+            is_digit = False
+            last_underscore_position = i[0][1].rfind('_')
+            if 0 < last_underscore_position < len(i[0][1])-1:
+                is_digit = i[0][1][last_underscore_position+1:].isdigit()
+            # Else do nothing
+
+            if is_digit:
+                name = i[0][1]
+                relationship_str = "".join([name.replace(" ", "_").replace("-", ""),
+                                            middle_arrow,
+                                            name[0:name.index('_')].replace(" ", "_").replace("-", ""),
+                                            '_o '])
+            else:
+                name = i[0][1].replace(" ", "_").replace("-", "")
+                relationship_str = "".join([name, middle_arrow, name, '_o '])
+            if len(i[1]) > 1:
+                self.string += self.create_multiple_arrow(relationship_str, output_flow_str, i)
+            else:
+                self.append_string(relationship_str, ' : ', i[1][0], '\n')
+
+    def create_input_flow(self, input_flow_list):
+        """Update the PlantUml text for input flows list
+        @param[in] input_flow_list input flows list
+        @return None
+        """
+        input_flow_str = ""
+        for i in input_flow_list:
+            is_digit = False
+            last_underscore_position = i[0][1].rfind('_')
+            if 0 < last_underscore_position < len(i[0][1])-1:
+                is_digit = i[0][1][last_underscore_position+1:].isdigit()
+            # Else do nothing
+
+            if is_digit:
+                name = i[0][1]
+                relationship_str = "".join([name[0:name.index('_')].replace(" ", "_").replace("-", ""),
+                                            '_i',
+                                            ' --> ',
+                                            name.replace(" ", "_").replace("-", "")])
+            else:
+                name = i[0][1].replace(" ", "_").replace("-", "")
+                relationship_str = "".join([name, '_i', ' --> ', name])
+            if len(i[1]) > 1:
+                self.string += self.create_multiple_arrow(relationship_str, input_flow_str, i)
+            else:
+                self.append_string(relationship_str, ' : ', i[1][0], '\n')
+
+    def create_data_flow(self, data_flow_list):
+        """Update the PlantUml text for data flows list
+        @param[in] data_flow_list data flows list
+        @return None
+        """
+        flow_str = ""
+        for i in data_flow_list:
+            relationship_str = "".join([i[0][0].replace(" ", "_").replace("-", ""), ' #--> ',
+                                        i[0][1].replace(" ", "_").replace("-", "")])
+            if len(i[1]) > 1:
+                self.string += self.create_multiple_arrow(relationship_str, flow_str, i)
+            else:
+                self.append_string(relationship_str, ' : ', i[1][0], '\n')
+
+    def create_interface(self, interface_list):
+        """Update the PlantUml text for interface list
+        @param[in] interface_list interface list
+        @return None
+        """
+        for i in interface_list:
+            relationship_str = ""
+            if i[0] and i[1]:
+                relationship_str = i[0].name.lower().replace(" ", "_").replace("-", "") + ' -- ' \
+                                   + i[1].name.lower().replace(" ", "_").replace("-", "")
+            elif not i[0] and i[1]:
+                circle_name = i[1].name.lower().replace(" ", "_").replace("-", "") + '_o'
+                relationship_str = 'circle ' + circle_name + '\n'
+                relationship_str += i[1].name.lower().replace(" ", "_").replace("-", "") \
+                                    + ' -- ' + circle_name
+            elif i[0] and not i[1]:
+                circle_name = i[0].name.lower().replace(" ", "_").replace("-", "") + '_o'
+                relationship_str = 'circle ' + circle_name + '\n'
+                relationship_str += circle_name + ' -- ' +\
+                                    i[0].name.lower().replace(" ", "_").replace("-", "")
+
+            self.append_string(relationship_str, ' : ',
+                               i[2].name.lower().replace(" ", "_").replace("-", ""), '\n')
+
+    @classmethod
+    def create_object_attributes(cls, wanted_object, attribute_list):
+        """Update the PlantUml text for object attribute list
+        @param[in] wanted_object object
+        @param[in] attribute_list object attribute list
+        @return None
+        """
+        attribute_str = ''
+        if attribute_list:
+            for attribute in attribute_list:
+                for described_item in attribute.described_item_list:
+                    if described_item[0] == wanted_object.id:
+                        attribute_str += attribute.name + " = " + described_item[1] + "\n"
+        return attribute_str
+
+    @classmethod
+    def create_multiple_arrow(cls, relationship_str, flow_str, flow_list):
+        """Create multiples arrow, to split data names across for visualization improvements"""
+        extended_flow_list = []
+        new_prod_cons_flow_list = []
+        producer_consumer_name = (flow_list[0][0], flow_list[0][1])
+        flow_list = flow_list[1]
+        flow_str += relationship_str + ' : ' + flow_list[0]
+        count = 0
+        for k, p in enumerate(flow_list):
+            if k < len(flow_list) and k - 1 >= 0:
+                count += len(p)
+                if count < 350:
+                    flow_str += '\\n' + flow_list[k]
+                else:
+                    extended_flow_list.append(p)
+        flow_str += '\n'
+        if len(extended_flow_list) > 0:
+            rest = producer_consumer_name, extended_flow_list
+            new_prod_cons_flow_list += rest
+            return cls.create_multiple_arrow(relationship_str, flow_str, new_prod_cons_flow_list)
+        return flow_str
```

### Comparing `jarvis4se-1.3.5/src/tools/config.py` & `jarvis4se-1.4.0/src/tools/config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-"""@defgroup tools
-Tooling module
-"""
-
-# Libraries
-import os
-
-
-# Modules
-
-
-class Config:
-    """@ingroup tools
-    @anchor Config
-    Jarvis configurator
-    """
-
-    is_log_file = False
-    is_diagram_file = False
-    verbose_level = 1
-
-    @classmethod
-    def read(cls):
-        """ Read the configuration file if any
-        @return None
-        """
-        try:
-            if os.path.isdir("config"):
-                with open("config/config.cfg", "r", encoding='utf-8') as file_reader:
-                    line = file_reader.readline()
-
-                    error = False
-                    while (line != '') & (not error):
-                        lines = line.split('=')
-                        if len(lines) > 1:
-                            if lines[0].strip() == 'log':
-                                if 'True' == lines[1].strip() or '1' == lines[1].strip():
-                                    cls.is_log_file = True
-                                    # Logger depends from Config. Thus simple print
-                                    print("Log file storage activated")
-                            elif lines[0].strip() == 'diagram':
-                                if 'True' == lines[1].strip() or '1' == lines[1].strip():
-                                    cls.is_diagram_file = True
-                                    # Logger depends from Config. Thus simple print
-                                    print("Diagram file storage activated")
-                            elif lines[0].strip() == 'verbose':
-                                if lines[1].strip().isnumeric():
-                                    cls.verbose_level = int(lines[1].strip())
-                                    # Logger depends from Config. Thus simple print
-                                    if cls.verbose_level == 0:
-                                        print(f"ERROR and WARNING messages display activated")
-                                    elif cls.verbose_level == 1:
-                                        print(f"ERROR, WARNING and INFO messages display activated")
-                                    else:
-                                        print(f"ERROR, WARNING, INFO and DEBUG messages display activated")
-                                else:
-                                    error = True
-                            else:
-                                error = True
-                        else:
-                            error = True
-                        line = file_reader.readline()
-
-                    if error:
-                        # Logger depends from Config. Thus simple print
-                        print("[ERROR] Configuration file is not correctly formatted")
-            else:
-                # Logger depends from Config. Thus simple print
-                print(f"No configuration file detected in {os.getcwd()}\\config")
-        except EnvironmentError as ex:
-            # Logger depends from Config. Thus simple print
-            print(f"[ERROR] Unable to read the configuration file in {os.getcwd()}\\config: {ex}")
+"""@defgroup tools
+Tooling module
+"""
+
+# Libraries
+import os
+
+
+# Modules
+
+
+class Config:
+    """@ingroup tools
+    @anchor Config
+    Jarvis configurator
+    """
+
+    is_log_file = False
+    is_diagram_file = False
+    verbose_level = 1
+
+    @classmethod
+    def read(cls):
+        """ Read the configuration file if any
+        @return None
+        """
+        try:
+            if os.path.isdir("config"):
+                with open("config/config.cfg", "r", encoding='utf-8') as file_reader:
+                    line = file_reader.readline()
+
+                    error = False
+                    while (line != '') & (not error):
+                        lines = line.split('=')
+                        if len(lines) > 1:
+                            if lines[0].strip() == 'log':
+                                if 'True' == lines[1].strip() or '1' == lines[1].strip():
+                                    cls.is_log_file = True
+                                    # Logger depends from Config. Thus simple print
+                                    print("Log file storage activated")
+                            elif lines[0].strip() == 'diagram':
+                                if 'True' == lines[1].strip() or '1' == lines[1].strip():
+                                    cls.is_diagram_file = True
+                                    # Logger depends from Config. Thus simple print
+                                    print("Diagram file storage activated")
+                            elif lines[0].strip() == 'verbose':
+                                if lines[1].strip().isnumeric():
+                                    cls.verbose_level = int(lines[1].strip())
+                                    # Logger depends from Config. Thus simple print
+                                    if cls.verbose_level == 0:
+                                        print(f"ERROR and WARNING messages display activated")
+                                    elif cls.verbose_level == 1:
+                                        print(f"ERROR, WARNING and INFO messages display activated")
+                                    else:
+                                        print(f"ERROR, WARNING, INFO and DEBUG messages display activated")
+                                else:
+                                    error = True
+                            else:
+                                error = True
+                        else:
+                            error = True
+                        line = file_reader.readline()
+
+                    if error:
+                        # Logger depends from Config. Thus simple print
+                        print("[ERROR] Configuration file is not correctly formatted")
+            else:
+                # Logger depends from Config. Thus simple print
+                print(f"No configuration file detected in {os.getcwd()}\\config")
+        except EnvironmentError as ex:
+            # Logger depends from Config. Thus simple print
+            print(f"[ERROR] Unable to read the configuration file in {os.getcwd()}\\config: {ex}")
```

### Comparing `jarvis4se-1.3.5/src/tools/logger.py` & `jarvis4se-1.4.0/src/tools/logger.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-"""@defgroup tools
-Tooling module
-"""
-
-# Libraries
-from datetime import datetime
-import os
-
-
-# Modules
-from . import Config
-
-
-class Logger:
-    """@ingroup tools
-    @anchor Logger
-    Jarvis logger
-    """
-
-    @classmethod
-    def set_debug(cls, module_name, msg):
-        """Format DEBUG message
-
-        DEBUG message are displayed with verbosity level greater than or equal to 2
-        @param[in] module_name module name responsible for the message
-        @param[in] msg message to be formatted
-        @return None
-        """
-        if Config.verbose_level >= 2:
-            print("[DEBUG] " + msg)
-            if Config.is_log_file:
-                cls.write("DEBUG", module_name, msg)
-
-    @classmethod
-    def set_info(cls, module_name, msg):
-        """Format INFO message
-
-        INFO message are displayed with verbosity level greater than 1
-        @param[in] module_name module name responsible for the message
-        @param[in] msg message to be formatted
-        @return None
-        """
-        if Config.verbose_level >= 1:
-            print(msg)
-            if Config.is_log_file:
-                cls.write("INFO", module_name, msg)
-
-    @classmethod
-    def set_warning(cls, module_name, msg):
-        """Format WARNING message
-
-        WARNING message are always displayed (no verbosity level consideration)
-        @param[in] module_name module name responsible for the message
-        @param[in] msg message to be formatted
-        @return None
-        """
-        print("[WARNING] " + msg)
-        if Config.is_log_file:
-            cls.write("WARNING", module_name, msg)
-
-    @classmethod
-    def set_error(cls, module_name, msg):
-        """Format ERROR message
-
-        ERROR message are always displayed (no verbosity level consideration)
-        @param[in] module_name module name responsible for the message
-        @param[in] msg message to be formatted
-        @return None
-        """
-        print("[ERROR] " + msg)
-        if Config.is_log_file:
-            cls.write("ERROR", module_name, msg)
-
-    @classmethod
-    def write(cls, msg_type, module_name, msg):
-        """Write message in the log file
-        @param[in] msg_type message type
-        @param[in] module_name module name responsible for the message
-        @param[in] msg message to be written
-        @return None
-        """
-        try:
-            now = datetime.now()
-            date = now.strftime("%Y-%m-%d")
-            time = now.strftime("%H:%M:%S")
-
-            if not os.path.isdir("log"):
-                os.makedirs("log")
-
-            with open("log/log_" + date + ".log", "a+", newline='', encoding='utf-8') as file_writer:
-                file_writer.write(date + ";"
-                                  + time + ";"
-                                  + msg_type + ";"
-                                  + module_name + ";"
-                                  + msg + "\n")
-        except EnvironmentError as ex:
-            print(f"[ERROR] Unable to write log file in {os.getcwd()}\\log: {ex}")
+"""@defgroup tools
+Tooling module
+"""
+
+# Libraries
+from datetime import datetime
+import os
+
+
+# Modules
+from . import Config
+
+
+class Logger:
+    """@ingroup tools
+    @anchor Logger
+    Jarvis logger
+    """
+
+    @classmethod
+    def set_debug(cls, module_name, msg):
+        """Format DEBUG message
+
+        DEBUG message are displayed with verbosity level greater than or equal to 2
+        @param[in] module_name module name responsible for the message
+        @param[in] msg message to be formatted
+        @return None
+        """
+        if Config.verbose_level >= 2:
+            print("[DEBUG] " + msg)
+            if Config.is_log_file:
+                cls.write("DEBUG", module_name, msg)
+
+    @classmethod
+    def set_info(cls, module_name, msg):
+        """Format INFO message
+
+        INFO message are displayed with verbosity level greater than 1
+        @param[in] module_name module name responsible for the message
+        @param[in] msg message to be formatted
+        @return None
+        """
+        if Config.verbose_level >= 1:
+            print(msg)
+            if Config.is_log_file:
+                cls.write("INFO", module_name, msg)
+
+    @classmethod
+    def set_warning(cls, module_name, msg):
+        """Format WARNING message
+
+        WARNING message are always displayed (no verbosity level consideration)
+        @param[in] module_name module name responsible for the message
+        @param[in] msg message to be formatted
+        @return None
+        """
+        print("[WARNING] " + msg)
+        if Config.is_log_file:
+            cls.write("WARNING", module_name, msg)
+
+    @classmethod
+    def set_error(cls, module_name, msg):
+        """Format ERROR message
+
+        ERROR message are always displayed (no verbosity level consideration)
+        @param[in] module_name module name responsible for the message
+        @param[in] msg message to be formatted
+        @return None
+        """
+        print("[ERROR] " + msg)
+        if Config.is_log_file:
+            cls.write("ERROR", module_name, msg)
+
+    @classmethod
+    def write(cls, msg_type, module_name, msg):
+        """Write message in the log file
+        @param[in] msg_type message type
+        @param[in] module_name module name responsible for the message
+        @param[in] msg message to be written
+        @return None
+        """
+        try:
+            now = datetime.now()
+            date = now.strftime("%Y-%m-%d")
+            time = now.strftime("%H:%M:%S")
+
+            if not os.path.isdir("log"):
+                os.makedirs("log")
+
+            with open("log/log_" + date + ".log", "a+", newline='', encoding='utf-8') as file_writer:
+                file_writer.write(date + ";"
+                                  + time + ";"
+                                  + msg_type + ";"
+                                  + module_name + ";"
+                                  + msg + "\n")
+        except EnvironmentError as ex:
+            print(f"[ERROR] Unable to write log file in {os.getcwd()}\\log: {ex}")
```

### Comparing `jarvis4se-1.3.5/src/tools/magic_tools.py` & `jarvis4se-1.4.0/src/tools/magic_tools.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-"""@defgroup tools
-Tooling module
-"""
-
-# Libraries
-from sys import version as py_ver
-from importlib.metadata import version
-from IPython.core.magic import (Magics, magics_class, cell_magic, line_magic)
-from IPython.display import display, HTML, Markdown
-
-# Modules
-from .util import get_hyperlink
-
-
-@magics_class
-class MagicTools(Magics):
-    """@ingroup tools
-    @anchor MagicTools
-    Magic call for IPython interface
-    """
-
-    def __init__(self, shell, generator):
-        """
-        @var generator
-        Jarvis diagram generator
-        """
-
-        # You must call the parent constructor
-        super().__init__(shell)
-        self.generator = generator
-
-    @staticmethod
-    @line_magic
-    def retrieve_pkg_version(_):
-        """Magic line that get Jarvis dependencies versions
-        @return None
-        """
-        pkg = ['ipython', 'lxml', 'notebook', 'plantuml', 'jarvis4se', 'pandas', 'requests']
-        pkg_ver =  "\n".join(['=='.join(tups) for tups in zip(pkg, map(version, pkg))])
-        print(pkg_ver, "\npython=={}".format(py_ver[:6]))
-
-    @cell_magic
-    def diagram(self, _, cell):
-        """Magic cell that allows to call directly Jarvis diagram generator
-        @param[in] cell cell instance
-        @param[in] _ not used
-        @return None
-        """
-        out = self.generator.get_diagram_url(cell, True)
-        if out:
-            hyper = get_hyperlink(out)
-            display(HTML(hyper))
-            # Single display (not related to logging)
-            print("Overview :")
-            display(Markdown(f'![figure]({out})'))
+"""@defgroup tools
+Tooling module
+"""
+
+# Libraries
+from sys import version as py_ver
+from importlib.metadata import version
+from IPython.core.magic import (Magics, magics_class, cell_magic, line_magic)
+from IPython.display import display, HTML, Markdown
+
+# Modules
+from .util import get_hyperlink
+
+
+@magics_class
+class MagicTools(Magics):
+    """@ingroup tools
+    @anchor MagicTools
+    Magic call for IPython interface
+    """
+
+    def __init__(self, shell, generator):
+        """
+        @var generator
+        Jarvis diagram generator
+        """
+
+        # You must call the parent constructor
+        super().__init__(shell)
+        self.generator = generator
+
+    @staticmethod
+    @line_magic
+    def retrieve_pkg_version(_):
+        """Magic line that get Jarvis dependencies versions
+        @return None
+        """
+        pkg = ['ipython', 'lxml', 'notebook', 'plantuml', 'jarvis4se', 'pandas', 'requests']
+        pkg_ver =  "\n".join(['=='.join(tups) for tups in zip(pkg, map(version, pkg))])
+        print(pkg_ver, "\npython=={}".format(py_ver[:6]))
+
+    @cell_magic
+    def diagram(self, _, cell):
+        """Magic cell that allows to call directly Jarvis diagram generator
+        @param[in] cell cell instance
+        @param[in] _ not used
+        @return None
+        """
+        out = self.generator.get_diagram_url(cell, True)
+        if out:
+            hyper = get_hyperlink(out)
+            display(HTML(hyper))
+            # Single display (not related to logging)
+            print("Overview :")
+            display(Markdown(f'![figure]({out})'))
```

### Comparing `jarvis4se-1.3.5/tests/test_input_cell.py` & `jarvis4se-1.4.0/tests/test_input_cell.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-"""@defgroup test_input_cell
-Tests about Jarvis outputs
-"""
-# Libraries
-
-
-# Modules
-import test_lib
-
-# Initialisation of Jarvis
-jarvis4se = test_lib.get_jarvis4se()[0]
-
-
-def test_attribute_declaration_in(capsys, input_test_fun_elem_with_attribute):
-    """@ingroup test_input_cell
-    @anchor test_attribute_declaration_in
-    Test attribute declaration
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_fun_elem_with_attribute : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_fun_elem_with_attribute
-    """
-    file_name = "test_attribute_declaration_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[1]}\n")
-
-    captured = capsys.readouterr()
-    expected = [f"Creating {file_name}.xml !\n",
-                "C is an attribute\n",
-                "A is an attribute\n",
-                "B is an attribute\n",
-                f"{file_name}.xml updated"]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert all(i in captured.out for i in expected)
-
-
-def test_instantiated_attribute_in(capsys, input_test_fun_elem_with_attribute):
-    """@ingroup test_input_cell
-    @anchor test_instantiated_attribute_in
-    Test attribute instantiation
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_fun_elem_with_attribute : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_fun_elem_with_attribute
-    """
-    file_name = "test_instantiated_attribute_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[0]}\n")
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[1]}\n")
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[2]}\n")
-
-    captured = capsys.readouterr()
-    expected = [f"{file_name}.xml parsed\n",
-                "Attribute A for F1 with value 4,2\n",
-                "Attribute C for F1 with value pink\n",
-                "Attribute B for Fun elem with value 8,5\n",
-                "Attribute A for Fun elem with value 100\n",
-                f"{file_name}.xml updated\n"]
-    # Get las part from capsys
-    last_out = captured.out[-len(''.join(expected)) - 1:len(captured.out)]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert all(i in last_out for i in expected)
-
-
-def test_functional_interface_in(capsys, input_test_functional_interface):
-    """@ingroup test_input_cell
-    @anchor test_functional_interface_in
-    Test data allocation to functional interface
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_functional_interface : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_functional_interface
-    """
-    file_name = "test_functional_interface_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_functional_interface}\n")
-
-    captured = capsys.readouterr()
-    expected = [f"Creating {file_name}.xml !\n",
-                "A is a Data\n",
-                "Fun_inter is a Functional interface\n",
-                "Color is an attribute\n",
-                "The alias for Fun_inter is FI\n",
-                "[ERROR] Data A has no producer(s) nor consumer(s) allocated to functional "
-                "elements exposing Fun_inter, A not allocated to Fun_inter\n",
-                "Attribute Color for Fun_inter with value pink\n",
-                f"{file_name}.xml updated\n"]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert len(captured.out) == len("".join(expected))
-    assert all(i in captured.out for i in expected)
-
-
-def test_fun_elem_exposes_interface_in(capsys, input_test_fun_elem_exposes_interface):
-    """@ingroup test_input_cell
-    @anchor test_fun_elem_exposes_interface_in
-    Test functional interface allocation to functional element
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_fun_elem_exposes_interface : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_fun_elem_exposes_interface
-    """
-    file_name = "test_fun_elem_exposes_interface_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_exposes_interface}\n")
-
-    captured = capsys.readouterr()
-    expected = ["Fun_elem exposes Fun_inter\n",
-                "Fun_elem_6 exposes Fun_inter\n",
-                "Fun_elem_ext exposes Fun_inter\n",
-                "[ERROR] toto does not exist, choose a valid name/alias for: "
-                "'Functional Element' exposes Fun_inter\n",
-                "[ERROR] tata and titi do not exist, choose valid names/aliases for: "
-                "'Functional Element' exposes 'Functional Interface'\n",
-                "[ERROR] coco does not exist, choose a valid name/alias for: "
-                "Fun_elem exposes 'Functional Interface'\n",
-                f"{file_name}.xml updated\n"]
-    # Get last part from capsys
-    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert all(i in last_out for i in expected)
-
-
-def test_function_output_auto_in(capsys, input_test_function_output_auto_decomposition):
-    """@ingroup test_input_cell
-    @anchor test_function_output_auto_in
-    Test function decomposition
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_function_output_auto_decomposition : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_function_output_auto_decomposition
-    """
-    file_name = "test_function_output_auto_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[0]}\n"
-                         f"{input_test_function_output_auto_decomposition[1]}\n")
-
-    captured = capsys.readouterr()
-    expected = ["F is a Function\n",
-                "a is a Data\n",
-                "F1 is a Function\n",
-                "F2 is a Function\n",
-                "F is composed of F1\n",
-                "F is composed of F2\n",
-                "[WARNING] No producer found for a\n",
-                "[WARNING] No producer found for a\n"
-                "F2 consumes a\n",
-                "F consumes a\n",
-                "F does not consume a anymore\n",
-                "F produces a\n",
-                "F1 produces a\n",
-                f"{file_name}.xml updated\n"]
-
-    # Get last part from capsys
-    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert all(i in last_out for i in expected)
-
-
-def test_function_output_auto_splitted_in(capsys, input_test_function_output_auto_decomposition):
-    """@ingroup test_input_cell
-    @anchor test_function_output_auto_splitted_in
-    Test function decomposition done in multiple cells
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_function_output_auto_decomposition : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_function_output_auto_decomposition
-    """
-    file_name = "test_function_output_auto_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[0]}\n")
-
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[1]}\n")
-
-    captured = capsys.readouterr()
-    expected = ["F2 is a Function\n",
-                "F is composed of F2\n",
-                "F does not produce a anymore\n",
-                "F2 consumes a\n",
-                f"{file_name}.xml updated\n"]
-
-    # Get last part from capsys
-    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert all(i in last_out for i in expected)
-
-
-def test_function_output_auto_external_in(capsys, input_test_function_output_auto_decomposition):
-    """@ingroup test_input_cell
-    @anchor test_function_output_auto_external_in
-    Test function decomposition done in multiple cells and with external function
-
-    @param[in] capsys : capture fixture reference
-    @param[in] input_test_function_output_auto_decomposition : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_function_output_auto_decomposition
-    """
-    file_name = "test_function_output_auto_in"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[0]}\n")
-
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[1]}\n")
-
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[2]}\n")
-
-    captured = capsys.readouterr()
-    expected = ["FE is a Function\n",
-                "F produces a due to one of its children\n",
-                "FE consumes a\n",
-                f"{file_name}.xml updated\n"]
-
-    # Get last part from capsys
-    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
-
-    test_lib.remove_xml_file(file_name)
-
-    assert all(i in last_out for i in expected)
+"""@defgroup test_input_cell
+Tests about Jarvis outputs
+"""
+# Libraries
+
+
+# Modules
+import test_lib
+
+# Initialisation of Jarvis
+jarvis4se = test_lib.get_jarvis4se()[0]
+
+
+def test_attribute_declaration_in(capsys, input_test_fun_elem_with_attribute):
+    """@ingroup test_input_cell
+    @anchor test_attribute_declaration_in
+    Test attribute declaration
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_fun_elem_with_attribute : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_fun_elem_with_attribute
+    """
+    file_name = "test_attribute_declaration_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[1]}\n")
+
+    captured = capsys.readouterr()
+    expected = [f"Creating {file_name}.xml !\n",
+                "C is an attribute\n",
+                "A is an attribute\n",
+                "B is an attribute\n",
+                f"{file_name}.xml updated"]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert all(i in captured.out for i in expected)
+
+
+def test_instantiated_attribute_in(capsys, input_test_fun_elem_with_attribute):
+    """@ingroup test_input_cell
+    @anchor test_instantiated_attribute_in
+    Test attribute instantiation
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_fun_elem_with_attribute : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_fun_elem_with_attribute
+    """
+    file_name = "test_instantiated_attribute_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[0]}\n")
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[1]}\n")
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[2]}\n")
+
+    captured = capsys.readouterr()
+    expected = [f"{file_name}.xml parsed\n",
+                "Attribute A for F1 with value 4,2\n",
+                "Attribute C for F1 with value pink\n",
+                "Attribute B for Fun elem with value 8,5\n",
+                "Attribute A for Fun elem with value 100\n",
+                f"{file_name}.xml updated\n"]
+    # Get las part from capsys
+    last_out = captured.out[-len(''.join(expected)) - 1:len(captured.out)]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert all(i in last_out for i in expected)
+
+
+def test_functional_interface_in(capsys, input_test_functional_interface):
+    """@ingroup test_input_cell
+    @anchor test_functional_interface_in
+    Test data allocation to functional interface
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_functional_interface : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_functional_interface
+    """
+    file_name = "test_functional_interface_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_functional_interface}\n")
+
+    captured = capsys.readouterr()
+    expected = [f"Creating {file_name}.xml !\n",
+                "A is a Data\n",
+                "Fun_inter is a Functional interface\n",
+                "Color is an attribute\n",
+                "The alias for Fun_inter is FI\n",
+                "[ERROR] Data A has no producer(s) nor consumer(s) allocated to functional "
+                "elements exposing Fun_inter, A not allocated to Fun_inter\n",
+                "Attribute Color for Fun_inter with value pink\n",
+                f"{file_name}.xml updated\n"]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert len(captured.out) == len("".join(expected))
+    assert all(i in captured.out for i in expected)
+
+
+def test_fun_elem_exposes_interface_in(capsys, input_test_fun_elem_exposes_interface):
+    """@ingroup test_input_cell
+    @anchor test_fun_elem_exposes_interface_in
+    Test functional interface allocation to functional element
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_fun_elem_exposes_interface : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_fun_elem_exposes_interface
+    """
+    file_name = "test_fun_elem_exposes_interface_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_exposes_interface}\n")
+
+    captured = capsys.readouterr()
+    expected = ["Fun_elem exposes Fun_inter\n",
+                "Fun_elem_6 exposes Fun_inter\n",
+                "Fun_elem_ext exposes Fun_inter\n",
+                "[ERROR] toto does not exist, choose a valid name/alias for: "
+                "'Functional Element' exposes Fun_inter\n",
+                "[ERROR] tata and titi do not exist, choose valid names/aliases for: "
+                "'Functional Element' exposes 'Functional Interface'\n",
+                "[ERROR] coco does not exist, choose a valid name/alias for: "
+                "Fun_elem exposes 'Functional Interface'\n",
+                f"{file_name}.xml updated\n"]
+    # Get last part from capsys
+    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert all(i in last_out for i in expected)
+
+
+def test_function_output_auto_in(capsys, input_test_function_output_auto_decomposition):
+    """@ingroup test_input_cell
+    @anchor test_function_output_auto_in
+    Test function decomposition
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_function_output_auto_decomposition : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_function_output_auto_decomposition
+    """
+    file_name = "test_function_output_auto_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[0]}\n"
+                         f"{input_test_function_output_auto_decomposition[1]}\n")
+
+    captured = capsys.readouterr()
+    expected = ["F is a Function\n",
+                "a is a Data\n",
+                "F1 is a Function\n",
+                "F2 is a Function\n",
+                "F is composed of F1\n",
+                "F is composed of F2\n",
+                "[WARNING] No producer found for a\n",
+                "[WARNING] No producer found for a\n"
+                "F2 consumes a\n",
+                "F consumes a\n",
+                "F does not consume a anymore\n",
+                "F produces a\n",
+                "F1 produces a\n",
+                f"{file_name}.xml updated\n"]
+
+    # Get last part from capsys
+    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert all(i in last_out for i in expected)
+
+
+def test_function_output_auto_splitted_in(capsys, input_test_function_output_auto_decomposition):
+    """@ingroup test_input_cell
+    @anchor test_function_output_auto_splitted_in
+    Test function decomposition done in multiple cells
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_function_output_auto_decomposition : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_function_output_auto_decomposition
+    """
+    file_name = "test_function_output_auto_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[0]}\n")
+
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[1]}\n")
+
+    captured = capsys.readouterr()
+    expected = ["F2 is a Function\n",
+                "F is composed of F2\n",
+                "F does not produce a anymore\n",
+                "F2 consumes a\n",
+                f"{file_name}.xml updated\n"]
+
+    # Get last part from capsys
+    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert all(i in last_out for i in expected)
+
+
+def test_function_output_auto_external_in(capsys, input_test_function_output_auto_decomposition):
+    """@ingroup test_input_cell
+    @anchor test_function_output_auto_external_in
+    Test function decomposition done in multiple cells and with external function
+
+    @param[in] capsys : capture fixture reference
+    @param[in] input_test_function_output_auto_decomposition : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_function_output_auto_decomposition
+    """
+    file_name = "test_function_output_auto_in"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[0]}\n")
+
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[1]}\n")
+
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[2]}\n")
+
+    captured = capsys.readouterr()
+    expected = ["FE is a Function\n",
+                "F produces a due to one of its children\n",
+                "FE consumes a\n",
+                f"{file_name}.xml updated\n"]
+
+    # Get last part from capsys
+    last_out = captured.out[-len(''.join(expected)):len(captured.out)]
+
+    test_lib.remove_xml_file(file_name)
+
+    assert all(i in last_out for i in expected)
```

### Comparing `jarvis4se-1.3.5/tests/test_lib.py` & `jarvis4se-1.4.0/tests/test_lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-"""@defgroup test_lib
-Test libraries
-"""
-
-# Libraries
-import os
-from pathlib import Path
-from IPython import get_ipython
-
-# Modules
-import jarvis
-
-
-def get_jarvis4se():
-    """@ingroup test_lib
-    Start an ipython session, init parser and jarvis4se magic call
-
-    @return jarvis4se magic call, jarvis4se diagram generator, jarvis4se magic tool
-    """
-    ip = get_ipython()
-    generator_jarvis = jarvis.PlantUmlGen()
-    parser = jarvis.command_parser.CmdParser(generator_jarvis)
-    my_magic_jarvis = jarvis.MagicJarvis(ip, parser)
-    my_magic_tool = jarvis.MagicTools(ip, generator_jarvis)
-    return my_magic_jarvis, generator_jarvis, my_magic_tool
-
-
-def remove_xml_file(file_name):
-    """@ingroup test_lib
-    Remove the XML file generated during the test
-
-    @return None
-    """
-    file_path = os.path.join("./", f"{file_name}.xml")
-    path = Path(file_path)
-    if path:
-        os.remove(path)
+"""@defgroup test_lib
+Test libraries
+"""
+
+# Libraries
+import os
+from pathlib import Path
+from IPython import get_ipython
+
+# Modules
+import jarvis
+
+
+def get_jarvis4se():
+    """@ingroup test_lib
+    Start an ipython session, init parser and jarvis4se magic call
+
+    @return jarvis4se magic call, jarvis4se diagram generator, jarvis4se magic tool
+    """
+    ip = get_ipython()
+    generator_jarvis = jarvis.PlantUmlGen()
+    parser = jarvis.command_parser.CmdParser(generator_jarvis)
+    my_magic_jarvis = jarvis.MagicJarvis(ip, parser)
+    my_magic_tool = jarvis.MagicTools(ip, generator_jarvis)
+    return my_magic_jarvis, generator_jarvis, my_magic_tool
+
+
+def remove_xml_file(file_name):
+    """@ingroup test_lib
+    Remove the XML file generated during the test
+
+    @return None
+    """
+    file_path = os.path.join("./", f"{file_name}.xml")
+    path = Path(file_path)
+    if path:
+        os.remove(path)
+
+
+def remove_csv_file(file_name):
+    """@ingroup test_lib
+    Remove the CSV file generated during the test
+
+    @return None
+    """
+    file_path = os.path.join("./", f"{file_name}.csv")
+    path = Path(file_path)
+    if path:
+        os.remove(path)
```

### Comparing `jarvis4se-1.3.5/tests/test_magic_tools.py` & `jarvis4se-1.4.0/tests/test_magic_tools.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""@defgroup test_magic_tools
-Tests about Jarvis IPython magic tools
-"""
-# Libraries
-
-
-# Modules
-import test_lib
-
-# Initialisation of Jarvis
-jarvis4se_all = test_lib.get_jarvis4se()
-generator = jarvis4se_all[1]
-jarvis4se_tool = jarvis4se_all[2]
-
-
-def test_retrieve_pkg_version_tool(capsys):
-    """@ingroup test_magic_tools
-    Test the magic line "%retrieve_pkg_version"
-
-    @param[in] capsys : capture fixture reference
-    @return None
-    """
-    jarvis4se_tool.retrieve_pkg_version('')
-    captured = capsys.readouterr()
-    expected = ["lxml==", "notebook==", "plantuml==", "jarvis4se==", "pandas==", "python=="]
-    assert all(i in captured.out for i in expected)
-
-
-def test_diagram_cell_tool(capsys, mocker):
-    """@ingroup test_magic_tools
-    Test the magic cell "%%diagram"
-
-    @param[in] capsys : capture fixture reference
-    @param[in] mocker : mocker fixture reference
-    @return None
-    """
-    spy = mocker.spy(generator, "get_diagram_url")
-    jarvis4se_tool.diagram('', "@startuml\n"
-                         "!define Junction_Or circle #black\n"
-                         "!define Junction_And circle #whitesmoke\n"
-                         "\n"
-                         "\n"
-                         "Junction_And JunctionAnd\n"
-                         "Junction_Or JunctionOr\n"
-                         "\n"
-                         "archimate #Technology 'VPN Server' as vpnServerA <<technology-device>>\n"
-                         "\n"
-                         "rectangle GO #lightgreen\n"
-                         "rectangle STOP #red\n"
-                         "rectangle WAIT #orange\n"
-                         "GO -up-> JunctionOr\n"
-                         "STOP -up-> JunctionOr\n"
-                         "STOP -down-> JunctionAnd\n"
-                         "WAIT -down-> JunctionAnd\n"
-                         "@enduml\n")
-    expected_plantuml_link = "http://www.plantuml.com/plantuml/svg/TL2nhi8m3Dpz5KOTcFe7gA8JUWmK" \
-                             "YGf651BJHgGESjCY_fx04oW8sExEToVRypue2KFdO6BeQ9bmER0ErlE-4jHMj2FC3ax" \
-                             "fqwUZPFEoN5eRgE_yYG3WpV4a4KDQ_iIL02ZHhUrKY4KrwPQzyyqLfzlr2ZSa8yaKLO" \
-                             "_ZcVzPYRDPUFboGwFLL1G0GZeeRk92YmepPvisD4B4oM1JLslCX4oYxSg_6ZClaH74P" \
-                             "3wSyo9Ty17weHf_uKI_d_de-pQO4vlxisy="
-    expected_notebook_output = "<IPython.core.display.HTML object>\n" \
-                               "Overview :\n" \
-                               "<IPython.core.display.Markdown object>\n"
-    captured = capsys.readouterr()
-    assert spy.spy_return == expected_plantuml_link
-    assert captured.out == expected_notebook_output
+"""@defgroup test_magic_tools
+Tests about Jarvis IPython magic tools
+"""
+# Libraries
+
+
+# Modules
+import test_lib
+
+# Initialisation of Jarvis
+jarvis4se_all = test_lib.get_jarvis4se()
+generator = jarvis4se_all[1]
+jarvis4se_tool = jarvis4se_all[2]
+
+
+def test_retrieve_pkg_version_tool(capsys):
+    """@ingroup test_magic_tools
+    Test the magic line "%retrieve_pkg_version"
+
+    @param[in] capsys : capture fixture reference
+    @return None
+    """
+    jarvis4se_tool.retrieve_pkg_version('')
+    captured = capsys.readouterr()
+    expected = ["lxml==", "notebook==", "plantuml==", "jarvis4se==", "pandas==", "python=="]
+    assert all(i in captured.out for i in expected)
+
+
+def test_diagram_cell_tool(capsys, mocker):
+    """@ingroup test_magic_tools
+    Test the magic cell "%%diagram"
+
+    @param[in] capsys : capture fixture reference
+    @param[in] mocker : mocker fixture reference
+    @return None
+    """
+    spy = mocker.spy(generator, "get_diagram_url")
+    jarvis4se_tool.diagram('', "@startuml\n"
+                         "!define Junction_Or circle #black\n"
+                         "!define Junction_And circle #whitesmoke\n"
+                         "\n"
+                         "\n"
+                         "Junction_And JunctionAnd\n"
+                         "Junction_Or JunctionOr\n"
+                         "\n"
+                         "archimate #Technology 'VPN Server' as vpnServerA <<technology-device>>\n"
+                         "\n"
+                         "rectangle GO #lightgreen\n"
+                         "rectangle STOP #red\n"
+                         "rectangle WAIT #orange\n"
+                         "GO -up-> JunctionOr\n"
+                         "STOP -up-> JunctionOr\n"
+                         "STOP -down-> JunctionAnd\n"
+                         "WAIT -down-> JunctionAnd\n"
+                         "@enduml\n")
+    expected_plantuml_link = "http://www.plantuml.com/plantuml/svg/TL2nhi8m3Dpz5KOTcFe7gA8JUWmK" \
+                             "YGf651BJHgGESjCY_fx04oW8sExEToVRypue2KFdO6BeQ9bmER0ErlE-4jHMj2FC3ax" \
+                             "fqwUZPFEoN5eRgE_yYG3WpV4a4KDQ_iIL02ZHhUrKY4KrwPQzyyqLfzlr2ZSa8yaKLO" \
+                             "_ZcVzPYRDPUFboGwFLL1G0GZeeRk92YmepPvisD4B4oM1JLslCX4oYxSg_6ZClaH74P" \
+                             "3wSyo9Ty17weHf_uKI_d_de-pQO4vlxisy="
+    expected_notebook_output = "<IPython.core.display.HTML object>\n" \
+                               "Overview :\n" \
+                               "<IPython.core.display.Markdown object>\n"
+    captured = capsys.readouterr()
+    assert spy.spy_return == expected_plantuml_link
+    assert captured.out == expected_notebook_output
```

### Comparing `jarvis4se-1.3.5/tests/test_xml_file.py` & `jarvis4se-1.4.0/tests/test_xml_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,338 +1,339 @@
-"""@defgroup test_xml_file
-Tests about xml file generation
-"""
-# Libraries
-import os
-from pathlib import Path
-
-# Modules
-import test_lib
-from xml_adapter import XmlParser3SE
-from datamodel import BaseType
-
-# Initialisation of Jarvis
-jarvis4se = test_lib.get_jarvis4se()[0]
-xml_parser = XmlParser3SE()
-
-
-def test_template_xml():
-    """@ingroup test_xml_file
-    @anchor test_template_xml
-    Test the structure of the xml generated file against the xml template
-
-    @return None
-    """
-    file_name = "test_template_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n")
-    path = Path(os.path.join("./", file_name + ".xml"))
-    with path as file:
-        read_xml = file.read_text(encoding="utf-8")
-        base_xml = "<?xml version='1.0' encoding='UTF-8'?>\n" \
-                   "<systemAnalysis>\n" \
-                   "  <funcArch>\n" \
-                   "    <functionList/>\n" \
-                   "    <dataList/>\n" \
-                   "    <stateList/>\n" \
-                   "    <transitionList/>\n" \
-                   "    <functionalElementList/>\n" \
-                   "    <functionalInterfaceList/>\n" \
-                   "  </funcArch>\n" \
-                   "  <phyArch>\n" \
-                   "    <physicalElementList/>\n" \
-                   "    <physicalInterfaceList/>\n" \
-                   "  </phyArch>\n" \
-                   "  <viewPoint>\n" \
-                   "    <viewList/>\n" \
-                   "    <attributeList/>\n" \
-                   "    <typeList/>\n" \
-                   "  </viewPoint>\n" \
-                   "</systemAnalysis>\n"
-        assert base_xml in read_xml
-
-    test_lib.remove_xml_file(file_name)
-
-
-def test_simple_function_xml(input_test_simple_function):
-    """@ingroup test_xml_file
-    @anchor test_simple_function_xml
-    Test xml file for a single function without input / output
-
-    @param[in] input_test_simple_function : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_simple_function
-    """
-    file_name = "test_simple_function_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_simple_function}\n")
-
-    function_list = xml_parser.parse_xml(file_name + ".xml")['xml_function_list']
-
-    test_lib.remove_xml_file(file_name)
-
-    assert len(function_list) == 1
-    assert [fun.name == "F1" for fun in function_list]
-
-
-def test_instantiated_attribute_xml(input_test_fun_elem_with_attribute):
-    """@ingroup test_xml_file
-    @anchor test_instantiated_attribute_xml
-    Test attribute instantiation in xml file
-
-    @param[in] input_test_fun_elem_with_attribute : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_fun_elem_with_attribute
-    """
-    file_name = "test_instantiated_attribute_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[0]}\n")
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[1]}\n")
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_with_attribute[2]}\n")
-
-    obj_dict = xml_parser.parse_xml(file_name + ".xml")
-
-    expected = {('A', 'F1', '4,2'), ('B', 'Fun elem', '8,5'),
-                ('C', 'F1', 'pink'), ('A', 'Fun elem', '100')}
-    # xml_adapter.parse_xml() returns mainly set(), so the order can change
-    # thus we have to compare it with a set also
-    result = set()
-    assert len(obj_dict['xml_attribute_list']) == 3
-    for attribute in obj_dict['xml_attribute_list']:
-        for item in attribute.described_item_list:
-            for function in obj_dict['xml_function_list']:
-                if item[0] == function.id:
-                    result.add((attribute.name, function.name, item[1]))
-            for fun_elem in obj_dict['xml_fun_elem_list']:
-                if item[0] == fun_elem.id:
-                    result.add((attribute.name, fun_elem.name, item[1]))
-
-    test_lib.remove_xml_file(file_name)
-
-    assert expected == result
-
-
-def test_extended_attribute_xml(input_test_extended_attribute):
-    """@ingroup test_xml_file
-    @anchor test_extended_attribute_xml
-    Test attribute extension in xml file
-
-    @param[in] input_test_extended_attribute : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_extended_attribute
-    """
-    file_name = "test_extended_attribute_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_extended_attribute}\n")
-
-    attribute_list = xml_parser.parse_xml(file_name + ".xml")['xml_attribute_list']
-    expected = {('A', 'attribute type A'), ('B', 'attribute type B')}
-    # xml_adapter.parse_xml() returns mainly set(), so the order can change
-    # thus we have to compare it with a set also
-    result = set()
-    assert len(attribute_list) == 2
-    for attribute in attribute_list:
-        result.add((attribute.name, attribute.type.name))
-
-    test_lib.remove_xml_file(file_name)
-
-    assert expected == result
-
-
-def test_functional_interface_with_attribute_xml(input_test_functional_interface_with_attribute):
-    """@ingroup test_xml_file
-    @anchor test_functional_interface_with_attribute_xml
-    Test functional interface with attribute in xml file
-
-    @param[in] input_test_functional_interface_with_attribute : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_functional_interface_with_attribute
-    """
-    file_name = "test_functional_interface_with_attribute_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_functional_interface_with_attribute}\n")
-
-    obj_dict = xml_parser.parse_xml(file_name + ".xml")
-
-    assert (len(obj_dict['xml_data_list']) == len(obj_dict['xml_attribute_list']) ==
-            len(obj_dict['xml_fun_inter_list'])) == 1
-    data = obj_dict['xml_data_list'].pop()
-    fun_inter = obj_dict['xml_fun_inter_list'].pop()
-    attribute = obj_dict['xml_attribute_list'].pop()
-    assert data.name == 'A'
-    assert fun_inter.name == 'Fun_inter'
-    assert fun_inter.alias == 'FI'
-    assert fun_inter.type == BaseType['FUNCTIONAL_INTERFACE']
-    assert attribute.name == 'Color'
-    described_item = attribute.described_item_list.pop()
-    assert described_item[0] == fun_inter.id and described_item[1] == 'pink'
-    assert fun_inter.allocated_data_list.pop() == data.id
-
-    test_lib.remove_xml_file(file_name)
-
-
-def test_fun_elem_exposes_interface_xml(input_test_fun_elem_exposes_interface):
-    """@ingroup test_xml_file
-    @anchor test_fun_elem_exposes_interface_xml
-    Test functional interface allocation to functional element
-
-    @param[in] input_test_fun_elem_exposes_interface : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_fun_elem_exposes_interface
-    """
-    file_name = "test_fun_elem_exposes_interface_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_fun_elem_exposes_interface}\n")
-
-    obj_dict = xml_parser.parse_xml(file_name + ".xml")
-
-    expected_child = {('Fun_elem', 'Fun_elem_2'), ('Fun_elem_2', 'Fun_elem_3'),
-                      ('Fun_elem_3', 'Fun_elem_4'), ('Fun_elem_4', 'Fun_elem_5'),
-                      ('Fun_elem_5', 'Fun_elem_6')}
-    expected_exposed = {('Fun_elem', 'Fun_inter'), ('Fun_elem_6', 'Fun_inter'),
-                        ('Fun_elem_ext', 'Fun_inter')}
-
-    assert len(obj_dict['xml_fun_inter_list']) == 1 and len(obj_dict['xml_fun_elem_list']) == 8
-    fun_inter = obj_dict['xml_fun_inter_list'].pop()
-    assert fun_inter.name == 'Fun_inter'
-
-    result_exposed = set()
-    result_child = set()
-    for fun_elem in obj_dict['xml_fun_elem_list']:
-        for child in fun_elem.child_list:
-            result_child.add((fun_elem.name, child.name))
-        if fun_inter.id in fun_elem.exposed_interface_list:
-            result_exposed.add((fun_elem.name, fun_inter.name))
-
-    assert expected_child == result_child
-    assert expected_exposed == result_exposed
-
-    test_lib.remove_xml_file(file_name)
-
-
-def test_function_output_auto_xml(input_test_function_output_auto_decomposition):
-    """@ingroup test_xml_file
-    @anchor test_function_output_auto_xml
-    Test function decomposition
-
-    @param[in] input_test_function_output_auto_decomposition : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_function_output_auto_decomposition
-    """
-    file_name = "test_function_output_auto_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[0]}\n"
-                         f"{input_test_function_output_auto_decomposition[1]}\n")
-
-    obj_dict = xml_parser.parse_xml(file_name + ".xml")
-
-    assert len(obj_dict['xml_function_list']) == 3
-
-    expected_consumer_list = {('a', 'F2')}
-    expected_producer_list = {('a', 'F1'), ('a', 'F')}
-
-    result_consumer_list = set()
-    result_producer_list = set()
-    for flow_cons_list in obj_dict['xml_consumer_function_list']:
-        result_consumer_list.add((flow_cons_list[0], flow_cons_list[1].name))
-
-    for flow_prod_list in obj_dict['xml_producer_function_list']:
-        result_producer_list.add((flow_prod_list[0], flow_prod_list[1].name))
-
-    assert result_consumer_list == expected_consumer_list
-    assert result_producer_list == expected_producer_list
-
-    test_lib.remove_xml_file(file_name)
-
-
-def test_function_output_auto_splitted_xml(input_test_function_output_auto_decomposition):
-    """@ingroup test_xml_file
-    @anchor test_function_output_auto_splitted_xml
-    Test function decomposition done in multiple cells
-
-    @param[in] input_test_function_output_auto_decomposition : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_function_output_auto_decomposition
-    """
-    file_name = "test_function_output_auto_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[0]}\n")
-
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[1]}\n")
-
-    obj_dict = xml_parser.parse_xml(file_name + ".xml")
-
-    assert len(obj_dict['xml_function_list']) == 3
-
-    expected_consumer_list = {('a', 'F2')}
-    expected_producer_list = {('a', 'F1')}
-
-    result_consumer_list = set()
-    result_producer_list = set()
-    for flow_cons_list in obj_dict['xml_consumer_function_list']:
-        result_consumer_list.add((flow_cons_list[0], flow_cons_list[1].name))
-
-    for flow_prod_list in obj_dict['xml_producer_function_list']:
-        result_producer_list.add((flow_prod_list[0], flow_prod_list[1].name))
-
-    assert result_consumer_list == expected_consumer_list
-    assert result_producer_list == expected_producer_list
-
-    test_lib.remove_xml_file(file_name)
-
-
-def test_function_output_auto_external_xml(input_test_function_output_auto_decomposition):
-    """@ingroup test_xml_file
-    @anchor test_function_output_auto_external_xml
-    Test function decomposition done in multiple cells and with external function
-
-    @param[in] input_test_function_output_auto_decomposition : input fixture reference
-    @return None
-
-    **Jarvis4se equivalent:**
-    @ref input_test_function_output_auto_decomposition
-    """
-    file_name = "test_function_output_auto_xml"
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[0]}\n")
-
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[1]}\n")
-
-    jarvis4se.jarvis("", f"with {file_name}\n"
-                         f"{input_test_function_output_auto_decomposition[2]}\n")
-
-    obj_dict = xml_parser.parse_xml(file_name + ".xml")
-
-    assert len(obj_dict['xml_function_list']) == 4
-
-    expected_consumer_list = {('a', 'F2'), ('a', 'FE')}
-    expected_producer_list = {('a', 'F1'), ('a', 'F')}
-
-    result_consumer_list = set()
-    result_producer_list = set()
-    for flow_cons_list in obj_dict['xml_consumer_function_list']:
-        result_consumer_list.add((flow_cons_list[0], flow_cons_list[1].name))
-
-    for flow_prod_list in obj_dict['xml_producer_function_list']:
-        result_producer_list.add((flow_prod_list[0], flow_prod_list[1].name))
-
-    assert result_consumer_list == expected_consumer_list
-    assert result_producer_list == expected_producer_list
-
-    test_lib.remove_xml_file(file_name)
+"""@defgroup test_xml_file
+Tests about xml file generation
+"""
+# Libraries
+import os
+from pathlib import Path
+
+# Modules
+import test_lib
+from xml_adapter import XmlParser3SE
+from datamodel import BaseType
+
+# Initialisation of Jarvis
+jarvis4se = test_lib.get_jarvis4se()[0]
+xml_parser = XmlParser3SE()
+
+
+def test_template_xml():
+    """@ingroup test_xml_file
+    @anchor test_template_xml
+    Test the structure of the xml generated file against the xml template
+
+    @return None
+    """
+    file_name = "test_template_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n")
+    path = Path(os.path.join("./", file_name + ".xml"))
+    with path as file:
+        read_xml = file.read_text(encoding="utf-8")
+        base_xml = "<?xml version='1.0' encoding='UTF-8'?>\n" \
+                   "<systemAnalysis>\n" \
+                   "  <funcArch>\n" \
+                   "    <functionList/>\n" \
+                   "    <dataList/>\n" \
+                   "    <stateList/>\n" \
+                   "    <transitionList/>\n" \
+                   "    <functionalElementList/>\n" \
+                   "    <functionalInterfaceList/>\n" \
+                   "  </funcArch>\n" \
+                   "  <phyArch>\n" \
+                   "    <physicalElementList/>\n" \
+                   "    <physicalInterfaceList/>\n" \
+                   "  </phyArch>\n" \
+                   "  <viewPoint>\n" \
+                   "    <viewList/>\n" \
+                   "    <attributeList/>\n" \
+                   "    <requirementList/>\n" \
+                   "    <typeList/>\n" \
+                   "  </viewPoint>\n" \
+                   "</systemAnalysis>\n"
+        assert base_xml in read_xml
+
+    test_lib.remove_xml_file(file_name)
+
+
+def test_simple_function_xml(input_test_simple_function):
+    """@ingroup test_xml_file
+    @anchor test_simple_function_xml
+    Test xml file for a single function without input / output
+
+    @param[in] input_test_simple_function : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_simple_function
+    """
+    file_name = "test_simple_function_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_simple_function}\n")
+
+    function_list = xml_parser.parse_xml(file_name + ".xml")['xml_function_list']
+
+    test_lib.remove_xml_file(file_name)
+
+    assert len(function_list) == 1
+    assert [fun.name == "F1" for fun in function_list]
+
+
+def test_instantiated_attribute_xml(input_test_fun_elem_with_attribute):
+    """@ingroup test_xml_file
+    @anchor test_instantiated_attribute_xml
+    Test attribute instantiation in xml file
+
+    @param[in] input_test_fun_elem_with_attribute : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_fun_elem_with_attribute
+    """
+    file_name = "test_instantiated_attribute_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[0]}\n")
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[1]}\n")
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_with_attribute[2]}\n")
+
+    obj_dict = xml_parser.parse_xml(file_name + ".xml")
+
+    expected = {('A', 'F1', '4,2'), ('B', 'Fun elem', '8,5'),
+                ('C', 'F1', 'pink'), ('A', 'Fun elem', '100')}
+    # xml_adapter.parse_xml() returns mainly set(), so the order can change
+    # thus we have to compare it with a set also
+    result = set()
+    assert len(obj_dict['xml_attribute_list']) == 3
+    for attribute in obj_dict['xml_attribute_list']:
+        for item in attribute.described_item_list:
+            for function in obj_dict['xml_function_list']:
+                if item[0] == function.id:
+                    result.add((attribute.name, function.name, item[1]))
+            for fun_elem in obj_dict['xml_fun_elem_list']:
+                if item[0] == fun_elem.id:
+                    result.add((attribute.name, fun_elem.name, item[1]))
+
+    test_lib.remove_xml_file(file_name)
+
+    assert expected == result
+
+
+def test_extended_attribute_xml(input_test_extended_attribute):
+    """@ingroup test_xml_file
+    @anchor test_extended_attribute_xml
+    Test attribute extension in xml file
+
+    @param[in] input_test_extended_attribute : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_extended_attribute
+    """
+    file_name = "test_extended_attribute_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_extended_attribute}\n")
+
+    attribute_list = xml_parser.parse_xml(file_name + ".xml")['xml_attribute_list']
+    expected = {('A', 'attribute type A'), ('B', 'attribute type B')}
+    # xml_adapter.parse_xml() returns mainly set(), so the order can change
+    # thus we have to compare it with a set also
+    result = set()
+    assert len(attribute_list) == 2
+    for attribute in attribute_list:
+        result.add((attribute.name, attribute.type.name))
+
+    test_lib.remove_xml_file(file_name)
+
+    assert expected == result
+
+
+def test_functional_interface_with_attribute_xml(input_test_functional_interface_with_attribute):
+    """@ingroup test_xml_file
+    @anchor test_functional_interface_with_attribute_xml
+    Test functional interface with attribute in xml file
+
+    @param[in] input_test_functional_interface_with_attribute : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_functional_interface_with_attribute
+    """
+    file_name = "test_functional_interface_with_attribute_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_functional_interface_with_attribute}\n")
+
+    obj_dict = xml_parser.parse_xml(file_name + ".xml")
+
+    assert (len(obj_dict['xml_data_list']) == len(obj_dict['xml_attribute_list']) ==
+            len(obj_dict['xml_fun_inter_list'])) == 1
+    data = obj_dict['xml_data_list'].pop()
+    fun_inter = obj_dict['xml_fun_inter_list'].pop()
+    attribute = obj_dict['xml_attribute_list'].pop()
+    assert data.name == 'A'
+    assert fun_inter.name == 'Fun_inter'
+    assert fun_inter.alias == 'FI'
+    assert fun_inter.type == BaseType['FUNCTIONAL_INTERFACE']
+    assert attribute.name == 'Color'
+    described_item = attribute.described_item_list.pop()
+    assert described_item[0] == fun_inter.id and described_item[1] == 'pink'
+    assert fun_inter.allocated_data_list.pop() == data.id
+
+    test_lib.remove_xml_file(file_name)
+
+
+def test_fun_elem_exposes_interface_xml(input_test_fun_elem_exposes_interface):
+    """@ingroup test_xml_file
+    @anchor test_fun_elem_exposes_interface_xml
+    Test functional interface allocation to functional element
+
+    @param[in] input_test_fun_elem_exposes_interface : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_fun_elem_exposes_interface
+    """
+    file_name = "test_fun_elem_exposes_interface_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_fun_elem_exposes_interface}\n")
+
+    obj_dict = xml_parser.parse_xml(file_name + ".xml")
+
+    expected_child = {('Fun_elem', 'Fun_elem_2'), ('Fun_elem_2', 'Fun_elem_3'),
+                      ('Fun_elem_3', 'Fun_elem_4'), ('Fun_elem_4', 'Fun_elem_5'),
+                      ('Fun_elem_5', 'Fun_elem_6')}
+    expected_exposed = {('Fun_elem', 'Fun_inter'), ('Fun_elem_6', 'Fun_inter'),
+                        ('Fun_elem_ext', 'Fun_inter')}
+
+    assert len(obj_dict['xml_fun_inter_list']) == 1 and len(obj_dict['xml_fun_elem_list']) == 8
+    fun_inter = obj_dict['xml_fun_inter_list'].pop()
+    assert fun_inter.name == 'Fun_inter'
+
+    result_exposed = set()
+    result_child = set()
+    for fun_elem in obj_dict['xml_fun_elem_list']:
+        for child in fun_elem.child_list:
+            result_child.add((fun_elem.name, child.name))
+        if fun_inter.id in fun_elem.exposed_interface_list:
+            result_exposed.add((fun_elem.name, fun_inter.name))
+
+    assert expected_child == result_child
+    assert expected_exposed == result_exposed
+
+    test_lib.remove_xml_file(file_name)
+
+
+def test_function_output_auto_xml(input_test_function_output_auto_decomposition):
+    """@ingroup test_xml_file
+    @anchor test_function_output_auto_xml
+    Test function decomposition
+
+    @param[in] input_test_function_output_auto_decomposition : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_function_output_auto_decomposition
+    """
+    file_name = "test_function_output_auto_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[0]}\n"
+                         f"{input_test_function_output_auto_decomposition[1]}\n")
+
+    obj_dict = xml_parser.parse_xml(file_name + ".xml")
+
+    assert len(obj_dict['xml_function_list']) == 3
+
+    expected_consumer_list = {('a', 'F2')}
+    expected_producer_list = {('a', 'F1'), ('a', 'F')}
+
+    result_consumer_list = set()
+    result_producer_list = set()
+    for flow_cons_list in obj_dict['xml_consumer_function_list']:
+        result_consumer_list.add((flow_cons_list[0], flow_cons_list[1].name))
+
+    for flow_prod_list in obj_dict['xml_producer_function_list']:
+        result_producer_list.add((flow_prod_list[0], flow_prod_list[1].name))
+
+    assert result_consumer_list == expected_consumer_list
+    assert result_producer_list == expected_producer_list
+
+    test_lib.remove_xml_file(file_name)
+
+
+def test_function_output_auto_splitted_xml(input_test_function_output_auto_decomposition):
+    """@ingroup test_xml_file
+    @anchor test_function_output_auto_splitted_xml
+    Test function decomposition done in multiple cells
+
+    @param[in] input_test_function_output_auto_decomposition : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_function_output_auto_decomposition
+    """
+    file_name = "test_function_output_auto_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[0]}\n")
+
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[1]}\n")
+
+    obj_dict = xml_parser.parse_xml(file_name + ".xml")
+
+    assert len(obj_dict['xml_function_list']) == 3
+
+    expected_consumer_list = {('a', 'F2')}
+    expected_producer_list = {('a', 'F1')}
+
+    result_consumer_list = set()
+    result_producer_list = set()
+    for flow_cons_list in obj_dict['xml_consumer_function_list']:
+        result_consumer_list.add((flow_cons_list[0], flow_cons_list[1].name))
+
+    for flow_prod_list in obj_dict['xml_producer_function_list']:
+        result_producer_list.add((flow_prod_list[0], flow_prod_list[1].name))
+
+    assert result_consumer_list == expected_consumer_list
+    assert result_producer_list == expected_producer_list
+
+    test_lib.remove_xml_file(file_name)
+
+
+def test_function_output_auto_external_xml(input_test_function_output_auto_decomposition):
+    """@ingroup test_xml_file
+    @anchor test_function_output_auto_external_xml
+    Test function decomposition done in multiple cells and with external function
+
+    @param[in] input_test_function_output_auto_decomposition : input fixture reference
+    @return None
+
+    **Jarvis4se equivalent:**
+    @ref input_test_function_output_auto_decomposition
+    """
+    file_name = "test_function_output_auto_xml"
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[0]}\n")
+
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[1]}\n")
+
+    jarvis4se.jarvis("", f"with {file_name}\n"
+                         f"{input_test_function_output_auto_decomposition[2]}\n")
+
+    obj_dict = xml_parser.parse_xml(file_name + ".xml")
+
+    assert len(obj_dict['xml_function_list']) == 4
+
+    expected_consumer_list = {('a', 'F2'), ('a', 'FE')}
+    expected_producer_list = {('a', 'F1'), ('a', 'F')}
+
+    result_consumer_list = set()
+    result_producer_list = set()
+    for flow_cons_list in obj_dict['xml_consumer_function_list']:
+        result_consumer_list.add((flow_cons_list[0], flow_cons_list[1].name))
+
+    for flow_prod_list in obj_dict['xml_producer_function_list']:
+        result_producer_list.add((flow_prod_list[0], flow_prod_list[1].name))
+
+    assert result_consumer_list == expected_consumer_list
+    assert result_producer_list == expected_producer_list
+
+    test_lib.remove_xml_file(file_name)
```

