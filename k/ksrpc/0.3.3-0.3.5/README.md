# Comparing `tmp/ksrpc-0.3.3.tar.gz` & `tmp/ksrpc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ksrpc-0.3.3.tar", last modified: Fri Mar  3 08:09:02 2023, max compression
+gzip compressed data, was "ksrpc-0.3.5.tar", last modified: Wed May  1 09:32:01 2024, max compression
```

## Comparing `ksrpc-0.3.3.tar` & `ksrpc-0.3.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.757473 ksrpc-0.3.3/
--rw-rw-rw-   0        0        0     1083 2022-05-21 09:04:32.000000 ksrpc-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     6676 2023-03-03 08:09:02.757473 ksrpc-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6133 2023-03-02 11:50:37.000000 ksrpc-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.538288 ksrpc-0.3.3/ksrpc/
--rw-rw-rw-   0        0        0       35 2022-05-17 15:40:11.000000 ksrpc-0.3.3/ksrpc/__init__.py
--rw-rw-rw-   0        0        0       74 2022-06-09 04:23:44.000000 ksrpc-0.3.3/ksrpc/__main__.py
--rw-rw-rw-   0        0        0       23 2023-03-03 07:19:44.000000 ksrpc-0.3.3/ksrpc/_version.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.590065 ksrpc-0.3.3/ksrpc/app/
--rw-rw-rw-   0        0        0        0 2022-05-16 08:39:54.000000 ksrpc-0.3.3/ksrpc/app/__init__.py
--rw-rw-rw-   0        0        0       75 2022-05-26 11:32:45.000000 ksrpc-0.3.3/ksrpc/app/app_.py
--rw-rw-rw-   0        0        0     5123 2022-06-02 06:10:51.000000 ksrpc-0.3.3/ksrpc/app/http_.py
--rw-rw-rw-   0        0        0     7674 2023-03-02 11:22:00.000000 ksrpc-0.3.3/ksrpc/app/websocket_.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 09:33:00.000000 ksrpc-0.3.3/ksrpc/cache.py
--rw-rw-rw-   0        0        0     7978 2023-03-02 11:22:00.000000 ksrpc-0.3.3/ksrpc/caller.py
--rw-rw-rw-   0        0        0     2822 2023-03-02 11:47:28.000000 ksrpc-0.3.3/ksrpc/config.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.612065 ksrpc-0.3.3/ksrpc/connections/
--rw-rw-rw-   0        0        0        0 2022-05-16 08:34:37.000000 ksrpc-0.3.3/ksrpc/connections/__init__.py
--rw-rw-rw-   0        0        0     4459 2022-05-27 10:49:22.000000 ksrpc-0.3.3/ksrpc/connections/http.py
--rw-rw-rw-   0        0        0     7356 2023-03-03 08:00:26.000000 ksrpc-0.3.3/ksrpc/connections/websocket.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.644083 ksrpc-0.3.3/ksrpc/hack/
--rw-rw-rw-   0        0        0      132 2022-05-18 15:35:57.000000 ksrpc-0.3.3/ksrpc/hack/WindPy.py
--rw-rw-rw-   0        0        0      143 2022-05-18 08:15:25.000000 ksrpc-0.3.3/ksrpc/hack/__init__.py
--rw-rw-rw-   0        0        0      792 2022-05-18 11:52:27.000000 ksrpc-0.3.3/ksrpc/hack/jqdatasdk.py
--rw-rw-rw-   0        0        0      881 2022-05-18 08:18:04.000000 ksrpc-0.3.3/ksrpc/hack/rqdatac.py
--rw-rw-rw-   0        0        0      347 2022-05-18 08:18:04.000000 ksrpc-0.3.3/ksrpc/hack/tushare.py
--rw-rw-rw-   0        0        0     1050 2022-05-26 13:06:44.000000 ksrpc-0.3.3/ksrpc/model.py
--rw-rw-rw-   0        0        0     2309 2022-06-03 12:11:47.000000 ksrpc-0.3.3/ksrpc/rpc_client.py
--rw-rw-rw-   0        0        0     2012 2023-03-03 07:51:06.000000 ksrpc-0.3.3/ksrpc/rpc_reverse.py
--rw-rw-rw-   0        0        0      543 2022-06-09 04:24:44.000000 ksrpc-0.3.3/ksrpc/run_app.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.664081 ksrpc-0.3.3/ksrpc/serializer/
--rw-rw-rw-   0        0        0        0 2022-05-16 08:34:37.000000 ksrpc-0.3.3/ksrpc/serializer/__init__.py
--rw-rw-rw-   0        0        0     2882 2022-05-17 03:07:28.000000 ksrpc-0.3.3/ksrpc/serializer/json_.py
--rw-rw-rw-   0        0        0      974 2022-05-17 11:20:59.000000 ksrpc-0.3.3/ksrpc/serializer/pkl_gzip.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.732090 ksrpc-0.3.3/ksrpc/server/
--rw-rw-rw-   0        0        0      963 2022-05-18 16:13:33.000000 ksrpc-0.3.3/ksrpc/server/WindPy.py
--rw-rw-rw-   0        0        0      355 2022-05-25 06:12:28.000000 ksrpc-0.3.3/ksrpc/server/__init__.py
--rw-rw-rw-   0        0        0       85 2022-06-03 14:26:57.000000 ksrpc-0.3.3/ksrpc/server/config.py
--rw-rw-rw-   0        0        0      831 2022-06-03 13:13:32.000000 ksrpc-0.3.3/ksrpc/server/demo.py
--rw-rw-rw-   0        0        0      297 2022-06-03 13:17:31.000000 ksrpc-0.3.3/ksrpc/server/eikon.py
--rw-rw-rw-   0        0        0     1073 2022-06-03 13:04:29.000000 ksrpc-0.3.3/ksrpc/server/jqdatasdk.py
--rw-rw-rw-   0        0        0      828 2022-06-03 13:01:32.000000 ksrpc-0.3.3/ksrpc/server/rqdatac.py
--rw-rw-rw-   0        0        0      630 2022-06-03 13:12:59.000000 ksrpc-0.3.3/ksrpc/server/tushare.py
--rw-rw-rw-   0        0        0      891 2022-06-02 09:38:21.000000 ksrpc-0.3.3/ksrpc/update_quota.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.757473 ksrpc-0.3.3/ksrpc/utils/
--rw-rw-rw-   0        0        0        0 2022-05-16 08:34:37.000000 ksrpc-0.3.3/ksrpc/utils/__init__.py
--rw-rw-rw-   0        0        0     2971 2022-05-26 14:11:20.000000 ksrpc-0.3.3/ksrpc/utils/async_.py
--rw-rw-rw-   0        0        0     1594 2022-06-02 08:35:52.000000 ksrpc-0.3.3/ksrpc/utils/check_.py
--rw-rw-rw-   0        0        0     1794 2022-05-17 09:14:30.000000 ksrpc-0.3.3/ksrpc/utils/date_.py
-drwxrwxrwx   0        0        0        0 2023-03-03 08:09:02.553929 ksrpc-0.3.3/ksrpc.egg-info/
--rw-rw-rw-   0        0        0     6676 2023-03-03 08:09:01.000000 ksrpc-0.3.3/ksrpc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-03-03 08:09:02.000000 ksrpc-0.3.3/ksrpc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 08:09:01.000000 ksrpc-0.3.3/ksrpc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2023-03-03 08:09:01.000000 ksrpc-0.3.3/ksrpc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-03 08:09:01.000000 ksrpc-0.3.3/ksrpc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-03 08:09:02.757473 ksrpc-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-03-02 11:07:14.000000 ksrpc-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.301270 ksrpc-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 09:31:56.000000 ksrpc-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-01 09:32:01.301270 ksrpc-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-01 09:31:56.000000 ksrpc-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.297270 ksrpc-0.3.5/ksrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.297270 ksrpc-0.3.5/ksrpc/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/app/app_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/app/http_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/app/websocket_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/caller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.297270 ksrpc-0.3.5/ksrpc/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/connections/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/connections/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.297270 ksrpc-0.3.5/ksrpc/hack/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/hack/WindPy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/hack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/hack/jqdatasdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/hack/rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/hack/tushare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/rpc_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/run_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.301270 ksrpc-0.3.5/ksrpc/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/serializer/json_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/serializer/pkl_gzip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.301270 ksrpc-0.3.5/ksrpc/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/WindPy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/eikon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/jqdatasdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/server/tushare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/update_quota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.301270 ksrpc-0.3.5/ksrpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/utils/check_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/utils/date_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 09:31:56.000000 ksrpc-0.3.5/ksrpc/utils/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:32:01.301270 ksrpc-0.3.5/ksrpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-01 09:32:01.000000 ksrpc-0.3.5/ksrpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-01 09:32:01.000000 ksrpc-0.3.5/ksrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:32:01.000000 ksrpc-0.3.5/ksrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-01 09:32:01.000000 ksrpc-0.3.5/ksrpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 09:32:01.000000 ksrpc-0.3.5/ksrpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-01 09:31:56.000000 ksrpc-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:32:01.301270 ksrpc-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 09:31:56.000000 ksrpc-0.3.5/setup.py
```

### Comparing `ksrpc-0.3.3/PKG-INFO` & `ksrpc-0.3.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,152 +1,131 @@
-Metadata-Version: 2.1
-Name: ksrpc
-Version: 0.3.3
-Summary: Keep Simple RPC
-Home-page: https://github.com/wukan1986/ksrpc
-Author: wukan
-Author-email: wu-kan@163.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: server
-Provides-Extra: client
-License-File: LICENSE
-
-# ksrpc
-Keep Simple RPC。免注册远程过程调用
-
-## 项目背景
-团队里常常需要通过平台下载各数据，但只有一套账号。通常的方案如下：
-1. 一个账号大家共用。最简单粗暴
-    1. 账号还能登录平台的其它功能，不便于分享
-    2. 账号可能有在线数上限，会导致互踢
-    3. 不同成员可能重复下载相同数据，同一成员也可能反复下载相同数据
-2. 由IT团队将数据提前下载过来。人力成本最高
-    1. IT团队需要提前规划部署，并向研究团队推广
-    2. 不同数据需要IT团队针对性的提前准备下载，时效性一般
-    3. 有些数据只是临时少量需要，需求变化快
-
-如果搭建一套服务，客户端不需账号，基本不用改动代码，是否解决多成员分享问题？所以这个项目就是为了API转发，只是后来发现本质上是RPC
-
-## 目标及特性
-1. 不修改第三方API源代码，实现客户端免登录
-2. 新接口与原接口一致，基本不用改动代码
-3. 数据缓存功能，减少下载次数。针对有数据有限额、调用次数有限制等情况
-4. 跨语言，能将大量Python的数据API转成HTTP服务，由其它语言调用
-5. 既支持同步调用，又支持异步调用
-
-## 应用场景
-1. 数据缓存转发
-2. 源代码保护。核心代码不提供，只向外暴露服务
-3. 远程控制。可调os、sys等库
-
-## 与其它RPC的区别
-1. 免注册就可以向外自动暴露所有API
-    1. 不得不添加函数白名单与黑名单功能
-    2. 添加了简易版的token认证功能
-2. 所有API都自动暴露，但并不是所有API都能正常使用。例如：
-    1. 输入与输出无法序列化和反序列化
-    2. 部分API使用方法特殊，也可能无法使用
-    3. 数据量太大，序列化、网络传输都不太现实
-3. 可先选择不同的通讯方式，目前提供的方式有：HTTP、WebSocket
-4. 出于数据版权保护，默认添加了IP地址校验开关，限制只在内网使用
-5. 多人使用时，少数人超量使用，所以又添加了数据量限额功能
-
-## 服务端安装
-1. 安装`ksrpc`库
-> pip install ksrpc[server] -i https://mirrors.aliyun.com/pypi/simple --upgrade
-2. 直接运行`python -m ksrpc`, 观察提示的`config.py`文件路径
-2. 编辑`config.py`文件，进行`ksrpy`的功能管理。如权限配置等`ENABLE_SERVER = True`
-4. 再次运行`python -m ksrpc`或对应目录下运行`python run_app.py`
-5. 确保服务器上防火墙已经开放对应端口
-
-## 客户端安装
-1. 安装`ksrpc`库
-> pip install ksrpc[client] -i https://mirrors.aliyun.com/pypi/simple --upgrade
-2. 编辑`examples`目录下的`demo_http.py`和`demo_websocket.py`中对应的服务地址
-3. 运行`demo_http.py`和`demo_websocket.py`，检查是否运行正常
-
-## 示例
-1. 直接可替代的。如`tests`目录下的：os、numpy、pandas、akshare等
-    1. 客户端没有安装相应包的情况下，IDE无法自动补全
-2. 需要服务端进行登录等一类处理的。如`server`目录下的，jqdatasdk、tushare、WindPy等
-3. 客户端参数无法序列化，需要特殊处理的。如`hack`目录下的jqdatasdk、WindPy等
-    1. 需要客户端安装第三方库，IDE的自动补全功能正常
-
-```python
-from ksrpc import RpcClient
-from ksrpc.connections.http import HttpxConnection
-
-conn = HttpxConnection('http://127.0.0.1:8000/api/file')
-conn.timeout = None
-math = RpcClient('math', conn, async_local=False)
-math.cache_get = True
-math.cache_expire = 86400
-
-# 模块中变量获取方法。加了括号
-print(math.pi())
-print(math.pow(2, 3))
-```
-
-```python
-# 创建客户连接
-from ksrpc import RpcClient
-from ksrpc.connections.http import HttpxConnection
-
-conn = HttpxConnection('http://127.0.0.1:8000/api/file')
-conn.timeout = None
-client = RpcClient('tushare', conn, async_local=False)
-client.cache_get = True
-client.cache_expire = 86400
-
-# 对原版库进行定制处理，需要已经安装了原版库
-from ksrpc.hack.tushare import hack
-
-hack(client)
-
-# 原版代码可都保持不变
-import tushare as ts
-
-ts.set_token('TUSHARE_TOKEN')
-pro = ts.pro_api()
-df = pro.trade_cal(exchange='', start_date='20210901', end_date='20211231')
-print(df)
-df = pro.daily(ts_code='000001.SZ,600000.SH', start_date='20180701', end_date='20180718')
-print(df)
-```
-
-## 部分支持转发的库
-1. [AkShare](tests/akshare_.py)(已测)
-2. TuShare [方法一](examples/tushare_hack.py) [方法二](examples/tushare_client.py)(已测)
-3. [rqdatac](examples/rqdatac_hack.py)(已测)
-4. [jqdatasdk](examples/jqdatasdk_hack.py)(缺账号，未测)
-5. [Wind](examples/wind_hack.py)(缺账号，未测)
-6. 其它...
-
-## 跨语言开发文档
-跨语言示例代码在`lang`目录下
-[跨语言开发文档](lang/)
-
-## 声明
-此库仅供学习交流，请在数据提供方的授权范围内使用。请勿向第三方转发数据
-
-## 反弹RPC(反向RPC)/中继服务
-如果提供服务的机器在内网，无法搭建服务，也无法直接访问怎么办？参考Reverse Shell的概念，本项目提供了Reverse RPC功能
-1. 公网服务器上安装`pip install ksrpc[server]`，修改配置，运行`python run_app.py`，记下公网IP
-2. 内网服务器上安装`pip install ksrpc`(如果网络受限，可下载whl文件本地安装)，修改`rpc_reverse.py`中为公网IP，运行`python rpc_reverse.py`。此代码可粘贴到Notebook中运行
-3. 观察内网脚本是否能连接公网服务器
-4. 个人电脑上安装`pip install ksrpc[client]`，编辑`examples/demo_reverse.py`中为公网IP，运行，观察结果
-5. 注意地址不同，内网被控端连接公网IP下的`/client`, 个人电脑连接公网IP下的`/admin`，并且要用完全一样的房间号
-6. 默认情况下，`config.py`中的`ENABLE_RELAY = True`已经开启
-
-## 参考项目
-开发到一定阶段后才发现与`rpyc`这个免注册暴露函数的功能类似，大家也可以去学习一下
-https://github.com/tomerfiliba-org/rpyc
-
-
-
+# ksrpc
+Keep Simple RPC。免注册远程过程调用
+
+## 项目背景
+团队里常常需要通过平台下载各数据，但只有一套账号。通常的方案如下：
+1. 一个账号大家共用。最简单粗暴
+    1. 账号还能登录平台的其它功能，不便于分享
+    2. 账号可能有在线数上限，会导致互踢
+    3. 不同成员可能重复下载相同数据，同一成员也可能反复下载相同数据
+2. 由IT团队将数据提前下载过来。人力成本最高
+    1. IT团队需要提前规划部署，并向研究团队推广
+    2. 不同数据需要IT团队针对性的提前准备下载，时效性一般
+    3. 有些数据只是临时少量需要，需求变化快
+
+如果搭建一套服务，客户端不需账号，基本不用改动代码，是否解决多成员分享问题？所以这个项目就是为了API转发，只是后来发现本质上是RPC
+
+## 目标及特性
+1. 不修改第三方API源代码，实现客户端免登录
+2. 新接口与原接口一致，基本不用改动代码
+3. 数据缓存功能，减少下载次数。针对有数据有限额、调用次数有限制等情况
+4. 跨语言，能将大量Python的数据API转成HTTP服务，由其它语言调用
+5. 既支持同步调用，又支持异步调用
+
+## 应用场景
+1. 数据缓存转发
+2. 源代码保护。核心代码不提供，只向外暴露服务
+3. 远程控制。可调os、sys等库
+
+## 与其它RPC的区别
+1. 免注册就可以向外自动暴露所有API
+    1. 不得不添加函数白名单与黑名单功能
+    2. 添加了简易版的token认证功能
+2. 所有API都自动暴露，但并不是所有API都能正常使用。例如：
+    1. 输入与输出无法序列化和反序列化
+    2. 部分API使用方法特殊，也可能无法使用
+    3. 数据量太大，序列化、网络传输都不太现实
+3. 可先选择不同的通讯方式，目前提供的方式有：HTTP、WebSocket
+4. 出于数据版权保护，默认添加了IP地址校验开关，限制只在内网使用
+5. 多人使用时，少数人超量使用，所以又添加了数据量限额功能
+
+## 服务端安装
+1. 安装`ksrpc`库
+> pip install ksrpc[server] -i https://mirrors.aliyun.com/pypi/simple --upgrade
+2. 直接运行`python -m ksrpc`, 观察提示的`config.py`文件路径
+2. 编辑`config.py`文件，进行`ksrpy`的功能管理。如权限配置等`ENABLE_SERVER = True`
+4. 再次运行`python -m ksrpc`或对应目录下运行`python run_app.py`
+5. 确保服务器上防火墙已经开放对应端口
+
+## 客户端安装
+1. 安装`ksrpc`库
+> pip install ksrpc[client] -i https://mirrors.aliyun.com/pypi/simple --upgrade
+2. 编辑`examples`目录下的`demo_http.py`和`demo_websocket.py`中对应的服务地址
+3. 运行`demo_http.py`和`demo_websocket.py`，检查是否运行正常
+
+## 示例
+1. 直接可替代的。如`tests`目录下的：os、numpy、pandas、akshare等
+    1. 客户端没有安装相应包的情况下，IDE无法自动补全
+2. 需要服务端进行登录等一类处理的。如`server`目录下的，jqdatasdk、tushare、WindPy等
+3. 客户端参数无法序列化，需要特殊处理的。如`hack`目录下的jqdatasdk、WindPy等
+    1. 需要客户端安装第三方库，IDE的自动补全功能正常
+
+```python
+from ksrpc import RpcClient
+from ksrpc.connections.http import HttpxConnection
+
+conn = HttpxConnection('http://127.0.0.1:8000/api/file')
+conn.timeout = None
+math = RpcClient('math', conn, async_local=False)
+math.cache_get = True
+math.cache_expire = 86400
+
+# 模块中变量获取方法。加了括号
+print(math.pi())
+print(math.pow(2, 3))
+```
+
+```python
+# 创建客户连接
+from ksrpc import RpcClient
+from ksrpc.connections.http import HttpxConnection
+
+conn = HttpxConnection('http://127.0.0.1:8000/api/file')
+conn.timeout = None
+client = RpcClient('tushare', conn, async_local=False)
+client.cache_get = True
+client.cache_expire = 86400
+
+# 对原版库进行定制处理，需要已经安装了原版库
+from ksrpc.hack.tushare import hack
+
+hack(client)
+
+# 原版代码可都保持不变
+import tushare as ts
+
+ts.set_token('TUSHARE_TOKEN')
+pro = ts.pro_api()
+df = pro.trade_cal(exchange='', start_date='20210901', end_date='20211231')
+print(df)
+df = pro.daily(ts_code='000001.SZ,600000.SH', start_date='20180701', end_date='20180718')
+print(df)
+```
+
+## 部分支持转发的库
+1. [AkShare](tests/akshare_.py)(已测)
+2. TuShare [方法一](examples/tushare_hack.py) [方法二](examples/tushare_client.py)(已测)
+3. [rqdatac](examples/rqdatac_hack.py)(已测)
+4. [jqdatasdk](examples/jqdatasdk_hack.py)(缺账号，未测)
+5. [Wind](examples/wind_hack.py)(缺账号，未测)
+6. 其它...
+
+## 跨语言开发文档
+跨语言示例代码在`lang`目录下
+[跨语言开发文档](lang/)
+
+## 声明
+此库仅供学习交流，请在数据提供方的授权范围内使用。请勿向第三方转发数据
+
+## 反弹RPC(反向RPC)/中继服务
+如果提供服务的机器在内网，无法搭建服务，也无法直接访问怎么办？参考Reverse Shell的概念，本项目提供了Reverse RPC功能
+1. 公网服务器上安装`pip install ksrpc[server]`，修改配置，运行`python run_app.py`，记下公网IP
+2. 内网服务器上安装`pip install ksrpc`(如果网络受限，可下载whl文件本地安装)，修改`rpc_reverse.py`中为公网IP，运行`python rpc_reverse.py`。此代码可粘贴到Notebook中运行
+3. 观察内网脚本是否能连接公网服务器
+4. 个人电脑上安装`pip install ksrpc[client]`，编辑`examples/demo_reverse.py`中为公网IP，运行，观察结果
+5. 注意地址不同，内网被控端连接公网IP下的`/client`, 个人电脑连接公网IP下的`/admin`，并且要用完全一样的房间号
+6. 默认情况下，`config.py`中的`ENABLE_RELAY = True`已经开启
+
+## 参考项目
+开发到一定阶段后才发现与`rpyc`这个免注册暴露函数的功能类似，大家也可以去学习一下
+https://github.com/tomerfiliba-org/rpyc
+
```

### Comparing `ksrpc-0.3.3/ksrpc/app/http_.py` & `ksrpc-0.3.5/ksrpc/app/http_.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-"""
-HTTP服务端
-1. 提交json，返回csv或json。通过浏览器访问，或通过其它语言，可以走此通道
-2. 提交pickle，返回pickle。python语言限定，这种方法更强大
-
-通过FastAPI搭建的服务
-1. 大量使用异步， 所以需要被调用的API也能转成异步，否则会阻塞之后的请求
-2. 其它语言用户请走`/api/get`或`/api/post`
-3. `/api/file`为python内部使用
-
-"""
-from datetime import datetime
-from typing import Dict, Any, List
-
-from fastapi import Query, Body, File, Depends
-from fastapi import status
-from fastapi.requests import Request
-from fastapi.responses import PlainTextResponse, StreamingResponse
-from fastapi.security import OAuth2PasswordBearer
-
-from .app_ import app
-from ..caller import call, before_call
-from ..model import Format, RspModel
-from ..serializer.json_ import obj_to_dict
-from ..serializer.pkl_gzip import deserialize, serialize
-
-oauth2_scheme = OAuth2PasswordBearer(tokenUrl="token", auto_error=False)
-
-
-async def get_current_user(token: str = Depends(oauth2_scheme)):
-    from ..config import AUTH_TOKENS, AUTH_CHECK
-
-    if not AUTH_CHECK:
-        return 'anonymous'
-    return AUTH_TOKENS.get(token, None)
-
-
-@app.get("/api/get")
-async def api_get(request: Request,
-                  func: str = Query(..., min_length=1),
-
-                  fmt: Format = Query(Format.CSV),
-                  cache_get: bool = Query(True), cache_expire: int = Query(86400, lt=86400 * 15),
-                  async_remote: bool = Query(True),
-                  user: str = Depends(get_current_user),
-                  ):
-    """无参数函数。可以通过get发起请求。可在浏览器中直接发起"""
-    return await _do(**locals())
-
-
-@app.post("/api/post")
-async def api_post(request: Request,
-                   args: List[Any] = Body([]),
-                   kwargs: Dict[str, Any] = Body({}),
-
-                   func: str = Query(..., min_length=1),
-
-                   fmt: Format = Query(Format.CSV),
-                   cache_get: bool = Query(True), cache_expire: int = Query(86400, lt=86400 * 15),
-                   async_remote: bool = Query(True),
-                   user: str = Depends(get_current_user),
-                   ):
-    """简单参数函数。可通过post请求，使用body区传json参数。可跨语言。可用Postman发起"""
-    return await _do(**locals())
-
-
-@app.post("/api/file")
-async def api_file(request: Request,
-                   file: bytes = File(...),  # file要写在最前面，否则报错
-
-                   func: str = Query(..., min_length=1),
-
-                   fmt: Format = Query(Format.CSV),
-                   cache_get: bool = Query(True), cache_expire: int = Query(86400, lt=86400 * 15),
-                   async_remote: bool = Query(True),
-                   user: str = Depends(get_current_user),
-                   ):
-    """复杂参数函数。通过文件上传二进制方式。不可跨语言。"""
-    return await _do(**locals(), **deserialize(file))
-
-
-async def _do(request: Request,
-              func: str,
-
-              args: List[Any] = [],
-              kwargs: Dict[str, Any] = {},
-
-              fmt: Format = Format.CSV,
-              cache_get: bool = True, cache_expire: int = 86400,
-              async_remote: bool = True,
-              file: bytes = None,  # 用于兼容文件上传模式，但实际没有使用
-              user: str = None,  # 没有用到，用于token认证
-              ):
-    """实际处理函数"""
-    try:
-        before_call(request.client.host, user, func)
-        key, buf, data = await call(user, func, args, kwargs, cache_get, cache_expire, async_remote)
-    except Exception as e:
-        # 主要是处理
-        key = type(e).__name__
-        # 这里没有缓存，因为这个错误是服务器内部检查
-        data = RspModel(status=status.HTTP_401_UNAUTHORIZED,
-                        datetime=datetime.now().isoformat(),
-                        func=func, args=args, kwargs=kwargs)
-        data.type = type(e).__name__
-        data.data = repr(e)
-        data = data.dict()
-        buf = serialize(data).read()
-
-    # 直接二进制返回
-    if fmt == Format.PKL_GZIP:
-        r = StreamingResponse(iter([buf]), media_type="application/octet-stream")
-        content_disposition = f'attachment; filename="{key}.{Format.PKL_GZIP}"'
-        r.headers.setdefault("content-disposition", content_disposition)
-        return r
-
-    # 从缓存中获取的，但又要转成json等其它功能，需要解码
-    if data is None:
-        data = deserialize(buf)
-
-    # DataFrame需要csv格式时走此路径
-    if fmt == Format.CSV and data['type'] in ('DataFrame', 'Series'):
-        # 指定返回的Content-Type，这样MATLAB的webread可自动识别
-        r = PlainTextResponse(data['data'].to_csv(), media_type="text/csv")
-        return r
-
-    # JSON格式时，为了方便DataFrame的显示，做一下转换
-    data['data'] = obj_to_dict(data['data'])
-
-    return data
+"""
+HTTP服务端
+1. 提交json，返回csv或json。通过浏览器访问，或通过其它语言，可以走此通道
+2. 提交pickle，返回pickle。python语言限定，这种方法更强大
+
+通过FastAPI搭建的服务
+1. 大量使用异步， 所以需要被调用的API也能转成异步，否则会阻塞之后的请求
+2. 其它语言用户请走`/api/get`或`/api/post`
+3. `/api/file`为python内部使用
+
+"""
+from datetime import datetime
+from typing import Dict, Any, List
+
+from fastapi import Query, Body, File, Depends
+from fastapi import status
+from fastapi.requests import Request
+from fastapi.responses import PlainTextResponse, StreamingResponse
+from fastapi.security import OAuth2PasswordBearer
+
+from .app_ import app
+from ..caller import call, before_call
+from ..model import Format, RspModel
+from ..serializer.json_ import obj_to_dict
+from ..serializer.pkl_gzip import deserialize, serialize
+
+oauth2_scheme = OAuth2PasswordBearer(tokenUrl="token", auto_error=False)
+
+
+async def get_current_user(token: str = Depends(oauth2_scheme)):
+    from ..config import AUTH_TOKENS, AUTH_CHECK
+
+    if not AUTH_CHECK:
+        return 'anonymous'
+    return AUTH_TOKENS.get(token, None)
+
+
+@app.get("/api/get")
+async def api_get(request: Request,
+                  func: str = Query(..., min_length=1),
+
+                  fmt: Format = Query(Format.CSV),
+                  cache_get: bool = Query(True), cache_expire: int = Query(86400, lt=86400 * 15),
+                  async_remote: bool = Query(True),
+                  user: str = Depends(get_current_user),
+                  ):
+    """无参数函数。可以通过get发起请求。可在浏览器中直接发起"""
+    return await _do(**locals())
+
+
+@app.post("/api/post")
+async def api_post(request: Request,
+                   args: List[Any] = Body([]),
+                   kwargs: Dict[str, Any] = Body({}),
+
+                   func: str = Query(..., min_length=1),
+
+                   fmt: Format = Query(Format.CSV),
+                   cache_get: bool = Query(True), cache_expire: int = Query(86400, lt=86400 * 15),
+                   async_remote: bool = Query(True),
+                   user: str = Depends(get_current_user),
+                   ):
+    """简单参数函数。可通过post请求，使用body区传json参数。可跨语言。可用Postman发起"""
+    return await _do(**locals())
+
+
+@app.post("/api/file")
+async def api_file(request: Request,
+                   file: bytes = File(...),  # file要写在最前面，否则报错
+
+                   func: str = Query(..., min_length=1),
+
+                   fmt: Format = Query(Format.CSV),
+                   cache_get: bool = Query(True), cache_expire: int = Query(86400, lt=86400 * 15),
+                   async_remote: bool = Query(True),
+                   user: str = Depends(get_current_user),
+                   ):
+    """复杂参数函数。通过文件上传二进制方式。不可跨语言。"""
+    return await _do(**locals(), **deserialize(file))
+
+
+async def _do(request: Request,
+              func: str,
+
+              args: List[Any] = [],
+              kwargs: Dict[str, Any] = {},
+
+              fmt: Format = Format.CSV,
+              cache_get: bool = True, cache_expire: int = 86400,
+              async_remote: bool = True,
+              file: bytes = None,  # 用于兼容文件上传模式，但实际没有使用
+              user: str = None,  # 没有用到，用于token认证
+              ):
+    """实际处理函数"""
+    try:
+        before_call(request.client.host, user, func)
+        key, buf, data = await call(user, func, args, kwargs, cache_get, cache_expire, async_remote)
+    except Exception as e:
+        # 主要是处理
+        key = type(e).__name__
+        # 这里没有缓存，因为这个错误是服务器内部检查
+        data = RspModel(status=status.HTTP_401_UNAUTHORIZED,
+                        datetime=datetime.now().isoformat(),
+                        func=func, args=args, kwargs=kwargs)
+        data.type = type(e).__name__
+        data.data = repr(e)
+        data = data.dict()
+        buf = serialize(data).read()
+
+    # 直接二进制返回
+    if fmt == Format.PKL_GZIP:
+        r = StreamingResponse(iter([buf]), media_type="application/octet-stream")
+        content_disposition = f'attachment; filename="{key}.{Format.PKL_GZIP}"'
+        r.headers.setdefault("content-disposition", content_disposition)
+        return r
+
+    # 从缓存中获取的，但又要转成json等其它功能，需要解码
+    if data is None:
+        data = deserialize(buf)
+
+    # DataFrame需要csv格式时走此路径
+    if fmt == Format.CSV and data['type'] in ('DataFrame', 'Series'):
+        # 指定返回的Content-Type，这样MATLAB的webread可自动识别
+        r = PlainTextResponse(data['data'].to_csv(), media_type="text/csv")
+        return r
+
+    # JSON格式时，为了方便DataFrame的显示，做一下转换
+    data['data'] = obj_to_dict(data['data'])
+
+    return data
```

### Comparing `ksrpc-0.3.3/ksrpc/app/websocket_.py` & `ksrpc-0.3.5/ksrpc/app/websocket_.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-"""
-WebSocket服务器
-1. 提交json格式，返回也json格式。可在浏览器中用JS调用，或通过其它语言访问
-2. 提交pickle格式，返回也json格式。内部调用
-
-使用FastAPI搭建的WebSocket服务
-1. pip install uvicorn[standard], 必须指定stanadard，否则安装后不支持websocket服务
-2. `/ws/json` 可用其它语言调用
-3. `/ws/bytes` 内部调用
-4. `/ws/client` `/ws/amdin`, 反弹RPC
-
-反向RPC时偶尔出现无响应的情况，应当是大数据量时导致的不稳定，所以自己实现了分片功能
-"""
-from datetime import datetime
-from typing import List, Any, Dict, Union
-
-from IPy import IP
-from fastapi import WebSocket, WebSocketDisconnect, Depends, Query
-from fastapi import status
-from fastapi.security.utils import get_authorization_scheme_param
-from loguru import logger
-
-from .app_ import app
-from ..caller import call, before_call
-from ..config import IP_BLOCK, IP_ALLOW, ENABLE_RELAY
-from ..model import Format, RspModel
-from ..serializer.json_ import obj_to_dict, dict_to_json
-from ..serializer.pkl_gzip import deserialize, serialize
-from ..utils.check_ import check_ip
-
-# 二进制拆包
-BYTES_PER_SEND = 1024 * 32
-
-
-async def get_current_user(ws: WebSocket, token: Union[str, None] = Query(None)):
-    from ..config import AUTH_CHECK, AUTH_TOKENS
-    if not AUTH_CHECK:
-        return 'anonymous'
-    authorization: str = ws.headers.get("Authorization")
-    scheme, param = get_authorization_scheme_param(authorization)
-    # 如果从头取不到token就从query中取
-    if param:
-        token = param
-    return AUTH_TOKENS.get(token, None)
-
-
-class ConnectionManager:
-    def __init__(self):
-        self.active_connections: List[WebSocket] = []
-
-    async def connect(self, ws: WebSocket):
-        await ws.accept()
-        self.active_connections.append(ws)
-
-    def disconnect(self, ws: WebSocket):
-        self.active_connections.remove(ws)
-
-    @staticmethod
-    async def send_personal_message(message: str, ws: WebSocket):
-        await ws.send_text(message)
-
-    async def broadcast(self, message: str):
-        for connection in self.active_connections:
-            await connection.send_text(message)
-
-
-manager = ConnectionManager()
-
-
-async def _do(ws: WebSocket,
-              func: str,
-
-              args: List[Any] = [],
-              kwargs: Dict[str, Any] = {},
-              fmt: Format = Format.JSON,
-              cache_get: bool = True, cache_expire: int = 86400,
-              async_remote: bool = True,
-              user: str = None,  # 没有用到，用于token认证
-              ):
-    """实际处理函数"""
-    try:
-        before_call(ws.client.host, user, func)
-        key, buf, data = await call(user, func, args, kwargs, cache_get, cache_expire, async_remote)
-    except Exception as e:
-        # 主要是处理
-        key = type(e).__name__
-        # 这里没有缓存，因为这个错误是服务器内部检查
-        data = RspModel(status=status.HTTP_401_UNAUTHORIZED,
-                        datetime=datetime.now().isoformat(),
-                        func=func, args=args, kwargs=kwargs)
-        data.type = type(e).__name__
-        data.data = repr(e)
-        data = data.dict()
-        buf = serialize(data).read()
-
-    if fmt == Format.PKL_GZIP:
-        return buf
-
-    if data is None:
-        data = deserialize(buf)
-
-    # DataFrame需要csv格式时走此路径
-    if fmt == Format.CSV and data['type'] in ('DataFrame', 'Series'):
-        return data['data'].to_csv()
-
-    # JSON格式时，为了方便DataFrame的显示，做一下转换
-    data['data'] = obj_to_dict(data['data'])
-
-    return data
-
-
-@app.websocket("/ws/json")
-async def websocket_endpoint_json(websocket: WebSocket, user=Depends(get_current_user)):
-    """处理JSON，发送JSON或csv"""
-    await manager.connect(websocket)
-    try:
-        while True:
-            req = await websocket.receive_json(mode="text")
-            logger.info(req)
-            rsp = await _do(websocket, **req, user=user)
-            # 部分类型换转json有问题，所以使用特殊的转换函数
-            await websocket.send_text(dict_to_json(rsp))
-    except WebSocketDisconnect:
-        manager.disconnect(websocket)
-
-
-@app.websocket("/ws/bytes")
-async def websocket_endpoint_bytes(websocket: WebSocket, user=Depends(get_current_user)):
-    """处理pkl.gz发送pkl.gz"""
-    await manager.connect(websocket)
-    try:
-        while True:
-            req = await websocket.receive_bytes()
-            bl = deserialize(req)
-            req = b''
-            while len(req) < bl:
-                req += await websocket.receive_bytes()
-            req = deserialize(req)
-            logger.info(req)
-            req['fmt'] = Format.PKL_GZIP
-            b = await _do(websocket, **req, user=user)
-            bl = len(b)
-            await websocket.send_bytes(serialize(bl).read())
-            for i in range(0, len(b), BYTES_PER_SEND):
-                await websocket.send_bytes(b[i:i + BYTES_PER_SEND])
-
-    except WebSocketDisconnect:
-        manager.disconnect(websocket)
-
-
-# 房间，分存客户端和管理端，中转时用于查找对应的ws
-rooms_client: Dict[str, WebSocket] = {}
-rooms_admin: Dict[str, WebSocket] = {}
-
-
-@app.websocket("/ws/client")
-async def websocket_endpoint_client(websocket: WebSocket, room: str, user=Depends(get_current_user)):
-    """被控端。肉鸡接入后，等待控制端接入，然后转发到肉鸡，然后转发。必须要进入同一房间"""
-    await manager.connect(websocket)
-    try:
-        if not ENABLE_RELAY:
-            raise Exception(f'Relay offline')
-
-        if user is None:
-            raise Exception(f"Unauthorized")
-
-        rooms_client[room] = websocket
-        while True:
-            req = await websocket.receive_bytes()
-            # 可以将被控端的二进制解码，然后转成json，实现跨语言，这里先不处理
-            await rooms_admin[room].send_bytes(req)
-
-    except WebSocketDisconnect:
-        manager.disconnect(websocket)
-    except Exception as e:
-        logger.error(e)
-        manager.disconnect(websocket)
-        await websocket.close()
-
-
-# 两张清单数据提前处理，加快处理速度
-__IP_ALLOW__ = {IP(k): v for k, v in IP_ALLOW.items()}
-__IP_BLOCK__ = {IP(k): v for k, v in IP_BLOCK.items()}
-
-
-@app.websocket("/ws/admin")
-async def websocket_endpoint_admin(websocket: WebSocket, room: str, user=Depends(get_current_user)):
-    """控制端。等待控制端接入，然后转发"""
-    await manager.connect(websocket)
-    try:
-        # 确保连上admin的用户有权限
-        from ..config import IP_CHECK
-
-        if not ENABLE_RELAY:
-            raise Exception(f'Relay offline')
-
-        if IP_CHECK:
-            host = IP(websocket.client.host)
-            if not check_ip(__IP_ALLOW__, host, False):
-                raise Exception(f'IP Not Allowed, {host} not in allowlist')
-            if not check_ip(__IP_BLOCK__, host, True):
-                raise Exception(f'IP Not Allowed, {host} in blocklist')
-
-        if user is None:
-            raise Exception(f"Unauthorized")
-
-        rooms_admin[room] = websocket
-        while True:
-            req = await websocket.receive_bytes()
-            await rooms_client[room].send_bytes(req)
-
-    except WebSocketDisconnect:
-        manager.disconnect(websocket)
-    except Exception as e:
-        logger.error(e)
-        manager.disconnect(websocket)
-        await websocket.close()
+"""
+WebSocket服务器
+1. 提交json格式，返回也json格式。可在浏览器中用JS调用，或通过其它语言访问
+2. 提交pickle格式，返回也json格式。内部调用
+
+使用FastAPI搭建的WebSocket服务
+1. pip install uvicorn[standard], 必须指定stanadard，否则安装后不支持websocket服务
+2. `/ws/json` 可用其它语言调用
+3. `/ws/bytes` 内部调用
+4. `/ws/client` `/ws/amdin`, 反弹RPC
+
+反向RPC时偶尔出现无响应的情况，应当是大数据量时导致的不稳定，所以自己实现了分片功能
+"""
+from datetime import datetime
+from typing import List, Any, Dict, Union
+
+from IPy import IP
+from fastapi import WebSocket, WebSocketDisconnect, Depends, Query
+from fastapi import status
+from fastapi.security.utils import get_authorization_scheme_param
+from loguru import logger
+
+from .app_ import app
+from ..caller import call, before_call
+from ..config import IP_BLOCK, IP_ALLOW, ENABLE_RELAY
+from ..model import Format, RspModel
+from ..serializer.json_ import obj_to_dict, dict_to_json
+from ..serializer.pkl_gzip import deserialize, serialize
+from ..utils.check_ import check_ip
+
+# 二进制拆包
+BYTES_PER_SEND = 1024 * 32
+
+
+async def get_current_user(ws: WebSocket, token: Union[str, None] = Query(None)):
+    from ..config import AUTH_CHECK, AUTH_TOKENS
+    if not AUTH_CHECK:
+        return 'anonymous'
+    authorization: str = ws.headers.get("Authorization")
+    scheme, param = get_authorization_scheme_param(authorization)
+    # 如果从头取不到token就从query中取
+    if param:
+        token = param
+    return AUTH_TOKENS.get(token, None)
+
+
+class ConnectionManager:
+    def __init__(self):
+        self.active_connections: List[WebSocket] = []
+
+    async def connect(self, ws: WebSocket):
+        await ws.accept()
+        self.active_connections.append(ws)
+
+    def disconnect(self, ws: WebSocket):
+        self.active_connections.remove(ws)
+
+    @staticmethod
+    async def send_personal_message(message: str, ws: WebSocket):
+        await ws.send_text(message)
+
+    async def broadcast(self, message: str):
+        for connection in self.active_connections:
+            await connection.send_text(message)
+
+
+manager = ConnectionManager()
+
+
+async def _do(ws: WebSocket,
+              func: str,
+
+              args: List[Any] = [],
+              kwargs: Dict[str, Any] = {},
+              fmt: Format = Format.JSON,
+              cache_get: bool = True, cache_expire: int = 86400,
+              async_remote: bool = True,
+              user: str = None,  # 没有用到，用于token认证
+              ):
+    """实际处理函数"""
+    try:
+        before_call(ws.client.host, user, func)
+        key, buf, data = await call(user, func, args, kwargs, cache_get, cache_expire, async_remote)
+    except Exception as e:
+        # 主要是处理
+        key = type(e).__name__
+        # 这里没有缓存，因为这个错误是服务器内部检查
+        data = RspModel(status=status.HTTP_401_UNAUTHORIZED,
+                        datetime=datetime.now().isoformat(),
+                        func=func, args=args, kwargs=kwargs)
+        data.type = type(e).__name__
+        data.data = repr(e)
+        data = data.dict()
+        buf = serialize(data).read()
+
+    if fmt == Format.PKL_GZIP:
+        return buf
+
+    if data is None:
+        data = deserialize(buf)
+
+    # DataFrame需要csv格式时走此路径
+    if fmt == Format.CSV and data['type'] in ('DataFrame', 'Series'):
+        return data['data'].to_csv()
+
+    # JSON格式时，为了方便DataFrame的显示，做一下转换
+    data['data'] = obj_to_dict(data['data'])
+
+    return data
+
+
+@app.websocket("/ws/json")
+async def websocket_endpoint_json(websocket: WebSocket, user=Depends(get_current_user)):
+    """处理JSON，发送JSON或csv"""
+    await manager.connect(websocket)
+    try:
+        while True:
+            req = await websocket.receive_json(mode="text")
+            logger.info(req)
+            rsp = await _do(websocket, **req, user=user)
+            # 部分类型换转json有问题，所以使用特殊的转换函数
+            await websocket.send_text(dict_to_json(rsp))
+    except WebSocketDisconnect:
+        manager.disconnect(websocket)
+
+
+@app.websocket("/ws/bytes")
+async def websocket_endpoint_bytes(websocket: WebSocket, user=Depends(get_current_user)):
+    """处理pkl.gz发送pkl.gz"""
+    await manager.connect(websocket)
+    try:
+        while True:
+            req = await websocket.receive_bytes()
+            bl = deserialize(req)
+            req = b''
+            while len(req) < bl:
+                req += await websocket.receive_bytes()
+            req = deserialize(req)
+            logger.info(req)
+            req['fmt'] = Format.PKL_GZIP
+            b = await _do(websocket, **req, user=user)
+            bl = len(b)
+            await websocket.send_bytes(serialize(bl).read())
+            for i in range(0, len(b), BYTES_PER_SEND):
+                await websocket.send_bytes(b[i:i + BYTES_PER_SEND])
+
+    except WebSocketDisconnect:
+        manager.disconnect(websocket)
+
+
+# 房间，分存客户端和管理端，中转时用于查找对应的ws
+rooms_client: Dict[str, WebSocket] = {}
+rooms_admin: Dict[str, WebSocket] = {}
+
+
+@app.websocket("/ws/client")
+async def websocket_endpoint_client(websocket: WebSocket, room: str, user=Depends(get_current_user)):
+    """被控端。肉鸡接入后，等待控制端接入，然后转发到肉鸡，然后转发。必须要进入同一房间"""
+    await manager.connect(websocket)
+    try:
+        if not ENABLE_RELAY:
+            raise Exception(f'Relay offline')
+
+        if user is None:
+            raise Exception(f"Unauthorized")
+
+        rooms_client[room] = websocket
+        while True:
+            req = await websocket.receive_bytes()
+            # 可以将被控端的二进制解码，然后转成json，实现跨语言，这里先不处理
+            await rooms_admin[room].send_bytes(req)
+
+    except WebSocketDisconnect:
+        manager.disconnect(websocket)
+    except Exception as e:
+        logger.error(e)
+        manager.disconnect(websocket)
+        await websocket.close()
+
+
+# 两张清单数据提前处理，加快处理速度
+__IP_ALLOW__ = {IP(k): v for k, v in IP_ALLOW.items()}
+__IP_BLOCK__ = {IP(k): v for k, v in IP_BLOCK.items()}
+
+
+@app.websocket("/ws/admin")
+async def websocket_endpoint_admin(websocket: WebSocket, room: str, user=Depends(get_current_user)):
+    """控制端。等待控制端接入，然后转发"""
+    await manager.connect(websocket)
+    try:
+        # 确保连上admin的用户有权限
+        from ..config import IP_CHECK
+
+        if not ENABLE_RELAY:
+            raise Exception(f'Relay offline')
+
+        if IP_CHECK:
+            host = IP(websocket.client.host)
+            if not check_ip(__IP_ALLOW__, host, False):
+                raise Exception(f'IP Not Allowed, {host} not in allowlist')
+            if not check_ip(__IP_BLOCK__, host, True):
+                raise Exception(f'IP Not Allowed, {host} in blocklist')
+
+        if user is None:
+            raise Exception(f"Unauthorized")
+
+        rooms_admin[room] = websocket
+        while True:
+            req = await websocket.receive_bytes()
+            await rooms_client[room].send_bytes(req)
+
+    except WebSocketDisconnect:
+        manager.disconnect(websocket)
+    except Exception as e:
+        logger.error(e)
+        manager.disconnect(websocket)
+        await websocket.close()
```

### Comparing `ksrpc-0.3.3/ksrpc/cache.py` & `ksrpc-0.3.5/ksrpc/cache.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-05-15
-"""
-缓存
-将查询的结果缓存起来，减少对外部数据源的压力，减少限额消耗
-"""
-from .config import CACHE_TYPE
-
-# 测试时使用的内存redis
-if CACHE_TYPE == 'fakeredis':
-    import fakeredis
-
-    cache = fakeredis.FakeStrictRedis()
-    cache_is_async = False
-
-# 异步版Redis
-if CACHE_TYPE == 'aioredis':
-    import aioredis
-    from .config import REDIS_URL
-
-    cache = aioredis.StrictRedis.from_url(REDIS_URL)
-    cache_is_async = True
-
-
-async def async_cache_get(name):
-    """统一缓存读取方式"""
-    if cache_is_async:
-        return await cache.get(name)
-    # 阻塞方式调用
-    return cache.get(name)
-
-
-async def async_cache_setex(name, time, value):
-    """统一缓存写入方式"""
-    if cache_is_async:
-        return await cache.setex(name, time, value)
-    # 阻塞方式调用
-    cache.setex(name, time, value)
-
-
-async def async_cache_incrby(name, amount):
-    """统一缓存写入方式"""
-    if cache_is_async:
-        return await cache.incrby(name, amount)
-    # 阻塞方式调用
-    cache.incrby(name, amount)
-
-
-async def async_cache_decrby(name, amount):
-    """统一缓存写入方式"""
-    if cache_is_async:
-        return await cache.decrby(name, amount)
-    # 阻塞方式调用
-    cache.decrby(name, amount)
-
-
-async def async_cache_keys(pattern):
-    """统一缓存读取方式"""
-    if cache_is_async:
-        return await cache.keys(pattern)
-    # 阻塞方式调用
-    return cache.keys(pattern)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-05-15
+"""
+缓存
+将查询的结果缓存起来，减少对外部数据源的压力，减少限额消耗
+"""
+from .config import CACHE_TYPE
+
+# 测试时使用的内存redis
+if CACHE_TYPE == 'fakeredis':
+    import fakeredis
+
+    cache = fakeredis.FakeStrictRedis()
+    cache_is_async = False
+
+# 异步版Redis
+if CACHE_TYPE == 'aioredis':
+    import aioredis
+    from .config import REDIS_URL
+
+    cache = aioredis.StrictRedis.from_url(REDIS_URL)
+    cache_is_async = True
+
+
+async def async_cache_get(name):
+    """统一缓存读取方式"""
+    if cache_is_async:
+        return await cache.get(name)
+    # 阻塞方式调用
+    return cache.get(name)
+
+
+async def async_cache_setex(name, time, value):
+    """统一缓存写入方式"""
+    if cache_is_async:
+        return await cache.setex(name, time, value)
+    # 阻塞方式调用
+    cache.setex(name, time, value)
+
+
+async def async_cache_incrby(name, amount):
+    """统一缓存写入方式"""
+    if cache_is_async:
+        return await cache.incrby(name, amount)
+    # 阻塞方式调用
+    cache.incrby(name, amount)
+
+
+async def async_cache_decrby(name, amount):
+    """统一缓存写入方式"""
+    if cache_is_async:
+        return await cache.decrby(name, amount)
+    # 阻塞方式调用
+    cache.decrby(name, amount)
+
+
+async def async_cache_keys(pattern):
+    """统一缓存读取方式"""
+    if cache_is_async:
+        return await cache.keys(pattern)
+    # 阻塞方式调用
+    return cache.keys(pattern)
```

### Comparing `ksrpc-0.3.3/ksrpc/caller.py` & `ksrpc-0.3.5/ksrpc/caller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-05-09
-"""
-调用器
-根据指定参数，调用，并返回结果
-"""
-
-import hashlib
-from datetime import datetime
-
-import numpy as np
-import pandas as pd
-# from fastapi import status
-from IPy import IP
-from loguru import logger
-
-from .cache import async_cache_get, async_cache_setex, async_cache_incrby
-from .config import QUOTA_CHECK, IP_ALLOW, IP_BLOCK, IP_CHECK, METHODS_CHECK, ENABLE_SERVER
-from .model import RspModel
-from .serializer.pkl_gzip import serialize
-from .utils.async_ import to_async, to_sync
-from .utils.check_ import check_methods, check_ip, get_quota
-
-
-def make_key(func, args, kwargs):
-    """生成缓存key"""
-    args_kwargs = f'{repr(args)}_{repr(kwargs)}'
-    if len(args_kwargs) > 32:
-        args_kwargs = hashlib.md5(args_kwargs.encode('utf-8')).hexdigest()
-    return f'{func}_{args_kwargs}'
-
-
-# 两张清单数据提前处理，加快处理速度
-__IP_ALLOW__ = {IP(k): v for k, v in IP_ALLOW.items()}
-__IP_BLOCK__ = {IP(k): v for k, v in IP_BLOCK.items()}
-
-
-def before_call(host, user, func):
-    """调用前的检查"""
-    from .config import (
-        METHODS_ALLOW, METHODS_BLOCK,
-    )
-
-    if not ENABLE_SERVER:
-        raise Exception(f'Service offline')
-
-    if IP_CHECK:
-        host = IP(host)
-        if not check_ip(__IP_ALLOW__, host, False):
-            raise Exception(f'IP Not Allowed, {host} not in allowlist')
-        if not check_ip(__IP_BLOCK__, host, True):
-            raise Exception(f'IP Not Allowed, {host} in blocklist')
-
-    if user is None:
-        raise Exception(f"Unauthorized")
-
-    methods = func.split('.')
-
-    if METHODS_CHECK:
-        if not check_methods(METHODS_ALLOW, methods, False):
-            raise Exception(f'Method Not Allowed, {func} not in allowlist')
-        if not check_methods(METHODS_BLOCK, methods, True):
-            raise Exception(f'Method Not Allowed, {func} in blocklist')
-
-
-async def call(user, func, args, kwargs, cache_get, cache_expire, async_remote, fmt=None):
-    try:
-        buf = None
-        data = None  # None表示从缓存中取的，需要其它格式时需要转换
-        # cache所用的key
-        key = make_key(func, args, kwargs)
-
-        if cache_get:
-            # 优先取缓存
-            buf = await async_cache_get(key)
-        if buf is None:
-            cache_expire, buf, data = await _call(user, func, args, kwargs, cache_expire, async_remote)
-
-            # 过短的缓存时间没有必要
-            if cache_expire >= 30:
-                # 就算强行去查询数据，也会想办法存下，再次取时还能从缓存中取
-                await async_cache_setex(key, cache_expire, buf)
-                logger.info(f'To cache: expire:{cache_expire}\tlen:{len(buf)}\t{key}')
-        else:
-            logger.info(f'From cache: {func}\t{args}\t{kwargs}')
-
-    except Exception as e:
-        key = type(e).__name__
-        # 这里没有缓存，因为这个错误是服务器内部检查
-        data = RspModel(status=403,  # status.HTTP_403_FORBIDDEN,
-                        datetime=datetime.now().isoformat(),
-                        func=func, args=args, kwargs=kwargs)
-        data.type = type(e).__name__
-        data.data = repr(e)
-        data = data.dict()
-        buf = serialize(data).read()
-
-    return key, buf, data
-
-
-async def _call(user, func_name, args, kwargs, cache_expire, async_remote):
-    """进行实际调用
-
-    将配额计算放在调用第三方代码时，优化用户体验
-    """
-
-    methods = func_name.split('.')
-    module = methods[0]
-
-    m_quota_key = f'QUOTA/{user}/{module}'
-    f_quota_key = f'QUOTA/{user}/{func_name}'
-    if QUOTA_CHECK:
-        # 配额检查
-        from .config import QUOTA_MODULE, QUOTA_MODULE_DEFAULT, QUOTA_FUNC, QUOTA_FUNC_DEFAULT
-
-        m_quota = int(await async_cache_get(m_quota_key) or 0)
-        f_quota = int(await async_cache_get(f_quota_key) or 0)
-        quota = get_quota(QUOTA_FUNC, methods, QUOTA_FUNC_DEFAULT)
-        if f_quota > quota:
-            raise Exception(f'Over quota: user:{user}, {func_name}:{f_quota}>{quota}')
-        quota = get_quota(QUOTA_MODULE, [module], QUOTA_MODULE_DEFAULT)
-        if m_quota > quota:
-            raise Exception(f'Over quota: user:{user}, {module}:{quota}')
-
-    try:
-        # 当前server目录下文件，用于特别处理
-        api = __import__(f'{__package__}.server.{module}', fromlist=['*'])
-    except ModuleNotFoundError as e:
-        # 导入系统包
-        if module == __package__:
-            raise Exception(f'Not Allowed to call {__package__}')
-        api = __import__(module, fromlist=['*'])
-
-    # 返回的数据包
-    d = RspModel(status=200,  # status.HTTP_200_OK,
-                 datetime=datetime.now().isoformat(),  # 加查询时间，缓存中也许可以判断是否过期
-                 func=func_name,
-                 args=args,
-                 kwargs=kwargs)
-
-    methods = methods[1:]
-    try:
-        # 转成字符串，后面可能于做cache的key
-        logger.info(f'Call: {func_name}\t{args}\t{kwargs}'[:200])
-
-        func = api
-        for method in methods:
-            func = getattr(func, method)
-
-        # 可以调用的属性
-        if callable(func):
-            # 例如os.remove
-            type_ = 'function'
-            if async_remote:
-                func = await to_async(func)(*args, **kwargs)
-            else:
-                func = to_sync(func)(*args, **kwargs)
-
-        # 结果的类型名
-        class_name = func.__class__.__name__
-
-        # 不可调用的直接返回
-        if class_name == 'module':
-            # 例如os.path，但用法为os.path()
-            data = repr(func)
-            cache_expire = min(cache_expire, 0)
-        elif class_name in ('dict_keys', 'dict_values'):
-            # 无法序列化，只能强行转换
-            # 例如：sys.modules.keys(), 也可以sys.modules.keys.__list()
-            data = list(func)
-            cache_expire = min(cache_expire, 0)
-        else:
-            # 例如math.pi，但用法math.pi()
-            data = func
-
-            if QUOTA_CHECK:
-                # 模块和函数都进行配额统计，是按行记（聚宽），按单元格记（万得），还是按调用次数记？
-                if isinstance(data, (pd.DataFrame, pd.Series, np.ndarray, list)):
-                    # # 按调用次数
-                    # await async_cache_incrby(m_quota_key, 1)
-                    # await async_cache_incrby(f_quota_key, 1)
-
-                    # 按行统计
-                    await async_cache_incrby(m_quota_key, len(data))
-                    await async_cache_incrby(f_quota_key, len(data))
-
-                    # # 按单元格统计
-                    # if hasattr(data, 'size'):
-                    #     await async_cache_incrby(m_quota_key, data.size)
-                    #     await async_cache_incrby(f_quota_key, data.size)
-                    # else:
-                    #     await async_cache_incrby(m_quota_key, len(data))
-                    #     await async_cache_incrby(f_quota_key, len(data))
-
-        d.type = type(func).__name__
-        d.data = data
-
-        # pkl序列化，为了能完整还源
-        d = d.dict()
-        buf = serialize(d).read()
-
-    except Exception as e:
-        d.status = 500  # status.HTTP_500_INTERNAL_SERVER_ERROR
-        d.type = type(e).__name__
-        d.data = repr(e)
-        # 错误也缓存一会，防止用户写了死循环搞崩上游
-        cache_expire = min(cache_expire, 60)
-        d = d.dict()
-        # 由于错误信息也想缓存，所以这里进行编码
-        buf = serialize(d).read()
-
-    return cache_expire, buf, d
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-05-09
+"""
+调用器
+根据指定参数，调用，并返回结果
+"""
+
+import hashlib
+from datetime import datetime
+
+import numpy as np
+import pandas as pd
+# from fastapi import status
+from IPy import IP
+from loguru import logger
+from revolving_asyncio import to_async, to_sync
+
+from .cache import async_cache_get, async_cache_setex, async_cache_incrby
+from .config import QUOTA_CHECK, IP_ALLOW, IP_BLOCK, IP_CHECK, METHODS_CHECK, ENABLE_SERVER
+from .model import RspModel
+from .serializer.pkl_gzip import serialize
+from .utils.check_ import check_methods, check_ip, get_quota
+
+
+def make_key(func, args, kwargs):
+    """生成缓存key"""
+    args_kwargs = f'{repr(args)}_{repr(kwargs)}'
+    if len(args_kwargs) > 32:
+        args_kwargs = hashlib.md5(args_kwargs.encode('utf-8')).hexdigest()
+    return f'{func}_{args_kwargs}'
+
+
+# 两张清单数据提前处理，加快处理速度
+__IP_ALLOW__ = {IP(k): v for k, v in IP_ALLOW.items()}
+__IP_BLOCK__ = {IP(k): v for k, v in IP_BLOCK.items()}
+
+
+def before_call(host, user, func):
+    """调用前的检查"""
+    from .config import (
+        METHODS_ALLOW, METHODS_BLOCK,
+    )
+
+    if not ENABLE_SERVER:
+        raise Exception(f'Service offline')
+
+    if IP_CHECK:
+        host = IP(host)
+        if not check_ip(__IP_ALLOW__, host, False):
+            raise Exception(f'IP Not Allowed, {host} not in allowlist')
+        if not check_ip(__IP_BLOCK__, host, True):
+            raise Exception(f'IP Not Allowed, {host} in blocklist')
+
+    if user is None:
+        raise Exception(f"Unauthorized")
+
+    methods = func.split('.')
+
+    if METHODS_CHECK:
+        if not check_methods(METHODS_ALLOW, methods, False):
+            raise Exception(f'Method Not Allowed, {func} not in allowlist')
+        if not check_methods(METHODS_BLOCK, methods, True):
+            raise Exception(f'Method Not Allowed, {func} in blocklist')
+
+
+async def call(user, func, args, kwargs, cache_get, cache_expire, async_remote, fmt=None):
+    try:
+        buf = None
+        data = None  # None表示从缓存中取的，需要其它格式时需要转换
+        # cache所用的key
+        key = make_key(func, args, kwargs)
+
+        if cache_get:
+            # 优先取缓存
+            buf = await async_cache_get(key)
+        if buf is None:
+            cache_expire, buf, data = await _call(user, func, args, kwargs, cache_expire, async_remote)
+
+            # 过短的缓存时间没有必要
+            if cache_expire >= 30:
+                # 就算强行去查询数据，也会想办法存下，再次取时还能从缓存中取
+                await async_cache_setex(key, cache_expire, buf)
+                logger.info(f'To cache: expire:{cache_expire}\tlen:{len(buf)}\t{key}')
+        else:
+            logger.info(f'From cache: {func}\t{args}\t{kwargs}')
+
+    except Exception as e:
+        key = type(e).__name__
+        # 这里没有缓存，因为这个错误是服务器内部检查
+        data = RspModel(status=403,  # status.HTTP_403_FORBIDDEN,
+                        datetime=datetime.now().isoformat(),
+                        func=func, args=args, kwargs=kwargs)
+        data.type = type(e).__name__
+        data.data = repr(e)
+        data = data.dict()
+        buf = serialize(data).read()
+
+    return key, buf, data
+
+
+async def _call(user, func_name, args, kwargs, cache_expire, async_remote):
+    """进行实际调用
+
+    将配额计算放在调用第三方代码时，优化用户体验
+    """
+
+    methods = func_name.split('.')
+    module = methods[0]
+
+    m_quota_key = f'QUOTA/{user}/{module}'
+    f_quota_key = f'QUOTA/{user}/{func_name}'
+    if QUOTA_CHECK:
+        # 配额检查
+        from .config import QUOTA_MODULE, QUOTA_MODULE_DEFAULT, QUOTA_FUNC, QUOTA_FUNC_DEFAULT
+
+        m_quota = int(await async_cache_get(m_quota_key) or 0)
+        f_quota = int(await async_cache_get(f_quota_key) or 0)
+        quota = get_quota(QUOTA_FUNC, methods, QUOTA_FUNC_DEFAULT)
+        if f_quota > quota:
+            raise Exception(f'Over quota: user:{user}, {func_name}:{f_quota}>{quota}')
+        quota = get_quota(QUOTA_MODULE, [module], QUOTA_MODULE_DEFAULT)
+        if m_quota > quota:
+            raise Exception(f'Over quota: user:{user}, {module}:{quota}')
+
+    try:
+        # 当前server目录下文件，用于特别处理
+        api = __import__(f'{__package__}.server.{module}', fromlist=['*'])
+    except ModuleNotFoundError as e:
+        # 导入系统包
+        if module == __package__:
+            raise Exception(f'Not Allowed to call {__package__}')
+        api = __import__(module, fromlist=['*'])
+
+    # 返回的数据包
+    d = RspModel(status=200,  # status.HTTP_200_OK,
+                 datetime=datetime.now().isoformat(),  # 加查询时间，缓存中也许可以判断是否过期
+                 func=func_name,
+                 args=args,
+                 kwargs=kwargs)
+
+    methods = methods[1:]
+    try:
+        # 转成字符串，后面可能于做cache的key
+        logger.info(f'Call: {func_name}\t{args}\t{kwargs}'[:200])
+
+        func = api
+        for method in methods:
+            func = getattr(func, method)
+
+        # 可以调用的属性
+        if callable(func):
+            # 例如os.remove
+            type_ = 'function'
+            if async_remote:
+                func = await to_async(func)(*args, **kwargs)
+            else:
+                func = to_sync(func)(*args, **kwargs)
+
+        # 结果的类型名
+        class_name = func.__class__.__name__
+
+        # 不可调用的直接返回
+        if class_name == 'module':
+            # 例如os.path，但用法为os.path()
+            data = repr(func)
+            cache_expire = min(cache_expire, 0)
+        elif class_name in ('dict_keys', 'dict_values'):
+            # 无法序列化，只能强行转换
+            # 例如：sys.modules.keys(), 也可以sys.modules.keys.__list()
+            data = list(func)
+            cache_expire = min(cache_expire, 0)
+        else:
+            # 例如math.pi，但用法math.pi()
+            data = func
+
+            if QUOTA_CHECK:
+                # 模块和函数都进行配额统计，是按行记（聚宽），按单元格记（万得），还是按调用次数记？
+                if isinstance(data, (pd.DataFrame, pd.Series, np.ndarray, list)):
+                    # # 按调用次数
+                    # await async_cache_incrby(m_quota_key, 1)
+                    # await async_cache_incrby(f_quota_key, 1)
+
+                    # 按行统计
+                    await async_cache_incrby(m_quota_key, len(data))
+                    await async_cache_incrby(f_quota_key, len(data))
+
+                    # # 按单元格统计
+                    # if hasattr(data, 'size'):
+                    #     await async_cache_incrby(m_quota_key, data.size)
+                    #     await async_cache_incrby(f_quota_key, data.size)
+                    # else:
+                    #     await async_cache_incrby(m_quota_key, len(data))
+                    #     await async_cache_incrby(f_quota_key, len(data))
+
+        d.type = type(func).__name__
+        d.data = data
+
+        # pkl序列化，为了能完整还源
+        d = d.dict()
+        buf = serialize(d).read()
+
+    except Exception as e:
+        d.status = 500  # status.HTTP_500_INTERNAL_SERVER_ERROR
+        d.type = type(e).__name__
+        d.data = repr(e)
+        # 错误也缓存一会，防止用户写了死循环搞崩上游
+        cache_expire = min(cache_expire, 60)
+        d = d.dict()
+        # 由于错误信息也想缓存，所以这里进行编码
+        buf = serialize(d).read()
+
+    return cache_expire, buf, d
```

### Comparing `ksrpc-0.3.3/ksrpc/config.py` & `ksrpc-0.3.5/ksrpc/config.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-"""
-全局开关
-!!!中继功能不需修改，提供服务功能需要手工开启
-"""
-# 是否可以调用当前服务器中的Python库
-# 为了安全，默认关闭，有需要用户请修改配置
-ENABLE_SERVER = False
-# 是否启用中继功能。启用此功能可实现反向RPC功能。
-# 此功能只转发请求，并不执行其中的内容，对当前中继服务器没有安全威胁
-# 鼓励有公网IP的用户开放提供此功能
-ENABLE_RELAY = True
-
-"""
-服务端配置
-"""
-
-"""
-是否检查可调用的方法。
-!!! 生产环境中请不要随意关闭，否则权限过大
-"""
-METHODS_CHECK = False
-
-# 允许的方法
-# 没有列出的module和method默认值为False表示不可调用
-METHODS_ALLOW = {
-    'pandas': {
-        'read_csv': True,
-        'util': {
-            'testing': {
-                'makeTimeDataFrame': True,
-                'makeDataFrame': False,
-            }
-        }
-    },
-    'os': True,
-    'ntpath': True,
-    'numpy': True,
-    'math': True,
-    'sys': True,
-    'jqdatasdk': True,
-    'WindPy': True,
-    'tushare': True,
-    'rqdatac': True,
-    'demo': True,
-    'xbbg': True,
-    'eikon': True,
-}
-
-# 禁止的方法
-# 没有列出的module和method默认值为True表示放行
-METHODS_BLOCK = {
-    'os': {
-        'remove': False,
-    },
-    'ksrpc': {
-        'config': False,  # !!!一定要注意此处，否则客户端可以盗取账号
-    }
-}
-
-"""
-是否进行IP检查，可屏蔽外网访问
-"""
-IP_CHECK = False
-
-IP_ALLOW = {
-    '127.0.0.0/8': True,  # 回环地址
-    '192.168.0.0/16': True,  # C类内网
-    '172.16.0.0/12': True,  # B类内网
-    '10.0.0.0/8': True,  # A类内网
-}
-IP_BLOCK = {
-    '8.8.8.8/32': False,
-    '8.8.4.4/32': False,
-}
-
-"""
-是否启用授权
-"""
-AUTH_CHECK = False
-# API授权
-AUTH_TOKENS = {
-    "secret-token-1": "john",
-    "secret-token-2": "susan",
-}
-
-"""
-是否进行配额检查，可限制用户超量下载
-只限制初始请求数据，第二次请求走缓存不消耗配额
-"""
-QUOTA_CHECK = False
-
-QUOTA_MODULE = {
-    'demo': 1000,
-}
-
-QUOTA_FUNC = {
-    'demo': {
-        'test': 500,
-    }
-}
-QUOTA_MODULE_DEFAULT = 10000 * 10000  # 1亿行
-QUOTA_FUNC_DEFAULT = 10000 * 1000  # 1千万行
-
-# 缓存类型。生产环境请配置redis服务
-CACHE_TYPE = 'fakeredis'  # fakeredis, aioredis
-# 缓存服务地址
-REDIS_URL = "redis://:password@localhost:6379/0"
-
-# 聚宽账号
-JQ_USERNAME = '13912345678'
-JQ_PASSWORD = '12345678'
-
-# TuShare账号
-TUSHARE_TOKEN = '12345678'
-
-# eikon账号
-EIKON_APP_KEY = '12345678'
-
-# 米筐账号
-RQ_USERNAME = '13912345678'
-RQ_PASSWORD = '12345678'
-
-# 启用万得
-WIND_ENABLE = False
-
-# 打印当前配置
-print('current config:', __file__)
+"""
+全局开关
+!!!中继功能不需修改，提供服务功能需要手工开启
+"""
+# 是否可以调用当前服务器中的Python库
+# 为了安全，默认关闭，有需要用户请修改配置
+ENABLE_SERVER = False
+# 是否启用中继功能。启用此功能可实现反向RPC功能。
+# 此功能只转发请求，并不执行其中的内容，对当前中继服务器没有安全威胁
+# 鼓励有公网IP的用户开放提供此功能
+ENABLE_RELAY = True
+
+"""
+服务端配置
+"""
+
+"""
+是否检查可调用的方法。
+!!! 生产环境中请不要随意关闭，否则权限过大
+"""
+METHODS_CHECK = False
+
+# 允许的方法
+# 没有列出的module和method默认值为False表示不可调用
+METHODS_ALLOW = {
+    'pandas': {
+        'read_csv': True,
+        'util': {
+            'testing': {
+                'makeTimeDataFrame': True,
+                'makeDataFrame': False,
+            }
+        }
+    },
+    'os': True,
+    'ntpath': True,
+    'numpy': True,
+    'math': True,
+    'sys': True,
+    'jqdatasdk': True,
+    'WindPy': True,
+    'tushare': True,
+    'rqdatac': True,
+    'demo': True,
+    'xbbg': True,
+    'eikon': True,
+}
+
+# 禁止的方法
+# 没有列出的module和method默认值为True表示放行
+METHODS_BLOCK = {
+    'os': {
+        'remove': False,
+    },
+    'ksrpc': {
+        'config': False,  # !!!一定要注意此处，否则客户端可以盗取账号
+    }
+}
+
+"""
+是否进行IP检查，可屏蔽外网访问
+"""
+IP_CHECK = False
+
+IP_ALLOW = {
+    '127.0.0.0/8': True,  # 回环地址
+    '192.168.0.0/16': True,  # C类内网
+    '172.16.0.0/12': True,  # B类内网
+    '10.0.0.0/8': True,  # A类内网
+}
+IP_BLOCK = {
+    '8.8.8.8/32': False,
+    '8.8.4.4/32': False,
+}
+
+"""
+是否启用授权
+"""
+AUTH_CHECK = False
+# API授权
+AUTH_TOKENS = {
+    "secret-token-1": "john",
+    "secret-token-2": "susan",
+}
+
+"""
+是否进行配额检查，可限制用户超量下载
+只限制初始请求数据，第二次请求走缓存不消耗配额
+"""
+QUOTA_CHECK = False
+
+QUOTA_MODULE = {
+    'demo': 1000,
+}
+
+QUOTA_FUNC = {
+    'demo': {
+        'test': 500,
+    }
+}
+QUOTA_MODULE_DEFAULT = 10000 * 10000  # 1亿行
+QUOTA_FUNC_DEFAULT = 10000 * 1000  # 1千万行
+
+# 缓存类型。生产环境请配置redis服务
+CACHE_TYPE = 'fakeredis'  # fakeredis, aioredis
+# 缓存服务地址
+REDIS_URL = "redis://:password@localhost:6379/0"
+
+# 聚宽账号
+JQ_USERNAME = '13912345678'
+JQ_PASSWORD = '12345678'
+
+# TuShare账号
+TUSHARE_TOKEN = '12345678'
+
+# eikon账号
+EIKON_APP_KEY = '12345678'
+
+# 米筐账号
+RQ_USERNAME = '13912345678'
+RQ_PASSWORD = '12345678'
+
+# 启用万得
+WIND_ENABLE = False
+
+# 打印当前配置
+print('current config:', __file__)
```

### Comparing `ksrpc-0.3.3/ksrpc/connections/http.py` & `ksrpc-0.3.5/ksrpc/connections/http.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-05-15
-
-"""
-HTTP客户端
-默认提交pickle格式，返回也是pickle格式
-
-1. RequestsConnection，使用requests实现。原本只支持同步，但此处已经改成支持异步
-2. HttpxConnection，使用httpx实现。使用异步，但也可以指定成同步使用
-
-"""
-from io import BytesIO
-from urllib.parse import urlparse
-
-import pandas as pd
-
-from ..model import Format
-from ..serializer.json_ import dict_to_obj
-from ..serializer.pkl_gzip import deserialize, serialize
-from ..utils.async_ import to_sync
-
-
-def process_response(r):
-    """处理HTTP响应。根据不同的响应分别处理
-
-    Parameters
-    ----------
-    r: Response
-
-    Returns
-    -------
-    object
-    json
-    csv
-
-    """
-    if r.status_code != 200:
-        raise Exception(f'{r.status_code}, {r.text}')
-    content_type = r.headers['content-type']
-    if content_type.startswith('application/octet-stream'):
-        data = deserialize(r.content)
-        if data['status'] == 200:
-            return data['data']
-        return data
-    elif content_type.startswith('application/json'):
-        data = r.json()
-        if data.get('type', None) in ('DataFrame', 'Series', 'ndarray'):
-            return dict_to_obj(data['data'])
-        if data['status'] == 200:
-            return data['data']
-        return data
-    elif content_type.startswith('text/plain'):
-        # 纯文本，表示返回的CSV格式
-        return pd.read_csv(BytesIO(r.content), index_col=0)
-
-
-class HttpxConnection:
-    """使用httpx实现的客户端连接支持同步和异步"""
-    # 超时，请求超求和响应超时，秒
-    timeout = (5, 30)
-
-    def __init__(self, url, token=None):
-        import httpx
-
-        path = urlparse(url).path
-        assert path.endswith(('/get', '/post', '/file')), 'Python语言优先使用file，其它语言使用post'
-        if path.endswith('/file'):
-            self._fmt = Format.PKL_GZIP
-        else:
-            self._fmt = Format.JSON
-
-        self._url = url
-        self._token = token
-        self._client = httpx.AsyncClient()
-
-    async def __aenter__(self):
-        """异步async with"""
-        await self._client.__aenter__()
-        return self
-
-    async def __aexit__(self, exc_type=None, exc_value=None, traceback=None):
-        """异步async with"""
-        await self._client.__aexit__(exc_type, exc_value, traceback)
-
-    def __enter__(self):
-        """同步with"""
-        to_sync(self._client.__aenter__)()
-        return self
-
-    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
-        """同步with"""
-        to_sync(self._client.__aexit__)()
-
-    async def call(self, func, args, kwargs,
-                   fmt: Format = Format.PKL_GZIP,
-                   cache_get: bool = True, cache_expire: int = 3600,
-                   async_remote=True):
-        """调用函数
-
-        Parameters
-        ----------
-        func: str
-            函数全名
-        args: tuple
-            函数位置参数
-        kwargs: dict
-            函数命名参数
-        fmt: Format
-            指定响应格式
-        cache_get: bool
-            是否优先从缓存中获取
-        cache_expire: int
-            指定缓存超时。超时此时间将过期，指定0表示不进行缓存
-        async_remote: bool
-            异步方式调用
-
-        """
-        # 如果是JSON格式可以考虑返回CSV
-        rsp_fmt = self._fmt
-
-        # httpx解析枚举有问题，只能提前转成value，而requests没有此问题
-        params = dict(func=func, fmt=rsp_fmt.value,
-                      cache_get=cache_get, cache_expire=cache_expire, async_remote=async_remote)
-        data = {'args': args, 'kwargs': kwargs}
-        headers = None if self._token is None else {"Authorization": f"Bearer {self._token}"}
-
-        if self._fmt == Format.PKL_GZIP:
-            files = {"file": serialize(data).read()}
-            r = await self._client.post(self._url, headers=headers, params=params, timeout=self.timeout, files=files)
-        elif self._fmt == Format.JSON:
-            r = await self._client.post(self._url, headers=headers, params=params, timeout=self.timeout, json=data)
-
-        return process_response(r)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-05-15
+
+"""
+HTTP客户端
+默认提交pickle格式，返回也是pickle格式
+
+1. RequestsConnection，使用requests实现。原本只支持同步，但此处已经改成支持异步
+2. HttpxConnection，使用httpx实现。使用异步，但也可以指定成同步使用
+
+"""
+from io import BytesIO
+from urllib.parse import urlparse
+
+import pandas as pd
+
+from ..model import Format
+from ..serializer.json_ import dict_to_obj
+from ..serializer.pkl_gzip import deserialize, serialize
+from ..utils.async_ import to_sync
+
+
+def process_response(r):
+    """处理HTTP响应。根据不同的响应分别处理
+
+    Parameters
+    ----------
+    r: Response
+
+    Returns
+    -------
+    object
+    json
+    csv
+
+    """
+    if r.status_code != 200:
+        raise Exception(f'{r.status_code}, {r.text}')
+    content_type = r.headers['content-type']
+    if content_type.startswith('application/octet-stream'):
+        data = deserialize(r.content)
+        if data['status'] == 200:
+            return data['data']
+        return data
+    elif content_type.startswith('application/json'):
+        data = r.json()
+        if data.get('type', None) in ('DataFrame', 'Series', 'ndarray'):
+            return dict_to_obj(data['data'])
+        if data['status'] == 200:
+            return data['data']
+        return data
+    elif content_type.startswith('text/plain'):
+        # 纯文本，表示返回的CSV格式
+        return pd.read_csv(BytesIO(r.content), index_col=0)
+
+
+class HttpxConnection:
+    """使用httpx实现的客户端连接支持同步和异步"""
+    # 超时，请求超求和响应超时，秒
+    timeout = (5, 30)
+
+    def __init__(self, url, token=None):
+        import httpx
+
+        path = urlparse(url).path
+        assert path.endswith(('/get', '/post', '/file')), 'Python语言优先使用file，其它语言使用post'
+        if path.endswith('/file'):
+            self._fmt = Format.PKL_GZIP
+        else:
+            self._fmt = Format.JSON
+
+        self._url = url
+        self._token = token
+        self._client = httpx.AsyncClient()
+
+    async def __aenter__(self):
+        """异步async with"""
+        await self._client.__aenter__()
+        return self
+
+    async def __aexit__(self, exc_type=None, exc_value=None, traceback=None):
+        """异步async with"""
+        await self._client.__aexit__(exc_type, exc_value, traceback)
+
+    def __enter__(self):
+        """同步with"""
+        to_sync(self._client.__aenter__)()
+        return self
+
+    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
+        """同步with"""
+        to_sync(self._client.__aexit__)()
+
+    async def call(self, func, args, kwargs,
+                   fmt: Format = Format.PKL_GZIP,
+                   cache_get: bool = True, cache_expire: int = 3600,
+                   async_remote=True):
+        """调用函数
+
+        Parameters
+        ----------
+        func: str
+            函数全名
+        args: tuple
+            函数位置参数
+        kwargs: dict
+            函数命名参数
+        fmt: Format
+            指定响应格式
+        cache_get: bool
+            是否优先从缓存中获取
+        cache_expire: int
+            指定缓存超时。超时此时间将过期，指定0表示不进行缓存
+        async_remote: bool
+            异步方式调用
+
+        """
+        # 如果是JSON格式可以考虑返回CSV
+        rsp_fmt = self._fmt
+
+        # httpx解析枚举有问题，只能提前转成value，而requests没有此问题
+        params = dict(func=func, fmt=rsp_fmt.value,
+                      cache_get=cache_get, cache_expire=cache_expire, async_remote=async_remote)
+        data = {'args': args, 'kwargs': kwargs}
+        headers = None if self._token is None else {"Authorization": f"Bearer {self._token}"}
+
+        if self._fmt == Format.PKL_GZIP:
+            files = {"file": serialize(data).read()}
+            r = await self._client.post(self._url, headers=headers, params=params, timeout=self.timeout, files=files)
+        elif self._fmt == Format.JSON:
+            r = await self._client.post(self._url, headers=headers, params=params, timeout=self.timeout, json=data)
+
+        return process_response(r)
```

### Comparing `ksrpc-0.3.3/ksrpc/connections/websocket.py` & `ksrpc-0.3.5/ksrpc/connections/websocket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,196 +1,207 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-05-16
-
-"""
-使用wesockets实现的客户端
-1. 默认提交pickle格式，返回也是pickle格式
-2. 原接口是异步版，必须使用async with，封装成了同步版with
-3. 为了使用方便，还提供了不需with的版本，可直接调用
-
-"""
-import asyncio
-from datetime import datetime
-from urllib.parse import urlparse
-
-from loguru import logger
-
-from ..caller import call
-from ..model import Format, RspModel
-from ..serializer.json_ import dict_to_json, json_to_dict, dict_to_obj
-from ..serializer.pkl_gzip import serialize, deserialize
-from ..utils.async_ import to_sync
-from ..utils.check_ import check_methods
-
-# 二进制拆包
-BYTES_PER_SEND = 1024 * 32
-
-
-def process_response_dict(data):
-    # data = deserialize(r)
-    if data['status'] == 200:
-        return data['data']
-    return data
-
-
-def process_response_json(r):
-    # json字符串转成字字典
-    data = json_to_dict(r)
-    # 特殊类型先还原
-    if data.get('type', None) in ('DataFrame', 'Series', 'ndarray'):
-        data['data'] = dict_to_obj(data['data'])
-    # 成功响应直接返回数据区
-    if data['status'] == 200:
-        return data['data']
-    return data
-
-
-class WebSocketConnection:
-    def __init__(self, url: str, token=None):
-        path = urlparse(url).path
-        assert path.endswith(('/json', '/bytes', '/client', '/admin')), 'Python语言优先使用bytes，其它语言使用json'
-
-        if path.endswith('/json'):
-            self._fmt = Format.JSON
-        else:
-            self._fmt = Format.PKL_GZIP
-
-        self._url = url
-        self._token = token
-        self._with = False  # 记录是否用了with
-
-    async def __aenter__(self):
-        """异步async with"""
-        from websockets import connect
-
-        headers = None if self._token is None else {"Authorization": f"Bearer {self._token}"}
-        # 默认是2**20，只有1MB，扩充一下成8MB
-        self._client = connect(self._url, extra_headers=headers, max_size=2 ** 23)
-
-        self._ws = await self._client.__aenter__()
-        self._with = True
-        return self
-
-    async def __aexit__(self, exc_type=None, exc_value=None, traceback=None):
-        """异步async with"""
-        await self._client.__aexit__(exc_type, exc_value, traceback)
-
-    def __enter__(self):
-        """同步with"""
-        to_sync(self.__aenter__)()
-        return self
-
-    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
-        """同步with"""
-        to_sync(self.__aexit__)()
-
-    async def call(self, func, args, kwargs,
-                   fmt: Format = Format.PKL_GZIP,
-                   cache_get: bool = True, cache_expire: int = 3600,
-                   async_remote=True):
-        # 还没有执行过with就内部主动执行一次
-        if not self._with:
-            await self.__aenter__()
-
-        # 如果是JSON格式可以考虑返回CSV
-        rsp_fmt = self._fmt
-
-        d = dict(func=func, args=args, kwargs=kwargs,
-                 fmt=rsp_fmt.value,
-                 cache_get=cache_get, cache_expire=cache_expire, async_remote=async_remote)
-
-        if self._fmt == Format.PKL_GZIP:
-            # 二进制格式
-            b = serialize(d).read()
-            bl = len(b)
-            await self._ws.send(serialize(bl).read())
-            for i in range(0, len(b), BYTES_PER_SEND):
-                await self._ws.send(b[i:i + BYTES_PER_SEND])
-        else:
-            # json格式
-            await self._ws.send(dict_to_json(d))
-
-        # 这里收到的数据是否需要解析一下，如果是二进制的，需要特别处理
-        rsp = await self._ws.recv()
-        if isinstance(rsp, bytes):
-            # 二进制，反序列化后是字典
-            bl = deserialize(rsp)
-            rsp = b''
-            while len(rsp) < bl:
-                rsp += await self._ws.recv()
-            return process_response_dict(deserialize(rsp))
-        else:
-            return process_response_json(rsp)
-
-    async def reverse(self, recv_timeout=True):
-        """反弹RPC的被控端"""
-        recv_count = 0
-        while True:
-            if recv_timeout:
-                # 对第一个数据包长度添加超时机制
-                timeout_count = 0
-                while True:
-                    try:
-                        # 等15秒
-                        req = await asyncio.wait_for(self._ws.recv(), 30)
-                        timeout_count = 0
-                        break
-                    except asyncio.TimeoutError:
-                        timeout_count += 1
-                        # print('接收超时')
-                        if timeout_count >= 2:
-                            # 约60秒
-                            # print('接收超时断开')
-                            return recv_count
-            else:
-                # 一直等待，无超时
-                req = await self._ws.recv()
-
-            recv_count += 1
-            bl = deserialize(req)
-            req = b''
-            while len(req) < bl:
-                req += await self._ws.recv()
-            req = deserialize(req)
-            # 可能显示太多，需要裁剪一些
-            logger.info(repr(req)[:200])
-            # 不需要缓存
-            req['cache_get'] = False
-            req['cache_expire'] = 0
-            func = req['func']
-            try:
-                from ..config import METHODS_ALLOW, METHODS_BLOCK, METHODS_CHECK
-
-                # 反弹RPC权限要进行限制
-                if METHODS_CHECK:
-                    methods = func.split('.')
-                    if not check_methods(METHODS_ALLOW, methods, False):
-                        raise Exception(f'Method Not Allowed, {func} not in allowlist')
-                    if not check_methods(METHODS_BLOCK, methods, True):
-                        raise Exception(f'Method Not Allowed, {func} in blocklist')
-                # 每个连上去的都分别使用了自己的用户名，这里不需要用户名即可操作
-                user = 'reverse'
-                key, buf, data = await call(user, **req)
-            except Exception as e:
-                # 主要是处理
-                key = type(e).__name__
-                # 这里没有缓存，因为这个错误是服务器内部检查
-                data = RspModel(status=401,  # status.HTTP_401_UNAUTHORIZED,
-                                datetime=datetime.now().isoformat(),
-                                func=func, args=req['args'], kwargs=req['kwargs'])
-                data.type = type(e).__name__
-                data.data = repr(e)
-                data = data.dict()
-                buf = serialize(data).read()
-
-            # 将这里分成两种处理方法
-            bl = len(buf)
-            print(f'需发送字节数:{bl} ', end='')
-            await self._ws.send(serialize(bl).read())
-            for i in range(0, len(buf), BYTES_PER_SEND):
-                print('>', end='')
-                await self._ws.send(buf[i:i + BYTES_PER_SEND])
-                print('\b=', end='')
-            print(' 发送完成')
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-05-16
+
+"""
+使用wesockets实现的客户端
+1. 默认提交pickle格式，返回也是pickle格式
+2. 原接口是异步版，必须使用async with，封装成了同步版with
+3. 为了使用方便，还提供了不需with的版本，可直接调用
+
+"""
+import asyncio
+from datetime import datetime
+from urllib.parse import urlparse
+
+from loguru import logger
+from revolving_asyncio import to_sync
+
+from ..caller import call
+from ..model import Format, RspModel
+from ..serializer.json_ import dict_to_json, json_to_dict, dict_to_obj
+from ..serializer.pkl_gzip import serialize, deserialize
+from ..utils.check_ import check_methods
+from ..utils.notebook import clear_output
+
+# 二进制拆包
+BYTES_PER_SEND = 1024 * 32
+
+
+def process_response_dict(data):
+    # data = deserialize(r)
+    if data['status'] == 200:
+        return data['data']
+    return data
+
+
+def process_response_json(r):
+    # json字符串转成字字典
+    data = json_to_dict(r)
+    # 特殊类型先还原
+    if data.get('type', None) in ('DataFrame', 'Series', 'ndarray'):
+        data['data'] = dict_to_obj(data['data'])
+    # 成功响应直接返回数据区
+    if data['status'] == 200:
+        return data['data']
+    return data
+
+
+class WebSocketConnection:
+    def __init__(self, url: str, token=None):
+        path = urlparse(url).path
+        assert path.endswith(('/json', '/bytes', '/client', '/admin')), 'Python语言优先使用bytes，其它语言使用json'
+
+        if path.endswith('/json'):
+            self._fmt = Format.JSON
+        else:
+            self._fmt = Format.PKL_GZIP
+
+        self._url = url
+        self._token = token
+        self._with = False  # 记录是否用了with
+
+    async def __aenter__(self):
+        """异步async with"""
+        from websockets import connect
+
+        headers = None if self._token is None else {"Authorization": f"Bearer {self._token}"}
+        # 默认是2**20，只有1MB，扩充一下成8MB
+        self._client = connect(self._url, extra_headers=headers, max_size=2 ** 23)
+
+        self._ws = await self._client.__aenter__()
+        self._with = True
+        return self
+
+    async def __aexit__(self, exc_type=None, exc_value=None, traceback=None):
+        """异步async with"""
+        await self._client.__aexit__(exc_type, exc_value, traceback)
+
+    def __enter__(self):
+        """同步with"""
+        to_sync(self.__aenter__)()
+        return self
+
+    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
+        """同步with"""
+        to_sync(self.__aexit__)()
+
+    async def call(self, func, args, kwargs,
+                   fmt: Format = Format.PKL_GZIP,
+                   cache_get: bool = True, cache_expire: int = 3600,
+                   async_remote=True):
+        # 还没有执行过with就内部主动执行一次
+        if not self._with:
+            await self.__aenter__()
+
+        # 如果是JSON格式可以考虑返回CSV
+        rsp_fmt = self._fmt
+
+        d = dict(func=func, args=args, kwargs=kwargs,
+                 fmt=rsp_fmt.value,
+                 cache_get=cache_get, cache_expire=cache_expire, async_remote=async_remote)
+
+        if self._fmt == Format.PKL_GZIP:
+            # 二进制格式
+            b = serialize(d).read()
+            bl = len(b)
+            await self._ws.send(serialize(bl).read())
+            for i in range(0, len(b), BYTES_PER_SEND):
+                await self._ws.send(b[i:i + BYTES_PER_SEND])
+        else:
+            # json格式
+            await self._ws.send(dict_to_json(d))
+
+        # 这里收到的数据是否需要解析一下，如果是二进制的，需要特别处理
+        rsp = await self._ws.recv()
+        if isinstance(rsp, bytes):
+            # 二进制，反序列化后是字典
+            bl = deserialize(rsp)
+            rsp = b''
+            while len(rsp) < bl:
+                rsp += await self._ws.recv()
+            return process_response_dict(deserialize(rsp))
+        else:
+            return process_response_json(rsp)
+
+    async def reverse(self, recv_timeout=True, clear_cnt=5):
+        """反弹RPC的被控端"""
+        recv_count = 0
+        _clear_cnt = 0
+        while True:
+            if recv_timeout:
+                # 对第一个数据包长度添加超时机制
+                timeout_count = 0
+                while True:
+                    try:
+                        # 等15秒
+                        req = await asyncio.wait_for(self._ws.recv(), 30)
+                        timeout_count = 0
+                        break
+                    except asyncio.TimeoutError:
+                        timeout_count += 1
+                        # print('接收超时')
+                        if timeout_count >= 2:
+                            # 约60秒
+                            # print('接收超时断开')
+                            return recv_count
+            else:
+                # 一直等待，无超时
+                req = await self._ws.recv()
+
+            recv_count += 1
+            bl = deserialize(req)
+            req = b''
+            while len(req) < bl:
+                req += await self._ws.recv()
+            req = deserialize(req)
+            # 可能显示太多，需要裁剪一些
+            logger.info(repr(req)[:200])
+            # 不需要缓存
+            req['cache_get'] = False
+            req['cache_expire'] = 0
+            func = req['func']
+            try:
+                from ..config import METHODS_ALLOW, METHODS_BLOCK, METHODS_CHECK
+
+                # 反弹RPC权限要进行限制
+                if METHODS_CHECK:
+                    methods = func.split('.')
+                    if not check_methods(METHODS_ALLOW, methods, False):
+                        raise Exception(f'Method Not Allowed, {func} not in allowlist')
+                    if not check_methods(METHODS_BLOCK, methods, True):
+                        raise Exception(f'Method Not Allowed, {func} in blocklist')
+                # 每个连上去的都分别使用了自己的用户名，这里不需要用户名即可操作
+                user = 'reverse'
+                key, buf, data = await call(user, **req)
+            except Exception as e:
+                # 主要是处理
+                key = type(e).__name__
+                # 这里没有缓存，因为这个错误是服务器内部检查
+                data = RspModel(status=401,  # status.HTTP_401_UNAUTHORIZED,
+                                datetime=datetime.now().isoformat(),
+                                func=func, args=req['args'], kwargs=req['kwargs'])
+                data.type = type(e).__name__
+                data.data = repr(e)
+                data = data.dict()
+                buf = serialize(data).read()
+
+            # 释放内存
+            del data
+            del req
+            # 将这里分成两种处理方法
+            bl = len(buf)
+            print(f'需发送字节数:{bl} ', end='')
+            await self._ws.send(serialize(bl).read())
+            for i in range(0, len(buf), BYTES_PER_SEND):
+                print('>', end='')
+                await self._ws.send(buf[i:i + BYTES_PER_SEND])
+                print('\b=', end='')
+            print(' 发送完成')
+            # 释放内存
+            del buf
+            _clear_cnt += 1
+            if _clear_cnt >= clear_cnt:
+                _clear_cnt = 0
+                clear_output()
```

### Comparing `ksrpc-0.3.3/ksrpc/hack/jqdatasdk.py` & `ksrpc-0.3.5/ksrpc/hack/jqdatasdk.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-jqdatasdk客户端替换
-1. 将底层的instance替换成RpcClient。实现数据库相关的操作也能操作
-"""
-
-
-def hack(client):
-    # 内部类就可以了，不用暴露出去
-    class HackClient:
-        def __init__(self, c):
-            self.client = c
-            self.not_auth = False
-
-        def __getattr__(self, item):
-            return self.client.__getattr__(item)
-
-        def __call__(self, *args, **kwargs):
-            return self
-
-        def _reset(self):
-            pass
-
-        def ensure_auth(self):
-            pass
-
-        def logout(self):
-            pass
-
-    # 最简洁的用法，直接将最低层取数据的部分替换
-    import jqdatasdk.client
-    jqdatasdk.client.JQDataClient.instance = HackClient(client)
+"""
+jqdatasdk客户端替换
+1. 将底层的instance替换成RpcClient。实现数据库相关的操作也能操作
+"""
+
+
+def hack(client):
+    # 内部类就可以了，不用暴露出去
+    class HackClient:
+        def __init__(self, c):
+            self.client = c
+            self.not_auth = False
+
+        def __getattr__(self, item):
+            return self.client.__getattr__(item)
+
+        def __call__(self, *args, **kwargs):
+            return self
+
+        def _reset(self):
+            pass
+
+        def ensure_auth(self):
+            pass
+
+        def logout(self):
+            pass
+
+    # 最简洁的用法，直接将最低层取数据的部分替换
+    import jqdatasdk.client
+    jqdatasdk.client.JQDataClient.instance = HackClient(client)
```

### Comparing `ksrpc-0.3.3/ksrpc/hack/rqdatac.py` & `ksrpc-0.3.5/ksrpc/hack/rqdatac.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-rqdatac客户端替换
-1. 将底层的rqdatac.client替换成RpcClient
-2. init替换，防止登陆
-"""
-
-
-def hack(client):
-    # 内部类就可以了，不用暴露出去
-    class HackClient:
-        PID = -1
-
-        def __init__(self, c):
-            self.client = c
-
-        def execute(self, *args, **kwargs):
-            return self.client.execute(*args, **kwargs)
-
-        def reset(self):
-            pass
-
-        def info(self):
-            pass
-
-        def close(self):
-            pass
-
-    def __init(username=None, password=None, addr=("rqdatad-pro.ricequant.com", 16011), *_, **kwargs):
-        pass
-
-    # 最简洁的用法，直接将最低层取数据的部分替换
-    import rqdatac.client
-    rqdatac.client._CLIENT = HackClient(client)
-    rqdatac.client.init = __init
-    import rqdatac
-    rqdatac.init = __init
+"""
+rqdatac客户端替换
+1. 将底层的rqdatac.client替换成RpcClient
+2. init替换，防止登陆
+"""
+
+
+def hack(client):
+    # 内部类就可以了，不用暴露出去
+    class HackClient:
+        PID = -1
+
+        def __init__(self, c):
+            self.client = c
+
+        def execute(self, *args, **kwargs):
+            return self.client.execute(*args, **kwargs)
+
+        def reset(self):
+            pass
+
+        def info(self):
+            pass
+
+        def close(self):
+            pass
+
+    def __init(username=None, password=None, addr=("rqdatad-pro.ricequant.com", 16011), *_, **kwargs):
+        pass
+
+    # 最简洁的用法，直接将最低层取数据的部分替换
+    import rqdatac.client
+    rqdatac.client._CLIENT = HackClient(client)
+    rqdatac.client.init = __init
+    import rqdatac
+    rqdatac.init = __init
```

### Comparing `ksrpc-0.3.3/ksrpc/model.py` & `ksrpc-0.3.5/ksrpc/model.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from enum import Enum
-from typing import List, Any, Dict
-
-# from fastapi import status
-from pydantic import BaseModel
-
-
-class Format(str, Enum):
-    JSON = 'json'  # 请求和响应用Json可以跨语言
-    PKL_GZIP = 'pkl.gz'  # pickle格式再压缩，可用于网络传输和缓存，限定客户端为python语言
-    CSV = 'csv'  # 响应是DataFrame时，返回CSV格式。其它语言解析时可能比较容易
-
-
-class RspModel(BaseModel):
-    # 状态
-    status: int = 200  # status.HTTP_200_OK
-    # 发生时间
-    datetime: str = 'now'
-    # #请求信息
-    func: str = 'call'
-    args: List[Any] = []
-    kwargs: Dict[str, Any] = {}
-
-    # #响应信息
-    type: str = ''
-    data: Any = None
-
-
-class ReqModel(BaseModel):
-    # #以下在query区，进行提交
-    func: str = 'call'
-    fmt: Format = Format.CSV
-    cache_get: bool = True
-    cache_expire: int = 86400
-
-    # #以下在body区使用json格式或二进制格式提交
-    args: List[Any] = []
-    kwargs: Dict[str, Any] = {}
+from enum import Enum
+from typing import List, Any, Dict
+
+# from fastapi import status
+from pydantic import BaseModel
+
+
+class Format(str, Enum):
+    JSON = 'json'  # 请求和响应用Json可以跨语言
+    PKL_GZIP = 'pkl.gz'  # pickle格式再压缩，可用于网络传输和缓存，限定客户端为python语言
+    CSV = 'csv'  # 响应是DataFrame时，返回CSV格式。其它语言解析时可能比较容易
+
+
+class RspModel(BaseModel):
+    # 状态
+    status: int = 200  # status.HTTP_200_OK
+    # 发生时间
+    datetime: str = 'now'
+    # #请求信息
+    func: str = 'call'
+    args: List[Any] = []
+    kwargs: Dict[str, Any] = {}
+
+    # #响应信息
+    type: str = ''
+    data: Any = None
+
+
+class ReqModel(BaseModel):
+    # #以下在query区，进行提交
+    func: str = 'call'
+    fmt: Format = Format.CSV
+    cache_get: bool = True
+    cache_expire: int = 86400
+
+    # #以下在body区使用json格式或二进制格式提交
+    args: List[Any] = []
+    kwargs: Dict[str, Any] = {}
```

### Comparing `ksrpc-0.3.3/ksrpc/rpc_client.py` & `ksrpc-0.3.5/ksrpc/rpc_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-# 客户端，用于处理请求
-# 需要选择到底是http还是ws，还是nng一类的
-
-from .utils.async_ import to_async, to_sync
-
-
-class RpcClient:
-    """是否优先从缓存中获取"""
-    cache_get: bool = True
-    """缓存超时时间，秒"""
-    cache_expire: int = 86400
-    """本地是否暴露为异步，async def函数中才能启用"""
-    async_local = False
-    """远程是否以异步方式掉用，某些情况下设置成同步才不报错"""
-    async_remote = True
-
-    def __init__(self,
-                 module,
-                 connection,
-                 async_local=False,
-                 async_remote=True,
-                 ):
-        """初始化
-
-        Parameters
-        ----------
-        module: str
-            模块名
-        connection: Connection
-            连接对象
-        async_local: bool
-            是否暴露为异步调用，async def函数中才能启用
-        async_remote: bool
-            远程是否以异步方式掉用，某些情况下设置成同步才不报错
-        """
-        self._connection = connection
-        self._module = module
-        self._methods = [module]
-        self.async_local = async_local
-        self.async_remote = async_remote
-
-    def __getattr__(self, method):
-        self._methods.append(method)
-        return self
-
-    def __call__(self, *args, **kwargs):
-        # 排序，参数顺序统一后，排序生成key便不会浪费了
-        kwargs = dict(sorted(kwargs.items()))
-
-        func = '.'.join(self._methods)
-        # 用完后得重置，否则第二次用时不正确了
-        self._methods = [self._module]
-        # 指定外部调用方式是同步还是异步
-        if self.async_local:
-            f = to_async(self._connection.call)
-        else:
-            f = to_sync(self._connection.call)
-
-        # 注意：这里没有指定输入输出格式，只有输入二进制，输出二进制的格式
-        # 服务器可以支持多种格式是用于非python客户端
-        return f(func, args, kwargs,
-                 cache_get=self.cache_get, cache_expire=self.cache_expire, async_remote=self.async_remote)
-
-    def __len__(self):
-        # 不知怎么回事，被主动调用了
-        return 0
+# 客户端，用于处理请求
+# 需要选择到底是http还是ws，还是nng一类的
+from revolving_asyncio import to_async, to_sync
+
+
+class RpcClient:
+    """是否优先从缓存中获取"""
+    cache_get: bool = True
+    """缓存超时时间，秒"""
+    cache_expire: int = 86400
+    """本地是否暴露为异步，async def函数中才能启用"""
+    async_local = False
+    """远程是否以异步方式掉用，某些情况下设置成同步才不报错"""
+    async_remote = True
+
+    def __init__(self,
+                 module,
+                 connection,
+                 async_local=False,
+                 async_remote=True,
+                 ):
+        """初始化
+
+        Parameters
+        ----------
+        module: str
+            模块名
+        connection: Connection
+            连接对象
+        async_local: bool
+            是否暴露为异步调用，async def函数中才能启用
+        async_remote: bool
+            远程是否以异步方式掉用，某些情况下设置成同步才不报错
+        """
+        self._connection = connection
+        self._module = module
+        self._methods = [module]
+        self.async_local = async_local
+        self.async_remote = async_remote
+
+    def __getattr__(self, method):
+        self._methods.append(method)
+        return self
+
+    def __call__(self, *args, **kwargs):
+        # 排序，参数顺序统一后，排序生成key便不会浪费了
+        kwargs = dict(sorted(kwargs.items()))
+
+        func = '.'.join(self._methods)
+        # 用完后得重置，否则第二次用时不正确了
+        self._methods = [self._module]
+        # 指定外部调用方式是同步还是异步
+        if self.async_local:
+            f = to_async(self._connection.call)
+        else:
+            f = to_sync(self._connection.call)
+
+        # 注意：这里没有指定输入输出格式，只有输入二进制，输出二进制的格式
+        # 服务器可以支持多种格式是用于非python客户端
+        return f(func, args, kwargs,
+                 cache_get=self.cache_get, cache_expire=self.cache_expire, async_remote=self.async_remote)
+
+    def __len__(self):
+        # 不知怎么回事，被主动调用了
+        return 0
```

### Comparing `ksrpc-0.3.3/ksrpc/rpc_reverse.py` & `ksrpc-0.3.5/ksrpc/rpc_reverse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-# !/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-05-26
-"""
-reverse rpc，反弹rpc
-如果要调用的服务器在内网，并且由于条件所限，无法安装更多的库
-所以这里只需小规模的安装即可
-
-以下代码可以直接复制在Notebook中使用
-
-!!!一定要自行修改房间号!!!
-"""
-
-import asyncio
-
-from loguru import logger
-
-from ksrpc.connections.websocket import WebSocketConnection
-
-# 重试次数，防止忘记关闭Notebook内核导致占用资源
-RETRY_COUNT = 10
-TOKEN = 'secret-token-2'
-# 注意：房间号请设置一个复杂的字符串，一定不要与其他用户的冲突，否则数据会乱
-URL = 'ws://127.0.0.1:8000/ws/client?room=HA9527'
-
-
-async def async_main():
-    logger.info('强调!!!使用完后一定要停止内核，防止长期占用资源!!!')
-
-    cnt = RETRY_COUNT
-    while cnt > 0:  # 重连次数，约1分钟
-        logger.info('try to connect. {}', cnt)
-        try:
-            # 连接被控端地址（带/client），同时还要指定约定的房间号字符串
-            async with WebSocketConnection(URL, token=TOKEN) as conn:
-                logger.info('connected')
-                recv_count = await conn.reverse(recv_timeout=True)
-                # 空闲断开时会走到这一步
-                logger.info('recv timeout')
-                if recv_count == 0:
-                    # 内部空闲超时是60秒，为了快速停止，加快超时设定
-                    cnt -= 2
-                else:
-                    # 底层收到过数据包，外层重新计数
-                    cnt = RETRY_COUNT
-        except Exception as e:
-            logger.info(e)
-            # 重试不能太块，一直在重试时，试着点击重启内核
-            await asyncio.sleep(5)
-            cnt -= 1
-    logger.info('done')
-
-
-if __name__ == '__main__':
-    asyncio.run(async_main())
+# !/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-05-26
+"""
+reverse rpc，反弹rpc
+如果要调用的服务器在内网，并且由于条件所限，无法安装更多的库
+所以这里只需小规模的安装即可
+
+以下代码可以直接复制在Notebook中使用
+
+!!!一定要自行修改房间号!!!
+
+!pip install ksrpc-0.3.3-py3-none-any.whl --user --upgrade
+"""
+
+import asyncio
+
+from loguru import logger
+
+from ksrpc.connections.websocket import WebSocketConnection
+
+# 重试次数，防止忘记关闭Notebook内核导致占用资源
+RETRY_COUNT = 30
+TOKEN = 'secret-token-2'
+# 注意：房间号请设置一个复杂的字符串，一定不要与其他用户的冲突，否则数据会乱
+URL = 'ws://127.0.0.1:8000/ws/client?room=HA9527'
+
+
+async def async_main():
+    logger.info('强调!!!使用完后一定要停止内核，防止长期占用资源!!!')
+
+    cnt = RETRY_COUNT
+    while cnt > 0:  # 重连次数，约1分钟
+        logger.info('try to connect. {}', cnt)
+        try:
+            # 连接被控端地址（带/client），同时还要指定约定的房间号字符串
+            async with WebSocketConnection(URL, token=TOKEN) as conn:
+                logger.info('connected')
+                recv_count = await conn.reverse(recv_timeout=True, clear_cnt=3)
+                # 空闲断开时会走到这一步
+                logger.info('recv timeout')
+                if recv_count == 0:
+                    # 内部空闲超时是60秒，为了快速停止，加快超时设定
+                    cnt -= 2
+                else:
+                    # 底层收到过数据包，外层重新计数
+                    cnt = RETRY_COUNT
+        except Exception as e:
+            logger.info(e)
+            # 重试不能太块，一直在重试时，试着点击重启内核
+            await asyncio.sleep(5)
+            cnt -= 1
+    logger.info('done')
+
+
+if __name__ == '__main__':
+    asyncio.run(async_main())
```

### Comparing `ksrpc-0.3.3/ksrpc/serializer/json_.py` & `ksrpc-0.3.5/ksrpc/serializer/json_.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-05-02
-
-"""
-特殊设计的json互转
-1. DataFrame和Series的解析最好能在信息完整与空间大小之间平衡，所以选择tight模式
-    1. to_dict有tight模式，而to_json却没有
-2. 时间希望能正确的转为字符串。pandas._libs.json能正确解析时间
-
-"""
-import copy
-
-import numpy as np
-import pandas as pd
-# 不使用内置json是为了方便处理时间格式
-import pandas._libs.json as json
-
-
-def obj_to_dict(obj):
-    """将pandas转成字典，方便后期转成json格式"""
-    if isinstance(obj, pd.DataFrame):
-        d = obj.to_dict(orient='tight')
-    elif isinstance(obj, pd.Series):
-        d = obj.to_dict()
-    else:
-        # 复制一下，防止后期修改了原数据
-        if hasattr(obj, 'copy'):
-            d = obj.copy()
-        else:
-            d = copy.copy(obj)
-    return d
-
-
-def dict_to_json(d: dict):
-    """字典转json
-
-    调用import pandas._libs.json as json来进行转换，解决时间格式转换问题
-    """
-    # 复合索引的元组可能简单的只拼接成字符串，导致无法还原
-    return json.dumps(d, iso_dates=True)
-
-
-def json_to_dict(text):
-    """json转字典
-
-    调用import pandas._libs.json as json来进行转换，解决时间格式转换问题
-    """
-    return json.loads(text)
-
-
-def dict_to_obj(d):
-    """dict转pandas"""
-    # ndarray直接返回即可
-    if isinstance(d, np.ndarray):
-        return d
-    # list可以转成一维或二维ndarray
-    if isinstance(d, list):
-        return np.array(d)
-    if isinstance(d, dict):
-        if 'data' in d:
-            # 与to_dict参数对应
-            return pd.DataFrame.from_dict(d, orient='tight')
-        else:
-            # 丢失了index上的name
-            return pd.Series(d)
-
-
-def _display(o1):
-    """显示测试"""
-    print('=' * 100)
-    d1 = obj_to_dict(o1)
-    print('-' * 60, 'pandas转dict')
-    print(d1)
-    j1 = dict_to_json(d1)
-    print('-' * 60, 'dict转json')
-    print(j1)
-    print('-' * 60, 'dict转object')
-    print(dict_to_obj(d1))
-    d2 = json_to_dict(j1)
-    print('-' * 60, 'json转dict')
-    print(d2)
-    o2 = dict_to_obj(d2)
-    print('-' * 60, 'dict转pandas')
-    print(o2)
-
-
-if __name__ == '__main__':
-    MINUTES_PER_YEAR = 8
-    NUMBER_OF_SHARES = 5
-
-    pd._testing._N = MINUTES_PER_YEAR
-    pd._testing._K = NUMBER_OF_SHARES  # 只会显示26个字母
-
-    df = pd._testing.makeTimeDataFrame(freq="5min")
-    # df = pd._testing.makeDataFrame()
-
-    # 复合索引测试
-    # df = df.set_index('A', append=True)
-
-    _display(df.values)
-    _display(df)
-    _display(df['B'].values)
-    _display(df['B'])
-    print(df['B'].to_json())
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-05-02
+
+"""
+特殊设计的json互转
+1. DataFrame和Series的解析最好能在信息完整与空间大小之间平衡，所以选择tight模式
+    1. to_dict有tight模式，而to_json却没有
+2. 时间希望能正确的转为字符串。pandas._libs.json能正确解析时间
+
+"""
+import copy
+
+import numpy as np
+import pandas as pd
+# 不使用内置json是为了方便处理时间格式
+import pandas._libs.json as json
+
+
+def obj_to_dict(obj):
+    """将pandas转成字典，方便后期转成json格式"""
+    if isinstance(obj, pd.DataFrame):
+        d = obj.to_dict(orient='tight')
+    elif isinstance(obj, pd.Series):
+        d = obj.to_dict()
+    else:
+        # 复制一下，防止后期修改了原数据
+        if hasattr(obj, 'copy'):
+            d = obj.copy()
+        else:
+            d = copy.copy(obj)
+    return d
+
+
+def dict_to_json(d: dict):
+    """字典转json
+
+    调用import pandas._libs.json as json来进行转换，解决时间格式转换问题
+    """
+    # 复合索引的元组可能简单的只拼接成字符串，导致无法还原
+    return json.dumps(d, iso_dates=True)
+
+
+def json_to_dict(text):
+    """json转字典
+
+    调用import pandas._libs.json as json来进行转换，解决时间格式转换问题
+    """
+    return json.loads(text)
+
+
+def dict_to_obj(d):
+    """dict转pandas"""
+    # ndarray直接返回即可
+    if isinstance(d, np.ndarray):
+        return d
+    # list可以转成一维或二维ndarray
+    if isinstance(d, list):
+        return np.array(d)
+    if isinstance(d, dict):
+        if 'data' in d:
+            # 与to_dict参数对应
+            return pd.DataFrame.from_dict(d, orient='tight')
+        else:
+            # 丢失了index上的name
+            return pd.Series(d)
+
+
+def _display(o1):
+    """显示测试"""
+    print('=' * 100)
+    d1 = obj_to_dict(o1)
+    print('-' * 60, 'pandas转dict')
+    print(d1)
+    j1 = dict_to_json(d1)
+    print('-' * 60, 'dict转json')
+    print(j1)
+    print('-' * 60, 'dict转object')
+    print(dict_to_obj(d1))
+    d2 = json_to_dict(j1)
+    print('-' * 60, 'json转dict')
+    print(d2)
+    o2 = dict_to_obj(d2)
+    print('-' * 60, 'dict转pandas')
+    print(o2)
+
+
+if __name__ == '__main__':
+    MINUTES_PER_YEAR = 8
+    NUMBER_OF_SHARES = 5
+
+    pd._testing._N = MINUTES_PER_YEAR
+    pd._testing._K = NUMBER_OF_SHARES  # 只会显示26个字母
+
+    df = pd._testing.makeTimeDataFrame(freq="5min")
+    # df = pd._testing.makeDataFrame()
+
+    # 复合索引测试
+    # df = df.set_index('A', append=True)
+
+    _display(df.values)
+    _display(df)
+    _display(df['B'].values)
+    _display(df['B'])
+    print(df['B'].to_json())
```

### Comparing `ksrpc-0.3.3/ksrpc/server/WindPy.py` & `ksrpc-0.3.5/ksrpc/server/WindPy.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""
-Wind服务转发
-1. 必须先开启Wind客户端再启动此服务
-2. 返回的数据做了额外处理，额外抛出异常，用于控制缓存
-"""
-from functools import wraps
-
-from WindPy import w
-
-# TODO: 是否能在线程中启动，需要测试
-# print(w.start())
-
-__path__ = []
-__all__ = []
-
-
-def _post_func(func, name):
-    @wraps(func)
-    def decorated(*args, **kwargs):
-        # print(name)
-        # 是否能获取到函数名
-        error, data = func(*args, **kwargs)
-        # 原始错误上层无法感知，导致可能按用户指定的时间缓存一天
-        # 所以特别处理一下，遇到错误抛出异常，这样上层就能识别将缓存缩短成1分钟
-        if error != 0:
-            raise Exception(data)
-        return error, data
-
-    return decorated
-
-
-def __getattr__(name):
-    # 对数据做后处理
-    return _post_func(getattr(w, name), name)
-
-
-def start():
-    pass
+"""
+Wind服务转发
+1. 必须先开启Wind客户端再启动此服务
+2. 返回的数据做了额外处理，额外抛出异常，用于控制缓存
+"""
+from functools import wraps
+
+from WindPy import w
+
+# TODO: 是否能在线程中启动，需要测试
+# print(w.start())
+
+__path__ = []
+__all__ = []
+
+
+def _post_func(func, name):
+    @wraps(func)
+    def decorated(*args, **kwargs):
+        # print(name)
+        # 是否能获取到函数名
+        error, data = func(*args, **kwargs)
+        # 原始错误上层无法感知，导致可能按用户指定的时间缓存一天
+        # 所以特别处理一下，遇到错误抛出异常，这样上层就能识别将缓存缩短成1分钟
+        if error != 0:
+            raise Exception(data)
+        return error, data
+
+    return decorated
+
+
+def __getattr__(name):
+    # 对数据做后处理
+    return _post_func(getattr(w, name), name)
+
+
+def start():
+    pass
```

### Comparing `ksrpc-0.3.3/ksrpc/server/rqdatac.py` & `ksrpc-0.3.5/ksrpc/server/rqdatac.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-rqdatac服务转发
-1. 屏蔽init功能，由服务端进行统一认证
-2. 客户端替换了client, 服务端将请求转到client，统一进行execute
-
-"""
-from atexit import register
-
-from loguru import logger
-from rqdatac import init, reset
-from rqdatac.client import get_client
-
-from ..config import RQ_USERNAME, RQ_PASSWORD
-
-init(username=RQ_USERNAME, password=RQ_PASSWORD)
-# 用完后清空，防止被客户端获取
-del RQ_USERNAME
-del RQ_PASSWORD
-
-
-@register
-def _atexit():
-    logger.info("{} {}", __name__, _atexit.__name__)
-    reset()
-
-
-def execute(method, *args, **kwargs):
-    return get_client().execute(method, *args, **kwargs)
-
-
-def init(username=None, password=None, addr=("rqdatad-pro.ricequant.com", 16011), *_, **kwargs):
-    # 防止用户调用到了init
-    pass
+"""
+rqdatac服务转发
+1. 屏蔽init功能，由服务端进行统一认证
+2. 客户端替换了client, 服务端将请求转到client，统一进行execute
+
+"""
+from atexit import register
+
+from loguru import logger
+from rqdatac import init, reset
+from rqdatac.client import get_client
+
+from ..config import RQ_USERNAME, RQ_PASSWORD
+
+init(username=RQ_USERNAME, password=RQ_PASSWORD)
+# 用完后清空，防止被客户端获取
+del RQ_USERNAME
+del RQ_PASSWORD
+
+
+@register
+def _atexit():
+    logger.info("{} {}", __name__, _atexit.__name__)
+    reset()
+
+
+def execute(method, *args, **kwargs):
+    return get_client().execute(method, *args, **kwargs)
+
+
+def init(username=None, password=None, addr=("rqdatad-pro.ricequant.com", 16011), *_, **kwargs):
+    # 防止用户调用到了init
+    pass
```

### Comparing `ksrpc-0.3.3/ksrpc/server/tushare.py` & `ksrpc-0.3.5/ksrpc/server/tushare.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-TuShare服务转发
-1. 屏蔽set_token功能，由服务端进行统一认证
-2. 客户端替换了pro, 服务端将请求转到pro
-
-"""
-
-import tushare as ts
-
-from ..config import TUSHARE_TOKEN
-
-ts.set_token(TUSHARE_TOKEN)
-# 用完后清空，防止被客户端获取
-del TUSHARE_TOKEN
-pro = ts.pro_api()
-
-__path__ = []
-__all__ = []
-
-
-def __getattr__(name):
-    return pro.__getattr__(name)
-
-
-def set_token(token):
-    # 防止用户调用到了pro.set_token
-    pass
-
-
-def get_token():
-    return ""
-
-
-def pro_api(token='', timeout=30):
-    # 防止用户调用到了pro.pro_api
-    pass
+"""
+TuShare服务转发
+1. 屏蔽set_token功能，由服务端进行统一认证
+2. 客户端替换了pro, 服务端将请求转到pro
+
+"""
+
+import tushare as ts
+
+from ..config import TUSHARE_TOKEN
+
+ts.set_token(TUSHARE_TOKEN)
+# 用完后清空，防止被客户端获取
+del TUSHARE_TOKEN
+pro = ts.pro_api()
+
+__path__ = []
+__all__ = []
+
+
+def __getattr__(name):
+    return pro.__getattr__(name)
+
+
+def set_token(token):
+    # 防止用户调用到了pro.set_token
+    pass
+
+
+def get_token():
+    return ""
+
+
+def pro_api(token='', timeout=30):
+    # 防止用户调用到了pro.pro_api
+    pass
```

### Comparing `ksrpc-0.3.3/ksrpc/update_quota.py` & `ksrpc-0.3.5/ksrpc/update_quota.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# 应当用计划任务，每天凌晨0点执行
-# 每天按需求重值部分用户的配额信息，第二天即可使用
-import asyncio
-
-from ksrpc.cache import async_cache_setex, async_cache_get, async_cache_keys
-
-
-async def test():
-    user = 'nobody'
-    module = 'demo'
-    func_name = 'demo.test'
-
-    m_quota_key = f'QUOTA/{user}/{module}'
-    f_quota_key = f'QUOTA/{user}/{func_name}'
-    await async_cache_setex(m_quota_key, 86400 * 7, 100)
-    await async_cache_setex(f_quota_key, 86400 * 7, 200)
-
-
-async def async_main():
-    keys = await async_cache_keys('QUOTA*')
-    for key in keys:
-        print(await async_cache_get(key))
-    for key in keys:
-        await async_cache_setex(key, 86400 * 7, 0)
-    for key in keys:
-        print(await async_cache_get(key))
-
-
-if __name__ == '__main__':
-    asyncio.run(test())
-    asyncio.run(async_main())
+# 应当用计划任务，每天凌晨0点执行
+# 每天按需求重值部分用户的配额信息，第二天即可使用
+import asyncio
+
+from ksrpc.cache import async_cache_setex, async_cache_get, async_cache_keys
+
+
+async def test():
+    user = 'nobody'
+    module = 'demo'
+    func_name = 'demo.test'
+
+    m_quota_key = f'QUOTA/{user}/{module}'
+    f_quota_key = f'QUOTA/{user}/{func_name}'
+    await async_cache_setex(m_quota_key, 86400 * 7, 100)
+    await async_cache_setex(f_quota_key, 86400 * 7, 200)
+
+
+async def async_main():
+    keys = await async_cache_keys('QUOTA*')
+    for key in keys:
+        print(await async_cache_get(key))
+    for key in keys:
+        await async_cache_setex(key, 86400 * 7, 0)
+    for key in keys:
+        print(await async_cache_get(key))
+
+
+if __name__ == '__main__':
+    asyncio.run(test())
+    asyncio.run(async_main())
```

### Comparing `ksrpc-0.3.3/ksrpc/utils/check_.py` & `ksrpc-0.3.5/ksrpc/utils/check_.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-def check_ip(ip_list, ip, default):
-    """IP检查
-
-    找到了，就用约定的值
-    没找到，就用默认值default
-    """
-    for x, y in ip_list.items():
-        # if IP(ip) in IP(x):
-        if ip in x:
-            # 返回指定值
-            return y
-    # 没找到，反回默认值
-    return default
-
-
-def check_methods(dict_, list_, default):
-    """方法权限检查
-
-    找到了，就用约定的值
-    没找到，就用默认值default
-    """
-    d = dict_
-    for x in list_:
-        d = d.get(x, default)
-        if isinstance(d, bool):
-            return d
-    return default
-
-
-def get_quota(dict_, list_, default):
-    """方法权限检查
-
-    找到了，就用约定的值
-    没找到，就用默认值default
-    """
-    d = dict_
-    for x in list_:
-        d = d.get(x, default)
-        if isinstance(d, int):
-            return d
-    return default
-
-
-if __name__ == "__main__":
-    from IPy import IP
-
-    IP_ALLOW = {
-        IP('127.0.0.0/8'): True,  # 回环地址
-        IP('192.168.0.0/16'): True,  # C类内网
-        IP('172.16.0.0/12'): True,  # B类内网
-        IP('10.0.0.0/8'): True,  # A类内网
-    }
-    IP_BLOCK = {
-        IP('8.8.8.8/32'): False,
-        IP('8.8.4.4/32'): False,
-    }
-    print(check_ip(IP_ALLOW, IP('127.0.0.1'), False))
-    print(check_ip(IP_ALLOW, IP('172.31.0.0'), False))
-    print(check_ip(IP_ALLOW, IP('114.114.114.114'), False))
-    print(check_ip(IP_BLOCK, IP('8.8.8.8'), True))
-    print(check_ip(IP_BLOCK, IP('114.114.114.114'), True))
+def check_ip(ip_list, ip, default):
+    """IP检查
+
+    找到了，就用约定的值
+    没找到，就用默认值default
+    """
+    for x, y in ip_list.items():
+        # if IP(ip) in IP(x):
+        if ip in x:
+            # 返回指定值
+            return y
+    # 没找到，反回默认值
+    return default
+
+
+def check_methods(dict_, list_, default):
+    """方法权限检查
+
+    找到了，就用约定的值
+    没找到，就用默认值default
+    """
+    d = dict_
+    for x in list_:
+        d = d.get(x, default)
+        if isinstance(d, bool):
+            return d
+    return default
+
+
+def get_quota(dict_, list_, default):
+    """方法权限检查
+
+    找到了，就用约定的值
+    没找到，就用默认值default
+    """
+    d = dict_
+    for x in list_:
+        d = d.get(x, default)
+        if isinstance(d, int):
+            return d
+    return default
+
+
+if __name__ == "__main__":
+    from IPy import IP
+
+    IP_ALLOW = {
+        IP('127.0.0.0/8'): True,  # 回环地址
+        IP('192.168.0.0/16'): True,  # C类内网
+        IP('172.16.0.0/12'): True,  # B类内网
+        IP('10.0.0.0/8'): True,  # A类内网
+    }
+    IP_BLOCK = {
+        IP('8.8.8.8/32'): False,
+        IP('8.8.4.4/32'): False,
+    }
+    print(check_ip(IP_ALLOW, IP('127.0.0.1'), False))
+    print(check_ip(IP_ALLOW, IP('172.31.0.0'), False))
+    print(check_ip(IP_ALLOW, IP('114.114.114.114'), False))
+    print(check_ip(IP_BLOCK, IP('8.8.8.8'), True))
+    print(check_ip(IP_BLOCK, IP('114.114.114.114'), True))
```

### Comparing `ksrpc-0.3.3/ksrpc/utils/date_.py` & `ksrpc-0.3.5/ksrpc/utils/date_.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022, wukan
-# @Date       :2022-03-02
-
-"""
-API输入时间参数过于动态不利于缓存key生成
-
-例如date.now()时间一直在变化，如果转成日期或转成周五，可以大量减少key
-"""
-
-from datetime import datetime
-
-import numpy as np
-import pandas as pd
-
-
-def to_date_str(dt):
-    """只取日期部分"""
-    if isinstance(dt, int):
-        dt = str(dt)
-    if isinstance(dt, str):
-        if ':' in dt:
-            return dt[:10]
-        if len(dt) == 10:
-            return dt
-    if isinstance(dt, (str, np.datetime64)):
-        dt = pd.to_datetime(dt)
-    return f'{dt:%Y-%m-%d}'
-
-
-def eq_today(end_date):
-    """等于今天"""
-    return to_date_str(end_date) == f'{datetime.today():%Y-%m-%d}'
-
-
-def ge_today(end_date):
-    """大于等于今天"""
-    return to_date_str(end_date) >= f'{datetime.today():%Y-%m-%d}'
-
-
-if __name__ == '__main__':
-    print(eq_today(20210925))
-    print(eq_today(20210929))
-    print(to_date_str(20210925))
-    print(to_date_str('2021-09-25 01:44:29.477371'))
-    print(to_date_str('2021-09-25T01:44:29.477371'))
-    print(eq_today('2021-09-29T01:44:29.477371'))
-    print(eq_today('2021-09-30'))
-    print(ge_today('2021-09-30'))
-    print(to_date_str(datetime.now()))
-    print(to_date_str(datetime.now().date()))
-    print(to_date_str(pd.to_datetime(datetime.now())))
-    print(to_date_str(np.datetime64(datetime.now())))
-
-    from dateutil.relativedelta import relativedelta, FR
-
-    print(datetime(2021, 9, 25) + relativedelta(weekday=FR(-1)))
-    print(datetime(2021, 9, 25) + relativedelta(weekday=FR(0)))
-    print(datetime(2021, 9, 25) + relativedelta(weekday=FR(+1)))
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022, wukan
+# @Date       :2022-03-02
+
+"""
+API输入时间参数过于动态不利于缓存key生成
+
+例如date.now()时间一直在变化，如果转成日期或转成周五，可以大量减少key
+"""
+
+from datetime import datetime
+
+import numpy as np
+import pandas as pd
+
+
+def to_date_str(dt):
+    """只取日期部分"""
+    if isinstance(dt, int):
+        dt = str(dt)
+    if isinstance(dt, str):
+        if ':' in dt:
+            return dt[:10]
+        if len(dt) == 10:
+            return dt
+    if isinstance(dt, (str, np.datetime64)):
+        dt = pd.to_datetime(dt)
+    return f'{dt:%Y-%m-%d}'
+
+
+def eq_today(end_date):
+    """等于今天"""
+    return to_date_str(end_date) == f'{datetime.today():%Y-%m-%d}'
+
+
+def ge_today(end_date):
+    """大于等于今天"""
+    return to_date_str(end_date) >= f'{datetime.today():%Y-%m-%d}'
+
+
+if __name__ == '__main__':
+    print(eq_today(20210925))
+    print(eq_today(20210929))
+    print(to_date_str(20210925))
+    print(to_date_str('2021-09-25 01:44:29.477371'))
+    print(to_date_str('2021-09-25T01:44:29.477371'))
+    print(eq_today('2021-09-29T01:44:29.477371'))
+    print(eq_today('2021-09-30'))
+    print(ge_today('2021-09-30'))
+    print(to_date_str(datetime.now()))
+    print(to_date_str(datetime.now().date()))
+    print(to_date_str(pd.to_datetime(datetime.now())))
+    print(to_date_str(np.datetime64(datetime.now())))
+
+    from dateutil.relativedelta import relativedelta, FR
+
+    print(datetime(2021, 9, 25) + relativedelta(weekday=FR(-1)))
+    print(datetime(2021, 9, 25) + relativedelta(weekday=FR(0)))
+    print(datetime(2021, 9, 25) + relativedelta(weekday=FR(+1)))
```

### Comparing `ksrpc-0.3.3/ksrpc.egg-info/SOURCES.txt` & `ksrpc-0.3.5/ksrpc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 ksrpc/__init__.py
 ksrpc/__main__.py
 ksrpc/_version.py
 ksrpc/cache.py
 ksrpc/caller.py
 ksrpc/config.py
@@ -37,10 +38,10 @@
 ksrpc/server/config.py
 ksrpc/server/demo.py
 ksrpc/server/eikon.py
 ksrpc/server/jqdatasdk.py
 ksrpc/server/rqdatac.py
 ksrpc/server/tushare.py
 ksrpc/utils/__init__.py
-ksrpc/utils/async_.py
 ksrpc/utils/check_.py
-ksrpc/utils/date_.py
+ksrpc/utils/date_.py
+ksrpc/utils/notebook.py
```

