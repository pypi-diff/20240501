# Comparing `tmp/workflows-2.8.tar.gz` & `tmp/workflows-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workflows-2.8.tar", last modified: Tue May 18 07:21:35 2021, max compression
+gzip compressed data, was "workflows-2.9.tar", last modified: Mon Jun  7 08:37:02 2021, max compression
```

## Comparing `workflows-2.8.tar` & `workflows-2.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1486 2021-05-18 07:21:30.000000 workflows-2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      262 2021-05-18 07:21:30.000000 workflows-2.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     3876 2021-05-18 07:21:35.990951 workflows-2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2327 2021-05-18 07:21:30.000000 workflows-2.8/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)       29 2021-05-18 07:21:30.000000 workflows-2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     2045 2021-05-18 07:21:35.990951 workflows-2.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      154 2021-05-18 07:21:30.000000 workflows-2.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.982951 workflows-2.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.982951 workflows-2.8/src/workflows/
--rw-r--r--   0 vsts      (1001) docker     (121)      346 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/contrib/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/contrib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5323 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/contrib/start_service.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8929 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/contrib/status_monitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/frontend/
--rw-r--r--   0 vsts      (1001) docker     (121)    18492 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/frontend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1987 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/frontend/utilization.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/logging/
--rw-r--r--   0 vsts      (1001) docker     (121)     2316 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/logging/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/recipe/
--rw-r--r--   0 vsts      (1001) docker     (121)     5282 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/recipe/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14083 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/recipe/recipe.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2181 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/recipe/validate.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8860 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/recipe/wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/services/
--rw-r--r--   0 vsts      (1001) docker     (121)     1037 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19213 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/services/common_service.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1438 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/services/sample_consumer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1266 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/services/sample_producer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3263 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/services/sample_transaction.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/transport/
--rw-r--r--   0 vsts      (1001) docker     (121)      887 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/transport/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21514 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/transport/common_transport.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22340 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/transport/pika_transport.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20136 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/transport/stomp_transport.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/util/
--rw-r--r--   0 vsts      (1001) docker     (121)      298 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows/util/zocalo/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/util/zocalo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1643 2021-05-18 07:21:30.000000 workflows-2.8/src/workflows/util/zocalo/configuration.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.986951 workflows-2.8/src/workflows.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     3876 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1811 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      780 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       31 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       10 2021-05-18 07:21:35.000000 workflows-2.8/src/workflows.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/contrib/
--rw-r--r--   0 vsts      (1001) docker     (121)     1781 2021-05-18 07:21:30.000000 workflows-2.8/tests/contrib/test_start_service.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1391 2021-05-18 07:21:30.000000 workflows-2.8/tests/contrib/test_status_monitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/frontend/
--rw-r--r--   0 vsts      (1001) docker     (121)    22047 2021-05-18 07:21:30.000000 workflows-2.8/tests/frontend/test_frontend.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4230 2021-05-18 07:21:30.000000 workflows-2.8/tests/frontend/test_utilization.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/recipe/
--rw-r--r--   0 vsts      (1001) docker     (121)    11300 2021-05-18 07:21:30.000000 workflows-2.8/tests/recipe/test_recipe.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3776 2021-05-18 07:21:30.000000 workflows-2.8/tests/recipe/test_validate.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7294 2021-05-18 07:21:30.000000 workflows-2.8/tests/recipe/test_wrap_subscription.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12240 2021-05-18 07:21:30.000000 workflows-2.8/tests/recipe/test_wrapped_recipe.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/services/
--rw-r--r--   0 vsts      (1001) docker     (121)      198 2021-05-18 07:21:30.000000 workflows-2.8/tests/services/test.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21655 2021-05-18 07:21:30.000000 workflows-2.8/tests/services/test_common_service.py
--rw-r--r--   0 vsts      (1001) docker     (121)      963 2021-05-18 07:21:30.000000 workflows-2.8/tests/services/test_sample_consumer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1306 2021-05-18 07:21:30.000000 workflows-2.8/tests/services/test_sample_producer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4828 2021-05-18 07:21:30.000000 workflows-2.8/tests/services/test_sample_transaction.py
--rw-r--r--   0 vsts      (1001) docker     (121)      204 2021-05-18 07:21:30.000000 workflows-2.8/tests/test_basics.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2150 2021-05-18 07:21:30.000000 workflows-2.8/tests/test_logging.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/transport/
--rw-r--r--   0 vsts      (1001) docker     (121)      332 2021-05-18 07:21:30.000000 workflows-2.8/tests/transport/test.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11531 2021-05-18 07:21:30.000000 workflows-2.8/tests/transport/test_common.py
--rw-r--r--   0 vsts      (1001) docker     (121)    26192 2021-05-18 07:21:30.000000 workflows-2.8/tests/transport/test_pika.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25184 2021-05-18 07:21:30.000000 workflows-2.8/tests/transport/test_stomp.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-05-18 07:21:35.990951 workflows-2.8/tests/util/
--rw-r--r--   0 vsts      (1001) docker     (121)      185 2021-05-18 07:21:30.000000 workflows-2.8/tests/util/test.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.428833 workflows-2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1486 2021-06-07 08:36:58.000000 workflows-2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      262 2021-06-07 08:36:58.000000 workflows-2.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     3876 2021-06-07 08:37:02.428833 workflows-2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2327 2021-06-07 08:36:58.000000 workflows-2.9/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      130 2021-06-07 08:36:58.000000 workflows-2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2042 2021-06-07 08:37:02.428833 workflows-2.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      154 2021-06-07 08:36:58.000000 workflows-2.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.420833 workflows-2.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.420833 workflows-2.9/src/workflows/
+-rw-r--r--   0 vsts      (1001) docker     (121)      346 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/contrib/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/contrib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5323 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/contrib/start_service.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8929 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/contrib/status_monitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/frontend/
+-rw-r--r--   0 vsts      (1001) docker     (121)    18492 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/frontend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1987 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/frontend/utilization.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/logging/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2316 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/logging/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/recipe/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5282 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/recipe/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14083 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/recipe/recipe.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2181 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/recipe/validate.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8860 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/recipe/wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/services/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1037 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/services/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19297 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/services/common_service.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1438 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/services/sample_consumer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1266 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/services/sample_producer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3263 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/services/sample_transaction.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/transport/
+-rw-r--r--   0 vsts      (1001) docker     (121)      887 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/transport/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21514 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/transport/common_transport.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22340 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/transport/pika_transport.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20186 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/transport/stomp_transport.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)      298 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/src/workflows/util/zocalo/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/util/zocalo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1643 2021-06-07 08:36:58.000000 workflows-2.9/src/workflows/util/zocalo/configuration.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.420833 workflows-2.9/src/workflows.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3876 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1811 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      780 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       10 2021-06-07 08:37:02.000000 workflows-2.9/src/workflows.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/tests/contrib/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1781 2021-06-07 08:36:58.000000 workflows-2.9/tests/contrib/test_start_service.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1391 2021-06-07 08:36:58.000000 workflows-2.9/tests/contrib/test_status_monitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.424833 workflows-2.9/tests/frontend/
+-rw-r--r--   0 vsts      (1001) docker     (121)    22047 2021-06-07 08:36:58.000000 workflows-2.9/tests/frontend/test_frontend.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4230 2021-06-07 08:36:58.000000 workflows-2.9/tests/frontend/test_utilization.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.428833 workflows-2.9/tests/recipe/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11300 2021-06-07 08:36:58.000000 workflows-2.9/tests/recipe/test_recipe.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3776 2021-06-07 08:36:58.000000 workflows-2.9/tests/recipe/test_validate.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7294 2021-06-07 08:36:58.000000 workflows-2.9/tests/recipe/test_wrap_subscription.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12240 2021-06-07 08:36:58.000000 workflows-2.9/tests/recipe/test_wrapped_recipe.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.428833 workflows-2.9/tests/services/
+-rw-r--r--   0 vsts      (1001) docker     (121)      198 2021-06-07 08:36:58.000000 workflows-2.9/tests/services/test.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21655 2021-06-07 08:36:58.000000 workflows-2.9/tests/services/test_common_service.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      963 2021-06-07 08:36:58.000000 workflows-2.9/tests/services/test_sample_consumer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1306 2021-06-07 08:36:58.000000 workflows-2.9/tests/services/test_sample_producer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4828 2021-06-07 08:36:58.000000 workflows-2.9/tests/services/test_sample_transaction.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      204 2021-06-07 08:36:58.000000 workflows-2.9/tests/test_basics.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2150 2021-06-07 08:36:58.000000 workflows-2.9/tests/test_logging.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.428833 workflows-2.9/tests/transport/
+-rw-r--r--   0 vsts      (1001) docker     (121)      332 2021-06-07 08:36:58.000000 workflows-2.9/tests/transport/test.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11531 2021-06-07 08:36:58.000000 workflows-2.9/tests/transport/test_common.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26192 2021-06-07 08:36:58.000000 workflows-2.9/tests/transport/test_pika.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25374 2021-06-07 08:36:58.000000 workflows-2.9/tests/transport/test_stomp.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-07 08:37:02.428833 workflows-2.9/tests/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)      185 2021-06-07 08:36:58.000000 workflows-2.9/tests/util/test.py
```

### Comparing `workflows-2.8/LICENSE` & `workflows-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `workflows-2.8/PKG-INFO` & `workflows-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: workflows
-Version: 2.8
+Version: 2.9
 Summary: Data processing in distributed environments
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software et al.
 Author-email: scientificsoftware@diamond.ac.uk
 License: BSD
 Project-URL: Download, https://github.com/DiamondLightSource/python-workflows/releases
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-workflows
```

### Comparing `workflows-2.8/README.rst` & `workflows-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `workflows-2.8/setup.cfg` & `workflows-2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = workflows
-version = 2.8
+version = 2.9
 description = Data processing in distributed environments
 long_description = file: README.rst
 author = Diamond Light Source - Scientific Software et al.
 author_email = scientificsoftware@diamond.ac.uk
 license = BSD
 license_file = LICENSE
 classifiers = 
@@ -24,15 +24,15 @@
 	GitHub = https://github.com/DiamondLightSource/python-workflows
 	Bug-Tracker = https://github.com/DiamondLightSource/python-workflows/issues
 
 [options]
 install_requires = 
 	pika
 	setuptools
-	stomp.py<6.1.1
+	stomp.py>=7
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.6
 zip_safe = False
 
 [options.entry_points]
```

### Comparing `workflows-2.8/src/workflows/contrib/start_service.py` & `workflows-2.9/src/workflows/contrib/start_service.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/contrib/status_monitor.py` & `workflows-2.9/src/workflows/contrib/status_monitor.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/frontend/__init__.py` & `workflows-2.9/src/workflows/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/frontend/utilization.py` & `workflows-2.9/src/workflows/frontend/utilization.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/logging/__init__.py` & `workflows-2.9/src/workflows/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/recipe/__init__.py` & `workflows-2.9/src/workflows/recipe/__init__.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/recipe/recipe.py` & `workflows-2.9/src/workflows/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/recipe/validate.py` & `workflows-2.9/src/workflows/recipe/validate.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/recipe/wrapper.py` & `workflows-2.9/src/workflows/recipe/wrapper.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/services/__init__.py` & `workflows-2.9/src/workflows/services/__init__.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/services/common_service.py` & `workflows-2.9/src/workflows/services/common_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,18 @@
 
     def __send_to_frontend(self, data_structure):
         """Put a message in the pipe for the frontend."""
         if self.__pipe_frontend:
             self.__pipe_frontend.send(data_structure)
 
     @property
+    def config(self):
+        return self._environment.get("config")
+
+    @property
     def transport(self):
         return self._transport
 
     @transport.setter
     def transport(self, value):
         if self._transport:
             raise AttributeError("Transport already defined")
```

### Comparing `workflows-2.8/src/workflows/services/sample_consumer.py` & `workflows-2.9/src/workflows/services/sample_consumer.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/services/sample_producer.py` & `workflows-2.9/src/workflows/services/sample_producer.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/services/sample_transaction.py` & `workflows-2.9/src/workflows/services/sample_transaction.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/transport/__init__.py` & `workflows-2.9/src/workflows/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/transport/common_transport.py` & `workflows-2.9/src/workflows/transport/common_transport.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/transport/pika_transport.py` & `workflows-2.9/src/workflows/transport/pika_transport.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows/transport/stomp_transport.py` & `workflows-2.9/src/workflows/transport/stomp_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self._connected = False
         self._namespace = ""
         self._idcounter = 0
         self._lock = threading.RLock()
         self._stomp_listener = stomp.listener.ConnectionListener()
         #   self._stomp_listener = stomp.PrintingListener()
         self._stomp_listener.on_message = self._on_message
-        self._stomp_listener.on_before_message = lambda x, y: (x, y)
+        self._stomp_listener.on_before_message = lambda frame: frame
 
     def get_namespace(self):
         """Return the stomp namespace. This is a prefix used for all topic and
         queue names."""
         if self._namespace.endswith("."):
             return self._namespace[:-1]
         return self._namespace
@@ -482,15 +482,17 @@
         try:
             return json.loads(message)
         except (TypeError, ValueError):
             return message
 
     ## Stomp listener methods #####################################################
 
-    def _on_message(self, headers, body):
+    def _on_message(self, frame):
+        headers = frame.headers
+        body = frame.body
         subscription_id = int(headers.get("subscription"))
         target_function = self.subscription_callback(subscription_id)
         if target_function:
             target_function(headers, body)
         else:
             raise workflows.Error(
                 "Unhandled message {} {}".format(repr(headers), repr(body))
```

### Comparing `workflows-2.8/src/workflows/util/zocalo/configuration.py` & `workflows-2.9/src/workflows/util/zocalo/configuration.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows.egg-info/PKG-INFO` & `workflows-2.9/src/workflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: workflows
-Version: 2.8
+Version: 2.9
 Summary: Data processing in distributed environments
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software et al.
 Author-email: scientificsoftware@diamond.ac.uk
 License: BSD
 Project-URL: Download, https://github.com/DiamondLightSource/python-workflows/releases
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-workflows
```

### Comparing `workflows-2.8/src/workflows.egg-info/SOURCES.txt` & `workflows-2.9/src/workflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `workflows-2.8/src/workflows.egg-info/entry_points.txt` & `workflows-2.9/src/workflows.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/contrib/test_start_service.py` & `workflows-2.9/tests/contrib/test_start_service.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/contrib/test_status_monitor.py` & `workflows-2.9/tests/contrib/test_status_monitor.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/frontend/test_frontend.py` & `workflows-2.9/tests/frontend/test_frontend.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/frontend/test_utilization.py` & `workflows-2.9/tests/frontend/test_utilization.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/recipe/test_recipe.py` & `workflows-2.9/tests/recipe/test_recipe.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/recipe/test_validate.py` & `workflows-2.9/tests/recipe/test_validate.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/recipe/test_wrap_subscription.py` & `workflows-2.9/tests/recipe/test_wrap_subscription.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/recipe/test_wrapped_recipe.py` & `workflows-2.9/tests/recipe/test_wrapped_recipe.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/services/test_common_service.py` & `workflows-2.9/tests/services/test_common_service.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/services/test_sample_consumer.py` & `workflows-2.9/tests/services/test_sample_consumer.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/services/test_sample_producer.py` & `workflows-2.9/tests/services/test_sample_producer.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/services/test_sample_transaction.py` & `workflows-2.9/tests/services/test_sample_transaction.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/test_logging.py` & `workflows-2.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/transport/test_common.py` & `workflows-2.9/tests/transport/test_common.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/transport/test_pika.py` & `workflows-2.9/tests/transport/test_pika.py`

 * *Files identical despite different names*

### Comparing `workflows-2.8/tests/transport/test_stomp.py` & `workflows-2.9/tests/transport/test_stomp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 import decimal
 import importlib
 import inspect
 import json
 import optparse
 import os
 import tempfile
+from collections import namedtuple
 from unittest import mock
 
 import pytest
 import stomp as stomppy
 
 import workflows
 import workflows.transport
 from workflows.transport.stomp_transport import StompTransport
 
+_frame = namedtuple("frame", "headers, body")
+
 
 def test_lookup_and_initialize_stomp_transport_layer():
     """Find the stomp transport layer via the lookup mechanism and run
     its constructor with default settings."""
     stomp = workflows.transport.lookup("StompTransport")
     assert stomp == StompTransport
     stomp()
@@ -407,46 +410,50 @@
     mockconn = mockstomp.Connection.return_value
     message_handler = mockconn.set_listener.call_args[0][1].on_message
 
     # Test subscriptions
     callback = mock.Mock()
     stomp.subscribe("channel", callback)
     subscription_id = mockconn.subscribe.call_args[0][1]
-    message_handler({"subscription": subscription_id}, banana_str)
+    message_handler(_frame({"subscription": subscription_id}, banana_str))
     callback.assert_called_once_with({"subscription": subscription_id}, banana)
 
-    message_handler({"subscription": subscription_id}, mock.sentinel.undeserializable)
+    message_handler(
+        _frame({"subscription": subscription_id}, mock.sentinel.undeserializable)
+    )
     callback.assert_called_with(
         {"subscription": subscription_id}, mock.sentinel.undeserializable
     )
 
     # Test broadcast subscriptions
     callback = mock.Mock()
     stomp.subscribe_broadcast("channel", callback)
     subscription_id = mockconn.subscribe.call_args[0][1]
-    message_handler({"subscription": subscription_id}, banana_str)
+    message_handler(_frame({"subscription": subscription_id}, banana_str))
     callback.assert_called_once_with({"subscription": subscription_id}, banana)
 
-    message_handler({"subscription": subscription_id}, mock.sentinel.undeserializable)
+    message_handler(
+        _frame({"subscription": subscription_id}, mock.sentinel.undeserializable)
+    )
     callback.assert_called_with(
         {"subscription": subscription_id}, mock.sentinel.undeserializable
     )
 
     # Test subscriptions with mangling disabled
     callback = mock.Mock()
     stomp.subscribe("channel", callback, disable_mangling=True)
     subscription_id = mockconn.subscribe.call_args[0][1]
-    message_handler({"subscription": subscription_id}, banana_str)
+    message_handler(_frame({"subscription": subscription_id}, banana_str))
     callback.assert_called_once_with({"subscription": subscription_id}, banana_str)
 
     # Test broadcast subscriptions with mangling disabled
     callback = mock.Mock()
     stomp.subscribe_broadcast("channel", callback, disable_mangling=True)
     subscription_id = mockconn.subscribe.call_args[0][1]
-    message_handler({"subscription": subscription_id}, banana_str)
+    message_handler(_frame({"subscription": subscription_id}, banana_str))
     callback.assert_called_once_with({"subscription": subscription_id}, banana_str)
 
 
 @mock.patch("workflows.transport.stomp_transport.stomp")
 def test_subscribe_to_queue(mockstomp):
     """Test subscribing to a queue (producer-consumer), callback functions and unsubscribe."""
     mock_cb1 = mock.Mock()
@@ -504,19 +511,19 @@
             "transformation": "jms-object-json",
             "activemq.priority": 42,
         },
         "ack": "auto",
     }
 
     assert mock_cb1.call_count == 0
-    listener.on_message({"subscription": 1}, mock.sentinel.message1)
+    listener.on_message(_frame({"subscription": 1}, mock.sentinel.message1))
     mock_cb1.assert_called_once_with({"subscription": 1}, mock.sentinel.message1)
 
     assert mock_cb2.call_count == 0
-    listener.on_message({"subscription": 2}, mock.sentinel.message2)
+    listener.on_message(_frame({"subscription": 2}, mock.sentinel.message2))
     mock_cb2.assert_called_once_with({"subscription": 2}, mock.sentinel.message2)
 
     stomp._subscribe(3, str(mock.sentinel.channel3), mock_cb2, acknowledgement=True)
     assert mockconn.subscribe.call_count == 3
     args, kwargs = mockconn.subscribe.call_args
     assert args == ("/queue/" + str(mock.sentinel.channel3), 3)
     assert kwargs == {"headers": {}, "ack": "client-individual"}
@@ -568,19 +575,19 @@
     args, kwargs = mockconn.subscribe.call_args
     assert args == ("/topic/" + str(mock.sentinel.channel2), 2)
     assert kwargs == {
         "headers": {"activemq.retroactive": "true", "transformation": "jms-object-json"}
     }
 
     assert mock_cb1.call_count == 0
-    listener.on_message({"subscription": 1}, mock.sentinel.message1)
+    listener.on_message(_frame({"subscription": 1}, mock.sentinel.message1))
     mock_cb1.assert_called_once_with({"subscription": 1}, mock.sentinel.message1)
 
     assert mock_cb2.call_count == 0
-    listener.on_message({"subscription": 2}, mock.sentinel.message2)
+    listener.on_message(_frame({"subscription": 2}, mock.sentinel.message2))
     mock_cb2.assert_called_once_with({"subscription": 2}, mock.sentinel.message2)
 
     stomp._unsubscribe(1)
     mockconn.unsubscribe.assert_called_once_with(id=1)
     stomp._unsubscribe(2)
     mockconn.unsubscribe.assert_called_with(id=2)
```

