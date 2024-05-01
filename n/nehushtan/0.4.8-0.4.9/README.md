# Comparing `tmp/nehushtan-0.4.8.tar.gz` & `tmp/nehushtan-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nehushtan-0.4.8.tar", last modified: Wed Jul 14 04:01:15 2021, max compression
+gzip compressed data, was "nehushtan-0.4.9.tar", last modified: Wed Jul 14 06:52:26 2021, max compression
```

## Comparing `nehushtan-0.4.8.tar` & `nehushtan-0.4.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.779438 nehushtan-0.4.8/
--rw-r--r--   0 leqee      (501) staff       (20)       17 2020-12-15 14:20:35.000000 nehushtan-0.4.8/MANIFEST.in
--rw-r--r--   0 leqee      (501) staff       (20)     2070 2021-07-14 04:01:15.778873 nehushtan-0.4.8/PKG-INFO
--rw-r--r--   0 leqee      (501) staff       (20)     1256 2021-03-22 08:53:28.000000 nehushtan-0.4.8/README.md
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.576541 nehushtan-0.4.8/nehushtan/
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.581694 nehushtan-0.4.8/nehushtan/cli/
--rw-r--r--   0 leqee      (501) staff       (20)     6852 2021-03-22 08:04:50.000000 nehushtan-0.4.8/nehushtan/cli/NehushtanArgumentParser.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/cli/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.584834 nehushtan-0.4.8/nehushtan/helper/
--rw-r--r--   0 leqee      (501) staff       (20)     4034 2021-04-21 09:32:51.000000 nehushtan-0.4.8/nehushtan/helper/CommonHelper.py
--rw-r--r--   0 leqee      (501) staff       (20)     1480 2021-03-05 10:34:43.000000 nehushtan-0.4.8/nehushtan/helper/SignalHandler.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/helper/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.596357 nehushtan-0.4.8/nehushtan/httpd/
--rw-r--r--   0 leqee      (501) staff       (20)      498 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPConstant.py
--rw-r--r--   0 leqee      (501) staff       (20)     4014 2021-05-06 10:01:26.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRequestController.py
--rw-r--r--   0 leqee      (501) staff       (20)      787 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRequestFilter.py
--rw-r--r--   0 leqee      (501) staff       (20)    14327 2021-05-11 07:55:36.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRequestHandler.py
--rw-r--r--   0 leqee      (501) staff       (20)     3206 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPResponseBuffer.py
--rw-r--r--   0 leqee      (501) staff       (20)      736 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRoute.py
--rw-r--r--   0 leqee      (501) staff       (20)     1333 2021-05-06 10:01:26.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRouter.py
--rw-r--r--   0 leqee      (501) staff       (20)     1763 2021-05-08 05:56:23.000000 nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPService.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-28 09:44:18.000000 nehushtan-0.4.8/nehushtan/httpd/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.603320 nehushtan-0.4.8/nehushtan/httpd/exceptions/
--rw-r--r--   0 leqee      (501) staff       (20)      493 2021-05-06 10:01:26.000000 nehushtan-0.4.8/nehushtan/httpd/exceptions/NehushtanHTTPError.py
--rw-r--r--   0 leqee      (501) staff       (20)      447 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/exceptions/NehushtanNoRouteMatchedError.py
--rw-r--r--   0 leqee      (501) staff       (20)      458 2021-05-06 10:01:26.000000 nehushtan-0.4.8/nehushtan/httpd/exceptions/NehushtanRequestDeniedByFilterError.py
--rw-r--r--   0 leqee      (501) staff       (20)      706 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/exceptions/NehushtanRequestParameterError.py
--rw-r--r--   0 leqee      (501) staff       (20)      270 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/exceptions/NehushtanRequestProcessTargetError.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-29 05:40:51.000000 nehushtan-0.4.8/nehushtan/httpd/exceptions/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.610346 nehushtan-0.4.8/nehushtan/httpd/implement/
--rw-r--r--   0 leqee      (501) staff       (20)     3305 2021-05-08 06:52:03.000000 nehushtan-0.4.8/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexArgs.py
--rw-r--r--   0 leqee      (501) staff       (20)     2590 2021-05-08 06:46:11.000000 nehushtan-0.4.8/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexKwargs.py
--rw-r--r--   0 leqee      (501) staff       (20)     3460 2021-05-06 09:53:49.000000 nehushtan-0.4.8/nehushtan/httpd/implement/NehushtanHTTPRouteWithRestFul.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-30 07:28:12.000000 nehushtan-0.4.8/nehushtan/httpd/implement/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.616224 nehushtan-0.4.8/nehushtan/logger/
--rw-r--r--   0 leqee      (501) staff       (20)     7864 2021-06-08 07:13:03.000000 nehushtan-0.4.8/nehushtan/logger/NehushtanFileLogger.py
--rw-r--r--   0 leqee      (501) staff       (20)     4489 2021-03-23 02:59:30.000000 nehushtan-0.4.8/nehushtan/logger/NehushtanLogger.py
--rw-r--r--   0 leqee      (501) staff       (20)     1434 2021-03-05 06:13:46.000000 nehushtan-0.4.8/nehushtan/logger/NehushtanLogging.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/logger/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.621806 nehushtan-0.4.8/nehushtan/mail/
--rw-r--r--   0 leqee      (501) staff       (20)     7456 2021-07-14 02:32:54.000000 nehushtan-0.4.8/nehushtan/mail/IMAPAgent.py
--rw-r--r--   0 leqee      (501) staff       (20)     3696 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/mail/SMTPAgent.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/mail/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.623376 nehushtan-0.4.8/nehushtan/mail/rfc2047/
--rw-r--r--   0 leqee      (501) staff       (20)     1931 2021-07-01 07:33:06.000000 nehushtan-0.4.8/nehushtan/mail/rfc2047/EncodedWordsKit.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-07-01 04:18:25.000000 nehushtan-0.4.8/nehushtan/mail/rfc2047/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.624952 nehushtan-0.4.8/nehushtan/mail/rfc3501/
--rw-r--r--   0 leqee      (501) staff       (20)     9198 2021-07-01 07:33:49.000000 nehushtan-0.4.8/nehushtan/mail/rfc3501/SearchCommandKit.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-07-01 05:46:52.000000 nehushtan-0.4.8/nehushtan/mail/rfc3501/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.627903 nehushtan-0.4.8/nehushtan/mail/rfc822/
--rw-r--r--   0 leqee      (501) staff       (20)     2319 2021-07-14 02:53:20.000000 nehushtan-0.4.8/nehushtan/mail/rfc822/NehushtanEmailMessage.py
--rw-r--r--   0 leqee      (501) staff       (20)     2035 2021-07-14 03:56:26.000000 nehushtan-0.4.8/nehushtan/mail/rfc822/NehushtanMessagePart.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-07-01 02:54:24.000000 nehushtan-0.4.8/nehushtan/mail/rfc822/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.644829 nehushtan-0.4.8/nehushtan/multiprocessing/
--rw-r--r--   0 leqee      (501) staff       (20)     1062 2021-03-10 08:57:29.000000 nehushtan-0.4.8/nehushtan/multiprocessing/NehushtanMPJob.py
--rw-r--r--   0 leqee      (501) staff       (20)     6761 2021-03-11 08:32:58.000000 nehushtan-0.4.8/nehushtan/multiprocessing/NehushtanMPQueue.py
--rw-r--r--   0 leqee      (501) staff       (20)       92 2021-03-09 08:06:17.000000 nehushtan-0.4.8/nehushtan/multiprocessing/NehushtanMPTerminatedSituation.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-09 04:59:28.000000 nehushtan-0.4.8/nehushtan/multiprocessing/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.673148 nehushtan-0.4.8/nehushtan/mysql/
--rw-r--r--   0 leqee      (501) staff       (20)      634 2021-03-13 05:48:36.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLAnyTable.py
--rw-r--r--   0 leqee      (501) staff       (20)      627 2021-03-13 05:48:36.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLAnyView.py
--rw-r--r--   0 leqee      (501) staff       (20)    10608 2021-04-13 08:02:30.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLCondition.py
--rw-r--r--   0 leqee      (501) staff       (20)    10850 2021-04-20 10:28:04.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLKit.py
--rw-r--r--   0 leqee      (501) staff       (20)     1869 2020-12-30 15:03:34.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLKitConfig.py
--rw-r--r--   0 leqee      (501) staff       (20)     5437 2021-04-14 07:07:13.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLQueryResult.py
--rw-r--r--   0 leqee      (501) staff       (20)     3101 2021-04-20 10:27:22.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLSelectionMixin.py
--rw-r--r--   0 leqee      (501) staff       (20)      740 2021-03-13 05:40:46.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLTableExistence.py
--rw-r--r--   0 leqee      (501) staff       (20)    11784 2021-04-13 06:46:48.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLTableMixin.py
--rw-r--r--   0 leqee      (501) staff       (20)     4554 2021-04-20 10:27:22.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLTableSelection.py
--rw-r--r--   0 leqee      (501) staff       (20)     1282 2021-04-20 10:27:22.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLUnionSelection.py
--rw-r--r--   0 leqee      (501) staff       (20)      581 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/mysql/MySQLViewMixin.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/mysql/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.677592 nehushtan-0.4.8/nehushtan/mysql/constant/
--rw-r--r--   0 leqee      (501) staff       (20)     1237 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/mysql/constant/MySQLConditionConstant.py
--rw-r--r--   0 leqee      (501) staff       (20)      384 2021-04-13 06:44:51.000000 nehushtan-0.4.8/nehushtan/mysql/constant/MySQLQueryResultConstant.py
--rw-r--r--   0 leqee      (501) staff       (20)      164 2020-12-15 14:20:35.000000 nehushtan-0.4.8/nehushtan/mysql/constant/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.683330 nehushtan-0.4.8/nehushtan/queue/
--rw-r--r--   0 leqee      (501) staff       (20)    11973 2021-06-09 03:17:18.000000 nehushtan-0.4.8/nehushtan/queue/NehushtanQueue.py
--rw-r--r--   0 leqee      (501) staff       (20)     7609 2021-06-08 07:13:03.000000 nehushtan-0.4.8/nehushtan/queue/NehushtanQueueDelegate.py
--rw-r--r--   0 leqee      (501) staff       (20)     1610 2021-03-05 06:13:46.000000 nehushtan-0.4.8/nehushtan/queue/NehushtanQueueTask.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-30 15:03:34.000000 nehushtan-0.4.8/nehushtan/queue/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.688713 nehushtan-0.4.8/nehushtan/queue/situation/
--rw-r--r--   0 leqee      (501) staff       (20)       47 2021-01-12 08:20:12.000000 nehushtan-0.4.8/nehushtan/queue/situation/NoNextTaskSituation.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-30 15:03:34.000000 nehushtan-0.4.8/nehushtan/queue/situation/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.579103 nehushtan-0.4.8/nehushtan.egg-info/
--rw-r--r--   0 leqee      (501) staff       (20)     2070 2021-07-14 04:01:15.000000 nehushtan-0.4.8/nehushtan.egg-info/PKG-INFO
--rw-r--r--   0 leqee      (501) staff       (20)     4108 2021-07-14 04:01:15.000000 nehushtan-0.4.8/nehushtan.egg-info/SOURCES.txt
--rw-r--r--   0 leqee      (501) staff       (20)        1 2021-07-14 04:01:15.000000 nehushtan-0.4.8/nehushtan.egg-info/dependency_links.txt
--rw-r--r--   0 leqee      (501) staff       (20)       30 2021-07-14 04:01:15.000000 nehushtan-0.4.8/nehushtan.egg-info/requires.txt
--rw-r--r--   0 leqee      (501) staff       (20)       16 2021-07-14 04:01:15.000000 nehushtan-0.4.8/nehushtan.egg-info/top_level.txt
--rw-r--r--   0 leqee      (501) staff       (20)       38 2021-07-14 04:01:15.779616 nehushtan-0.4.8/setup.cfg
--rw-r--r--   0 leqee      (501) staff       (20)      752 2021-07-14 03:56:26.000000 nehushtan-0.4.8/setup.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.705216 nehushtan-0.4.8/tests/
--rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-30 15:03:34.000000 nehushtan-0.4.8/tests/__init__.py
--rw-r--r--   0 leqee      (501) staff       (20)      293 2020-12-24 17:44:42.000000 nehushtan-0.4.8/tests/config.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.710219 nehushtan-0.4.8/tests/httpd/
--rw-r--r--   0 leqee      (501) staff       (20)      979 2021-05-08 05:56:23.000000 nehushtan-0.4.8/tests/httpd/TestRequestHandler.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-29 03:12:43.000000 nehushtan-0.4.8/tests/httpd/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.712485 nehushtan-0.4.8/tests/httpd/filter/
--rw-r--r--   0 leqee      (501) staff       (20)      637 2021-05-06 08:57:52.000000 nehushtan-0.4.8/tests/httpd/filter/TestFilter.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-05-06 05:33:06.000000 nehushtan-0.4.8/tests/httpd/filter/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.715658 nehushtan-0.4.8/tests/httpd/process_chain/
--rw-r--r--   0 leqee      (501) staff       (20)      866 2021-04-30 10:20:20.000000 nehushtan-0.4.8/tests/httpd/process_chain/TestProcessChainA.py
--rw-r--r--   0 leqee      (501) staff       (20)     1087 2021-05-08 07:22:44.000000 nehushtan-0.4.8/tests/httpd/process_chain/TestProcessChainB.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-29 07:34:57.000000 nehushtan-0.4.8/tests/httpd/process_chain/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.717233 nehushtan-0.4.8/tests/httpd/process_chain/api/
--rw-r--r--   0 leqee      (501) staff       (20)      198 2021-05-06 05:34:01.000000 nehushtan-0.4.8/tests/httpd/process_chain/api/TestApi.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-05-06 05:31:11.000000 nehushtan-0.4.8/tests/httpd/process_chain/api/__init__.py
--rw-r--r--   0 leqee      (501) staff       (20)     1680 2021-05-08 06:44:54.000000 nehushtan-0.4.8/tests/httpd/test-for-httpd.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.718288 nehushtan-0.4.8/tests/logger/
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-01-25 04:51:40.000000 nehushtan-0.4.8/tests/logger/__init__.py
--rw-r--r--   0 leqee      (501) staff       (20)     1353 2021-05-12 05:40:56.000000 nehushtan-0.4.8/tests/logger/test-for-file-logger.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.723455 nehushtan-0.4.8/tests/mysql/
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-01-11 04:00:36.000000 nehushtan-0.4.8/tests/mysql/__init__.py
--rw-r--r--   0 leqee      (501) staff       (20)     1900 2021-04-13 07:36:29.000000 nehushtan-0.4.8/tests/mysql/benchmark-raw.py
--rw-r--r--   0 leqee      (501) staff       (20)     1081 2021-03-23 02:59:30.000000 nehushtan-0.4.8/tests/mysql/test-replace-lastrowid.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.765334 nehushtan-0.4.8/tests/queue/
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-01-21 07:45:05.000000 nehushtan-0.4.8/tests/queue/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.773086 nehushtan-0.4.8/tests/queue/plan2/
--rw-r--r--   0 leqee      (501) staff       (20)      270 2021-03-05 06:13:47.000000 nehushtan-0.4.8/tests/queue/plan2/Test2NehushtanQueue.py
--rw-r--r--   0 leqee      (501) staff       (20)     3060 2021-03-23 02:59:30.000000 nehushtan-0.4.8/tests/queue/plan2/Test2NehushtanQueueDelegate.py
--rw-r--r--   0 leqee      (501) staff       (20)     1275 2021-03-05 06:13:47.000000 nehushtan-0.4.8/tests/queue/plan2/Test2NehushtanQueueTask.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-05 06:13:47.000000 nehushtan-0.4.8/tests/queue/plan2/__init__.py
--rw-r--r--   0 leqee      (501) staff       (20)      561 2021-03-05 06:13:47.000000 nehushtan-0.4.8/tests/queue/plan2/main.py
--rw-r--r--   0 leqee      (501) staff       (20)      371 2021-01-21 08:08:21.000000 nehushtan-0.4.8/tests/queue/test-raw.py
--rw-r--r--   0 leqee      (501) staff       (20)     1195 2021-07-14 03:56:26.000000 nehushtan-0.4.8/tests/test-for-imap.py
--rw-r--r--   0 leqee      (501) staff       (20)     1252 2020-12-18 09:13:47.000000 nehushtan-0.4.8/tests/test-for-logger-reuse.py
--rw-r--r--   0 leqee      (501) staff       (20)     1153 2020-12-15 14:20:35.000000 nehushtan-0.4.8/tests/test-for-logger-sync.py
--rw-r--r--   0 leqee      (501) staff       (20)     2329 2020-12-15 14:20:35.000000 nehushtan-0.4.8/tests/test-for-logger.py
--rw-r--r--   0 leqee      (501) staff       (20)      418 2020-12-15 14:20:35.000000 nehushtan-0.4.8/tests/test-for-mysql-condition.py
--rw-r--r--   0 leqee      (501) staff       (20)      651 2020-12-15 14:20:35.000000 nehushtan-0.4.8/tests/test-for-mysql-kit.py
--rw-r--r--   0 leqee      (501) staff       (20)      541 2020-12-30 15:03:34.000000 nehushtan-0.4.8/tests/test-for-smtp.py
--rw-r--r--   0 leqee      (501) staff       (20)     1040 2021-03-23 02:59:30.000000 nehushtan-0.4.8/tests/test-for-table-mixin-type.py
--rw-r--r--   0 leqee      (501) staff       (20)     1963 2020-12-30 15:03:34.000000 nehushtan-0.4.8/tests/test-for-table.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.773839 nehushtan-0.4.8/tests/unit/
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-19 05:30:58.000000 nehushtan-0.4.8/tests/unit/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.775135 nehushtan-0.4.8/tests/unit/cli/
--rw-r--r--   0 leqee      (501) staff       (20)     1578 2021-03-22 08:05:24.000000 nehushtan-0.4.8/tests/unit/cli/TestForArgumentParser.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-19 06:41:05.000000 nehushtan-0.4.8/tests/unit/cli/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.776533 nehushtan-0.4.8/tests/unit/helper/
--rw-r--r--   0 leqee      (501) staff       (20)     3724 2021-03-22 06:14:50.000000 nehushtan-0.4.8/tests/unit/helper/TestForCommonHelper.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-19 05:31:08.000000 nehushtan-0.4.8/tests/unit/helper/__init__.py
-drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 04:01:15.777855 nehushtan-0.4.8/tests/unit/mysql/
--rw-r--r--   0 leqee      (501) staff       (20)     2596 2021-04-20 10:25:09.000000 nehushtan-0.4.8/tests/unit/mysql/TestForMySQLSelection.py
--rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-20 09:47:53.000000 nehushtan-0.4.8/tests/unit/mysql/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.293422 nehushtan-0.4.9/
+-rw-r--r--   0 leqee      (501) staff       (20)       17 2020-12-15 14:20:35.000000 nehushtan-0.4.9/MANIFEST.in
+-rw-r--r--   0 leqee      (501) staff       (20)     2070 2021-07-14 06:52:26.293139 nehushtan-0.4.9/PKG-INFO
+-rw-r--r--   0 leqee      (501) staff       (20)     1256 2021-03-22 08:53:28.000000 nehushtan-0.4.9/README.md
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.175261 nehushtan-0.4.9/nehushtan/
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.179566 nehushtan-0.4.9/nehushtan/cli/
+-rw-r--r--   0 leqee      (501) staff       (20)     6852 2021-03-22 08:04:50.000000 nehushtan-0.4.9/nehushtan/cli/NehushtanArgumentParser.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/cli/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.182582 nehushtan-0.4.9/nehushtan/helper/
+-rw-r--r--   0 leqee      (501) staff       (20)     4034 2021-04-21 09:32:51.000000 nehushtan-0.4.9/nehushtan/helper/CommonHelper.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1480 2021-03-05 10:34:43.000000 nehushtan-0.4.9/nehushtan/helper/SignalHandler.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/helper/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.194565 nehushtan-0.4.9/nehushtan/httpd/
+-rw-r--r--   0 leqee      (501) staff       (20)      498 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPConstant.py
+-rw-r--r--   0 leqee      (501) staff       (20)     4014 2021-05-06 10:01:26.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRequestController.py
+-rw-r--r--   0 leqee      (501) staff       (20)      787 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRequestFilter.py
+-rw-r--r--   0 leqee      (501) staff       (20)    14327 2021-05-11 07:55:36.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRequestHandler.py
+-rw-r--r--   0 leqee      (501) staff       (20)     3206 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPResponseBuffer.py
+-rw-r--r--   0 leqee      (501) staff       (20)      736 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRoute.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1333 2021-05-06 10:01:26.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRouter.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1763 2021-05-08 05:56:23.000000 nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPService.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-28 09:44:18.000000 nehushtan-0.4.9/nehushtan/httpd/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.203216 nehushtan-0.4.9/nehushtan/httpd/exceptions/
+-rw-r--r--   0 leqee      (501) staff       (20)      493 2021-05-06 10:01:26.000000 nehushtan-0.4.9/nehushtan/httpd/exceptions/NehushtanHTTPError.py
+-rw-r--r--   0 leqee      (501) staff       (20)      447 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/exceptions/NehushtanNoRouteMatchedError.py
+-rw-r--r--   0 leqee      (501) staff       (20)      458 2021-05-06 10:01:26.000000 nehushtan-0.4.9/nehushtan/httpd/exceptions/NehushtanRequestDeniedByFilterError.py
+-rw-r--r--   0 leqee      (501) staff       (20)      706 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/exceptions/NehushtanRequestParameterError.py
+-rw-r--r--   0 leqee      (501) staff       (20)      270 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/exceptions/NehushtanRequestProcessTargetError.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-29 05:40:51.000000 nehushtan-0.4.9/nehushtan/httpd/exceptions/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.207772 nehushtan-0.4.9/nehushtan/httpd/implement/
+-rw-r--r--   0 leqee      (501) staff       (20)     3305 2021-05-08 06:52:03.000000 nehushtan-0.4.9/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexArgs.py
+-rw-r--r--   0 leqee      (501) staff       (20)     2590 2021-05-08 06:46:11.000000 nehushtan-0.4.9/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexKwargs.py
+-rw-r--r--   0 leqee      (501) staff       (20)     3460 2021-05-06 09:53:49.000000 nehushtan-0.4.9/nehushtan/httpd/implement/NehushtanHTTPRouteWithRestFul.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-30 07:28:12.000000 nehushtan-0.4.9/nehushtan/httpd/implement/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.212918 nehushtan-0.4.9/nehushtan/logger/
+-rw-r--r--   0 leqee      (501) staff       (20)     7864 2021-06-08 07:13:03.000000 nehushtan-0.4.9/nehushtan/logger/NehushtanFileLogger.py
+-rw-r--r--   0 leqee      (501) staff       (20)     4489 2021-03-23 02:59:30.000000 nehushtan-0.4.9/nehushtan/logger/NehushtanLogger.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1434 2021-03-05 06:13:46.000000 nehushtan-0.4.9/nehushtan/logger/NehushtanLogging.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/logger/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.216488 nehushtan-0.4.9/nehushtan/mail/
+-rw-r--r--   0 leqee      (501) staff       (20)     7456 2021-07-14 02:32:54.000000 nehushtan-0.4.9/nehushtan/mail/IMAPAgent.py
+-rw-r--r--   0 leqee      (501) staff       (20)     3696 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/mail/SMTPAgent.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/mail/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.220416 nehushtan-0.4.9/nehushtan/mail/rfc2047/
+-rw-r--r--   0 leqee      (501) staff       (20)     1931 2021-07-01 07:33:06.000000 nehushtan-0.4.9/nehushtan/mail/rfc2047/EncodedWordsKit.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-07-01 04:18:25.000000 nehushtan-0.4.9/nehushtan/mail/rfc2047/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.221905 nehushtan-0.4.9/nehushtan/mail/rfc3501/
+-rw-r--r--   0 leqee      (501) staff       (20)     9198 2021-07-01 07:33:49.000000 nehushtan-0.4.9/nehushtan/mail/rfc3501/SearchCommandKit.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-07-01 05:46:52.000000 nehushtan-0.4.9/nehushtan/mail/rfc3501/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.225716 nehushtan-0.4.9/nehushtan/mail/rfc822/
+-rw-r--r--   0 leqee      (501) staff       (20)     2532 2021-07-14 05:43:10.000000 nehushtan-0.4.9/nehushtan/mail/rfc822/NehushtanEmailMessage.py
+-rw-r--r--   0 leqee      (501) staff       (20)     2038 2021-07-14 04:09:46.000000 nehushtan-0.4.9/nehushtan/mail/rfc822/NehushtanMessagePart.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-07-01 02:54:24.000000 nehushtan-0.4.9/nehushtan/mail/rfc822/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.229697 nehushtan-0.4.9/nehushtan/multiprocessing/
+-rw-r--r--   0 leqee      (501) staff       (20)     1062 2021-03-10 08:57:29.000000 nehushtan-0.4.9/nehushtan/multiprocessing/NehushtanMPJob.py
+-rw-r--r--   0 leqee      (501) staff       (20)     6761 2021-03-11 08:32:58.000000 nehushtan-0.4.9/nehushtan/multiprocessing/NehushtanMPQueue.py
+-rw-r--r--   0 leqee      (501) staff       (20)       92 2021-03-09 08:06:17.000000 nehushtan-0.4.9/nehushtan/multiprocessing/NehushtanMPTerminatedSituation.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-09 04:59:28.000000 nehushtan-0.4.9/nehushtan/multiprocessing/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.249318 nehushtan-0.4.9/nehushtan/mysql/
+-rw-r--r--   0 leqee      (501) staff       (20)      634 2021-03-13 05:48:36.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLAnyTable.py
+-rw-r--r--   0 leqee      (501) staff       (20)      627 2021-03-13 05:48:36.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLAnyView.py
+-rw-r--r--   0 leqee      (501) staff       (20)    10608 2021-04-13 08:02:30.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLCondition.py
+-rw-r--r--   0 leqee      (501) staff       (20)    10850 2021-04-20 10:28:04.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLKit.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1869 2020-12-30 15:03:34.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLKitConfig.py
+-rw-r--r--   0 leqee      (501) staff       (20)     5437 2021-04-14 07:07:13.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLQueryResult.py
+-rw-r--r--   0 leqee      (501) staff       (20)     3101 2021-04-20 10:27:22.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLSelectionMixin.py
+-rw-r--r--   0 leqee      (501) staff       (20)      740 2021-03-13 05:40:46.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLTableExistence.py
+-rw-r--r--   0 leqee      (501) staff       (20)    11784 2021-04-13 06:46:48.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLTableMixin.py
+-rw-r--r--   0 leqee      (501) staff       (20)     4554 2021-04-20 10:27:22.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLTableSelection.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1282 2021-04-20 10:27:22.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLUnionSelection.py
+-rw-r--r--   0 leqee      (501) staff       (20)      581 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/mysql/MySQLViewMixin.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/mysql/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.251969 nehushtan-0.4.9/nehushtan/mysql/constant/
+-rw-r--r--   0 leqee      (501) staff       (20)     1237 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/mysql/constant/MySQLConditionConstant.py
+-rw-r--r--   0 leqee      (501) staff       (20)      384 2021-04-13 06:44:51.000000 nehushtan-0.4.9/nehushtan/mysql/constant/MySQLQueryResultConstant.py
+-rw-r--r--   0 leqee      (501) staff       (20)      164 2020-12-15 14:20:35.000000 nehushtan-0.4.9/nehushtan/mysql/constant/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.257875 nehushtan-0.4.9/nehushtan/queue/
+-rw-r--r--   0 leqee      (501) staff       (20)    11973 2021-06-09 03:17:18.000000 nehushtan-0.4.9/nehushtan/queue/NehushtanQueue.py
+-rw-r--r--   0 leqee      (501) staff       (20)     7609 2021-06-08 07:13:03.000000 nehushtan-0.4.9/nehushtan/queue/NehushtanQueueDelegate.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1610 2021-03-05 06:13:46.000000 nehushtan-0.4.9/nehushtan/queue/NehushtanQueueTask.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-30 15:03:34.000000 nehushtan-0.4.9/nehushtan/queue/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.259478 nehushtan-0.4.9/nehushtan/queue/situation/
+-rw-r--r--   0 leqee      (501) staff       (20)       47 2021-01-12 08:20:12.000000 nehushtan-0.4.9/nehushtan/queue/situation/NoNextTaskSituation.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-30 15:03:34.000000 nehushtan-0.4.9/nehushtan/queue/situation/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.177831 nehushtan-0.4.9/nehushtan.egg-info/
+-rw-r--r--   0 leqee      (501) staff       (20)     2070 2021-07-14 06:52:25.000000 nehushtan-0.4.9/nehushtan.egg-info/PKG-INFO
+-rw-r--r--   0 leqee      (501) staff       (20)     4108 2021-07-14 06:52:25.000000 nehushtan-0.4.9/nehushtan.egg-info/SOURCES.txt
+-rw-r--r--   0 leqee      (501) staff       (20)        1 2021-07-14 06:52:25.000000 nehushtan-0.4.9/nehushtan.egg-info/dependency_links.txt
+-rw-r--r--   0 leqee      (501) staff       (20)       30 2021-07-14 06:52:25.000000 nehushtan-0.4.9/nehushtan.egg-info/requires.txt
+-rw-r--r--   0 leqee      (501) staff       (20)       16 2021-07-14 06:52:25.000000 nehushtan-0.4.9/nehushtan.egg-info/top_level.txt
+-rw-r--r--   0 leqee      (501) staff       (20)       38 2021-07-14 06:52:26.293504 nehushtan-0.4.9/setup.cfg
+-rw-r--r--   0 leqee      (501) staff       (20)      752 2021-07-14 06:51:33.000000 nehushtan-0.4.9/setup.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.270683 nehushtan-0.4.9/tests/
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2020-12-30 15:03:34.000000 nehushtan-0.4.9/tests/__init__.py
+-rw-r--r--   0 leqee      (501) staff       (20)      293 2020-12-24 17:44:42.000000 nehushtan-0.4.9/tests/config.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.272520 nehushtan-0.4.9/tests/httpd/
+-rw-r--r--   0 leqee      (501) staff       (20)      979 2021-05-08 05:56:23.000000 nehushtan-0.4.9/tests/httpd/TestRequestHandler.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-29 03:12:43.000000 nehushtan-0.4.9/tests/httpd/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.274587 nehushtan-0.4.9/tests/httpd/filter/
+-rw-r--r--   0 leqee      (501) staff       (20)      637 2021-05-06 08:57:52.000000 nehushtan-0.4.9/tests/httpd/filter/TestFilter.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-05-06 05:33:06.000000 nehushtan-0.4.9/tests/httpd/filter/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.278931 nehushtan-0.4.9/tests/httpd/process_chain/
+-rw-r--r--   0 leqee      (501) staff       (20)      866 2021-04-30 10:20:20.000000 nehushtan-0.4.9/tests/httpd/process_chain/TestProcessChainA.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1087 2021-05-08 07:22:44.000000 nehushtan-0.4.9/tests/httpd/process_chain/TestProcessChainB.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-29 07:34:57.000000 nehushtan-0.4.9/tests/httpd/process_chain/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.280431 nehushtan-0.4.9/tests/httpd/process_chain/api/
+-rw-r--r--   0 leqee      (501) staff       (20)      198 2021-05-06 05:34:01.000000 nehushtan-0.4.9/tests/httpd/process_chain/api/TestApi.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-05-06 05:31:11.000000 nehushtan-0.4.9/tests/httpd/process_chain/api/__init__.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1680 2021-05-08 06:44:54.000000 nehushtan-0.4.9/tests/httpd/test-for-httpd.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.280946 nehushtan-0.4.9/tests/logger/
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-01-25 04:51:40.000000 nehushtan-0.4.9/tests/logger/__init__.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1353 2021-05-12 05:40:56.000000 nehushtan-0.4.9/tests/logger/test-for-file-logger.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.283794 nehushtan-0.4.9/tests/mysql/
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-01-11 04:00:36.000000 nehushtan-0.4.9/tests/mysql/__init__.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1900 2021-04-13 07:36:29.000000 nehushtan-0.4.9/tests/mysql/benchmark-raw.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1081 2021-03-23 02:59:30.000000 nehushtan-0.4.9/tests/mysql/test-replace-lastrowid.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.285344 nehushtan-0.4.9/tests/queue/
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-01-21 07:45:05.000000 nehushtan-0.4.9/tests/queue/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.289323 nehushtan-0.4.9/tests/queue/plan2/
+-rw-r--r--   0 leqee      (501) staff       (20)      270 2021-03-05 06:13:47.000000 nehushtan-0.4.9/tests/queue/plan2/Test2NehushtanQueue.py
+-rw-r--r--   0 leqee      (501) staff       (20)     3060 2021-03-23 02:59:30.000000 nehushtan-0.4.9/tests/queue/plan2/Test2NehushtanQueueDelegate.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1275 2021-03-05 06:13:47.000000 nehushtan-0.4.9/tests/queue/plan2/Test2NehushtanQueueTask.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-05 06:13:47.000000 nehushtan-0.4.9/tests/queue/plan2/__init__.py
+-rw-r--r--   0 leqee      (501) staff       (20)      561 2021-03-05 06:13:47.000000 nehushtan-0.4.9/tests/queue/plan2/main.py
+-rw-r--r--   0 leqee      (501) staff       (20)      371 2021-01-21 08:08:21.000000 nehushtan-0.4.9/tests/queue/test-raw.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1195 2021-07-14 03:56:26.000000 nehushtan-0.4.9/tests/test-for-imap.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1252 2020-12-18 09:13:47.000000 nehushtan-0.4.9/tests/test-for-logger-reuse.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1153 2020-12-15 14:20:35.000000 nehushtan-0.4.9/tests/test-for-logger-sync.py
+-rw-r--r--   0 leqee      (501) staff       (20)     2329 2020-12-15 14:20:35.000000 nehushtan-0.4.9/tests/test-for-logger.py
+-rw-r--r--   0 leqee      (501) staff       (20)      418 2020-12-15 14:20:35.000000 nehushtan-0.4.9/tests/test-for-mysql-condition.py
+-rw-r--r--   0 leqee      (501) staff       (20)      651 2020-12-15 14:20:35.000000 nehushtan-0.4.9/tests/test-for-mysql-kit.py
+-rw-r--r--   0 leqee      (501) staff       (20)      541 2020-12-30 15:03:34.000000 nehushtan-0.4.9/tests/test-for-smtp.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1040 2021-03-23 02:59:30.000000 nehushtan-0.4.9/tests/test-for-table-mixin-type.py
+-rw-r--r--   0 leqee      (501) staff       (20)     1963 2020-12-30 15:03:34.000000 nehushtan-0.4.9/tests/test-for-table.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.289978 nehushtan-0.4.9/tests/unit/
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-19 05:30:58.000000 nehushtan-0.4.9/tests/unit/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.291031 nehushtan-0.4.9/tests/unit/cli/
+-rw-r--r--   0 leqee      (501) staff       (20)     1578 2021-03-22 08:05:24.000000 nehushtan-0.4.9/tests/unit/cli/TestForArgumentParser.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-19 06:41:05.000000 nehushtan-0.4.9/tests/unit/cli/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.291833 nehushtan-0.4.9/tests/unit/helper/
+-rw-r--r--   0 leqee      (501) staff       (20)     3724 2021-03-22 06:14:50.000000 nehushtan-0.4.9/tests/unit/helper/TestForCommonHelper.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-03-19 05:31:08.000000 nehushtan-0.4.9/tests/unit/helper/__init__.py
+drwxr-xr-x   0 leqee      (501) staff       (20)        0 2021-07-14 06:52:26.292788 nehushtan-0.4.9/tests/unit/mysql/
+-rw-r--r--   0 leqee      (501) staff       (20)     2596 2021-04-20 10:25:09.000000 nehushtan-0.4.9/tests/unit/mysql/TestForMySQLSelection.py
+-rw-r--r--   0 leqee      (501) staff       (20)        0 2021-04-20 09:47:53.000000 nehushtan-0.4.9/tests/unit/mysql/__init__.py
```

### Comparing `nehushtan-0.4.8/PKG-INFO` & `nehushtan-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nehushtan
-Version: 0.4.8
+Version: 0.4.9
 Summary: A toolkit for projects in Python
 Home-page: https://sinri.github.io/nehushtan/
 Author: Sinri Edogawa
 Author-email: e.joshua.s.e@gmail.com
 License: MIT
 Description: # Nehushtan (נְחֻשְׁתָּן)
```

### Comparing `nehushtan-0.4.8/README.md` & `nehushtan-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/cli/NehushtanArgumentParser.py` & `nehushtan-0.4.9/nehushtan/cli/NehushtanArgumentParser.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/helper/CommonHelper.py` & `nehushtan-0.4.9/nehushtan/helper/CommonHelper.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/helper/SignalHandler.py` & `nehushtan-0.4.9/nehushtan/helper/SignalHandler.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRequestController.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRequestController.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRequestFilter.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRequestFilter.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRequestHandler.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRequestHandler.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPResponseBuffer.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPResponseBuffer.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRoute.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRoute.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPRouter.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPRouter.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/NehushtanHTTPService.py` & `nehushtan-0.4.9/nehushtan/httpd/NehushtanHTTPService.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/exceptions/NehushtanRequestParameterError.py` & `nehushtan-0.4.9/nehushtan/httpd/exceptions/NehushtanRequestParameterError.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexArgs.py` & `nehushtan-0.4.9/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexArgs.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexKwargs.py` & `nehushtan-0.4.9/nehushtan/httpd/implement/NehushtanHTTPRouteWithRegexKwargs.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/httpd/implement/NehushtanHTTPRouteWithRestFul.py` & `nehushtan-0.4.9/nehushtan/httpd/implement/NehushtanHTTPRouteWithRestFul.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/logger/NehushtanFileLogger.py` & `nehushtan-0.4.9/nehushtan/logger/NehushtanFileLogger.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/logger/NehushtanLogger.py` & `nehushtan-0.4.9/nehushtan/logger/NehushtanLogger.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/logger/NehushtanLogging.py` & `nehushtan-0.4.9/nehushtan/logger/NehushtanLogging.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mail/IMAPAgent.py` & `nehushtan-0.4.9/nehushtan/mail/IMAPAgent.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mail/SMTPAgent.py` & `nehushtan-0.4.9/nehushtan/mail/SMTPAgent.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mail/rfc2047/EncodedWordsKit.py` & `nehushtan-0.4.9/nehushtan/mail/rfc2047/EncodedWordsKit.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mail/rfc3501/SearchCommandKit.py` & `nehushtan-0.4.9/nehushtan/mail/rfc3501/SearchCommandKit.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mail/rfc822/NehushtanEmailMessage.py` & `nehushtan-0.4.9/nehushtan/mail/rfc822/NehushtanEmailMessage.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,7 +69,15 @@
             elif address_piece[2] and address_piece[3]:
                 address = address_piece[3]
                 name = address_piece[2]
                 # EncodedWordsKit.decode_string_following_rfc2047(name)
 
             list_of_mail_address_tuple.append((address, name))
         return list_of_mail_address_tuple
+
+    @staticmethod
+    def extract_email_address(x: str):
+        """
+        Since 0.4.9
+        """
+        email_rule_express = r'[A-Za-z0-9.-]+@[A-Za-z0-9.-]+'
+        return re.findall(email_rule_express, x)
```

### Comparing `nehushtan-0.4.8/nehushtan/mail/rfc822/NehushtanMessagePart.py` & `nehushtan-0.4.9/nehushtan/mail/rfc822/NehushtanMessagePart.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def get_message(self):
         return self.__message
 
     def get_sub_message_list(self):
         return self.__sub_message_list
 
     def is_leaf(self):
-        return len(self.__sub_message_list)==0
+        return len(self.__sub_message_list) == 0
 
     # def append_sub_message(self, sub_message):
     #     self.__sub_message_list.append(sub_message)
     #     return self
 
     def __organize_parts(self):
         if self.__message.is_multipart():
@@ -41,15 +41,15 @@
     def get_content_type(self):
         return self.__message.get_content_type()
 
     def get_content_disposition(self):
         return self.__message.get_content_disposition()
 
     def get_body_content(self, i=None):
-        x:bytes = self.__message.get_payload(i=i, decode=True)
+        x: bytes = self.__message.get_payload(i=i, decode=True)
         return x.decode(encoding=self.__message.get_content_charset('ascii'))
 
     def get_attachement_filename_of_this_part(self) -> Optional[str]:
         if self.__message.is_attachment():
             return self.__message.get_filename()
 
     def get_attachement_content_of_this_part(self, i=None):
```

### Comparing `nehushtan-0.4.8/nehushtan/multiprocessing/NehushtanMPJob.py` & `nehushtan-0.4.9/nehushtan/multiprocessing/NehushtanMPJob.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/multiprocessing/NehushtanMPQueue.py` & `nehushtan-0.4.9/nehushtan/multiprocessing/NehushtanMPQueue.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLAnyTable.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLAnyTable.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLAnyView.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLAnyView.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLCondition.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLCondition.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLKit.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLKit.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLKitConfig.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLKitConfig.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLQueryResult.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLQueryResult.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLSelectionMixin.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLSelectionMixin.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLTableExistence.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLTableExistence.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLTableMixin.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLTableMixin.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLTableSelection.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLTableSelection.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLUnionSelection.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLUnionSelection.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/MySQLViewMixin.py` & `nehushtan-0.4.9/nehushtan/mysql/MySQLViewMixin.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/mysql/constant/MySQLConditionConstant.py` & `nehushtan-0.4.9/nehushtan/mysql/constant/MySQLConditionConstant.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/queue/NehushtanQueue.py` & `nehushtan-0.4.9/nehushtan/queue/NehushtanQueue.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/queue/NehushtanQueueDelegate.py` & `nehushtan-0.4.9/nehushtan/queue/NehushtanQueueDelegate.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan/queue/NehushtanQueueTask.py` & `nehushtan-0.4.9/nehushtan/queue/NehushtanQueueTask.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/nehushtan.egg-info/PKG-INFO` & `nehushtan-0.4.9/nehushtan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nehushtan
-Version: 0.4.8
+Version: 0.4.9
 Summary: A toolkit for projects in Python
 Home-page: https://sinri.github.io/nehushtan/
 Author: Sinri Edogawa
 Author-email: e.joshua.s.e@gmail.com
 License: MIT
 Description: # Nehushtan (נְחֻשְׁתָּן)
```

### Comparing `nehushtan-0.4.8/nehushtan.egg-info/SOURCES.txt` & `nehushtan-0.4.9/nehushtan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/setup.py` & `nehushtan-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='nehushtan',
-    version='0.4.8',
+    version='0.4.9',
     packages=find_packages(),
     url='https://sinri.github.io/nehushtan/',
     license='MIT',
     author='Sinri Edogawa',
     author_email='e.joshua.s.e@gmail.com',
     description='A toolkit for projects in Python',
     long_description=long_description,
```

### Comparing `nehushtan-0.4.8/tests/httpd/TestRequestHandler.py` & `nehushtan-0.4.9/tests/httpd/TestRequestHandler.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/httpd/filter/TestFilter.py` & `nehushtan-0.4.9/tests/httpd/filter/TestFilter.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/httpd/process_chain/TestProcessChainA.py` & `nehushtan-0.4.9/tests/httpd/process_chain/TestProcessChainA.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/httpd/process_chain/TestProcessChainB.py` & `nehushtan-0.4.9/tests/httpd/process_chain/TestProcessChainB.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/httpd/test-for-httpd.py` & `nehushtan-0.4.9/tests/httpd/test-for-httpd.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/logger/test-for-file-logger.py` & `nehushtan-0.4.9/tests/logger/test-for-file-logger.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/mysql/benchmark-raw.py` & `nehushtan-0.4.9/tests/mysql/benchmark-raw.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/mysql/test-replace-lastrowid.py` & `nehushtan-0.4.9/tests/mysql/test-replace-lastrowid.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/queue/plan2/Test2NehushtanQueueDelegate.py` & `nehushtan-0.4.9/tests/queue/plan2/Test2NehushtanQueueDelegate.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/queue/plan2/Test2NehushtanQueueTask.py` & `nehushtan-0.4.9/tests/queue/plan2/Test2NehushtanQueueTask.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/queue/plan2/main.py` & `nehushtan-0.4.9/tests/queue/plan2/main.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-imap.py` & `nehushtan-0.4.9/tests/test-for-imap.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-logger-reuse.py` & `nehushtan-0.4.9/tests/test-for-logger-reuse.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-logger-sync.py` & `nehushtan-0.4.9/tests/test-for-logger-sync.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-logger.py` & `nehushtan-0.4.9/tests/test-for-logger.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-mysql-kit.py` & `nehushtan-0.4.9/tests/test-for-mysql-kit.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-smtp.py` & `nehushtan-0.4.9/tests/test-for-smtp.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-table-mixin-type.py` & `nehushtan-0.4.9/tests/test-for-table-mixin-type.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/test-for-table.py` & `nehushtan-0.4.9/tests/test-for-table.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/unit/cli/TestForArgumentParser.py` & `nehushtan-0.4.9/tests/unit/cli/TestForArgumentParser.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/unit/helper/TestForCommonHelper.py` & `nehushtan-0.4.9/tests/unit/helper/TestForCommonHelper.py`

 * *Files identical despite different names*

### Comparing `nehushtan-0.4.8/tests/unit/mysql/TestForMySQLSelection.py` & `nehushtan-0.4.9/tests/unit/mysql/TestForMySQLSelection.py`

 * *Files identical despite different names*

