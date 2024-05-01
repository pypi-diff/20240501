# Comparing `tmp/spaceone-core-2.0.8.tar.gz` & `tmp/spaceone-core-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-core-2.0.8.tar", last modified: Mon Oct 30 02:03:21 2023, max compression
+gzip compressed data, was "spaceone-core-2.0.9.tar", last modified: Wed Nov  1 08:35:45 2023, max compression
```

## Comparing `spaceone-core-2.0.8.tar` & `spaceone-core-2.0.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.044078 spaceone-core-2.0.8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/auth/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/auth/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/auth/jwt/jwt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/cache/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/cache/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/cache/redis_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/config/default_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/connector/space_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/fastapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/fastapi/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/fastapi/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/fastapi/extension/health.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/fastapi/extension/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/fastapi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/handler/
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/handler/authentication_api_key_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/handler/authentication_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/handler/authorization_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/handler/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/handler/mutation_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/locator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/logger/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/logger/filters/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.048078 spaceone-core-2.0.8/spaceone/core/model/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/model/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/model/mongo_model/
--rw-r--r--   0 runner    (1001) docker     (127)    45629 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/model/mongo_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/model/mongo_model/filter_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/model/mongo_model/stat_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/opentelemetry/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/opentelemetry/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/pygrpc/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/pygrpc/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/extension/grpc_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/extension/server_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/pygrpc/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/queue/redis_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/scheduler/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/scheduler/task_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/scheduler/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/service/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/service/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/info/helloworld_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/interface/grpc/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/interface/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/interface/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/interface/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.052078 spaceone-core-2.0.8/spaceone/core/skeleton/manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/manager/helloworld_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/spaceone/core/skeleton/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/spaceone/core/skeleton/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/skeleton/service/helloworld_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/spaceone/core/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/unittest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/unittest/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/unittest/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2023-10-30 02:03:08.000000 spaceone-core-2.0.8/spaceone/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 02:03:21.056078 spaceone-core-2.0.8/spaceone_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-30 02:03:20.000000 spaceone-core-2.0.8/spaceone_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/auth/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/auth/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/auth/jwt/jwt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/redis_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/config/default_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/connector/space_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/fastapi/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/extension/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/extension/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/authentication_api_key_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/authentication_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/authorization_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/mutation_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/logger/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/model/mongo_model/
+-rw-r--r--   0 runner    (1001) docker     (127)    45629 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/mongo_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/mongo_model/filter_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/mongo_model/stat_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/opentelemetry/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/opentelemetry/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/pygrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/grpc_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/queue/redis_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/service/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/info/helloworld_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/manager/helloworld_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/service/helloworld_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/unittest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/unittest/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/unittest/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/top_level.txt
```

### Comparing `spaceone-core-2.0.8/setup.py` & `spaceone-core-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/auth/jwt/__init__.py` & `spaceone-core-2.0.9/spaceone/core/auth/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/auth/jwt/jwt_util.py` & `spaceone-core-2.0.9/spaceone/core/auth/jwt/jwt_util.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/cache/__init__.py` & `spaceone-core-2.0.9/spaceone/core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/cache/base_cache.py` & `spaceone-core-2.0.9/spaceone/core/cache/base_cache.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/cache/local_cache.py` & `spaceone-core-2.0.9/spaceone/core/cache/local_cache.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/cache/redis_cache.py` & `spaceone-core-2.0.9/spaceone/core/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/command.py` & `spaceone-core-2.0.9/spaceone/core/command.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/config/__init__.py` & `spaceone-core-2.0.9/spaceone/core/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     if package is None:
         raise ValueError(f'Package is undefined.')
 
     global_module = __import__(f'{package}.conf.global_conf', fromlist=['global_conf'])
     for key, value in vars(global_module).items():
         if not key.startswith('__'):
             if key in _GLOBAL:
-                _GLOBAL[key] = utils.deep_merge(value, _GLOBAL[key])
+                if isinstance(value, dict):
+                    _GLOBAL[key] = utils.deep_merge(value, _GLOBAL[key])
+                else:
+                    _GLOBAL[key] = value
             else:
                 _GLOBAL[key] = value
 
 
 def get_global(key=None, default=None):
     if key:
         return copy.deepcopy(_GLOBAL.get(key, default))
```

### Comparing `spaceone-core-2.0.8/spaceone/core/config/default_conf.py` & `spaceone-core-2.0.9/spaceone/core/config/default_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/connector/space_connector.py` & `spaceone-core-2.0.9/spaceone/core/connector/space_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/error.py` & `spaceone-core-2.0.9/spaceone/core/error.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/fastapi/api.py` & `spaceone-core-2.0.9/spaceone/core/fastapi/api.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/fastapi/extension/reflection.py` & `spaceone-core-2.0.9/spaceone/core/fastapi/extension/reflection.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/fastapi/server.py` & `spaceone-core-2.0.9/spaceone/core/fastapi/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/handler/__init__.py` & `spaceone-core-2.0.9/spaceone/core/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/handler/authentication_api_key_handler.py` & `spaceone-core-2.0.9/spaceone/core/handler/authentication_api_key_handler.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/handler/authentication_handler.py` & `spaceone-core-2.0.9/spaceone/core/handler/authentication_handler.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/handler/authorization_handler.py` & `spaceone-core-2.0.9/spaceone/core/handler/authorization_handler.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/handler/event_handler.py` & `spaceone-core-2.0.9/spaceone/core/handler/event_handler.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/handler/mutation_handler.py` & `spaceone-core-2.0.9/spaceone/core/handler/mutation_handler.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/locator.py` & `spaceone-core-2.0.9/spaceone/core/locator.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/logger/__init__.py` & `spaceone-core-2.0.9/spaceone/core/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/logger/filters/masking.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/masking.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/logger/filters/parameter.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/parameter.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/logger/filters/traceback.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/traceback.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/logger/filters/transaction.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/transaction.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/model/base_model.py` & `spaceone-core-2.0.9/spaceone/core/model/base_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/model/mongo_model/__init__.py` & `spaceone-core-2.0.9/spaceone/core/model/mongo_model/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/model/mongo_model/filter_operator.py` & `spaceone-core-2.0.9/spaceone/core/model/mongo_model/filter_operator.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/model/mongo_model/stat_operator.py` & `spaceone-core-2.0.9/spaceone/core/model/mongo_model/stat_operator.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/opentelemetry/metrics.py` & `spaceone-core-2.0.9/spaceone/core/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/opentelemetry/tracer.py` & `spaceone-core-2.0.9/spaceone/core/opentelemetry/tracer.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/pygrpc/api.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/api.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/pygrpc/client.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/client.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/pygrpc/extension/grpc_health.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/extension/grpc_health.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/pygrpc/extension/server_info.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/extension/server_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/pygrpc/message_type.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/message_type.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/pygrpc/server.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/queue/__init__.py` & `spaceone-core-2.0.9/spaceone/core/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/queue/redis_queue.py` & `spaceone-core-2.0.9/spaceone/core/queue/redis_queue.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/scheduler/scheduler.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/scheduler/server.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/scheduler/task_schema.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/task_schema.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/scheduler/worker.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/worker.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/service/service.py` & `spaceone-core-2.0.9/spaceone/core/service/service.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/service/utils.py` & `spaceone-core-2.0.9/spaceone/core/service/utils.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/skeleton/conf/global_conf.py` & `spaceone-core-2.0.9/spaceone/core/skeleton/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/skeleton/interface/grpc/helloworld.py` & `spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/helloworld.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/token.py` & `spaceone-core-2.0.9/spaceone/core/token.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/transaction.py` & `spaceone-core-2.0.9/spaceone/core/transaction.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/unittest/result.py` & `spaceone-core-2.0.9/spaceone/core/unittest/result.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/unittest/runner.py` & `spaceone-core-2.0.9/spaceone/core/unittest/runner.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone/core/utils.py` & `spaceone-core-2.0.9/spaceone/core/utils.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.8/spaceone_core.egg-info/SOURCES.txt` & `spaceone-core-2.0.9/spaceone_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

