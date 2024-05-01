# Comparing `tmp/zer1t0_aze-0.0.7.tar.gz` & `tmp/zer1t0_aze-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0_aze-0.0.7.tar", last modified: Mon Apr 29 21:21:38 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.8.tar", last modified: Wed May  1 19:39:08 2024, max compression
```

## Comparing `zer1t0_aze-0.0.7.tar` & `zer1t0_aze-0.0.8.tar`

### file list

```diff
@@ -1,85 +1,48 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.594982 zer1t0_aze-0.0.7/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2414 2024-04-29 21:21:38.594982 zer1t0_aze-0.0.7/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1994 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.578982 zer1t0_aze-0.0.7/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      767 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/arm_api.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_brute_add_app_secret.py
--rw-rw-r--   0 user      (1000) user      (1000)     3167 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_brute_blob_containers.py
--rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_brute_passwords.py
--rw-rw-r--   0 user      (1000) user      (1000)     6867 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_brute_service_subdomains.py
--rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_brute_usernames.py
--rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_get_tenant_domains.py
--rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_get_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     3369 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_list_blobs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1131 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_list_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)      800 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_list_sp_app_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)     9596 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_search_token_in_cache.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)       80 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/error.py
--rw-rw-r--   0 user      (1000) user      (1000)      754 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/graph_api.py
--rw-rw-r--   0 user      (1000) user      (1000)     1248 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/permutations.py
--rw-rw-r--   0 user      (1000) user      (1000)      817 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      679 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/request_az.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)     2768 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/tokens.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-29 21:21:38.594982 zer1t0_aze-0.0.7/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1475 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.594982 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2414 2024-04-29 21:21:38.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     2613 2024-04-29 21:21:38.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/az-get-login-info
--rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/az-inspect-token
--rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/az-login-with-token
--rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/az-tenant-id
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/az-whoami
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.586982 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.594982 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/az_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.590982 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-29 21:21:38.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/dependency_links.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 21:21:38.594982 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/dist/
--rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
--rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
--rw-rw-r--   0 user      (1000) user      (1000)      864 2024-04-29 21:21:38.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-29 21:21:38.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-29 21:20:29.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-29 21:21:38.000000 zer1t0_aze-0.0.7/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-01 19:39:08.661866 zer1t0_aze-0.0.8/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2816 2024-05-01 19:39:08.657866 zer1t0_aze-0.0.8/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2396 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-01 19:39:08.657866 zer1t0_aze-0.0.8/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      767 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/arm_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_add_app_secret.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3167 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_blob_containers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7007 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      787 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_administrative_unit_members.py
+-rw-rw-r--   0 user      (1000) user      (1000)      804 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_administrative_unit_role_members.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3369 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_blobs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1109 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_sp_app_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)      813 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_user_memberof.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9478 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_search_token_in_cache.py
+-rw-rw-r--   0 user      (1000) user      (1000)      746 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_show_ad_role.py
+-rw-rw-r--   0 user      (1000) user      (1000)      771 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_show_administrative_unit.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1814 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/graph_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1248 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/permutations.py
+-rw-rw-r--   0 user      (1000) user      (1000)      817 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      960 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/request_az.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2882 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/tokens.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-01 19:39:08.661866 zer1t0_aze-0.0.8/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1653 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-01 19:39:08.657866 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2816 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1042 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1205 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0_aze-0.0.7/LICENSE` & `zer1t0_aze-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/PKG-INFO` & `zer1t0_aze-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,41 @@
-Metadata-Version: 2.1
-Name: zer1t0-aze
-Version: 0.0.7
-Summary: Enhance azure cli
-Home-page: https://gitlab.com/Zer1t0/aze
-Author: Eloy Pérez González
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: msal_extensions
-Requires-Dist: dnspython
-
 # AZE (Azure Cli Enhacement)
 
 Extended utilities for azure management.
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
 
 ## Commands
 
 AZE includes the following commands, many of them require to be
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
-- **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
+- **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains (No auth).
 - **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-list-blobs**: List blobs of container from URL (No auth).
-- **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
+- **az-list-administrative-unit-members**: List Administrative Unit members (Auth).
+- **az-list-administrative-unit-role-members**: List Administrative Unit scoped role members (Auth).
+- **az-list-role-assignment**: List roles without requiring a graph access token. (Auth)
+- **az-list-sp-app-role-assignment**: List App roles for a service principal. (Auth)
+- **az-list-user-memberof**: List membership of user, both groups and administrative units. (Auth)
 - **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
-- **az-list-sp-app-role-assignment**: List App roles for a service principal (Auth).
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
-- **az-whoami**: Shorcut for "az ad signed-in-user show" (Auth).
+- **az-show-ad-role**: Show Entra ID role. (Auth)
+- **az-show-administrative-unit**: Show Administrative Unit. (Auth)
+- **az-whoami**: Shorcut for "az ad signed-in-user show". (Auth)
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zer1t0_aze-0.0.7/aze/arm_api.py` & `zer1t0_aze-0.0.8/aze/arm_api.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_brute_add_app_secret.py` & `zer1t0_aze-0.0.8/aze/az_brute_add_app_secret.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_brute_blob_containers.py` & `zer1t0_aze-0.0.8/aze/az_brute_blob_containers.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_brute_passwords.py` & `zer1t0_aze-0.0.8/aze/az_brute_passwords.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_brute_service_subdomains.py` & `zer1t0_aze-0.0.8/aze/az_brute_service_subdomains.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	"azurewebsites.net": "App Services",
 	"p.azurewebsites.net": "App Services",
 	"cloudapp.net": "App Services",
 	"file.core.windows.net": "Storage Accounts - Files",
 	"blob.core.windows.net": "Storage Accounts - Blobs",
 	"queue.core.windows.net": "Storage Accounts - Queues",
 	"table.core.windows.net": "Storage Accounts - Tables",
+    "dfs.core.windows.net": "Storage Accounts - Data Lake",
 	"mail.protection.outlook.com": "Email",
 	"sharepoint.com": "SharePoint",
 	"redis.cache.windows.net": "Databases-Redis",
 	"documents.azure.com": "Databases-Cosmos DB",
 	"database.windows.net": "Databases-MSSQL",
 	"vault.azure.net": "Key Vaults",
 	"azureedge.net": "CDN",
@@ -41,21 +42,25 @@
         "p.azurewebsites.net",
         "cloudapp.net",
     ],
 	"file": ["file.core.windows.net"],
     "blob": ["blob.core.windows.net"],
 	"queue": ["queue.core.windows.net"],
     "table": ["table.core.windows.net"],
-    "lake": ["azuredatalakestore.net"],
+    "lake": [
+        "azuredatalakestore.net",
+        "dfs.core.windows.net",
+    ],
     "storage": [
         "file.core.windows.net",
         "blob.core.windows.net",
         "queue.core.windows.net",
         "table.core.windows.net",
-        "azuredatalakestore.net"
+        "azuredatalakestore.net",
+        "dfs.core.windows.net",
     ],
     "email": ["mail.protection.outlook.com"],
     "mail": ["mail.protection.outlook.com"],
     "sharepoint": ["sharepoint.com"],
 	"redis": ["redis.cache.windows.net"],
     "cosmos": ["documents.azure.com"],
     "mssql": ["database.windows.net"],
```

### Comparing `zer1t0_aze-0.0.7/aze/az_brute_usernames.py` & `zer1t0_aze-0.0.8/aze/az_brute_usernames.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_get_login_info.py` & `zer1t0_aze-0.0.8/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_get_tenant_domains.py` & `zer1t0_aze-0.0.8/aze/az_get_tenant_domains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_get_tenant_id.py` & `zer1t0_aze-0.0.8/aze/az_get_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_inspect_token.py` & `zer1t0_aze-0.0.8/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_list_blobs.py` & `zer1t0_aze-0.0.8/aze/az_list_blobs.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_list_role_assignment.py` & `zer1t0_aze-0.0.8/aze/az_list_role_assignment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 from . import arm_api
 import json
 from . import profile
 from .tokens import search_token_for_subscription
-from . import arm_api
 
 def parse_args():
     parser = argparse.ArgumentParser(
         "List roles without requiring a graph access token."
     )
     args = parser.parse_args()
     return args
```

### Comparing `zer1t0_aze-0.0.7/aze/az_list_sp_app_role_assignment.py` & `zer1t0_aze-0.0.8/aze/az_list_sp_app_role_assignment.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/az_login_with_token.py` & `zer1t0_aze-0.0.8/aze/az_login_with_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,14 @@
     refresh_token = args.refresh_token
     tenant = args.tenant
 
 
     resp_subscriptions = []
     if access_tokens:
         t_infos = [TokenInformation(at) for at in access_tokens]
-        for t_info in t_infos:
-            if t_info.endpoint == "https://management.core.windows.net/"\
-               or t_info["aud"] == "https://management.azure.com/":
-                resp_subscriptions = arm_api.list_subscriptions(
-                    t_info.access_token
-                )
-                break
     elif refresh_token:
         if not tenant:
             utils.eprint("--tenant required when using refresh token")
             return -1
         tenant_id = resolve_tenant_id(tenant)
         tokens = request_tokens_from_refresh(tenant_id, refresh_token)
 
@@ -63,14 +56,22 @@
             scope=tokens["scope"],
             client_info=tokens["client_info"],
             expires_in=tokens["expires_in"],
             ext_expires_in=tokens["ext_expires_in"],
         )
         t_infos = [at_info]
 
+    for t_info in t_infos:
+        if t_info.endpoint == "https://management.core.windows.net/"\
+           or t_info["aud"] == "https://management.azure.com/":
+            resp_subscriptions = arm_api.list_subscriptions(
+                t_info.access_token
+            )
+            break
+
     token_cache = load_token_cache()
     store_tokens(t_infos, token_cache)
     set_subscriptions(t_infos[0], resp_subscriptions)
 
 
 
 
@@ -169,15 +170,19 @@
         "refresh_token": refresh_token,
         "scope": "https://management.core.windows.net//.default offline_access openid profile",
     }
 
     resp = requests.post(url, data)
     if resp.status_code != 200:
         raise AzeError(
-            "Unable to get access token: error code {}".format(resp.status_code)
+            "Unable to get access token, error {}: {} - {}".format(
+                resp.status_code,
+                resp.json().get("error", ""),
+                resp.json().get("error_description", "")
+            )
         )
 
     return resp.json()
 
 
 def store_tokens(tokens_info, token_cache):
     if not tokens_info:
@@ -206,14 +211,25 @@
             utils.add_b64_padding(jwt_payload)
         ).decode())
 
         self._scope = scope
         self.id_token = id_token
         self.refresh_token = refresh_token
 
+        self.tenant_id = self._info["tid"]
+
+        if "upn" in self._info:
+            self.username = self._info["upn"]
+            self.account_id = self._info["oid"]
+        else:
+            self.username = self._info["appid"]
+            self.account_id = self._info["appid"]
+
+        self.endpoint = aud_to_endpoint(self._info["aud"])
+
         if client_info:
             self.client_info = client_info
         else:
             self.client_info = base64.b64encode(json.dumps({
                 "uid": self.account_id,
                 "utid": self.tenant_id,
             }).encode()).decode()
@@ -229,46 +245,14 @@
         else:
             self.ext_expires_in = self.expires_in
 
 
     def __getitem__(self,key):
         return self._info[key]
 
-    @property
-    def account_id(self):
-        if self._info["idtyp"] == "app":
-            return self._info["appid"]
-        else:
-            return self._info["oid"]
-
-    @property
-    def username(self):
-        if self._info["idtyp"] == "app":
-            return self._info["appid"]
-        else:
-            return self._info["upn"]
-
-    @property
-    def endpoint(self):
-        endpoint = self._info["aud"]
-
-        # Seems that management.azure.com is the new endpoint
-        # but still not used by Azure Cli, so we replace it
-        # with the old endpoint to make it compatible
-        if endpoint.startswith("https://management.azure.com"):
-            endpoint = "https://management.core.windows.net/"
-        if not endpoint.endswith("/"):
-            endpoint += "/"
-        return endpoint
-
-
-    @property
-    def tenant_id(self):
-        return self._info["tid"]
-
     def get(self, *args, **kwargs):
         return self._info.get(*args, **kwargs)
 
     @property
     def scopes(self):
         if self._scope:
             scopes = self._scope.split()
@@ -281,15 +265,22 @@
                         scopes.append(scope)
                     else:
                         scopes.append("{}/{}".format(endpoint, scope))
             except KeyError:
                 pass
         return scopes
 
+def aud_to_endpoint(aud):
+    # Seems that management.azure.com is the new endpoint
+    # but still not used by Azure Cli, so we replace it
+    # with the old endpoint to make it compatible
+    if aud.startswith("https://management.azure.com"):
+        return "https://management.core.windows.net/"
 
+    return aud
 
 def create_event_from_token_info(t_info):
     scopes = t_info.scopes
     resp = {
         "token_type": "Bearer",
         "scope": scopes,
         "access_token": t_info.access_token,
```

### Comparing `zer1t0_aze-0.0.7/aze/az_search_token_in_cache.py` & `zer1t0_aze-0.0.8/aze/az_search_token_in_cache.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/graph_api.py` & `zer1t0_aze-0.0.8/aze/graph_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .request_az import request_az_api
+from .request_az import request_az_api, request_az_api_values_until_no_more
 
 
 def add_secret_to_application(access_token, app_id):
     return request_az_api(
         "https://graph.microsoft.com/v1.0/applications/{}/addPassword".format(app_id),
         access_token,
         method="POST",
@@ -21,7 +21,36 @@
 
 def list_sp_app_role_asignments(access_token, sp_id):
     return request_az_api(
         "https://graph.microsoft.com/v1.0/servicePrincipals/{}/appRoleAssignments".format(sp_id),
         access_token,
     )["value"]
 
+def list_user_memberof(access_token, user):
+    return request_az_api(
+        "https://graph.microsoft.com/v1.0/users/{}/memberOf".format(user),
+        access_token,
+    )["value"]
+
+def show_ad_role(access_token, role_id):
+    return request_az_api(
+        "https://graph.microsoft.com/v1.0/directoryRoles/{}".format(role_id),
+        access_token,
+    )
+
+def show_administrative_unit(access_token, au):
+    return request_az_api(
+        "https://graph.microsoft.com/v1.0/directory/administrativeUnits/{}".format(au),
+        access_token,
+    )
+
+def list_administrative_unit_members(access_token, au):
+    return request_az_api_values_until_no_more(
+        "https://graph.microsoft.com/v1.0/directory/administrativeUnits/{}/members".format(au),
+        access_token,
+    )
+
+def list_administrative_unit_role_members(access_token, au):
+    return request_az_api_values_until_no_more(
+        "https://graph.microsoft.com/v1.0/directory/administrativeUnits/{}/scopedRoleMembers".format(au),
+        access_token,
+    )
```

### Comparing `zer1t0_aze-0.0.7/aze/permutations.py` & `zer1t0_aze-0.0.8/aze/permutations.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/profile.py` & `zer1t0_aze-0.0.8/aze/profile.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/read_in.py` & `zer1t0_aze-0.0.8/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/aze/request_az.py` & `zer1t0_aze-0.0.8/aze/request_az.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 import requests
 from .error import AzeRequestError
 
+def request_az_api_values_until_no_more(url, access_token):
+    values = []
+    next_link = url
+    while next_link:
+        resp = request_az_api(next_link, access_token)
+        values.extend(resp["value"])
+        next_link = resp.get("@odata.nextLink", "")
+
+    return values
+
 def request_az_api(url, access_token, method="GET", json=None):
     headers = {
         "Authorization": "Bearer {}".format(access_token)
     }
 
     if method.upper() == "POST":
         req = requests.post
```

### Comparing `zer1t0_aze-0.0.7/aze/tokens.py` & `zer1t0_aze-0.0.8/aze/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,24 @@
 #         ACCOUNT = "Account"  # Not exactly a credential type, but we put it here
 #         ID_TOKEN = "IdToken"
 #         APP_METADATA = "AppMetadata"
 
 def search_token_for_subscription(subscription, scopes, token_cache=None):
     token_cache = token_cache or load_token_cache()
 
+    if subscription["id"] == subscription["tenantId"]:
+        realm = subscription["id"]
+    else:
+        realm = "organizations"
+
     accounts = search_token_in_cache(
         CredentialType.ACCOUNT,
         query={
             "username": subscription["user"]["name"],
-            "realm": subscription["tenantId"],
+            "realm": realm,
         },
         token_cache=token_cache,
     )
     if not accounts:
         raise AzeError("Unable to find account for subscription")
 
     account = accounts[0]
```

### Comparing `zer1t0_aze-0.0.7/aze/utils.py` & `zer1t0_aze-0.0.8/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.7/setup.py` & `zer1t0_aze-0.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,20 +21,25 @@
     "az-brute-usernames",
     "az-brute-service-subdomains",
     "az-brute-blob-containers",
     "az-get-login-info",
     "az-get-tenant-domains",
     "az-get-tenant-id",
     "az-inspect-token",
+    "az-list-administrative-unit-members",
+    "az-list-administrative-unit-role-members",
     "az-list-blobs",
     "az-list-subscriptions",
     "az-list-role-assignment",
     "az-list-sp-app-role-assignment",
+    "az-list-user-memberof",
     "az-login-with-token",
     "az-search-token-in-cache",
+    "az-show-ad-role",
+    "az-show-administrative-unit",
     "az-whoami",
 ]
 
 console_scripts = [
     "{} = {}.{}:main".format(script, name, script.replace("-", "_"))
     for script in scripts
 ]
```

### Comparing `zer1t0_aze-0.0.7/zer1t0_aze.egg-info/PKG-INFO` & `zer1t0_aze-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.7
+Version: 0.0.8
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,29 +22,34 @@
 
 ## Commands
 
 AZE includes the following commands, many of them require to be
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
-- **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
+- **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains (No auth).
 - **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-list-blobs**: List blobs of container from URL (No auth).
-- **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
+- **az-list-administrative-unit-members**: List Administrative Unit members (Auth).
+- **az-list-administrative-unit-role-members**: List Administrative Unit scoped role members (Auth).
+- **az-list-role-assignment**: List roles without requiring a graph access token. (Auth)
+- **az-list-sp-app-role-assignment**: List App roles for a service principal. (Auth)
+- **az-list-user-memberof**: List membership of user, both groups and administrative units. (Auth)
 - **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
-- **az-list-sp-app-role-assignment**: List App roles for a service principal (Auth).
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
-- **az-whoami**: Shorcut for "az ad signed-in-user show" (Auth).
+- **az-show-ad-role**: Show Entra ID role. (Auth)
+- **az-show-administrative-unit**: Show Administrative Unit. (Auth)
+- **az-whoami**: Shorcut for "az ad signed-in-user show". (Auth)
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
```

