# Comparing `tmp/echobox-1.5.40.tar.gz` & `tmp/echobox-1.5.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echobox-1.5.40.tar", last modified: Fri Mar 15 16:25:02 2024, max compression
+gzip compressed data, was "echobox-1.5.41.tar", last modified: Wed May  1 04:03:52 2024, max compression
```

## Comparing `echobox-1.5.40.tar` & `echobox-1.5.41.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.622026 echobox-1.5.40/
--rw-r--r--   0 qingbao    (501) staff       (20)       43 2023-12-16 14:37:07.000000 echobox-1.5.40/MANIFEST.in
--rw-r--r--   0 qingbao    (501) staff       (20)      618 2024-03-15 16:25:02.621691 echobox-1.5.40/PKG-INFO
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.587609 echobox-1.5.40/echobox/
--rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:27:12.000000 echobox-1.5.40/echobox/__init__.py
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.593391 echobox-1.5.40/echobox/app/
--rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:27:22.000000 echobox-1.5.40/echobox/app/__init__.py
--rw-r--r--   0 qingbao    (501) staff       (20)      585 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/app/appconfig.py
--rw-r--r--   0 qingbao    (501) staff       (20)     8840 2024-03-15 16:23:01.000000 echobox-1.5.40/echobox/app/devops.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1186 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/app/env.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1063 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/app/eventlog.py
--rw-r--r--   0 qingbao    (501) staff       (20)     7531 2023-03-25 10:27:11.000000 echobox-1.5.40/echobox/app/multiuser.py
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.597557 echobox-1.5.40/echobox/clis/
--rwxr-xr-x   0 qingbao    (501) staff       (20)        0 2023-03-25 10:26:24.000000 echobox-1.5.40/echobox/clis/__init__.py
--rw-r--r--   0 qingbao    (501) staff       (20)     3346 2023-03-25 10:27:12.000000 echobox-1.5.40/echobox/clis/mysqlcli.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1362 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/clis/pipcli.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1865 2023-03-25 10:27:12.000000 echobox-1.5.40/echobox/clis/rediscli.py
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.612151 echobox-1.5.40/echobox/tool/
--rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:26:24.000000 echobox-1.5.40/echobox/tool/__init__.py
--rw-r--r--   0 qingbao    (501) staff       (20)     3426 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/aliyunoss.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1464 2023-12-28 16:33:57.000000 echobox-1.5.40/echobox/tool/array.py
--rw-r--r--   0 qingbao    (501) staff       (20)     4355 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/cache.py
--rw-r--r--   0 qingbao    (501) staff       (20)     6134 2023-03-25 10:27:11.000000 echobox-1.5.40/echobox/tool/concurrent.py
--rw-r--r--   0 qingbao    (501) staff       (20)      197 2024-02-11 06:23:40.000000 echobox-1.5.40/echobox/tool/conda.py
--rw-r--r--   0 qingbao    (501) staff       (20)    13664 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/crontab.py
--rw-r--r--   0 qingbao    (501) staff       (20)     4743 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/datatypes.py
--rw-r--r--   0 qingbao    (501) staff       (20)     2338 2023-03-25 10:27:11.000000 echobox-1.5.40/echobox/tool/dockerutil.py
--rw-r--r--   0 qingbao    (501) staff       (20)     3677 2024-03-15 16:23:26.000000 echobox-1.5.40/echobox/tool/file.py
--rw-r--r--   0 qingbao    (501) staff       (20)    13936 2024-02-21 15:52:22.000000 echobox-1.5.40/echobox/tool/functocli.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1100 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/http.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1147 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/local_cache.py
--rw-r--r--   0 qingbao    (501) staff       (20)     8380 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/logger.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1374 2023-12-23 13:56:44.000000 echobox-1.5.40/echobox/tool/net.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1579 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/redistool.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1578 2023-03-25 10:27:12.000000 echobox-1.5.40/echobox/tool/spec.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1393 2023-03-25 10:26:24.000000 echobox-1.5.40/echobox/tool/strings.py
--rw-r--r--   0 qingbao    (501) staff       (20)      210 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/strjson.py
--rw-r--r--   0 qingbao    (501) staff       (20)     2766 2024-02-21 15:52:22.000000 echobox-1.5.40/echobox/tool/system.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1246 2024-02-21 15:51:16.000000 echobox-1.5.40/echobox/tool/systemd.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1604 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/template.py
--rw-r--r--   0 qingbao    (501) staff       (20)      845 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/testutils.py
--rw-r--r--   0 qingbao    (501) staff       (20)      286 2023-12-16 14:37:07.000000 echobox-1.5.40/echobox/tool/timeutil.py
--rw-r--r--   0 qingbao    (501) staff       (20)     3270 2024-03-15 16:22:26.000000 echobox-1.5.40/echobox/tool/utils.py
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.589469 echobox-1.5.40/echobox.egg-info/
--rw-r--r--   0 qingbao    (501) staff       (20)      618 2024-03-15 16:25:01.000000 echobox-1.5.40/echobox.egg-info/PKG-INFO
--rw-r--r--   0 qingbao    (501) staff       (20)     1426 2024-03-15 16:25:01.000000 echobox-1.5.40/echobox.egg-info/SOURCES.txt
--rw-r--r--   0 qingbao    (501) staff       (20)        1 2024-03-15 16:25:01.000000 echobox-1.5.40/echobox.egg-info/dependency_links.txt
--rw-r--r--   0 qingbao    (501) staff       (20)      292 2024-03-15 16:25:01.000000 echobox-1.5.40/echobox.egg-info/requires.txt
--rw-r--r--   0 qingbao    (501) staff       (20)       14 2024-03-15 16:25:01.000000 echobox-1.5.40/echobox.egg-info/top_level.txt
--rw-r--r--   0 qingbao    (501) staff       (20)      387 2023-12-23 13:56:44.000000 echobox-1.5.40/requirements.txt
--rw-r--r--   0 qingbao    (501) staff       (20)       38 2024-03-15 16:25:02.622131 echobox-1.5.40/setup.cfg
--rw-r--r--   0 qingbao    (501) staff       (20)     1149 2024-03-15 16:24:22.000000 echobox-1.5.40/setup.py
-drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-03-15 16:25:02.620901 echobox-1.5.40/tests/
--rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:26:24.000000 echobox-1.5.40/tests/__init__.py
--rw-r--r--   0 qingbao    (501) staff       (20)      714 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_array.py
--rw-r--r--   0 qingbao    (501) staff       (20)     2117 2023-03-25 10:27:11.000000 echobox-1.5.40/tests/test_concurrent.py
--rw-r--r--   0 qingbao    (501) staff       (20)      279 2023-03-25 10:27:12.000000 echobox-1.5.40/tests/test_dockerutil.py
--rw-r--r--   0 qingbao    (501) staff       (20)      521 2023-03-25 10:27:12.000000 echobox-1.5.40/tests/test_eventlog.py
--rw-r--r--   0 qingbao    (501) staff       (20)      957 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_file.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1043 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_functocli.py
--rw-r--r--   0 qingbao    (501) staff       (20)     2370 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_nameiddict.py
--rw-r--r--   0 qingbao    (501) staff       (20)      570 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_net.py
--rw-r--r--   0 qingbao    (501) staff       (20)      379 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_strings.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1001 2024-03-15 16:22:40.000000 echobox-1.5.40/tests/test_system.py
--rw-r--r--   0 qingbao    (501) staff       (20)      953 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_template.py
--rw-r--r--   0 qingbao    (501) staff       (20)      885 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_threadpool.py
--rw-r--r--   0 qingbao    (501) staff       (20)      741 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_timer.py
--rw-r--r--   0 qingbao    (501) staff       (20)     3679 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_tool_cache.py
--rw-r--r--   0 qingbao    (501) staff       (20)     1427 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_tool_redis.py
--rw-r--r--   0 qingbao    (501) staff       (20)      886 2023-12-16 14:37:07.000000 echobox-1.5.40/tests/test_utils.py
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.193551 echobox-1.5.41/
+-rw-r--r--   0 qingbao    (501) staff       (20)       43 2023-12-16 14:37:07.000000 echobox-1.5.41/MANIFEST.in
+-rw-r--r--   0 qingbao    (501) staff       (20)      618 2024-05-01 04:03:52.193132 echobox-1.5.41/PKG-INFO
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.148506 echobox-1.5.41/echobox/
+-rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:27:12.000000 echobox-1.5.41/echobox/__init__.py
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.155189 echobox-1.5.41/echobox/app/
+-rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:27:22.000000 echobox-1.5.41/echobox/app/__init__.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      585 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/app/appconfig.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     8840 2024-03-15 16:23:01.000000 echobox-1.5.41/echobox/app/devops.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1186 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/app/env.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1063 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/app/eventlog.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     7531 2023-03-25 10:27:11.000000 echobox-1.5.41/echobox/app/multiuser.py
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.158122 echobox-1.5.41/echobox/clis/
+-rwxr-xr-x   0 qingbao    (501) staff       (20)        0 2023-03-25 10:26:24.000000 echobox-1.5.41/echobox/clis/__init__.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     3346 2023-03-25 10:27:12.000000 echobox-1.5.41/echobox/clis/mysqlcli.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1362 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/clis/pipcli.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1865 2023-03-25 10:27:12.000000 echobox-1.5.41/echobox/clis/rediscli.py
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.178658 echobox-1.5.41/echobox/tool/
+-rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:26:24.000000 echobox-1.5.41/echobox/tool/__init__.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     3426 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/aliyunoss.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1464 2023-12-28 16:33:57.000000 echobox-1.5.41/echobox/tool/array.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     4355 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/cache.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     6134 2023-03-25 10:27:11.000000 echobox-1.5.41/echobox/tool/concurrent.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      197 2024-02-11 06:23:40.000000 echobox-1.5.41/echobox/tool/conda.py
+-rw-r--r--   0 qingbao    (501) staff       (20)    13664 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/crontab.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     4743 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/datatypes.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     2338 2023-03-25 10:27:11.000000 echobox-1.5.41/echobox/tool/dockerutil.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     3677 2024-03-15 16:23:26.000000 echobox-1.5.41/echobox/tool/file.py
+-rw-r--r--   0 qingbao    (501) staff       (20)    13936 2024-02-21 15:52:22.000000 echobox-1.5.41/echobox/tool/functocli.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1100 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/http.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1147 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/local_cache.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     8380 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/logger.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1374 2023-12-23 13:56:44.000000 echobox-1.5.41/echobox/tool/net.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1579 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/redistool.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1578 2023-03-25 10:27:12.000000 echobox-1.5.41/echobox/tool/spec.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1393 2023-03-25 10:26:24.000000 echobox-1.5.41/echobox/tool/strings.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      210 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/strjson.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     2766 2024-02-21 15:52:22.000000 echobox-1.5.41/echobox/tool/system.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1246 2024-02-21 15:51:16.000000 echobox-1.5.41/echobox/tool/systemd.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1604 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/template.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      845 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/testutils.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      286 2023-12-16 14:37:07.000000 echobox-1.5.41/echobox/tool/timeutil.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     3270 2024-03-15 16:22:26.000000 echobox-1.5.41/echobox/tool/utils.py
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.150783 echobox-1.5.41/echobox.egg-info/
+-rw-r--r--   0 qingbao    (501) staff       (20)      618 2024-05-01 04:03:51.000000 echobox-1.5.41/echobox.egg-info/PKG-INFO
+-rw-r--r--   0 qingbao    (501) staff       (20)     1426 2024-05-01 04:03:51.000000 echobox-1.5.41/echobox.egg-info/SOURCES.txt
+-rw-r--r--   0 qingbao    (501) staff       (20)        1 2024-05-01 04:03:51.000000 echobox-1.5.41/echobox.egg-info/dependency_links.txt
+-rw-r--r--   0 qingbao    (501) staff       (20)      292 2024-05-01 04:03:51.000000 echobox-1.5.41/echobox.egg-info/requires.txt
+-rw-r--r--   0 qingbao    (501) staff       (20)       14 2024-05-01 04:03:51.000000 echobox-1.5.41/echobox.egg-info/top_level.txt
+-rw-r--r--   0 qingbao    (501) staff       (20)      387 2024-05-01 04:00:05.000000 echobox-1.5.41/requirements.txt
+-rw-r--r--   0 qingbao    (501) staff       (20)       38 2024-05-01 04:03:52.193701 echobox-1.5.41/setup.cfg
+-rw-r--r--   0 qingbao    (501) staff       (20)     1149 2024-05-01 04:01:29.000000 echobox-1.5.41/setup.py
+drwxr-xr-x   0 qingbao    (501) staff       (20)        0 2024-05-01 04:03:52.192241 echobox-1.5.41/tests/
+-rw-r--r--   0 qingbao    (501) staff       (20)        0 2023-03-25 10:26:24.000000 echobox-1.5.41/tests/__init__.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      714 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_array.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     2117 2023-03-25 10:27:11.000000 echobox-1.5.41/tests/test_concurrent.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      279 2023-03-25 10:27:12.000000 echobox-1.5.41/tests/test_dockerutil.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      521 2023-03-25 10:27:12.000000 echobox-1.5.41/tests/test_eventlog.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      957 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_file.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1043 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_functocli.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     2370 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_nameiddict.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      570 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_net.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      379 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_strings.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1001 2024-03-15 16:22:40.000000 echobox-1.5.41/tests/test_system.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      953 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_template.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      885 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_threadpool.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      741 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_timer.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     3679 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_tool_cache.py
+-rw-r--r--   0 qingbao    (501) staff       (20)     1427 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_tool_redis.py
+-rw-r--r--   0 qingbao    (501) staff       (20)      886 2023-12-16 14:37:07.000000 echobox-1.5.41/tests/test_utils.py
```

### Comparing `echobox-1.5.40/PKG-INFO` & `echobox-1.5.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echobox
-Version: 1.5.40
+Version: 1.5.41
 Summary: echobox
 Home-page: 
 Author: kiuber
 Author-email: kiuber.zhang@gmail.com
 Keywords: echobox,kiuber
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `echobox-1.5.40/echobox/app/appconfig.py` & `echobox-1.5.41/echobox/app/appconfig.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/app/devops.py` & `echobox-1.5.41/echobox/app/devops.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/app/env.py` & `echobox-1.5.41/echobox/app/env.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/app/eventlog.py` & `echobox-1.5.41/echobox/app/eventlog.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/app/multiuser.py` & `echobox-1.5.41/echobox/app/multiuser.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/clis/mysqlcli.py` & `echobox-1.5.41/echobox/clis/mysqlcli.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/clis/pipcli.py` & `echobox-1.5.41/echobox/clis/pipcli.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/clis/rediscli.py` & `echobox-1.5.41/echobox/clis/rediscli.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/aliyunoss.py` & `echobox-1.5.41/echobox/tool/aliyunoss.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/array.py` & `echobox-1.5.41/echobox/tool/array.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/cache.py` & `echobox-1.5.41/echobox/tool/cache.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/concurrent.py` & `echobox-1.5.41/echobox/tool/concurrent.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/crontab.py` & `echobox-1.5.41/echobox/tool/crontab.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/datatypes.py` & `echobox-1.5.41/echobox/tool/datatypes.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/dockerutil.py` & `echobox-1.5.41/echobox/tool/dockerutil.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/file.py` & `echobox-1.5.41/echobox/tool/file.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/functocli.py` & `echobox-1.5.41/echobox/tool/functocli.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/http.py` & `echobox-1.5.41/echobox/tool/http.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/local_cache.py` & `echobox-1.5.41/echobox/tool/local_cache.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/logger.py` & `echobox-1.5.41/echobox/tool/logger.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/net.py` & `echobox-1.5.41/echobox/tool/net.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/redistool.py` & `echobox-1.5.41/echobox/tool/redistool.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/spec.py` & `echobox-1.5.41/echobox/tool/spec.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/strings.py` & `echobox-1.5.41/echobox/tool/strings.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/system.py` & `echobox-1.5.41/echobox/tool/system.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/systemd.py` & `echobox-1.5.41/echobox/tool/systemd.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/template.py` & `echobox-1.5.41/echobox/tool/template.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/testutils.py` & `echobox-1.5.41/echobox/tool/testutils.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox/tool/utils.py` & `echobox-1.5.41/echobox/tool/utils.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/echobox.egg-info/PKG-INFO` & `echobox-1.5.41/echobox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echobox
-Version: 1.5.40
+Version: 1.5.41
 Summary: echobox
 Home-page: 
 Author: kiuber
 Author-email: kiuber.zhang@gmail.com
 Keywords: echobox,kiuber
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `echobox-1.5.40/echobox.egg-info/SOURCES.txt` & `echobox-1.5.41/echobox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/setup.py` & `echobox-1.5.41/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('requirements.txt', 'r') as f:
     lines = [line.strip() for line in f.readlines()]
 
 install_requires = [line for line in lines if line and not line.startswith('#')]
 
 name = 'echobox'
-version = '1.5.40'
+version = '1.5.41'
 author = 'kiuber'
 author_email = 'kiuber.zhang@gmail.com'
 
 packages = find_packages()
 print(f'packages: {packages}')
 
 setup(
```

### Comparing `echobox-1.5.40/tests/test_array.py` & `echobox-1.5.41/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_concurrent.py` & `echobox-1.5.41/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_eventlog.py` & `echobox-1.5.41/tests/test_eventlog.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_file.py` & `echobox-1.5.41/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_functocli.py` & `echobox-1.5.41/tests/test_functocli.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_nameiddict.py` & `echobox-1.5.41/tests/test_nameiddict.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_net.py` & `echobox-1.5.41/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_system.py` & `echobox-1.5.41/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_template.py` & `echobox-1.5.41/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_threadpool.py` & `echobox-1.5.41/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_timer.py` & `echobox-1.5.41/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_tool_cache.py` & `echobox-1.5.41/tests/test_tool_cache.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_tool_redis.py` & `echobox-1.5.41/tests/test_tool_redis.py`

 * *Files identical despite different names*

### Comparing `echobox-1.5.40/tests/test_utils.py` & `echobox-1.5.41/tests/test_utils.py`

 * *Files identical despite different names*

