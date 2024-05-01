# Comparing `tmp/SpiffWorkflow-3.0.0rc0.tar.gz` & `tmp/SpiffWorkflow-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiffWorkflow-3.0.0rc0.tar", last modified: Fri Feb  9 14:47:37 2024, max compression
+gzip compressed data, was "SpiffWorkflow-3.0.0rc2.tar", last modified: Fri Feb  9 16:42:44 2024, max compression
```

## Comparing `SpiffWorkflow-3.0.0rc0.tar` & `SpiffWorkflow-3.0.0rc2.tar`

### file list

```diff
@@ -1,20 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:47:37.050413 SpiffWorkflow-3.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-09 14:47:37.050413 SpiffWorkflow-3.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:47:37.046414 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/task.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:47:37.050413 SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-09 14:47:37.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-09 14:47:37.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 14:47:37.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-09 14:47:37.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-09 14:47:37.000000 SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-09 14:47:29.000000 SpiffWorkflow-3.0.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 14:47:37.050413 SpiffWorkflow-3.0.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.423913 SpiffWorkflow-3.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-09 16:42:44.423913 SpiffWorkflow-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.395913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.395913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.399913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/BpmnParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/ProcessParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/TaskParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/ValidationException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/node_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.399913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/schema/DC.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/schema/DI.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    60913 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/schema/Semantic.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/spec_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/task_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/parser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.399913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/script_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/script_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12330 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/script_engine/feel_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/script_engine/python_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/script_engine/python_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.399913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.403913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/default/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/default/process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/default/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/default/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.403913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/helpers/bpmn_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/helpers/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/helpers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/helpers/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.403913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/migration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/migration/version_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/migration/version_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/migration/version_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/migration/version_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/serializer/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.403913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/bpmn_task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.403913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/item_aware_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/event_definitions/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.407913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.407913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/events/end_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/events/start_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/manual_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/none_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/script_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/service_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/specs/mixins/user_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.407913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/util/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/util/subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/util/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/bpmn/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.407913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.407913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/parser/CamundaParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/parser/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/serializer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/serializer/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/specs/business_rule_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/specs/event_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/specs/multiinstance_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/camunda/specs/user_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/engine/DMNEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/BpmnDmnParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/DMNParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/DC.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/DMN.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/DMN12.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/DMN13.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.411913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/specs/business_rule_task_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/dmn/specs/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.415913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22609 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/dotv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/prettyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28931 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/serializer/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/AcquireMutex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/CancelTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Choose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/ExclusiveChoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/MultiChoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/MultiInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/ReleaseMutex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/StartTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/SubWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/ThreadMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/ThreadSplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/ThreadStart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/WorkflowSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/specs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/schema/spiffworkflow.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/parser/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/serializer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/serializer/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/serializer/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/data_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/event_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.419913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/mixins/service_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/spiff/specs/spiff_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.423913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/deep_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/util/weakmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:42:44.423913 SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-09 16:42:44.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-02-09 16:42:44.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:42:44.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-09 16:42:44.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-09 16:42:44.000000 SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-09 16:42:37.000000 SpiffWorkflow-3.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:42:44.423913 SpiffWorkflow-3.0.0rc2/setup.cfg
```

### Comparing `SpiffWorkflow-3.0.0rc0/COPYING` & `SpiffWorkflow-3.0.0rc2/COPYING`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/PKG-INFO` & `SpiffWorkflow-3.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiffWorkflow
-Version: 3.0.0rc0
+Version: 3.0.0rc2
 Summary: A workflow framework and BPMN/DMN Processor
 Author-email: Sartography <dan@sartography.com>
 License: lGPLv3
 Project-URL: Homepage, https://github.com/sartography/SpiffWorkflow
 Project-URL: Documentation, https://spiffworkflow.readthedocs.io
 Keywords: spiff,workflow,bpmn,engine
 Classifier: Development Status :: 4 - Beta
```

### Comparing `SpiffWorkflow-3.0.0rc0/README.md` & `SpiffWorkflow-3.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/SpiffWorkflow/__init__.py` & `SpiffWorkflow-3.0.0rc2/SpiffWorkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/SpiffWorkflow/exceptions.py` & `SpiffWorkflow-3.0.0rc2/SpiffWorkflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/SpiffWorkflow/operators.py` & `SpiffWorkflow-3.0.0rc2/SpiffWorkflow/operators.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/SpiffWorkflow/task.py` & `SpiffWorkflow-3.0.0rc2/SpiffWorkflow/task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/SpiffWorkflow/workflow.py` & `SpiffWorkflow-3.0.0rc2/SpiffWorkflow/workflow.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-3.0.0rc0/SpiffWorkflow.egg-info/PKG-INFO` & `SpiffWorkflow-3.0.0rc2/SpiffWorkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiffWorkflow
-Version: 3.0.0rc0
+Version: 3.0.0rc2
 Summary: A workflow framework and BPMN/DMN Processor
 Author-email: Sartography <dan@sartography.com>
 License: lGPLv3
 Project-URL: Homepage, https://github.com/sartography/SpiffWorkflow
 Project-URL: Documentation, https://spiffworkflow.readthedocs.io
 Keywords: spiff,workflow,bpmn,engine
 Classifier: Development Status :: 4 - Beta
```

### Comparing `SpiffWorkflow-3.0.0rc0/pyproject.toml` & `SpiffWorkflow-3.0.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     "sphinx_rtd_theme",
 ]
 dev = [
     "build",
     "coverage",
 ]
 
-[tool.setuptools]
-packages = ["SpiffWorkflow"]
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["SpiffWorkflow*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "SpiffWorkflow.__version__"}
 
 [tool.setuptools.package-data]
 "*" = ["schema/*.xsd"]
```

