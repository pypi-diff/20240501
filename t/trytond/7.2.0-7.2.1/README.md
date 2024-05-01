# Comparing `tmp/trytond-7.2.0.tar.gz` & `tmp/trytond-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond-7.2.0.tar", last modified: Mon Apr 29 15:55:40 2024, max compression
+gzip compressed data, was "trytond-7.2.1.tar", last modified: Wed May  1 09:08:01 2024, max compression
```

## Comparing `trytond-7.2.0.tar` & `trytond-7.2.1.tar`

### file list

```diff
@@ -1,609 +1,609 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.988837 trytond-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)    41204 2024-04-29 15:31:10.000000 trytond-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-04-29 15:31:09.000000 trytond-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-04-15 07:12:15.000000 trytond-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-29 15:55:40.988837 trytond-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-04-15 07:12:16.000000 trytond-7.2.0/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2890 2024-04-27 16:30:39.000000 trytond-7.2.0/bin/trytond
--rwxr-xr-x   0 ced       (1000) ced       (1000)      878 2024-04-22 12:14:37.000000 trytond-7.2.0/bin/trytond-admin
--rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-04-15 07:12:15.000000 trytond-7.2.0/bin/trytond-console
--rwxr-xr-x   0 ced       (1000) ced       (1000)      949 2024-04-27 16:30:39.000000 trytond-7.2.0/bin/trytond-cron
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-04-15 07:12:16.000000 trytond-7.2.0/bin/trytond-stat
--rwxr-xr-x   0 ced       (1000) ced       (1000)     1088 2024-04-27 16:30:39.000000 trytond-7.2.0/bin/trytond-worker
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2367 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/doc/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/doc/modules/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     3741 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/res/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/modules/res/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/res/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/res/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/ref/
--rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/backend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2656 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/cache.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/exceptions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    32469 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/ref/filestore.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/ref/i18n.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    33575 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/models.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/pool.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/ref/pyson.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-03-17 11:01:36.000000 trytond-7.2.0/doc/ref/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2640 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/sendmail.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4738 2024-04-26 10:28:17.000000 trytond-7.2.0/doc/ref/tests.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/ref/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/barcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/tools/email.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/tools/immutabledict.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/logging.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1959 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/ref/tools/misc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/qrcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/tools/singleton.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/tools/timezone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5550 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/ref/transaction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6064 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/ref/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-13 17:12:23.000000 trytond-7.2.0/doc/topics/access_rights.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/actions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4014 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/topics/backend_types.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14914 2024-03-17 11:01:36.000000 trytond-7.2.0/doc/topics/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/cron.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/domain.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/topics/install.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/logs.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/models/
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/topics/models/fields_default_value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/models/fields_on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/models/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-10-24 13:25:05.000000 trytond-7.2.0/doc/topics/modules/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/pyson.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/reports/
--rw-r--r--   0 ced       (1000) ced       (1000)     8742 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/topics/reports/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2024-02-26 09:40:58.000000 trytond-7.2.0/doc/topics/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/start_server.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/task_queue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2884 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/topics/testing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/translation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/triggers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2024-04-26 10:38:57.000000 trytond-7.2.0/doc/topics/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/user_errors_warnings.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.948838 trytond-7.2.0/doc/topics/views/
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/views/extension.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    25819 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/topics/views/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/wizard.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.948838 trytond-7.2.0/doc/tutorial/
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.948838 trytond-7.2.0/doc/tutorial/module/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/anatomy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/default_values.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/domains.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/extend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/function_fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3949 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/tutorial/module/model.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3727 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/tutorial/module/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/tutorial/module/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/states.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4746 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/tutorial/module/table_query.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5047 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/tutorial/module/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4727 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/tutorial/module/workflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:55:40.988837 trytond-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5625 2024-04-27 16:30:39.000000 trytond-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      624 2024-03-17 11:01:36.000000 trytond-7.2.0/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-29 15:31:05.000000 trytond-7.2.0/trytond/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6968 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/admin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1455 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/application.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/backend/
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4455 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/database.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/backend/postgresql/
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/postgresql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26951 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/backend/postgresql/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4829 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/postgresql/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    29327 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/postgresql/table.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/backend/sqlite/
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/sqlite/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20807 2024-04-01 22:30:57.000000 trytond-7.2.0/trytond/backend/sqlite/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/sqlite/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    15183 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/sqlite/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4248 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16924 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7715 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/commandline.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-13 17:12:23.000000 trytond-7.2.0/trytond/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2280 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/console.py
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31204 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/convert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-10-07 21:28:39.000000 trytond-7.2.0/trytond/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2098 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/i18n.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.955505 trytond-7.2.0/trytond/ir/
--rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    40622 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10524 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/action.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2865 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/attachment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6508 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-01 10:31:26.000000 trytond-7.2.0/trytond/ir/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/ir/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4282 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/calendar_.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7912 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/cron.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2024-02-07 17:19:02.000000 trytond-7.2.0/trytond/ir/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4502 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/email.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20520 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6087 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/error.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3523 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/error.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/export.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/export.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.955505 trytond-7.2.0/trytond/ir/fonts/
--rw-r--r--   0 ced       (1000) ced       (1000)     4384 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/fonts/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    58284 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/fonts/karla.ttf
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22311 2024-04-07 14:43:04.000000 trytond-7.2.0/trytond/ir/lang.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27181 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/lang.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.958838 trytond-7.2.0/trytond/ir/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   101916 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   101483 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88269 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103114 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   102346 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82984 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    95005 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   104146 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87944 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103187 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97890 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87741 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97492 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93391 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93357 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100910 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100618 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98326 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100578 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   104248 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96213 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88080 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   113027 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97870 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/message.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22606 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    64603 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15908 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/model.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    18462 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/ir/module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8238 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/module.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/ir/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/note.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/queue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9479 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/queue_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7910 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10185 2024-04-26 10:38:57.000000 trytond-7.2.0/trytond/ir/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12027 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16164 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4927 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5562 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/ir/session.py
--rw-r--r--   0 ced       (1000) ced       (1000)    67671 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/translation.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/translation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11517 2024-04-03 14:12:24.000000 trytond-7.2.0/trytond/ir/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/trigger.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.958838 trytond-7.2.0/trytond/ir/ui/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/board.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    18063 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/board.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/ui/calendar.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     3508 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/calendar.rng
--rw-r--r--   0 ced       (1000) ced       (1000)    10397 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/form.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    35542 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/form.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/graph.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5214 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/graph.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/icon.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/icon.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.958838 trytond-7.2.0/trytond/ir/ui/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/ui/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-board.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-calendar.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-folder.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-form.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-graph.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-list.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-settings.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-tree.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    10200 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/ui/menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2962 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/menu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3895 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/ui/tree.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/tree.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/ui.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    26813 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/view.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8412 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/view.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.968838 trytond-7.2.0/trytond/ir/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_domain_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_domain_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_domain_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_act_window_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_act_window_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-06-23 11:39:44.000000 trytond-7.2.0/trytond/ir/view/action_act_window_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_view_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      952 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/action_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1358 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_report_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_report_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_url_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_url_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_wizard_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_wizard_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/attachment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/attachment_form_preview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/attachment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/email_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/error_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/error_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/export_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/export_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/icon_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/icon_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/lang_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/lang_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/lang_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/model_button_click_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/view/model_button_click_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_button_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_button_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/model_button_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/model_button_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_data_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_data_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      388 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/view/model_log_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/view/model_log_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/model_print_model_graph_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_activate_upgrade_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_activate_upgrade_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/module_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_first_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_item_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_other_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_dependency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_dependency_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/module_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/note_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/note_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/rule_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/rule_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/view/sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/sequence_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_clean_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_clean_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/translation_export_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/translation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/translation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_set_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_set_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/translation_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1035 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/trigger_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/trigger_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_menu_favorite_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/ui_menu_favorite_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/ui_menu_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_menu_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_menu_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      859 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_list_extension.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_search_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_optional_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_optional_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_state_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_state_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_width_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_width_list.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.968838 trytond-7.2.0/trytond/model/
--rw-r--r--   0 ced       (1000) ced       (1000)     1199 2024-02-22 16:15:03.000000 trytond-7.2.0/trytond/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/active.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1050 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/model/descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9327 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/dictschema.py
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/digits.py
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/model/fields/
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/fields/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/model/fields/boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9426 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/fields/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7052 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8365 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/fields/dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26432 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/model/fields/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3164 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/fmany2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8403 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/fields/function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18816 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/fields/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14114 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4401 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/fields/numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16101 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/fields/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/model/fields/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8415 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/fields/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7508 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3439 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/text.py
--rw-r--r--   0 ced       (1000) ced       (1000)      899 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/match.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17673 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-07 14:43:13.000000 trytond-7.2.0/trytond/model/modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    90408 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    84791 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    38145 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/model/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2712 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/order.py
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/symbol.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/union.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/workflow.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)    13764 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/modules/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8803 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/pool.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/protocols/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/protocols/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9185 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/protocols/dispatcher.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5827 2024-04-18 16:40:25.000000 trytond-7.2.0/trytond/protocols/jsonrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10447 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/protocols/wrappers.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-10-07 21:54:42.000000 trytond-7.2.0/trytond/protocols/xmlrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24260 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/report/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/report/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20078 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/report/report.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     1235 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1496 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/res/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2430 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/group.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8327 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22621 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.975504 trytond-7.2.0/trytond/res/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    13763 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14072 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12042 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14246 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14217 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11652 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13112 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14122 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14674 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13523 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12552 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12870 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15494 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13624 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14006 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13892 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13963 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13949 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13969 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15820 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13532 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1570 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2458 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)    43182 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7748 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.975504 trytond-7.2.0/trytond/res/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1153 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-08-27 09:41:33.000000 trytond-7.2.0/trytond/res/view/user_application_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-08-27 09:41:33.000000 trytond-7.2.0/trytond/res/view/user_application_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/user_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1527 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/res/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1386 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/res/view/user_form_preferences.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/res/view/user_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/res/view/user_warning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/res/view/user_warning_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3973 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/security.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5662 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3227 2024-04-13 17:12:23.000000 trytond-7.2.0/trytond/status.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/copy_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2023 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/export_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_function.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7491 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5212 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3161 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1489 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1224 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)        9 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/forbidden.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      917 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/import_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/import_data.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1069 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4719 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1493 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8936 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7720 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8965 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/modelview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/path.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)      971 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36123 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6920 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/test_backend.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12678 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_copy.py
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15266 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_exportdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7404 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-10-21 11:43:01.000000 trytond-7.2.0/trytond/tests/test_field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-08-15 21:07:26.000000 trytond-7.2.0/trytond/tests/test_field_depends.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3641 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10446 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25088 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15103 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12677 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17303 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23590 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9827 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20622 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9360 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17308 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3794 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_i18n.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20525 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/test_importdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19232 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_mixins.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17190 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6973 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_model_index.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4808 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_model_match.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    61345 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31037 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31080 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/tests/test_modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3450 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_path.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_protocols.py
--rw-r--r--   0 ced       (1000) ced       (1000)    36764 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2413 2024-02-26 09:40:58.000000 trytond-7.2.0/trytond/tests/test_res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6365 2024-02-25 16:44:42.000000 trytond-7.2.0/trytond/tests/test_routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-08-16 08:35:53.000000 trytond-7.2.0/trytond/tests/test_rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25750 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4299 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5462 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)    48966 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/test_transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12469 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)    45182 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_tryton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_union.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11366 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5406 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3171 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_wsgi.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1307 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-07-23 09:59:26.000000 trytond-7.2.0/trytond/tests/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/workflow.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tools/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tools/barcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/decimal_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tools/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2562 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tools/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/gevent.py
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/immutabledict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-04-18 16:16:44.000000 trytond-7.2.0/trytond/tools/logging.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9631 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tools/misc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1595 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tools/qrcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tools/singleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-07 14:01:56.000000 trytond-7.2.0/trytond/tools/string_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/timezone.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12819 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1445 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tryton.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/tryton.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2754 2024-02-26 09:40:58.000000 trytond-7.2.0/trytond/url.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond/wizard/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/wizard/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15037 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/wizard/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/worker.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9735 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/wsgi.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond-7.2.0/trytond.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.671817 trytond-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41305 2024-05-01 09:07:58.000000 trytond-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-05-01 09:07:58.000000 trytond-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2024-04-30 17:21:00.000000 trytond-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-05-01 09:08:01.668483 trytond-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2024-04-30 17:21:00.000000 trytond-7.2.1/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2890 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      878 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-admin
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-console
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      949 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-cron
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-stat
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     1088 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-worker
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2367 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/modules/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3741 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/ref/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/backend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2656 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/cache.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/exceptions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    32469 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1171 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/filestore.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/i18n.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    33575 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/models.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/pool.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8787 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/pyson.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2640 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/sendmail.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4738 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tests.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/ref/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/barcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/email.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/immutabledict.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/logging.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1959 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/misc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/qrcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/singleton.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      608 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/timezone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5550 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/transaction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6064 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/access_rights.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/actions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4014 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/backend_types.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14914 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1431 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/cron.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7848 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/domain.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/install.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1108 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/logs.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/models/
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/models/fields_default_value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/models/fields_on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1376 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/models/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6022 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/modules/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3887 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/pyson.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/reports/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8742 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/reports/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/start_server.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/task_queue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2884 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/testing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/translation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/triggers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/user_errors_warnings.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/views/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/views/extension.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    25819 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/views/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1669 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/wizard.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/tutorial/
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/doc/tutorial/module/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/anatomy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/default_values.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3334 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/domains.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2917 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/extend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3524 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/function_fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3949 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/model.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2662 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3727 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/states.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4746 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/table_query.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6258 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5047 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4727 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/workflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:08:01.671817 trytond-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5625 2024-04-30 17:21:00.000000 trytond-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      624 2024-04-30 17:21:00.000000 trytond-7.2.1/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/trytond/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-30 17:21:06.000000 trytond-7.2.1/trytond/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6968 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/admin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1455 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/application.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/trytond/backend/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4455 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/database.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/trytond/backend/postgresql/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26951 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4829 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    29327 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/table.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.635151 trytond-7.2.1/trytond/backend/sqlite/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20807 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    15183 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4248 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9431 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16924 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7715 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/commandline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2280 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/console.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31204 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/convert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2098 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/i18n.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.638484 trytond-7.2.1/trytond/ir/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    40622 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10524 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/action.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2865 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1960 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/attachment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4282 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/calendar_.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1459 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7912 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/cron.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4502 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/email.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20520 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6087 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/error.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3523 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/error.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/export.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.638484 trytond-7.2.1/trytond/ir/fonts/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4384 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/fonts/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    58284 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/fonts/karla.ttf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22311 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/lang.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27181 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/lang.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.638484 trytond-7.2.1/trytond/ir/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   104527 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103796 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90725 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   105509 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   104656 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85420 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97499 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   106723 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90400 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   105628 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100392 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90128 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100022 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95895 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95896 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103249 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103641 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100851 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103060 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   106898 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    98720 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90532 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   115724 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100387 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/message.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22606 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    64603 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15908 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/model.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    18462 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8238 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/module.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4199 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/note.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/queue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9479 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/queue_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7910 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10185 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12027 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16164 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4927 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/session.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    67671 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/translation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7726 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/translation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11517 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/trigger.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.641817 trytond-7.2.1/trytond/ir/ui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/board.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    18063 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/board.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/calendar.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     3508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/calendar.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)    10397 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/form.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    35542 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/form.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/graph.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5214 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/graph.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icon.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1521 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icon.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.641817 trytond-7.2.1/trytond/ir/ui/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-board.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-calendar.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-folder.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-form.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-graph.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-list.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-settings.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-tree.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    10200 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2962 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/menu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3895 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/tree.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/tree.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/ui.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    26813 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/view.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8412 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.648484 trytond-7.2.1/trytond/ir/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_domain_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_domain_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_domain_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_view_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      952 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1358 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_report_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_report_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_url_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_url_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_wizard_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_wizard_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/attachment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/attachment_form_preview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/attachment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1204 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/error_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/error_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/icon_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/icon_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/lang_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/lang_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/lang_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_click_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_click_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_data_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_data_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      682 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      388 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_log_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_log_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_print_model_graph_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_activate_upgrade_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_activate_upgrade_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_first_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_item_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_other_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_dependency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_dependency_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/note_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/note_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_clean_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_clean_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_export_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_set_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_set_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1035 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/trigger_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/trigger_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_favorite_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_favorite_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      859 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_list_extension.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_search_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_optional_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_optional_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_state_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_state_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_width_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_width_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.651817 trytond-7.2.1/trytond/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1199 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/active.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1050 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9327 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/dictschema.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/digits.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.651817 trytond-7.2.1/trytond/model/fields/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4592 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9426 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7052 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8365 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26432 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2603 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3164 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/fmany2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8403 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18816 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14114 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4401 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16101 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2116 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8415 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3439 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      899 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17673 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    90408 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    84791 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    38145 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2712 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/symbol.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/workflow.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.651817 trytond-7.2.1/trytond/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13764 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/modules/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8803 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/pool.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/protocols/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9185 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/dispatcher.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5827 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/jsonrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10447 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/wrappers.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5602 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/xmlrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/report/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/report/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20078 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/report/report.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1235 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1496 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2430 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/group.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8327 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22621 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/res/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13763 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14164 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12042 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14493 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14297 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11652 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13112 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14122 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14674 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13523 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12552 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12870 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15494 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13624 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14229 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14286 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13963 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13949 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13969 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15820 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13532 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1570 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2458 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)    43182 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7748 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.658484 trytond-7.2.1/trytond/res/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1153 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_application_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_application_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1527 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1386 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_form_preferences.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_warning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_warning_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3973 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/security.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5662 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3227 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/status.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1202 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/copy_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2023 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/export_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2372 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_function.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7491 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3161 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1981 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1489 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1224 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)        9 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/forbidden.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5599 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/import_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/import_data.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1069 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1083 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4719 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1493 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8936 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7720 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8965 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      971 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36123 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6920 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_backend.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12678 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_copy.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15266 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_exportdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7404 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7503 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22837 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1021 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13633 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15520 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7608 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_depends.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27461 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13029 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3641 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10446 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25088 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15103 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12677 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17303 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23590 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9827 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20622 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9360 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19472 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15036 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3019 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17308 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3794 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_i18n.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20525 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_importdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19232 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_mixins.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17190 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6973 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model_index.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4808 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model_match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    61345 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31037 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31080 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3450 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8733 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3726 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_protocols.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    36764 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2413 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6365 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4377 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25750 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4299 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5462 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    48966 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12469 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15386 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    45182 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_tryton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3353 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11366 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5406 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3171 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_wsgi.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1307 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1180 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/workflow.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2592 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/barcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/decimal_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/gevent.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/immutabledict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/logging.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9631 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/misc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1595 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/qrcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/singleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/string_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/timezone.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12819 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tryton.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tryton.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2754 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/url.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond/wizard/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/wizard/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15037 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/wizard/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/worker.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9735 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/wsgi.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/top_level.txt
```

### Comparing `trytond-7.2.0/CHANGELOG` & `trytond-7.2.1/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.1 - 2024-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Do not accept compressed content from unauthenticated request (#13142)
 * Set loading eager to visible xxx2many on form view
 * Add loading attribute to form view
 * Add a contextual read limit on Model.read
```

### Comparing `trytond-7.2.0/COPYRIGHT` & `trytond-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/LICENSE` & `trytond-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/PKG-INFO` & `trytond-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton server
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond-7.2.0/bin/trytond` & `trytond-7.2.1/bin/trytond`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/bin/trytond-admin` & `trytond-7.2.1/bin/trytond-admin`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/bin/trytond-console` & `trytond-7.2.1/bin/trytond-console`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/bin/trytond-cron` & `trytond-7.2.1/bin/trytond-cron`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/bin/trytond-stat` & `trytond-7.2.1/bin/trytond-stat`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/bin/trytond-worker` & `trytond-7.2.1/bin/trytond-worker`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/conf.py` & `trytond-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/index.rst` & `trytond-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/modules/res/design.rst` & `trytond-7.2.1/doc/modules/res/design.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/modules/res/setup.rst` & `trytond-7.2.1/doc/modules/res/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/modules/res/usage.rst` & `trytond-7.2.1/doc/modules/res/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/backend.rst` & `trytond-7.2.1/doc/ref/backend.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/bus.rst` & `trytond-7.2.1/doc/ref/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/cache.rst` & `trytond-7.2.1/doc/ref/cache.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/exceptions.rst` & `trytond-7.2.1/doc/ref/exceptions.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/fields.rst` & `trytond-7.2.1/doc/ref/fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/filestore.rst` & `trytond-7.2.1/doc/ref/filestore.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/i18n.rst` & `trytond-7.2.1/doc/ref/i18n.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/models.rst` & `trytond-7.2.1/doc/ref/models.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/pool.rst` & `trytond-7.2.1/doc/ref/pool.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/pyson.rst` & `trytond-7.2.1/doc/ref/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/rpc.rst` & `trytond-7.2.1/doc/ref/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/sendmail.rst` & `trytond-7.2.1/doc/ref/sendmail.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/tests.rst` & `trytond-7.2.1/doc/ref/tests.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/tools/barcode.rst` & `trytond-7.2.1/doc/ref/tools/barcode.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/tools/email.rst` & `trytond-7.2.1/doc/ref/tools/email.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/tools/logging.rst` & `trytond-7.2.1/doc/ref/tools/logging.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/tools/misc.rst` & `trytond-7.2.1/doc/ref/tools/misc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/tools/timezone.rst` & `trytond-7.2.1/doc/ref/tools/timezone.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/transaction.rst` & `trytond-7.2.1/doc/ref/transaction.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/ref/wizard.rst` & `trytond-7.2.1/doc/ref/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/access_rights.rst` & `trytond-7.2.1/doc/topics/access_rights.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/actions.rst` & `trytond-7.2.1/doc/topics/actions.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/backend_types.rst` & `trytond-7.2.1/doc/topics/backend_types.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/bus.rst` & `trytond-7.2.1/doc/topics/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/configuration.rst` & `trytond-7.2.1/doc/topics/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/cron.rst` & `trytond-7.2.1/doc/topics/cron.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/domain.rst` & `trytond-7.2.1/doc/topics/domain.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/index.rst` & `trytond-7.2.1/doc/topics/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/install.rst` & `trytond-7.2.1/doc/topics/install.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/logs.rst` & `trytond-7.2.1/doc/topics/logs.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/models/fields_default_value.rst` & `trytond-7.2.1/doc/topics/models/fields_default_value.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/models/fields_on_change.rst` & `trytond-7.2.1/doc/topics/models/fields_on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/models/index.rst` & `trytond-7.2.1/doc/topics/models/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/modules/index.rst` & `trytond-7.2.1/doc/topics/modules/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/pyson.rst` & `trytond-7.2.1/doc/topics/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/reports/index.rst` & `trytond-7.2.1/doc/topics/reports/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/rpc.rst` & `trytond-7.2.1/doc/topics/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/setup_database.rst` & `trytond-7.2.1/doc/topics/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/start_server.rst` & `trytond-7.2.1/doc/topics/start_server.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/task_queue.rst` & `trytond-7.2.1/doc/topics/task_queue.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/testing.rst` & `trytond-7.2.1/doc/topics/testing.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/translation.rst` & `trytond-7.2.1/doc/topics/translation.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/triggers.rst` & `trytond-7.2.1/doc/topics/triggers.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/user_application.rst` & `trytond-7.2.1/doc/topics/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/user_errors_warnings.rst` & `trytond-7.2.1/doc/topics/user_errors_warnings.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/views/extension.rst` & `trytond-7.2.1/doc/topics/views/extension.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/views/index.rst` & `trytond-7.2.1/doc/topics/views/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/topics/wizard.rst` & `trytond-7.2.1/doc/topics/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/anatomy.rst` & `trytond-7.2.1/doc/tutorial/module/anatomy.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/default_values.rst` & `trytond-7.2.1/doc/tutorial/module/default_values.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/domains.rst` & `trytond-7.2.1/doc/tutorial/module/domains.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/extend.rst` & `trytond-7.2.1/doc/tutorial/module/extend.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/function_fields.rst` & `trytond-7.2.1/doc/tutorial/module/function_fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/index.rst` & `trytond-7.2.1/doc/tutorial/module/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/model.rst` & `trytond-7.2.1/doc/tutorial/module/model.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/on_change.rst` & `trytond-7.2.1/doc/tutorial/module/on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/report.rst` & `trytond-7.2.1/doc/tutorial/module/report.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/setup.rst` & `trytond-7.2.1/doc/tutorial/module/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/setup_database.rst` & `trytond-7.2.1/doc/tutorial/module/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/states.rst` & `trytond-7.2.1/doc/tutorial/module/states.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/table_query.rst` & `trytond-7.2.1/doc/tutorial/module/table_query.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/view.rst` & `trytond-7.2.1/doc/tutorial/module/view.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/wizard.rst` & `trytond-7.2.1/doc/tutorial/module/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/doc/tutorial/module/workflow.rst` & `trytond-7.2.1/doc/tutorial/module/workflow.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/setup.py` & `trytond-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/tox.ini` & `trytond-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/__init__.py` & `trytond-7.2.1/trytond/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from lxml import etree, objectify
 
 try:
     from requests import utils as requests_utils
 except ImportError:
     requests_utils = None
 
-__version__ = "7.2.0"
+__version__ = "7.2.1"
 
 os.environ.setdefault(
     'TRYTOND_APPNAME',
     os.path.basename(getattr(__main__, '__file__', 'trytond')))
 os.environ.setdefault('TRYTOND_TZ', os.environ.get('TZ', 'UTC'))
 os.environ['TZ'] = 'UTC'
 if hasattr(time, 'tzset'):
```

### Comparing `trytond-7.2.0/trytond/admin.py` & `trytond-7.2.1/trytond/admin.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/application.py` & `trytond-7.2.1/trytond/application.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/__init__.py` & `trytond-7.2.1/trytond/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/database.py` & `trytond-7.2.1/trytond/backend/database.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/postgresql/database.py` & `trytond-7.2.1/trytond/backend/postgresql/database.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/postgresql/init.sql` & `trytond-7.2.1/trytond/backend/postgresql/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/postgresql/table.py` & `trytond-7.2.1/trytond/backend/postgresql/table.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/sqlite/database.py` & `trytond-7.2.1/trytond/backend/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/sqlite/init.sql` & `trytond-7.2.1/trytond/backend/sqlite/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/sqlite/table.py` & `trytond-7.2.1/trytond/backend/sqlite/table.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/backend/table.py` & `trytond-7.2.1/trytond/backend/table.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/bus.py` & `trytond-7.2.1/trytond/bus.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/cache.py` & `trytond-7.2.1/trytond/cache.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/commandline.py` & `trytond-7.2.1/trytond/commandline.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/config.py` & `trytond-7.2.1/trytond/config.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/console.py` & `trytond-7.2.1/trytond/console.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/convert.py` & `trytond-7.2.1/trytond/convert.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/cron.py` & `trytond-7.2.1/trytond/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/exceptions.py` & `trytond-7.2.1/trytond/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/filestore.py` & `trytond-7.2.1/trytond/filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/i18n.py` & `trytond-7.2.1/trytond/i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/__init__.py` & `trytond-7.2.1/trytond/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/action.py` & `trytond-7.2.1/trytond/ir/action.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/action.xml` & `trytond-7.2.1/trytond/ir/action.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/attachment.py` & `trytond-7.2.1/trytond/ir/attachment.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/attachment.xml` & `trytond-7.2.1/trytond/ir/attachment.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/avatar.py` & `trytond-7.2.1/trytond/ir/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/calendar_.py` & `trytond-7.2.1/trytond/ir/calendar_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/calendar_.xml` & `trytond-7.2.1/trytond/ir/calendar_.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/configuration.py` & `trytond-7.2.1/trytond/ir/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/cron.py` & `trytond-7.2.1/trytond/ir/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/cron.xml` & `trytond-7.2.1/trytond/ir/cron.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/date.py` & `trytond-7.2.1/trytond/ir/date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/email.xml` & `trytond-7.2.1/trytond/ir/email.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/email_.py` & `trytond-7.2.1/trytond/ir/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/error.py` & `trytond-7.2.1/trytond/ir/error.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/error.xml` & `trytond-7.2.1/trytond/ir/error.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/exceptions.py` & `trytond-7.2.1/trytond/ir/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/export.py` & `trytond-7.2.1/trytond/ir/export.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/export.xml` & `trytond-7.2.1/trytond/ir/export.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/fonts/LICENSE` & `trytond-7.2.1/trytond/ir/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/fonts/karla.ttf` & `trytond-7.2.1/trytond/ir/fonts/karla.ttf`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ir.xml` & `trytond-7.2.1/trytond/ir/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/lang.py` & `trytond-7.2.1/trytond/ir/lang.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/lang.xml` & `trytond-7.2.1/trytond/ir/lang.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/locale/bg.po` & `trytond-7.2.1/trytond/ir/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Стойност на котекст"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Стойност на домейн"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
@@ -110,14 +115,19 @@
 msgid "Records"
 msgstr "ID на запис"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Критерии за търсене"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
@@ -202,19 +212,29 @@
 msgid "Keywords"
 msgstr "Ключови думи"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Модул"
 
 #, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
+#, fuzzy
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Име на прикачен файл"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -325,14 +345,19 @@
 msgstr "Ключови думи"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Модел"
 
 #, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
+#, fuzzy
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Име на прикачен файл"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -847,14 +872,19 @@
 msgid "Model Name"
 msgstr "Име на модел"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Модул"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Описание на модел"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Описание"
@@ -863,14 +893,19 @@
 msgid "Group"
 msgstr "Група"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Права за създаване"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Права за изтриване"
@@ -897,14 +932,19 @@
 msgid "Help"
 msgstr "Помощ"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Име на прикачен файл"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
@@ -972,18 +1012,28 @@
 msgid "Values on File System"
 msgstr ""
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Модул"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Без обновяване"
 
 #, fuzzy
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
@@ -1006,18 +1056,28 @@
 msgid "Help"
 msgstr "Помощ"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Модул"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Име"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Модел на връзка"
@@ -1030,19 +1090,34 @@
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Поле"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Поле"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Група"
 
 #, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Модел"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
+#, fuzzy
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Права за създаване"
 
 #, fuzzy
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
@@ -1238,14 +1313,19 @@
 msgid "Global"
 msgstr "Глобален"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Име"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Права за създаване"
@@ -1396,22 +1476,31 @@
 msgid "Model"
 msgstr "Модел"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Модул"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Име на поле"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID на ресурс"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Източник"
@@ -1508,14 +1597,19 @@
 msgid "Icon"
 msgstr "Икона"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Модул"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Име на прикачен файл"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Път към SVG файл"
@@ -1563,40 +1657,64 @@
 msgid "User"
 msgstr "Потребител"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Архитектура на изгледа"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Данни"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Домейн"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Разширение"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Наследено поле"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Наследено поле"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Наследен изглед"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Модул"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Модул"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Име на прикачен файл"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Важност"
@@ -1672,18 +1790,28 @@
 msgid "User"
 msgstr "Потребител"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Поле"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Поле"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Модел"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Потребител"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Ширина"
@@ -1802,15 +1930,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Модула в който този модел е зададен"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1838,15 +1966,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Модул в който този модел е зададен"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2706,14 +2834,22 @@
 msgstr "This record is part of the base configuration."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Името на модула трябва да е уникално!"
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -3223,14 +3359,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/ca.po` & `trytond-7.2.1/trytond/ir/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Context Domain"
 msgstr "Domini del context"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Model del context"
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Model del context"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Valor del domini"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Dominis"
@@ -102,14 +106,18 @@
 msgid "Records"
 msgstr "Registres"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Filtrat"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tipus"
@@ -186,18 +194,26 @@
 msgid "Keywords"
 msgstr "Accions de teclat"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Nom del registre"
@@ -294,14 +310,18 @@
 msgid "Keywords"
 msgstr "Accions de teclat"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Registres"
@@ -778,14 +798,18 @@
 msgid "Model Name"
 msgstr "Model"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Descripció model"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Descripció"
@@ -794,14 +818,18 @@
 msgid "Group"
 msgstr "Grup"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Permís per crear"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Permís per eliminar"
@@ -826,14 +854,18 @@
 msgid "Help"
 msgstr "Ajuda"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Reinicia"
@@ -894,18 +926,26 @@
 msgid "Values on File System"
 msgstr "Valors en sistema de fitxers"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "No actualitzat"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Sense sincronitzar"
@@ -926,18 +966,26 @@
 msgid "Help"
 msgstr "Ajuda"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Relació model"
@@ -950,18 +998,30 @@
 msgid "Description"
 msgstr "Descripció"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Camp"
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Camp"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grup"
 
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Model"
+
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Permís per crear"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Permís per eliminar"
@@ -1142,14 +1202,18 @@
 msgid "Global"
 msgstr "Global"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Permís per crear"
@@ -1298,22 +1362,30 @@
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Nom del camp"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Mòdul anul·lant"
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Mòdul de substitució"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "Identificador del recurs"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Original"
@@ -1406,14 +1478,18 @@
 msgid "Icon"
 msgstr "Icona"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Ruta SVG"
@@ -1458,38 +1534,58 @@
 msgid "User"
 msgstr "Usuari"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Arquitectura de la vista"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr "Bases"
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Dades"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domini"
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Extensions"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Camp fills"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Camp fills"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Vista heretada"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Mòdul"
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Mòdul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioritat"
@@ -1554,18 +1650,26 @@
 msgid "User"
 msgstr "Usuari"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Camp"
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Camp"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Usuari"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Amplada"
@@ -1678,15 +1782,15 @@
 msgid "RFC 4646 tag."
 msgstr "Etiqueta RFC 4646."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Codi del pare excepcional"
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Mòdul en què es defineix aquest model."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr "El text que s'utilitzarà per demanar confirmació al clicar el botó."
 
@@ -1714,15 +1818,15 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Si es marca, els permisos d'accés al model del camp també es comproven a la "
 "relació del camp."
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Mòdul en el qual es defineix aquest camp."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2518,14 +2622,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Aquest registre es part de la configuració inicial."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "El nom del botó ha de ser únic per model."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr "A la data/hora: %(datetime)s"
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr "Als grups: %(groups)s"
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No podeu crear registres a \"%(model)s\" perquè no compleixen almenys alguna d'aquestes regles:\n"
 "%(rules)s"
@@ -2656,32 +2768,30 @@
 msgid "Type"
 msgstr "Tipus"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Si"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
 "record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
-"El nombre de dígits del valor \"%(value)r\" del camp \"%(field)s\" del "
+"El nombre de dígits en el valor \"%(value)r\" del camp \"%(field)s\" del "
 "registre \"%(record)s\" de \"%(model)s\" excedeix el seu límit de "
 "\"%(digits)i\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
-"El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
-" no és correcte segons el seu domini."
+"El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s\" de"
+" \"%(model)s\" no és correcte segons el seu domini."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Editat el"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
@@ -2723,22 +2833,21 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (nom del model)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "\"%(field)s (cadena)"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s\" de"
-" \"%(model)s\" conté caràcters invàlids \"%(chars)s\"."
+" \"%(model)s\" conté alguns caràcters invàlids \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 "Els registres no s'han pogut eliminar perquè s'utilitzen en el camp "
@@ -2852,15 +2961,14 @@
 "La definició del nom de registre no és vàlida per a l'informe \"%(report)s\""
 " amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Es requereix un valor pel camp \"%(field)s\" de \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
 msgid ""
 "A value is required for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\"."
 msgstr ""
 "Es requereix un valor pel camp \"%(field)s\" del registre \"%(record)s\" de "
 "\"%(model)s\"."
@@ -2873,15 +2981,14 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "La regla del domini \"%(name)s\" es invàlida."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Falta la funció de cerca del camp \"%(field)s\" a \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s \"de"
 " \"%(model)s\" no és un dels seus valors permesos."
@@ -2904,15 +3011,15 @@
 "(%(number_next)s) with exception \"%(exception)s\"."
 msgstr ""
 "El \"Número d'increment\" (%(number_increment)s) o el \"Següent número\" "
 "(%(number_next)s) és invalid amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_prefix"
 msgid "Invalid prefix \"%(affix)s\" for sequence \"%(sequence)s\"."
-msgstr "El prefix \"%(prefix)s\" de la seqüència \"%(sequence)s\" es invàlid."
+msgstr "El prefix \"%(affix)s\" de la seqüència \"%(sequence)s\" es invàlid."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_suffix"
 msgid "Invalid suffix \"%(affix)s\" for sequence \"%(sequence)s\"."
 msgstr "El sufix \"%(affix)s\" de la seqüència \"%(sequence)s\" es invàlid."
 
 msgctxt "model:ir.message,text:msg_sequence_last_timestamp_future"
 msgid "The \"Last Timestamp\" cannot be in the future for sequence \"%s\"."
@@ -2931,27 +3038,25 @@
 msgstr "Només es pot crear un singleton."
 
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
-"El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
-" es massa llarg (%(size)i > %(max_size)i)."
+"El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s\" de"
+" \"%(model)s\" es massa llarg (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
-" es massa llarg (%(size)i > %(max_size)i)."
+"El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s\" de"
+" \"%(model)s\" es massa llarg (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
 "The time value \"%(value)s\" for field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "El valor de temps \"%(value)s\" del camp %(field)s\" del registre "
 "\"%(record)s\" de \"%(model)s\" no és vàlid."
@@ -2989,15 +3094,15 @@
 msgstr "S'han trobat massa relacions: \"%(value)r\" en \"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_translation_overridden"
 msgid ""
 "You can not export translation \"%(name)s\" because it has been overridden "
 "by module \"%(overriding_module)s\"."
 msgstr ""
-"No podeu exportar la traducció \"%(name)\"s perquè s'ha sobreescrit en el "
+"No podeu exportar la traducció \"%(name)s\" perquè s'ha sobreescrit en el "
 "mòdul \"%(overriding_module)s\"."
 
 msgctxt "model:ir.message,text:msg_trigger_exclusive"
 msgid ""
 "You can not select \"On Time\" and any other on the same time, they are "
 "mutually exclusive."
 msgstr "No es pot activar \"Al moment\" i altres perquè són mútuament exclusius."
@@ -3044,23 +3149,26 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No podeu modificar els registres \"%(ids)s\" de \"%(model)s\" per almenys una d'aquestes regles:\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "No podeu modificar el camp \"%(field)s\" del registre \"%(record)s\" de "
 "\"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr "ID XML"
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Error de sintaxis per l'ID de XML: %(value)r\" en \"%(field)s\" de "
 "\"%(model)s\" (%(column)s)."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/cs.po` & `trytond-7.2.1/trytond/ir/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 msgid "Icon"
 msgstr "Icons"
 
 msgctxt "field:ir.action,keywords:"
 msgid "Keywords"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.action,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action,type:"
@@ -56,14 +55,18 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr ""
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr ""
@@ -77,18 +80,17 @@
 msgid "Keywords"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,limit:"
 msgid "Limit"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.action.act_window,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.action.act_window,order:"
 msgid "Order Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,pyson_context:"
 msgid "PySON Context"
@@ -112,14 +114,19 @@
 msgstr "Record Rules"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr ""
@@ -142,18 +149,17 @@
 msgid "Count"
 msgstr ""
 
 msgctxt "field:ir.action.act_window.domain,domain:"
 msgid "Domain"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.action.act_window.domain,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actions"
 
 #, fuzzy
@@ -208,22 +214,31 @@
 
 #, fuzzy
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Record Rules"
 
 #, fuzzy
@@ -285,18 +300,17 @@
 msgid "Icon"
 msgstr "Icons"
 
 msgctxt "field:ir.action.url,keywords:"
 msgid "Keywords"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.action.url,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.url,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action.url,type:"
@@ -327,17 +341,21 @@
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action.wizard,type:"
@@ -389,18 +407,17 @@
 msgid "Last User"
 msgstr ""
 
 msgctxt "field:ir.attachment,link:"
 msgid "Link"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.attachment,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.attachment,resource:"
 msgid "Resource"
 msgstr ""
 
 msgctxt "field:ir.attachment,summary:"
 msgid "Summary"
@@ -458,48 +475,45 @@
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:ir.avatar.cache,size:"
 msgid "Size"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.cache,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.cache,timestamp:"
 msgid "Timestamp"
 msgstr ""
 
 msgctxt "field:ir.calendar.day,abbreviation:"
 msgid "Abbreviation"
 msgstr ""
 
 msgctxt "field:ir.calendar.day,index:"
 msgid "Index"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.calendar.day,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.calendar.month,abbreviation:"
 msgid "Abbreviation"
 msgstr ""
 
 msgctxt "field:ir.calendar.month,index:"
 msgid "Index"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.calendar.month,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.configuration,hostname:"
 msgid "Hostname"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.configuration,language:"
@@ -596,18 +610,17 @@
 msgstr "Models"
 
 #, fuzzy
 msgctxt "field:ir.email.template,model_name:"
 msgid "Model Name"
 msgstr "Models Access"
 
-#, fuzzy
 msgctxt "field:ir.email.template,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.email.template,recipients:"
 msgid "Recipients"
 msgstr ""
 
 msgctxt "field:ir.email.template,recipients_hidden:"
 msgid "Hidden Recipients"
@@ -681,18 +694,17 @@
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "field:ir.export,header:"
 msgid "Header"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.export,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.export,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.export,resource:"
@@ -704,18 +716,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.export.line,export:"
 msgid "Export"
 msgstr "Exports"
 
-#, fuzzy
 msgctxt "field:ir.export.line,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.lang,am:"
 msgid "AM"
 msgstr ""
 
 msgctxt "field:ir.lang,code:"
 msgid "Code"
@@ -758,18 +769,17 @@
 msgid "Negative Separate by Space"
 msgstr ""
 
 msgctxt "field:ir.lang,n_sign_posn:"
 msgid "Negative Sign Position"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.lang,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.lang,negative_sign:"
 msgid "Negative Sign"
 msgstr ""
 
 msgctxt "field:ir.lang,p_cs_precedes:"
 msgid "Positive Currency Symbol Precedes"
@@ -834,14 +844,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr ""
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr ""
@@ -851,14 +866,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -886,17 +906,21 @@
 
 #, fuzzy
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
 
 msgctxt "field:ir.model.button,reset_by:"
 msgid "Reset by"
@@ -959,18 +983,28 @@
 
 #, fuzzy
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
@@ -995,22 +1029,31 @@
 
 #, fuzzy
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr ""
 
 msgctxt "field:ir.model.field,ttype:"
 msgid "Field Type"
@@ -1021,18 +1064,33 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Fields"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Fields"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -1078,18 +1136,17 @@
 msgid "Childs"
 msgstr ""
 
 msgctxt "field:ir.module,dependencies:"
 msgid "Dependencies"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.module,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.module,parents:"
 msgid "Parents"
 msgstr ""
 
 msgctxt "field:ir.module,state:"
 msgid "State"
@@ -1122,18 +1179,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.module.dependency,module:"
 msgid "Module"
 msgstr "Modules"
 
-#, fuzzy
 msgctxt "field:ir.module.dependency,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.module.dependency,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:ir.note,copy_to_resources:"
 msgid "Copy to Resources"
@@ -1193,18 +1249,17 @@
 msgid "Expected at"
 msgstr ""
 
 msgctxt "field:ir.queue,finished_at:"
 msgid "Finished at"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.queue,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.queue,scheduled_at:"
 msgid "Scheduled at"
 msgstr ""
 
 msgctxt "field:ir.rule,domain:"
 msgid "Domain"
@@ -1224,17 +1279,21 @@
 
 #, fuzzy
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.rule.group,perm_delete:"
 msgid "Delete Access"
@@ -1389,22 +1448,31 @@
 msgstr "Models"
 
 #, fuzzy
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr ""
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr ""
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr ""
@@ -1468,18 +1536,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.trigger,model:"
 msgid "Model"
 msgstr "Models"
 
-#, fuzzy
 msgctxt "field:ir.trigger,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.trigger,on_create:"
 msgid "On Create"
 msgstr ""
 
 msgctxt "field:ir.trigger,on_delete:"
 msgid "On Delete"
@@ -1509,17 +1576,21 @@
 
 #, fuzzy
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.menu,action:"
@@ -1565,45 +1636,67 @@
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr ""
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Export Translations"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr ""
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr ""
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr ""
 
 msgctxt "field:ir.ui.view,type:"
 msgid "View Type"
@@ -1614,18 +1707,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view_search,model:"
 msgid "Model"
 msgstr "Models"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_search,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:ir.ui.view_search,user:"
 msgid "User"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,field:"
@@ -1672,18 +1764,28 @@
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Fields"
 
 #, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Fields"
+
+#, fuzzy
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr ""
@@ -1786,15 +1888,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1818,15 +1920,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2614,14 +2716,22 @@
 msgid "This record is part of the base configuration."
 msgstr "This record is part of the base configuration."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_created_at"
@@ -2713,18 +2823,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_multiselection"
 msgid "MultiSelection"
 msgstr "Scheduled Actions"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_name"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_dict_schema_numeric"
 msgid "Numeric"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_selection"
@@ -3118,14 +3227,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 #, fuzzy
```

### Comparing `trytond-7.2.0/trytond/ir/locale/de.po` & `trytond-7.2.1/trytond/ir/locale/de.po`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Context Domain"
 msgstr "Kontext des Wertebereichs"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Kontextmodell"
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Kontextmodell"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Wertebereich (Domain)"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Wertebereiche (Domains)"
@@ -102,14 +106,18 @@
 msgid "Records"
 msgstr "Datensätze"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Suchkriterien"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Typ"
@@ -186,18 +194,26 @@
 msgid "Keywords"
 msgstr "Schlüsselwörter"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Bezeichnung des Datensatzes"
@@ -294,14 +310,18 @@
 msgid "Keywords"
 msgstr "Schlüsselwörter"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Datensätze"
@@ -778,14 +798,18 @@
 msgid "Model Name"
 msgstr "Modellname"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Modell Beschreibung"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Beschreibung"
@@ -794,14 +818,18 @@
 msgid "Group"
 msgstr "Gruppe"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Erstellen"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Löschen"
@@ -826,14 +854,18 @@
 msgid "Help"
 msgstr "Hilfe"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Zurücksetzen"
@@ -894,18 +926,26 @@
 msgid "Values on File System"
 msgstr "Werte im Dateisystem"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Kein Update"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Nicht synchronisiert"
@@ -926,18 +966,26 @@
 msgid "Help"
 msgstr "Hilfe"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Beziehung Modell"
@@ -950,18 +998,30 @@
 msgid "Description"
 msgstr "Beschreibung"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Feld"
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Feld"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Gruppe"
 
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Modell"
+
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Erstellen"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Löschen"
@@ -1142,14 +1202,18 @@
 msgid "Global"
 msgstr "Global"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Erstellen"
@@ -1298,22 +1362,30 @@
 msgid "Model"
 msgstr "Modell"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Feldname"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Überschreibendes Modul"
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Überschreibendes Modul"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID Ressource"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Quelle"
@@ -1407,14 +1479,18 @@
 msgid "Icon"
 msgstr "Icon"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Pfad"
@@ -1459,38 +1535,58 @@
 msgid "User"
 msgstr "Benutzer"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Architektur Sicht"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr "Basis"
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Daten"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Wertebereich (Domain)"
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Erweiterungen"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Untergeordnetes Feld"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Untergeordnetes Feld"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Vererbte Sicht"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modul"
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Priorität"
@@ -1555,18 +1651,26 @@
 msgid "User"
 msgstr "Benutzer"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Feld"
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Feld"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Modell"
 
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Benutzer"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Breite"
@@ -1680,15 +1784,15 @@
 msgid "RFC 4646 tag."
 msgstr "RFC 4646 Tag."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Code des außerordentlichen Elternsatzes"
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Modul, in dem dieses Modell definiert ist."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "Der Text der zur Benutzerbestätigung beim Button-Klick erscheinen soll."
@@ -1717,15 +1821,15 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Bei Aktivierung werden die Berechtigungen für das Modell des Feldes auch "
 "gegen die Relation des Feldes geprüft."
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Modul, in dem dieses Feld definiert ist."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2529,14 +2633,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Dieser Datensatz ist Teil der Basiskonfiguration."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Der Name des Buttons muss pro Modell eindeutig sein."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr "Zum Zeitpunkt: %(datetime)s"
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr "In den Gruppen: %(groups)s"
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Sie sind nicht berechtigt Datensätze vom Typ \"%(model)s\" zu erstellen, da sie gegen mindestens eine der folgenden Regeln verstoßen:\n"
 "%(rules)s"
@@ -2669,31 +2781,30 @@
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Ja"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
 "record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
-"Die Anzahl der Nachkommastellen im Wert \"%(value)s\" für Feld \"%(field)s\""
-" von \"%(model)s\" überschreitet das Limit von \"%(digits)i\"."
+"Die Anzahl der Nachkommastellen im Wert \"%(value)s\" des Feldes "
+"\"%(field)s\" im Datensatz \"%(record)s\" von \"%(model)s\" überschreitet "
+"das Limit von \"%(digits)i\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
-"Der Wert \"%(value)s\" des Feldes \"%(field)s\" in \"%(record)s\" von "
-"\"%(model)s\" liegt nicht im gültigen Wertebereich (Domain)."
+"Der Wert \"%(value)s\" des Feldes \"%(field)s\" im Datensatz \"%(record)s\" "
+"von \"%(model)s\" liegt nicht im gültigen Wertebereich (Domain)."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Bearbeitet um"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
@@ -2735,22 +2846,21 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (Modellname)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (Zeichenkette)"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
-"Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(record)s\" von "
-"\"%(model)s\" enthält die ungültigen Zeichen \"%(chars)s\"."
+"Der Wert \"%(value)s\" des Feldes \"%(field)s\" im Datensatz \"%(record)s\" "
+"von \"%(model)s\" enthält die ungültigen Zeichen \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 "Die Datensätze konnten nicht gelöscht werden, weil sie im Feld \"%(field)s\""
@@ -2864,43 +2974,41 @@
 "Ungültige Definition für den Berichtsnamen von Bericht \"%(report)s\" mit "
 "Fehler \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Für das Feld \"%(field)s\" von \"%(model)s\" ist ein Wert erforderlich."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
 msgid ""
 "A value is required for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\"."
 msgstr ""
-"Für das Feld \"%(field)s\" in \"%(record)s\" von \"%(model)s\" ist ein Wert "
-"erforderlich."
+"Für das Feld \"%(field)s\" im Datensatz \"%(record)s\" von \"%(model)s\" ist"
+" ein Wert erforderlich."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Die Ressourcen zu denen dieser Datensatz kopiert werden muss."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "Ungültiger Wertebereich (Domain) in Regel \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Fehlende Suchfunktion für Feld \"%(field)s\" in \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
-"Der Wert \"%(value)s\" von Feld \"%(field)s\" in \"%(record)s\" von "
-"\"%(model)s\" ist nicht in der Auswahl enthalten."
+"Der Wert \"%(value)s\" des Feldes \"%(field)s\" im Datensatz \"%(record)s\" "
+"von \"%(model)s\" ist nicht in der Auswahl enthalten."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Reihenfolge"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
@@ -2948,31 +3056,29 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(model)s\" ist zu lang "
 "(%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(record)s\" von "
-"\"%(model)s\" ist zu lang (%(size)i > %(max_size)i)."
+"Der Wert \"%(value)s\" des Feldes \"%(field)s\" im Datensatz \"%(record)s\" "
+"von \"%(model)s\" ist zu lang (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
 "The time value \"%(value)s\" for field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
-"Der Wert der Zeit \"%(value)s\" für Feld \"%(field)s\" in \"%(record)s\" von"
-" \"%(model)s\" ist ungültig."
+"Der Wert der Zeitangabe \"%(value)s\" des Feldes \"%(field)s\" im Datensatz "
+"\"%(record)s\" von \"%(model)s\" ist ungültig."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "m"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
 msgid "Y"
@@ -3061,22 +3167,25 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Sie sind aufgrund mindestens einer der folgenden Regeln nicht dazu berechtigt, die Datensätze \"%(ids)s\" vom Typ \"%(model)s\" zu verändern:\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
-"Keine Berechtigung zur Änderung des Feldes \"%(field)s\" in \"%(record)s\" "
-"von \"%(model)s\"."
+"Keine Berechtigung zur Änderung des Feldes \"%(field)s\" im Datensatz "
+"\"%(record)s\" von \"%(model)s\"."
+
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr "XML-ID"
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Syntaxfehler für XML-ID: %(value)r in \"%(field)s\" von \"%(model)s\" "
```

### Comparing `trytond-7.2.0/trytond/ir/locale/es.po` & `trytond-7.2.1/trytond/ir/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Context Domain"
 msgstr "Dominio del contexto"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Modelo del contexto"
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Modelo de contexto"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Valor del dominio"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Dominios"
@@ -102,14 +106,18 @@
 msgid "Records"
 msgstr "Registros"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Criterio de búsqueda"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tipo"
@@ -186,18 +194,26 @@
 msgid "Keywords"
 msgstr "Acciones de teclado"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Nombre del registro"
@@ -294,14 +310,18 @@
 msgid "Keywords"
 msgstr "Acciones de teclado"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Registros"
@@ -778,14 +798,18 @@
 msgid "Model Name"
 msgstr "Modelo"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Descripción modelo"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Descripción"
@@ -794,14 +818,18 @@
 msgid "Group"
 msgstr "Grupo"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Permiso para crear"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Permiso para eliminar"
@@ -826,14 +854,18 @@
 msgid "Help"
 msgstr "Ayuda"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Reiniciar"
@@ -894,18 +926,26 @@
 msgid "Values on File System"
 msgstr "Valores en sistema de ficheros"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "No actualizar"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Sin sincronizar"
@@ -926,18 +966,26 @@
 msgid "Help"
 msgstr "Ayuda"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Relación del modelo"
@@ -950,18 +998,30 @@
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Campo"
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Campo"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grupo"
 
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Modelo"
+
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Permiso para crear"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Permiso para eliminar"
@@ -1142,14 +1202,18 @@
 msgid "Global"
 msgstr "Global"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Permiso para crear"
@@ -1298,22 +1362,30 @@
 msgid "Model"
 msgstr "Modelo"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Nombre del campo"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Módulo principal"
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Módulo sobrescrito"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID del recurso"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Original"
@@ -1406,14 +1478,18 @@
 msgid "Icon"
 msgstr "Icono"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Ruta SVG"
@@ -1458,38 +1534,58 @@
 msgid "User"
 msgstr "Usuario"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Arquitectura de la vista"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr "Bases"
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Datos"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Dominio"
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Extensiones"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Campo hijos"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Campo hijos"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Vista heredada"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Módulo"
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioridad"
@@ -1554,18 +1650,26 @@
 msgid "User"
 msgstr "Usuario"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Campo"
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Campo"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Modelo"
 
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Usuario"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Ancho"
@@ -1678,15 +1782,15 @@
 msgid "RFC 4646 tag."
 msgstr "Etiqueta RFC 4646."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Código del padre excepcional"
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Módulo donde se define este modelo."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "El texto que se va a utilizar para pedir confirmación al ciclar el botón."
@@ -1715,15 +1819,15 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Si se marca, los permisos de acceso al modelo del campo también se "
 "comprueban en la relación del campo."
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Módulo donde se define este campo."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2523,14 +2627,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Este registro es parte de la configuración inicial."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "El nombre del botón debe ser único por cada modelo."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr "A la fecha/hora: %(datetime)s"
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr "En los grupos: %(groups)s"
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No puede crear registros de \"%(model)s\" porque incumplen alguna de estas reglas:\n"
 "%(rules)s"
@@ -2662,25 +2774,23 @@
 msgid "Type"
 msgstr "Tipo"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Sí"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
 "record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "El número de dígitos en el valor \"%(value)r\" del campo \"%(field)s\" en el"
 " registro \"%(record)s\" de \"%(model)s\" excede el límite de "
 "\"%(digits)i\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(record)s\" "
 "de \"%(model)s\" no es correcto según su dominio."
@@ -2729,23 +2839,21 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (nombre del modelo)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (cadena)"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
-"El valor \"%(value)s\" para el campo \"%(field)s\" del registro "
-"\"%(record)s\" en \"%(model)s\" contiene algunos caracteres inválidos "
-"\"%(chars)s\"."
+"El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(record)s\" "
+"en \"%(model)s\" contiene algunos caracteres inválidos \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 "Los registros no pueden eliminarse porque se utilizan en el campo "
@@ -2860,15 +2968,14 @@
 "La definición del nombre de registro no és válida en el informe "
 "\"%(report)s\" con la excepción \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Se requiere un valor para el campo \"%(field)s\" de \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
 msgid ""
 "A value is required for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\"."
 msgstr ""
 "Se requiere un valor para el campo \"%(field)s\" en el registro "
 "\"%(record)s\" de \"%(model)s\"."
@@ -2881,22 +2988,21 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "El dominio de la regla \"%(name)s\" no es valido."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Falta la función de búsqueda del campo \"%(field)s\" a \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(record)s\" "
-"en \"%(model)s\" no es uno de sus valores permitidos."
+"en \"%(model)s\" no es una de sus opciones permitidas."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Secuencia"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
@@ -2912,15 +3018,15 @@
 "(%(number_next)s) with exception \"%(exception)s\"."
 msgstr ""
 "El \"Número de incremento\" (%(number_increment)s) o el \"Siguiente Numero\""
 " (%(number_next)s) son inválidos con la excepción \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_prefix"
 msgid "Invalid prefix \"%(affix)s\" for sequence \"%(sequence)s\"."
-msgstr "El prefijo \"%(prefix)s\" de la secuencia \"%(sequence)s\" es inválido."
+msgstr "El prefijo \"%(affix)s\" de la secuencia \"%(sequence)s\" es inválido."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_suffix"
 msgid "Invalid suffix \"%(affix)s\" for sequence \"%(sequence)s\"."
 msgstr "El sufijo \"%(affix)s\" de la secuencia \"%(sequence)s\" es invlido."
 
 msgctxt "model:ir.message,text:msg_sequence_last_timestamp_future"
 msgid "The \"Last Timestamp\" cannot be in the future for sequence \"%s\"."
@@ -2939,27 +3045,25 @@
 msgstr "Solo se puede crear un singleton."
 
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
-"El valor del campo \"%(field)s\" del registro \"%(model)s\" en \"%(model)s\""
-" es demasiado largo (%(size)i > %(max_size)i)."
+"El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(model)s\" en"
+" \"%(model)s\" es demasiado largo (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"El valor del campo \"%(field)s\" del registro \"%(record)s\" en "
-"\"%(model)s\" es demasiado largo (%(size)i > %(max_size)i)."
+"El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(record)s\" "
+"en \"%(model)s\" es demasiado largo (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
 "The time value \"%(value)s\" for field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "El valor del tiempo \"%(value)s\" del campo \"%(field)s\" del registro "
 "\"%(record)s\" de \"%(model)s) no es valido."
@@ -3055,23 +3159,26 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No puede modificar los registros \"%(ids)s\" de \"%(model)s\" debido a alguna de estas reglas:\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "No podéis modificar el campo \"%(field)s\" del registro \"%(record)s\" de "
 "\"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr "ID XML"
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Error de sintaxis para el id de XML: %(value)r\" en \"%(field)s\" de "
 "\"%(model)s\" (%(column)s)."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/es_419.po` & `trytond-7.2.1/trytond/ir/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr ""
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr ""
@@ -104,14 +108,19 @@
 msgid "Records"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr ""
@@ -191,18 +200,27 @@
 msgid "Keywords"
 msgstr ""
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -300,14 +318,19 @@
 msgid "Keywords"
 msgstr ""
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr ""
@@ -791,14 +814,18 @@
 msgid "Model Name"
 msgstr ""
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr ""
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr ""
@@ -807,14 +834,19 @@
 msgid "Group"
 msgstr ""
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -839,14 +871,19 @@
 msgid "Help"
 msgstr ""
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
@@ -907,18 +944,27 @@
 msgid "Values on File System"
 msgstr ""
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr ""
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr ""
@@ -940,18 +986,27 @@
 msgid "Help"
 msgstr ""
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr ""
@@ -965,18 +1020,33 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Fields"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Fields"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -1159,14 +1229,19 @@
 msgid "Global"
 msgstr ""
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr ""
@@ -1315,22 +1390,30 @@
 msgid "Model"
 msgstr ""
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr ""
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr ""
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr ""
@@ -1423,14 +1506,18 @@
 msgid "Icon"
 msgstr ""
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr ""
@@ -1475,38 +1562,59 @@
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr ""
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr ""
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr ""
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr ""
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr ""
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr ""
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr ""
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr ""
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr ""
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr ""
@@ -1575,18 +1683,28 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Fields"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Fields"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr ""
@@ -1689,15 +1807,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1721,15 +1839,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2512,14 +2630,22 @@
 msgid "This record is part of the base configuration."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -2977,14 +3103,18 @@
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/et.po` & `trytond-7.2.1/trytond/ir/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 msgid "Context Domain"
 msgstr "Konteksti domeen"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Konteksti mudel"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Konteksti mudel"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Domeeni väärtus"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domeenid"
@@ -104,14 +109,19 @@
 msgid "Records"
 msgstr "Kirje ID"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Otsingukriteerium"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tüüp"
@@ -189,18 +199,28 @@
 msgid "Keywords"
 msgstr "Märksõnad"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nimi"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -300,14 +320,19 @@
 msgid "Keywords"
 msgstr "Märksõnad"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nimi"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -811,14 +836,19 @@
 msgid "Model Name"
 msgstr "Mudeli nimi"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Mudeli kirjeldus"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Kirjeldus"
@@ -827,14 +857,19 @@
 msgid "Group"
 msgstr "Grupp"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Loomisõigus"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Kustutamisõigus"
@@ -859,14 +894,19 @@
 msgid "Help"
 msgstr "Abi"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Reset"
@@ -927,18 +967,28 @@
 msgid "Values on File System"
 msgstr "Failisüsteemi väärtused"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Ei ole uuendatud"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Sünkroonist väljas"
@@ -960,18 +1010,28 @@
 msgid "Help"
 msgstr "Abi"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Mudeli seos"
@@ -984,18 +1044,33 @@
 msgid "Description"
 msgstr "Kirjeldus"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Väli"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Väli"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grupp"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Mudel"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Loomisõigus"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Kustutamisõigus"
@@ -1181,14 +1256,19 @@
 msgid "Global"
 msgstr "Globaalne"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Loomisõigus"
@@ -1339,22 +1419,32 @@
 msgid "Model"
 msgstr "Mudel"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Välja nimi"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Kirjuta moodul üle"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Kirjuta moodul üle"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "Ressursi ID"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Allikas"
@@ -1451,14 +1541,19 @@
 msgid "Icon"
 msgstr "Ikoon"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "SVG asukoht"
@@ -1503,38 +1598,62 @@
 msgid "User"
 msgstr "Kasutaja"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Vaata arhitektuuri"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Andmed"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domeen"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Laiendus"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Alamväli"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Alamväli"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Päritud vaade"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Moodul"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Moodul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioriteet"
@@ -1603,18 +1722,28 @@
 msgid "User"
 msgstr "Kasutaja"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Väli"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Väli"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Mudel"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Kasutaja"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Laius"
@@ -1721,15 +1850,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Moodul, milles mudel on defineeritud"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr "Kasutaja kinnitus, kui vajutatakse nupule."
 
@@ -1755,15 +1884,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Moodul, milles väli on defineeritud"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2560,14 +2689,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Kirje on algseadistuste osa"
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -3086,14 +3223,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "Mudeli \"%(model)s\" välja \"%(field)s\" jaoks on väärtus nõutud."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "XML süntaksi viga: \"%(value)r\" in \"%(field)s\"."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/fa.po` & `trytond-7.2.1/trytond/ir/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 msgid "Context Domain"
 msgstr "دامنه مفاد"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "مدل مفاد"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "مدل مفاد"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "ارزش دامنه"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "دامنه ها"
@@ -105,14 +110,19 @@
 msgid "Records"
 msgstr "شناسه رکورد"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "معیارهای جستجوی"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "نوع"
@@ -190,18 +200,28 @@
 msgid "Keywords"
 msgstr "کلیدواژه‌ها"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "نام"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -301,14 +321,19 @@
 msgid "Keywords"
 msgstr "کلیدواژه‌ها"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "نام"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -816,14 +841,19 @@
 msgid "Model Name"
 msgstr "نام مدل"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "شرح مدل"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "شرح"
@@ -832,14 +862,19 @@
 msgid "Group"
 msgstr "گروه"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "دسترسی ایجاد کردن"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "دسترسی حذف کردن"
@@ -864,14 +899,19 @@
 msgid "Help"
 msgstr "کمک"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "تنظیم مجدد"
@@ -932,18 +972,28 @@
 msgid "Values on File System"
 msgstr "مقادیر در سیستم فایل"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "بدون بروزرسانی"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "خارج از همگام سازی"
@@ -965,18 +1015,28 @@
 msgid "Help"
 msgstr "کمک"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "رابطه مدل"
@@ -989,18 +1049,33 @@
 msgid "Description"
 msgstr "شرح"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "فیلد"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "فیلد"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "گروه"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "مدل"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "دسترسی ایجاد کردن"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "دسترسی حذف کردن"
@@ -1186,14 +1261,19 @@
 msgid "Global"
 msgstr "سراسری"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "دسترسی ایجاد کردن"
@@ -1344,22 +1424,32 @@
 msgid "Model"
 msgstr "مدل"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "نام فیلد"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "بازنویسی کردن ماژول"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "بازنویسی کردن ماژول"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "شناسه مرجع"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "منبع"
@@ -1456,14 +1546,19 @@
 msgid "Icon"
 msgstr "آیکون"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "مسیر SVG"
@@ -1508,38 +1603,62 @@
 msgid "User"
 msgstr "کاربر"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "نمای معماری"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "داده"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "دامنه"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "توسعه"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "فیلد زیرمجموعه"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "فیلد زیرمجموعه"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "نمای ارث بری"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "ماژول"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "ماژول"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "اولویت"
@@ -1608,18 +1727,28 @@
 msgid "User"
 msgstr "کاربر"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "فیلد"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "فیلد"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "مدل"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "کاربر"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "عرض"
@@ -1739,15 +1868,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "کد منبع استثنایی"
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "ماژولی که این مدل در آن تعریف شده است"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr "متن برای دریافت تایید کاربر هنگام کلیک کردن بر روی دکمه."
 
@@ -1775,15 +1904,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "ماژولی که این فیلد در آن تعریف شده است"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2596,14 +2725,22 @@
 msgstr "این پرونده بخشی از پیکره بندی پایه میباشد."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "نام مدل باید منحصر به فرد باشد!"
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -3122,14 +3259,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "یک مقدار برای فیلد :\"%(field)s\" در\"%(model)s\" مورد نیاز است."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "خطای نحوی برای شناسه xml :\"%(value)r\" در \"%(field)s\"."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/fi.po` & `trytond-7.2.1/trytond/ir/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 msgctxt "field:ir.action,keywords:"
 msgid "Keywords"
 msgstr ""
 
 msgctxt "field:ir.action,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:ir.action,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action,type:"
@@ -55,14 +55,18 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr ""
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr ""
@@ -78,15 +82,15 @@
 
 msgctxt "field:ir.action.act_window,limit:"
 msgid "Limit"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.action.act_window,order:"
 msgid "Order Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,pyson_context:"
 msgid "PySON Context"
@@ -110,14 +114,19 @@
 msgstr "Record Rules"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr ""
@@ -142,15 +151,15 @@
 
 msgctxt "field:ir.action.act_window.domain,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window.domain,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actions"
 
 #, fuzzy
@@ -205,21 +214,31 @@
 
 #, fuzzy
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Record Rules"
 
 #, fuzzy
@@ -283,15 +302,15 @@
 
 msgctxt "field:ir.action.url,keywords:"
 msgid "Keywords"
 msgstr ""
 
 msgctxt "field:ir.action.url,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:ir.action.url,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action.url,type:"
@@ -321,17 +340,22 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action.wizard,type:"
@@ -365,15 +389,15 @@
 
 msgctxt "field:ir.attachment,data_size:"
 msgid "Data size"
 msgstr ""
 
 msgctxt "field:ir.attachment,description:"
 msgid "Description"
-msgstr ""
+msgstr "Tanım"
 
 msgctxt "field:ir.attachment,file_id:"
 msgid "File ID"
 msgstr ""
 
 msgctxt "field:ir.attachment,last_modification:"
 msgid "Last Modification"
@@ -385,15 +409,15 @@
 
 msgctxt "field:ir.attachment,link:"
 msgid "Link"
 msgstr ""
 
 msgctxt "field:ir.attachment,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.attachment,resource:"
 msgid "Resource"
 msgstr ""
 
 msgctxt "field:ir.attachment,summary:"
 msgid "Summary"
@@ -453,43 +477,45 @@
 
 msgctxt "field:ir.avatar.cache,size:"
 msgid "Size"
 msgstr ""
 
 msgctxt "field:ir.cache,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.cache,timestamp:"
 msgid "Timestamp"
 msgstr ""
 
 msgctxt "field:ir.calendar.day,abbreviation:"
 msgid "Abbreviation"
 msgstr ""
 
 msgctxt "field:ir.calendar.day,index:"
 msgid "Index"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.calendar.day,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.calendar.month,abbreviation:"
 msgid "Abbreviation"
 msgstr ""
 
 msgctxt "field:ir.calendar.month,index:"
 msgid "Index"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.calendar.month,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.configuration,hostname:"
 msgid "Hostname"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.configuration,language:"
@@ -586,17 +612,18 @@
 msgstr "Models"
 
 #, fuzzy
 msgctxt "field:ir.email.template,model_name:"
 msgid "Model Name"
 msgstr "Models Access"
 
+#, fuzzy
 msgctxt "field:ir.email.template,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.email.template,recipients:"
 msgid "Recipients"
 msgstr ""
 
 msgctxt "field:ir.email.template,recipients_hidden:"
 msgid "Hidden Recipients"
@@ -632,17 +659,18 @@
 msgid "Report"
 msgstr "Reports"
 
 msgctxt "field:ir.email.template-ir.action.report,template:"
 msgid "Template"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.error,description:"
 msgid "Description"
-msgstr ""
+msgstr "Tanım"
 
 msgctxt "field:ir.error,message:"
 msgid "Message"
 msgstr ""
 
 msgctxt "field:ir.error,origin:"
 msgid "Origin"
@@ -661,26 +689,25 @@
 msgid "State"
 msgstr "Tree State"
 
 msgctxt "field:ir.error,summary:"
 msgid "Summary"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.export,export_fields:"
 msgid "Fields"
-msgstr "Fields"
+msgstr "Alanlar"
 
 msgctxt "field:ir.export,header:"
 msgid "Header"
 msgstr ""
 
 msgctxt "field:ir.export,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:ir.export,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.export,resource:"
@@ -694,15 +721,15 @@
 #, fuzzy
 msgctxt "field:ir.export.line,export:"
 msgid "Export"
 msgstr "Exports"
 
 msgctxt "field:ir.export.line,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.lang,am:"
 msgid "AM"
 msgstr ""
 
 msgctxt "field:ir.lang,code:"
 msgid "Code"
@@ -747,15 +774,15 @@
 
 msgctxt "field:ir.lang,n_sign_posn:"
 msgid "Negative Sign Position"
 msgstr ""
 
 msgctxt "field:ir.lang,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.lang,negative_sign:"
 msgid "Negative Sign"
 msgstr ""
 
 msgctxt "field:ir.lang,p_cs_precedes:"
 msgid "Positive Currency Symbol Precedes"
@@ -798,18 +825,17 @@
 msgid "Languages"
 msgstr "Languages"
 
 msgctxt "field:ir.message,text:"
 msgid "Text"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.model,fields:"
 msgid "Fields"
-msgstr "Fields"
+msgstr "Alanlar"
 
 msgctxt "field:ir.model,global_search_p:"
 msgid "Global Search"
 msgstr ""
 
 msgctxt "field:ir.model,info:"
 msgid "Information"
@@ -820,31 +846,41 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr ""
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
-msgstr ""
+msgstr "Tanım"
 
 msgctxt "field:ir.model.access,group:"
 msgid "Group"
-msgstr ""
+msgstr "Grup"
 
 #, fuzzy
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -871,17 +907,22 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
 
 msgctxt "field:ir.model.button,reset_by:"
 msgid "Reset by"
@@ -920,15 +961,15 @@
 
 msgctxt "field:ir.model.button.rule,condition:"
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:ir.model.button.rule,description:"
 msgid "Description"
-msgstr ""
+msgstr "Tanım"
 
 msgctxt "field:ir.model.button.rule,number_user:"
 msgid "Number of User"
 msgstr ""
 
 msgctxt "field:ir.model.data,db_id:"
 msgid "Resource ID"
@@ -944,18 +985,28 @@
 
 #, fuzzy
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
@@ -980,42 +1031,66 @@
 
 #, fuzzy
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr ""
 
 msgctxt "field:ir.model.field,ttype:"
 msgid "Field Type"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,description:"
 msgid "Description"
-msgstr ""
+msgstr "Tanım"
 
-#, fuzzy
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
-msgstr "Fields"
+msgstr "Alan"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Alan"
 
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
-msgstr ""
+msgstr "Grup"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Models"
 
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
@@ -1048,31 +1123,31 @@
 
 msgctxt "field:ir.model.log,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
-msgstr ""
+msgstr "Filtre"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
-msgstr ""
+msgstr "Seviye"
 
 msgctxt "field:ir.module,childs:"
 msgid "Childs"
 msgstr ""
 
 msgctxt "field:ir.module,dependencies:"
 msgid "Dependencies"
 msgstr ""
 
 msgctxt "field:ir.module,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.module,parents:"
 msgid "Parents"
 msgstr ""
 
 msgctxt "field:ir.module,state:"
 msgid "State"
@@ -1107,15 +1182,15 @@
 #, fuzzy
 msgctxt "field:ir.module.dependency,module:"
 msgid "Module"
 msgstr "Modules"
 
 msgctxt "field:ir.module.dependency,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.module.dependency,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:ir.note,copy_to_resources:"
 msgid "Copy to Resources"
@@ -1175,46 +1250,52 @@
 msgid "Expected at"
 msgstr ""
 
 msgctxt "field:ir.queue,finished_at:"
 msgid "Finished at"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.queue,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.queue,scheduled_at:"
 msgid "Scheduled at"
 msgstr ""
 
 msgctxt "field:ir.rule,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:ir.rule,rule_group:"
 msgid "Group"
-msgstr ""
+msgstr "Grup"
 
 msgctxt "field:ir.rule.group,default_p:"
 msgid "Default"
 msgstr ""
 
 msgctxt "field:ir.rule.group,global_p:"
 msgid "Global"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.rule.group,perm_delete:"
 msgid "Delete Access"
@@ -1369,22 +1450,31 @@
 msgstr "Models"
 
 #, fuzzy
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr ""
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr ""
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr ""
@@ -1450,15 +1540,15 @@
 #, fuzzy
 msgctxt "field:ir.trigger,model:"
 msgid "Model"
 msgstr "Models"
 
 msgctxt "field:ir.trigger,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.trigger,on_create:"
 msgid "On Create"
 msgstr ""
 
 msgctxt "field:ir.trigger,on_delete:"
 msgid "On Delete"
@@ -1487,17 +1577,22 @@
 msgstr "Icons"
 
 #, fuzzy
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.menu,action:"
@@ -1543,44 +1638,67 @@
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr ""
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Export Translations"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr ""
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr ""
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr ""
 
 msgctxt "field:ir.ui.view,type:"
 msgid "View Type"
@@ -1593,24 +1711,24 @@
 #, fuzzy
 msgctxt "field:ir.ui.view_search,model:"
 msgid "Model"
 msgstr "Models"
 
 msgctxt "field:ir.ui.view_search,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:ir.ui.view_search,user:"
 msgid "User"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,field:"
 msgid "Field"
-msgstr "Fields"
+msgstr "Alan"
 
 msgctxt "field:ir.ui.view_tree_optional,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_optional,value:"
 msgid "Value"
@@ -1642,24 +1760,33 @@
 msgid "Selected Nodes"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_state,user:"
 msgid "User"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
-msgstr "Fields"
+msgstr "Alan"
+
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Alan"
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr ""
@@ -1762,15 +1889,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1794,15 +1921,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -1993,14 +2120,15 @@
 msgid "Fields Access"
 msgstr "Fields Access"
 
 msgctxt "model:ir.action,name:act_model_field_access_form_relate_field"
 msgid "Access"
 msgstr "Access"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_model_fields_form"
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
@@ -2505,17 +2633,18 @@
 msgid "Configure languages"
 msgstr "Configure Modules"
 
 msgctxt "model:ir.message,name:"
 msgid "Message"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_ID"
 msgid "ID"
-msgstr ""
+msgstr "ID"
 
 msgctxt "model:ir.message,text:msg_access_button_error"
 msgid "Calling button \"%(button)s on \"%(model)s\" is not allowed."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_access_rule_error"
 msgid "You are not allowed to access \"%(model)s\"."
@@ -2590,14 +2719,22 @@
 msgid "This record is part of the base configuration."
 msgstr "This record is part of the base configuration."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_created_at"
@@ -2689,17 +2826,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_multiselection"
 msgid "MultiSelection"
 msgstr "Scheduled Actions"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_name"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "model:ir.message,text:msg_dict_schema_numeric"
 msgid "Numeric"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_selection"
@@ -3093,14 +3231,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 #, fuzzy
@@ -3546,14 +3688,15 @@
 msgid "Tree State"
 msgstr "Tree State"
 
 msgctxt "model:ir.ui.menu,name:menu_view_tree_width"
 msgid "View Tree Width"
 msgstr "View Tree Width"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:model_model_fields_form"
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.ui.menu.favorite,name:"
 msgid "Menu Favorite"
 msgstr ""
@@ -3939,18 +4082,17 @@
 msgid "Hexadecimal Timestamp"
 msgstr ""
 
 msgctxt "selection:ir.sequence.strict,type:"
 msgid "Incremental"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:ir.translation,type:"
 msgid "Field"
-msgstr "Fields"
+msgstr "Alan"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Help"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.translation,type:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/fr.po` & `trytond-7.2.1/trytond/ir/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Context Domain"
 msgstr "Contexte du domaine"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Modèle de context"
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Modèle de context"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Valeur du domaine"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domaines"
@@ -102,14 +106,18 @@
 msgid "Records"
 msgstr "Enregistrements"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Critères de recherche"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Type"
@@ -186,18 +194,26 @@
 msgid "Keywords"
 msgstr "Mots-clés"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Nom de l'enregistrement"
@@ -294,14 +310,18 @@
 msgid "Keywords"
 msgstr "Mots-clés"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Enregistrements"
@@ -778,14 +798,18 @@
 msgid "Model Name"
 msgstr "Nom du modèle"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Description du modèle"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Description"
@@ -794,14 +818,18 @@
 msgid "Group"
 msgstr "Groupe"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Accès en creation"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Accès en suppression"
@@ -826,14 +854,18 @@
 msgid "Help"
 msgstr "Aide"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Réinitialiser"
@@ -894,18 +926,26 @@
 msgid "Values on File System"
 msgstr "Valeurs sur le système de fichier"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Pas de mise à jour"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Désynchronisé"
@@ -926,18 +966,26 @@
 msgid "Help"
 msgstr "Aide"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Modèle associé"
@@ -950,18 +998,30 @@
 msgid "Description"
 msgstr "Description"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Champ"
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Champ"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Groupe"
 
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Modèle"
+
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Accès en creation"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Accès en suppression"
@@ -1142,14 +1202,18 @@
 msgid "Global"
 msgstr "Global"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Accès en creation"
@@ -1298,22 +1362,30 @@
 msgid "Model"
 msgstr "Modèle"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Nom du champ"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Module surchargeant"
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Module surchargeant"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID de la ressource"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Source"
@@ -1406,14 +1478,18 @@
 msgid "Icon"
 msgstr "Icône"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Chemin vers le fichier SVG"
@@ -1458,38 +1534,58 @@
 msgid "User"
 msgstr "Utilisateur"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Architecture de la vue"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr "Base"
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Données"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domaine"
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Extensions"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Champ enfant"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
-msgstr "Champs enfants"
+msgstr "Champ enfant"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Vue héritée"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Priorité"
@@ -1554,18 +1650,26 @@
 msgid "User"
 msgstr "Utilisateur"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Champ"
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Champ"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Modèle"
 
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Utilisateur"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Largeur"
@@ -1678,15 +1782,15 @@
 msgid "RFC 4646 tag."
 msgstr "Balise RFC 4646."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Code du parent exceptionnel"
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Module dans lequel ce modèle est défini."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "Le texte pour demander confirmation à l'utilisateur quand il clique sur le "
@@ -1716,15 +1820,15 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Si coché, le droit d'accès sur le modèle du champ est également testé par "
 "rapport à la relation du champ."
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Module dans lequel ce champ est défini."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2523,14 +2627,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Cet enregistrement fait partie de la configuration de base."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Le nom du bouton doit être unique par modèle."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr "À la date/heure : %(datetime)s"
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr "Au sein des groupes : %(groups)s"
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Vous n'êtes pas autorisé à créer les enregistrements de « %(model)s » car ils échouent à au moins une de ces règles :\n"
 "%(rules)s"
@@ -2662,32 +2774,30 @@
 msgid "Type"
 msgstr "Type"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Oui"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
 "record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "Le nombre de décimales de la valeur « %(value)r » pour le champs "
-"« %(field)s » sur « %(record)s » de « %(model)s » excède la limite de "
-"« %(digits)i »."
+"« %(field)s » sur l'enregistrement « %(record)s » de « %(model)s » excède la"
+" limite de « %(digits)i »."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
-"La valeur « %(value)s » du champ « %(field)s » sur « %(record)s » de "
-"« %(model)s » n'est pas valide selon son domaine."
+"La valeur « %(value)s » du champ « %(field)s » sur l'enregistrement "
+"« %(record)s » de « %(model)s » n'est pas valide selon son domaine."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Édité le"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
@@ -2727,24 +2837,24 @@
 
 msgctxt "model:ir.message,text:msg_field_model_name"
 msgid "%(field)s (model name)"
 msgstr "%(field)s (nom du modèle)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
-msgstr "%(champ)s (chaîne)"
+msgstr "%(field)s (chaîne)"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
-"La valeur « %(value)s » pour le champ « %(field)s » dans « %(record)s » de "
-"« %(model)s » contient des caractères non valides « %(chars)s »."
+"La valeur « %(value)s » pour le champ « %(field)s » sur l'enregistrement "
+"« %(record)s » de « %(model)s » contient des caractères non valides "
+"« %(chars)s »."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 "Les enregistrements ne peuvent pas être supprimés car ils sont utilisés par "
@@ -2860,22 +2970,21 @@
 "Définition de nom d'enregistrement non valide pour le rapport « %(report)s »"
 " avec l'exception «%(exception)s »."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Une valeur est requise pour le champ « %(field)s » sur « %(model)s »."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
 msgid ""
 "A value is required for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\"."
 msgstr ""
-"Une valeur est requise pour le champ « %(field)s » sur « %(record)s » de "
-"« %(model)s »."
+"Une valeur est requise pour le champ « %(field)s » sur l'enregistrement "
+"« %(record)s » de « %(model)s »."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Les ressources sur lesquelles cet enregistrement doit être copié."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
@@ -2883,22 +2992,21 @@
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 "Fonction de recherche manquante pour le champ « %(field)s » sur "
 "« %(model)s »."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
-"La valeur « %(value)s » pour le champ « %(field)s » sur « %(record)s » de "
-"« %(model)s » n'est pas une des options permises."
+"La valeur « %(value)s » pour le champ « %(field)s » sur l'enregistrement "
+"« %(record)s » de « %(model)s » n'est pas une des options permises."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Séquence"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
@@ -2948,31 +3056,29 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "La valeur « %(value)s » pour le champ « %(field)s » sur « %(model)s » est "
 "trop longue (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"La valeur « %(value)s » pour le champ « %(field)s » sur « %(record)s » de "
-"« %(model)s » est trop longue (%(size)i > %(max_size)i)."
+"La valeur « %(value)s » pour le champ « %(field)s » sur l'enregistrement "
+"« %(record)s » de « %(model)s » est trop longue (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
 "The time value \"%(value)s\" for field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "La valeur de temps « %(value)s » pour le champ « %(field)s » sur "
-"« %(record)s » de « %(model)s » n'est pas valide."
+"l'enregistrement « %(record)s » de « %(model)s » n'est pas valide."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
 msgid "Y"
@@ -3063,22 +3169,25 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Vous n'êtes pas autorisé à écrire sur les enregistrements « %(ids)s » de « %(model)s » à cause d'au moins une de ces règles :\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "Vous n'êtes pas autorisé à modifier le champ « %(field)s » sur "
-"« %(record)s » de « %(model)s »."
+"l'enregistrement « %(record)s » de « %(model)s »."
+
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr "XML ID"
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Erreur de syntaxe pour l'id XML : %(value)r sur « %(field)s » de "
```

### Comparing `trytond-7.2.0/trytond/ir/locale/hu.po` & `trytond-7.2.1/trytond/ir/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Összefüggés"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Értéktartomány"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Értéktartomány"
@@ -105,14 +110,19 @@
 msgid "Records"
 msgstr "Adat ID"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Keresési feltételek"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Típus"
@@ -190,18 +200,28 @@
 msgid "Keywords"
 msgstr "Kulcsszavak"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Név"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -301,14 +321,19 @@
 msgid "Keywords"
 msgstr "Kulcsszavak"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Név"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -801,14 +826,19 @@
 msgid "Model Name"
 msgstr "Mintanév"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Minta leírás"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Leírás"
@@ -817,14 +847,19 @@
 msgid "Group"
 msgstr "Csoport"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Létrehozni"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Törlés"
@@ -850,14 +885,19 @@
 msgid "Help"
 msgstr "Súgó"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
@@ -918,18 +958,28 @@
 msgid "Values on File System"
 msgstr "Értékek a fájlrendszerben"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Nincs frissítés"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Nem szinkronizált"
@@ -951,18 +1001,28 @@
 msgid "Help"
 msgstr "Súgó"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Minta kapcsolat"
@@ -975,18 +1035,33 @@
 msgid "Description"
 msgstr "Leírás"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Mező"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Mező"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Csoport"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Minta"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Létrehoz"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Törlés"
@@ -1173,14 +1248,19 @@
 msgid "Global"
 msgstr "A teljes alkalmazásban érvényes"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Létrehozás"
@@ -1331,22 +1411,32 @@
 msgid "Model"
 msgstr "Minta"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Mezőnév"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Átírandó modul"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Átírandó modul"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "Rekord ID"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Forrás"
@@ -1439,14 +1529,19 @@
 msgid "Icon"
 msgstr "Ikon"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "SVG útvonal"
@@ -1491,38 +1586,62 @@
 msgid "User"
 msgstr "Felhasználó"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Nézet felépítése"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Adat"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Érvényesség"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Dokumentum típusa"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Alárendelt mező"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Alárendelt mező"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Örökölt nézet"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioritás"
@@ -1591,18 +1710,28 @@
 msgid "User"
 msgstr "Felhasználó"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Mező"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Mező"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Minta"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Felhasználó"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Szélesség"
@@ -1718,15 +1847,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Modul, melyben ez a minta van definiálva"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1753,15 +1882,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Modul, melyben ez a mező van definiálva"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2602,14 +2731,22 @@
 msgstr "This record is part of the base configuration."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Egy modul neve csak egyszer adható."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nem tud „%(model)s” rekordokat létrehozni, mert a következő szabályok legalább egyike nem teljesül:\n"
 "%(rules)s"
@@ -3140,14 +3277,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "A „%(model)s” elem „%(field)s” mezőjét ki kell tölteni."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/id.po` & `trytond-7.2.1/trytond/ir/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr ""
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr ""
@@ -104,14 +108,19 @@
 msgid "Records"
 msgstr "Rekaman"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Kriteria Pencarian"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Jenis"
@@ -189,18 +198,28 @@
 msgid "Keywords"
 msgstr "Kata Kunci"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nama"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -298,14 +317,19 @@
 msgid "Keywords"
 msgstr "Kata Kunci"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nama"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -797,14 +821,19 @@
 msgid "Model Name"
 msgstr "Nama Model"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Deskripsi Model"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Deskripsi"
@@ -813,14 +842,19 @@
 msgid "Group"
 msgstr "Kelompok"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -845,14 +879,19 @@
 msgid "Help"
 msgstr "Bantuan"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
@@ -913,18 +952,28 @@
 msgid "Values on File System"
 msgstr ""
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Tidak Ada Pembaharuan"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr ""
@@ -945,18 +994,28 @@
 msgid "Help"
 msgstr "Bantuan"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr ""
@@ -969,18 +1028,32 @@
 msgid "Description"
 msgstr "Deskripsi"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr ""
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr ""
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Kelompok"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Model"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -1165,14 +1238,19 @@
 msgid "Global"
 msgstr ""
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr ""
@@ -1323,22 +1401,31 @@
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr ""
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID Sumber daya"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
@@ -1432,14 +1519,19 @@
 msgid "Icon"
 msgstr ""
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr ""
@@ -1484,38 +1576,61 @@
 msgid "User"
 msgstr "Pengguna"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr ""
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr ""
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Cabang"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr ""
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr ""
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioritas"
@@ -1581,18 +1696,27 @@
 msgid "User"
 msgstr "Pengguna"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr ""
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr ""
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Pengguna"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Lebar"
@@ -1695,15 +1819,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1727,15 +1851,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2519,14 +2643,22 @@
 msgid "This record is part of the base configuration."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_created_at"
@@ -2993,14 +3125,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "Kesalahan sintaks untuk id XML: \"%(value)r\" di dalam \"%(field)s\"."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/it.po` & `trytond-7.2.1/trytond/ir/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "modello context"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "modello context"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Valore di Dominio"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Dominii"
@@ -105,14 +110,19 @@
 msgid "Records"
 msgstr "Record ID"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Criteri di ricerca"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tipo"
@@ -190,18 +200,28 @@
 msgid "Keywords"
 msgstr "Keywords"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nome"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -302,14 +322,19 @@
 msgid "Keywords"
 msgstr "Keywords"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nome"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -817,14 +842,19 @@
 msgid "Model Name"
 msgstr "Nome modello"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Descrizione Modello"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Descrizione"
@@ -833,14 +863,19 @@
 msgid "Group"
 msgstr "Gruppo"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Creazione Accesso"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Eliminazione dell'accesso"
@@ -866,14 +901,19 @@
 msgid "Help"
 msgstr "Aiuto"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Azzera"
@@ -934,18 +974,28 @@
 msgid "Values on File System"
 msgstr "Valori nel File System"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Nessun Aggiornamento"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Out of Sync"
@@ -967,18 +1017,28 @@
 msgid "Help"
 msgstr "Aiuto"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Relazione modello"
@@ -991,18 +1051,33 @@
 msgid "Description"
 msgstr "Descrizione"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Campo"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Campo"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Gruppo"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Modello"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Creazione Accesso"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Eliminazione dell'accesso"
@@ -1189,14 +1264,19 @@
 msgid "Global"
 msgstr "Globale"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Creazione Accesso"
@@ -1347,22 +1427,32 @@
 msgid "Model"
 msgstr "Modello"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Nome campo"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Modulo non tenuto in conto"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Modulo non tenuto in conto"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID Risorsa"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Source"
@@ -1459,14 +1549,19 @@
 msgid "Icon"
 msgstr "Icona"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Percorso SVG"
@@ -1511,38 +1606,62 @@
 msgid "User"
 msgstr "Utente"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Architettura della vista"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Dati"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Dominio"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Estensione"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Campo Figlio"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Campo Figlio"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Vista incrementale"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modulo"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modulo"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "PrioritÃÂÃÂÃÂÃÂÃÂÃÂÃÂÃÂ "
@@ -1611,18 +1730,28 @@
 msgid "User"
 msgstr "Utente"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Campo"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Campo"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Modello"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Utente"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Larghezza"
@@ -1738,15 +1867,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Modulo dove ÃÂÃÂÃÂÃÂÃÂÃÂÃÂÃÂ¨ definito questo modello"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1774,15 +1903,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Modulo dove ÃÂÃÂÃÂÃÂÃÂÃÂÃÂÃÂ¨ definito questo campo"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2656,14 +2785,22 @@
 msgstr "This record is part of the base configuration."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Il nome del modulo dev'essere unico"
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_created_at"
@@ -3202,14 +3339,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/lo.po` & `trytond-7.2.1/trytond/ir/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr ""
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr ""
@@ -114,14 +118,19 @@
 msgstr "Record Rules"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
@@ -213,19 +222,29 @@
 
 #, fuzzy
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -336,14 +355,19 @@
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -859,14 +883,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
@@ -878,14 +907,19 @@
 msgstr "ໝວດ"
 
 #, fuzzy
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -913,14 +947,19 @@
 
 #, fuzzy
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
@@ -988,18 +1027,28 @@
 
 #, fuzzy
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
@@ -1025,19 +1074,29 @@
 
 #, fuzzy
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr ""
@@ -1053,18 +1112,33 @@
 
 #, fuzzy
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "ຟິນລ໌"
 
 #, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "ຟິນລ໌"
+
+#, fuzzy
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "ໝວດ"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -1264,14 +1338,19 @@
 
 #, fuzzy
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr ""
@@ -1431,22 +1510,31 @@
 msgstr "Models"
 
 #, fuzzy
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr ""
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr ""
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr ""
@@ -1552,14 +1640,19 @@
 
 #, fuzzy
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr ""
@@ -1610,42 +1703,66 @@
 msgid "User"
 msgstr "ຜູ້ໃຊ້"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr ""
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "ວັນທີ:"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Export Translations"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "ໝວດຍ່ອຍ"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr ""
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modules"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr ""
@@ -1721,19 +1838,29 @@
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "ຟິນລ໌"
 
 #, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "ຟິນລ໌"
+
+#, fuzzy
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "ຜູ້ໃຊ້"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr ""
@@ -1836,15 +1963,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1868,15 +1995,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2688,14 +2815,22 @@
 msgid "This record is part of the base configuration."
 msgstr "This record is part of the base configuration."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -3197,14 +3332,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 #, fuzzy
```

### Comparing `trytond-7.2.0/trytond/ir/locale/lt.po` & `trytond-7.2.1/trytond/ir/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 msgid "Context Domain"
 msgstr "Konteksto domenas"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Konteksto modelis"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Konteksto modelis"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Domeno vertė"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domenai"
@@ -105,14 +110,19 @@
 msgid "Records"
 msgstr "Įrašo ID"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Paieškos kriterijus"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tipas"
@@ -190,18 +200,28 @@
 msgid "Keywords"
 msgstr "Raktiniai žodžiai"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -301,14 +321,19 @@
 msgid "Keywords"
 msgstr "Raktiniai žodžiai"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -811,14 +836,19 @@
 msgid "Model Name"
 msgstr "Modelio pavadinimas"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Modelio aprašymas"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Aprašymas"
@@ -827,14 +857,19 @@
 msgid "Group"
 msgstr "Groupė"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Teisė sukurti"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Teisė trinti"
@@ -859,14 +894,19 @@
 msgid "Help"
 msgstr "Pagalba"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Atstatyti"
@@ -927,18 +967,28 @@
 msgid "Values on File System"
 msgstr "Failų sistemos vertės"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Nėra atnaujinimų"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Nesinchronizuota"
@@ -960,18 +1010,28 @@
 msgid "Help"
 msgstr "Pagalba"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Modelio ryšys"
@@ -984,18 +1044,33 @@
 msgid "Description"
 msgstr "Aprašymas"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Laukas"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Laukas"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Groupė"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Modelis"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Teisė sukurti"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Teisė trinti"
@@ -1181,14 +1256,19 @@
 msgid "Global"
 msgstr "Globali"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Teisė sukurti"
@@ -1339,22 +1419,32 @@
 msgid "Model"
 msgstr "Modelis"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Lauko pavadinimas"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Perrašantis modulis"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Perrašantis modulis"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "Resurso ID"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Šaltinis"
@@ -1451,14 +1541,19 @@
 msgid "Icon"
 msgstr "Ikona"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Kelias prie SVG"
@@ -1503,38 +1598,62 @@
 msgid "User"
 msgstr "Naudotojas"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Rodinio architektūra"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Duomenys"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domenas"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Plėtinys"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Dukterinis laukas"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Dukterinis laukas"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Paveldėtas rodinys"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modulis"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modulis"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioritetas"
@@ -1603,18 +1722,28 @@
 msgid "User"
 msgstr "Naudotojas"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Laukas"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Laukas"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Modelis"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Naudotojas"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Plotis"
@@ -1717,15 +1846,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1749,15 +1878,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2546,14 +2675,22 @@
 msgid "This record is part of the base configuration."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_created_at"
@@ -3051,14 +3188,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/nl.po` & `trytond-7.2.1/trytond/ir/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Context Domain"
 msgstr "Context domein"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Context model"
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Context model"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Domein waarde"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domeinen"
@@ -102,14 +106,18 @@
 msgid "Records"
 msgstr "Records"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Zoekargumenten"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Type"
@@ -186,18 +194,26 @@
 msgid "Keywords"
 msgstr "Trefwoorden"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Recordnaam"
@@ -294,14 +310,18 @@
 msgid "Keywords"
 msgstr "Trefwoorden"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Records"
@@ -778,14 +798,18 @@
 msgid "Model Name"
 msgstr "Naam model"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Model omschrijving"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Omschrijving"
@@ -794,14 +818,18 @@
 msgid "Group"
 msgstr "Groep"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Toegang aanmaken"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Toegang verwijderen"
@@ -826,14 +854,18 @@
 msgid "Help"
 msgstr "Help"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Resetten"
@@ -894,18 +926,26 @@
 msgid "Values on File System"
 msgstr "Waarden op bestandssysteem"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Niet bijwerken"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Niet gesynchroniseerd"
@@ -926,18 +966,26 @@
 msgid "Help"
 msgstr "Help"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Model relatie"
@@ -950,18 +998,30 @@
 msgid "Description"
 msgstr "Omschrijving"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Veld"
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Veld"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Groep"
 
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Model"
+
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Toegang aanmaken"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Toegang verwijderen"
@@ -1142,14 +1202,18 @@
 msgid "Global"
 msgstr "Algmeen"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Toegang aanmaken"
@@ -1298,22 +1362,30 @@
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Veldnaam"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Module overschrijven"
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Module overschrijven"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "Bron ID"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Bron"
@@ -1406,14 +1478,18 @@
 msgid "Icon"
 msgstr "Pictogram"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "SVG pad"
@@ -1458,38 +1534,58 @@
 msgid "User"
 msgstr "Gebruiker"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Architectuur weergave"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr "Basis"
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Gegevens"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domein"
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Extensies"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Onderliggende velden"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Onderliggende velden"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Overgenomen weergave"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Module"
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Module"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioriteit"
@@ -1554,18 +1650,26 @@
 msgid "User"
 msgstr "Gebruiker"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Veld"
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Veld"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Gebruiker"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Breedte"
@@ -1679,15 +1783,15 @@
 msgid "RFC 4646 tag."
 msgstr "RFC 4646-tag."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Code van de uitzonderlijke ouder"
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Module waarin dit model is gedefinieerd."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "Tekst om bevestiging van de gebruiker te vragen wanneer er op de knop wordt "
@@ -1717,15 +1821,15 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Indien aangevinkt, wordt het toegangsrecht op het model van het veld ook "
 "getoetst aan de relatie van het veld."
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Module waarin dit veld is gedefinieerd."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2522,14 +2626,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Deze record maakt deel uit van de basisconfiguratie."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "De naam van de knop moet uniek zijn per model."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr "Op datum/tijd: %(datetime)s"
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr "Binnen de groepen: %(groups)s"
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "U mag geen records van \"%(model)s\" aanmaken omdat ze ten minste één van deze regels niet naleven:\n"
 "%(rules)s"
@@ -2662,32 +2774,30 @@
 msgid "Type"
 msgstr "Type"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Ja"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
 "record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
-"Het aantal decimalen in de waarde \"%(value)s\" voor het veld \"%(field)s\" "
-"in \"%(record)s\" van \"%(model)s\" overschrijdt de limiet van "
+"Het aantal decimalen in de waarde \"%(value)r\" voor veld \"%(field)s\" in "
+"record \"%(record)s\" van \"%(model)s\" overschrijdt de limiet van "
 "\"%(digits)i\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
-"De waarde \"%(value)s\" voor veld \"%(field)s\" in \"%(record)s\" van "
-"\"%(model)s\" valt niet binnen het geldige waardebereik."
+"De waarde \"%(value)s\" voor veld \"%(field)s\" in record \"%(record)s\" van"
+" \"%(model)s\" valt niet binnen het geldige waardebereik."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Bewerkt op"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
@@ -2729,22 +2839,21 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (model naam)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (tekst)"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
-"De waarde \"%(value)s\" voor veld \"%(field)s\" in \"%(record)s\" van "
-"\"%(model)s\" bevat ongeldige tekens \"%(chars)s\"."
+"De waarde \"%(value)s\" voor veld \"%(field)s\" in record \"%(record)s\" van"
+" \"%(model)s\" bevat ongeldige tekens \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 "De records konden niet worden verwijderd omdat ze worden gebruikt door veld "
@@ -2857,15 +2966,14 @@
 "Ongeldige recordnaamdefinitie voor rapport \"%(report)s\" met uitzondering "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Een waarde is vereist voor veld \"%(field)s\" in \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
 msgid ""
 "A value is required for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\"."
 msgstr ""
 "Een waarde is vereist voor veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\"."
@@ -2878,22 +2986,21 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "Ongeldig domein in regel \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Zoekfunctie ontbreekt voor veld \"%(field)s\" in \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
-"De waarde \"%(value)s\" voor het veld \"%(field)s\" in \"%(record)s\" van "
-"\"%(model)s\" is geen van de toegestane opties."
+"De waarde \"%(value)s\" voor veld \"%(field)s\" in record \"%(record)s\" van"
+" \"%(model)s\" is geen van de toegestane opties."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Reeks"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
@@ -2909,15 +3016,15 @@
 "(%(number_next)s) with exception \"%(exception)s\"."
 msgstr ""
 "Ongeldig \"Toenamenummer\" (%(number_increment)s) of \"Volgend nummer\" "
 "(%(number_next)s) met uitzondering \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_prefix"
 msgid "Invalid prefix \"%(affix)s\" for sequence \"%(sequence)s\"."
-msgstr "Ongeldig voorvoegsel \"%(affix) s\" voor reeks \"%(sequence)s\"."
+msgstr "Ongeldig voorvoegsel \"%(affix)s\" voor reeks \"%(sequence)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_suffix"
 msgid "Invalid suffix \"%(affix)s\" for sequence \"%(sequence)s\"."
 msgstr "Ongeldig achtervoegsel \"%(affix)s\" voor reeks \"%(sequence)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_last_timestamp_future"
 msgid "The \"Last Timestamp\" cannot be in the future for sequence \"%s\"."
@@ -2938,33 +3045,31 @@
 msgstr "Er kan slecht één singleton worden aangemaakt."
 
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
-"De waarde voor veld \"%(field)s\" in \"%(model)s\" is te lang (%(size)i > "
-"%(max_size)i)."
+"De waarde \"%(value)s\" voor veld \"%(field)s\" in \"%(model)s\" is te lang "
+"(%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"De waarde voor veld \"%(field)s\" in \"%(record)s\" van \"%(model)s\" is te "
-"lang (%(size)i > %(max_size)i)."
+"De waarde \"%(value)s\" voor veld \"%(field)s\" in record \"%(record)s\" van"
+" \"%(model)s\" is te lang (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
 "The time value \"%(value)s\" for field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
-"De tijd \"%(value)s\" voor veld \"%(field)s\" in \"%(record)s\" van "
+"De tijd \"%(value)s\" voor veld \"%(field)s\" in record \"%(record)s\" van "
 "\"%(model)s\" is niet geldig."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
@@ -2996,16 +3101,16 @@
 msgstr "Te veel relaties gevonden: %(value)r\" in \"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_translation_overridden"
 msgid ""
 "You can not export translation \"%(name)s\" because it has been overridden "
 "by module \"%(overriding_module)s\"."
 msgstr ""
-"U kunt vertaling \"%(name)s\" niet exporteren omdat deze overschreven wordt "
-"door module %(value)r\" in \"%(model)s\"."
+"U kunt de vertaling \"%(name)s\" niet exporteren omdat deze is overschreven "
+"door module \"%(overriding_module)s\"."
 
 msgctxt "model:ir.message,text:msg_trigger_exclusive"
 msgid ""
 "You can not select \"On Time\" and any other on the same time, they are "
 "mutually exclusive."
 msgstr ""
 "U kunt niet tegelijkertijd \"Op Tijd\" en iets anders selecteren; ze sluiten"
@@ -3029,15 +3134,15 @@
 
 msgctxt "model:ir.message,text:msg_view_invalid_xml"
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr "Ongeldige XML voor weergave \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
-msgstr "Ongeldig domein of zoekcriteria \"%(domain)s\" voor zoekactie \"%(action)s\"."
+msgstr "Ongeldig domein of zoekcriteria \"%(domain)s\" voor zoekactie \"%(search)s\"."
 
 msgctxt "model:ir.message,text:msg_view_tree_optional_type"
 msgid "You cannot store optional on view \"%(view)s\"."
 msgstr "U kunt de optionele weergave niet opslaan in weergave \"%(view)s\"."
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
@@ -3051,23 +3156,26 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Het is niet toegestaan om te schrijven in de records \"%(ids)s\" van \"%(model)s\"vanwege ten minste één van deze regels:\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
-"U hebt geen rechten om het veld \"%(field)s\" in \"%(record)s\" van "
+"U hebt geen rechten om het veld \"%(field)s\" van record \"%(record)s\" van "
 "\"%(model)s\" te wijzigen."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr "XML id"
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Syntaxfout voor XML-id: \"%(value)r\" in \"%(field)s\" van \"%(model)s\" "
 "(%(column)s)."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/pl.po` & `trytond-7.2.1/trytond/ir/locale/pl.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:ir.action,action:"
 msgid "Action"
 msgstr "Akcja"
 
 msgctxt "field:ir.action,icon:"
 msgid "Icon"
 msgstr "Ikona"
@@ -15,18 +14,17 @@
 msgid "Keywords"
 msgstr "Słowa kluczowe"
 
 msgctxt "field:ir.action,name:"
 msgid "Name"
 msgstr "Nazwa"
 
-#, fuzzy
 msgctxt "field:ir.action,records:"
 msgid "Records"
-msgstr "ID rekordu"
+msgstr "Rekordy"
 
 msgctxt "field:ir.action,type:"
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "field:ir.action,usage:"
 msgid "Usage"
@@ -52,14 +50,18 @@
 msgid "Context Domain"
 msgstr "Domena kontekstu"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Model kontekstu"
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Model kontekstu"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Wartość domeny"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domeny"
@@ -96,23 +98,26 @@
 msgid "PySON Order"
 msgstr "Porządek PySON"
 
 msgctxt "field:ir.action.act_window,pyson_search_value:"
 msgid "PySON Search Criteria"
 msgstr "Kryteria wyszukiwania PySON"
 
-#, fuzzy
 msgctxt "field:ir.action.act_window,records:"
 msgid "Records"
-msgstr "ID rekordu"
+msgstr "Rekordy"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Kryteria wyszukiwania"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Typ"
@@ -141,15 +146,14 @@
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Akcja"
 
-#, fuzzy
 msgctxt "field:ir.action.act_window.view,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Widok"
@@ -190,31 +194,37 @@
 msgid "Keywords"
 msgstr "Słowa kluczowe"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nazwa"
 
-#, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Nazwa rekordu"
 
-#, fuzzy
 msgctxt "field:ir.action.report,records:"
 msgid "Records"
-msgstr "ID rekordu"
+msgstr "Rekordy"
 
 msgctxt "field:ir.action.report,report:"
 msgid "Path"
 msgstr "Ścieżka"
 
 msgctxt "field:ir.action.report,report_content:"
 msgid "Content"
@@ -268,18 +278,17 @@
 msgid "Keywords"
 msgstr "Słowa kluczowe"
 
 msgctxt "field:ir.action.url,name:"
 msgid "Name"
 msgstr "Nazwa"
 
-#, fuzzy
 msgctxt "field:ir.action.url,records:"
 msgid "Records"
-msgstr "ID rekordu"
+msgstr "Rekordy"
 
 msgctxt "field:ir.action.url,type:"
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "field:ir.action.url,url:"
 msgid "Action Url"
@@ -301,22 +310,25 @@
 msgid "Keywords"
 msgstr "Słowa kluczowe"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nazwa"
 
-#, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
-msgstr "ID rekordu"
+msgstr "Rekordy"
 
 msgctxt "field:ir.action.wizard,type:"
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "field:ir.action.wizard,usage:"
 msgid "Usage"
@@ -378,71 +390,65 @@
 msgid "Summary"
 msgstr "Skrót opisu"
 
 msgctxt "field:ir.attachment,type:"
 msgid "Type"
 msgstr "Typ"
 
-#, fuzzy
 msgctxt "field:ir.avatar,cache:"
 msgid "Cache"
 msgstr "Pamięć podręczna"
 
-#, fuzzy
 msgctxt "field:ir.avatar,copy_to_resources:"
 msgid "Copy to Resources"
 msgstr "Skopiuj do zasobów"
 
-#, fuzzy
 msgctxt "field:ir.avatar,copy_to_resources_visible:"
 msgid "Copy to Resources Visible"
 msgstr "Kopiuj do widocznych zasobów"
 
 msgctxt "field:ir.avatar,image:"
 msgid "Image"
-msgstr ""
+msgstr "Obraz"
 
 msgctxt "field:ir.avatar,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "ID obrazu"
 
-#, fuzzy
 msgctxt "field:ir.avatar,last_modification:"
 msgid "Last Modification"
 msgstr "Ostatnia modyfikacja"
 
-#, fuzzy
 msgctxt "field:ir.avatar,last_user:"
 msgid "Last User"
 msgstr "Ostatnio używał"
 
-#, fuzzy
 msgctxt "field:ir.avatar,resource:"
 msgid "Resource"
 msgstr "Zasób"
 
 msgctxt "field:ir.avatar,uuid:"
 msgid "UUID"
-msgstr ""
+msgstr "UUID"
 
 msgctxt "field:ir.avatar.cache,avatar:"
 msgid "Avatar"
-msgstr ""
+msgstr "Avatar"
 
 msgctxt "field:ir.avatar.cache,image:"
 msgid "Image"
-msgstr ""
+msgstr "Obraz"
 
 msgctxt "field:ir.avatar.cache,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "ID obrazu"
 
 msgctxt "field:ir.avatar.cache,size:"
 msgid "Size"
-msgstr ""
+msgstr "Rozmiar"
 
 msgctxt "field:ir.cache,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.cache,timestamp:"
 msgid "Timestamp"
@@ -504,18 +510,17 @@
 msgid "Minute"
 msgstr "Minuta"
 
 msgctxt "field:ir.cron,next_call:"
 msgid "Next Call"
 msgstr "Kolejne wywołanie"
 
-#, fuzzy
 msgctxt "field:ir.cron,timezone:"
 msgid "Timezone"
-msgstr "Czas"
+msgstr "Strefa czasowa"
 
 msgctxt "field:ir.cron,weekday:"
 msgid "Day of Week"
 msgstr "Dzień tygodnia"
 
 msgctxt "field:ir.email,addresses:"
 msgid "Addresses"
@@ -613,69 +618,62 @@
 msgid "Report"
 msgstr "Raport"
 
 msgctxt "field:ir.email.template-ir.action.report,template:"
 msgid "Template"
 msgstr "Szablon"
 
-#, fuzzy
 msgctxt "field:ir.error,description:"
 msgid "Description"
 msgstr "Opis"
 
-#, fuzzy
 msgctxt "field:ir.error,message:"
 msgid "Message"
 msgstr "Wiadomość"
 
 msgctxt "field:ir.error,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Pochodzenie"
 
-#, fuzzy
 msgctxt "field:ir.error,processed_by:"
 msgid "Processed by"
-msgstr "Utworzył"
+msgstr "Przetworzył"
 
 msgctxt "field:ir.error,solved_by:"
 msgid "Solved by"
-msgstr ""
+msgstr "Rozwiązał"
 
-#, fuzzy
 msgctxt "field:ir.error,state:"
 msgid "State"
 msgstr "Stan"
 
-#, fuzzy
 msgctxt "field:ir.error,summary:"
 msgid "Summary"
-msgstr "Skrót opisu"
+msgstr "Streszczenie"
 
 msgctxt "field:ir.export,export_fields:"
 msgid "Fields"
 msgstr "Pola"
 
 msgctxt "field:ir.export,header:"
 msgid "Header"
-msgstr ""
+msgstr "Nagłówek"
 
 msgctxt "field:ir.export,name:"
 msgid "Name"
 msgstr "Nazwa"
 
-#, fuzzy
 msgctxt "field:ir.export,records:"
 msgid "Records"
-msgstr "ID rekordu"
+msgstr "Rekordy"
 
 msgctxt "field:ir.export,resource:"
 msgid "Resource"
 msgstr "Zasób"
 
-#, fuzzy
 msgctxt "field:ir.export,user:"
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:ir.export.line,export:"
 msgid "Export"
 msgstr "Wyeksportuj"
@@ -754,15 +752,15 @@
 
 msgctxt "field:ir.lang,parent:"
 msgid "Parent Code"
 msgstr "Kod elementu nadrzędnego"
 
 msgctxt "field:ir.lang,pg_text_search:"
 msgid "PostgreSQL Text Search Configuration"
-msgstr ""
+msgstr "Konfiguracja wyszukiwania tekstowego PostgreSQL"
 
 msgctxt "field:ir.lang,pm:"
 msgid "PM"
 msgstr "po południu"
 
 msgctxt "field:ir.lang,positive_sign:"
 msgid "Positive Sign"
@@ -800,14 +798,18 @@
 msgid "Model Name"
 msgstr "Nazwa modelu"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Opis modelu"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Opis"
@@ -816,14 +818,18 @@
 msgid "Group"
 msgstr "Grupa"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Tworzenie"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Usuwanie"
@@ -848,14 +854,18 @@
 msgid "Help"
 msgstr "Pomoc"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Przywróć"
@@ -916,31 +926,38 @@
 msgid "Values on File System"
 msgstr "Wartości w systemie plików"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Brak aktualizacji"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Niezsynchronizowany"
 
 msgctxt "field:ir.model.data,values:"
 msgid "Values"
 msgstr "Wartości"
 
-#, fuzzy
 msgctxt "field:ir.model.field,access:"
 msgid "Access"
 msgstr "Dostęp"
 
 msgctxt "field:ir.model.field,field_description:"
 msgid "Field Description"
 msgstr "Opis pola"
@@ -949,18 +966,26 @@
 msgid "Help"
 msgstr "Pomoc"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Relacja modelu"
@@ -973,18 +998,30 @@
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Pole"
 
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Pole"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grupa"
 
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Model"
+
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Utworzenie"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Usunięcie"
@@ -993,33 +1030,30 @@
 msgid "Read Access"
 msgstr "Odczyt"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Zapis"
 
-#, fuzzy
 msgctxt "field:ir.model.log,action:"
 msgid "Action"
 msgstr "Akcja"
 
 msgctxt "field:ir.model.log,event:"
 msgid "Event"
-msgstr ""
+msgstr "Zdarzenie"
 
-#, fuzzy
 msgctxt "field:ir.model.log,resource:"
 msgid "Resource"
 msgstr "Zasób"
 
 msgctxt "field:ir.model.log,target:"
 msgid "Target"
-msgstr ""
+msgstr "Cel"
 
-#, fuzzy
 msgctxt "field:ir.model.log,user:"
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtr"
@@ -1052,15 +1086,14 @@
 msgid "Version"
 msgstr "Wersja"
 
 msgctxt "field:ir.module.activate_upgrade.start,module_info:"
 msgid "Modules to update"
 msgstr "Moduły przeznaczone do aktualizacji"
 
-#, fuzzy
 msgctxt "field:ir.module.config.start,modules:"
 msgid "Modules"
 msgstr "Moduły"
 
 msgctxt "field:ir.module.config_wizard.item,action:"
 msgid "Action"
 msgstr "Akcja"
@@ -1169,14 +1202,18 @@
 msgid "Global"
 msgstr "Globalne"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Utworzenie"
@@ -1223,15 +1260,15 @@
 
 msgctxt "field:ir.sequence,prefix:"
 msgid "Prefix"
 msgstr "Prefiks"
 
 msgctxt "field:ir.sequence,preview:"
 msgid "Preview"
-msgstr ""
+msgstr "Podgląd"
 
 msgctxt "field:ir.sequence,sequence_type:"
 msgid "Sequence Type"
 msgstr "Typ sekwencji"
 
 msgctxt "field:ir.sequence,suffix:"
 msgid "Suffix"
@@ -1275,15 +1312,15 @@
 
 msgctxt "field:ir.sequence.strict,prefix:"
 msgid "Prefix"
 msgstr "Prefiks"
 
 msgctxt "field:ir.sequence.strict,preview:"
 msgid "Preview"
-msgstr ""
+msgstr "Podgląd"
 
 msgctxt "field:ir.sequence.strict,sequence_type:"
 msgid "Sequence Type"
 msgstr "Typy sekwencji"
 
 msgctxt "field:ir.sequence.strict,suffix:"
 msgid "Suffix"
@@ -1325,22 +1362,30 @@
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Nazwa pola"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Nadpisany moduł"
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Nadpisany moduł"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID zasobu"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Źródło"
@@ -1433,14 +1478,18 @@
 msgid "Icon"
 msgstr "Ikona"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Ścieżka SVG"
@@ -1485,38 +1534,58 @@
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Architektura widoku"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr "Podstawa"
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Dane"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domena"
 
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Rozszerzenia"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Pole elementów podrzędnych"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Pole elementów podrzędnych"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Widok odziedziczony"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Moduł"
 
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Moduł"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Priorytet"
@@ -1537,33 +1606,29 @@
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.ui.view_search,user:"
 msgid "User"
 msgstr "Użytkownik"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,field:"
 msgid "Field"
 msgstr "Pole"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,user:"
 msgid "User"
 msgstr "Użytkownik"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,value:"
 msgid "Value"
-msgstr "Wartości"
+msgstr "Wartość"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,view_id:"
 msgid "View ID"
-msgstr "Widok"
+msgstr "ID widoku"
 
 msgctxt "field:ir.ui.view_tree_state,child_name:"
 msgid "Child Name"
 msgstr "Nazwa elementu podrzędnego"
 
 msgctxt "field:ir.ui.view_tree_state,domain:"
 msgid "Domain"
@@ -1585,43 +1650,49 @@
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Pole"
 
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Pole"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Szerokość"
 
-#, fuzzy
 msgctxt "help:ir.action,records:"
 msgid "The records on which the action runs."
-msgstr "Zasoby, do których należy skopiować ten rekord."
+msgstr "Rekordy, na których działa akcja."
 
 msgctxt "help:ir.action.act_window,context_domain:"
 msgid "Part of the domain that will be evaluated on each refresh."
 msgstr "Część domeny, która będzie ewaluowana przy każdym odświeżeniu."
 
 msgctxt "help:ir.action.act_window,limit:"
 msgid "Default limit for the list view."
 msgstr "Domyślny limit dla widoku listy."
 
-#, fuzzy
 msgctxt "help:ir.action.act_window,records:"
 msgid "The records on which the action runs."
-msgstr "Zasoby, do których należy skopiować ten rekord."
+msgstr "Rekordy, na których działa akcja."
 
 msgctxt "help:ir.action.act_window,search_value:"
 msgid "Default search criteria for the list view."
 msgstr "Domyślne kryteria wyszukiwania dla widoku listy."
 
 msgctxt "help:ir.action.report,extension:"
 msgid ""
@@ -1632,37 +1703,36 @@
 " formatu."
 
 msgctxt "help:ir.action.report,record_name:"
 msgid ""
 "A Genshi expression to compute the name using 'record'.\n"
 "Leave empty for the default name."
 msgstr ""
+"Wyrażenie Genshi do ustalenia nazwy przy użyciu „rekordu”.\n"
+"Pozostaw puste dla nazwy domyślnej."
 
-#, fuzzy
 msgctxt "help:ir.action.report,records:"
 msgid "The records on which the action runs."
-msgstr "Zasoby, do których należy skopiować ten rekord."
+msgstr "Rekordy, na których działa akcja."
 
 msgctxt "help:ir.action.report,single:"
 msgid "Check if the template works only for one record."
 msgstr "Sprawdź, czy szablon pracuje tylko dla jednego rekordu."
 
 msgctxt "help:ir.action.report,translatable:"
 msgid "Uncheck to disable translations for this report."
 msgstr "Odznacz, aby wyłączyć tłumaczenie dla tego raportu."
 
-#, fuzzy
 msgctxt "help:ir.action.url,records:"
 msgid "The records on which the action runs."
-msgstr "Zasoby, do których należy skopiować ten rekord."
+msgstr "Rekordy, na których działa akcja."
 
-#, fuzzy
 msgctxt "help:ir.action.wizard,records:"
 msgid "The records on which the action runs."
-msgstr "Zasoby, do których należy skopiować ten rekord."
+msgstr "Rekordy, na których działa akcja."
 
 msgctxt "help:ir.action.wizard,window:"
 msgid "Run wizard in a new window."
 msgstr "Uruchom kreatora w nowym oknie."
 
 msgctxt "help:ir.email.template,recipients:"
 msgid "The field that contains the recipient(s)."
@@ -1698,30 +1768,29 @@
 "record represented by \"self\"."
 msgstr ""
 "Wyrażenie PYSON generujące listę dodatkowych odbiorców z rekordem "
 "reprezentowanym przez „self”."
 
 msgctxt "help:ir.export,header:"
 msgid "Check to include field names on the export."
-msgstr ""
+msgstr "Zaznacz, aby przy eksporcie uwzględnić nazwy pól."
 
-#, fuzzy
 msgctxt "help:ir.export,records:"
 msgid "The records on which the export runs."
-msgstr "Zasoby, do których należy skopiować ten rekord."
+msgstr "Rekordy, na których działa eksport."
 
 msgctxt "help:ir.lang,code:"
 msgid "RFC 4646 tag."
-msgstr ""
+msgstr "Znacznik RFC 4646."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Kod elementu nadrzędnego powodującego wyjątek"
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Moduł, w którym ten model jest zdefiniowany."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "Tekst umożliwiający użytkownikowi potwierdzenie po wciśnięciu przycisku."
@@ -1747,16 +1816,18 @@
 msgstr "Identyfikator rekordu znany w systemie plików."
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
+"Jeśli opcja jest zaznaczona, prawo dostępu do modelu pola jest również "
+"sprawdzane w odniesieniu do relacji pola."
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Moduł, w którym to pole jest zdefiniowane."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -1768,22 +1839,21 @@
 msgid "When the task should be done."
 msgstr "Kiedy zadanie powinno zostać ukończone."
 
 msgctxt "help:ir.queue,scheduled_at:"
 msgid "When the task can start."
 msgstr "Kiedy zadanie może zostać rozpoczęte."
 
-#, fuzzy
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "Domain is evaluated with a PYSON context containing:\n"
 "- \"groups\" as list of ids from the current user"
 msgstr ""
 "Domena jest ewaluowana przez kontekst PYSON zawierający:\n"
-"- \"user\" jako aktualny użytkownik"
+"- \"groups\" jako lista identyfikatorów bieżącego użytkownika"
 
 msgctxt "help:ir.rule.group,default_p:"
 msgid "Add this rule to all users by default."
 msgstr "Dodaj domyślnie tę regułę do wszystkich użytkowników."
 
 msgctxt "help:ir.rule.group,global_p:"
 msgid ""
@@ -1805,32 +1875,40 @@
 "Reguła spełnia wymagania jeśli wynik przynajmniej jednego testu jest True."
 
 msgctxt "help:ir.sequence,prefix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Bieżącą datę można sformatować w formacie strftime poprzedzając "
+"podkreśleniem: np.: ${date_Y}"
 
 msgctxt "help:ir.sequence,suffix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Bieżącą datę można sformatować w formacie strftime poprzedzając "
+"podkreśleniem: np.: ${date_Y}"
 
 msgctxt "help:ir.sequence.strict,prefix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Bieżącą datę można sformatować w formacie strftime poprzedzając "
+"podkreśleniem: np.: ${date_Y}"
 
 msgctxt "help:ir.sequence.strict,suffix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Bieżącą datę można sformatować w formacie strftime poprzedzając "
+"podkreśleniem: np.: ${date_Y}"
 
 msgctxt "help:ir.trigger,condition:"
 msgid ""
 "A PYSON statement evaluated with record represented by \"self\"\n"
 "It triggers the action if true."
 msgstr ""
 "Wyrażenie PYSON odnoszące się do rekordu reprezentowanego przez \"self\"\n"
@@ -1884,36 +1962,33 @@
 msgid "Attachments"
 msgstr "Załączniki"
 
 msgctxt "model:ir.action,name:act_config_wizard_item_form"
 msgid "Config Wizard Items"
 msgstr "Elementy kreatora konfiguracji"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_cron_form"
 msgid "Actions"
 msgstr "Akcje"
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "E-mails"
 msgstr "E-mail"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_email_form_relate"
 msgid "E-mail Archives"
-msgstr "Adres e-mail"
+msgstr "Archiwa wiadomości e-mail"
 
 msgctxt "model:ir.action,name:act_email_template_form"
 msgid "E-mail Templates"
 msgstr "Szablony e-maili"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_error_form"
 msgid "Errors"
-msgstr "Błąd"
+msgstr "Błędy"
 
 msgctxt "model:ir.action,name:act_export_form"
 msgid "Exports"
 msgstr "Wyeksportowania"
 
 msgctxt "model:ir.action,name:act_icon_form"
 msgid "Icons"
@@ -1931,18 +2006,17 @@
 msgid "Menu"
 msgstr "Menu"
 
 msgctxt "model:ir.action,name:act_menu_tree"
 msgid "Menu"
 msgstr "Menu"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_message_form"
 msgid "Messages"
-msgstr "Wiadomość"
+msgstr "Wiadomości"
 
 msgctxt "model:ir.action,name:act_model_access_form"
 msgid "Models Access"
 msgstr "Dostęp do modeli"
 
 msgctxt "model:ir.action,name:act_model_access_form_relate_model"
 msgid "Access"
@@ -1974,15 +2048,15 @@
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modele"
 
 msgctxt "model:ir.action,name:act_model_log_form"
 msgid "Logs"
-msgstr ""
+msgstr "Logi"
 
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Wykonaj aktywację/aktualizację"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
@@ -2008,18 +2082,17 @@
 msgid "Sequences"
 msgstr "Sekwencje"
 
 msgctxt "model:ir.action,name:act_sequence_strict_form"
 msgid "Sequences Strict"
 msgstr "Sekwencje ciągłe"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_sequence_type_form"
 msgid "Types"
-msgstr "Typ"
+msgstr "Typy"
 
 msgctxt "model:ir.action,name:act_translation_clean"
 msgid "Clean Translations"
 msgstr "Oczyść tłumaczenia"
 
 msgctxt "model:ir.action,name:act_translation_export"
 msgid "Export Translations"
@@ -2053,18 +2126,17 @@
 msgid "View Search"
 msgstr "Wyszukiwanie widoku"
 
 msgctxt "model:ir.action,name:act_view_show"
 msgid "Show View"
 msgstr "Pokaż widok"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_view_tree_optional_form"
 msgid "View Tree Optional"
-msgstr "Stan drzewa widoku"
+msgstr "Opcjonalny widok drzewa"
 
 msgctxt "model:ir.action,name:act_view_tree_state"
 msgid "Tree State"
 msgstr "Stan drzewa"
 
 msgctxt "model:ir.action,name:act_view_tree_width_form"
 msgid "View Tree Width"
@@ -2090,28 +2162,26 @@
 msgid "Action act window"
 msgstr "Okno działania akcji"
 
 msgctxt "model:ir.action.act_window.domain,name:"
 msgid "Action act window domain"
 msgstr "Domena okna działania akcji"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_error_form_domain_all"
 msgid "All"
 msgstr "Wszystko"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_error_form_domain_open"
 msgid "Open"
 msgstr "Otwórz"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_error_form_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "Przetwarzanie"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_model_data_form_domain_all"
 msgid "All"
 msgstr "Wszystko"
 
 msgctxt ""
@@ -2151,19 +2221,19 @@
 
 msgctxt "model:ir.attachment,name:"
 msgid "Attachment"
 msgstr "Załącznik"
 
 msgctxt "model:ir.avatar,name:"
 msgid "Avatar"
-msgstr ""
+msgstr "Awatar"
 
 msgctxt "model:ir.avatar.cache,name:"
 msgid "Avatar Cache"
-msgstr ""
+msgstr "Pamięć podręczna awatara"
 
 msgctxt "model:ir.cache,name:"
 msgid "Cache"
 msgstr "Pamięć podręczna"
 
 msgctxt "model:ir.calendar.day,abbreviation:Friday"
 msgid "Fri"
@@ -2349,15 +2419,14 @@
 msgid "Email Template"
 msgstr "Szablon e-maili"
 
 msgctxt "model:ir.email.template-ir.action.report,name:"
 msgid "Email Template - Report"
 msgstr "Szablon e-maili - Raport"
 
-#, fuzzy
 msgctxt "model:ir.error,name:"
 msgid "Error"
 msgstr "Błąd"
 
 msgctxt "model:ir.export,name:"
 msgid "Export"
 msgstr "Eksport"
@@ -2442,18 +2511,17 @@
 msgid "Polish"
 msgstr "Polski"
 
 msgctxt "model:ir.lang,name:lang_pt"
 msgid "Portuguese"
 msgstr "Portugalski"
 
-#, fuzzy
 msgctxt "model:ir.lang,name:lang_ro"
 msgid "Romanian"
-msgstr "Estoński"
+msgstr "Rumuński"
 
 msgctxt "model:ir.lang,name:lang_ru"
 msgid "Russian"
 msgstr "Rosyjski"
 
 msgctxt "model:ir.lang,name:lang_sl"
 msgid "Slovenian"
@@ -2461,21 +2529,20 @@
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turecki"
 
 msgctxt "model:ir.lang,name:lang_uk"
 msgid "Ukrainian"
-msgstr ""
+msgstr "Ukraiński"
 
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chiński uproszczony"
 
-#, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Skonfiguruj języki"
 
 msgctxt "model:ir.message,name:"
 msgid "Message"
 msgstr "Wiadomość"
@@ -2536,41 +2603,47 @@
 
 msgctxt "model:ir.message,text:msg_attachments"
 msgid "Attachments"
 msgstr "Załączniki"
 
 msgctxt "model:ir.message,text:msg_avatar"
 msgid "Avatar"
-msgstr ""
+msgstr "Awatar"
 
 msgctxt "model:ir.message,text:msg_avatar_resource_unique"
 msgid "Only one avatar is allowed per resource."
-msgstr ""
+msgstr "Na jeden zasób dozwolony jest tylko jeden awatar."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_avatar_size_unique"
 msgid "The size of an avatar must be unique."
-msgstr "Nazwa modelu musi być unikalna!"
+msgstr "Rozmiar awatara musi być unikatowy."
 
 msgctxt "model:ir.message,text:msg_avatar_url"
 msgid "Avatar URL"
-msgstr ""
+msgstr "URL awatara"
 
 msgctxt "model:ir.message,text:msg_avatars"
 msgid "Avatars"
-msgstr ""
+msgstr "Awatary"
 
 msgctxt "model:ir.message,text:msg_base_config_record"
 msgid "This record is part of the base configuration."
 msgstr "Ten rekord jest częścią podstawowej konfiguracji."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
-msgstr "Nazwa modelu musi być unikalna!"
+msgstr "Nazwa przycisku musi być unikalna dla każdego modelu."
+
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr "Data/czas: %(datetime)s"
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr "W grupach: %(groups)s"
 
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nie masz uprawnień do utworzenia rekordów w \"%(model)s\" z powodu niezgodności przynajmniej jednej z reguł:\n"
@@ -2588,25 +2661,21 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "Nie masz uprawnień do usunięcia rekordów \"%(ids)s\" z modelu \"%(model)s\" z powodu niezgodności przynajmniej jednej z reguł:\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
 msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
-msgstr ""
-"Nie masz uprawnień do uruchomienia kreatora \"%(wizard)s\" w modelu "
-"\"%(model)s\"."
+msgstr "Nie możesz usunąć rekordu \"%(record)s\" z \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
-msgstr "Lis"
+msgstr "Nie"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
 msgstr "Boolean"
 
 msgctxt "model:ir.message,text:msg_dict_schema_char"
 msgid "Char"
@@ -2632,41 +2701,39 @@
 msgid "Float"
 msgstr "Float"
 
 msgctxt "model:ir.message,text:msg_dict_schema_help"
 msgid "Help"
 msgstr "Pomoc"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_help_selection"
 msgid "Help Selection"
-msgstr "Zaznaczenie"
+msgstr "Wybór pomocy"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_help_selection_help"
 msgid "The key followed by the help text separated by a \":\", one per line."
-msgstr "Para klucza i etykiety rozdzielone w linii przez \":\"."
+msgstr ""
+"Klucz, po którym następuje tekst pomocy oddzielony znakiem \":\" po jednym w"
+" wierszu."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_help_selection_json"
 msgid "Help Selection JSON"
-msgstr "Zaznaczenie JSON"
+msgstr "Wybór pomocy JSON"
 
 msgctxt "model:ir.message,text:msg_dict_schema_integer"
 msgid "Integer"
 msgstr "Integer"
 
 msgctxt "model:ir.message,text:msg_dict_schema_invalid_domain"
 msgid "Invalid domain in schema \"%(schema)s\"."
 msgstr "Nieprawidłowa domena w schemacie \"%(schema)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_invalid_help_selection"
 msgid "Invalid help selection in schema \"%(schema)s\"."
-msgstr "Nieprawidłowe zaznaczenie w schemacie \"%(schema)s\"."
+msgstr "Nieprawidłowy wybór pomocy w schemacie \"%(schema)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_schema_invalid_selection"
 msgid "Invalid selection in schema \"%(schema)s\"."
 msgstr "Nieprawidłowe zaznaczenie w schemacie \"%(schema)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_schema_multiselection"
 msgid "MultiSelection"
@@ -2706,33 +2773,31 @@
 
 msgctxt "model:ir.message,text:msg_dict_schema_type"
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
-msgstr ""
+msgstr "Tak"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
 "record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
-"Liczba cyfr w wartości \"%(value)s\" w polu \"%(field)s\" modelu "
-"\"%(model)s\" przekroczyła limit \"%(digits)i\"."
+"Liczba cyfr wartości \"%(value)r\" dla pola \"%(field)s\" w rekordzie "
+"\"%(record)s\" z modelu \"%(model)s\" przekracza limit \"%(digits)i\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
-"Wartość w polu \"%(field)s\" dla \"%(model)s\" jest nieprawidłowa względem "
-"swojej domeny."
+"Wartość \"%(value)s\" dla pola \"%(field)s\" w rekordzie \"%(record)s\" w "
+"modelu \"%(model)s\" jest nieprawidłowa ze względu na swoją dziedzinę."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Data utworzenia"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
@@ -2766,28 +2831,27 @@
 "\"%(exception)s\"."
 msgstr ""
 "Nieprawidłowy temat w szablonie e-mail \"%(template)s\" generujący wyjątek "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_field_model_name"
 msgid "%(field)s (model name)"
-msgstr ""
+msgstr "%(field)s (nazwa modelu)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
-msgstr ""
+msgstr "%(field)s (łańcuch znakowy)"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
-"Niepoprawna wartość czasu \"%(value)s\" pola \"%(field)s\" w modelu "
-"\"%(model)s\"."
+"Wartość \"%(value)s\" w polu \"%(field)s\" w rekordzie \"%(record)s\" w "
+"modelu \"%(model)s\" zawiera nieprawidłowe znaki \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 "Rekordy nie mogą zostać usunięte ponieważ są używane w polu \"%(field)s\" "
@@ -2801,18 +2865,17 @@
 msgid "Failed to save, please retry."
 msgstr "Problem z zapisem, spróbuj ponownie."
 
 msgctxt "model:ir.message,text:msg_id_positive"
 msgid "ID must be positive."
 msgstr "ID musi być dodatnie."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_language_code_unique"
 msgid "The code on language must be unique."
-msgstr "Model musi być unikalny!"
+msgstr "Kod języka musi być unikalny."
 
 msgctxt "model:ir.message,text:msg_language_default_translatable"
 msgid "The default language \"%(language)s\" must be translatable."
 msgstr "Domyślny język \"%(language)s\" musi być przetłumaczalny."
 
 msgctxt "model:ir.message,text:msg_language_delete_default"
 msgid "The default language \"%(language)s\" can not be deleted."
@@ -2846,19 +2909,18 @@
 "activated."
 msgstr "Nie możesz usunąć modułu, który jest aktywny lub będzie aktywny."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notatki"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
 msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
-"Próbujesz odczytać rekordy \"%(ids)s\" modelu \"%(model)s\", które już nie "
+"Próbujesz odczytać rekordy \"%(ids)s\" z modelu \"%(model)s\", które nie "
 "istnieją."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
@@ -2874,91 +2936,88 @@
 "Recursion error: Record \"%(rec_name)s\" with parent \"%(parent_rec_name)s\""
 " was configured as ancestor of itself."
 msgstr ""
 "Błąd rekurencji: Rekord \"%(rec_name)s\" z elementem nadrzędnym "
 "\"%(parent_rec_name)s\" został skonfigurowany jako element nadrzędny siebie "
 "samego."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_reference_syntax_error"
 msgid ""
 "Syntax error for reference: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
-msgstr "Błąd składni dla referencji: \"%(value)r\" w \"%(field)s\"."
+msgstr ""
+"Błąd składniowy dla referencji: %(value)r w \"%(pole)s\" z modelu "
+"\"%(model)s\" (%(column)s)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_relation_not_found"
 msgid "Relation not found: %(value)r in \"%(model)s\" (%(column)s)."
-msgstr "Brak relacji: \"%(value)r\" w \"%(model)s\"."
+msgstr "Brak relacji: \"%(value)r\" w \"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_report_invalid_email"
 msgid "Invalid email definition for report \"%(name)s\"."
 msgstr "Nieprawidłowe określenie e-maila w raporcie \"%s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_report_invalid_record_name"
 msgid ""
 "Invalid record name definition for report \"%(report)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Nieprawidłowa treść w szablonie e-mail \"%(template)s\" generująca wyjątek "
-"\"%(exception)s\"."
+"Nieprawidłowa definicja nazwy rekordu dla raportu \"%(raport)s\" z wyjątkiem"
+" \"%(wyjątek)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
 msgid ""
 "A value is required for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\"."
-msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
+msgstr ""
+"W polu \"%(fields)s\" w rekordzie \"%(record)s\" w modelu \"%(model)s\" "
+"wymagana jest wartość."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Zasoby, do których należy skopiować ten rekord."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "Nieprawidłowa domena w regule \"%s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Brak funkcji wyszukiwania w polu \"%s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
-"Brak w elementach wyboru wartości \"%(value)s\" pola \"%(field)s\" dla "
-"modelu \"%(model)s\"."
+"Wartość \"%(value)s\" w polu \"%(field)s\" w rekordzie \"%(record)s\" w "
+"modelu \"%(model)s\" nie jest jedną z dozwolonych opcji."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Sekwencja"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
 "You cannot change the sequence type of a sequence instead create a new "
 "sequence."
 msgstr ""
 "Typ sekwencji nie może zostać zmieniony. Należy utworzyć nową sekwencję."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sequence_invalid_number_increment_next"
 msgid ""
 "Invalid \"Increment Number\" (%(number_increment)s) or \"Next Number\" "
 "(%(number_next)s) with exception \"%(exception)s\"."
 msgstr ""
-"Nieprawidłowa treść w szablonie e-mail \"%(template)s\" generująca wyjątek "
-"\"%(exception)s\"."
+"Nieprawidłowy \"Numer przyrostu\" (%(number_increment)s) lub \"Następny "
+"numer\" (%(number_next)s) z wyjątkiem \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_prefix"
 msgid "Invalid prefix \"%(affix)s\" for sequence \"%(sequence)s\"."
 msgstr "Niewłaściwy prefiks \"%(prefix)s\" w sekwencji \"%(sequence)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_suffix"
 msgid "Invalid suffix \"%(affix)s\" for sequence \"%(sequence)s\"."
@@ -2974,42 +3033,39 @@
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Brakująca funkcja setter dla pola \"%(field)s\" w \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_singleton"
 msgid "Only one singleton can be created."
-msgstr ""
+msgstr "Można utworzyć tylko jeden singleton."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
-"Wartość pola \"%(field)s\" w \"%(model)s\" jest zbyt długa (%(size)i > "
-"%(max_size)i)."
+"Wartość \"%(value)s\" w polu \"%(field)s\" w modelu \"%(model)s\" jest za "
+"długa (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"Wartość pola \"%(field)s\" w \"%(model)s\" jest zbyt długa (%(size)i > "
-"%(max_size)i)."
+"Wartość \"%(value)s\" w polu \"%(field)s\" w rekordzie \"%(record)s\" w "
+"modelu \"%(model)s\" jest za długa (%(size)i > %(max_size)i)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
 "The time value \"%(value)s\" for field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
-"Niepoprawna wartość czasu \"%(value)s\" pola \"%(field)s\" w modelu "
-"\"%(model)s\"."
+"Wartość czasu \"%(value)s\" w polu \"%(field)s\" w rekordzie \"%(record)s\" "
+"w modelu \"%(model)s\" jest nieprawidłowa."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
 msgid "Y"
@@ -3031,65 +3087,64 @@
 msgid "s"
 msgstr "s"
 
 msgctxt "model:ir.message,text:msg_timedelta_w"
 msgid "w"
 msgstr "t"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_too_many_relations_found"
 msgid "Too many relations found: %(value)r in \"%(model)s\" (%(column)s)."
-msgstr "Znaleziono zbyt wiele relacji: \"%(value)r\" w \"%(model)s\"."
+msgstr "Znaleziono zbyt wiele relacji: %(value)r w \"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_translation_overridden"
 msgid ""
 "You can not export translation \"%(name)s\" because it has been overridden "
 "by module \"%(overriding_module)s\"."
 msgstr ""
 "Nie możesz eksportować tłumaczenia %(name)s ponieważ jest ono nadpisane "
 "przez moduł %(overriding_module)s."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_trigger_exclusive"
 msgid ""
 "You can not select \"On Time\" and any other on the same time, they are "
 "mutually exclusive."
-msgstr "\"Na czas\" i pozostałe wzajemnie wykluczają się!"
+msgstr ""
+"Nie można wybrać opcji „Na czas” i żadnej innej w tym samym czasie, ponieważ"
+" wykluczają się one wzajemnie."
 
 msgctxt "model:ir.message,text:msg_trigger_invalid_condition"
 msgid ""
 "Condition \"%(condition)s\" is not a valid PYSON expression for trigger "
 "\"%(trigger)s\"."
 msgstr ""
 "Warunek \"%(condition)s\" nie jest poprawnym wyrażeniem PYSON dla wyzwalacza"
 " \"%(trigger)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_value_syntax_error"
 msgid ""
 "Syntax error for value: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
-msgstr "Błąd składni w XML id: \"%(value)r\" w \"%(field)s\"."
+msgstr ""
+"Błąd składni dla wartości: %(value)r w polu \"%(pole)s\" w modelu "
+"\"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_view_invalid_xml"
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr "Niewłaściwy XML dla widoku \"%s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
-"Nieprawidłowa domena lub kryteria wyszukiwania \"%(domain)s\" dla akcji "
-"\"%(action)s\"."
+"Nieprawidłowa domena lub kryteria wyszukiwania \"%(domain)s\" dla "
+"wyszukiwania \"%(search)s\"."
 
 msgctxt "model:ir.message,text:msg_view_tree_optional_type"
 msgid "You cannot store optional on view \"%(view)s\"."
-msgstr ""
+msgstr "Nie można zapisać opcjonalnej kolumny w widoku \"%(view)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
 "exist."
 msgstr ""
 "Próbujesz zapisać rekordy \"%(ids)s\" z modelu \"%(model)s\", które już nie "
 "istnieją."
@@ -3098,27 +3153,33 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nie masz uprawnień do zapisu rekordów \"%(ids)s\" modelu \"%(model)s\" z powodu przynajmniej jednego z reguł:\n"
 "%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
-msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
+msgstr ""
+"Nie możesz modyfikować pola \"%(field)s\" w rekordzie \"%(record)s\" w "
+"modelu \"%(model)s\"."
+
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr "ID XML"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
-msgstr "Błąd składni w XML id: \"%(value)r\" w \"%(field)s\"."
+msgstr ""
+"Błąd składni w XML id: %(value)r w \"%(field)s\" w modelu \"%(model)s\" "
+"(%(column)s)."
 
 msgctxt "model:ir.model,name:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "model:ir.model.access,name:"
 msgid "Model access"
@@ -3136,27 +3197,25 @@
 msgid "Model Button"
 msgstr "Przycisk modelu"
 
 msgctxt "model:ir.model.button,string:cron_run_once_button"
 msgid "Run Once"
 msgstr "Uruchom jednokrotnie"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:error_open_button"
 msgid "Open"
 msgstr "Otwórz"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:error_process_button"
 msgid "Process"
-msgstr "Dostęp"
+msgstr "Procesuj"
 
 msgctxt "model:ir.model.button,string:error_solve_button"
 msgid "Solve"
-msgstr ""
+msgstr "Rozwiąż"
 
 msgctxt "model:ir.model.button,string:lang_load_translations_button"
 msgid "Load translations"
 msgstr "Prześlij tłumaczenia"
 
 msgctxt "model:ir.model.button,string:lang_unload_translations_button"
 msgid "Unload translations"
@@ -3214,18 +3273,17 @@
 msgid "Model field"
 msgstr "Pole modelu"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Dostęp do pola modelu"
 
-#, fuzzy
 msgctxt "model:ir.model.log,name:"
 msgid "Log"
-msgstr "Laotański"
+msgstr "Log"
 
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Wykres modelu druku"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
@@ -3235,15 +3293,14 @@
 msgid "Module Activate Upgrade Done"
 msgstr "Uruchomiono aktywację/aktualizację modułu"
 
 msgctxt "model:ir.module.activate_upgrade.start,name:"
 msgid "Module Activate Upgrade Start"
 msgstr "Rozpoczęcie aktywacji/aktualizacji modułu"
 
-#, fuzzy
 msgctxt "model:ir.module.config.start,name:"
 msgid "Configure Modules"
 msgstr "Skonfiguruj moduły"
 
 msgctxt "model:ir.module.config_wizard.done,name:"
 msgid "Module Config Wizard Done"
 msgstr "Uruchomiono kreatora konfiguracji modułu"
@@ -3384,44 +3441,41 @@
 msgid "Attachments"
 msgstr "Załączniki"
 
 msgctxt "model:ir.ui.menu,name:menu_config_wizard_item_form"
 msgid "Config Wizard Items"
 msgstr "Elementy kreatora konfiguracji"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_cron_form"
 msgid "Actions"
 msgstr "Akcje"
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "E-mails"
 msgstr "E-mails"
 
 msgctxt "model:ir.ui.menu,name:menu_email_template_form"
 msgid "E-mail Templates"
 msgstr "Szablony e-maili"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_error_form"
 msgid "Errors"
-msgstr "Błąd"
+msgstr "Błędy"
 
 msgctxt "model:ir.ui.menu,name:menu_export_form"
 msgid "Exports"
 msgstr "Wyeksportowania"
 
 msgctxt "model:ir.ui.menu,name:menu_icon_form"
 msgid "Icons"
 msgstr "Ikony"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_ir_sequence_type"
 msgid "Types"
-msgstr "Typ"
+msgstr "Typy"
 
 msgctxt "model:ir.ui.menu,name:menu_lang_form"
 msgid "Languages"
 msgstr "Języki"
 
 msgctxt "model:ir.ui.menu,name:menu_localization"
 msgid "Localization"
@@ -3453,15 +3507,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modele"
 
 msgctxt "model:ir.ui.menu,name:menu_model_log_form"
 msgid "Logs"
-msgstr ""
+msgstr "Logi"
 
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modele"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
@@ -3531,18 +3585,17 @@
 msgid "Views"
 msgstr "Widoki"
 
 msgctxt "model:ir.ui.menu,name:menu_view_search"
 msgid "View Search"
 msgstr "Wyszukiwanie widoku"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_view_tree_optional"
 msgid "View Tree Optional"
-msgstr "Stan drzewa widoku"
+msgstr "Opcjonalny widok drzewa"
 
 msgctxt "model:ir.ui.menu,name:menu_view_tree_state"
 msgid "Tree State"
 msgstr "Stan drzewa"
 
 msgctxt "model:ir.ui.menu,name:menu_view_tree_width"
 msgid "View Tree Width"
@@ -3564,104 +3617,89 @@
 msgid "Show view"
 msgstr "Pokaż widok"
 
 msgctxt "model:ir.ui.view_search,name:"
 msgid "View Search"
 msgstr "Wyszukiwanie widoku"
 
-#, fuzzy
 msgctxt "model:ir.ui.view_tree_optional,name:"
 msgid "View Tree Optional"
-msgstr "Stan drzewa widoku"
+msgstr "Opcjonalny widok drzewa"
 
 msgctxt "model:ir.ui.view_tree_state,name:"
 msgid "View Tree State"
 msgstr "Stan drzewa widoku"
 
 msgctxt "model:ir.ui.view_tree_width,name:"
 msgid "View Tree Width"
 msgstr "Szerokość drzewa widoku"
 
-#, fuzzy
 msgctxt "selection:ir.action,action:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action,action:"
 msgid "URL"
-msgstr "Adresy URL"
+msgstr "Adres URL"
 
-#, fuzzy
 msgctxt "selection:ir.action,action:"
 msgid "Window"
 msgstr "Okno"
 
-#, fuzzy
 msgctxt "selection:ir.action,action:"
 msgid "Wizard"
-msgstr "Kreatory"
+msgstr "Kreator"
 
 msgctxt "selection:ir.action,records:"
 msgid "Listed"
-msgstr ""
+msgstr "Skatalogowany"
 
-#, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
-msgstr "Zaznaczone węzły"
+msgstr "Wybrany"
 
-#, fuzzy
 msgctxt "selection:ir.action,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action,type:"
 msgid "URL"
-msgstr "Adresy URL"
+msgstr "Adres URL"
 
-#, fuzzy
 msgctxt "selection:ir.action,type:"
 msgid "Window"
 msgstr "Okno"
 
-#, fuzzy
 msgctxt "selection:ir.action,type:"
 msgid "Wizard"
-msgstr "Kreatory"
+msgstr "Kreator"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
-msgstr ""
+msgstr "Skatalogowany"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
-msgstr "Zaznaczone węzły"
+msgstr "Wybrany"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "URL"
-msgstr "Adresy URL"
+msgstr "Adres URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "Window"
 msgstr "Okno"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "Wizard"
-msgstr "Kreatory"
+msgstr "Kreator"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Formularz akcji"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
@@ -3677,98 +3715,83 @@
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Print form"
 msgstr "Drukuj formularz"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Listed"
-msgstr ""
+msgstr "Skatalogowany"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
-msgstr "Zaznaczone węzły"
+msgstr "Wybrany"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "URL"
-msgstr "Adresy URL"
+msgstr "Adres URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "Window"
 msgstr "Okno"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "Wizard"
-msgstr "Kreatory"
+msgstr "Kreator"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
-msgstr ""
+msgstr "Skatalogowany"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
-msgstr "Zaznaczone węzły"
+msgstr "Wybrany"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "URL"
-msgstr "Adresy URL"
+msgstr "Adres URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "Window"
 msgstr "Okno"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "Wizard"
-msgstr "Kreatory"
+msgstr "Kreator"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
-msgstr ""
+msgstr "Skatalogowany"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
-msgstr "Zaznaczone węzły"
+msgstr "Wybrany"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "URL"
-msgstr "Adresy URL"
+msgstr "Adres URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "Window"
 msgstr "Okno"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "Wizard"
-msgstr "Kreatory"
+msgstr "Kreator"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Dane"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
@@ -3792,85 +3815,79 @@
 
 msgctxt "selection:ir.cron,interval_type:"
 msgid "Weeks"
 msgstr "Tygodnie"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Clean Errors"
-msgstr ""
+msgstr "Wyczyść błędy"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Clean Task Queue"
 msgstr "Wyczyść kolejkę zadań"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Run On Time Triggers"
 msgstr "Wyzwalacze uruchamiane o określonym czasie"
 
-#, fuzzy
 msgctxt "selection:ir.error,origin:"
 msgid "Action"
 msgstr "Akcja"
 
 msgctxt "selection:ir.error,origin:"
 msgid "Task"
-msgstr ""
+msgstr "Zadanie"
 
-#, fuzzy
 msgctxt "selection:ir.error,state:"
 msgid "Open"
 msgstr "Otwórz"
 
 msgctxt "selection:ir.error,state:"
 msgid "Processing"
-msgstr ""
+msgstr "Przetwarzanie"
 
 msgctxt "selection:ir.error,state:"
 msgid "Solved"
-msgstr ""
+msgstr "Rozwiązany"
 
 msgctxt "selection:ir.export,records:"
 msgid "Listed"
-msgstr ""
+msgstr "Skatalogowany"
 
-#, fuzzy
 msgctxt "selection:ir.export,records:"
 msgid "Selected"
-msgstr "Zaznaczone węzły"
+msgstr "Wybrany"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Left-to-right"
 msgstr "Od lewej do prawej"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Od prawej do lewej"
 
-#, fuzzy
 msgctxt "selection:ir.model.log,event:"
 msgid "Clicked on"
-msgstr "Kliknięcia"
+msgstr "Kliknięty"
 
-#, fuzzy
 msgctxt "selection:ir.model.log,event:"
 msgid "Deleted"
-msgstr "Przy usunięciu"
+msgstr "Usunięty"
 
 msgctxt "selection:ir.model.log,event:"
 msgid "Launched"
-msgstr ""
+msgstr "Uruchomiony"
 
 msgctxt "selection:ir.model.log,event:"
 msgid "Modified"
-msgstr ""
+msgstr "Zmodyfikowany"
 
-#, fuzzy
 msgctxt "selection:ir.model.log,event:"
 msgid "Transitioned to"
-msgstr "Tłumaczenie"
+msgstr "Przeniesiony do"
 
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Aktywny"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
@@ -4002,37 +4019,35 @@
 
 msgctxt "view:ir.action:"
 msgid "General"
 msgstr "Ogólne"
 
 msgctxt "view:ir.attachment:"
 msgid "Document"
-msgstr ""
+msgstr "Dokument"
 
 msgctxt "view:ir.attachment:"
 msgid "Last Modification Time"
 msgstr "Czas ostatniej modyfikacji"
 
 msgctxt "view:ir.cron:"
 msgid "At"
 msgstr "O"
 
 msgctxt "view:ir.cron:"
 msgid "Every"
 msgstr "Każdy"
 
-#, fuzzy
 msgctxt "view:ir.cron:"
 msgid "Next Call Date"
-msgstr "Kolejne wywołanie"
+msgstr "Data następnej rozmowy"
 
-#, fuzzy
 msgctxt "view:ir.cron:"
 msgid "Next Call Time"
-msgstr "Kolejne wywołanie"
+msgstr "Czas następnej rozmowy"
 
 msgctxt "view:ir.cron:"
 msgid "Run Once"
 msgstr "Uruchom jednorazowo"
 
 msgctxt "view:ir.email.template:"
 msgid "Hidden Recipients:"
@@ -4044,17 +4059,16 @@
 
 msgctxt "view:ir.email.template:"
 msgid "Secondary Recipients:"
 msgstr "Dodatkowi odbiorcy:"
 
 msgctxt "view:ir.error:"
 msgid "Origin"
-msgstr ""
+msgstr "Źródło"
 
-#, fuzzy
 msgctxt "view:ir.lang.config.start:"
 msgid "You can now load additional translations to the system."
 msgstr "Możesz przesłać teraz do systemu dodatkowe tłumaczenia."
 
 msgctxt "view:ir.lang:"
 msgid "Date Formatting"
 msgstr "Formatowanie daty"
@@ -4063,45 +4077,41 @@
 msgid "Monetary Formatting"
 msgstr "Formatowanie pieniężne"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Formatowanie liczb"
 
-#, fuzzy
 msgctxt "view:ir.model.log:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "view:ir.model.log:"
 msgid "Hour"
 msgstr "Godzina"
 
-#, fuzzy
 msgctxt "view:ir.model.log:"
 msgid "at"
-msgstr "Sob"
+msgstr "o"
 
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Moduły zostały zaktualizowane / aktywowane."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Wykonanie operacji może zająć kilka minut."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Your system will be upgraded."
 msgstr "System zostanie zaktualizowany."
 
-#, fuzzy
 msgctxt "view:ir.module.config.start:"
 msgid "You can now activate additional modules to the system."
-msgstr "Możesz przesłać teraz do systemu dodatkowe tłumaczenia."
+msgstr "Teraz możesz aktywować dodatkowe moduły do systemu."
 
 msgctxt "view:ir.module.config_wizard.done:"
 msgid "The configuration is done."
 msgstr "Konfiguracja została ukończona."
 
 msgctxt "view:ir.module.config_wizard.first:"
 msgid ""
@@ -4171,15 +4181,14 @@
 msgid "Synchronize Translations?"
 msgstr "Zsynchronizować tłumaczenia?"
 
 msgctxt "view:ir.translation.set.succeed:"
 msgid "Translations set successfully."
 msgstr "Tłumaczenia zostały pomyślnie zdefiniowane."
 
-#, fuzzy
 msgctxt "view:ir.ui.menu:"
 msgid "Actions"
 msgstr "Akcje"
 
 msgctxt "wizard_button:ir.lang.config,start,end:"
 msgid "Cancel"
 msgstr "Anuluj"
@@ -4192,33 +4201,30 @@
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgctxt "wizard_button:ir.model.print_model_graph,start,print_:"
 msgid "Print"
 msgstr "Wydruk"
 
-#, fuzzy
 msgctxt "wizard_button:ir.module.activate_upgrade,done,next_:"
 msgid "OK"
 msgstr "OK"
 
 msgctxt "wizard_button:ir.module.activate_upgrade,start,end:"
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgctxt "wizard_button:ir.module.activate_upgrade,start,upgrade:"
 msgid "Start Upgrade"
 msgstr "Rozpocznij aktualizację"
 
-#, fuzzy
 msgctxt "wizard_button:ir.module.config,start,activate:"
 msgid "Activate"
-msgstr "Aktywny"
+msgstr "Aktywuj"
 
-#, fuzzy
 msgctxt "wizard_button:ir.module.config,start,end:"
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgctxt "wizard_button:ir.module.config_wizard,done,end:"
 msgid "OK"
 msgstr "OK"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/pt.po` & `trytond-7.2.1/trytond/ir/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 msgid "Context Domain"
 msgstr "Contexto do Domínio"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Contexto do Modelo"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Contexto do Modelo"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Valor do domínio"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domínios"
@@ -105,14 +110,19 @@
 msgid "Records"
 msgstr "ID do registro"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Critérios de busca"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tipo"
@@ -190,18 +200,28 @@
 msgid "Keywords"
 msgstr "Palavras-chave"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Nome"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -301,14 +321,19 @@
 msgid "Keywords"
 msgstr "Palavras-chave"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Nome"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -814,14 +839,19 @@
 msgid "Model Name"
 msgstr "Nome do modelo"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Descrição do modelo"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Descrição"
@@ -830,14 +860,19 @@
 msgid "Group"
 msgstr "Grupo"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Acesso de criação"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Acesso de deleção"
@@ -862,14 +897,19 @@
 msgid "Help"
 msgstr "Ajuda"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Reiniciar"
@@ -930,18 +970,28 @@
 msgid "Values on File System"
 msgstr "Valores no Sistema de Arquivos"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Sem atualização"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Fora de Sincronia"
@@ -963,18 +1013,28 @@
 msgid "Help"
 msgstr "Ajuda"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Relação do modelo"
@@ -987,18 +1047,33 @@
 msgid "Description"
 msgstr "Descrição"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Campo"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Campo"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grupo"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Modelo"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Acesso de criação"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Acesso de deleção"
@@ -1184,14 +1259,19 @@
 msgid "Global"
 msgstr "Global"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Acesso de criação"
@@ -1342,22 +1422,32 @@
 msgid "Model"
 msgstr "Modelo"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Nome do campo"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Módulo sobreescrevente"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Módulo sobreescrevente"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID do Recurso"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Origem"
@@ -1454,14 +1544,19 @@
 msgid "Icon"
 msgstr "Ícone"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Caminho do SVG"
@@ -1506,38 +1601,62 @@
 msgid "User"
 msgstr "Usuário"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Arquitetura da visão"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Dados"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domínio"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Extensão"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Campos filhos"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Campos filhos"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Visão herdada"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Módulo"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Módulo"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioridade"
@@ -1606,18 +1725,28 @@
 msgid "User"
 msgstr "Usuário"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Campo"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Campo"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Modelo"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Usuário"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Largura"
@@ -1737,15 +1866,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Código de exceção do pai"
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Módulo no qual este modelo está definido"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "Texto de confirmação para exibir ao usuário quando clicar em um botão."
@@ -1774,15 +1903,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Módulo no qual este campo está definido"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2593,14 +2722,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Esse registro é parte da configuração base."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -3134,14 +3271,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "É necessário um valor para o campo \"%(field)s\" em \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "Erro de sintaxe para XML id: \"%(value)r\" em \"%(field)s\"."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/ro.po` & `trytond-7.2.1/trytond/ir/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 msgid "Context Domain"
 msgstr "Domeniu Context"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Model context"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Model context"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Valoare Domeniu"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domenii"
@@ -102,14 +107,19 @@
 msgid "Records"
 msgstr "Înregistrare"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Criteriu de cautare"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Tip"
@@ -186,18 +196,28 @@
 msgid "Keywords"
 msgstr "Cuvinte cheie"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Denumire Înregistrare"
@@ -294,14 +314,19 @@
 msgid "Keywords"
 msgstr "Cuvinte cheie"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Înregistrare"
@@ -779,14 +804,19 @@
 msgid "Model Name"
 msgstr "Numele modelului"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Descrierea modelului"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Descriere"
@@ -795,14 +825,19 @@
 msgid "Group"
 msgstr "Grup"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Creați acces"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Ștergeți accesul"
@@ -827,14 +862,19 @@
 msgid "Help"
 msgstr "Ajutor"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Resetare"
@@ -895,18 +935,28 @@
 msgid "Values on File System"
 msgstr "Valorile sistemului de fișiere"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Lipsă actualizare"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Nesincronizat"
@@ -927,18 +977,28 @@
 msgid "Help"
 msgstr "Ajutor"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Relația modelului"
@@ -951,18 +1011,33 @@
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Câmp"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Câmp"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grup"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Model"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Creați acces"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Ștergere Access"
@@ -1143,14 +1218,19 @@
 msgid "Global"
 msgstr "Global"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Creați acces"
@@ -1301,22 +1381,31 @@
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Denumire Câmpului"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID-ul resursei"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Sursă"
@@ -1409,14 +1498,19 @@
 msgid "Icon"
 msgstr "Pictogramă"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Calea SVG"
@@ -1461,38 +1555,62 @@
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Vizualizați Arhitectura"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Date"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domeniu"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Extensie"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Câmpul Copiilor"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Câmpul Copiilor"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Vedere moștenită"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioritate"
@@ -1557,18 +1675,28 @@
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Câmp"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Câmp"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Lăţime"
@@ -1684,15 +1812,16 @@
 msgid "RFC 4646 tag."
 msgstr "Eticheta RFC 4646."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Codul părintelui excepțional"
 
-msgctxt "help:ir.model,module:"
+#, fuzzy
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Modul în care este definit acest model."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 "Text pentru a solicita confirmarea utilizatorului atunci când faceți clic pe"
@@ -1724,15 +1853,16 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Dacă este bifat, dreptul de acces pe modelul câmpului este, de asemenea, "
 "testat față de relația câmpului."
 
-msgctxt "help:ir.model.field,module:"
+#, fuzzy
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Modulul în care este definit acest câmp."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2538,14 +2668,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Aceasta inregistrare face parte din configuratia de baza."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Numele butonului trebuie sa fie unic per model."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nu aveți permisiunea de a crea înregistrări pentru \"%(model)s\" deoarece nu respectă cel puțin una dintre aceste reguli:\n"
 "%(rules)s"
@@ -3076,14 +3214,18 @@
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "Nu aveți permisiunea de a face modificări câmpului \"%(field)s\" din "
 "\"%(record)s\" din \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/ru.po` & `trytond-7.2.1/trytond/ir/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Значение контекста"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Значение области выборки"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Домены"
@@ -105,14 +110,19 @@
 msgid "Records"
 msgstr "Идентификатор записи"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Критерии поиска"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Тип"
@@ -191,18 +201,28 @@
 msgid "Keywords"
 msgstr "Ключевые слова"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Наименование"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
@@ -303,14 +323,19 @@
 msgid "Keywords"
 msgstr "Ключевые слова"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Наименование"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
@@ -822,14 +847,19 @@
 msgid "Model Name"
 msgstr "Наименование модели"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Описание модели"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Описание"
@@ -838,14 +868,19 @@
 msgid "Group"
 msgstr "Группа"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Добавление"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Удаление"
@@ -872,14 +907,19 @@
 msgid "Help"
 msgstr "Помощь"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
@@ -947,18 +987,28 @@
 msgid "Values on File System"
 msgstr ""
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Нет обновлений"
 
 #, fuzzy
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
@@ -981,18 +1031,28 @@
 msgid "Help"
 msgstr "Помощь"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Связь модели"
@@ -1005,18 +1065,33 @@
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Поле"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Поле"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Группа"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Модель"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Добавление"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Удаление"
@@ -1210,14 +1285,19 @@
 msgid "Global"
 msgstr "Общий"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Добавление"
@@ -1368,22 +1448,31 @@
 msgid "Model"
 msgstr "Модель"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Название поля"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "Ресурс ID"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Исходный текст"
@@ -1480,14 +1569,19 @@
 msgid "Icon"
 msgstr "Иконка"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Путь к SVG"
@@ -1533,38 +1627,62 @@
 msgid "User"
 msgstr "Пользователь"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Арихитуктура вида"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Данные"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Домен"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Расширение"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Подчиненое поле"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Подчиненое поле"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Наследованный вид"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Приоритет"
@@ -1636,18 +1754,28 @@
 msgid "User"
 msgstr "Пользователь"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Поле"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Поле"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Пользователь"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Ширина"
@@ -1766,15 +1894,15 @@
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Модуль, в котором эта модель определена"
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1802,15 +1930,15 @@
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
 #, fuzzy
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Модуль, в котором это поле определяется"
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2678,14 +2806,22 @@
 msgstr "This record is part of the base configuration."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Наименование модуля должно быть уникальным"
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
@@ -3221,14 +3357,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/sl.po` & `trytond-7.2.1/trytond/ir/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 msgid "Context Domain"
 msgstr "Kontekstna domena"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Kontekstni model"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Kontekstni model"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Vrednost domene"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Domene"
@@ -102,14 +107,19 @@
 msgid "Records"
 msgstr "Zapisi"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Kriterij iskanja"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Vrsta"
@@ -186,18 +196,28 @@
 msgid "Keywords"
 msgstr "Ključne besede"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Naziv zapisa"
@@ -294,14 +314,19 @@
 msgid "Keywords"
 msgstr "Ključne besede"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Zapisi"
@@ -778,14 +803,19 @@
 msgid "Model Name"
 msgstr "Naziv modela"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Opis modela"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Opis"
@@ -794,14 +824,19 @@
 msgid "Group"
 msgstr "Skupina"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Izdelava"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Brisanje"
@@ -826,14 +861,19 @@
 msgid "Help"
 msgstr "Pomoč"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Ponastavitev"
@@ -894,18 +934,28 @@
 msgid "Values on File System"
 msgstr "Vrednosti v datotečnem sistemu"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Brez posodabljanja"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Izven sinhronizacije"
@@ -926,18 +976,28 @@
 msgid "Help"
 msgstr "Pomoč"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Vezni model"
@@ -950,18 +1010,33 @@
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Polje"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Polje"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Skupina"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Model"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Izdelava"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Brisanje"
@@ -1142,14 +1217,19 @@
 msgid "Global"
 msgstr "Globalno"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Izdelava"
@@ -1298,22 +1378,32 @@
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Naziv polja"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Razširjevalni modul"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Razširjevalni modul"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID vira"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Izvor"
@@ -1406,14 +1496,19 @@
 msgid "Icon"
 msgstr "Ikona"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "SVG pot"
@@ -1458,38 +1553,62 @@
 msgid "User"
 msgstr "Uporabnik"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Zgradba"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Podatki"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Domena"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Končnica"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Podpolja"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Podpolja"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Izpeljan iz"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modul"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modul"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Prioriteta"
@@ -1554,18 +1673,28 @@
 msgid "User"
 msgstr "Uporabnik"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Polje"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Polje"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Uporabnik"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Širina"
@@ -1672,15 +1801,16 @@
 msgid "RFC 4646 tag."
 msgstr "RFC 4646 značka."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+#, fuzzy
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Modul, v katerem je ta model določen."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1706,15 +1836,16 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+#, fuzzy
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Modul, v katerem je to polje določeno."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2499,14 +2630,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Ta zapis je del osnovne konfiguracije."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Naziv gumba mora biti edinstven na modelu."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nimate dovoljenja za ustvarjanja zapisov na modelu \"%(model)s\", saj ne ustreza vsaj enemu od pravil:\n"
 "%(rules)s"
@@ -2997,14 +3136,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "Nimate dovoljenja za brisanje zapisa \"%(record)s\" na modelu \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/tr.po` & `trytond-7.2.1/trytond/ir/locale/cs.po`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 msgid "Icon"
 msgstr "Icons"
 
 msgctxt "field:ir.action,keywords:"
 msgid "Keywords"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.action,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:ir.action,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action,type:"
@@ -55,14 +56,18 @@
 msgid "Context Domain"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr ""
 
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr ""
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr ""
@@ -76,17 +81,18 @@
 msgid "Keywords"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,limit:"
 msgid "Limit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.action.act_window,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.action.act_window,order:"
 msgid "Order Value"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,pyson_context:"
 msgid "PySON Context"
@@ -110,14 +116,19 @@
 msgstr "Record Rules"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr ""
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr ""
@@ -140,17 +151,18 @@
 msgid "Count"
 msgstr ""
 
 msgctxt "field:ir.action.act_window.domain,domain:"
 msgid "Domain"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.action.act_window.domain,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actions"
 
 #, fuzzy
@@ -205,21 +217,32 @@
 
 #, fuzzy
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Record Rules"
 
 #, fuzzy
@@ -281,17 +304,18 @@
 msgid "Icon"
 msgstr "Icons"
 
 msgctxt "field:ir.action.url,keywords:"
 msgid "Keywords"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.action.url,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:ir.action.url,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action.url,type:"
@@ -321,17 +345,23 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.action.wizard,type:"
@@ -365,15 +395,15 @@
 
 msgctxt "field:ir.attachment,data_size:"
 msgid "Data size"
 msgstr ""
 
 msgctxt "field:ir.attachment,description:"
 msgid "Description"
-msgstr "Tanım"
+msgstr ""
 
 msgctxt "field:ir.attachment,file_id:"
 msgid "File ID"
 msgstr ""
 
 msgctxt "field:ir.attachment,last_modification:"
 msgid "Last Modification"
@@ -383,17 +413,18 @@
 msgid "Last User"
 msgstr ""
 
 msgctxt "field:ir.attachment,link:"
 msgid "Link"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.attachment,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.attachment,resource:"
 msgid "Resource"
 msgstr ""
 
 msgctxt "field:ir.attachment,summary:"
 msgid "Summary"
@@ -451,17 +482,18 @@
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:ir.avatar.cache,size:"
 msgid "Size"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.cache,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.cache,timestamp:"
 msgid "Timestamp"
 msgstr ""
 
 msgctxt "field:ir.calendar.day,abbreviation:"
 msgid "Abbreviation"
@@ -470,28 +502,28 @@
 msgctxt "field:ir.calendar.day,index:"
 msgid "Index"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.calendar.day,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.calendar.month,abbreviation:"
 msgid "Abbreviation"
 msgstr ""
 
 msgctxt "field:ir.calendar.month,index:"
 msgid "Index"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.calendar.month,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.configuration,hostname:"
 msgid "Hostname"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.configuration,language:"
@@ -591,15 +623,15 @@
 msgctxt "field:ir.email.template,model_name:"
 msgid "Model Name"
 msgstr "Models Access"
 
 #, fuzzy
 msgctxt "field:ir.email.template,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.email.template,recipients:"
 msgid "Recipients"
 msgstr ""
 
 msgctxt "field:ir.email.template,recipients_hidden:"
 msgid "Hidden Recipients"
@@ -635,18 +667,17 @@
 msgid "Report"
 msgstr "Reports"
 
 msgctxt "field:ir.email.template-ir.action.report,template:"
 msgid "Template"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.error,description:"
 msgid "Description"
-msgstr "Tanım"
+msgstr ""
 
 msgctxt "field:ir.error,message:"
 msgid "Message"
 msgstr ""
 
 msgctxt "field:ir.error,origin:"
 msgid "Origin"
@@ -665,25 +696,27 @@
 msgid "State"
 msgstr "Tree State"
 
 msgctxt "field:ir.error,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.export,export_fields:"
 msgid "Fields"
-msgstr "Alanlar"
+msgstr "Fields"
 
 msgctxt "field:ir.export,header:"
 msgid "Header"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.export,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:ir.export,records:"
 msgid "Records"
 msgstr "Record Rules"
 
 msgctxt "field:ir.export,resource:"
@@ -695,17 +728,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.export.line,export:"
 msgid "Export"
 msgstr "Exports"
 
+#, fuzzy
 msgctxt "field:ir.export.line,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.lang,am:"
 msgid "AM"
 msgstr ""
 
 msgctxt "field:ir.lang,code:"
 msgid "Code"
@@ -748,17 +782,18 @@
 msgid "Negative Separate by Space"
 msgstr ""
 
 msgctxt "field:ir.lang,n_sign_posn:"
 msgid "Negative Sign Position"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.lang,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.lang,negative_sign:"
 msgid "Negative Sign"
 msgstr ""
 
 msgctxt "field:ir.lang,p_cs_precedes:"
 msgid "Positive Currency Symbol Precedes"
@@ -801,17 +836,18 @@
 msgid "Languages"
 msgstr "Languages"
 
 msgctxt "field:ir.message,text:"
 msgid "Text"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.model,fields:"
 msgid "Fields"
-msgstr "Alanlar"
+msgstr "Fields"
 
 msgctxt "field:ir.model,global_search_p:"
 msgid "Global Search"
 msgstr ""
 
 msgctxt "field:ir.model,info:"
 msgid "Information"
@@ -822,31 +858,41 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr ""
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
-msgstr "Tanım"
+msgstr ""
 
 msgctxt "field:ir.model.access,group:"
 msgid "Group"
-msgstr "Grup"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr ""
@@ -873,17 +919,23 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr ""
 
 msgctxt "field:ir.model.button,reset_by:"
 msgid "Reset by"
@@ -922,15 +974,15 @@
 
 msgctxt "field:ir.model.button.rule,condition:"
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:ir.model.button.rule,description:"
 msgid "Description"
-msgstr "Tanım"
+msgstr ""
 
 msgctxt "field:ir.model.button.rule,number_user:"
 msgid "Number of User"
 msgstr ""
 
 msgctxt "field:ir.model.data,db_id:"
 msgid "Resource ID"
@@ -946,18 +998,28 @@
 
 #, fuzzy
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
@@ -982,41 +1044,68 @@
 
 #, fuzzy
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr ""
 
 msgctxt "field:ir.model.field,ttype:"
 msgid "Field Type"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,description:"
 msgid "Description"
-msgstr "Tanım"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
-msgstr "Alan"
+msgstr "Fields"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Fields"
 
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
-msgstr "Grup"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Models"
 
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
@@ -1049,31 +1138,32 @@
 
 msgctxt "field:ir.model.log,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
-msgstr "Filtre"
+msgstr ""
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
-msgstr "Seviye"
+msgstr ""
 
 msgctxt "field:ir.module,childs:"
 msgid "Childs"
 msgstr ""
 
 msgctxt "field:ir.module,dependencies:"
 msgid "Dependencies"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.module,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.module,parents:"
 msgid "Parents"
 msgstr ""
 
 msgctxt "field:ir.module,state:"
 msgid "State"
@@ -1106,17 +1196,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.module.dependency,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
 msgctxt "field:ir.module.dependency,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.module.dependency,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:ir.note,copy_to_resources:"
 msgid "Copy to Resources"
@@ -1179,44 +1270,50 @@
 msgctxt "field:ir.queue,finished_at:"
 msgid "Finished at"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.queue,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.queue,scheduled_at:"
 msgid "Scheduled at"
 msgstr ""
 
 msgctxt "field:ir.rule,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:ir.rule,rule_group:"
 msgid "Group"
-msgstr "Grup"
+msgstr ""
 
 msgctxt "field:ir.rule.group,default_p:"
 msgid "Default"
 msgstr ""
 
 msgctxt "field:ir.rule.group,global_p:"
 msgid "Global"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr ""
 
 msgctxt "field:ir.rule.group,perm_delete:"
 msgid "Delete Access"
@@ -1371,22 +1468,31 @@
 msgstr "Models"
 
 #, fuzzy
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr ""
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr ""
 
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr ""
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr ""
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr ""
@@ -1450,17 +1556,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.trigger,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
 msgctxt "field:ir.trigger,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.trigger,on_create:"
 msgid "On Create"
 msgstr ""
 
 msgctxt "field:ir.trigger,on_delete:"
 msgid "On Delete"
@@ -1489,17 +1596,23 @@
 msgstr "Icons"
 
 #, fuzzy
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.menu,action:"
@@ -1545,44 +1658,68 @@
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr ""
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Export Translations"
+
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr ""
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr ""
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Models"
 
 #, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Modules"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Modules"
+
+#, fuzzy
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr ""
 
 msgctxt "field:ir.ui.view,type:"
 msgid "View Type"
@@ -1593,26 +1730,27 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view_search,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
 msgctxt "field:ir.ui.view_search,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "field:ir.ui.view_search,user:"
 msgid "User"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,field:"
 msgid "Field"
-msgstr "Alan"
+msgstr "Fields"
 
 msgctxt "field:ir.ui.view_tree_optional,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_optional,value:"
 msgid "Value"
@@ -1644,23 +1782,34 @@
 msgid "Selected Nodes"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_state,user:"
 msgid "User"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
-msgstr "Alan"
+msgstr "Fields"
+
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Fields"
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Models"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Models"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr ""
@@ -1763,15 +1912,15 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr ""
 
-msgctxt "help:ir.model,module:"
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr ""
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr ""
 
@@ -1795,15 +1944,15 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 
-msgctxt "help:ir.model.field,module:"
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr ""
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -1994,15 +2143,14 @@
 msgid "Fields Access"
 msgstr "Fields Access"
 
 msgctxt "model:ir.action,name:act_model_field_access_form_relate_field"
 msgid "Access"
 msgstr "Access"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_model_fields_form"
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
@@ -2507,18 +2655,17 @@
 msgid "Configure languages"
 msgstr "Configure Modules"
 
 msgctxt "model:ir.message,name:"
 msgid "Message"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_ID"
 msgid "ID"
-msgstr "ID"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_access_button_error"
 msgid "Calling button \"%(button)s on \"%(model)s\" is not allowed."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_access_rule_error"
 msgid "You are not allowed to access \"%(model)s\"."
@@ -2593,14 +2740,22 @@
 msgid "This record is part of the base configuration."
 msgstr "This record is part of the base configuration."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_created_at"
@@ -2695,15 +2850,15 @@
 msgctxt "model:ir.message,text:msg_dict_schema_multiselection"
 msgid "MultiSelection"
 msgstr "Scheduled Actions"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_name"
 msgid "Name"
-msgstr "Ad"
+msgstr "Namu"
 
 msgctxt "model:ir.message,text:msg_dict_schema_numeric"
 msgid "Numeric"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_selection"
@@ -3097,14 +3252,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 #, fuzzy
@@ -3550,15 +3709,14 @@
 msgid "Tree State"
 msgstr "Tree State"
 
 msgctxt "model:ir.ui.menu,name:menu_view_tree_width"
 msgid "View Tree Width"
 msgstr "View Tree Width"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:model_model_fields_form"
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.ui.menu.favorite,name:"
 msgid "Menu Favorite"
 msgstr ""
@@ -3944,17 +4102,18 @@
 msgid "Hexadecimal Timestamp"
 msgstr ""
 
 msgctxt "selection:ir.sequence.strict,type:"
 msgid "Incremental"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:ir.translation,type:"
 msgid "Field"
-msgstr "Alan"
+msgstr "Fields"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Help"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.translation,type:"
```

### Comparing `trytond-7.2.0/trytond/ir/locale/uk.po` & `trytond-7.2.1/trytond/ir/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 msgid "Context Domain"
 msgstr "Контекстний домен"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "Контекстна модель"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "Контекстна модель"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "Значення домену"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "Домени"
@@ -103,14 +108,19 @@
 msgid "Records"
 msgstr "Записи"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "Критерії пошуку"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "Тип"
@@ -188,18 +198,28 @@
 msgid "Keywords"
 msgstr "Ключові слова"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "Ім'я запису"
@@ -296,14 +316,19 @@
 msgid "Keywords"
 msgstr "Ключові слова"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "Записи"
@@ -783,14 +808,19 @@
 msgid "Model Name"
 msgstr "Ім'я моделі"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "Опис моделі"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "Опис"
@@ -799,14 +829,19 @@
 msgid "Group"
 msgstr "Група"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "Створення"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Видалення"
@@ -831,14 +866,19 @@
 msgid "Help"
 msgstr "Довідка"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "Скинути"
@@ -899,18 +939,28 @@
 msgid "Values on File System"
 msgstr "Значення у файловій системі"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "Немає оновлень"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "Не вдалося синхронізувати"
@@ -931,18 +981,28 @@
 msgid "Help"
 msgstr "Довідка"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "Зв'язок моделі"
@@ -955,18 +1015,33 @@
 msgid "Description"
 msgstr "Опис"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "Поле"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "Поле"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Група"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "Модель"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "Створення"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "Видалення"
@@ -1150,14 +1225,19 @@
 msgid "Global"
 msgstr "Глобальний"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "Створення"
@@ -1306,22 +1386,32 @@
 msgid "Model"
 msgstr "Модель"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "Ім'я поля"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "Перевизначаючий модуль"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "Перевизначаючий модуль"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "ID ресурсу"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "Джерело"
@@ -1414,14 +1504,19 @@
 msgid "Icon"
 msgstr "Піктограма"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "Шлях до SVG"
@@ -1466,38 +1561,62 @@
 msgid "User"
 msgstr "Користувач"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "Перегляд архітектури"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "Дані"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "Домен"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "Розширення"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "Діти"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "Діти"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "Успадкований перегляд"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "Модуль"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "Модуль"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "Пріоритет"
@@ -1562,18 +1681,28 @@
 msgid "User"
 msgstr "Користувач"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "Поле"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "Поле"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Модель"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "Користувач"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "Ширина"
@@ -1687,15 +1816,16 @@
 msgid "RFC 4646 tag."
 msgstr ""
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Код виняткового батька"
 
-msgctxt "help:ir.model,module:"
+#, fuzzy
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "Модуль, у якому визначено цю модель."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr "Текст для підтвердження користувача під час натискання кнопки."
 
@@ -1723,15 +1853,16 @@
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
 "Якщо позначено, доступ до моделі поля також перевіряється на записах, "
 "пов'язаних з цим полем."
 
-msgctxt "help:ir.model.field,module:"
+#, fuzzy
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "Модуль, у якому визначено це поле."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2517,14 +2648,22 @@
 msgid "This record is part of the base configuration."
 msgstr "Цей запис є частиною базової конфігурації."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "Назва кнопки має бути унікальною для кожної моделі."
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Вам заборонено створювати записи \"%(model)s\" через принаймні одне з цих правил:\n"
 "%(rules)s"
@@ -3048,14 +3187,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "Потрібно значення для поля \"%(field)s\" в \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Синтаксична помилка для XML id: %(value)r в полі \"%(field)s\" моделі "
 "\"%(model)s\" (%(column)s)."
```

### Comparing `trytond-7.2.0/trytond/ir/locale/zh_CN.po` & `trytond-7.2.1/trytond/ir/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 msgid "Context Domain"
 msgstr "上下文域"
 
 msgctxt "field:ir.action.act_window,context_model:"
 msgid "Context Model"
 msgstr "上下文模型"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,context_model_ref:"
+msgid "Context Model"
+msgstr "上下文模型"
+
 msgctxt "field:ir.action.act_window,domain:"
 msgid "Domain Value"
 msgstr "域取值"
 
 msgctxt "field:ir.action.act_window,domains:"
 msgid "Domains"
 msgstr "域"
@@ -102,14 +107,19 @@
 msgid "Records"
 msgstr "记录"
 
 msgctxt "field:ir.action.act_window,res_model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window,res_model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.action.act_window,search_value:"
 msgid "Search Criteria"
 msgstr "查找条件"
 
 msgctxt "field:ir.action.act_window,type:"
 msgid "Type"
 msgstr "类型"
@@ -186,18 +196,28 @@
 msgid "Keywords"
 msgstr "关键词"
 
 msgctxt "field:ir.action.report,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.action.report,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.action.report,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.action.report,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.action.report,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.action.report,record_name:"
 msgid "Record Name"
 msgstr "记录名称"
@@ -294,14 +314,19 @@
 msgid "Keywords"
 msgstr "关键词"
 
 msgctxt "field:ir.action.wizard,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.action.wizard,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.action.wizard,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.action.wizard,records:"
 msgid "Records"
 msgstr "记录"
@@ -778,14 +803,19 @@
 msgid "Model Name"
 msgstr "模型名称"
 
 msgctxt "field:ir.model,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.model,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.model,name:"
 msgid "Model Description"
 msgstr "模型描述"
 
 msgctxt "field:ir.model.access,description:"
 msgid "Description"
 msgstr "描述"
@@ -794,14 +824,19 @@
 msgid "Group"
 msgstr "用户组"
 
 msgctxt "field:ir.model.access,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.model.access,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.model.access,perm_create:"
 msgid "Create Access"
 msgstr "创建访问权限"
 
 msgctxt "field:ir.model.access,perm_delete:"
 msgid "Delete Access"
 msgstr "删除访问权限"
@@ -826,14 +861,19 @@
 msgid "Help"
 msgstr "帮助"
 
 msgctxt "field:ir.model.button,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.model.button,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.model.button,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.model.button,reset:"
 msgid "Reset"
 msgstr "重置"
@@ -894,18 +934,28 @@
 msgid "Values on File System"
 msgstr "文件系统里的取值"
 
 msgctxt "field:ir.model.data,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.model.data,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.model.data,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.model.data,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.model.data,noupdate:"
 msgid "No Update"
 msgstr "不更新"
 
 msgctxt "field:ir.model.data,out_of_sync:"
 msgid "Out of Sync"
 msgstr "未同步"
@@ -926,18 +976,28 @@
 msgid "Help"
 msgstr "帮助"
 
 msgctxt "field:ir.model.field,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.model.field,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.model.field,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.model.field,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.model.field,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.model.field,relation:"
 msgid "Model Relation"
 msgstr "模型关系"
@@ -950,18 +1010,33 @@
 msgid "Description"
 msgstr "描述"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
 msgstr "字段"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,field_ref:"
+msgid "Field"
+msgstr "字段"
+
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "用户组"
 
+#, fuzzy
+msgctxt "field:ir.model.field.access,model:"
+msgid "Model"
+msgstr "模型"
+
+#, fuzzy
+msgctxt "field:ir.model.field.access,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
 msgstr "新建访问权限"
 
 msgctxt "field:ir.model.field.access,perm_delete:"
 msgid "Delete Access"
 msgstr "删除访问权限"
@@ -1142,14 +1217,19 @@
 msgid "Global"
 msgstr "全局"
 
 msgctxt "field:ir.rule.group,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.rule.group,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.rule.group,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.rule.group,perm_create:"
 msgid "Create Access"
 msgstr "创建访问权限"
@@ -1298,22 +1378,32 @@
 msgid "Model"
 msgstr "模型"
 
 msgctxt "field:ir.translation,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.translation,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.translation,name:"
 msgid "Field Name"
 msgstr "字段名称"
 
 msgctxt "field:ir.translation,overriding_module:"
 msgid "Overriding Module"
 msgstr "覆盖模块"
 
+#, fuzzy
+msgctxt "field:ir.translation,overriding_module_ref:"
+msgid "Overriding Module"
+msgstr "覆盖模块"
+
 msgctxt "field:ir.translation,res_id:"
 msgid "Resource ID"
 msgstr "资源 ID"
 
 msgctxt "field:ir.translation,src:"
 msgid "Source"
 msgstr "源"
@@ -1406,14 +1496,19 @@
 msgid "Icon"
 msgstr "图标"
 
 msgctxt "field:ir.ui.icon,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.ui.icon,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.ui.icon,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.ui.icon,path:"
 msgid "SVG Path"
 msgstr "SVG 路径"
@@ -1458,38 +1553,62 @@
 msgid "User"
 msgstr "用户"
 
 msgctxt "field:ir.ui.view,arch:"
 msgid "View Architecture"
 msgstr "视图结构"
 
+msgctxt "field:ir.ui.view,basis:"
+msgid "Basis"
+msgstr ""
+
 msgctxt "field:ir.ui.view,data:"
 msgid "Data"
 msgstr "数据"
 
 msgctxt "field:ir.ui.view,domain:"
 msgid "Domain"
 msgstr "域"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,extensions:"
+msgid "Extensions"
+msgstr "扩展"
+
+#, fuzzy
+msgctxt "field:ir.ui.view,field_children:"
+msgid "Children Field"
+msgstr "子字段"
+
 msgctxt "field:ir.ui.view,field_childs:"
 msgid "Children Field"
 msgstr "子字段"
 
 msgctxt "field:ir.ui.view,inherit:"
 msgid "Inherited View"
 msgstr "继承的视图"
 
 msgctxt "field:ir.ui.view,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.ui.view,module:"
 msgid "Module"
 msgstr "模块"
 
+#, fuzzy
+msgctxt "field:ir.ui.view,module_ref:"
+msgid "Module"
+msgstr "模块"
+
 msgctxt "field:ir.ui.view,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.ui.view,priority:"
 msgid "Priority"
 msgstr "优先级"
@@ -1554,18 +1673,28 @@
 msgid "User"
 msgstr "用户"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
 msgstr "字段"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,field_ref:"
+msgid "Field"
+msgstr "字段"
+
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "模型"
 
+#, fuzzy
+msgctxt "field:ir.ui.view_tree_width,model_ref:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
 msgstr "用户"
 
 msgctxt "field:ir.ui.view_tree_width,width:"
 msgid "Width"
 msgstr "宽度"
@@ -1670,15 +1799,16 @@
 msgid "RFC 4646 tag."
 msgstr "RFC 4646 标签。"
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "特殊父级的代码"
 
-msgctxt "help:ir.model,module:"
+#, fuzzy
+msgctxt "help:ir.model,module_ref:"
 msgid "Module in which this model is defined."
 msgstr "定义该模型的模块."
 
 msgctxt "help:ir.model.button,confirm:"
 msgid "Text to ask user confirmation when clicking the button."
 msgstr "单击按钮时询问用户确认的文本."
 
@@ -1704,15 +1834,16 @@
 
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr "如果选中，系统会根据字段的关系测试对字段模型的访问权限。"
 
-msgctxt "help:ir.model.field,module:"
+#, fuzzy
+msgctxt "help:ir.model.field,module_ref:"
 msgid "Module in which this field is defined."
 msgstr "定义该字段的模块."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
 "Entering a Python Regular Expression will exclude matching models from the "
 "graph."
@@ -2495,14 +2626,22 @@
 msgid "This record is part of the base configuration."
 msgstr "该记录是基本配置的一部分。"
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
 msgstr "每个模型的按钮名称不能重复。"
 
+msgctxt "model:ir.message,text:msg_context_datetime"
+msgid "At date/time: %(datetime)s"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_context_groups"
+msgid "Within groups: %(groups)s"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "不允许创建\"%(model)s\"的记录，因为在以下规则中，至少有一条不满足：\n"
 "%(rules)s"
@@ -2980,14 +3119,18 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
 "You are not allowed to modify the field \"%(field)s\" in record "
 "\"%(record)s\" of \"%(model)s\"."
 msgstr "不允许修改 \"%(model)s\" 的 \"%(record)s\" 中的字段 \"%(field)s\"。"
 
+msgctxt "model:ir.message,text:msg_xml_id"
+msgid "XML ID"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "\"%(model)s\"（%(column)s 的 \"%(field)s\"）中的 XML %(value)r 的语法错误。"
 
 msgctxt "model:ir.model,name:"
```

### Comparing `trytond-7.2.0/trytond/ir/message.py` & `trytond-7.2.1/trytond/ir/message.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/message.xml` & `trytond-7.2.1/trytond/ir/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/model.py` & `trytond-7.2.1/trytond/ir/model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/model.xml` & `trytond-7.2.1/trytond/ir/model.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/module.py` & `trytond-7.2.1/trytond/ir/module.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/module.xml` & `trytond-7.2.1/trytond/ir/module.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/note.py` & `trytond-7.2.1/trytond/ir/note.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/note.xml` & `trytond-7.2.1/trytond/ir/note.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/queue_.py` & `trytond-7.2.1/trytond/ir/queue_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/resource.py` & `trytond-7.2.1/trytond/ir/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/routes.py` & `trytond-7.2.1/trytond/ir/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/rule.py` & `trytond-7.2.1/trytond/ir/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/rule.xml` & `trytond-7.2.1/trytond/ir/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/sequence.py` & `trytond-7.2.1/trytond/ir/sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/sequence.xml` & `trytond-7.2.1/trytond/ir/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/session.py` & `trytond-7.2.1/trytond/ir/session.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/translation.py` & `trytond-7.2.1/trytond/ir/translation.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/translation.xml` & `trytond-7.2.1/trytond/ir/translation.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/trigger.py` & `trytond-7.2.1/trytond/ir/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/trigger.xml` & `trytond-7.2.1/trytond/ir/trigger.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/board.rnc` & `trytond-7.2.1/trytond/ir/ui/board.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/board.rng` & `trytond-7.2.1/trytond/ir/ui/board.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/calendar.rnc` & `trytond-7.2.1/trytond/ir/ui/calendar.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/calendar.rng` & `trytond-7.2.1/trytond/ir/ui/calendar.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/form.rnc` & `trytond-7.2.1/trytond/ir/ui/form.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/form.rng` & `trytond-7.2.1/trytond/ir/ui/form.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/graph.rnc` & `trytond-7.2.1/trytond/ir/ui/graph.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/graph.rng` & `trytond-7.2.1/trytond/ir/ui/graph.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/icon.py` & `trytond-7.2.1/trytond/ir/ui/icon.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/icon.xml` & `trytond-7.2.1/trytond/ir/ui/icon.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/icons/LICENSE` & `trytond-7.2.1/trytond/ir/ui/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/icons/tryton-settings.svg` & `trytond-7.2.1/trytond/ir/ui/icons/tryton-settings.svg`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/menu.py` & `trytond-7.2.1/trytond/ir/ui/menu.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/menu.xml` & `trytond-7.2.1/trytond/ir/ui/menu.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/tree.rnc` & `trytond-7.2.1/trytond/ir/ui/tree.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/tree.rng` & `trytond-7.2.1/trytond/ir/ui/tree.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/ui.xml` & `trytond-7.2.1/trytond/ir/ui/ui.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/view.py` & `trytond-7.2.1/trytond/ir/ui/view.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/ui/view.xml` & `trytond-7.2.1/trytond/ir/ui/view.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/action_act_window_domain_form.xml` & `trytond-7.2.1/trytond/ir/view/action_act_window_domain_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/action_act_window_form.xml` & `trytond-7.2.1/trytond/ir/view/action_act_window_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/action_form.xml` & `trytond-7.2.1/trytond/ir/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/action_report_form.xml` & `trytond-7.2.1/trytond/ir/view/action_report_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/attachment_form.xml` & `trytond-7.2.1/trytond/ir/view/attachment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/attachment_list.xml` & `trytond-7.2.1/trytond/ir/view/attachment_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/cron_form.xml` & `trytond-7.2.1/trytond/ir/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/cron_list.xml` & `trytond-7.2.1/trytond/ir/view/cron_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/email_form.xml` & `trytond-7.2.1/trytond/ir/view/email_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/email_template_form.xml` & `trytond-7.2.1/trytond/ir/view/email_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/error_form.xml` & `trytond-7.2.1/trytond/ir/view/error_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/lang_form.xml` & `trytond-7.2.1/trytond/ir/view/lang_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_access_form.xml` & `trytond-7.2.1/trytond/ir/view/model_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_button_form.xml` & `trytond-7.2.1/trytond/ir/view/model_button_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_button_rule_form.xml` & `trytond-7.2.1/trytond/ir/view/model_button_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_data_form.xml` & `trytond-7.2.1/trytond/ir/view/model_data_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_field_access_form.xml` & `trytond-7.2.1/trytond/ir/view/model_field_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_field_form.xml` & `trytond-7.2.1/trytond/ir/view/model_field_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/model_form.xml` & `trytond-7.2.1/trytond/ir/view/model_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/module_activate_upgrade_start_form.xml` & `trytond-7.2.1/trytond/ir/view/module_activate_upgrade_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/module_form.xml` & `trytond-7.2.1/trytond/ir/view/module_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/module_list.xml` & `trytond-7.2.1/trytond/ir/view/module_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/note_form.xml` & `trytond-7.2.1/trytond/ir/view/note_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/note_list.xml` & `trytond-7.2.1/trytond/ir/view/note_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/rule_group_form.xml` & `trytond-7.2.1/trytond/ir/view/rule_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/sequence_form.xml` & `trytond-7.2.1/trytond/ir/view/sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/translation_form.xml` & `trytond-7.2.1/trytond/ir/view/translation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/translation_list.xml` & `trytond-7.2.1/trytond/ir/view/translation_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/trigger_form.xml` & `trytond-7.2.1/trytond/ir/view/trigger_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/ui_menu_form.xml` & `trytond-7.2.1/trytond/ir/view/ui_menu_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/ui_view_form.xml` & `trytond-7.2.1/trytond/ir/view/ui_view_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/ir/view/ui_view_tree_state_form.xml` & `trytond-7.2.1/trytond/ir/view/ui_view_tree_state_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/__init__.py` & `trytond-7.2.1/trytond/model/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/active.py` & `trytond-7.2.1/trytond/model/active.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/avatar.py` & `trytond-7.2.1/trytond/model/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/descriptors.py` & `trytond-7.2.1/trytond/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/dictschema.py` & `trytond-7.2.1/trytond/model/dictschema.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/digits.py` & `trytond-7.2.1/trytond/model/digits.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/exceptions.py` & `trytond-7.2.1/trytond/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/__init__.py` & `trytond-7.2.1/trytond/model/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/binary.py` & `trytond-7.2.1/trytond/model/fields/binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/boolean.py` & `trytond-7.2.1/trytond/model/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/char.py` & `trytond-7.2.1/trytond/model/fields/char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/date.py` & `trytond-7.2.1/trytond/model/fields/date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/dict.py` & `trytond-7.2.1/trytond/model/fields/dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/field.py` & `trytond-7.2.1/trytond/model/fields/field.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/float.py` & `trytond-7.2.1/trytond/model/fields/float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/fmany2one.py` & `trytond-7.2.1/trytond/model/fields/fmany2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/function.py` & `trytond-7.2.1/trytond/model/fields/function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/many2many.py` & `trytond-7.2.1/trytond/model/fields/many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/many2one.py` & `trytond-7.2.1/trytond/model/fields/many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/multiselection.py` & `trytond-7.2.1/trytond/model/fields/multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/numeric.py` & `trytond-7.2.1/trytond/model/fields/numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/one2many.py` & `trytond-7.2.1/trytond/model/fields/one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/one2one.py` & `trytond-7.2.1/trytond/model/fields/one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/reference.py` & `trytond-7.2.1/trytond/model/fields/reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/selection.py` & `trytond-7.2.1/trytond/model/fields/selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/fields/text.py` & `trytond-7.2.1/trytond/model/fields/text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/match.py` & `trytond-7.2.1/trytond/model/match.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/model.py` & `trytond-7.2.1/trytond/model/model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/modelsingleton.py` & `trytond-7.2.1/trytond/model/modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/modelsql.py` & `trytond-7.2.1/trytond/model/modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/modelstorage.py` & `trytond-7.2.1/trytond/model/modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/modelview.py` & `trytond-7.2.1/trytond/model/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/multivalue.py` & `trytond-7.2.1/trytond/model/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/order.py` & `trytond-7.2.1/trytond/model/order.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/symbol.py` & `trytond-7.2.1/trytond/model/symbol.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/tree.py` & `trytond-7.2.1/trytond/model/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/union.py` & `trytond-7.2.1/trytond/model/union.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/model/workflow.py` & `trytond-7.2.1/trytond/model/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/modules/__init__.py` & `trytond-7.2.1/trytond/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/pool.py` & `trytond-7.2.1/trytond/pool.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/protocols/dispatcher.py` & `trytond-7.2.1/trytond/protocols/dispatcher.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/protocols/jsonrpc.py` & `trytond-7.2.1/trytond/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/protocols/wrappers.py` & `trytond-7.2.1/trytond/protocols/wrappers.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/protocols/xmlrpc.py` & `trytond-7.2.1/trytond/protocols/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/pyson.py` & `trytond-7.2.1/trytond/pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/report/report.py` & `trytond-7.2.1/trytond/report/report.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/__init__.py` & `trytond-7.2.1/trytond/res/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/email_reset_password.html` & `trytond-7.2.1/trytond/res/email_reset_password.html`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/group.py` & `trytond-7.2.1/trytond/res/group.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/group.xml` & `trytond-7.2.1/trytond/res/group.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/ir.py` & `trytond-7.2.1/trytond/res/ir.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/ir.xml` & `trytond-7.2.1/trytond/res/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/bg.po` & `trytond-7.2.1/trytond/res/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/ca.po` & `trytond-7.2.1/trytond/res/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -483,33 +483,34 @@
 msgid "Login Attempt"
 msgstr "Intent d'inici de sessió"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Alerta usuari"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
 "Hello,\n"
 "                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
 "                You can connect with this temporary password [3:%(password)s] to[4:]\n"
 "                [5:tryton://%(host)s/%(database)s][6:]\n"
 "                [7:%(http_host)s/#%(database)s][8:]\n"
 "                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "La contrasenya del teu compte, [1:%(login)s], s'ha resetablert.[2:]\n"
 "                Heu d'establir una nova contraseña des de les preferències del usuari.[3:]\n"
 "                Podeu conectar amb aquesta contraseña temporal [4:%(password)s] a [5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(host)s/#%(database)s]"
+"                [8:%(http_host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
+"Si no heu fet aquesta sol·licitud, podeu ignorar aquest correu electrònic "
+"amb seguretat."
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Restableix la contrasenya"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
```

### Comparing `trytond-7.2.0/trytond/res/locale/cs.po` & `trytond-7.2.1/trytond/res/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/de.po` & `trytond-7.2.1/trytond/res/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -484,33 +484,35 @@
 msgid "Login Attempt"
 msgstr "Login Versuch"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Benutzer Warnung"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
 "Hello,\n"
 "                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
 "                You can connect with this temporary password [3:%(password)s] to[4:]\n"
 "                [5:tryton://%(host)s/%(database)s][6:]\n"
 "                [7:%(http_host)s/#%(database)s][8:]\n"
 "                You must set a new one from the user's preferences.[9:]"
 msgstr ""
-"Das Passwort für Ihr Konto, [1:%(login)s], wurde zurückgesetzt.[2:]\n"
-"                Sie müssen ein neues über die Benutzereinstellungen vergeben.[3:]\n"
-"                Sie können sich mit diesem temporären Passwort [4:%(password)s] verbinden mit[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hallo,\n"
+"                wir haben eine Anfrage zum Zurücksetzen des Passworts für den Benutzer [1:%(login)s] erhalten. Bisher wurden noch keine Änderungen an ihrem Benutzerkonto vorgenommen.[2:]\n"
+"                Sie können sich mit dem temporären Passwort [3:%(password)s] verbinden mit[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                Sie müssen anschließend in den Benutzereinstellungen ein neues Passwort vergeben.[9:]"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
+"Sollten Sie keine Zurücksetzung des Passworts beantragt haben, ignorieren "
+"Sie bitte diese E-Mail."
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Passwort zurücksetzen"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
```

### Comparing `trytond-7.2.0/trytond/res/locale/es.po` & `trytond-7.2.1/trytond/res/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -484,33 +484,34 @@
 msgid "Login Attempt"
 msgstr "Intento de inicio de sesión"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Aviso usuario"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
 "Hello,\n"
 "                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
 "                You can connect with this temporary password [3:%(password)s] to[4:]\n"
 "                [5:tryton://%(host)s/%(database)s][6:]\n"
 "                [7:%(http_host)s/#%(database)s][8:]\n"
 "                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "La contraseña para su cuenta, [1:%(login)s], se ha reseteado.[2:]\n"
 "                Debe establecer una nueva desde las preferencias de usuario.[3:]\n"
 "                Puede conectar con esta contraseña temporal [4:%(password)s] a [5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(host)s/#%(database)s]"
+"                [8:%(http_host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
+"Si no has realizado esta petición, puedes ignorar este correo "
+"tranquilamente."
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Restablecer contraseña"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
```

### Comparing `trytond-7.2.0/trytond/res/locale/es_419.po` & `trytond-7.2.1/trytond/res/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/et.po` & `trytond-7.2.1/trytond/res/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/fa.po` & `trytond-7.2.1/trytond/res/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/fi.po` & `trytond-7.2.1/trytond/res/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/fr.po` & `trytond-7.2.1/trytond/res/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/hu.po` & `trytond-7.2.1/trytond/res/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/id.po` & `trytond-7.2.1/trytond/res/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/it.po` & `trytond-7.2.1/trytond/res/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/lo.po` & `trytond-7.2.1/trytond/res/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/lt.po` & `trytond-7.2.1/trytond/res/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/nl.po` & `trytond-7.2.1/trytond/res/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -485,33 +485,33 @@
 msgid "Login Attempt"
 msgstr "Inlogpoging"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Gebruikerswaarschuwing"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
 "Hello,\n"
 "                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
 "                You can connect with this temporary password [3:%(password)s] to[4:]\n"
 "                [5:tryton://%(host)s/%(database)s][6:]\n"
 "                [7:%(http_host)s/#%(database)s][8:]\n"
 "                You must set a new one from the user's preferences.[9:]"
 msgstr ""
-"Het wachtwoord voor uw account, [1:%(login)s], is opnieuw ingesteld.[2:]\n"
-"                U moet er een nieuw aanmaken in de gebruikers voorkeuren[3:]\n"
-"               U kunt verbinding maken met dit tijdelijke wachtwoord [4:%(password)s] op[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(host)s/#%(database)s]"
+"Hallo,\n"
+"                We hebben het verzoek ontvangen om het wachtwoord voor de gebruiker geassocieerd met [1:%(login)s] opnieuw in te stellen. Op dit moment zijn er nog geen wijzigingen gedaan aan de gebruiker.[2:]\n"
+"                U kunt met het tijdelijke wachtwoord [3:%(password)s] connectie maken met[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                U moet een nieuwe wachtwoord instellen via de gebruikers voorkeuren.[9:]"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "If you didn't make this request, you can safely ignore this email."
-msgstr ""
+msgstr "Als u zit verzoek niet hebt gedaan, kunt u deze email negeren."
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Reset wachtwoord"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
```

### Comparing `trytond-7.2.0/trytond/res/locale/pl.po` & `trytond-7.2.1/trytond/res/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 msgid "Export"
 msgstr "Eksportuj"
 
 msgctxt "field:ir.export-write-res.group,group:"
 msgid "Group"
 msgstr "Grupa"
 
-#, fuzzy
 msgctxt "field:ir.model.button,groups:"
 msgid "Groups"
 msgstr "Grupy"
 
 msgctxt "field:ir.model.button-res.group,button:"
 msgid "Button"
 msgstr "Przycisk"
@@ -75,15 +74,14 @@
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:ir.model.button.rule,group:"
 msgid "Group"
 msgstr "Grupa"
 
-#, fuzzy
 msgctxt "field:ir.rule.group,groups:"
 msgid "Groups"
 msgstr "Grupy"
 
 msgctxt "field:ir.rule.group-res.group,group:"
 msgid "Group"
 msgstr "Grupa"
@@ -100,15 +98,14 @@
 msgid "User Groups"
 msgstr "Grupy użytkownika"
 
 msgctxt "field:ir.sequence.type-res.group,sequence_type:"
 msgid "Sequence Type"
 msgstr "Typ sekwencji"
 
-#, fuzzy
 msgctxt "field:ir.ui.menu,groups:"
 msgid "Groups"
 msgstr "Grupy"
 
 msgctxt "field:ir.ui.menu-res.group,group:"
 msgid "Group"
 msgstr "Grupa"
@@ -135,15 +132,15 @@
 
 msgctxt "field:res.group,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:res.group,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "Grupa nadrzędna"
 
 msgctxt "field:res.group,rule_groups:"
 msgid "Rules"
 msgstr "Reguły"
 
 msgctxt "field:res.group,users:"
 msgid "Users"
@@ -155,15 +152,15 @@
 
 msgctxt "field:res.user,applications:"
 msgid "Applications"
 msgstr "Aplikacje"
 
 msgctxt "field:res.user,avatar_badge_url:"
 msgid "Avatar Badge URL"
-msgstr ""
+msgstr "Avatar Badge URL"
 
 msgctxt "field:res.user,email:"
 msgid "Email"
 msgstr "E-mail"
 
 msgctxt "field:res.user,groups:"
 msgid "Groups"
@@ -255,24 +252,23 @@
 
 msgctxt "field:res.user.application,user:"
 msgid "User"
 msgstr "Użytkownik"
 
 msgctxt "field:res.user.device,cookie:"
 msgid "Cookie"
-msgstr ""
+msgstr "Ciasteczko"
 
-#, fuzzy
 msgctxt "field:res.user.device,login:"
 msgid "Login"
 msgstr "Login"
 
 msgctxt "field:res.user.login.attempt,device_cookie:"
 msgid "Device Cookie"
-msgstr ""
+msgstr "Ciasteczko urządzenia"
 
 msgctxt "field:res.user.login.attempt,ip_address:"
 msgid "IP Address"
 msgstr "Adres IP"
 
 msgctxt "field:res.user.login.attempt,ip_network:"
 msgid "IP Network"
@@ -304,15 +300,15 @@
 
 msgctxt "help:ir.sequence.type,groups:"
 msgid "Groups allowed to edit the sequences of this type."
 msgstr "Grupy uprawnione do edycji tego typu sekwencji."
 
 msgctxt "help:res.group,parent:"
 msgid "The group to inherit accesses from."
-msgstr ""
+msgstr "Grupa, z której mają być dziedziczone dostępy."
 
 msgctxt "help:res.user,actions:"
 msgid "Actions that will be run at login."
 msgstr "Akcje, które zostaną wykonane podczas logowania."
 
 msgctxt "model:ir.action,name:act_group_form"
 msgid "Groups"
@@ -340,27 +336,27 @@
 
 msgctxt "model:ir.export-write-res.group,name:"
 msgid "Export Modification Group"
 msgstr "Grupa zezwalająca na modyfikowanie eksportu"
 
 msgctxt "model:ir.message,text:msg_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
-msgstr ""
+msgstr "Adres e-mail \"%(email)s\" użytkownika \"%(user)s\" jest niepoprawny."
 
 msgctxt "model:ir.message,text:msg_password_email"
 msgid "The password cannot be the same as user's email address."
 msgstr "Hasło nie może być takie samo jak adres e-mail użytkownika."
 
 msgctxt "model:ir.message,text:msg_password_forbidden"
 msgid "The password is forbidden."
 msgstr "Takie hasło jest niedozwolone."
 
 msgctxt "model:ir.message,text:msg_password_length"
 msgid "The password must have at least %(length)i characters."
-msgstr ""
+msgstr "Hasło musi zawierać przynajmniej %(length)i znaków."
 
 msgctxt "model:ir.message,text:msg_password_login"
 msgid "The password cannot be the same as user's login."
 msgstr "Hasło nie może być takie samo jak login użytkownika."
 
 msgctxt "model:ir.message,text:msg_password_name"
 msgid "The password cannot be the same as user's name."
@@ -476,52 +472,51 @@
 
 msgctxt "model:res.user.config.start,name:"
 msgid "User Config Init"
 msgstr "Wstępne ustawienia użytkownika"
 
 msgctxt "model:res.user.device,name:"
 msgid "User Device"
-msgstr ""
+msgstr "Urządzenie użytkownika"
 
 msgctxt "model:res.user.login.attempt,name:"
 msgid "Login Attempt"
 msgstr "Próba logowania"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Ostrzeżenie użytkownika"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
 "Hello,\n"
 "                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
 "                You can connect with this temporary password [3:%(password)s] to[4:]\n"
 "                [5:tryton://%(host)s/%(database)s][6:]\n"
 "                [7:%(http_host)s/#%(database)s][8:]\n"
 "                You must set a new one from the user's preferences.[9:]"
 msgstr ""
-"Hasło do twojego konta, [1:%(login)s], zostało zresetowane.[2:]\n"
-"                Musisz ustawić nowe hasło w preferencjach użytkownika.[3:]\n"
-"                Możesz połączyć się używając tymczasowego hasła [4:%(password)s] do [5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(host)s/#%(database)s]"
+"Witaj,\n"
+"                otrzymaliśmy prośbę o zresetowanie hasła do konta powiązanego z [1:%(login)s]. Na Twoim koncie nie wprowadzono jeszcze żadnych zmian.[2:]\n"
+"                Możesz połączyć się za pomocą tymczasowego hasła [3:%(password)s] z [4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                Musisz ustawić nowe hasło w preferencjach użytkownika.[9:]"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "If you didn't make this request, you can safely ignore this email."
-msgstr ""
+msgstr "Jeśli nie Ty wysłałeś to żądanie, możesz zignorować tę wiadomość."
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Zresetuj hasło"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
-msgstr "Hasło wygaśnie o [1:%(datetime)s UTC]."
+msgstr "Hasło wygaśnie za [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Anulowano"
 
 msgctxt "selection:res.user.application,state:"
 msgid "Requested"
```

### Comparing `trytond-7.2.0/trytond/res/locale/pt.po` & `trytond-7.2.1/trytond/res/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/ro.po` & `trytond-7.2.1/trytond/res/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/ru.po` & `trytond-7.2.1/trytond/res/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/sl.po` & `trytond-7.2.1/trytond/res/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/tr.po` & `trytond-7.2.1/trytond/res/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/uk.po` & `trytond-7.2.1/trytond/res/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/locale/zh_CN.po` & `trytond-7.2.1/trytond/res/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/message.xml` & `trytond-7.2.1/trytond/res/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/routes.py` & `trytond-7.2.1/trytond/res/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/user.py` & `trytond-7.2.1/trytond/res/user.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/user.xml` & `trytond-7.2.1/trytond/res/user.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/view/group_form.xml` & `trytond-7.2.1/trytond/res/view/group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/view/user_application_form.xml` & `trytond-7.2.1/trytond/res/view/user_application_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/view/user_config_start_form.xml` & `trytond-7.2.1/trytond/res/view/user_config_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/view/user_form.xml` & `trytond-7.2.1/trytond/res/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/res/view/user_form_preferences.xml` & `trytond-7.2.1/trytond/res/view/user_form_preferences.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/rpc.py` & `trytond-7.2.1/trytond/rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/security.py` & `trytond-7.2.1/trytond/security.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/sendmail.py` & `trytond-7.2.1/trytond/sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/status.py` & `trytond-7.2.1/trytond/status.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/__init__.py` & `trytond-7.2.1/trytond/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/access.py` & `trytond-7.2.1/trytond/tests/access.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/copy_.py` & `trytond-7.2.1/trytond/tests/copy_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/export_data.py` & `trytond-7.2.1/trytond/tests/export_data.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_binary.py` & `trytond-7.2.1/trytond/tests/field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_boolean.py` & `trytond-7.2.1/trytond/tests/field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_char.py` & `trytond-7.2.1/trytond/tests/field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_context.py` & `trytond-7.2.1/trytond/tests/field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_date.py` & `trytond-7.2.1/trytond/tests/field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_datetime.py` & `trytond-7.2.1/trytond/tests/field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_dict.py` & `trytond-7.2.1/trytond/tests/field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_float.py` & `trytond-7.2.1/trytond/tests/field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_function.py` & `trytond-7.2.1/trytond/tests/field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_integer.py` & `trytond-7.2.1/trytond/tests/field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_many2many.py` & `trytond-7.2.1/trytond/tests/field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_many2one.py` & `trytond-7.2.1/trytond/tests/field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_multiselection.py` & `trytond-7.2.1/trytond/tests/field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_numeric.py` & `trytond-7.2.1/trytond/tests/field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_one2many.py` & `trytond-7.2.1/trytond/tests/field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_one2one.py` & `trytond-7.2.1/trytond/tests/field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_reference.py` & `trytond-7.2.1/trytond/tests/field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_selection.py` & `trytond-7.2.1/trytond/tests/field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_text.py` & `trytond-7.2.1/trytond/tests/field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_time.py` & `trytond-7.2.1/trytond/tests/field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/field_timedelta.py` & `trytond-7.2.1/trytond/tests/field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/history.py` & `trytond-7.2.1/trytond/tests/history.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/import_data.py` & `trytond-7.2.1/trytond/tests/import_data.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/import_data.xml` & `trytond-7.2.1/trytond/tests/import_data.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/message.xml` & `trytond-7.2.1/trytond/tests/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/mixin.py` & `trytond-7.2.1/trytond/tests/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/model.py` & `trytond-7.2.1/trytond/tests/model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/model_log.py` & `trytond-7.2.1/trytond/tests/model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/modelsql.py` & `trytond-7.2.1/trytond/tests/modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/modelstorage.py` & `trytond-7.2.1/trytond/tests/modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/modelview.py` & `trytond-7.2.1/trytond/tests/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/modelview.xml` & `trytond-7.2.1/trytond/tests/modelview.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/mptt.py` & `trytond-7.2.1/trytond/tests/mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/multivalue.py` & `trytond-7.2.1/trytond/tests/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/path.py` & `trytond-7.2.1/trytond/tests/path.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/resource.py` & `trytond-7.2.1/trytond/tests/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/rule.py` & `trytond-7.2.1/trytond/tests/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/sequence.xml` & `trytond-7.2.1/trytond/tests/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_access.py` & `trytond-7.2.1/trytond/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_backend.py` & `trytond-7.2.1/trytond/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_bus.py` & `trytond-7.2.1/trytond/tests/test_bus.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_cache.py` & `trytond-7.2.1/trytond/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_copy.py` & `trytond-7.2.1/trytond/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_exportdata.py` & `trytond-7.2.1/trytond/tests/test_exportdata.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_binary.py` & `trytond-7.2.1/trytond/tests/test_field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_boolean.py` & `trytond-7.2.1/trytond/tests/test_field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_char.py` & `trytond-7.2.1/trytond/tests/test_field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_context.py` & `trytond-7.2.1/trytond/tests/test_field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_date.py` & `trytond-7.2.1/trytond/tests/test_field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_datetime.py` & `trytond-7.2.1/trytond/tests/test_field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_depends.py` & `trytond-7.2.1/trytond/tests/test_field_depends.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_dict.py` & `trytond-7.2.1/trytond/tests/test_field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_float.py` & `trytond-7.2.1/trytond/tests/test_field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_function.py` & `trytond-7.2.1/trytond/tests/test_field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_integer.py` & `trytond-7.2.1/trytond/tests/test_field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_many2many.py` & `trytond-7.2.1/trytond/tests/test_field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_many2one.py` & `trytond-7.2.1/trytond/tests/test_field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_multiselection.py` & `trytond-7.2.1/trytond/tests/test_field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_numeric.py` & `trytond-7.2.1/trytond/tests/test_field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_one2many.py` & `trytond-7.2.1/trytond/tests/test_field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_one2one.py` & `trytond-7.2.1/trytond/tests/test_field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_reference.py` & `trytond-7.2.1/trytond/tests/test_field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_selection.py` & `trytond-7.2.1/trytond/tests/test_field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_text.py` & `trytond-7.2.1/trytond/tests/test_field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_time.py` & `trytond-7.2.1/trytond/tests/test_field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_field_timedelta.py` & `trytond-7.2.1/trytond/tests/test_field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_filestore.py` & `trytond-7.2.1/trytond/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_history.py` & `trytond-7.2.1/trytond/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_i18n.py` & `trytond-7.2.1/trytond/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_importdata.py` & `trytond-7.2.1/trytond/tests/test_importdata.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_ir.py` & `trytond-7.2.1/trytond/tests/test_ir.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_mixins.py` & `trytond-7.2.1/trytond/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_model.py` & `trytond-7.2.1/trytond/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_model_index.py` & `trytond-7.2.1/trytond/tests/test_model_index.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_model_log.py` & `trytond-7.2.1/trytond/tests/test_model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_model_match.py` & `trytond-7.2.1/trytond/tests/test_model_match.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_modelsingleton.py` & `trytond-7.2.1/trytond/tests/test_modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_modelsql.py` & `trytond-7.2.1/trytond/tests/test_modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_modelstorage.py` & `trytond-7.2.1/trytond/tests/test_modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_modelview.py` & `trytond-7.2.1/trytond/tests/test_modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_mptt.py` & `trytond-7.2.1/trytond/tests/test_mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_multivalue.py` & `trytond-7.2.1/trytond/tests/test_multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_order.py` & `trytond-7.2.1/trytond/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_path.py` & `trytond-7.2.1/trytond/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_protocols.py` & `trytond-7.2.1/trytond/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_pyson.py` & `trytond-7.2.1/trytond/tests/test_pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_report.py` & `trytond-7.2.1/trytond/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_res.py` & `trytond-7.2.1/trytond/tests/test_res.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_resource.py` & `trytond-7.2.1/trytond/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_routes.py` & `trytond-7.2.1/trytond/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_rpc.py` & `trytond-7.2.1/trytond/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_rule.py` & `trytond-7.2.1/trytond/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_sendmail.py` & `trytond-7.2.1/trytond/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_sequence.py` & `trytond-7.2.1/trytond/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_tools.py` & `trytond-7.2.1/trytond/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_transaction.py` & `trytond-7.2.1/trytond/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_tree.py` & `trytond-7.2.1/trytond/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_trigger.py` & `trytond-7.2.1/trytond/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_tryton.py` & `trytond-7.2.1/trytond/tests/test_tryton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_union.py` & `trytond-7.2.1/trytond/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_user.py` & `trytond-7.2.1/trytond/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_wizard.py` & `trytond-7.2.1/trytond/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_workflow.py` & `trytond-7.2.1/trytond/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/test_wsgi.py` & `trytond-7.2.1/trytond/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/tools.py` & `trytond-7.2.1/trytond/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/tree.py` & `trytond-7.2.1/trytond/tests/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/trigger.py` & `trytond-7.2.1/trytond/tests/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/wizard.py` & `trytond-7.2.1/trytond/tests/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/wizard.xml` & `trytond-7.2.1/trytond/tests/wizard.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tests/workflow.py` & `trytond-7.2.1/trytond/tests/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/__init__.py` & `trytond-7.2.1/trytond/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/barcode.py` & `trytond-7.2.1/trytond/tools/barcode.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/decimal_.py` & `trytond-7.2.1/trytond/tools/decimal_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/domain_inversion.py` & `trytond-7.2.1/trytond/tools/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/email_.py` & `trytond-7.2.1/trytond/tools/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/immutabledict.py` & `trytond-7.2.1/trytond/tools/immutabledict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/logging.py` & `trytond-7.2.1/trytond/tools/logging.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/misc.py` & `trytond-7.2.1/trytond/tools/misc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/qrcode.py` & `trytond-7.2.1/trytond/tools/qrcode.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/singleton.py` & `trytond-7.2.1/trytond/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/string_.py` & `trytond-7.2.1/trytond/tools/string_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tools/timezone.py` & `trytond-7.2.1/trytond/tools/timezone.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/transaction.py` & `trytond-7.2.1/trytond/transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tryton.rnc` & `trytond-7.2.1/trytond/tryton.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/tryton.rng` & `trytond-7.2.1/trytond/tryton.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/url.py` & `trytond-7.2.1/trytond/url.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/wizard/wizard.py` & `trytond-7.2.1/trytond/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/worker.py` & `trytond-7.2.1/trytond/worker.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond/wsgi.py` & `trytond-7.2.1/trytond/wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond.egg-info/PKG-INFO` & `trytond-7.2.1/trytond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton server
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond-7.2.0/trytond.egg-info/SOURCES.txt` & `trytond-7.2.1/trytond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond-7.2.0/trytond.egg-info/requires.txt` & `trytond-7.2.1/trytond.egg-info/requires.txt`

 * *Files identical despite different names*

