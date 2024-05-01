# Comparing `tmp/heptapod-4.6.0.tar.gz` & `tmp/heptapod-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heptapod-4.6.0.tar", last modified: Wed Mar 20 15:26:38 2024, max compression
+gzip compressed data, was "heptapod-4.7.0.tar", last modified: Wed May  1 15:37:50 2024, max compression
```

## Comparing `heptapod-4.6.0.tar` & `heptapod-4.7.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.920232 heptapod-4.6.0/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-07-07 20:49:25.000000 heptapod-4.6.0/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-07-07 20:49:25.000000 heptapod-4.6.0/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3813 2024-03-20 15:26:38.920232 heptapod-4.6.0/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3145 2022-07-07 20:49:25.000000 heptapod-4.6.0/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.907232 heptapod-4.6.0/heptapod/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-03-20 15:25:57.000000 heptapod-4.6.0/heptapod/VERSION
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      403 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.909232 heptapod-4.6.0/heptapod/gitlab/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7238 2024-01-20 11:37:32.000000 heptapod-4.6.0/heptapod/gitlab/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2447 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/change.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16323 2024-02-13 21:08:07.000000 heptapod-4.6.0/heptapod/gitlab/hooks.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3979 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/prune_reasons.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      940 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.909232 heptapod-4.6.0/heptapod/gitlab/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1214 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/tests/test_change.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4275 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/gitlab/tests/test_hooks_inner.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17239 2024-01-20 11:37:33.000000 heptapod-4.6.0/heptapod/gitlab/tests/test_hooks_integration.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      672 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/heptapod.example.hgrc
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.911232 heptapod-4.6.0/heptapod/hooks/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       77 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/check_publish.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      927 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/dev_util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      661 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/gitlab_mirror.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6758 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/perm.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      722 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/subrepos.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.911232 heptapod-4.6.0/heptapod/hooks/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2760 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/tests/test_check_publish.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2098 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/tests/test_check_write.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1228 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/tests/test_dev_utils.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      962 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/tests/test_gitlab_mirror.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      548 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/hooks/tests/utils.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1156 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/obsutil.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1365 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/patch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2344 2024-03-20 15:24:31.000000 heptapod-4.6.0/heptapod/required.hgrc
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.912232 heptapod-4.6.0/heptapod/testhelpers/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      475 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3452 2024-02-13 21:08:07.000000 heptapod-4.6.0/heptapod/testhelpers/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4960 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/gitlab.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3090 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/hg.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.912232 heptapod-4.6.0/heptapod/testhelpers/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1760 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/tests/test_git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      799 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/tests/test_gitlab.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2700 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/testhelpers/tests/test_repo_wrapper.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.913232 heptapod-4.6.0/heptapod/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      456 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/test_harness.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      597 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/test_package.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1201 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/test_patch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1062 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/test_util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5965 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/test_wsgi.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2356 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/tests/test_wsgi_webtest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1072 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10310 2022-07-07 20:49:25.000000 heptapod-4.6.0/heptapod/wsgi.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.908232 heptapod-4.6.0/heptapod.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3813 2024-03-20 15:26:38.000000 heptapod-4.6.0/heptapod.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2804 2024-03-20 15:26:38.000000 heptapod-4.6.0/heptapod.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-03-20 15:26:38.000000 heptapod-4.6.0/heptapod.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      189 2024-03-20 15:26:38.000000 heptapod-4.6.0/heptapod.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       18 2024-03-20 15:26:38.000000 heptapod-4.6.0/heptapod.egg-info/top_level.txt
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.913232 heptapod-4.6.0/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.915232 heptapod-4.6.0/hgext3rd/heptapod/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17105 2023-07-26 13:18:15.000000 heptapod-4.6.0/hgext3rd/heptapod/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2582 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9096 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4163 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/keep_around.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4177 2023-07-26 13:18:15.000000 heptapod-4.6.0/hgext3rd/heptapod/no_git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5068 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/special_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    48936 2024-02-13 21:08:07.000000 heptapod-4.6.0/hgext3rd/heptapod/state_maintainer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1305 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.918232 heptapod-4.6.0/hgext3rd/heptapod/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.919232 heptapod-4.6.0/hgext3rd/heptapod/tests/git/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      126 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/git/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17184 2023-07-26 13:18:15.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/git/test_inner.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      935 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    57440 2023-11-13 22:51:13.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/git/test_integration.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:26:38.919232 heptapod-4.6.0/hgext3rd/heptapod/tests/no_git/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/no_git/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2012 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/no_git/test_inner.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    43172 2023-11-13 22:51:13.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/no_git/test_integration.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3976 2023-11-13 22:51:13.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_backups.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8265 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_commands_misc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_config.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1287 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2510 2023-11-13 22:51:13.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_exchange.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      735 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_initial_import_mode.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1870 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_keep_arounds.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1221 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_patch_runsystem.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6927 2023-11-13 22:51:13.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_pull_force_topic.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3160 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_special_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3606 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/test_typed_refs.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      910 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/tests/utils.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3093 2022-07-07 20:49:25.000000 heptapod-4.6.0/hgext3rd/heptapod/topic.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6697 2023-07-26 13:18:11.000000 heptapod-4.6.0/hgext3rd/heptapod/typed_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      191 2024-03-20 15:24:31.000000 heptapod-4.6.0/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-03-20 15:26:38.920232 heptapod-4.6.0/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1144 2022-07-07 20:49:25.000000 heptapod-4.6.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.294649 heptapod-4.7.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-07-07 20:49:25.000000 heptapod-4.7.0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-07-07 20:49:25.000000 heptapod-4.7.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3813 2024-05-01 15:37:50.294649 heptapod-4.7.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3145 2022-07-07 20:49:25.000000 heptapod-4.7.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.280649 heptapod-4.7.0/heptapod/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-01 15:37:13.000000 heptapod-4.7.0/heptapod/VERSION
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      403 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.282649 heptapod-4.7.0/heptapod/gitlab/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7238 2024-01-20 11:37:32.000000 heptapod-4.7.0/heptapod/gitlab/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2447 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/change.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16323 2024-02-13 21:08:07.000000 heptapod-4.7.0/heptapod/gitlab/hooks.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3979 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/prune_reasons.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      940 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.282649 heptapod-4.7.0/heptapod/gitlab/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1214 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/tests/test_change.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4275 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/gitlab/tests/test_hooks_inner.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17239 2024-01-20 11:37:33.000000 heptapod-4.7.0/heptapod/gitlab/tests/test_hooks_integration.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      672 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/heptapod.example.hgrc
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.283649 heptapod-4.7.0/heptapod/hooks/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       77 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/check_publish.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      927 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/dev_util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      661 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/gitlab_mirror.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6758 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/perm.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      722 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/subrepos.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.284649 heptapod-4.7.0/heptapod/hooks/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2760 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/tests/test_check_publish.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2098 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/tests/test_check_write.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1228 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/tests/test_dev_utils.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      962 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/tests/test_gitlab_mirror.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      548 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/hooks/tests/utils.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1156 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/obsutil.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1365 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/patch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2344 2024-04-19 11:23:05.000000 heptapod-4.7.0/heptapod/required.hgrc
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.285649 heptapod-4.7.0/heptapod/testhelpers/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      475 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3452 2024-02-13 21:08:07.000000 heptapod-4.7.0/heptapod/testhelpers/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4960 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/gitlab.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3090 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/hg.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.285649 heptapod-4.7.0/heptapod/testhelpers/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1760 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/tests/test_git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      799 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/tests/test_gitlab.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2700 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/testhelpers/tests/test_repo_wrapper.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.286649 heptapod-4.7.0/heptapod/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      456 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/test_harness.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      597 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/test_package.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1201 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/test_patch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1062 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/test_util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5965 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/test_wsgi.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2356 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/tests/test_wsgi_webtest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1072 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10310 2022-07-07 20:49:25.000000 heptapod-4.7.0/heptapod/wsgi.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.280649 heptapod-4.7.0/heptapod.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3813 2024-05-01 15:37:50.000000 heptapod-4.7.0/heptapod.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2804 2024-05-01 15:37:50.000000 heptapod-4.7.0/heptapod.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-01 15:37:50.000000 heptapod-4.7.0/heptapod.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      184 2024-05-01 15:37:50.000000 heptapod-4.7.0/heptapod.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       18 2024-05-01 15:37:50.000000 heptapod-4.7.0/heptapod.egg-info/top_level.txt
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.286649 heptapod-4.7.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.289649 heptapod-4.7.0/hgext3rd/heptapod/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17151 2024-04-19 09:37:59.000000 heptapod-4.7.0/hgext3rd/heptapod/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2582 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9096 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4163 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/keep_around.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4177 2023-07-26 13:18:15.000000 heptapod-4.7.0/hgext3rd/heptapod/no_git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5068 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/special_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    48936 2024-02-13 21:08:07.000000 heptapod-4.7.0/hgext3rd/heptapod/state_maintainer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1305 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.292649 heptapod-4.7.0/hgext3rd/heptapod/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.292649 heptapod-4.7.0/hgext3rd/heptapod/tests/git/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      126 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/git/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17184 2023-07-26 13:18:15.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/git/test_inner.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      935 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    57440 2023-11-13 22:51:13.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/git/test_integration.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:37:50.293649 heptapod-4.7.0/hgext3rd/heptapod/tests/no_git/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/no_git/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2012 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/no_git/test_inner.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    43172 2023-11-13 22:51:13.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/no_git/test_integration.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3976 2023-11-13 22:51:13.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_backups.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8265 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_commands_misc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_config.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1287 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2510 2023-11-13 22:51:13.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_exchange.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      735 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_initial_import_mode.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1870 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_keep_arounds.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1221 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_patch_runsystem.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6927 2023-11-13 22:51:13.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_pull_force_topic.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3160 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_special_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3606 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/test_typed_refs.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      910 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/tests/utils.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3093 2022-07-07 20:49:25.000000 heptapod-4.7.0/hgext3rd/heptapod/topic.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6697 2023-07-26 13:18:11.000000 heptapod-4.7.0/hgext3rd/heptapod/typed_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      185 2024-04-19 11:23:21.000000 heptapod-4.7.0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-01 15:37:50.294649 heptapod-4.7.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1144 2022-07-07 20:49:25.000000 heptapod-4.7.0/setup.py
```

### Comparing `heptapod-4.6.0/LICENSE` & `heptapod-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/PKG-INFO` & `heptapod-4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heptapod
-Version: 4.6.0
+Version: 4.7.0
 Summary: Heptapod server-side Mercurial hooks, extension, etc.
 Home-page: https://foss.heptapod.net/heptapod/py-heptapod
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Classifier: Development Status :: 4 - Beta
```

### Comparing `heptapod-4.6.0/README.md` & `heptapod-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/branch.py` & `heptapod-4.7.0/heptapod/gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/change.py` & `heptapod-4.7.0/heptapod/gitlab/change.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/hooks.py` & `heptapod-4.7.0/heptapod/gitlab/hooks.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/prune_reasons.py` & `heptapod-4.7.0/heptapod/gitlab/prune_reasons.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/tag.py` & `heptapod-4.7.0/heptapod/gitlab/tag.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/tests/test_change.py` & `heptapod-4.7.0/heptapod/gitlab/tests/test_change.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/tests/test_hooks_inner.py` & `heptapod-4.7.0/heptapod/gitlab/tests/test_hooks_inner.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/gitlab/tests/test_hooks_integration.py` & `heptapod-4.7.0/heptapod/gitlab/tests/test_hooks_integration.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/heptapod.example.hgrc` & `heptapod-4.7.0/heptapod/heptapod.example.hgrc`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/dev_util.py` & `heptapod-4.7.0/heptapod/hooks/dev_util.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/gitlab_mirror.py` & `heptapod-4.7.0/heptapod/hooks/gitlab_mirror.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/perm.py` & `heptapod-4.7.0/heptapod/hooks/perm.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/subrepos.py` & `heptapod-4.7.0/heptapod/hooks/subrepos.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/tests/test_check_publish.py` & `heptapod-4.7.0/heptapod/hooks/tests/test_check_publish.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/tests/test_check_write.py` & `heptapod-4.7.0/heptapod/hooks/tests/test_check_write.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/tests/test_dev_utils.py` & `heptapod-4.7.0/heptapod/hooks/tests/test_dev_utils.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/tests/test_gitlab_mirror.py` & `heptapod-4.7.0/heptapod/hooks/tests/test_gitlab_mirror.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/hooks/tests/utils.py` & `heptapod-4.7.0/heptapod/hooks/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/obsutil.py` & `heptapod-4.7.0/heptapod/obsutil.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/patch.py` & `heptapod-4.7.0/heptapod/patch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/required.hgrc` & `heptapod-4.7.0/heptapod/required.hgrc`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/testhelpers/git.py` & `heptapod-4.7.0/heptapod/testhelpers/git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/testhelpers/gitlab.py` & `heptapod-4.7.0/heptapod/testhelpers/gitlab.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/testhelpers/hg.py` & `heptapod-4.7.0/heptapod/testhelpers/hg.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/testhelpers/tests/test_git.py` & `heptapod-4.7.0/heptapod/testhelpers/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/testhelpers/tests/test_gitlab.py` & `heptapod-4.7.0/heptapod/testhelpers/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/testhelpers/tests/test_repo_wrapper.py` & `heptapod-4.7.0/heptapod/testhelpers/tests/test_repo_wrapper.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/tests/test_package.py` & `heptapod-4.7.0/heptapod/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/tests/test_patch.py` & `heptapod-4.7.0/heptapod/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/tests/test_util.py` & `heptapod-4.7.0/heptapod/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/tests/test_wsgi.py` & `heptapod-4.7.0/heptapod/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/tests/test_wsgi_webtest.py` & `heptapod-4.7.0/heptapod/tests/test_wsgi_webtest.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/util.py` & `heptapod-4.7.0/heptapod/util.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod/wsgi.py` & `heptapod-4.7.0/heptapod/wsgi.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/heptapod.egg-info/PKG-INFO` & `heptapod-4.7.0/heptapod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heptapod
-Version: 4.6.0
+Version: 4.7.0
 Summary: Heptapod server-side Mercurial hooks, extension, etc.
 Home-page: https://foss.heptapod.net/heptapod/py-heptapod
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Classifier: Development Status :: 4 - Beta
```

### Comparing `heptapod-4.6.0/heptapod.egg-info/SOURCES.txt` & `heptapod-4.7.0/heptapod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/__init__.py` & `heptapod-4.7.0/hgext3rd/heptapod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,20 @@
     configitem(b'heptapod', b'no-git', False)
 
 
 cmdtable = {}
 command = registrar.command(cmdtable)
 
 
+def wrap_function(mod, name, fun):
+    if util.versiontuple() < (6, 7):
+        name = name.encode('ascii')  # hg<6.7
+    extensions.wrapfunction(mod, name, fun)
+
+
 def uipopulate(ui):
     if ui.configbool(b'heptapod', b'initial-import'):
         ui.note(b'hgext3rd.heptapod',
                 b"setting config options for initial import")
         ui.setconfig(b'heptapod', b'allow-multiple-heads', True)
         ui.setconfig(b'experimental',
                      b'topic.publish-bare-branch', False)
@@ -408,15 +414,15 @@
     if environ is None:
         environ = heptapod_env
     else:
         heptapod_env.update(environ)
     return orig(ui, cmd, environ=heptapod_env, cwd=cwd, out=out)
 
 
-extensions.wrapfunction(uimod.ui, b'_runsystem', runsystem)
+wrap_function(uimod.ui, '_runsystem', runsystem)
 
 
 def hggit_parse_hgsub(orig, lines):
     """A more robust version of .hgsub parser
 
     See heptapod#310 for an example where the conversion to Git fails
     because of the ``[subpaths]`` section.
@@ -429,15 +435,15 @@
     """
     parsed = config.config()
     parsed.parse(b'.hgsub', b"\n".join(lines))
     return collections.OrderedDict(parsed.items(b''))
 
 
 if hggit is not None:
-    extensions.wrapfunction(hggit.util, b'parse_hgsub', hggit_parse_hgsub)
+    wrap_function(hggit.util, 'parse_hgsub', hggit_parse_hgsub)
 
 
 def forbid_subrepo_get(orig, *args, **kwargs):
     raise error.Abort(b"Updating subrepos on the server side is "
                       b"not supported in this version of Heptapod and "
                       b"would be actually harmful. "
                       b"This may be reenabled in a subsequent version.")
@@ -451,26 +457,22 @@
     if not ignore_bookmarks:
         return orig(op, *args, **kwargs)
     # Not sure how important this is, but it's done in the original function
     # for the pushop in case of early return
     op.stepsdone.add(b'bookmarks')
 
 
-extensions.wrapfunction(subrepo.hgsubrepo, b'get', forbid_subrepo_get)
-extensions.wrapfunction(subrepo.gitsubrepo, b'get', forbid_subrepo_get)
-extensions.wrapfunction(subrepo.svnsubrepo, b'get', forbid_subrepo_get)
+wrap_function(subrepo.hgsubrepo, 'get', forbid_subrepo_get)
+wrap_function(subrepo.gitsubrepo, 'get', forbid_subrepo_get)
+wrap_function(subrepo.svnsubrepo, 'get', forbid_subrepo_get)
 
 
 def extsetup(ui):
     """Tweaks after all extensions went though their `uisetup`
 
     hgext3rd.heptapod is meant to be terminal, the only (debatable)
     exception being HGitaly, which could well adopt the whole of `heptapod`
     and `hgext3rd.heptapod` in the future.
     """
-    extensions.wrapfunction(exchange, b'_pullbookmarks', bookmarks_op_override)
-    extensions.wrapfunction(exchange, b'_pushbookmark', bookmarks_op_override)
-    extensions.wrapfunction(
-        exchange,
-        b'_pushb2bookmarkspart',
-        bookmarks_op_override
-    )
+    wrap_function(exchange, '_pullbookmarks', bookmarks_op_override)
+    wrap_function(exchange, '_pushbookmark', bookmarks_op_override)
+    wrap_function(exchange, '_pushb2bookmarkspart', bookmarks_op_override)
```

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/branch.py` & `heptapod-4.7.0/hgext3rd/heptapod/branch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/git.py` & `heptapod-4.7.0/hgext3rd/heptapod/git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/keep_around.py` & `heptapod-4.7.0/hgext3rd/heptapod/keep_around.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/no_git.py` & `heptapod-4.7.0/hgext3rd/heptapod/no_git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/special_ref.py` & `heptapod-4.7.0/hgext3rd/heptapod/special_ref.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/state_maintainer.py` & `heptapod-4.7.0/hgext3rd/heptapod/state_maintainer.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tag.py` & `heptapod-4.7.0/hgext3rd/heptapod/tag.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/git/test_inner.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/git/test_inner.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/git/test_integration.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/git/test_integration.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/no_git/test_inner.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/no_git/test_inner.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/no_git/test_integration.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/no_git/test_integration.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_backups.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_backups.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_commands_misc.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_commands_misc.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_config.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_default_branch.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_exchange.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_initial_import_mode.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_initial_import_mode.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_keep_arounds.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_keep_arounds.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_patch_runsystem.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_patch_runsystem.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_pull_force_topic.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_pull_force_topic.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_special_ref.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_special_ref.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/test_typed_refs.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/test_typed_refs.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/tests/utils.py` & `heptapod-4.7.0/hgext3rd/heptapod/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/topic.py` & `heptapod-4.7.0/hgext3rd/heptapod/topic.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/hgext3rd/heptapod/typed_ref.py` & `heptapod-4.7.0/hgext3rd/heptapod/typed_ref.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.6.0/setup.py` & `heptapod-4.7.0/setup.py`

 * *Files identical despite different names*

