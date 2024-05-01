# Comparing `tmp/lamindb_setup-0.70.0.tar.gz` & `tmp/lamindb_setup-0.71.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.70.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.71.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.70.0.tar` & `lamindb_setup-0.71.0.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0     8290 2024-04-16 19:27:14.643060 lamindb_setup-0.70.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.70.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.70.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.70.0/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.70.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.70.0/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.70.0/README.md
--rw-r--r--   0        0        0    97544 2024-04-24 10:46:02.552654 lamindb_setup-0.70.0/docs/changelog.md
--rw-r--r--   0        0        0     2573 2024-04-23 21:24:09.761470 lamindb_setup-0.70.0/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3947 2024-04-23 21:24:09.761588 lamindb_setup-0.70.0/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0     5817 2024-04-23 13:03:29.807601 lamindb_setup-0.70.0/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.70.0/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3111 2024-04-23 13:03:29.807936 lamindb_setup-0.70.0/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3806 2024-04-21 08:00:19.897288 lamindb_setup-0.70.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     2779 2024-04-23 21:24:09.761821 lamindb_setup-0.70.0/docs/hub-cloud/07-connect-hybrid-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.70.0/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.70.0/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-04-22 13:06:55.467504 lamindb_setup-0.70.0/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.70.0/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.70.0/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2711 2024-04-23 13:03:29.808107 lamindb_setup-0.70.0/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.70.0/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.70.0/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.70.0/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-04-22 20:26:08.605836 lamindb_setup-0.70.0/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.70.0/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.70.0/docs/index.md
--rw-r--r--   0        0        0      516 2024-04-23 21:24:09.762085 lamindb_setup-0.70.0/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.70.0/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-04-24 10:45:41.099277 lamindb_setup-0.70.0/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.70.0/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-04-23 11:01:04.804829 lamindb_setup-0.70.0/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.70.0/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.70.0/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.70.0/lamindb_setup/_close.py
--rw-r--r--   0        0        0    11908 2024-04-24 10:00:32.983268 lamindb_setup-0.70.0/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     5861 2024-04-24 09:58:58.984598 lamindb_setup-0.70.0/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.70.0/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2084 2024-04-15 04:44:50.596309 lamindb_setup-0.70.0/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1836 2024-04-15 06:35:29.022278 lamindb_setup-0.70.0/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11480 2024-04-23 14:54:28.059779 lamindb_setup-0.70.0/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8810 2024-04-23 21:24:09.762839 lamindb_setup-0.70.0/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      796 2024-04-23 14:54:28.060356 lamindb_setup-0.70.0/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.70.0/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3658 2024-04-23 14:54:28.060603 lamindb_setup-0.70.0/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.70.0/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      369 2024-04-16 15:26:03.848647 lamindb_setup-0.70.0/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.70.0/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.70.0/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.70.0/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5520 2024-04-15 15:03:26.266397 lamindb_setup-0.70.0/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    11294 2024-04-23 21:24:09.763136 lamindb_setup-0.70.0/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.70.0/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.70.0/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.70.0/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    13927 2024-04-24 09:59:49.631691 lamindb_setup-0.70.0/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3745 2024-04-23 14:54:28.061051 lamindb_setup-0.70.0/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2571 2024-04-23 14:54:28.061337 lamindb_setup-0.70.0/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    11750 2024-04-23 21:24:09.763780 lamindb_setup-0.70.0/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.70.0/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1282 2024-04-23 14:54:28.061801 lamindb_setup-0.70.0/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.70.0/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.70.0/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3411 2024-04-23 21:24:09.764077 lamindb_setup-0.70.0/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.70.0/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.70.0/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.70.0/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    25078 2024-04-23 14:26:22.574000 lamindb_setup-0.70.0/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.70.0/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.70.0/pyproject.toml
--rw-r--r--   0        0        0     5379 2024-04-23 21:24:09.764323 lamindb_setup-0.70.0/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.70.0/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     6179 2024-04-23 13:03:29.809705 lamindb_setup-0.70.0/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.70.0/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.70.0/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.70.0/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.70.0/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11329 2024-04-23 14:54:28.062287 lamindb_setup-0.70.0/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      398 2024-04-22 20:59:53.004753 lamindb_setup-0.70.0/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.70.0/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      158 2024-04-16 15:26:03.849537 lamindb_setup-0.70.0/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1432 2024-04-15 15:03:26.267758 lamindb_setup-0.70.0/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.70.0/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.70.0/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.70.0/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.70.0/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-04-22 06:08:16.280331 lamindb_setup-0.70.0/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.70.0/PKG-INFO
+-rw-r--r--   0        0        0     8451 2024-04-30 14:26:00.291346 lamindb_setup-0.71.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.71.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.71.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.71.0/.gitignore
+-rw-r--r--   0        0        0     1474 2024-04-25 16:11:02.471704 lamindb_setup-0.71.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.71.0/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.71.0/README.md
+-rw-r--r--   0        0        0    99141 2024-05-01 17:41:01.022816 lamindb_setup-0.71.0/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-04-29 07:49:33.469384 lamindb_setup-0.71.0/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-04-27 13:43:14.991516 lamindb_setup-0.71.0/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0     9828 2024-04-30 14:26:00.292134 lamindb_setup-0.71.0/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-04-25 13:58:37.156407 lamindb_setup-0.71.0/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3112 2024-04-26 09:07:16.588255 lamindb_setup-0.71.0/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3806 2024-04-25 13:58:37.138044 lamindb_setup-0.71.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-04-30 14:26:00.292361 lamindb_setup-0.71.0/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-04-25 13:58:37.156237 lamindb_setup-0.71.0/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472152 lamindb_setup-0.71.0/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-04-29 07:29:41.597110 lamindb_setup-0.71.0/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-04-25 13:58:37.175784 lamindb_setup-0.71.0/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-04-25 13:58:37.157085 lamindb_setup-0.71.0/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-04-27 13:43:14.991856 lamindb_setup-0.71.0/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-04-25 13:58:37.174178 lamindb_setup-0.71.0/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-04-25 13:58:37.139783 lamindb_setup-0.71.0/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-04-25 13:58:37.137631 lamindb_setup-0.71.0/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-04-27 13:43:14.992063 lamindb_setup-0.71.0/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472299 lamindb_setup-0.71.0/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.71.0/docs/index.md
+-rw-r--r--   0        0        0      513 2024-04-30 14:26:00.292603 lamindb_setup-0.71.0/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.71.0/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-01 17:38:56.943344 lamindb_setup-0.71.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1325 2024-04-30 14:26:00.293225 lamindb_setup-0.71.0/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      846 2024-04-25 16:11:02.473229 lamindb_setup-0.71.0/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-04-25 16:11:02.473531 lamindb_setup-0.71.0/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-04-25 16:11:02.473724 lamindb_setup-0.71.0/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-04-25 16:11:02.473895 lamindb_setup-0.71.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    11944 2024-04-30 14:26:00.293578 lamindb_setup-0.71.0/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     7267 2024-05-01 05:19:31.568362 lamindb_setup-0.71.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-04-25 16:11:02.474852 lamindb_setup-0.71.0/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-04-25 16:11:02.475059 lamindb_setup-0.71.0/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-04-25 16:11:02.475261 lamindb_setup-0.71.0/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11825 2024-05-01 05:38:35.719751 lamindb_setup-0.71.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-04-27 13:43:14.993255 lamindb_setup-0.71.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-04-30 14:26:00.294512 lamindb_setup-0.71.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-04-25 16:11:02.476265 lamindb_setup-0.71.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3670 2024-04-25 16:11:02.476440 lamindb_setup-0.71.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-04-25 16:11:02.476624 lamindb_setup-0.71.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-04-30 14:26:00.294783 lamindb_setup-0.71.0/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-25 16:11:02.477005 lamindb_setup-0.71.0/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-04-25 16:11:02.477187 lamindb_setup-0.71.0/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-04-25 16:11:02.477423 lamindb_setup-0.71.0/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-04-25 16:11:02.477677 lamindb_setup-0.71.0/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    15776 2024-05-01 05:19:31.563200 lamindb_setup-0.71.0/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4662 2024-04-30 14:26:00.295410 lamindb_setup-0.71.0/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-04-25 16:11:02.478546 lamindb_setup-0.71.0/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-04-30 14:26:00.295688 lamindb_setup-0.71.0/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16588 2024-04-30 14:26:00.296030 lamindb_setup-0.71.0/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3849 2024-04-27 13:43:14.994618 lamindb_setup-0.71.0/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2637 2024-04-27 13:43:14.994895 lamindb_setup-0.71.0/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    12739 2024-04-30 14:26:00.296388 lamindb_setup-0.71.0/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2043 2024-04-25 16:11:02.480541 lamindb_setup-0.71.0/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1344 2024-04-25 16:11:02.480798 lamindb_setup-0.71.0/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3002 2024-04-25 16:11:02.481032 lamindb_setup-0.71.0/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-04-27 13:43:14.995437 lamindb_setup-0.71.0/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3450 2024-04-30 14:26:00.296696 lamindb_setup-0.71.0/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-04-25 16:11:02.481611 lamindb_setup-0.71.0/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2218 2024-04-27 13:43:14.995719 lamindb_setup-0.71.0/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-04-25 16:11:02.482026 lamindb_setup-0.71.0/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    27965 2024-04-30 14:26:00.297107 lamindb_setup-0.71.0/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3325 2024-04-30 14:26:00.297371 lamindb_setup-0.71.0/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-04-30 14:26:00.297636 lamindb_setup-0.71.0/pyproject.toml
+-rw-r--r--   0        0        0     5410 2024-04-27 13:43:14.996364 lamindb_setup-0.71.0/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      320 2024-04-25 16:11:02.483189 lamindb_setup-0.71.0/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5590 2024-04-30 14:26:00.297937 lamindb_setup-0.71.0/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-04-25 16:11:02.483601 lamindb_setup-0.71.0/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-04-25 16:11:02.483785 lamindb_setup-0.71.0/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      355 2024-04-30 14:26:00.298229 lamindb_setup-0.71.0/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      582 2024-04-25 16:11:02.484159 lamindb_setup-0.71.0/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11218 2024-04-30 14:26:00.298556 lamindb_setup-0.71.0/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      734 2024-04-30 14:26:00.298827 lamindb_setup-0.71.0/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-04-25 16:11:02.484790 lamindb_setup-0.71.0/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-04-25 16:11:02.484963 lamindb_setup-0.71.0/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-04-25 16:11:02.485160 lamindb_setup-0.71.0/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-04-30 14:26:00.299030 lamindb_setup-0.71.0/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-04-27 13:43:14.997388 lamindb_setup-0.71.0/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-04-27 13:43:14.997583 lamindb_setup-0.71.0/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      824 2024-04-25 16:11:02.485962 lamindb_setup-0.71.0/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      878 2024-04-25 16:11:02.486161 lamindb_setup-0.71.0/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-04-25 16:11:02.486329 lamindb_setup-0.71.0/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.0/PKG-INFO
```

### Comparing `lamindb_setup-0.70.0/.github/workflows/build.yml` & `lamindb_setup-0.71.0/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,53 +12,52 @@
   # tests only on production hub
   hub-prod:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-          cache: 'pip'
-          cache-dependency-path: '.github/workflows/build.yml'
+          python-version: "3.9" # consciously run one job on Python 3.9
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
       - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - run: pip install -U laminci
-      - run: nox -s lint
       - run: nox -s "install(group='hub-prod')"
       - run: nox -s "build(lamin_env='prod', group='hub-prod')"
       - uses: actions/upload-artifact@v2
         with:
           name: coverage--hub-prod
           path: .coverage
 
   # tests both on production and staging hub
   hub-cloud:
     runs-on: ubuntu-22.04
     strategy:
       fail-fast: false
       matrix:
         lamin_env:
-          - 'staging'
-          - 'prod'
+          - "staging"
+          - "prod"
     timeout-minutes: 15
     steps:
       - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-          cache: 'pip'
-          cache-dependency-path: '.github/workflows/build.yml'
+          python-version: "3.11" # consciously run one job on Python 3.11
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
       - name: checkout laminhub
         uses: actions/checkout@v4
         with:
           repository: laminlabs/laminapp-ui
           token: ${{ secrets.GH_TOKEN_DEPLOY_LAMINAPP }}
           path: laminhub
           ref: main
@@ -92,19 +91,20 @@
   # test user access to storage
   storage:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-          cache: 'pip'
-          cache-dependency-path: '.github/workflows/build.yml'
+          python-version: "3.10" # consciously run one job on Python 3.10
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
       - run: pip install -U laminci
       - run: nox -s "install(group='storage')"
+      - run: nox -s lint
       - run: nox -s storage
         env:
           TEST_INSTANCE_PRIVATE_POSTGRES: ${{ secrets.TEST_INSTANCE_PRIVATE_POSTGRES }}
           TMP_AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
           TMP_AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
       - uses: actions/upload-artifact@v2
         with:
@@ -133,43 +133,43 @@
         run: |
           touch .env.local
           echo "AWS_ACCESS_KEY_ID_HOSTED_S3=${{ secrets.AWS_ACCESS_KEY_ID }}" >> .env.local
           echo "AWS_SECRET_ACCESS_KEY_HOSTED_S3=${{ secrets.AWS_SECRET_ACCESS_KEY }}" >> .env.local
         working-directory: laminhub/rest-hub/supabase
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-          cache: 'pip'
-          cache-dependency-path: '.github/workflows/build.yml'
+          python-version: "3.11" # consciously run one job on Python 3.11
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
       - run: pip install -U laminci
       - run: nox -s "install(group='hub-local')"
       - id: cache-supabase
         uses: actions/cache@v3
         with:
           path: /var/lib/docker
           key: cache-supabase
       - uses: supabase/setup-cli@v1
       - run: nox -s hub_local
         env:
-          LAMIN_ENV: 'local'
+          LAMIN_ENV: "local"
       - uses: actions/upload-artifact@v2
         with:
           name: coverage--hub-local
           path: .coverage
 
   coverage:
     needs: [hub-prod, hub-cloud, storage, hub-local]
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-          cache: 'pip'
-          cache-dependency-path: '.github/workflows/build.yml'
+          python-version: "3.10"
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
       - run: |
           pip install coverage[toml]
           pip install --no-deps .
       - uses: actions/download-artifact@v2
       - name: run coverage
         run: |
           coverage combine coverage--*/.coverage*
@@ -197,24 +197,24 @@
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-          cache: 'pip'
-          cache-dependency-path: '.github/workflows/build.yml'
+          python-version: "3.10"
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml"
       - run: pip install -U laminci
-      - run: nox -s "install(group='storage')"
+      - run: nox -s "install(group='docs')"
       - uses: actions/download-artifact@v2
       - run: nox -s docs
       - uses: nwtgck/actions-netlify@v1.2
         with:
-          publish-dir: '_build/html'
+          publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
           NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
 
@@ -226,18 +226,18 @@
     runs-on: ubuntu-latest
     steps:
       - uses: voxmedia/github-action-slack-notify-build@v1
         if: ${{ needs.hub-local.result == 'success' && needs.hub-cloud.result == 'success' && github.event_name == 'repository_dispatch' }}
         env:
           SLACK_BOT_TOKEN: ${{ secrets.SLACK_GITHUB_ACTION }}
         with:
-          channel: web-hub-tests
+          channel_id: C05S2C02JHM
           status: SUCCESS
           color: good
       - uses: voxmedia/github-action-slack-notify-build@v1
         if: ${{ ( needs.hub-local.result == 'failure' || needs.hub-cloud.result == 'failure' ) && github.event_name == 'repository_dispatch' }}
         env:
           SLACK_BOT_TOKEN: ${{ secrets.SLACK_GITHUB_ACTION }}
         with:
-          channel: web-hub-tests
+          channel_id: C05S2C02JHM
           status: FAILURE
           color: danger
```

### Comparing `lamindb_setup-0.70.0/.github/workflows/latest-changes.yml` & `lamindb_setup-0.71.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/.gitignore` & `lamindb_setup-0.71.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/.pre-commit-config.yaml` & `lamindb_setup-0.71.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,47 @@
 repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
-    hooks:
-      - id: trailing-whitespace
-      - id: end-of-file-fixer
-        exclude: |
-          (?x)(
-              .github/workflows/latest-changes.jinja2
-          )
-      - id: check-yaml
-      - id: check-added-large-files
-  - repo: https://github.com/psf/black
-    rev: 22.6.0
-    hooks:
-      - id: black-jupyter
-        exclude: |
-          (?x)(
-              _check_instance_setup.py
-          )
-  - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-black==0.3.3
-          - flake8-typing-imports==1.10.0
-        language_version: python3
-        args:
-          - --max-line-length=88
-          - --ignore=E203,W503,BLK100,TYP001
-        exclude: |
-          (?x)(
-              __init__.py
-          )
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.6.2
+    rev: v4.0.0-alpha.4
     hooks:
       - id: prettier
         exclude: |
           (?x)(
-              .github/workflows/build.yml
+            docs/changelog.md
           )
   - repo: https://github.com/kynan/nbstripout
-    rev: 0.3.9
+    rev: 0.6.1
     hooks:
       - id: nbstripout
         exclude: |
           (?x)(
               docs/examples/|
-              docs/notes/|
-              tests
+              docs/notes/
           )
-  - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.1.9
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.1.7
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix, --unsafe-fixes]
+      - id: ruff-format
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.5.0
     hooks:
-      - id: forbid-crlf
-      - id: remove-crlf
+      - id: detect-private-key
+      - id: check-ast
+      - id: end-of-file-fixer
+        exclude: |
+          (?x)(
+              .github/workflows/latest-changes.jinja2
+            )
+      - id: mixed-line-ending
+        args: [--fix=lf]
+      - id: trailing-whitespace
+      - id: check-case-conflict
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.940
+    rev: v1.7.1
     hooks:
       - id: mypy
         exclude: |
           (?x)(
               tests/hub-local/conftest.py
           )
   - repo: https://github.com/pycqa/pydocstyle
```

### Comparing `lamindb_setup-0.70.0/LICENSE` & `lamindb_setup-0.71.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/changelog.md` & `lamindb_setup-0.71.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix delete function | [741](https://github.com/laminlabs/lamindb-setup/pull/741) | [falexwolf](https://github.com/falexwolf) | 2024-04-30 | 0.71.0
+✨ Manage multiple storage locations with integrity | [738](https://github.com/laminlabs/lamindb-setup/pull/738) | [falexwolf](https://github.com/falexwolf) | 2024-04-30 |
+✨ Proper progress bars for upload and download | [739](https://github.com/laminlabs/lamindb-setup/pull/739) | [Koncopd](https://github.com/Koncopd) | 2024-04-28 |
+♻️ Truncate fsspec deps | [740](https://github.com/laminlabs/lamindb-setup/pull/740) | [Koncopd](https://github.com/Koncopd) | 2024-04-28 |
+♻️ Refactor storage management | [734](https://github.com/laminlabs/lamindb-setup/pull/734) | [falexwolf](https://github.com/falexwolf) | 2024-04-27 |
+⬆️ Upper and lower bounds for fsspec | [736](https://github.com/laminlabs/lamindb-setup/pull/736) | [Koncopd](https://github.com/Koncopd) | 2024-04-27 |
+♻️ Capitalize HOSTED | [733](https://github.com/laminlabs/lamindb-setup/pull/733) | [falexwolf](https://github.com/falexwolf) | 2024-04-26 |
+♻️ Refactor noxfile and manage `aws` extra here instead of in lamindb | [732](https://github.com/laminlabs/lamindb-setup/pull/732) | [falexwolf](https://github.com/falexwolf) | 2024-04-25 |
+🏷️ Add 3.10 types & ruff | [731](https://github.com/laminlabs/lamindb-setup/pull/731) | [falexwolf](https://github.com/falexwolf) | 2024-04-25 |
+♻️ Backward compat for older botocore | [730](https://github.com/laminlabs/lamindb-setup/pull/730) | [falexwolf](https://github.com/falexwolf) | 2024-04-25 |
 ✨ Introduce `local_storage` mode for cloud instances | [728](https://github.com/laminlabs/lamindb-setup/pull/728) | [falexwolf](https://github.com/falexwolf) | 2024-04-23 | 0.70.0
 🚚 Make `.uuid` attributes private | [727](https://github.com/laminlabs/lamindb-setup/pull/727) | [falexwolf](https://github.com/falexwolf) | 2024-04-23 |
 🚚 Rename `is_cloud` to `type_is_cloud` | [726](https://github.com/laminlabs/lamindb-setup/pull/726) | [falexwolf](https://github.com/falexwolf) | 2024-04-23 |
 🚸 In `.delete()`, check for data deletion & delete from hub | [725](https://github.com/laminlabs/lamindb-setup/pull/725) | [falexwolf](https://github.com/falexwolf) | 2024-04-22 |
 ✨ Upload dirs inplace | [722](https://github.com/laminlabs/lamindb-setup/pull/722) | [Koncopd](https://github.com/Koncopd) | 2024-04-20 | 0.69.5
 ♻️ Do not always read from local cache | [720](https://github.com/laminlabs/lamindb-setup/pull/720) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 | 0.69.4
 ♻️ Improve suffix handling | [718](https://github.com/laminlabs/lamindb-setup/pull/718) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 | 0.69.3
```

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997448979591836%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(11, '    == "*

 * *            'f"sqlite:///{Path(\\\'./mydata\\\').resolve().as_posix()}/{ln_setup.settings.instance._id.hex}.lndb"\\n\')], '*

 * *            'delete: [11]}}}'}*

```diff
@@ -54,15 +54,15 @@
                 "assert ln_setup.settings.instance.name == \"mydata\"\n",
                 "assert ln_setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
                 "storage_root = ln_setup.settings.storage.root\n",
                 "assert storage_root.exists()\n",
                 "assert ln_setup.settings.storage.id is not None\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
+                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/{ln_setup.settings.instance._id.hex}.lndb\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998664529914529%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(10, '    == "*

 * *            'f"sqlite:///{Path(\\\'./mydata_new_loc\\\').resolve().as_posix()}/{ln_setup.settings.instance._id.hex}.lndb"\\n\')], '*

 * *            'delete: [10]}}}'}*

```diff
@@ -96,15 +96,15 @@
                 "assert ln_setup.settings.instance.name == \"mydata\"\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
                 ")\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
+                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/{ln_setup.settings.instance._id.hex}.lndb\"\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "0986a5f3",
```

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.769040854978355%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}, 'source': ['# Connect with "*

 * *            '`keep_artifacts_local=True`\'], delete: [\'id\']}, 1: {\'source\': {insert: [(0, "# '*

 * *            'this shouldn\'t run in a notebook, but in the unit tests\\n"), (1, \'# currently '*

 * *            "still limited because of inability to load multiple instances\\n'), (2, '\\n'), (3, "*

 * *            "'import pytest\\n'), (5, 'from pathlib import Path\\n'), (6, '\\n'), (7, "*

 * *            '\'ln_setup.login("testuser1")\\n […]*

```diff
@@ -1,280 +1,216 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "# Add remote storage"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "6422b64e",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
+            "metadata": {},
             "source": [
-                "!lamin close\n",
-                "!yes | lamin delete pgtest"
+                "# Connect with `keep_artifacts_local=True`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
+                "# this shouldn't run in a notebook, but in the unit tests\n",
+                "# currently still limited because of inability to load multiple instances\n",
+                "\n",
+                "import pytest\n",
                 "import lamindb_setup as ln_setup\n",
-                "from lamindb_setup._add_remote_storage import switch_default_storage"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "a7cf42fb",
-            "metadata": {},
-            "source": [
-                "## Add remote storage"
+                "from pathlib import Path\n",
+                "\n",
+                "ln_setup.login(\"testuser1\")\n",
+                "ln_setup.init(storage=\"s3://lamindb-ci/keep-artifacts-local-setup\")\n",
+                "\n",
+                "assert ln_setup.settings.instance.name == \"keep-artifacts-local-setup\"\n",
+                "assert ln_setup.settings.instance.storage.type_is_cloud\n",
+                "assert (\n",
+                "    ln_setup.settings.instance.storage.root_as_str\n",
+                "    == \"s3://lamindb-ci/keep-artifacts-local-setup\"\n",
+                ")\n",
+                "assert (\n",
+                "    ln_setup.settings.instance._sqlite_file.as_posix()\n",
+                "    == f\"s3://lamindb-ci/keep-artifacts-local-setup/{ln_setup.settings.instance._id.hex}.lndb\"  # noqa\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8fd59ad3-04b9-42fb-83cc-ab7beedbec72",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "import laminci\n",
-                "\n",
-                "!docker stop pgtest && docker rm pgtest\n",
-                "pgurl = laminci.db.setup_local_test_postgres()"
+                "with pytest.raises(ValueError) as error:\n",
+                "    ln_setup.settings.instance.storage_local\n",
+                "assert error.exconly() == \"ValueError: `keep_artifacts_local` is not enabled for this instance.\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d6b0bd5e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.init(storage=\"./storage1\", db=pgurl)"
+                "ln_setup.settings.instance._keep_artifacts_local = True\n",
+                "with pytest.raises(ValueError) as error:\n",
+                "    ln_setup.settings.instance.storage_local"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "63392da0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.settings.storage.root"
+                "# now set local storage location\n",
+                "ln_setup.settings.instance.storage_local = \"./my_storage_local\"\n",
+                "\n",
+                "assert (\n",
+                "    ln_setup.settings.instance.storage_local.root.as_posix()\n",
+                "    == Path(\"./my_storage_local\").resolve().as_posix()\n",
+                ")\n",
+                "assert (ln_setup.settings.instance.storage_local.root / \".lamindb/_is_initialized\").read_text() == ln_setup.settings.instance.storage_local.uid\n",
+                "assert ln_setup.settings.instance.storage_local is not None\n",
+                "# the remote storage location is still in the regular slot\n",
+                "assert ln_setup.settings.instance.storage.root.as_posix() == \"s3://lamindb-ci/keep-artifacts-local-setup\""
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e6638f44",
             "metadata": {},
             "source": [
-                "Local storage:"
+                "Another one:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "49b9ef11",
             "metadata": {},
             "outputs": [],
             "source": [
-                "switch_default_storage(\"./storage_2\")"
+                "ln_setup.settings.instance.storage_local = \"./my_storage_local2\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "47b1f038",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.settings.storage.root"
+                "assert (\n",
+                "    ln_setup.settings.instance.storage_local.root.as_posix()\n",
+                "    == Path(\"./my_storage_local2\").resolve().as_posix()\n",
+                ")\n",
+                "assert (ln_setup.settings.instance.storage_local.root / \".lamindb/_is_initialized\").read_text() == ln_setup.settings.instance.storage_local.uid"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f943e220",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln_setup.settings.storage.root_as_str"
+                "See whether we can repeat this:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e481aa0",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "\n",
-                "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
+                "ln_setup.settings.instance.storage_local = \"./my_storage_local2\""
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "de1c12b8",
             "metadata": {},
             "source": [
-                "Cloud storage:"
+                "And back to the initial one:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "switch_default_storage(\"s3://lamindb-ci\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "af069899",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln_setup.settings.storage.root"
+                "ln_setup.settings.instance.storage_local = \"./my_storage_local\""
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "859a972e",
             "metadata": {},
             "source": [
-                "See an overview:"
+                "Add a test file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d2934990",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln_setup.settings.storage.type_is_cloud\n",
-                "assert ln_setup.settings.storage.root_as_str == \"s3://lamindb-ci\"\n",
-                "assert ln_setup.settings.storage.region == \"us-west-1\"\n",
-                "# root.fs contains the underlying fsspec filesystem\n",
-                "assert (\n",
-                "    ln_setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
-                ")"
+                "test_file = (ln_setup.settings.instance.storage_local.root / \".lamindb/test_file.txt\")\n",
+                "test_file.write_text(\"test\")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "ae953b6a",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You can set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
+                "ln_setup.settings.instance.storage_local.root.view_tree()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f9294082",
             "metadata": {},
             "outputs": [],
             "source": [
-                "switch_default_storage(\"s3://lamindb-ci\", cache_regions=False)"
+                "with pytest.raises(ln_setup.core.upath.InstanceNotEmpty):\n",
+                "    ln_setup.delete(\"keep-artifacts-local-setup\", force=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d6915638-db49-4d3d-bd91-819bb4719ef7",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# test cache_regions\n",
-                "assert not ln_setup.settings.storage.root.fs.cache_regions\n",
-                "# test setting storage not by owner\n",
-                "ln_setup.login(\"testuser2@lamin.ai\", key=\"goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz\")\n",
-                "switch_default_storage(\"./storage_3\")\n",
-                "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\"\n",
-                "!docker stop pgtest && docker rm pgtest"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "3fb6a223",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "### Currently not possible: setting storage for SQLite instance"
+                "test_file.unlink()"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "6ccb6573",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "If you try to set the storage for an sqlite instance, an error message is returned:\n",
-                "```\n",
-                "assert switch_default_storage(\"mydata_storage_2\") == \"set-storage-failed\"\n",
-                "```"
+                "ln_setup.delete(\"keep-artifacts-local-setup\", force=True)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "py310",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.13"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
-            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959160052910053%*

 * *Differences: {"'cells'": "{6: {'source': ['from lamindb_setup.core.upath import HOSTED_BUCKETS']}, 7: "*

 * *            "{'source': {insert: [(3, 'assert "*

 * *            "ln_setup.settings.storage.root.as_posix().startswith(HOSTED_BUCKETS)\\n')], delete: "*

 * *            '[3]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.13'}}"}*

```diff
@@ -77,27 +77,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lamindb_setup.core.upath import hosted_buckets"
+                "from lamindb_setup.core.upath import HOSTED_BUCKETS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert ln_setup.settings.instance.storage.type_is_cloud == True\n",
                 "assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle\n",
                 "assert ln_setup.settings.instance.name == \"my-hosted\"\n",
-                "assert ln_setup.settings.storage.root.as_posix().startswith(hosted_buckets)\n",
+                "assert ln_setup.settings.storage.root.as_posix().startswith(HOSTED_BUCKETS)\n",
                 "assert ln_setup.settings.storage.id is not None"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -119,13 +119,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.17"
+            "version": "3.10.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.71.0/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-empty-init.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997106481481481%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(5, '    == "*

 * *            'f"{root_str}/{ln_setup.settings.instance._id.hex}.lndb"\\n\')], delete: [5]}}}'}*

```diff
@@ -72,15 +72,15 @@
             "outputs": [],
             "source": [
                 "assert ln_setup.settings.storage.type_is_cloud\n",
                 "assert ln_setup.settings.storage.root_as_str == root_str\n",
                 "assert ln_setup.settings.storage.region == \"us-east-1\"\n",
                 "assert (\n",
                 "    str(ln_setup.settings.instance._sqlite_file)\n",
-                "    == f\"{root_str}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
+                "    == f\"{root_str}/{ln_setup.settings.instance._id.hex}.lndb\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a339197a",
```

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.70.0/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.71.0/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997632575757576%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(1, 'instance_id = ln_setup.settings.instance._id\\n')], "*

 * *            'delete: [1]}}}'}*

```diff
@@ -70,15 +70,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "201d1baf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln_setup.init(storage=\"s3://lamindb-ci/test-load-lock\", name=\"test-load-lock\")\n",
-                "instance_id = ln_setup.settings.instance.id\n",
+                "instance_id = ln_setup.settings.instance._id\n",
                 "ln_setup.close()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f628325e",
```

### Comparing `lamindb_setup-0.70.0/docs/notebooks.md` & `lamindb_setup-0.71.0/docs/notebooks.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 hub-cloud/init-local-instance
 hub-cloud/connect-local-instance
 hub-cloud/set-storage
 hub-cloud/test-bionty
 hub-cloud/init-hosted-instance
 hub-cloud/connect-hosted-instance
 hub-cloud/test-multi-session
-hub-cloud/connect-hybrid-instance
+hub-cloud/keep-artifacts-local
 
 hub-prod/test-cache-management
 hub-prod/test-empty-init
 hub-prod/test-import-schema
 hub-prod/test-invalid-schema
 hub-prod/test-insufficient-user-info
 hub-prod/test-connect-anonymously
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/__init__.py` & `lamindb_setup-0.71.0/lamindb_setup/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Setup & configure LaminDB.
 
-Every function in the API has a matching command in the `lamin` CLI.
-
-Typically, you'll want to use the CLI rather than this API.
+Many functions in this "setup API" have a matching command in the :doc:`docs:cli` CLI.
 
 Guide: :doc:`docs:setup`.
 
-Setup:
+Basic operations:
 
 .. autosummary::
    :toctree:
 
    login
    logout
    init
    close
    delete
 
-More instance operations:
+Instance operations:
 
 .. autosummary::
    :toctree:
 
    migrate
    register
 
@@ -32,30 +30,30 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.70.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.71.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
-from ._close import close  # noqa
-from ._delete import delete  # noqa
-from ._init_instance import init  # noqa
-from ._connect_instance import connect, load  # noqa
-from ._migrate import migrate
-from ._register_instance import register  # noqa
-from .core._settings import settings  # noqa
-from ._setup_user import login, logout  # noqa
-from ._django import django
 from ._check_setup import _check_instance_setup
+from ._close import close
+from ._connect_instance import connect, load
+from ._delete import delete
+from ._django import django
+from ._init_instance import init
+from ._migrate import migrate
+from ._register_instance import register
+from ._setup_user import login, logout
+from .core._settings import settings
 
 dev = core  # backward compat
 _TESTING = False  # used in lamindb tests
 
 # hide the supabase error in a thread on windows
 if _os_name == "nt":
     if sys.version_info.minor > 7:
@@ -66,7 +64,9 @@
         def _except_hook(args):
             is_overflow = args.exc_type is OverflowError
             for_timeout = str(args.exc_value) == "timeout value is too large"
             if not (is_overflow and for_timeout):
                 _original_excepthook(args)
 
         threading.excepthook = _except_hook
+
+settings.__doc__ = """Global :class:`~lamindb.setup.core.SetupSettings`."""
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.71.0/lamindb_setup/_add_remote_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,39 @@
-from lamin_utils import logger
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
-from lamindb_setup.core.types import UPathStr
+from lamin_utils import logger
 
-from ._init_instance import register_user_and_storage
+from ._init_instance import register_storage_in_instance
 from .core._settings import settings
-from .core._settings_instance import InstanceSettings
-from .core._settings_storage import StorageSettings
+from .core._settings_storage import init_storage
+
+if TYPE_CHECKING:
+    from lamindb_setup.core.types import UPathStr
 
 
-def switch_default_storage(root: UPathStr, **fs_kwargs):
+def add_managed_storage(root: UPathStr, **fs_kwargs):
     """Add a remote default storage location to a local instance.
 
     This can be used to selectively share data.
 
     Args:
         root: `UPathStr` - The new storage root, e.g., an S3 bucket.
         **fs_kwargs: Additional fsspec arguments for cloud root, e.g., profile.
 
-    Example:
-    >>> ln.setup.set.storage(
-    >>>    "s3://some-bucket",
-    >>>     profile="some_profile", # fsspec arg
-    >>>     cache_regions=True # fsspec arg for s3
-    >>> )
-
     """
     if settings.instance.dialect == "sqlite":
-        logger.error("can't set storage for sqlite instances.")
-        return "set-storage-failed"
-    ssettings = StorageSettings(root=root)
-    new_isettings = InstanceSettings(
-        owner=settings.instance.owner,
-        name=settings.instance.name,
-        storage=ssettings,
-        db=settings.instance.db,
-        schema=settings.instance._schema_str,
-        id=settings.instance.id,
+        raise ValueError(
+            "Can't add additional managed storage locations for sqlite instances."
+        )
+    if not settings.instance.is_on_hub:
+        raise ValueError(
+            "Can't add additional managed storage locations for instances that aren't managed through the hub."
+        )
+    ssettings = init_storage(
+        root=root, instance_id=settings.instance._id, register_hub=True
     )
-
-    new_isettings._persist()  # this also updates the settings object
-    register_user_and_storage(new_isettings, settings.user)
-    # we are not doing this for now because of difficulties to define the right RLS policy  # noqa
-    # https://laminlabs.slack.com/archives/C04FPE8V01W/p1687948324601929?thread_ts=1687531921.394119&cid=C04FPE8V01W
-    # if settings.instance.is_remote:
-    #     init_storage_hub(
-    #         root, account_handle=settings.instance.owner  # type: ignore
-    #     )
-
+    settings.instance._storage = ssettings
+    settings.instance._persist()  # this also updates the settings object
+    register_storage_in_instance(ssettings)
     settings.storage._set_fs_kwargs(**fs_kwargs)
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_cache.py` & `lamindb_setup-0.71.0/lamindb_setup/_cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import shutil
+
 from lamin_utils import logger
 
 
 def clear_cache_dir():
-    from lamindb_setup import settings, close
+    from lamindb_setup import close, settings
 
     if settings.instance._is_cloud_sqlite:
         logger.warning(
             "Closing the current instance to update the cloud sqlite database."
         )
         close()
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_check_setup.py` & `lamindb_setup-0.71.0/lamindb_setup/_check_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-from lamin_utils import logger
-from typing import Optional
+from __future__ import annotations
+
 import os
+from typing import TYPE_CHECKING, Optional
+
+from lamin_utils import logger
+
 from ._silence_loggers import silence_loggers
+from .core import django
+from .core._settings import settings
 from .core._settings_store import current_instance_settings_file
 from .core.exceptions import DefaultMessageException
-from .core._settings import settings
-from .core._settings_instance import InstanceSettings
-from .core import django
+
+if TYPE_CHECKING:
+    from .core._settings_instance import InstanceSettings
 
 
 class InstanceNotSetupError(DefaultMessageException):
     default_message = """\
 To use lamindb, you need to connect to an instance.
 
 Connect to an instance: `ln.connect()`. Init an instance: `ln.setup.init()`.
 
 If you used the CLI to set up lamindb in a notebook, restart the Python session.
 """
 
 
-CURRENT_ISETTINGS: Optional[InstanceSettings] = None
+CURRENT_ISETTINGS: InstanceSettings | None = None
 
 
-def _get_current_instance_settings() -> Optional[InstanceSettings]:
+def _get_current_instance_settings() -> InstanceSettings | None:
     global CURRENT_ISETTINGS
 
     if CURRENT_ISETTINGS is not None:
         return CURRENT_ISETTINGS
     if current_instance_settings_file().exists():
         from .core._settings_load import load_instance_settings
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_close.py` & `lamindb_setup-0.71.0/lamindb_setup/_close.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from lamin_utils import logger
 
 from .core._settings import settings
 from .core._settings_store import current_instance_settings_file
 from .core._setup_bionty_sources import delete_bionty_sources_yaml
 from .core.cloud_sqlite_locker import clear_locker
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.71.0/lamindb_setup/_connect_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-from pathlib import Path
-from typing import Optional, Union, Dict, Tuple
-from uuid import UUID
+from __future__ import annotations
+
 import os
+from typing import TYPE_CHECKING
+from uuid import UUID
+
 from lamin_utils import logger
-from lamindb_setup.core.types import UPathStr
-from lamindb_setup.core._hub_utils import (
+
+from ._check_setup import _check_instance_setup
+from ._close import close as close_instance
+from ._init_instance import MESSAGE_NO_MULTIPLE_INSTANCE, load_from_isettings
+from ._migrate import check_whether_migrations_in_sync
+from ._silence_loggers import silence_loggers
+from .core._hub_core import connect_instance as load_instance_from_hub
+from .core._hub_utils import (
     LaminDsn,
     LaminDsnModel,
 )
-from ._close import close as close_instance
-from ._init_instance import load_from_isettings
-from .core._settings import InstanceSettings, settings
-from ._silence_loggers import silence_loggers
+from .core._settings import settings
+from .core._settings_instance import InstanceSettings
 from .core._settings_load import load_instance_settings
 from .core._settings_storage import StorageSettings
 from .core._settings_store import instance_settings_file
 from .core.cloud_sqlite_locker import unlock_cloud_sqlite_upon_exception
-from ._init_instance import MESSAGE_NO_MULTIPLE_INSTANCE
-from ._check_setup import _check_instance_setup
-from .core._hub_core import connect_instance as load_instance_from_hub
-from ._migrate import check_whether_migrations_in_sync
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from .core.types import UPathStr
 
 # this is for testing purposes only
 # set to True only to test failed load
 _TEST_FAILED_LOAD = False
 
 
 INSTANCE_NOT_FOUND_MESSAGE = (
@@ -44,16 +50,16 @@
         and db_dsn_hub.host == db_dsn_local.host
         and db_dsn_hub.database == db_dsn_local.database
         and db_dsn_hub.port == db_dsn_local.port
     )
 
 
 def update_db_using_local(
-    hub_instance_result: Dict[str, str], settings_file: Path, db: Optional[str] = None
-) -> Optional[str]:
+    hub_instance_result: dict[str, str], settings_file: Path, db: str | None = None
+) -> str | None:
     db_updated = None
     # check if postgres
     if hub_instance_result["db_scheme"] == "postgresql":
         db_dsn_hub = LaminDsnModel(db=hub_instance_result["db"])
         if db is not None:
             db_dsn_local = LaminDsnModel(db=db)
         else:
@@ -94,19 +100,19 @@
     return db_updated
 
 
 @unlock_cloud_sqlite_upon_exception(ignore_prev_locker=True)
 def connect(
     slug: str,
     *,
-    db: Optional[str] = None,
-    storage: Optional[UPathStr] = None,
+    db: str | None = None,
+    storage: UPathStr | None = None,
     _raise_not_reachable_error: bool = True,
     _test: bool = False,
-) -> Optional[Union[str, Tuple]]:
+) -> str | tuple | None:
     """Connect to instance.
 
     Args:
         slug: The instance slug `account_handle/instance_name` or URL.
             If the instance is owned by you, it suffices to pass the instance name.
         db: Load the instance with an updated database URL.
         storage: Load the instance with an updated default storage.
@@ -129,15 +135,15 @@
 
         settings_file = instance_settings_file(name, owner)
 
         make_hub_request = True
         if settings_file.exists():
             isettings = load_instance_settings(settings_file)
             # mimic instance_result from hub
-            instance_result = {"id": isettings.id.hex}
+            instance_result = {"id": isettings._id.hex}
             # skip hub request for a purely local instance
             make_hub_request = isettings.is_remote
 
         if make_hub_request:
             # the following will return a string if the instance does not exist
             # on the hub
             hub_result = load_instance_from_hub(owner=owner, name=name)
@@ -157,32 +163,33 @@
                     id=UUID(instance_result["id"]),
                     owner=owner,
                     name=name,
                     storage=ssettings,
                     db=db_updated,
                     schema=instance_result["schema_str"],
                     git_repo=instance_result["git_repo"],
-                    local_storage=instance_result["storage_mode"] == "hybrid",
+                    keep_artifacts_local=bool(instance_result["keep_artifacts_local"]),
+                    is_on_hub=True,
                 )
                 check_whether_migrations_in_sync(instance_result["lamindb_version"])
             else:
                 message = INSTANCE_NOT_FOUND_MESSAGE.format(
                     owner=owner, name=name, hub_result=hub_result
                 )
                 if settings_file.exists():
                     isettings = load_instance_settings(settings_file)
                     if isettings.is_remote:
                         if _raise_not_reachable_error:
                             raise InstanceNotFoundError(message)
-                        return "instance-not-reachable"
+                        return "instance-not-found"
 
                 else:
                     if _raise_not_reachable_error:
                         raise InstanceNotFoundError(message)
-                    return "instance-not-reachable"
+                    return "instance-not-found"
 
         if storage is not None:
             update_isettings_with_storage(isettings, storage)
         isettings._persist()
         if _test:
             return None
         silence_loggers()
@@ -199,15 +206,15 @@
                     f" {isettings._sqlite_file_local}\nTo push the file to the cloud,"
                     " call: lamin close"
                 )
             elif _raise_not_reachable_error:
                 raise SystemExit(msg)
             else:
                 logger.warning(
-                    f"instance exists with id {isettings.id.hex}, but database is not"
+                    f"instance exists with id {isettings._id.hex}, but database is not"
                     " loadable: re-initializing"
                 )
                 return "instance-corrupted-or-deleted", instance_result
         # this is for testing purposes only
         if _TEST_FAILED_LOAD:
             raise RuntimeError("Technical testing error.")
 
@@ -220,17 +227,17 @@
         raise e
     return None
 
 
 def load(
     slug: str,
     *,
-    db: Optional[str] = None,
-    storage: Optional[UPathStr] = None,
-) -> Optional[Union[str, Tuple]]:
+    db: str | None = None,
+    storage: UPathStr | None = None,
+) -> str | tuple | None:
     """Connect to instance and set ``auto-connect`` to true.
 
     This is exactly the same as ``ln.connect()`` except for that
     ``ln.connect()`` doesn't change the state of ``auto-connect``.
     """
     # enable the message in the next release
     logger.warning(
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_delete.py` & `lamindb_setup-0.71.0/lamindb_setup/_delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+from __future__ import annotations
+
 import shutil
-from pathlib import Path
-from lamin_utils import logger
+from typing import TYPE_CHECKING, Optional
 from uuid import UUID
-from typing import Optional
-from .core._settings_instance import InstanceSettings
-from .core._settings_storage import StorageSettings
+
+from lamin_utils import logger
+
+from ._connect_instance import INSTANCE_NOT_FOUND_MESSAGE
+from .core._hub_core import connect_instance as load_instance_from_hub
+from .core._hub_core import delete_instance as delete_instance_on_hub
+from .core._hub_core import get_storage_records_for_instance
 from .core._settings import settings
+from .core._settings_instance import InstanceSettings
 from .core._settings_load import load_instance_settings
+from .core._settings_storage import StorageSettings
 from .core._settings_store import instance_settings_file
-from .core.upath import check_storage_is_empty, hosted_buckets
-from .core._hub_core import delete_instance as delete_instance_on_hub
-from .core._hub_core import connect_instance as load_instance_from_hub
-from ._connect_instance import INSTANCE_NOT_FOUND_MESSAGE
+from .core.upath import HOSTED_BUCKETS, check_storage_is_empty
+
+if TYPE_CHECKING:
+    from pathlib import Path
 
 
 def delete_cache(cache_dir: Path):
     if cache_dir is not None and cache_dir.exists():
         shutil.rmtree(cache_dir)
 
 
 def delete_exclusion_dir(isettings: InstanceSettings) -> None:
-    exclusion_dir = isettings.storage.root / f".lamindb/_exclusion/{isettings.id.hex}"
+    exclusion_dir = isettings.storage.root / f".lamindb/_exclusion/{isettings._id.hex}"
     if exclusion_dir.exists():
         exclusion_dir.rmdir()
 
 
 def delete_by_isettings(isettings: InstanceSettings) -> None:
     settings_file = isettings._get_settings_file()
     if settings_file.exists():
@@ -41,21 +48,19 @@
             )
             pass
     # unset the global instance settings
     if settings._instance_exists and isettings.slug == settings.instance.slug:
         if settings._instance_settings_path.exists():
             settings._instance_settings_path.unlink()
         settings._instance_settings = None
-    if isettings.storage._mark_storage_root.exists():
-        isettings.storage._mark_storage_root.unlink()
 
 
 def delete(
     instance_name: str, force: bool = False, require_empty: bool = True
-) -> Optional[int]:
+) -> int | None:
     """Delete a LaminDB instance.
 
     Args:
         instance_name (str): The name of the instance to delete.
         force (bool): Whether to skip the confirmation prompt.
         require_empty (bool): Whether to check if the instance is empty before deleting.
     """
@@ -90,25 +95,29 @@
                 uid=storage_result["lnid"],
             )
             isettings = InstanceSettings(
                 id=UUID(instance_result["id"]),
                 owner=settings.user.handle,
                 name=instance_name,
                 storage=ssettings,
-                local_storage=instance_result["storage_mode"] == "hybrid",
+                keep_artifacts_local=bool(instance_result["keep_artifacts_local"]),
                 db=instance_result["db"] if "db" in instance_result else None,
                 schema=instance_result["schema_str"],
                 git_repo=instance_result["git_repo"],
             )
         else:
             isettings = load_instance_settings(settings_file)
     if isettings.dialect != "sqlite":
         logger.warning(
             f"delete() does not yet affect your Postgres database at {isettings.db}"
         )
+    if isettings.is_on_hub and settings.user.handle == "anonymous":
+        logger.warning(
+            "won't delete the hub component of this instance because you're not logged in"
+        )
     if not force:
         valid_responses = ["y", "yes"]
         user_input = (
             input(f"Are you sure you want to delete instance {instance_slug}? (y/n) ")
             .strip()
             .lower()
         )
@@ -116,29 +125,53 @@
             return -1
 
     # the actual deletion process begins here
     if isettings.dialect == "sqlite" and isettings.is_remote:
         # delete the exlusion dir first because it's hard to count its objects
         delete_exclusion_dir(isettings)
     if isettings.storage.type_is_cloud and isettings.storage.root_as_str.startswith(
-        hosted_buckets
+        HOSTED_BUCKETS
     ):
         if not require_empty:
             logger.warning(
                 "hosted storage always has to be empty, ignoring `require_empty`"
             )
         require_empty = True
+    # first the default storage
     n_objects = check_storage_is_empty(
         isettings.storage.root,
         raise_error=require_empty,
         account_for_sqlite_file=isettings.dialect == "sqlite",
     )
+    if isettings.storage._mark_storage_root.exists():
+        isettings.storage._mark_storage_root.unlink(
+            missing_ok=True  # this is totally weird, but needed on Py3.11
+        )
+    # now everything that's on the hub
+    if settings.user.handle != "anonymous":
+        storage_records = get_storage_records_for_instance(isettings._id)
+        for storage_record in storage_records:
+            if storage_record["root"] == isettings.storage.root_as_str:
+                continue
+            check_storage_is_empty(
+                storage_record["root"],  # type: ignore
+                raise_error=require_empty,
+            )
+            ssettings = StorageSettings(storage_record["root"])  # type: ignore
+            if ssettings._mark_storage_root.exists():
+                ssettings._mark_storage_root.unlink(
+                    missing_ok=True  # this is totally weird, but needed on Py3.11
+                )
     logger.info(f"deleting instance {instance_slug}")
     # below we can skip check_storage_is_empty() because we already called
     # it above
-    delete_instance_on_hub(isettings.id, require_empty=False)
+    if settings.user.handle != "anonymous":
+        delete_instance_on_hub(isettings._id, require_empty=False)
     delete_by_isettings(isettings)
-    if n_objects == 0 and isettings.storage.type == "local":
+    # if .lndb file was delete, then we might count -1
+    if n_objects <= 0 and isettings.storage.type == "local":
         # dir is only empty after sqlite file was delete via delete_by_isettings
-        (isettings.storage.root / ".lamindb").rmdir()
-        isettings.storage.root.rmdir()
+        if (isettings.storage.root / ".lamindb").exists():
+            (isettings.storage.root / ".lamindb").rmdir()
+        if isettings.storage.root.exists():
+            isettings.storage.root.rmdir()
     return None
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_django.py` & `lamindb_setup-0.71.0/lamindb_setup/_django.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 from typing import Optional
+
 from .core._settings import settings
 from .core.django import setup_django
 
 
-def django(command: str, package_name: Optional[str] = None, **kwargs):
+def django(command: str, package_name: str | None = None, **kwargs):
     r"""Manage migrations.
 
     Examples:
 
     Reset auto-incrementing primary integer ids after a database import:
 
     >>> import lamindb as ln
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_exportdb.py` & `lamindb_setup-0.71.0/lamindb_setup/_exportdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from pathlib import Path
-from importlib import import_module
+from __future__ import annotations
 
+from importlib import import_module
+from pathlib import Path
 
 MODELS = {
     "core": {
         "Collection": False,
         "Artifact": False,
         "Transform": False,
         "Run": True,
@@ -42,14 +43,15 @@
 }
 
 
 def exportdb() -> None:
     directory = Path("./lamindb_export/")
     directory.mkdir(parents=True, exist_ok=True)
     import pandas as pd
+
     import lamindb_setup as ln_setup
 
     def export_registry(registry, directory):
         table_name = registry._meta.db_table
         df = pd.read_sql_table(table_name, ln_setup.settings.instance.db)
         df.to_parquet(directory / f"{table_name}.parquet", compression=None)
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_importdb.py` & `lamindb_setup-0.71.0/lamindb_setup/_importdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
+from importlib import import_module
 from pathlib import Path
+
 from ._exportdb import MODELS
-from importlib import import_module
 
 
 def import_registry(registry, directory, connection):
     import pandas as pd
 
     table_name = registry._meta.db_table
     df = pd.read_parquet(directory / f"{table_name}.parquet")
@@ -22,14 +25,15 @@
     if directory.exists():
         response = input(
             f"\n\nDo you want to import registries from here: {directory}? (y/n)\n"
         )
         if response != "y":
             return None
     from sqlalchemy import create_engine, text
+
     import lamindb_setup as ln_setup
 
     engine = create_engine(ln_setup.settings.instance.db, echo=False)
     with engine.begin() as connection:
         if ln_setup.settings.instance.dialect == "postgresql":
             connection.execute(text("SET CONSTRAINTS ALL DEFERRED;"))
         for schema_name, models in MODELS.items():
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_init_instance.py` & `lamindb_setup-0.71.0/lamindb_setup/_init_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+from __future__ import annotations
+
 import importlib
+import os
 import sys
-from typing import Optional, Union
 import uuid
+from typing import TYPE_CHECKING, Literal
 from uuid import UUID
-import os
-from lamin_utils import logger
-from typing import Tuple, Literal
-from pydantic import PostgresDsn
-from django.db.utils import OperationalError, ProgrammingError
+
 from django.core.exceptions import FieldError
+from django.db.utils import OperationalError, ProgrammingError
+from lamin_utils import logger
+
 from ._close import close as close_instance
-from .core._settings import settings
 from ._silence_loggers import silence_loggers
 from .core import InstanceSettings
-from .core.types import UPathStr
+from .core._settings import settings
 from .core._settings_storage import StorageSettings, init_storage
 from .core.upath import convert_pathlike
 
+if TYPE_CHECKING:
+    from pydantic import PostgresDsn
+
+    from .core.types import UPathStr
+
 
 def get_schema_module_name(schema_name) -> str:
     import importlib.util
 
     name_attempts = [f"lnschema_{schema_name.replace('-', '_')}", schema_name]
     for name in name_attempts:
         module_spec = importlib.util.find_spec(name)
@@ -28,60 +34,66 @@
             return name
     raise ImportError(
         f"Python package for '{schema_name}' is not installed, tried two package names:"
         f" {name_attempts}\nHave you installed the schema package using `pip install`?"
     )
 
 
-def register_storage(ssettings: StorageSettings):
+def register_storage_in_instance(ssettings: StorageSettings):
     from lnschema_core.models import Storage
     from lnschema_core.users import current_user_id
 
-    defaults = dict(
-        root=ssettings.root_as_str,
-        type=ssettings.type,
-        region=ssettings.region,
-        created_by_id=current_user_id(),
-    )
+    from .core.hashing import hash_and_encode_as_b62
+
+    assert ssettings._instance_id is not None
+
+    # how do we ensure that this function is only called passing
+    # the managing instance?
+    defaults = {
+        "root": ssettings.root_as_str,
+        "type": ssettings.type,
+        "region": ssettings.region,
+        "instance_uid": hash_and_encode_as_b62(ssettings._instance_id.hex)[:12],
+        "created_by_id": current_user_id(),
+    }
     if ssettings._uid is not None:
         defaults["uid"] = ssettings._uid
-
-    storage, created = Storage.objects.update_or_create(
+    storage, _ = Storage.objects.update_or_create(
         root=ssettings.root_as_str,
         defaults=defaults,
     )
     return storage
 
 
 def register_user(usettings):
     from lnschema_core.models import User
 
     if usettings.handle != "laminapp-admin":
         try:
             # need to have try except because of integer primary key migration
             user, created = User.objects.update_or_create(
                 uid=usettings.uid,
-                defaults=dict(
-                    handle=usettings.handle,
-                    name=usettings.name,
-                ),
+                defaults={
+                    "handle": usettings.handle,
+                    "name": usettings.name,
+                },
             )
         # for users with only read access, except via ProgrammingError
         # ProgrammingError: permission denied for table lnschema_core_user
         except (OperationalError, FieldError, ProgrammingError):
             pass
 
 
-def register_user_and_storage(isettings: InstanceSettings, usettings):
+def register_user_and_storage_in_instance(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
 
     try:
         register_user(usettings)
-        register_storage(isettings.storage)
+        register_storage_in_instance(isettings.storage)
     except OperationalError as error:
         logger.warning(f"instance seems not set up ({error})")
 
 
 def reload_schema_modules(isettings: InstanceSettings):
     schema_names = ["core"] + list(isettings.schema)
     schema_module_names = [get_schema_module_name(n) for n in schema_names]
@@ -119,19 +131,19 @@
 ERROR_SQLITE_CACHE = """
 Your cached local SQLite file exists, while your cloud SQLite file ({}) doesn't.
 Either delete your cache ({}) or add it back to the cloud (if delete was accidental).
 """
 
 
 def process_connect_response(
-    response: Union[Tuple, str], instance_identifier: str
-) -> Tuple[
+    response: tuple | str, instance_identifier: str
+) -> tuple[
     UUID,
     Literal[
-        "instance-corrupted-or-deleted", "account-not-exists", "instance-not-reachable"
+        "instance-corrupted-or-deleted", "account-not-exists", "instance-not-found"
     ],
 ]:
     # for internal use when creating instances through CICD
     if isinstance(response, tuple) and response[0] == "instance-corrupted-or-deleted":
         hub_result = response[1]
         instance_state = response[0]
         instance_id = UUID(hub_result["id"])
@@ -144,26 +156,26 @@
         instance_state = response
     return instance_id, instance_state
 
 
 def validate_init_args(
     *,
     storage: UPathStr,
-    name: Optional[str] = None,
-    db: Optional[PostgresDsn] = None,
-    schema: Optional[str] = None,
+    name: str | None = None,
+    db: PostgresDsn | None = None,
+    schema: str | None = None,
     _test: bool = False,
-) -> Tuple[
+) -> tuple[
     str,
-    Optional[UUID],
+    UUID | None,
     Literal[
         "connected",
         "instance-corrupted-or-deleted",
         "account-not-exists",
-        "instance-not-reachable",
+        "instance-not-found",
     ],
     str,
 ]:
     from ._connect_instance import connect
     from .core._hub_utils import (
         validate_schema_arg,
     )
@@ -173,15 +185,15 @@
     # test whether instance exists by trying to load it
     instance_slug = f"{settings.user.handle}/{name_str}"
     response = connect(instance_slug, _raise_not_reachable_error=False, _test=_test)
     instance_state: Literal[
         "connected",
         "instance-corrupted-or-deleted",
         "account-not-exists",
-        "instance-not-reachable",
+        "instance-not-found",
     ] = "connected"
     instance_id = None
     if response is not None:
         instance_id, instance_state = process_connect_response(response, instance_slug)
     schema = validate_schema_arg(schema)
     return name_str, instance_id, instance_state, instance_slug
 
@@ -192,17 +204,17 @@
 Try running on the CLI: lamin set auto-connect false
 """
 
 
 def init(
     *,
     storage: UPathStr,
-    name: Optional[str] = None,
-    db: Optional[PostgresDsn] = None,
-    schema: Optional[str] = None,
+    name: str | None = None,
+    db: PostgresDsn | None = None,
+    schema: str | None = None,
     _test: bool = False,
 ) -> None:
     """Create and load a LaminDB instance.
 
     Args:
         storage: Either ``"create-s3"``, local or
             remote folder (``"s3://..."`` or ``"gs://..."``).
@@ -218,25 +230,25 @@
 
         if _check_instance_setup() and not _test:
             raise RuntimeError(MESSAGE_NO_MULTIPLE_INSTANCE)
         else:
             close_instance(mute=True)
         from .core._hub_core import init_instance as init_instance_hub
 
-        name_str, instance_id, instance_state, instance_slug = validate_init_args(
+        name_str, instance_id, instance_state, _ = validate_init_args(
             storage=storage,
             name=name,
             db=db,
             schema=schema,
             _test=_test,
         )
         if instance_state == "connected":
             settings.auto_connect = True  # we can also debate this switch here
             return None
-        ssettings = init_storage(storage)
+        ssettings = init_storage(storage, instance_id=instance_id)
         isettings = InstanceSettings(
             id=instance_id,  # type: ignore
             owner=settings.user.handle,
             name=name_str,
             storage=ssettings,
             db=db,
             schema=schema,
@@ -257,37 +269,37 @@
                 " call: lamin close)"
             )
         # we can debate whether this is the right setting, but this is how
         # things have been and we'd like to not easily break backward compat
         settings.auto_connect = True
     except Exception as e:
         from ._delete import delete_by_isettings
-        from .core._hub_core import delete_storage_record as delete_storage_record
-        from .core._hub_core import delete_instance_record as delete_instance_record
+        from .core._hub_core import delete_instance_record, delete_storage_record
 
         if isettings is not None:
             delete_by_isettings(isettings)
-            delete_instance_record(isettings.id)
+            if settings.user.handle != "anonymous":
+                delete_instance_record(isettings._id)
             isettings._get_settings_file().unlink(missing_ok=True)  # type: ignore
-        if ssettings is not None:
+        if ssettings is not None and settings.user.handle != "anonymous":
             delete_storage_record(ssettings._uuid)  # type: ignore
         raise e
     return None
 
 
 def load_from_isettings(
     isettings: InstanceSettings,
     *,
     init: bool = False,
 ) -> None:
     from .core._setup_bionty_sources import load_bionty_sources, write_bionty_sources
 
     if init:
         # during init both user and storage need to be registered
-        register_user_and_storage(isettings, settings.user)
+        register_user_and_storage_in_instance(isettings, settings.user)
         write_bionty_sources(isettings)
         isettings._update_cloud_sqlite_file(unlock_cloud_sqlite=False)
     else:
         # when loading, django is already set up
         #
         # only register user if the instance is connected
         # for the first time in an environment
@@ -315,16 +327,16 @@
                 )
             )
 
 
 def infer_instance_name(
     *,
     storage: UPathStr,
-    name: Optional[str] = None,
-    db: Optional[PostgresDsn] = None,
+    name: str | None = None,
+    db: PostgresDsn | None = None,
 ) -> str:
     if name is not None:
         if "/" in name:
             raise ValueError("Invalid instance name: '/' delimiter not allowed.")
         return name
     if db is not None:
         logger.warning("using the sql database name for the instance name")
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_migrate.py` & `lamindb_setup-0.71.0/lamindb_setup/_migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Optional, Dict
+from __future__ import annotations
+
+from django.db import connection
+from django.db.migrations.loader import MigrationLoader
 from lamin_utils import logger
 from packaging import version
+
 from ._check_setup import _check_instance_setup
 from .core._settings import settings
 from .core.django import setup_django
-from django.db import connection
-from django.db.migrations.loader import MigrationLoader
 
 
 # for the django-based synching code, see laminhub_rest
 def check_whether_migrations_in_sync(db_version_str: str):
     from importlib import metadata
 
     try:
@@ -64,22 +66,22 @@
         setup_django(settings.instance, create_migrations=True)
 
     @classmethod
     def deploy(cls) -> None:
         """Deploy a migration."""
         if _check_instance_setup():
             raise RuntimeError("Restart Python session to migrate or use CLI!")
+        from lamindb_setup.core._hub_client import call_with_fallback_auth
         from lamindb_setup.core._hub_crud import (
-            update_instance,
-            select_instance_by_id,
             select_collaborator,
+            select_instance_by_id,
+            update_instance,
         )
-        from lamindb_setup.core._hub_client import call_with_fallback_auth
 
-        instance_id_str = settings.instance.id.hex
+        instance_id_str = settings.instance._id.hex
         instance = call_with_fallback_auth(
             select_instance_by_id, instance_id=instance_id_str
         )
         instance_is_on_hub = instance is not None
         if instance_is_on_hub:
             # double check that user is an admin, otherwise will fail below
             # without idempotence
@@ -100,15 +102,15 @@
         # this sets up django and deploys the migrations
         setup_django(settings.instance, deploy_migrations=True)
         # this populates the hub
         if instance_is_on_hub:
             logger.important(f"updating lamindb version in hub: {lamindb.__version__}")
             call_with_fallback_auth(
                 update_instance,
-                instance_id=settings.instance.id.hex,
+                instance_id=settings.instance._id.hex,
                 instance_fields={"lamindb_version": lamindb.__version__},
             )
 
     @classmethod
     def check(cls) -> bool:
         """Check whether Registry definitions are in sync with migrations."""
         from django.core.management import call_command
@@ -122,15 +124,15 @@
                 " migrate create"
             )
             return False
         return True
 
     @classmethod
     def squash(
-        cls, package_name, migration_nr, start_migration_nr: Optional[str] = None
+        cls, package_name, migration_nr, start_migration_nr: str | None = None
     ) -> None:
         """Squash migrations."""
         from django.core.management import call_command
 
         setup_django(settings.instance)
         if start_migration_nr is not None:
             call_command(
@@ -145,17 +147,18 @@
         from django.core.management import call_command
 
         setup_django(settings.instance)
         call_command("showmigrations")
 
     @classmethod
     def defined_migrations(cls, latest: bool = False):
-        from django.core.management import call_command
         from io import StringIO
 
+        from django.core.management import call_command
+
         def parse_migration_output(output):
             """Parse the output of the showmigrations command to get migration names."""
             lines = output.splitlines()
 
             # Initialize an empty dict to store migration names of each module
             migration_names = {}
 
@@ -206,28 +209,28 @@
                     latest_migrations[app] = name
 
             return latest_migrations
         else:
             # Load all migrations using Django's migration loader
             loader = MigrationLoader(connection)
             squashed_replacements = set()
-            for key, migration in loader.disk_migrations.items():
+            for _key, migration in loader.disk_migrations.items():
                 if hasattr(migration, "replaces"):
                     squashed_replacements.update(migration.replaces)
 
-            deployed_migrations: Dict = {}
+            deployed_migrations: dict = {}
             with connection.cursor() as cursor:
                 cursor.execute(
                     """
                     SELECT app, name, deployed
                     FROM django_migrations
                     ORDER BY app, deployed DESC
                 """
                 )
-                for app, name, deployed in cursor.fetchall():
+                for app, name, _deployed in cursor.fetchall():
                     # skip migrations that are part of a squashed migration
                     if (app, name) in squashed_replacements:
                         continue
 
                     if app not in deployed_migrations:
                         deployed_migrations[app] = []
                     deployed_migrations[app].append(name)
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_schema.py` & `lamindb_setup-0.71.0/lamindb_setup/_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from django.urls import path
 from lamin_utils import logger
 
 try:
     from schema_graph.views import Schema
 except ImportError:
     logger.error("to view the schema: pip install django-schema-graph")
@@ -9,16 +11,17 @@
 
 urlpatterns = [
     path("schema/", Schema.as_view()),
 ]
 
 
 def view():
-    from .core.django import setup_django
-    from .core._settings import settings
-    from ._check_setup import _check_instance_setup
     from django.core.management import call_command
 
+    from ._check_setup import _check_instance_setup
+    from .core._settings import settings
+    from .core.django import setup_django
+
     if _check_instance_setup():
         raise RuntimeError("Restart Python session or use CLI!")
     setup_django(settings.instance, view_schema=True)
     call_command("runserver")
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_setup_user.py` & `lamindb_setup-0.71.0/lamindb_setup/_setup_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Union, Optional
+from __future__ import annotations
+
+from typing import Optional, Union
 
 from lamin_utils import logger
 
 from ._check_setup import _check_instance_setup
 from ._init_instance import register_user
 from .core._settings import settings
 from .core._settings_load import load_or_create_user_settings, load_user_settings
 from .core._settings_save import save_user_settings
 from .core._settings_store import (
+    current_user_settings_file,
     user_settings_file_email,
     user_settings_file_handle,
-    current_user_settings_file,
 )
 
 
-def load_user(
-    email: Optional[str] = None, handle: Optional[str] = None
-) -> Union[str, None]:
+def load_user(email: str | None = None, handle: str | None = None) -> str | None:
     if email is not None:
         settings_file = user_settings_file_email(email)
     if handle is not None:
         settings_file = user_settings_file_handle(handle)
     if settings_file.exists():
         user_settings = load_user_settings(settings_file)
         save_user_settings(user_settings)  # needed to save to current_user.env
@@ -42,16 +42,16 @@
 
     return None
 
 
 def login(
     user: str,
     *,
-    key: Optional[str] = None,
-    password: Optional[str] = None,  # for backward compat
+    key: str | None = None,
+    password: str | None = None,  # for backward compat
 ) -> None:
     """Log in user.
 
     Args:
         user: handle or email
         key: API key or legacy passward
         password: Backward compat, will be removed
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.71.0/lamindb_setup/_silence_loggers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import logging
 
 silenced = False
 
 
-# from https://github.com/boto/boto3/blob/8c6e641bed8130a9d8cb4d97b4acbe7aa0d0657a/boto3/__init__.py#L37  # noqa
+# from https://github.com/boto/boto3/blob/8c6e641bed8130a9d8cb4d97b4acbe7aa0d0657a/boto3/__init__.py#L37
 def set_stream_logger(name, level):
     logger = logging.getLogger(name)
     logger.setLevel(level)
     handler = logging.StreamHandler()
     handler.setLevel(level)
     logger.addHandler(handler)
 
@@ -20,15 +22,15 @@
         set_stream_logger(name="botocore.credentials", level=logging.WARNING)
         set_stream_logger(name="botocore.hooks", level=logging.WARNING)
         set_stream_logger(name="botocore.utils", level=logging.WARNING)
         set_stream_logger(name="botocore.auth", level=logging.WARNING)
         set_stream_logger(name="botocore.endpoint", level=logging.WARNING)
         set_stream_logger(name="httpx", level=logging.WARNING)
         try:
-            import aiobotocore  # noqa
+            import aiobotocore
 
             # the 7th logging message of credentials came from aiobotocore
             set_stream_logger(name="aiobotocore.credentials", level=logging.WARNING)
         except ImportError:
             pass
         try:
             # google also aggressively logs authentication related warnings
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_aws_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+
 def get_location(ip="ipinfo.io"):
     import requests  # type: ignore
 
     response = requests.get(f"http://{ip}/json").json()
     loc = response["loc"].split(",")
     return {"latitude": float(loc[0]), "longitude": float(loc[1])}
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_deprecated.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-# BSD 3-Clause License
+from __future__ import annotations
 
+# BSD 3-Clause License
 # Copyright (c) 2017-2018 P. Angerer, F. Alexander Wolf, Theis Lab
 # All rights reserved.
-
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
-
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
-
 # * Redistributions in binary form must reproduce the above copyright notice,
 #   this list of conditions and the following disclaimer in the documentation
 #   and/or other materials provided with the distribution.
-
 # * Neither the name of the copyright holder nor the names of its
 #   contributors may be used to endorse or promote products derived from
 #   this software without specific prior written permission.
-
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 # AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 # IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 import warnings
 from functools import wraps
 
 
 def deprecated(new_name: str):
     """Deprecated.
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_hub_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import os
-from typing import Optional
-from supabase.lib.client_options import ClientOptions
 from urllib.request import urlretrieve
-from supabase import create_client, Client
-from pydantic import BaseSettings
+
 from gotrue.errors import AuthUnknownError
 from lamin_utils import logger
+from pydantic import BaseSettings
+from supabase import Client, create_client  # type: ignore
+from supabase.lib.client_options import ClientOptions
 
 
 class Connector(BaseSettings):
     url: str
     key: str
 
 
@@ -17,15 +19,15 @@
     url = "https://lamin-site-assets.s3.amazonaws.com/connector.env"
     connector_file, _ = urlretrieve(url)
     connector = Connector(_env_file=connector_file)
     return connector
 
 
 PROD_URL = "https://hub.lamin.ai"
-PROD_ANON_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImxhZXNhdW1tZHlkbGxwcGdmY2h1Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2NTY4NDA1NTEsImV4cCI6MTk3MjQxNjU1MX0.WUeCRiun0ExUxKIv5-CtjF6878H8u26t0JmCWx3_2-c"  # noqa
+PROD_ANON_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImxhZXNhdW1tZHlkbGxwcGdmY2h1Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2NTY4NDA1NTEsImV4cCI6MTk3MjQxNjU1MX0.WUeCRiun0ExUxKIv5-CtjF6878H8u26t0JmCWx3_2-c"
 
 
 class Environment:
     def __init__(self, fallback: bool = False):
         lamin_env = os.getenv("LAMIN_ENV")
         if lamin_env is None:
             lamin_env = "prod"
@@ -36,21 +38,21 @@
                 key = PROD_ANON_KEY
             else:
                 connector = load_fallback_connector()
                 url = connector.url
                 key = connector.key
         elif lamin_env == "staging":
             url = "https://amvrvdwndlqdzgedrqdv.supabase.co"
-            key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImFtdnJ2ZHduZGxxZHpnZWRycWR2Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2NzcxNTcxMzMsImV4cCI6MTk5MjczMzEzM30.Gelt3dQEi8tT4j-JA36RbaZuUvxRnczvRr3iyRtzjY0"  # noqa
+            key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImFtdnJ2ZHduZGxxZHpnZWRycWR2Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2NzcxNTcxMzMsImV4cCI6MTk5MjczMzEzM30.Gelt3dQEi8tT4j-JA36RbaZuUvxRnczvRr3iyRtzjY0"
         elif lamin_env == "staging-test":
             url = "https://iugyyajllqftbpidapak.supabase.co"
-            key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Iml1Z3l5YWpsbHFmdGJwaWRhcGFrIiwicm9sZSI6ImFub24iLCJpYXQiOjE2OTQyMjYyODMsImV4cCI6MjAwOTgwMjI4M30.s7B0gMogFhUatMSwlfuPJ95kWhdCZMn1ROhZ3t6Og90"  # noqa
+            key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Iml1Z3l5YWpsbHFmdGJwaWRhcGFrIiwicm9sZSI6ImFub24iLCJpYXQiOjE2OTQyMjYyODMsImV4cCI6MjAwOTgwMjI4M30.s7B0gMogFhUatMSwlfuPJ95kWhdCZMn1ROhZ3t6Og90"
         elif lamin_env == "prod-test":
             url = "https://xtdacpwiqwpbxsatoyrv.supabase.co"
-            key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Inh0ZGFjcHdpcXdwYnhzYXRveXJ2Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2OTQyMjYxNDIsImV4cCI6MjAwOTgwMjE0Mn0.Dbi27qujTt8Ei9gfp9KnEWTYptE5KUbZzEK6boL46k4"  # noqa
+            key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Inh0ZGFjcHdpcXdwYnhzYXRveXJ2Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2OTQyMjYxNDIsImV4cCI6MjAwOTgwMjE0Mn0.Dbi27qujTt8Ei9gfp9KnEWTYptE5KUbZzEK6boL46k4"
         else:
             url = os.environ["SUPABASE_API_URL"]
             key = os.environ["SUPABASE_ANON_KEY"]
         self.lamin_env: str = lamin_env
         self.supabase_api_url: str = url
         self.supabase_anon_key: str = key
 
@@ -62,15 +64,15 @@
     env = Environment(fallback=fallback_env)
     return create_client(env.supabase_api_url, env.supabase_anon_key, client_options)
 
 
 def connect_hub_with_auth(
     fallback_env: bool = False,
     renew_token: bool = False,
-    access_token: Optional[str] = None,
+    access_token: str | None = None,
 ) -> Client:
     hub = connect_hub(fallback_env=fallback_env)
     if access_token is None:
         from lamindb_setup import settings
 
         if renew_token:
             settings.user.access_token = get_access_token(
@@ -79,15 +81,15 @@
         access_token = settings.user.access_token
     hub.postgrest.auth(access_token)
     hub.functions.set_auth(access_token)
     return hub
 
 
 # runs ~0.5s
-def get_access_token(email: Optional[str] = None, password: Optional[str] = None):
+def get_access_token(email: str | None = None, password: str | None = None):
     hub = connect_hub()
     try:
         auth_response = hub.auth.sign_in_with_password(
             {
                 "email": email,
                 "password": password,
             }
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_hub_core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,240 @@
+from __future__ import annotations
+
+import json
 import os
-from typing import Optional, Tuple, Union, Dict
 import uuid
-from postgrest.exceptions import APIError
-from uuid import UUID
-from lamin_utils import logger
-from supabase import Client
-import lamindb_setup
-import json
 from importlib import metadata
-from ._settings_instance import InstanceSettings
-from ._settings_storage import StorageSettings, base62
+from typing import TYPE_CHECKING
+from uuid import UUID
 
+from lamin_utils import logger
+from postgrest.exceptions import APIError
 
 from ._hub_client import (
-    connect_hub,
-    call_with_fallback_auth,
     call_with_fallback,
+    call_with_fallback_auth,
+    connect_hub,
 )
 from ._hub_crud import (
-    select_instance_by_owner_name,
-    select_instance_by_id_with_storage,
+    _delete_instance_record,
     select_account_by_handle,
     select_db_user_by_instance,
+    select_instance_by_id_with_storage,
     select_instance_by_name,
+    select_instance_by_owner_name,
     select_storage,
-    _delete_instance_record,
 )
+from ._hub_crud import update_instance as _update_instance_record
 from ._hub_utils import (
     LaminDsn,
     LaminDsnModel,
 )
+from ._settings import settings
+from ._settings_storage import StorageSettings, base62
+
+if TYPE_CHECKING:
+    from supabase import Client  # type: ignore
+
+    from ._settings_instance import InstanceSettings
 
 
 def delete_storage_record(
     storage_uuid: UUID,
 ) -> None:
     return call_with_fallback_auth(
         _delete_storage_record,
         storage_uuid=storage_uuid,
     )
 
 
 def _delete_storage_record(storage_uuid: UUID, client: Client) -> None:
     if storage_uuid is None:
         return None
-    logger.important(f"deleting storage {storage_uuid.hex}")
-    client.table("storage").delete().eq("id", storage_uuid.hex).execute()
+    response = client.table("storage").delete().eq("id", storage_uuid.hex).execute()
+    if response.data:
+        logger.important(f"deleted storage record on hub {storage_uuid.hex}")
 
 
-def update_instance_record(instance_uuid: UUID, fields: Dict) -> None:
-    from ._hub_crud import update_instance
+def update_instance_record(instance_uuid: UUID, fields: dict) -> None:
+    return call_with_fallback_auth(
+        _update_instance_record, instance_id=instance_uuid.hex, instance_fields=fields
+    )
+
 
+def get_storage_records_for_instance(
+    instance_id: UUID,
+) -> list[dict[str, str | int]]:
     return call_with_fallback_auth(
-        update_instance, instance_id=instance_uuid.hex, instance_fields=fields
+        _get_storage_records_for_instance,
+        instance_id=instance_id,
+    )
+
+
+def _get_storage_records_for_instance(
+    instance_id: UUID, client: Client
+) -> list[dict[str, str | int]]:
+    response = (
+        client.table("storage").select("*").eq("instance_id", instance_id.hex).execute()
     )
+    return response.data
+
+
+def _select_storage(
+    ssettings: StorageSettings, update_uid: bool, client: Client
+) -> bool:
+    root = ssettings.root_as_str
+    response = client.table("storage").select("*").eq("root", root).execute()
+    if not response.data:
+        return False
+    else:
+        existing_storage = response.data[0]
+        if ssettings._instance_id is not None:
+            # consider storage settings that are meant to be managed by an instance
+            if UUID(existing_storage["instance_id"]) != ssettings._instance_id:
+                # everything is alright if the instance_id matches
+                # we're probably just switching storage locations
+                # below can be turned into a warning and then delegate the error
+                # to a unique constraint violation below
+                raise ValueError(
+                    f"Storage root {root} is already managed by instance {existing_storage['instance_id']}."
+                )
+        else:
+            # if the request is agnostic of the instance, that's alright,
+            # we'll update the instance_id with what's stored in the hub
+            ssettings._instance_id = UUID(existing_storage["instance_id"])
+        ssettings._uuid_ = UUID(existing_storage["id"])
+        if update_uid:
+            ssettings._uid = existing_storage["lnid"]
+        else:
+            assert ssettings._uid == existing_storage["lnid"]
+        return True
 
 
 def init_storage(
     ssettings: StorageSettings,
-) -> UUID:
-    return call_with_fallback_auth(
-        _init_storage,
-        ssettings=ssettings,
-    )
+) -> None:
+    if settings.user.handle != "anonymous":
+        return call_with_fallback_auth(
+            _init_storage,
+            ssettings=ssettings,
+        )
+    else:
+        storage_exists = call_with_fallback(
+            _select_storage, ssettings=ssettings, update_uid=True
+        )
+        if storage_exists:
+            return None
+        else:
+            raise ValueError("Log in to create a storage location on the hub.")
 
 
-def _init_storage(ssettings: StorageSettings, client: Client) -> UUID:
+def _init_storage(ssettings: StorageSettings, client: Client) -> None:
     from lamindb_setup import settings
 
     # storage roots are always stored without the trailing slash in the SQL
     # database
     root = ssettings.root_as_str
-    # in the future, we could also encode a prefix to model local storage
-    # locations
-    # f"{prefix}{root}"
-    id = uuid.uuid5(uuid.NAMESPACE_URL, root)
-    fields = dict(
-        id=id.hex,
-        lnid=ssettings.uid,
-        created_by=settings.user._uuid.hex,  # type: ignore
-        root=root,
-        region=ssettings.region,
-        type=ssettings.type,
-        aws_account_id=ssettings._aws_account_id,
-        description=ssettings._description,
-    )
+    if _select_storage(ssettings, update_uid=True, client=client):
+        return None
+    if ssettings.type_is_cloud:
+        id = uuid.uuid5(uuid.NAMESPACE_URL, root)
+    else:
+        id = uuid.uuid4()
+    if ssettings._instance_id is None:
+        logger.warning(
+            f"will manage storage location {ssettings.root_as_str} with instance {settings.instance.slug}"
+        )
+        ssettings._instance_id = settings.instance._id
+    fields = {
+        "id": id.hex,
+        "lnid": ssettings.uid,
+        "created_by": settings.user._uuid.hex,  # type: ignore
+        "root": root,
+        "region": ssettings.region,
+        "type": ssettings.type,
+        "instance_id": ssettings._instance_id.hex,
+        # the empty string is important as we want the user flow to be through LaminHub
+        # if this errors with unique constraint error, the user has to update
+        # the description in LaminHub
+        "description": "",
+    }
+    # TODO: add error message for violated unique constraint
+    # on root & description
     client.table("storage").upsert(fields).execute()
-    return id
+    ssettings._uuid_ = id
+    return None
 
 
-def delete_instance(identifier: Union[UUID, str], require_empty: bool = True) -> None:
+def delete_instance(identifier: UUID | str, require_empty: bool = True) -> str | None:
+    return call_with_fallback_auth(
+        _delete_instance, identifier=identifier, require_empty=require_empty
+    )
+
+
+def _delete_instance(
+    identifier: UUID | str, require_empty: bool, client: Client
+) -> str | None:
     """Fully delete an instance in the hub.
 
     This function deletes the relevant instance and storage records in the hub,
     conditional on the emptiness of the storage location.
     """
-    from .upath import check_storage_is_empty, create_path
     from ._settings_storage import mark_storage_root
+    from .upath import check_storage_is_empty, create_path
 
-    if isinstance(identifier, UUID):
-        instance_with_storage = call_with_fallback_auth(
-            select_instance_by_id_with_storage,
-            instance_id=identifier,
+    # the "/" check is for backward compatibility with the old identifier format
+    if isinstance(identifier, UUID) or "/" not in identifier:
+        if isinstance(identifier, UUID):
+            instance_id_str = identifier.hex
+        else:
+            instance_id_str = identifier
+        instance_with_storage = select_instance_by_id_with_storage(
+            instance_id=instance_id_str, client=client
         )
     else:
         owner, name = identifier.split("/")
-        instance_with_storage = call_with_fallback_auth(
-            select_instance_by_owner_name,
-            owner=owner,
-            name=name,
+        instance_with_storage = select_instance_by_owner_name(
+            owner=owner, name=name, client=client
         )
 
     if instance_with_storage is None:
-        logger.warning("instance not found")
-        return None
+        logger.important("not deleting instance from hub as instance not found there")
+        return "instance-not-found"
 
+    storage_records = _get_storage_records_for_instance(
+        UUID(instance_with_storage["id"]),
+        client,
+    )
     if require_empty:
-        root_string = instance_with_storage["storage"]["root"]
-        # gate storage and instance deletion on empty storage location for
-        root_path = create_path(root_string)
-        mark_storage_root(root_path)  # address permission error
-        account_for_sqlite_file = instance_with_storage["db_scheme"] is None
-        check_storage_is_empty(
-            root_path, account_for_sqlite_file=account_for_sqlite_file
-        )
-    delete_instance_record(UUID(instance_with_storage["id"]))
-    delete_storage_record(UUID(instance_with_storage["storage_id"]))
+        for storage_record in storage_records:
+            account_for_sqlite_file = (
+                instance_with_storage["db_scheme"] is None
+                and instance_with_storage["storage"]["root"] == storage_record["root"]
+            )
+            root_string = storage_record["root"]
+            # gate storage and instance deletion on empty storage location for
+            if client.auth.get_session() is not None:
+                access_token = client.auth.get_session().access_token
+            else:
+                access_token = None
+            root_path = create_path(root_string, access_token)
+            mark_storage_root(
+                root_path,
+                storage_record["lnid"],  # type: ignore
+            )  # address permission error
+            check_storage_is_empty(
+                root_path, account_for_sqlite_file=account_for_sqlite_file
+            )
+    _update_instance_record(instance_with_storage["id"], {"storage_id": None}, client)
+    # first delete the storage records because we will turn instance_id on
+    # storage into a FK soon
+    for storage_record in storage_records:
+        _delete_storage_record(UUID(storage_record["id"]), client)  # type: ignore
+    _delete_instance_record(UUID(instance_with_storage["id"]), client)
     return None
 
 
 def delete_instance_record(
     instance_id: UUID,
 ) -> None:
     return call_with_fallback_auth(
@@ -145,73 +250,76 @@
 def _init_instance(isettings: InstanceSettings, client: Client) -> None:
     from ._settings import settings
 
     try:
         lamindb_version = metadata.version("lamindb")
     except metadata.PackageNotFoundError:
         lamindb_version = None
-    fields = dict(
-        id=isettings.id.hex,
-        account_id=settings.user._uuid.hex,  # type: ignore
-        name=isettings.name,
-        storage_id=isettings.storage._uuid.hex,  # type: ignore
-        schema_str=isettings._schema_str,
-        lamindb_version=lamindb_version,
-        public=False,
-    )
+    fields = {
+        "id": isettings._id.hex,
+        "account_id": settings.user._uuid.hex,  # type: ignore
+        "name": isettings.name,
+        "storage_id": isettings.storage._uuid.hex,  # type: ignore
+        "lnid": isettings.uid,
+        "schema_str": isettings._schema_str,
+        "lamindb_version": lamindb_version,
+        "public": False,
+    }
     if isettings.dialect != "sqlite":
         db_dsn = LaminDsnModel(db=isettings.db)
-        fields.update(
-            {
-                "db_scheme": db_dsn.db.scheme,
-                "db_host": db_dsn.db.host,
-                "db_port": db_dsn.db.port,
-                "db_database": db_dsn.db.database,
-            }
-        )
+        db_fields = {
+            "db_scheme": db_dsn.db.scheme,
+            "db_host": db_dsn.db.host,
+            "db_port": db_dsn.db.port,
+            "db_database": db_dsn.db.database,
+        }
+        fields.update(db_fields)
     # I'd like the following to be an upsert, but this seems to violate RLS
     # Similarly, if we don't specify `returning="minimal"`, we'll violate RLS
     # we could make this idempotent by catching an error, but this seems dangerous
     # as then init_instance is no longer idempotent
     try:
         client.table("instance").insert(fields, returning="minimal").execute()
     except APIError as e:
         logger.warning("instance likely already exists")
         raise e
+    client.table("storage").update(
+        {"instance_id": isettings._id.hex, "is_default": True}
+    ).eq("id", isettings.storage._uuid.hex).execute()  # type: ignore
     logger.save(f"browse to: https://lamin.ai/{isettings.owner}/{isettings.name}")
 
 
 def connect_instance(
     *,
     owner: str,  # account_handle
     name: str,  # instance_name
-) -> Union[Tuple[dict, dict], str]:
+) -> tuple[dict, dict] | str:
     from ._settings import settings
 
     if settings.user.handle != "anonymous":
         return call_with_fallback_auth(_connect_instance, owner=owner, name=name)
     else:
         return call_with_fallback(_connect_instance, owner=owner, name=name)
 
 
 def _connect_instance(
     *,
     owner: str,  # account_handle
     name: str,  # instance_name
     client: Client,
-) -> Union[Tuple[dict, dict], str]:
+) -> tuple[dict, dict] | str:
     instance_account_storage = select_instance_by_owner_name(owner, name, client)
     if instance_account_storage is None:
         # try the via single requests, will take more time
         account = select_account_by_handle(owner, client)
         if account is None:
             return "account-not-exists"
         instance = select_instance_by_name(account["id"], name, client)
         if instance is None:
-            return "instance-not-reachable"
+            return "instance-not-found"
         # get default storage
         storage = select_storage(instance["storage_id"], client)
         if storage is None:
             return "storage-does-not-exist-on-hub"
     else:
         account = instance_account_storage.pop("account")
         storage = instance_account_storage.pop("storage")
@@ -234,27 +342,29 @@
             port=instance["db_port"],
             database=instance["db_database"],
         )
         instance["db"] = db_dsn
     return instance, storage
 
 
-def access_aws(storage_root: str, access_token: Optional[str] = None) -> Dict[str, str]:
+def access_aws(storage_root: str, access_token: str | None = None) -> dict[str, str]:
     from ._settings import settings
 
     if settings.user.handle != "anonymous" or access_token is not None:
         credentials = call_with_fallback_auth(
             _access_aws, storage_root=storage_root, access_token=access_token
         )
         return credentials
     else:
         raise RuntimeError("Can only get access to AWS if authenticated.")
 
 
-def _access_aws(*, storage_root: str, client: Client) -> Dict[str, str]:
+def _access_aws(*, storage_root: str, client: Client) -> dict[str, str]:
+    import lamindb_setup
+
     response = client.functions.invoke(
         "access-aws",
         invoke_options={"body": {"storage_root": storage_root}},
     )
     if response is not None and response != b"{}":
         loaded_credentials = json.loads(response)["Credentials"]
         credentials = {}
@@ -272,29 +382,29 @@
         if os.environ["LAMIN_ENV"] == "local":
             return "http://localhost:3000"
         elif os.environ["LAMIN_ENV"] == "staging":
             return "https://staging.lamin.ai"
     return "https://lamin.ai"
 
 
-def sign_up_local_hub(email) -> Union[str, Tuple[str, str, str]]:
+def sign_up_local_hub(email) -> str | tuple[str, str, str]:
     # raises gotrue.errors.AuthApiError: User already registered
     password = base62(40)  # generate new password
     sign_up_kwargs = {"email": email, "password": password}
     client = connect_hub()
     auth_response = client.auth.sign_up(sign_up_kwargs)
     client.auth.sign_out()
     return (
         password,
         auth_response.session.user.id,
         auth_response.session.access_token,
     )
 
 
-def _sign_in_hub(email: str, password: str, handle: Optional[str], client: Client):
+def _sign_in_hub(email: str, password: str, handle: str | None, client: Client):
     auth = client.auth.sign_in_with_password(
         {
             "email": email,
             "password": password,
         }
     )
     data = client.table("account").select("*").eq("id", auth.user.id).execute().data
@@ -316,16 +426,16 @@
         user_handle,
         user_name,
         auth.session.access_token,
     )
 
 
 def sign_in_hub(
-    email: str, password: str, handle: Optional[str] = None
-) -> Union[Exception, Tuple[UUID, str, str, str, str]]:
+    email: str, password: str, handle: str | None = None
+) -> Exception | tuple[UUID, str, str, str, str]:
     try:
         result = call_with_fallback(
             _sign_in_hub, email=email, password=password, handle=handle
         )
     except Exception as exception:  # this is bad, but I don't find APIError right now
         logger.error(exception)
         logger.error(
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_hub_crud.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from supabase.client import Client
-from typing import Optional, Dict
-from lamin_utils import logger
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 from uuid import UUID, uuid4
 
+from lamin_utils import logger
+from supabase.client import Client  # noqa
+
 
 def select_instance_by_owner_name(
     owner: str,
     name: str,
     client: Client,
-) -> Optional[Dict]:
+) -> dict | None:
     try:
         data = (
             client.table("instance")
             .select(
                 "*, account!inner!instance_account_id_28936e8f_fk_account_id(*),"
-                " storage(*)"
+                " storage!instance_storage_id_87963cc8_fk_storage_id(*)"
             )
             .eq("account.handle", owner)
             .eq("name", name)
             .execute()
             .data
         )
     except Exception:
@@ -78,15 +81,18 @@
 
 
 def select_instance_by_id_with_storage(
     instance_id: str,
     client: Client,
 ):
     response = (
-        client.table("instance").select("*, storage(*)").eq("id", instance_id).execute()
+        client.table("instance")
+        .select("*, storage!instance_storage_id_87963cc8_fk_storage_id(*)")
+        .eq("id", instance_id)
+        .execute()
     )
     if len(response.data) == 0:
         return None
     return response.data[0]
 
 
 def update_instance(instance_id: str, instance_fields: dict, client: Client):
@@ -174,12 +180,10 @@
         logger.warning("found multiple db credentials, using the first one")
     return data[0]
 
 
 def _delete_instance_record(instance_id: UUID, client: Client) -> None:
     if not isinstance(instance_id, UUID):
         instance_id = UUID(instance_id)
-    logger.important(f"deleting instance {instance_id.hex}")
-    client.table("instance").delete().eq("id", instance_id.hex).execute()
-
-
-sb_delete_instance = _delete_instance_record
+    response = client.table("instance").delete().eq("id", instance_id.hex).execute()
+    if response.data:
+        logger.important(f"deleted instance record on hub {instance_id.hex}")
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_hub_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+from __future__ import annotations
+
 from typing import Optional
+
 from pydantic import BaseModel, validator
 from pydantic.networks import MultiHostDsn
 
 
-def validate_schema_arg(schema: Optional[str] = None) -> str:
+def validate_schema_arg(schema: str | None = None) -> str:
     if schema is None or schema == "":
         return ""
     # currently no actual validation, can add back if we see a need
     # the following just strips white spaces
     to_be_validated = [s.strip() for s in schema.split(",")]
     return ",".join(to_be_validated)
 
 
-def validate_db_arg(db: Optional[str]) -> None:
+def validate_db_arg(db: str | None) -> None:
     if db is not None:
         LaminDsnModel(db=db)
 
 
 class LaminDsn(MultiHostDsn):
     """Custom DSN Type for Lamin.
 
@@ -39,21 +42,21 @@
         return self.path[1:]
 
     @classmethod
     def build(
         cls,
         *,
         scheme: str,
-        user: Optional[str] = None,
-        password: Optional[str] = None,
+        user: str | None = None,
+        password: str | None = None,
         host: str,
-        port: Optional[str] = None,
-        database: Optional[str] = None,
-        query: Optional[str] = None,
-        fragment: Optional[str] = None,
+        port: str | None = None,
+        database: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
         **_kwargs: str,
     ) -> str:
         return super().build(
             scheme=scheme,
             user=user,
             password=password,
             host=host,
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+from __future__ import annotations
+
 import os
-from typing import Union, Optional
-from lamindb_setup.core import InstanceSettings, StorageSettings, UserSettings
-from lamindb_setup.core._settings_load import (
+from typing import TYPE_CHECKING
+
+from ._settings_load import (
     load_instance_settings,
     load_or_create_user_settings,
 )
-from ._settings_store import current_instance_settings_file
-from pathlib import Path
-from ._settings_store import settings_dir
+from ._settings_store import current_instance_settings_file, settings_dir
 
+if TYPE_CHECKING:
+    from pathlib import Path
 
-class SetupSettings:
-    """Setup settings.
+    from lamindb_setup.core import InstanceSettings, StorageSettings, UserSettings
 
-    - :class:`~lamindb_setup.core.InstanceSettings`
-    - :class:`~lamindb_setup.core.StorageSettings`
-    - :class:`~lamindb_setup.core.UserSettings`
-    """
 
-    _using_key: Optional[str] = None  # set through lamindb.settings
+class SetupSettings:
+    """Setup settings."""
 
-    _user_settings: Union[UserSettings, None] = None
-    _instance_settings: Union[InstanceSettings, None] = None
+    _using_key: str | None = None  # set through lamindb.settings
 
-    _user_settings_env: Union[str, None] = None
-    _instance_settings_env: Union[str, None] = None
+    _user_settings: UserSettings | None = None
+    _instance_settings: InstanceSettings | None = None
+
+    _user_settings_env: str | None = None
+    _instance_settings_env: str | None = None
 
     _auto_connect_path: Path = settings_dir / "auto_connect"
 
     @property
     def _instance_settings_path(self) -> Path:
         return current_instance_settings_file()
 
@@ -46,45 +46,42 @@
         if value:
             self._auto_connect_path.touch()
         else:
             self._auto_connect_path.unlink(missing_ok=True)
 
     @property
     def user(self) -> UserSettings:
-        """User."""
-        if (
-            self._user_settings is None
-            or self._user_settings_env != get_env_name()  # noqa
-        ):
+        """:class:`~lamindb.setup.core.UserSettings`."""
+        if self._user_settings is None or self._user_settings_env != get_env_name():
             self._user_settings = load_or_create_user_settings()
             self._user_settings_env = get_env_name()
             if self._user_settings and self._user_settings.uid is None:
                 raise RuntimeError("Need to login, first: lamin login <email>")
         return self._user_settings  # type: ignore
 
     @property
     def instance(self) -> InstanceSettings:
-        """Instance."""
+        """:class:`~lamindb.setup.core.InstanceSettings`."""
         if (
             self._instance_settings is None
-            or self._instance_settings_env != get_env_name()  # noqa
+            or self._instance_settings_env != get_env_name()
         ):
             self._instance_settings = load_instance_settings()
             self._instance_settings_env = get_env_name()
         return self._instance_settings  # type: ignore
 
     @property
     def storage(self) -> StorageSettings:
-        """Storage."""
+        """:class:`~lamindb.setup.core.StorageSettings`."""
         return self.instance.storage
 
     @property
     def _instance_exists(self):
         try:
-            self.instance
+            self.instance  # noqa
             return True
         # this is implicit logic that catches if no instance is loaded
         except SystemExit:
             return False
 
     def __repr__(self) -> str:
         """Rich string representation."""
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings_instance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from __future__ import annotations
 
 import os
 import shutil
-from .upath import LocalPathClasses, convert_pathlike
 from pathlib import Path
-from typing import Literal, Optional, Set, Tuple
-from uuid import UUID
+from typing import TYPE_CHECKING, Literal
+
+from lamin_utils import logger
+
 from ._hub_client import call_with_fallback
 from ._hub_crud import select_account_handle_name_by_lnid
-from lamin_utils import logger
+from ._hub_utils import LaminDsn, LaminDsnModel
+from ._settings_save import save_instance_settings
+from ._settings_storage import StorageSettings, init_storage, mark_storage_root
+from ._settings_store import current_instance_settings_file, instance_settings_file
 from .cloud_sqlite_locker import (
-    InstanceLockedException,
     EXPIRATION_TIME,
+    InstanceLockedException,
 )
-from ._hub_utils import LaminDsnModel, LaminDsn
-from ._settings_save import save_instance_settings
-from ._settings_storage import StorageSettings
-from ._settings_store import current_instance_settings_file, instance_settings_file
-from .upath import UPath
+from .upath import LocalPathClasses, UPath, convert_pathlike
 
-LOCAL_STORAGE_ROOT_WARNING = (
-    "No local storage root found, set via `ln.setup.settings.instance.local_storage ="
-    " local_root`"
-)
+if TYPE_CHECKING:
+    from uuid import UUID
 
 
 def sanitize_git_repo_url(repo_url: str) -> str:
     assert repo_url.startswith("https://")
     return repo_url.replace(".git", "")
 
 
@@ -35,34 +33,36 @@
 
     def __init__(
         self,
         id: UUID,  # instance id/uuid
         owner: str,  # owner handle
         name: str,  # instance name
         storage: StorageSettings,  # storage location
-        local_storage: bool = False,  # default to local storage
-        uid: Optional[str] = None,  # instance uid/lnid
-        db: Optional[str] = None,  # DB URI
-        schema: Optional[str] = None,  # comma-separated string of schema names
-        git_repo: Optional[str] = None,  # a git repo URL
+        keep_artifacts_local: bool = False,  # default to local storage
+        uid: str | None = None,  # instance uid/lnid
+        db: str | None = None,  # DB URI
+        schema: str | None = None,  # comma-separated string of schema names
+        git_repo: str | None = None,  # a git repo URL
+        is_on_hub: bool = False,  # initialized from hub
     ):
         from ._hub_utils import validate_db_arg
 
-        self._id: UUID = id
+        self._id_: UUID = id
         self._owner: str = owner
         self._name: str = name
-        self._uid: Optional[str] = uid
+        self._uid: str | None = uid
         self._storage: StorageSettings = storage
         validate_db_arg(db)
-        self._db: Optional[str] = db
-        self._schema_str: Optional[str] = schema
+        self._db: str | None = db
+        self._schema_str: str | None = schema
         self._git_repo = None if git_repo is None else sanitize_git_repo_url(git_repo)
         # local storage
-        self._local_storage_on = local_storage
-        self._local_storage = None
+        self._keep_artifacts_local = keep_artifacts_local
+        self._storage_local: StorageSettings | None = None
+        self._is_on_hub = is_on_hub
 
     def __repr__(self):
         """Rich string representation."""
         representation = f"Current instance: {self.slug}"
         attrs = ["owner", "name", "storage", "db", "schema", "git_repo"]
         for attr in attrs:
             value = getattr(self, attr)
@@ -93,104 +93,157 @@
         return self._owner
 
     @property
     def name(self) -> str:
         """Instance name."""
         return self._name
 
-    def _search_local_root(self):
+    def _search_local_root(
+        self, local_root: str | None = None, mute_warning: bool = False
+    ) -> StorageSettings | None:
         from lnschema_core.models import Storage
 
-        records = Storage.objects.filter(type="local").all()
-        for record in records:
-            if Path(record.root).exists():
-                self._local_storage = StorageSettings(record.root)
-                logger.important(f"defaulting to local storage: {record}")
-                break
-        if self._local_storage is None:
-            logger.warning(LOCAL_STORAGE_ROOT_WARNING)
-
-    @property
-    def local_storage(self) -> StorageSettings:
-        """Default local storage.
-
-        Warning: Only enable if you're sure you want to use the more complicated
-        storage mode across local & cloud locations.
-
-        As an admin, enable via: `ln.setup.settings.instance.local_storage =
-        local_root`.
-
-        If enabled, you'll save artifacts to a default local storage
-        location at :attr:`~lamindb.setup.settings.InstanceSettings.local_storage`.
-
-        Upon passing `upload=True` in `artifact.save(upload=True)`, you upload the
-        artifact to the default cloud storage location:
-        :attr:`~lamindb.setup.core.InstanceSettings.storage`.
-        """
-        if not self._local_storage_on:
-            raise ValueError("Local storage is not enabled for this instance.")
-        if self._local_storage is None:
-            self._search_local_root()
-        if self._local_storage is None:
-            raise ValueError(LOCAL_STORAGE_ROOT_WARNING)
-        return self._local_storage
-
-    @local_storage.setter
-    def local_storage(self, local_root: Path):
-        from ._hub_core import update_instance_record
-        from .._init_instance import register_storage
-
-        self._search_local_root()
-        if self._local_storage is not None:
-            raise ValueError(
-                "You already configured a local storage root for this instance in this"
-                f" environment: {self.local_storage.root}"
+        if local_root is not None:
+            local_records = Storage.objects.filter(root=local_root)
+        else:
+            local_records = Storage.objects.filter(type="local")
+        found = False
+        for record in local_records.all():
+            root_path = Path(record.root)
+            if root_path.exists():
+                marker_path = root_path / ".lamindb/_is_initialized"
+                if marker_path.exists():
+                    uid = marker_path.read_text()
+                    if uid == record.uid:
+                        found = True
+                        break
+                    elif uid == "":
+                        # legacy instance that was not yet marked properly
+                        mark_storage_root(record.root, record.uid)
+                    else:
+                        continue
+                else:
+                    # legacy instance that was not yet marked at all
+                    mark_storage_root(record.root, record.uid)
+                    break
+        if found:
+            return StorageSettings(record.root)
+        elif not mute_warning:
+            logger.warning(
+                f"none of the registered local storage locations were found in your environment: {local_records}"
+                "\n❗ please register a new local storage location via `ln.settings.storage_local = local_root_path` "
+                "and re-load/connect the instance"
             )
+        return None
+
+    @property
+    def keep_artifacts_local(self) -> bool:
+        """Default to keeping artifacts local.
+
+        Enable this optional setting for cloud instances on lamin.ai.
+
+        Guide: :doc:`faq/keep-artifacts-local`
+        """
+        return self._keep_artifacts_local
+
+    @property
+    def storage(self) -> StorageSettings:
+        """Default storage.
+
+        For a cloud instance, this is cloud storage. For a local instance, this
+        is a local directory.
+        """
+        return self._storage
+
+    @property
+    def storage_local(self) -> StorageSettings:
+        """An additional local default storage.
+
+        Is only available if :attr:`keep_artifacts_local` is enabled.
+
+        Guide: :doc:`faq/keep-artifacts-local`
+        """
+        if not self._keep_artifacts_local:
+            raise ValueError("`keep_artifacts_local` is not enabled for this instance.")
+        if self._storage_local is None:
+            self._storage_local = self._search_local_root()
+        if self._storage_local is None:
+            # raise an error, there was a warning just before in search_local_root
+            raise ValueError()
+        return self._storage_local
+
+    @storage_local.setter
+    def storage_local(self, local_root: Path | str):
+        from lamindb_setup._init_instance import register_storage_in_instance
+
+        local_root = Path(local_root)
+        if not self._keep_artifacts_local:
+            raise ValueError("`keep_artifacts_local` is not enabled for this instance.")
+        storage_local = self._search_local_root(
+            local_root=StorageSettings(local_root).root_as_str, mute_warning=True
+        )
+        if storage_local is not None:
+            # great, we're merely switching storage location
+            self._storage_local = storage_local
+            logger.important(f"defaulting to local storage: {storage_local.root}")
+            return None
+        storage_local = self._search_local_root(mute_warning=True)
+        if storage_local is not None:
+            if os.getenv("LAMIN_TESTING") == "true":
+                response = "y"
+            else:
+                response = input(
+                    "You already configured a local storage root for this instance in this"
+                    f" environment: {self.storage_local.root}\nDo you want to register another one? (y/n)"
+                )
+            if response != "y":
+                return None
         local_root = convert_pathlike(local_root)
         assert isinstance(local_root, LocalPathClasses)
-        self._local_storage = StorageSettings(local_root)  # type: ignore
-        register_storage(self._local_storage)  # type: ignore
-        self._local_storage_on = True
-        update_instance_record(self.id, {"storage_mode": "hybrid"})
+        self._storage_local = init_storage(local_root, self._id, register_hub=True)  # type: ignore
+        register_storage_in_instance(self._storage_local)  # type: ignore
+        logger.important(f"defaulting to local storage: {self._storage_local.root}")
 
     @property
     def slug(self) -> str:
         """Unique semantic identifier of form `"{account_handle}/{instance_name}"`."""
         return f"{self.owner}/{self.name}"
 
     @property
-    def git_repo(self) -> Optional[str]:
+    def git_repo(self) -> str | None:
         """Sync transforms with scripts in git repository.
 
         Provide the full git repo URL.
         """
         return self._git_repo
 
     @property
-    def id(self) -> UUID:
+    def _id(self) -> UUID:
         """The internal instance id."""
-        return self._id
+        return self._id_
 
     @property
-    def uid(self) -> Optional[str]:
+    def uid(self) -> str:
         """The user-facing instance id."""
-        return self._uid
+        from .hashing import hash_and_encode_as_b62
+
+        return hash_and_encode_as_b62(self._id.hex)[:12]
 
     @property
-    def schema(self) -> Set[str]:
+    def schema(self) -> set[str]:
         """Schema modules in addition to core schema."""
         if self._schema_str is None:
             return {}  # type: ignore
         else:
             return {schema for schema in self._schema_str.split(",") if schema != ""}
 
     @property
     def _sqlite_file(self) -> UPath:
         """SQLite file."""
-        return self.storage.key_to_filepath(f"{self.id.hex}.lndb")
+        return self.storage.key_to_filepath(f"{self._id.hex}.lndb")
 
     @property
     def _sqlite_file_local(self) -> Path:
         """Local SQLite file."""
         return self.storage.cloud_to_local_no_update(self._sqlite_file)
 
     def _update_cloud_sqlite_file(self, unlock_cloud_sqlite: bool = True) -> None:
@@ -287,19 +340,14 @@
             except PermissionError:
                 logger.warning("read-only access - did not access locker")
                 return empty_locker
         else:
             return empty_locker
 
     @property
-    def storage(self) -> StorageSettings:
-        """Low-level access to storage location."""
-        return self._storage
-
-    @property
     def is_remote(self) -> bool:
         """Boolean indicating if an instance has no local component."""
         if not self.storage.type_is_cloud:
             return False
 
         def is_local_uri(uri: str):
             if "@localhost:" in uri:
@@ -313,14 +361,33 @@
         if self.dialect == "postgresql":
             if is_local_uri(self.db):
                 return False
         # returns True for cloud SQLite
         # and remote postgres
         return True
 
+    @property
+    def is_on_hub(self) -> bool:
+        """Is this instance on the hub.
+
+        Only works if user has access to the instance.
+        """
+        if self._is_on_hub is None:
+            from ._hub_client import call_with_fallback_auth
+            from ._hub_crud import select_instance_by_id
+
+            response = call_with_fallback_auth(
+                select_instance_by_id, instance_id=self._id.hex
+            )
+            if response is None:
+                self._is_on_hub = False
+            else:
+                self._is_on_hub = True
+        return self._is_on_hub
+
     def _get_settings_file(self) -> Path:
         return instance_settings_file(self.name, self.owner)
 
     def _persist(self) -> None:
         assert self.name is not None
 
         filepath = self._get_settings_file()
@@ -337,26 +404,27 @@
     def _init_db(self):
         from .django import setup_django
 
         setup_django(self, init=True)
 
     def _load_db(
         self, do_not_lock_for_laminapp_admin: bool = False
-    ) -> Tuple[bool, str]:
+    ) -> tuple[bool, str]:
         # Is the database available and initialized as LaminDB?
         # returns a tuple of status code and message
         if self.dialect == "sqlite" and not self._sqlite_file.exists():
             legacy_file = self.storage.key_to_filepath(f"{self.name}.lndb")
             if legacy_file.exists():
                 raise RuntimeError(
                     "The SQLite file has been renamed!\nPlease rename your SQLite file"
                     f" {legacy_file} to {self._sqlite_file}"
                 )
             return False, f"SQLite file {self._sqlite_file} does not exist"
         from lamindb_setup import settings  # to check user
+
         from .django import setup_django
 
         # lock in all cases except if do_not_lock_for_laminapp_admin is True and
         # user is `laminapp-admin`
         # value doesn't matter if not a cloud sqlite instance
         lock_cloud_sqlite = self._is_cloud_sqlite and (
             not do_not_lock_for_laminapp_admin
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-from pathlib import Path
-from typing import Optional
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Optional
 from uuid import UUID, uuid4
+
 from lamin_utils import logger
 from pydantic.error_wrappers import ValidationError
 
 from ._settings_instance import InstanceSettings
 from ._settings_storage import StorageSettings
 from ._settings_store import (
     InstanceSettingsStore,
     UserSettingsStore,
     current_instance_settings_file,
     current_user_settings_file,
 )
 from ._settings_user import UserSettings
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class SettingsEnvFileOutdated(Exception):
     pass
 
 
-def load_instance_settings(instance_settings_file: Optional[Path] = None):
+def load_instance_settings(instance_settings_file: Path | None = None):
     if instance_settings_file is None:
         instance_settings_file = current_instance_settings_file()
     if not instance_settings_file.exists():
         raise SystemExit("No instance is loaded! Call `lamin init` or `lamin load`")
     try:
         settings_store = InstanceSettingsStore(_env_file=instance_settings_file)
     except (ValidationError, TypeError) as error:
         with open(instance_settings_file) as f:
             content = f.read()
         raise SettingsEnvFileOutdated(
             f"\n\n{error}\n\nYour instance settings file with\n\n{content}\nis invalid"
             f" (likely outdated), please delete {instance_settings_file} &"
             " re-initialize (local) or re-connect to the instance (remote)"
-        )
+        ) from error
     if settings_store.id == "null":
         raise ValueError(
-            "Your instance.id is undefined, please either load your instance from the"
+            "Your instance._id is undefined, please either load your instance from the"
             f" hub or update {instance_settings_file} with a new id: {uuid4().hex}"
         )
     isettings = setup_instance_from_store(settings_store)
     return isettings
 
 
 def load_or_create_user_settings() -> UserSettings:
@@ -56,21 +61,21 @@
         usettings = load_user_settings(current_user_settings)
     return usettings
 
 
 def load_user_settings(user_settings_file: Path):
     try:
         settings_store = UserSettingsStore(_env_file=user_settings_file)
-    except (ValidationError, TypeError):
+    except (ValidationError, TypeError) as error:
         msg = (
             "Your user settings file is invalid, please delete"
             f" {user_settings_file} and log in again."
         )
         print(msg)
-        raise SettingsEnvFileOutdated(msg)
+        raise SettingsEnvFileOutdated(msg) from error
     settings = setup_user_from_store(settings_store)
     return settings
 
 
 def setup_instance_from_store(store: InstanceSettingsStore) -> InstanceSettings:
     ssettings = StorageSettings(
         root=store.storage_root,
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings_save.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from pathlib import Path
+from __future__ import annotations
 
-from typing import Any, Dict, Union, get_type_hints, Optional
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Optional, get_type_hints
 from uuid import UUID
 
 from ._settings_store import (
-    UserSettingsStore,
     InstanceSettingsStore,
+    UserSettingsStore,
     current_user_settings_file,
     user_settings_file_email,
     user_settings_file_handle,
 )
-from ._settings_user import UserSettings
-from .upath import UPath
+
+if TYPE_CHECKING:
+    from ._settings_user import UserSettings
+    from .upath import UPath
 
 
 def save_user_settings(settings: UserSettings):
     type_hints = get_type_hints(UserSettingsStore)
     prefix = "lamin_user_"
     save_settings(settings, current_user_settings_file(), type_hints, prefix)
     if settings.email is not None:
@@ -27,28 +30,28 @@
             settings, user_settings_file_handle(settings.handle), type_hints, prefix
         )
 
 
 def save_settings(
     settings: Any,
     settings_file: Path,
-    type_hints: Dict[str, Any],
+    type_hints: dict[str, Any],
     prefix: str,
 ):
     with open(settings_file, "w") as f:
         for store_key, type in type_hints.items():
             if type == Optional[str]:
                 type = str
             if "__" not in store_key:
                 if store_key == "storage_root":
                     value = settings.storage.root_as_str
                 elif store_key == "storage_region":
                     value = settings.storage.region
                 else:
-                    if store_key in {"db", "schema_str", "name_", "uuid"}:
+                    if store_key in {"db", "schema_str", "name_", "uuid", "id"}:
                         settings_key = f"_{store_key.rstrip('_')}"
                     else:
                         settings_key = store_key
                     value = getattr(settings, settings_key)
                 if value is None:
                     value = "null"
                 elif isinstance(value, UUID):
@@ -61,14 +64,14 @@
 def save_instance_settings(settings: Any, settings_file: Path):
     type_hints = get_type_hints(InstanceSettingsStore)
     prefix = "lamindb_instance_"
     save_settings(settings, settings_file, type_hints, prefix)
 
 
 def save_system_storage_settings(
-    cache_path: Union[str, Path, UPath, None], settings_file: Path
+    cache_path: str | Path | UPath | None, settings_file: Path
 ):
     cache_path = "null" if cache_path is None else cache_path
     if isinstance(cache_path, Path):  # also True for UPath
         cache_path = cache_path.as_posix()
     with open(settings_file, "w") as f:
         f.write(f"lamindb_cache_path={cache_path}")
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,47 @@
+from __future__ import annotations
+
 import os
+import secrets
 import shutil
-from lamin_utils import logger
+import string
 from pathlib import Path
-from typing import Any, Optional, Union, Literal
-from ._aws_storage import find_closest_aws_region
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
+
 from appdirs import AppDirs
+from lamin_utils import logger
+
+from ._aws_storage import find_closest_aws_region
 from ._settings_save import save_system_storage_settings
 from ._settings_store import system_storage_settings_file
-from .upath import LocalPathClasses, UPath, create_path, convert_pathlike
-from uuid import UUID
-import string
-import secrets
-from .types import UPathStr
-from .upath import hosted_regions
+from .upath import (
+    HOSTED_REGIONS,
+    LocalPathClasses,
+    UPath,
+    convert_pathlike,
+    create_path,
+)
+
+if TYPE_CHECKING:
+    from uuid import UUID
 
+    from .types import UPathStr
 
 DIRS = AppDirs("lamindb", "laminlabs")
 IS_INITIALIZED_KEY = ".lamindb/_is_initialized"
 
 
 def base62(n_char: int) -> str:
     """Like nanoid without hyphen and underscore."""
     alphabet = string.digits + string.ascii_letters.swapcase()
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
 
 
-def get_storage_region(storage_root: UPathStr) -> Optional[str]:
+def get_storage_region(storage_root: UPathStr) -> str | None:
     storage_root_str = str(storage_root)
     if storage_root_str.startswith("s3://"):
         import botocore.session as session
         from botocore.config import Config
         from botocore.exceptions import NoCredentialsError
 
         # strip the prefix and any suffixes of the bucket name
@@ -51,97 +62,108 @@
         # error message, this is how to do test for the "NoSuchBucket" error:
         #     exc.response["Error"]["Code"] == "NoSuchBucket"
     else:
         storage_region = None
     return storage_region
 
 
-def mark_storage_root(root: UPathStr):
+def mark_storage_root(root: UPathStr, uid: str):
     # we need to touch a 0-byte object in folder-like storage location on S3 to avoid
     # permission errors from leveraging s3fs on an empty hosted storage location
     # for consistency, we write this file everywhere
     root_upath = convert_pathlike(root)
     mark_upath = root_upath / IS_INITIALIZED_KEY
-    mark_upath.touch()
+    mark_upath.write_text(uid)
 
 
-def init_storage(root: UPathStr) -> "StorageSettings":
+def init_storage(
+    root: UPathStr, instance_id: UUID | None = None, register_hub: bool | None = None
+) -> StorageSettings:
     if root is None:
         raise ValueError("`storage` argument can't be `None`")
     root_str = str(root)  # ensure we have a string
-    uid = base62(8)
+    uid = base62(12)
     region = None
     lamin_env = os.getenv("LAMIN_ENV")
     if root_str.startswith("create-s3"):
         if root_str != "create-s3":
             assert "--" in root_str, "example: `create-s3--eu-central-1`"
             region = root_str.replace("create-s3--", "")
         if region is None:
             region = find_closest_aws_region()
         else:
-            if region not in hosted_regions:
-                raise ValueError(f"region has to be one of {hosted_regions}")
+            if region not in HOSTED_REGIONS:
+                raise ValueError(f"region has to be one of {HOSTED_REGIONS}")
         if lamin_env is None or lamin_env == "prod":
             root_str = f"s3://lamin-{region}/{uid}"
         else:
             root_str = f"s3://lamin-hosted-test/{uid}"
     elif root_str.startswith(("gs://", "s3://")):
         pass
     else:  # local path
         try:
             _ = Path(root_str)
         except Exception as e:
             logger.error("`storage` is not a valid local, GCP storage or AWS S3 path")
             raise e
-    ssettings = StorageSettings(uid=uid, root=root_str, region=region)
-    if ssettings.type_is_cloud:
+    ssettings = StorageSettings(
+        uid=uid,
+        root=root_str,
+        region=region,
+        instance_id=instance_id,
+    )
+    # the below might update the uid with one that's already taken on the hub
+    if ssettings.type_is_cloud or register_hub:
         from ._hub_core import init_storage as init_storage_hub
 
-        ssettings._description = f"Created as default storage for instance {uid}"
-        ssettings._uuid_ = init_storage_hub(ssettings)
-        logger.important(f"registered storage: {ssettings.root_as_str}")
-    mark_storage_root(ssettings.root)
+        init_storage_hub(ssettings)
+    # below comes last only if everything else was successful
+    mark_storage_root(ssettings.root, ssettings.uid)  # type: ignore
     return ssettings
 
 
-def _process_cache_path(cache_path: Union[str, Path, UPath, None]):
+def _process_cache_path(cache_path: str | Path | UPath | None):
     if cache_path is None or cache_path == "null":
         return None
     cache_dir = UPath(cache_path)
     if not isinstance(cache_dir, LocalPathClasses):
         raise ValueError("cache dir should be a local path.")
     if cache_dir.exists() and not cache_dir.is_dir():
         raise ValueError("cache dir should be a directory.")
     return cache_dir
 
 
 class StorageSettings:
-    """Manage cloud or local storage settings."""
+    """Settings for a given storage location (local or cloud)."""
 
     def __init__(
         self,
         root: UPathStr,
-        region: Optional[str] = None,
-        uid: Optional[str] = None,
-        uuid: Optional[UUID] = None,
-        access_token: Optional[str] = None,
+        region: str | None = None,
+        uid: str | None = None,
+        uuid: UUID | None = None,
+        instance_id: UUID | None = None,
+        access_token: str | None = None,
     ):
         self._uid = uid
         self._uuid_ = uuid
         self._root_init = convert_pathlike(root)
         if isinstance(self._root_init, LocalPathClasses):  # local paths
-            (self._root_init / ".lamindb").mkdir(parents=True, exist_ok=True)
-            self._root_init = self._root_init.resolve()
+            try:
+                (self._root_init / ".lamindb").mkdir(parents=True, exist_ok=True)
+                self._root_init = self._root_init.resolve()
+            except Exception:
+                logger.warning("unable to create .lamindb folder")
+                pass
         self._root = None
-        self._aws_account_id: Optional[int] = None
-        self._description: Optional[str] = None
+        self._instance_id = instance_id
         # we don't yet infer region here to make init fast
         self._region = region
         # would prefer to type below as Registry, but need to think through import order
-        self._record: Optional[Any] = None
+        self._record: Any | None = None
         # cache settings
         self._storage_settings_file = system_storage_settings_file()
         if self._storage_settings_file.exists():
             from dotenv import dotenv_values
 
             cache_path = dotenv_values(self._storage_settings_file)[
                 "lamindb_cache_path"
@@ -151,42 +173,44 @@
             self._cache_dir = None
         # save access_token here for use in self.root
         self.access_token = access_token
 
         # local storage
         self._has_local = False
         self._local = None
+        self._is_on_hub: bool | None = None
 
     @property
     def id(self) -> int:
-        """Storage id."""
+        """Storage id in current instance."""
         return self.record.id
 
     @property
-    def _uuid(self) -> Optional[UUID]:
+    def _uuid(self) -> UUID | None:
         """Lamin's internal storage uuid."""
         return self._uuid_
 
     @property
-    def uid(self) -> Optional[str]:
+    def uid(self) -> str | None:
         """Storage id."""
         if self._uid is None:
             self._uid = self.record.uid
         return self._uid
 
     @property
     def _mark_storage_root(self) -> UPath:
         return self.root / IS_INITIALIZED_KEY
 
     @property
     def record(self) -> Any:
-        """Storage record."""
+        """Storage record in current instance."""
         if self._record is None:
             # dynamic import because of import order
             from lnschema_core.models import Storage
+
             from ._settings import settings
 
             self._record = Storage.objects.using(settings._using_key).get(
                 root=self.root_as_str
             )
         return self._record
 
@@ -268,15 +292,15 @@
 
     @property
     def type_is_cloud(self) -> bool:
         """`True` if `storage_root` is in cloud, `False` otherwise."""
         return self.type != "local"
 
     @property
-    def region(self) -> Optional[str]:
+    def region(self) -> str | None:
         """Storage region."""
         if self._region is None:
             self._region = get_storage_region(self.root_as_str)
         return self._region
 
     @property
     def type(self) -> Literal["local", "s3", "gs"]:
@@ -286,32 +310,49 @@
         """
         import fsspec
 
         convert = {"file": "local"}
         protocol = fsspec.utils.get_protocol(self.root_as_str)
         return convert.get(protocol, protocol)  # type: ignore
 
-    def key_to_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
+    @property
+    def is_on_hub(self) -> bool:
+        """Is this instance on the hub.
+
+        Only works if user has access to the instance.
+        """
+        if self._is_on_hub is None:
+            from ._hub_client import call_with_fallback_auth
+            from ._hub_crud import select_storage
+
+            response = call_with_fallback_auth(select_storage, id=self._uuid.hex)  # type: ignore
+            if response is None:
+                self._is_on_hub = False
+            else:
+                self._is_on_hub = True
+        return self._is_on_hub
+
+    def key_to_filepath(self, filekey: Path | UPath | str) -> UPath:
         """Cloud or local filepath from filekey."""
         return self.root / filekey
 
-    def cloud_to_local(self, filepath: Union[Path, UPath], **kwargs) -> UPath:
+    def cloud_to_local(self, filepath: Path | UPath, **kwargs) -> UPath:
         """Local (cache) filepath from filepath."""
         local_filepath = self.cloud_to_local_no_update(filepath)  # type: ignore
         if isinstance(filepath, UPath) and not isinstance(filepath, LocalPathClasses):
             local_filepath.parent.mkdir(parents=True, exist_ok=True)
             filepath.synchronize(local_filepath, **kwargs)
         return local_filepath
 
     # conversion to Path via cloud_to_local() would trigger download
     # of remote file to cache if there already is one
     # in pure write operations that update the cloud, we don't want this
     # hence, we manually construct the local file path
     # using the `.parts` attribute in the following line
     def cloud_to_local_no_update(self, filepath: UPath) -> UPath:
         if isinstance(filepath, UPath) and not isinstance(filepath, LocalPathClasses):
-            return self.cache_dir.joinpath(filepath._url.netloc, *filepath.parts[1:])  # type: ignore # noqa
+            return self.cache_dir.joinpath(filepath._url.netloc, *filepath.parts[1:])  # type: ignore
         return filepath
 
-    def local_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
+    def local_filepath(self, filekey: Path | UPath | str) -> UPath:
         """Local (cache) filepath from filekey: `local(filepath(...))`."""
         return self.cloud_to_local(self.key_to_filepath(filekey))
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from pathlib import Path
 from typing import Optional
+
 from pydantic import BaseSettings
 
 if "LAMIN_SETTINGS_DIR" in os.environ:
     # Needed when running with AWS Lambda, as only tmp/ directory has a write access
     settings_dir = Path(f"{os.environ['LAMIN_SETTINGS_DIR']}/.lamin")
 else:
     # user_config_dir in appdirs is weird on MacOS!
@@ -47,16 +48,16 @@
     return settings_dir / "storage.env"
 
 
 class InstanceSettingsStore(BaseSettings):
     owner: str
     name: str
     storage_root: str
-    storage_region: Optional[str]
-    db: Optional[str]
+    storage_region: Optional[str]  # take old type annotations here because pydantic
+    db: Optional[str]  # doesn't like new types on 3.9 even with future annotations
     schema_str: Optional[str]
     id: str
     git_repo: Optional[str]
 
     class Config:
         env_prefix = "lamindb_instance_"
         env_file = ".env"
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_settings_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import Optional
-from uuid import UUID
+from typing import TYPE_CHECKING, Optional
+
+if TYPE_CHECKING:
+    from uuid import UUID
 
 
 class user_description:
     email = """User email."""
     password = """API key or legacy password."""
     uid = """Universal user ID."""
     handle = "Unique handle."
@@ -15,23 +19,23 @@
 class UserSettings:
     """User data. All synched from cloud."""
 
     handle: str = "anonymous"
     """Unique handle."""
     email: str = None  # type: ignore
     """User email."""
-    password: Optional[str] = None
+    password: str | None = None
     """API key or legacy password."""
-    access_token: Optional[str] = None
+    access_token: str | None = None
     """User access token."""
     uid: str = "null"
     """Universal user ID."""
-    _uuid: Optional[UUID] = None
+    _uuid: UUID | None = None
     """Lamin's internal user ID."""
-    name: Optional[str] = None
+    name: str | None = None
     """Full name."""
 
     def __repr__(self) -> str:
         """Rich string representation."""
         representation = f"Current user: {self.handle}"
         attrs = ["handle", "email", "uid"]
         for attr in attrs:
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.71.0/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-from ._settings_instance import InstanceSettings
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from django.db.utils import OperationalError, ProgrammingError
 
+if TYPE_CHECKING:
+    from ._settings_instance import InstanceSettings
+
 
 def write_bionty_sources(isettings: InstanceSettings) -> None:
     """Write bionty sources to PublicSource table."""
     if "bionty" not in isettings.schema:
         return None
     import shutil
-    from bionty_base.dev._handle_sources import parse_sources_yaml
+
     import bionty_base
+    from bionty_base.dev._handle_sources import parse_sources_yaml
     from lnschema_bionty.models import PublicSource
 
     shutil.copy(
         bionty_base.settings.current_sources, bionty_base.settings.lamindb_sources
     )
 
     all_sources = parse_sources_yaml(bionty_base.settings.local_sources)
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.71.0/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from __future__ import annotations
+
 from datetime import datetime, timezone
-from pathlib import Path
-from typing import Optional, Union
 from functools import wraps
-from uuid import UUID
+from typing import TYPE_CHECKING, Optional, Union
+
 from lamin_utils import logger
 
-from .upath import UPath, infer_filesystem, create_mapper
+from .upath import UPath, create_mapper, infer_filesystem
+
+if TYPE_CHECKING:
+    from pathlib import Path
+    from uuid import UUID
 
 EXPIRATION_TIME = 24 * 60 * 60 * 7  # 7 days
 
 MAX_MSG_COUNTER = 100  # print the msg after this number of iterations
 
 
 # raise if an instance is already locked
@@ -27,17 +32,15 @@
 
     @classmethod
     def unlock(cls):
         pass
 
 
 class Locker:
-    def __init__(
-        self, user_uid: str, storage_root: Union[UPath, Path], instance_id: UUID
-    ):
+    def __init__(self, user_uid: str, storage_root: UPath | Path, instance_id: UUID):
         logger.debug(
             f"init cloud sqlite locker: {user_uid}, {storage_root}, {instance_id}."
         )
 
         self._counter = 0
 
         self.user = user_uid
@@ -165,32 +168,32 @@
         if self._has_lock is None:
             logger.info("the lock has not been initialized, trying to obtain the lock.")
             self.lock()
 
         return self._has_lock
 
 
-_locker: Optional[Locker] = None
+_locker: Locker | None = None
 
 
 def get_locker(isettings) -> Locker:
     from ._settings import settings
 
     global _locker
 
     user_uid = settings.user.uid
     storage_root = isettings.storage.root
 
     if (
         _locker is None
         or _locker.user != user_uid
         or _locker.root is not storage_root
-        or _locker.instance_id != isettings.id
+        or _locker.instance_id != isettings._id
     ):
-        _locker = Locker(user_uid, storage_root, isettings.id)
+        _locker = Locker(user_uid, storage_root, isettings._id)
 
     return _locker
 
 
 def clear_locker():
     global _locker
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/django.py` & `lamindb_setup-0.71.0/lamindb_setup/core/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # flake8: noqa
 import builtins
 import os
 from pathlib import Path
 import shutil
 import time
 from lamin_utils import logger
@@ -100,9 +102,9 @@
         isettings._update_cloud_sqlite_file(unlock_cloud_sqlite=False)
     elif init:
         call_command("migrate", verbosity=0)
 
     global IS_SETUP
     IS_SETUP = True
 
-    if isettings._local_storage_on:
+    if isettings.keep_artifacts_local:
         isettings._search_local_root()
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/hashing.py` & `lamindb_setup-0.71.0/lamindb_setup/core/hashing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,50 @@
+from __future__ import annotations
+
 """Hashing.
 
 .. autosummary::
    :toctree: .
 
    hash_set
    hash_file
 
 """
 
 import base64
 import hashlib
-from typing import List, Set, Tuple
-from .types import Path, UPathStr
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .types import Path, UPathStr
+
+
+def hash_and_encode_as_b62(s: str) -> str:
+    from lamin_utils._base62 import encodebytes
+
+    return encodebytes(hashlib.md5(s.encode()).digest())
 
 
 def to_b64_str(bstr: bytes):
     b64 = base64.urlsafe_b64encode(bstr).decode().strip("=")
     return b64
 
 
 def b16_to_b64(s: str):
     return to_b64_str(base64.b16decode(s.strip('"'), casefold=True))
 
 
 # a lot to read about this: lamin-notes/2022/hashing
-def hash_set(s: Set[str]) -> str:
+def hash_set(s: set[str]) -> str:
     bstr = ":".join(sorted(s)).encode("utf-8")
     # as we're truncating at 20 b64, we choose md5 over sha512
     return to_b64_str(hashlib.md5(bstr).digest())[:20]
 
 
-def hash_md5s_from_dir(etags: List[str]) -> Tuple[str, str]:
+def hash_md5s_from_dir(etags: list[str]) -> tuple[str, str]:
     # need to sort below because we don't want the order of parsing the dir to
     # affect the hash
     digests = b"".join(
         hashlib.md5(etag.encode("utf-8")).digest() for etag in sorted(etags)
     )
     digest = hashlib.md5(digests).digest()
     return to_b64_str(digest)[:22], "md5-d"
@@ -45,15 +55,15 @@
         data = fp.read()
     data_size = len(data)
     header = f"blob {data_size}\0".encode()
     blob = header + data
     return hashlib.sha1(blob)
 
 
-def hash_file(file_path: Path, chunk_size=50 * 1024 * 1024) -> Tuple[str, str]:
+def hash_file(file_path: Path, chunk_size=50 * 1024 * 1024) -> tuple[str, str]:
     chunks = []
     with open(file_path, "rb") as fp:
         # read first chunk
         chunks = [fp.read(chunk_size)]
         # try reading the 2nd chunk
         data = fp.read(chunk_size)
         if data:
```

### Comparing `lamindb_setup-0.70.0/lamindb_setup/core/upath.py` & `lamindb_setup-0.71.0/lamindb_setup/core/upath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # we are not documenting UPath here because it's documented at lamindb.UPath
 """Paths & file systems."""
 
 from __future__ import annotations
 
 import os
+from collections import defaultdict
 from datetime import datetime, timezone
-import botocore.session
+from functools import partial
+from itertools import islice
 from pathlib import Path, PurePosixPath
-from typing import Literal, Dict
+from typing import TYPE_CHECKING, Any, Literal
+
+import botocore.session
 import fsspec
-from itertools import islice
-from typing import Optional, Set, Any, Tuple, List
-from collections import defaultdict
 from lamin_utils import logger
 from upath import UPath
-from upath.implementations.cloud import CloudPath, S3Path  # noqa  # keep CloudPath!
+from upath.implementations.cloud import CloudPath, S3Path  # keep CloudPath!
 from upath.implementations.local import LocalPath, PosixUPath, WindowsUPath
-from .types import UPathStr
+
 from .hashing import b16_to_b64, hash_md5s_from_dir
 
+if TYPE_CHECKING:
+    from .types import UPathStr
+
 LocalPathClasses = (PosixUPath, WindowsUPath, LocalPath)
 
 # also see https://gist.github.com/securifera/e7eed730cbe1ce43d0c29d7cd2d582f4
 #    ".gz" is not listed here as it typically occurs with another suffix
 # the complete list is at lamindb.core.storage._suffixes
 VALID_SUFFIXES = {
     #
@@ -53,15 +57,15 @@
     ".json",
 }
 
 
 TRAILING_SEP = (os.sep, os.altsep) if os.altsep is not None else os.sep
 
 
-def extract_suffix_from_path(path: Path, arg_name: Optional[str] = None) -> str:
+def extract_suffix_from_path(path: Path, arg_name: str | None = None) -> str:
     def process_digits(suffix: str):
         if suffix[1:].isdigit():  # :1 to skip the dot
             return ""  # digits are no valid suffixes
         else:
             return suffix
 
     if len(path.suffixes) <= 1:
@@ -137,77 +141,129 @@
         )
     else:
         return fsspec.FSMap(
             url, fs, check=check, create=create, missing_exceptions=missing_exceptions
         )
 
 
-def print_hook(size: int, value: int, **kwargs):
+def print_hook(size: int, value: int, objectname: str, action: str):
     progress_in_percent = (value / size) * 100
-    out = (
-        f"... {kwargs['action']} {Path(kwargs['filepath']).name}:"
-        f" {min(progress_in_percent, 100):4.1f}%"
-    )
-    if progress_in_percent >= 100:
-        out += "\n"
+    out = f"... {action} {objectname}:" f" {min(progress_in_percent, 100):4.1f}%"
     if "NBPRJ_TEST_NBPATH" not in os.environ:
         print(out, end="\r")
 
 
 class ProgressCallback(fsspec.callbacks.Callback):
-    def __init__(self, action: Literal["uploading", "downloading"]):
+    def __init__(
+        self,
+        objectname: str,
+        action: Literal["uploading", "downloading", "synchronizing"],
+        adjust_size: bool = False,
+    ):
+        assert action in {"uploading", "downloading", "synchronizing"}
+
         super().__init__()
+
         self.action = action
+        print_progress = partial(print_hook, objectname=objectname, action=action)
+        self.hooks = {"print_progress": print_progress}
+
+        self.adjust_size = adjust_size
+
+    def absolute_update(self, value):
+        pass
+
+    def relative_update(self, inc=1):
+        pass
+
+    def update_relative_value(self, inc=1):
+        self.value += inc
+        self.call()
 
     def branch(self, path_1, path_2, kwargs):
-        kwargs["callback"] = fsspec.callbacks.Callback(
-            hooks=dict(print_hook=print_hook), filepath=path_1, action=self.action
-        )
+        if self.adjust_size:
+            if Path(path_2 if self.action != "uploading" else path_1).is_dir():
+                self.size -= 1
+        kwargs["callback"] = ChildProgressCallback(self)
+
+    def branched(self, path_1, path_2, **kwargs):
+        self.branch(path_1, path_2, kwargs)
+        return kwargs["callback"]
+
+    def wrap(self, iterable):
+        if self.adjust_size:
+            paths = []
+            for lpath, rpath in iterable:
+                paths.append((lpath, rpath))
+                if Path(lpath).is_dir():
+                    self.size -= 1
+            self.adjust_size = False
+            return paths
+        else:
+            return iterable
 
-    def call(self, *args, **kwargs):
-        return None
+    @classmethod
+    def requires_progress(
+        cls,
+        maybe_callback: fsspec.callbacks.Callback | None,
+        print_progress: bool,
+        objectname: str,
+        action: Literal["uploading", "downloading", "synchronizing"],
+        **kwargs,
+    ):
+        if maybe_callback is None:
+            if print_progress:
+                return cls(objectname, action, **kwargs)
+            else:
+                return fsspec.callbacks.NoOpCallback()
+        return maybe_callback
+
+
+class ChildProgressCallback(fsspec.callbacks.Callback):
+    def __init__(self, parent: ProgressCallback):
+        super().__init__()
+
+        self.parent = parent
+
+    def parent_update(self, inc=1):
+        self.parent.update_relative_value(inc)
+
+    def relative_update(self, inc=1):
+        self.parent_update(inc / self.size)
 
 
 def download_to(self, path: UPathStr, print_progress: bool = False, **kwargs):
     """Download to a path."""
-    if print_progress:
-        # can't do path.is_dir() because path doesn't exist
-        # so assume any destination without a suffix is a dir
-        # this is temporary until we have a proper progress bar for directories
-        if os.path.splitext(path)[-1] not in {"", ".zrad", ".zarr"}:
-            cb = ProgressCallback("downloading")
-        else:
-            # todo: make proper progress bar for directories
-            cb = fsspec.callbacks.NoOpCallback()
-        kwargs["callback"] = cb
+    if print_progress and "callback" not in kwargs:
+        callback = ProgressCallback(
+            PurePosixPath(path).name, "downloading", adjust_size=True
+        )
+        kwargs["callback"] = callback
+
     self.fs.download(str(self), str(path), **kwargs)
 
 
 def upload_from(
     self,
     path: UPathStr,
     dir_inplace: bool = False,
     print_progress: bool = False,
     **kwargs,
 ):
     """Upload from a local path."""
-    path_is_dir = os.path.isdir(path)
+    path = Path(path)
+    path_is_dir = path.is_dir()
     if not path_is_dir:
         dir_inplace = False
 
-    if print_progress:
-        if not path_is_dir:
-            cb = ProgressCallback("uploading")
-        else:
-            # todo: make proper progress bar for directories
-            cb = fsspec.callbacks.NoOpCallback()
-        kwargs["callback"] = cb
+    if print_progress and "callback" not in kwargs:
+        callback = ProgressCallback(path.name, "uploading")
+        kwargs["callback"] = callback
 
     if dir_inplace:
-        path = Path(path)
         source = [f for f in path.rglob("*") if f.is_file()]
         destination = [str(self / f.relative_to(path)) for f in source]
         source = [str(f) for f in source]  # type: ignore
     else:
         source = str(path)  # type: ignore
         destination = str(self)  # type: ignore
     # this weird thing is to avoid s3fs triggering create_bucket in upload
@@ -229,15 +285,22 @@
 
     if cleanup_cache:
         # normally this is invalidated after the upload but still better to check
         if bucket in self.fs.dircache:
             del self.fs.dircache[bucket]
 
 
-def synchronize(self, objectpath: Path, error_no_origin: bool = True, **kwargs):
+def synchronize(
+    self,
+    objectpath: Path,
+    error_no_origin: bool = True,
+    print_progress: bool = False,
+    callback: fsspec.callbacks.Callback | None = None,
+    **kwargs,
+):
     """Sync to a local destination path."""
     # optimize the number of network requests
     if "timestamp" in kwargs:
         is_dir = False
         exists = True
         cloud_mts = kwargs.pop("timestamp")
     else:
@@ -288,23 +351,31 @@
                 need_synchronize = False
             else:
                 need_synchronize = True
         else:
             destination_exists = False
             need_synchronize = True
         if need_synchronize:
+            callback = ProgressCallback.requires_progress(
+                callback, print_progress, objectpath.name, "synchronizing"
+            )
+            callback.set_size(len(files))
             origin_file_keys = []
-            for file, stat in files.items():
-                destination = PurePosixPath(file).relative_to(self.path)
-                origin_file_keys.append(destination.as_posix())
+            for file, stat in callback.wrap(files.items()):
+                file_key = PurePosixPath(file).relative_to(self.path)
+                origin_file_keys.append(file_key.as_posix())
                 timestamp = stat[modified_key].timestamp()
-                origin = UPath(f"{self.protocol}://{file}", **self._kwargs)
-                origin.synchronize(
-                    objectpath / destination, timestamp=timestamp, **kwargs
+
+                origin = f"{self.protocol}://{file}"
+                destination = objectpath / file_key
+                child = callback.branched(origin, destination.as_posix())
+                UPath(origin, **self._kwargs).synchronize(
+                    destination, timestamp=timestamp, callback=child, **kwargs
                 )
+                child.close()
             if destination_exists:
                 local_files = [file for file in objectpath.rglob("*") if file.is_file()]
                 if len(local_files) > len(files):
                     for file in local_files:
                         if (
                             file.relative_to(objectpath).as_posix()
                             not in origin_file_keys
@@ -312,47 +383,55 @@
                             file.unlink()
                             parent = file.parent
                             if next(parent.iterdir(), None) is None:
                                 parent.rmdir()
         return None
 
     # synchronization logic for files
+    callback = ProgressCallback.requires_progress(
+        callback, print_progress, objectpath.name, "synchronizing"
+    )
+    kwargs["callback"] = callback
     if objectpath.exists():
         local_mts = objectpath.stat().st_mtime  # type: ignore
         need_synchronize = cloud_mts > local_mts
     else:
         objectpath.parent.mkdir(parents=True, exist_ok=True)
         need_synchronize = True
     if need_synchronize:
         self.download_to(objectpath, **kwargs)
         os.utime(objectpath, times=(cloud_mts, cloud_mts))
+    else:
+        # nothing happens if parent_update is not defined
+        # because of Callback.no_op
+        callback.parent_update()
 
 
-def modified(self) -> Optional[datetime]:
+def modified(self) -> datetime | None:
     """Return modified time stamp."""
     mtime = self.fs.modified(str(self))
     if mtime.tzinfo is None:
         mtime = mtime.replace(tzinfo=timezone.utc)
     return mtime.astimezone().replace(tzinfo=None)
 
 
 def compute_file_tree(
     path: Path,
     *,
     level: int = -1,
     only_dirs: bool = False,
-    limit: int = 1000,
-    include_paths: Optional[Set[Any]] = None,
-    skip_suffixes: Optional[List[str]] = None,
-) -> Tuple[str, int]:
+    n_max_files_per_dir_and_type: int = 100,
+    n_max_files: int = 1000,
+    include_paths: set[Any] | None = None,
+    skip_suffixes: list[str] | None = None,
+) -> tuple[str, int]:
     space = "    "
     branch = "│   "
     tee = "├── "
     last = "└── "
-    max_files_per_dir_per_type = 7
     if skip_suffixes is None:
         skip_suffixes_tuple = ()
     else:
         skip_suffixes_tuple = tuple(skip_suffixes)  # type: ignore
     n_objects = 0
     n_directories = 0
 
@@ -378,71 +457,72 @@
             i
             for i in dir_path.iterdir()
             if i.as_posix().rstrip("/") != stripped_dir_path
         ]
         if only_dirs:
             contents = [d for d in contents if d.is_dir()]
         pointers = [tee] * (len(contents) - 1) + [last]
-        n_files_per_dir_per_type = defaultdict(lambda: 0)  # type: ignore
-        for pointer, child_path in zip(pointers, contents):
+        n_files_per_dir_and_type = defaultdict(lambda: 0)  # type: ignore
+        for pointer, child_path in zip(pointers, contents, strict=False):  # type: ignore
             if child_path.is_dir():
                 if include_dirs and child_path not in include_dirs:
                     continue
                 yield prefix + pointer + child_path.name
                 n_directories += 1
-                n_files_per_dir_per_type = defaultdict(lambda: 0)
+                n_files_per_dir_and_type = defaultdict(lambda: 0)
                 extension = branch if pointer == tee else space
                 yield from inner(child_path, prefix=prefix + extension, level=level - 1)
             elif not only_dirs:
                 if include_paths and child_path not in include_paths:
                     continue
                 suffix = extract_suffix_from_path(child_path)
                 suffixes.add(suffix)
-                n_files_per_dir_per_type[suffix] += 1
+                n_files_per_dir_and_type[suffix] += 1
                 n_objects += 1
-                if n_files_per_dir_per_type[suffix] == max_files_per_dir_per_type:
+                if n_files_per_dir_and_type[suffix] == n_max_files_per_dir_and_type:
                     yield prefix + "..."
-                elif n_files_per_dir_per_type[suffix] > max_files_per_dir_per_type:
+                elif n_files_per_dir_and_type[suffix] > n_max_files_per_dir_and_type:
                     continue
                 else:
                     yield prefix + pointer + child_path.name
 
     folder_tree = ""
     iterator = inner(path, level=level)
-    for line in islice(iterator, limit):
+    for line in islice(iterator, n_max_files):
         folder_tree += f"\n{line}"
     if next(iterator, None):
-        folder_tree += f"\n... only showing {limit} out of {n_objects} files"
+        folder_tree += f"\n... only showing {n_max_files} out of {n_objects} files"
     directory_info = "directory" if n_directories == 1 else "directories"
     display_suffixes = ", ".join([f"{suffix!r}" for suffix in suffixes])
     suffix_message = f" with suffixes {display_suffixes}" if n_objects > 0 else ""
     message = (
         f"{path.name} ({n_directories} sub-{directory_info} &"
         f" {n_objects} files{suffix_message}): {folder_tree}"
     )
     return message, n_objects
 
 
 # adapted from: https://stackoverflow.com/questions/9727673
 def view_tree(
     path: Path,
     *,
-    level: int = -1,
+    level: int = 2,
     only_dirs: bool = False,
-    limit: int = 1000,
-    include_paths: Optional[Set[Any]] = None,
-    skip_suffixes: Optional[List[str]] = None,
+    n_max_files_per_dir_and_type: int = 100,
+    n_max_files: int = 1000,
+    include_paths: set[Any] | None = None,
+    skip_suffixes: list[str] | None = None,
 ) -> None:
     """Print a visual tree structure of files & directories.
 
     Args:
         level: If `1`, only iterate through one level, if `2` iterate through 2
             levels, if `-1` iterate through entire hierarchy.
         only_dirs: Only iterate through directories.
-        limit: Display limit. Will only show this many files. Doesn't affect count.
+        n_max_files: Display limit. Will only show this many files. Doesn't affect count.
         include_paths: Restrict to these paths.
         skip_suffixes: Skip directories with these suffixes.
 
     Examples:
         >>> dir_path = ln.core.datasets.generate_cell_ranger_files(
         >>>     "sample_001", ln.settings.storage
         >>> )
@@ -468,15 +548,16 @@
         ├── filtered_feature_bc_matrix.h5
         └── raw_feature_bc_matrix.h5
     """
     message, _ = compute_file_tree(
         path,
         level=level,
         only_dirs=only_dirs,
-        limit=limit,
+        n_max_files=n_max_files,
+        n_max_files_per_dir_and_type=n_max_files_per_dir_and_type,
         include_paths=include_paths,
         skip_suffixes=skip_suffixes,
     )
     logger.print(message)
 
 
 def to_url(upath):
@@ -493,17 +574,18 @@
     """
     if upath.protocol != "s3":
         raise ValueError("The provided UPath must be an S3 path.")
     key = "/".join(upath.parts[1:])
     bucket = upath._url.netloc
     if bucket == "scverse-spatial-eu-central-1":
         region = "eu-central-1"
-    elif f"s3://{bucket}" not in hosted_buckets:
-        metadata = upath.fs.call_s3("head_bucket", Bucket=upath._url.netloc)
-        region = metadata["BucketRegion"]
+    elif f"s3://{bucket}" not in HOSTED_BUCKETS:
+        response = upath.fs.call_s3("head_bucket", Bucket=upath._url.netloc)
+        headers = response["ResponseMetadata"]["HTTPHeaders"]
+        region = headers.get("x-amz-bucket-region")
     else:
         region = bucket.replace("lamin_", "")
     if region == "us-east-1":
         return f"https://{bucket}.s3.amazonaws.com/{key}"
     else:
         return f"https://{bucket}.s3-{region}.amazonaws.com/{key}"
 
@@ -574,62 +656,61 @@
         raise ValueError("pathlike should be of type UPathStr")
     # remove trailing slash
     if path._parts and path._parts[-1] == "":
         path._parts = path._parts[:-1]
     return path
 
 
-hosted_regions = [
+HOSTED_REGIONS = [
     "eu-central-1",
     "eu-west-2",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
 lamin_env = os.getenv("LAMIN_ENV")
 if lamin_env is None or lamin_env == "prod":
-    hosted_buckets_list = [f"s3://lamin-{region}" for region in hosted_regions]
+    hosted_buckets_list = [f"s3://lamin-{region}" for region in HOSTED_REGIONS]
     hosted_buckets_list.append("s3://scverse-spatial-eu-central-1")
-    hosted_buckets = tuple(hosted_buckets_list)
+    HOSTED_BUCKETS = tuple(hosted_buckets_list)
 else:
-    hosted_buckets = ("s3://lamin-hosted-test",)  # type: ignore
-credentials_cache: Dict[str, Dict[str, str]] = {}
+    HOSTED_BUCKETS = ("s3://lamin-hosted-test",)  # type: ignore
+credentials_cache: dict[str, dict[str, str]] = {}
 AWS_CREDENTIALS_PRESENT = None
 
 
-def create_path(path: UPath, access_token: Optional[str] = None) -> UPath:
+def create_path(path: UPath, access_token: str | None = None) -> UPath:
     path = convert_pathlike(path)
     # test whether we have an AWS S3 path
     if not isinstance(path, S3Path):
         return path
     # test whether AWS credentials are present
     global AWS_CREDENTIALS_PRESENT
 
     if AWS_CREDENTIALS_PRESENT is not None:
         anon = AWS_CREDENTIALS_PRESENT
     else:
         if path.fs.key is not None and path.fs.secret is not None:
             anon = False
         else:
-            # we can do
-            # path.fs.connect()
-            # and check path.fs.session._credentials, but it is slower
+            # we could do path.fs.connect()
+            # and check path.fs.session._credentials, but it'd be slower
             session = botocore.session.get_session()
             credentials = session.get_credentials()
             if credentials is None or credentials.access_key is None:
                 anon = True
             else:
                 anon = False
             # cache credentials and reuse further
             AWS_CREDENTIALS_PRESENT = anon
 
     # test whether we are on hosted storage or not
     path_str = path.as_posix()
-    is_hosted_storage = path_str.startswith(hosted_buckets)
+    is_hosted_storage = path_str.startswith(HOSTED_BUCKETS)
 
     if not is_hosted_storage:
         # make anon request if no credentials present
         return UPath(path, cache_regions=True, anon=anon)
 
     root_folder = "/".join(path_str.replace("s3://", "").split("/")[:2])
 
@@ -648,15 +729,15 @@
         path,
         key=credentials["key"],
         secret=credentials["secret"],
         token=credentials["token"],
     )
 
 
-def get_stat_file_cloud(stat: Dict) -> Tuple[int, str, str]:
+def get_stat_file_cloud(stat: dict) -> tuple[int, str, str]:
     size = stat["size"]
     # small files
     if "-" not in stat["ETag"]:
         # only store hash for non-multipart uploads
         # we can't rapidly validate multi-part uploaded files client-side
         # we can add more logic later down-the-road
         hash = b16_to_b64(stat["ETag"])
@@ -665,15 +746,15 @@
         stripped_etag, suffix = stat["ETag"].split("-")
         suffix = suffix.strip('"')
         hash = f"{b16_to_b64(stripped_etag)}-{suffix}"
         hash_type = "md5-n"  # this is the S3 chunk-hashing strategy
     return size, hash, hash_type
 
 
-def get_stat_dir_cloud(path: UPath) -> Tuple[int, str, str, int]:
+def get_stat_dir_cloud(path: UPath) -> tuple[int, str, str, int]:
     sizes = []
     md5s = []
     objects = path.fs.find(path.as_posix(), detail=True)
     if path.protocol == "s3":
         accessor = "ETag"
     elif path.protocol == "gs":
         accessor = "md5Hash"
@@ -697,27 +778,40 @@
     root_upath = convert_pathlike(root)
     root_string = root_upath.as_posix()  # type: ignore
     # we currently touch a 0-byte file in the root of a hosted storage location
     # ({storage_root}/.lamindb/_is_initialized) during storage initialization
     # since path.fs.find raises a PermissionError on empty hosted
     # subdirectories (see lamindb_setup/core/_settings_storage/init_storage).
     n_offset_objects = 1  # because of touched dummy file, see mark_storage_root()
-    if account_for_sqlite_file:
-        n_offset_objects += 1  # because of SQLite file
-    objects = root_upath.fs.find(root_string)
+    if root_string.startswith(HOSTED_BUCKETS):
+        # in hosted buckets, count across entire root
+        directory_string = root_string
+        # the SQLite file is not in the ".lamindb" directory
+        if account_for_sqlite_file:
+            n_offset_objects += 1  # because of SQLite file
+    else:
+        # in any other storage location, only count in .lamindb
+        if not root_string.endswith("/"):
+            root_string += "/"
+        directory_string = root_string + ".lamindb"
+    objects = root_upath.fs.find(directory_string)
     n_objects = len(objects)
     n_diff = n_objects - n_offset_objects
     ask_for_deletion = (
         "delete them prior to deleting the instance"
         if raise_error
         else "consider deleting them"
     )
+    hint = "'./lamindb/_is_initialized' "
+    if n_offset_objects == 2:
+        hint += "& SQLite file"
+    hint += " ignored"
     message = (
-        f"Storage location contains {n_objects} objects "
-        f"({n_offset_objects} ignored) - {ask_for_deletion}\n{objects}"
+        f"Storage {directory_string} contains {n_objects} objects "
+        f"({hint}) - {ask_for_deletion}\n{objects}"
     )
     if n_diff > 0:
         if raise_error:
             raise InstanceNotEmpty(message)
         else:
             logger.warning(message)
     return n_diff
```

### Comparing `lamindb_setup-0.70.0/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.71.0/tests/hub-cloud/test_connect_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import os
-from postgrest.exceptions import APIError
+
+import lamindb_setup as ln_setup
 import pytest
-from laminhub_rest.core.collaborator._add_collaborator import add_collaborator
-from laminhub_rest.core.collaborator._delete_collaborator import delete_collaborator
 from lamindb_setup._connect_instance import InstanceNotFoundError
-import lamindb_setup as ln_setup
 from lamindb_setup.core._hub_client import connect_hub_with_auth
 from lamindb_setup.core._hub_crud import update_instance
-
+from laminhub_rest.core.collaborator._add_collaborator import add_collaborator
+from laminhub_rest.core.collaborator._delete_collaborator import delete_collaborator
+from postgrest.exceptions import APIError
 
 # @pytest.fixture
 # def create_remote_test_instance():
 #     ln_setup.login("testuser1")
 #     ln_setup.init(storage="s3://lamindb-ci/load_remote_instance", _test=True)
 #     yield
 #     ln_setup.delete("load_remote_instance", force=True)
@@ -63,52 +65,52 @@
         ln_setup.login("testuser1@lamin.ai")
         ln_setup.connect(
             "https://lamin.ai/laminlabs/static-test-instance-private-sqlite", _test=True
         )
         admin_hub = connect_hub_with_auth()
         # make the instance private
         update_instance(
-            instance_id=ln_setup.settings.instance.id,
+            instance_id=ln_setup.settings.instance._id,
             instance_fields={"public": False},
             client=admin_hub,
         )
         # attempt to load instance with non-collaborator user
         ln_setup.login("testuser2")
         with pytest.raises(InstanceNotFoundError):
             ln_setup.connect(
                 "https://lamin.ai/laminlabs/static-test-instance-private-sqlite",
                 _test=True,
             )
         # make the instance public
         update_instance(
-            instance_id=ln_setup.settings.instance.id,
+            instance_id=ln_setup.settings.instance._id,
             instance_fields={"public": True},
             client=admin_hub,
         )
         # load instance with non-collaborator user, should work now
         ln_setup.connect(
             "https://lamin.ai/laminlabs/static-test-instance-private-sqlite", _test=True
         )
         # make the instance private again
         update_instance(
-            instance_id=ln_setup.settings.instance.id,
+            instance_id=ln_setup.settings.instance._id,
             instance_fields={"public": False},
             client=admin_hub,
         )
 
 
 def test_connect_with_db_parameter():
     if os.getenv("LAMIN_ENV") == "prod":
         # take a write-level access collaborator
         ln_setup.login("testuser1")
         # test load from hub
         ln_setup.connect("laminlabs/lamindata", _test=True)
         assert "root" in ln_setup.settings.instance.db
         # test load from provided db argument
-        db = "postgresql://testdbuser:testpwd@database2.cmyfs24wugc3.us-east-1.rds.amazonaws.com:5432/db1"  # noqa
+        db = "postgresql://testdbuser:testpwd@database2.cmyfs24wugc3.us-east-1.rds.amazonaws.com:5432/db1"
         ln_setup.connect("laminlabs/lamindata", db=db, _test=True)
         assert "testdbuser" in ln_setup.settings.instance.db
         # test ignore loading from cache because hub result has >read access
         ln_setup.connect("laminlabs/lamindata", _test=True)
         assert "root" in ln_setup.settings.instance.db
 
         # now take a user that has no collaborator status
```

### Comparing `lamindb_setup-0.70.0/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.71.0/tests/hub-cloud/test_init_instance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,25 @@
+from __future__ import annotations
+
 from pathlib import Path
 from uuid import UUID
 
-import pytest
-
 import lamindb_setup as ln_setup
+import pytest
 from lamindb_setup.core._hub_client import connect_hub_with_auth
 from lamindb_setup.core._hub_core import _connect_instance
 from lamindb_setup.core._hub_crud import (
     Client,
     select_account_by_handle,
     select_instance_by_name,
 )
 
 pgurl = "postgresql://postgres:pwd@0.0.0.0:5432/pgtest"
 
 
-def delete_instance(
-    id: str,
-    client: Client,
-):
-    data = client.table("instance").delete().eq("id", id).execute().data
-    if len(data) == 0:
-        return None
-    return data[0]
-
-
 @pytest.fixture
 def get_hub_client():
     ln_setup.login("testuser2")
     hub = connect_hub_with_auth()
     yield hub
     hub.auth.sign_out()
 
@@ -50,15 +41,15 @@
     assert instance["db"].startswith("postgresql://none:none")
     assert instance["name"] == instance_name
     assert instance["db_scheme"] == "postgresql"
     assert instance["db_host"] == "0.0.0.0"
     assert instance["db_port"] == 5432
     assert instance["db_database"] == "pgtest"
     # client checks
-    assert ln_setup.settings.instance.id == UUID(instance["id"])
+    assert ln_setup.settings.instance._id == UUID(instance["id"])
     assert ln_setup.settings.instance.name == "pgtest"
     assert not ln_setup.settings.instance.storage.type_is_cloud
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "postgresql"
     assert ln_setup.settings.instance.db == pgurl
     assert (
         ln_setup.settings.instance.storage.root.as_posix()
@@ -88,28 +79,28 @@
         handle=ln_setup.settings.instance.owner, client=hub
     )
     instance = select_instance_by_name(
         account_id=account["id"],
         name=ln_setup.settings.instance.name,
         client=hub,
     )
-    assert ln_setup.settings.instance.id == UUID(instance["id"])
+    assert ln_setup.settings.instance._id == UUID(instance["id"])
     assert ln_setup.settings.storage.type_is_cloud
     assert (
         str(ln_setup.settings.storage.root)
         == "s3://lamindb-ci/init_instance_cloud_aws_us"
     )
     assert (
         ln_setup.settings.storage.root_as_str
         == "s3://lamindb-ci/init_instance_cloud_aws_us"
     )
     assert ln_setup.settings.storage.region == "us-west-1"
     assert (
         str(ln_setup.settings.instance._sqlite_file)
-        == f"s3://lamindb-ci/init_instance_cloud_aws_us/{ln_setup.settings.instance.id.hex}.lndb"  # noqa
+        == f"s3://lamindb-ci/init_instance_cloud_aws_us/{ln_setup.settings.instance._id.hex}.lndb"
     )
 
 
 def test_init_instance_cloud_aws_europe():
     # do the same for an S3 bucket in Europe
     ln_setup.init(
         storage="s3://lndb-setup-ci-eu-central-1",
@@ -117,41 +108,29 @@
         _test=True,
     )
     assert ln_setup.settings.instance._id is not None
     assert ln_setup.settings.storage.region == "eu-central-1"
     assert ln_setup.settings.instance.name == "lamindb-ci-europe"
     assert (
         str(ln_setup.settings.instance._sqlite_file)
-        == f"s3://lndb-setup-ci-eu-central-1/{ln_setup.settings.instance.id.hex}.lndb"
+        == f"s3://lndb-setup-ci-eu-central-1/{ln_setup.settings.instance._id.hex}.lndb"
     )
 
 
 def test_init_instance_sqlite():
     ln_setup.init(
         storage="./mydatasqlite",
         name="local-sqlite-instance",
         _test=True,
     )
-    ln_setup.register(_test=True)
-    hub = connect_hub_with_auth()
-    account = select_account_by_handle(
-        handle=ln_setup.settings.instance.owner, client=hub
-    )
-    instance = select_instance_by_name(
-        account_id=account["id"],
-        name=ln_setup.settings.instance.name,
-        client=hub,
-    )
-    assert ln_setup.settings.instance.id == UUID(instance["id"])
     assert ln_setup.settings.instance.name == "local-sqlite-instance"
     assert not ln_setup.settings.instance.storage.type_is_cloud
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "sqlite"
     ln_setup.delete("local-sqlite-instance", force=True)
-    delete_instance(instance["id"], hub)
 
 
 def test_init_invalid_name():
     with pytest.raises(ValueError) as error:
         ln_setup.init(storage="./invalidname", name="invalid/name")
     assert (
         error.exconly()
```

### Comparing `lamindb_setup-0.70.0/tests/hub-local/conftest.py` & `lamindb_setup-0.71.0/tests/hub-local/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from __future__ import annotations
+
 import os
 
 from lamin_utils import logger
-
 from laminhub_rest.dev._setup_local_hub import setup_local_hub
 
-
 pytest_plugins = [
     "laminhub_rest.test.fixtures.user",
     "laminhub_rest.test.fixtures.run_id",
 ]
 
 local_setup_state = setup_local_hub()
```

### Comparing `lamindb_setup-0.70.0/tests/hub-local/test_all.py` & `lamindb_setup-0.71.0/tests/hub-local/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
+from __future__ import annotations
+
 import os
 from uuid import UUID, uuid4
+
+import lamindb_setup as ln_setup
 import pytest
-from lamindb_setup.core._hub_utils import LaminDsnModel
 from gotrue.errors import AuthApiError
-from postgrest.exceptions import APIError
-import lamindb_setup as ln_setup
-from lamindb_setup.core._settings_instance import InstanceSettings
 from lamindb_setup.core._hub_client import (
     Environment,
     connect_hub_with_auth,
 )
 from lamindb_setup.core._hub_core import (
-    init_storage,
-    init_instance,
     connect_instance,
+    init_instance,
+    init_storage,
     sign_in_hub,
     sign_up_local_hub,
 )
 from lamindb_setup.core._hub_crud import (
+    insert_db_user,
     select_collaborator,
     select_db_user_by_instance,
     select_instance_by_name,
     update_instance,
-    insert_db_user,
 )
-from laminhub_rest.core.collaborator._add_collaborator import add_collaborator_by_ids
 
 # typing
 # from lamindb.dev import UserSettings
 # from supabase import Client
-from lamindb_setup.core._hub_utils import LaminDsn
+from lamindb_setup.core._hub_utils import LaminDsn, LaminDsnModel
+from lamindb_setup.core._settings_instance import InstanceSettings
+from lamindb_setup.core._settings_save import save_user_settings
 from lamindb_setup.core._settings_storage import base62
 from lamindb_setup.core._settings_storage import init_storage as init_storage_base
-from lamindb_setup.core._settings_save import save_user_settings
 from lamindb_setup.core._settings_user import UserSettings
+from laminhub_rest.core.collaborator._add_collaborator import add_collaborator_by_ids
+from postgrest.exceptions import APIError
 
 
 def sign_up_user(email: str, handle: str, save_as_settings: bool = False):
     """Sign up user."""
     from lamindb_setup.core._hub_core import sign_up_local_hub
 
     result_or_error = sign_up_local_hub(email)
@@ -112,15 +114,17 @@
     admin_client, usettings = create_testadmin1_session
     instance_id = uuid4()
     db_str = "postgresql://postgres:pwd@fakeserver.xyz:5432/mydb"
     isettings = InstanceSettings(
         id=instance_id,
         owner=usettings.handle,
         name="myinstance",
-        storage=init_storage_base("s3://lamindb-ci/myinstance"),
+        storage=init_storage_base(
+            "s3://lamindb-ci/myinstance", instance_id=instance_id
+        ),
         db=db_str,
     )
     init_instance(isettings)
     # test loading it
     with pytest.raises(PermissionError) as error:
         ln_setup.connect("testadmin1/myinstance", _test=True)
     assert error.exconly().startswith(
@@ -252,15 +256,15 @@
 def test_connect_instance(create_myinstance, create_testadmin1_session):
     # trigger return for inexistent handle
     assert "account-not-exists" == connect_instance(
         owner="testusr1",  # testadmin1 with a typo
         name=create_myinstance["name"],
     )
     # trigger misspelled name
-    assert "instance-not-reachable" == connect_instance(
+    assert "instance-not-found" == connect_instance(
         owner="testadmin1",
         name="inexistent-name",  # inexistent name
     )
     # make instance public so that we can also test connection string
     client, _ = create_testadmin1_session
     update_instance(
         instance_id=create_myinstance["id"],
@@ -313,19 +317,17 @@
     ln_setup.settings.user.password = correct_password
     connect_instance(
         owner="testadmin1",
         name=create_myinstance["name"],
     )
 
 
-def test_init_storage(create_testadmin1_session):
-    client, _ = create_testadmin1_session
-    storage_id = init_storage(ssettings=init_storage_base("s3://lamindb-ci/myinstance"))
-    assert isinstance(storage_id, UUID)
-
-
 def test_init_storage_with_non_existing_bucket(create_testadmin1_session):
     from botocore.exceptions import ClientError
 
     with pytest.raises(ClientError) as error:
-        init_storage(ssettings=init_storage_base("s3://non_existing_storage_root"))
+        init_storage(
+            ssettings=init_storage_base(
+                "s3://non_existing_storage_root", instance_id=uuid4()
+            )
+        )
     assert error.exconly().endswith("Not Found")
```

### Comparing `lamindb_setup-0.70.0/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.71.0/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 import os
-import pytest
+
 import lamindb_setup as ln_setup
+import pytest
 from gotrue.errors import AuthRetryableError
 from lamindb_setup import login, settings
 from lamindb_setup.core._hub_core import (
     connect_instance,
     sign_in_hub,
 )
```

### Comparing `lamindb_setup-0.70.0/tests/storage/test_storage_access.py` & `lamindb_setup-0.71.0/tests/storage/test_storage_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
+
 import os
 from uuid import UUID
-import pytest
+
 import lamindb_setup as ln_setup
+import pytest
 from lamindb_setup.core._hub_client import connect_hub_with_auth
 from lamindb_setup.core._hub_crud import (
     select_account_by_handle,
     select_instance_by_name,
 )
 
 
@@ -39,9 +42,9 @@
     # Alex doesn't fully understand why we're testing the load from hub, here, but OK
     client = connect_hub_with_auth()
     account = select_account_by_handle("laminlabs", client)
     instance = select_instance_by_name(
         account["id"], ln_setup.settings.instance.name, client
     )
     client.auth.sign_out()
-    assert ln_setup.settings.instance.id == UUID(instance["id"])
+    assert ln_setup.settings.instance._id == UUID(instance["id"])
     ln_setup.close()
```

### Comparing `lamindb_setup-0.70.0/tests/storage/test_storage_basis.py` & `lamindb_setup-0.71.0/tests/storage/test_storage_basis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from lamindb_setup.core.upath import extract_suffix_from_path
+from __future__ import annotations
+
 from pathlib import Path
 
+from lamindb_setup.core.upath import extract_suffix_from_path
+
 
 def test_extract_suffix_from_path():
     # this is a collection of path, stem, suffix tuples
     collection = [
         ("a", ""),
         ("a.txt", ".txt"),
         ("a.123", ""),  # digits are no valid suffixes
```

### Comparing `lamindb_setup-0.70.0/tests/storage/test_storage_stats.py` & `lamindb_setup-0.71.0/tests/storage/test_storage_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from lamindb_setup.core.upath import get_stat_dir_cloud, UPath, compute_file_tree
+from __future__ import annotations
+
+from lamindb_setup.core.upath import UPath, compute_file_tree, get_stat_dir_cloud
 
 
 def test_get_stat_dir_cloud_aws():
     string_path = "s3://lamindb-dev-datasets/iris_studies/study0_raw_images"
     path = UPath(string_path, anon=True)
     _, n_objects_file_tree = compute_file_tree(path)
     size, hash, hash_type, n_objects = get_stat_dir_cloud(path)
```

### Comparing `lamindb_setup-0.70.0/PKG-INFO` & `lamindb_setup-0.71.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.70.0
+Version: 0.71.0
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
 Requires-Dist: pydantic[dotenv]<2.0.0
 Requires-Dist: appdirs<2.0.0
 Requires-Dist: requests
 Requires-Dist: universal_pathlib==0.1.4
 Requires-Dist: botocore<2.0.0
 Requires-Dist: supabase==2.2.1
-Requires-Dist: s3fs ; extra == "aws"
+Requires-Dist: urllib3<2 ; extra == "aws"
+Requires-Dist: aiobotocore[boto3]>=2.5.4,<3.0.0 ; extra == "aws"
+Requires-Dist: s3fs>=2023.12.2,<=2024.3.1 ; extra == "aws"
 Requires-Dist: pyjwt<3.0.0 ; extra == "dev"
 Requires-Dist: psycopg2-binary ; extra == "dev"
 Requires-Dist: python-dotenv ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "dev"
 Requires-Dist: pandas ; extra == "dev"
 Requires-Dist: django-schema-graph ; extra == "erdiagram"
-Requires-Dist: faker ; extra == "hub"
+Requires-Dist: gcsfs>=2023.12.2,<=2024.3.1 ; extra == "gcp"
 Project-URL: Home, https://github.com/laminlabs/lamindb-setup
 Provides-Extra: aws
 Provides-Extra: dev
 Provides-Extra: erdiagram
-Provides-Extra: hub
+Provides-Extra: gcp
 
 [![codecov](https://codecov.io/gh/laminlabs/lamindb-setup/branch/main/graph/badge.svg)](https://codecov.io/gh/laminlabs/lamindb-setup)
 
 # lamindb-setup: Setup LaminDB
 
 - User [docs](https://lamin.ai/docs)
 - Developer [docs](https://lamindb-setup-htry.netlify.app/)
```

