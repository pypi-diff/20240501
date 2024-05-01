# Comparing `tmp/testfixtures-8.1.0.tar.gz` & `tmp/testfixtures-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testfixtures-8.1.0.tar", last modified: Fri Mar  1 08:18:45 2024, max compression
+gzip compressed data, was "testfixtures-8.2.0.tar", last modified: Wed May  1 07:55:08 2024, max compression
```

## Comparing `testfixtures-8.1.0.tar` & `testfixtures-8.2.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.723653 testfixtures-8.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-03-01 08:18:36.000000 testfixtures-8.1.0/.carthorse.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.711653 testfixtures-8.1.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2024-03-01 08:18:36.000000 testfixtures-8.1.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2024-03-01 08:18:36.000000 testfixtures-8.1.0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-03-01 08:18:36.000000 testfixtures-8.1.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-03-01 08:18:36.000000 testfixtures-8.1.0/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40267 2024-03-01 08:18:36.000000 testfixtures-8.1.0/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2024-03-01 08:18:36.000000 testfixtures-8.1.0/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2361 2024-03-01 08:18:45.723653 testfixtures-8.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1786 2024-03-01 08:18:36.000000 testfixtures-8.1.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2024-03-01 08:18:36.000000 testfixtures-8.1.0/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.715653 testfixtures-8.1.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2576 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/api.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/changes.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30602 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/comparing.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1755 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14859 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/datetime.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/development.txt
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2496 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/django.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4474 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/exceptions.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22197 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/files.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/index.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/installation.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/license.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13508 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/logging.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19569 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/mocking.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7542 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/popen.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2751 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/streams.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/twisted.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/utilities.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-03-01 08:18:36.000000 testfixtures-8.1.0/docs/warnings.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-03-01 08:18:36.000000 testfixtures-8.1.0/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-01 08:18:45.723653 testfixtures-8.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1354 2024-03-01 08:18:36.000000 testfixtures-8.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.715653 testfixtures-8.1.0/testfixtures/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1215 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40513 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/comparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/compat.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24993 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/datetime.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2914 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/django.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11018 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/logcapture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1234 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/mock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4793 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/outputcapture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10863 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/popen.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12696 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/replace.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2357 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/resolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/rmtree.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3656 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/shouldraise.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2655 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/shouldwarn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2388 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/sybil.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13244 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tempdirectory.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.723653 testfixtures-8.1.0/testfixtures/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      832 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/configparser-read.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      775 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/configparser-write.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/directory-contents.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/sample1.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/sample2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/sample3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    63673 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_compare.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22618 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_comparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11094 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_date.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17442 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_datetime.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_diff.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.723653 testfixtures-8.1.0/testfixtures/tests/test_django/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_django/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_django/manage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_django/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_django/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_django/test_compare.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_django/test_shouldraise.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_generator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7379 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_log_capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19659 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_logcapture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9643 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_mappingcomparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2245 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_mock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4347 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_outputcapture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25173 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_popen.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7676 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_popen_docs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5330 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_rangecomparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33396 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_replace.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3906 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_replacer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4828 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_roundcomparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_sequencecomparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9560 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_should_raise.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6202 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_shouldwarn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1362 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_stringcomparison.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4302 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_sybil.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_tempdir.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11081 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_tempdirectory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7734 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_time.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5673 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_twisted.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6576 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/tests/test_wrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4907 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/twisted.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2803 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-03-01 08:18:36.000000 testfixtures-8.1.0/testfixtures/version.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 08:18:45.719653 testfixtures-8.1.0/testfixtures.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2361 2024-03-01 08:18:45.000000 testfixtures-8.1.0/testfixtures.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2705 2024-03-01 08:18:45.000000 testfixtures-8.1.0/testfixtures.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-01 08:18:45.000000 testfixtures-8.1.0/testfixtures.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-01 08:18:41.000000 testfixtures-8.1.0/testfixtures.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-03-01 08:18:45.000000 testfixtures-8.1.0/testfixtures.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-03-01 08:18:45.000000 testfixtures-8.1.0/testfixtures.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.850106 testfixtures-8.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-05-01 07:55:02.000000 testfixtures-8.2.0/.carthorse.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.834106 testfixtures-8.2.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2024-05-01 07:55:02.000000 testfixtures-8.2.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2024-05-01 07:55:02.000000 testfixtures-8.2.0/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-05-01 07:55:02.000000 testfixtures-8.2.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-05-01 07:55:02.000000 testfixtures-8.2.0/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40921 2024-05-01 07:55:02.000000 testfixtures-8.2.0/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2024-05-01 07:55:02.000000 testfixtures-8.2.0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2973 2024-05-01 07:55:08.850106 testfixtures-8.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1786 2024-05-01 07:55:02.000000 testfixtures-8.2.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2024-05-01 07:55:02.000000 testfixtures-8.2.0/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.838106 testfixtures-8.2.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2576 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/api.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/changes.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30602 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/comparing.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1755 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14859 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/datetime.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/development.txt
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2496 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/django.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4474 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/exceptions.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22197 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/files.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/index.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/installation.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/license.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13508 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/logging.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19569 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/mocking.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7542 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/popen.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2751 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/streams.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/twisted.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/utilities.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-05-01 07:55:02.000000 testfixtures-8.2.0/docs/warnings.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-05-01 07:55:02.000000 testfixtures-8.2.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-01 07:55:08.850106 testfixtures-8.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1354 2024-05-01 07:55:02.000000 testfixtures-8.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.842106 testfixtures-8.2.0/testfixtures/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1215 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40737 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/comparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/compat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24993 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/datetime.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2914 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/django.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11018 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/logcapture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1234 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/mock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4793 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/outputcapture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10863 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/popen.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13456 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/replace.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2357 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/resolve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/rmtree.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3656 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/shouldraise.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2655 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/shouldwarn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2388 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/sybil.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13244 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tempdirectory.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.846106 testfixtures-8.2.0/testfixtures/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      832 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/configparser-read.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      775 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/configparser-write.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/directory-contents.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/sample1.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/sample2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/sample3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64533 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_compare.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22618 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_comparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11094 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17442 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_datetime.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.846106 testfixtures-8.2.0/testfixtures/tests/test_django/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_django/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_django/manage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_django/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_django/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_django/test_compare.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_django/test_shouldraise.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_generator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7379 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_log_capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19659 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_logcapture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9643 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_mappingcomparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2245 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_mock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4347 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_outputcapture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25173 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_popen.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7676 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_popen_docs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5330 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_rangecomparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    44244 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_replace.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3906 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_replacer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4828 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_roundcomparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_sequencecomparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9560 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_should_raise.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6202 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_shouldwarn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1362 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_stringcomparison.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4302 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_sybil.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_tempdir.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11081 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_tempdirectory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7734 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_time.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5673 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_twisted.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6576 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/tests/test_wrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4907 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/twisted.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2803 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-01 07:55:02.000000 testfixtures-8.2.0/testfixtures/version.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 07:55:08.846106 testfixtures-8.2.0/testfixtures.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2973 2024-05-01 07:55:08.000000 testfixtures-8.2.0/testfixtures.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2705 2024-05-01 07:55:08.000000 testfixtures-8.2.0/testfixtures.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-01 07:55:08.000000 testfixtures-8.2.0/testfixtures.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-01 07:55:06.000000 testfixtures-8.2.0/testfixtures.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-05-01 07:55:08.000000 testfixtures-8.2.0/testfixtures.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-01 07:55:08.000000 testfixtures-8.2.0/testfixtures.egg-info/top_level.txt
```

### Comparing `testfixtures-8.1.0/.circleci/config.yml` & `testfixtures-8.2.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/CHANGELOG.rst` & `testfixtures-8.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changes
 =======
 
+8.2.0 (1 May 2024)
+------------------
+
+- The ``strict`` option is now correctly respected when :doc:`comparing <comparing>` nested objects.
+
+- When comparing :class:`~datetime.datetime` or :class:`~datetime.time` instances, if the fold
+  is the only thing that's different, it's now shown in the output.
+
+- A more detailed exception is now raised when resolving a :doc:`replacement <mocking>` doesn't give
+  what's expected.
+
+- :doc:`Replacement <mocking>` of methods on instances is now prevented when ``strict=True``.
+
+- An exception is now raised when :doc:`mocking <mocking>` and the original is not in the
+  ``__dict__`` of its containing objects.
+
 8.1.0 (1 Mar 2024)
 ------------------
 
 - Fix bug where replacement of methods on subclasses failed when using :meth:`Replacer.on_class`.
 
 - Implement :ref:`strict comparison <compare-datetime>` as an option for :class:`~datetime.datetime`
   and :class:`~datetime.time`.
```

### Comparing `testfixtures-8.1.0/LICENSE.txt` & `testfixtures-8.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/PKG-INFO` & `testfixtures-8.2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: testfixtures
-Version: 8.1.0
-Summary: A collection of helpers and mock objects for unit tests and doc tests.
-Home-page: https://github.com/Simplistix/testfixtures
-Author: Chris Withers
-Author-email: chris@simplistix.co.uk
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: build
-License-File: LICENSE.txt
-
 Testfixtures
 ============
 
 |CircleCI|_ |Docs|_
 
 .. |CircleCI| image:: https://circleci.com/gh/simplistix/testfixtures/tree/master.svg?style=shield
 .. _CircleCI: https://circleci.com/gh/simplistix/testfixtures/tree/master
```

### Comparing `testfixtures-8.1.0/conftest.py` & `testfixtures-8.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/Makefile` & `testfixtures-8.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/api.txt` & `testfixtures-8.2.0/docs/api.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/comparing.txt` & `testfixtures-8.2.0/docs/comparing.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/conf.py` & `testfixtures-8.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/datetime.txt` & `testfixtures-8.2.0/docs/datetime.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/development.txt` & `testfixtures-8.2.0/docs/development.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/django.txt` & `testfixtures-8.2.0/docs/django.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/exceptions.txt` & `testfixtures-8.2.0/docs/exceptions.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/files.txt` & `testfixtures-8.2.0/docs/files.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/index.txt` & `testfixtures-8.2.0/docs/index.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/installation.txt` & `testfixtures-8.2.0/docs/installation.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/logging.txt` & `testfixtures-8.2.0/docs/logging.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/make.bat` & `testfixtures-8.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/mocking.txt` & `testfixtures-8.2.0/docs/mocking.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/popen.txt` & `testfixtures-8.2.0/docs/popen.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/streams.txt` & `testfixtures-8.2.0/docs/streams.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/utilities.txt` & `testfixtures-8.2.0/docs/utilities.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/docs/warnings.txt` & `testfixtures-8.2.0/docs/warnings.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/setup.py` & `testfixtures-8.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/__init__.py` & `testfixtures-8.2.0/testfixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/comparison.py` & `testfixtures-8.2.0/testfixtures/comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
     if type(x) is not type(y) or isinstance(x, type):
         return compare_simple(x, y, context)
     x_attrs = _extract_attrs(x, _attrs_to_ignore(context, ignore_attributes, x))
     y_attrs = _extract_attrs(y, _attrs_to_ignore(context, ignore_attributes, y))
     if x_attrs is None or y_attrs is None or not (x_attrs and y_attrs):
         return compare_simple(x, y, context)
-    if context.ignore_eq or x_attrs != y_attrs:
+    if context.strict or context.ignore_eq or x_attrs != y_attrs:
         return _compare_mapping(x_attrs, y_attrs, context, x,
                                 'attributes ', '.%s')
 
 
 def compare_exception(
         x: Exception, y: Exception, context: 'CompareContext'
 ) -> Optional[str]:
@@ -449,15 +449,20 @@
 
 def compare_path(x: Path, y: Path, context: 'CompareContext') -> Optional[str]:
     return compare_text(str(x), str(y), context)
 
 
 def compare_with_fold(x: datetime, y: datetime, context: 'CompareContext') -> Optional[str]:
     if not (x == y and x.fold == y.fold):
-        return f'{x!r} != {y!r}'
+        repr_x = repr(x)
+        repr_y = repr(y)
+        if repr_x == repr_y:
+            repr_x += f' (fold={x.fold})'
+            repr_y += f' (fold={y.fold})'
+        return context.label('x', repr_x)+' != '+context.label('y', repr_y)
 
 
 def _short_repr(obj) -> str:
     repr_ = repr(obj)
     if len(repr_) > 30:
         repr_ = repr_[:30] + '...'
     return repr_
```

### Comparing `testfixtures-8.1.0/testfixtures/datetime.py` & `testfixtures-8.2.0/testfixtures/datetime.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/django.py` & `testfixtures-8.2.0/testfixtures/django.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/logcapture.py` & `testfixtures-8.2.0/testfixtures/logcapture.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/mock.py` & `testfixtures-8.2.0/testfixtures/mock.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/outputcapture.py` & `testfixtures-8.2.0/testfixtures/outputcapture.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/popen.py` & `testfixtures-8.2.0/testfixtures/popen.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/replace.py` & `testfixtures-8.2.0/testfixtures/replace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from contextlib import contextmanager
 from functools import partial
 from gc import get_referrers, get_referents
 from operator import setitem, getitem
-from types import ModuleType
+from types import ModuleType, MethodType
 from typing import Any, TypeVar, Callable, Dict, Tuple
 
 from testfixtures.resolve import resolve, not_there, Resolved, classmethod_type, class_type, Setter
 from testfixtures.utils import wrap, extend_docstring
 
 import warnings
 
@@ -62,54 +62,74 @@
         """
         if name is None and accessor is not None:
             raise TypeError('accessor is not used unless name is specified')
 
         if isinstance(target, str) and not name:
             resolved = resolve(target, container, sep)
         else:
-            found = not_there
             if container is None:
                 container = target
 
             name = name or getattr(target, '__name__', None)
             if name is None:
                 raise TypeError('name must be specified when target is not a string')
             else:
                 if accessor is None:
                     try:
                         accessor = getitem
                         found = accessor(container, name)
                     except KeyError:
-                        pass
+                        found = not_there
                     except TypeError:
                         accessor = getattr
                         found = accessor(container, name, not_there)
                 else:
                     try:
                         found = accessor(container, name)
                     except (KeyError, AttributeError):
-                        pass
+                        found = not_there
 
             if strict and not (found is not_there or target is container):
-                expected = accessor(container, name)
-                if target is not expected:
-                    raise AssertionError(f'{name!r} resolved to {found}, expected {target}')
+                if found is not target:
+                    if isinstance(found, MethodType):
+                        raise TypeError(
+                            'Cannot replace methods on instances with strict=True, '
+                            'replace on class or use strict=False'
+                        )
+                    raise AssertionError(
+                        f'{accessor} of {name!r} from {container!r} gave {found!r}, '
+                        f'expected {target}'
+                    )
 
             resolved = Resolved(
                 container,
                 setitem if accessor is getitem else setattr,
                 name,
                 found
             )
 
         if resolved.setter is None:
             raise ValueError('target must contain at least one dot!')
+
         if resolved.found is not_there and strict:
             raise AttributeError('Original %r not found' % resolved.name)
 
+        if (
+                hasattr(resolved.container, '__dict__') and
+                resolved.setter is setattr and
+                resolved.name not in resolved.container.__dict__
+        ):
+            if strict:
+                raise AttributeError(
+                    f'{resolved.container!r} has __dict__ but {resolved.name!r} is not in it'
+                )
+            else:
+                resolved.found = not_there
+
+
         replacement_to_use = replacement
 
         if isinstance(resolved.container, type):
 
             # if we have a descriptor, don't accidentally use the result of its __get__ method:
             if resolved.name in resolved.container.__dict__:
                 resolved.found = resolved.container.__dict__[resolved.name]
@@ -197,16 +217,16 @@
         self(container, name=name, accessor=getattr, replacement=replacement)
 
     def restore(self) -> None:
         """
         Restore all the original objects that have been replaced by
         calls to the :meth:`replace` method of this :class:`Replacer`.
         """
-        for id_, (target, original) in tuple(self.originals.items()):
-            self._replace(original, original.found)
+        for id_, (target, resolved) in tuple(self.originals.items()):
+            self._replace(resolved, resolved.found)
             del self.originals[id_]
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.restore()
```

### Comparing `testfixtures-8.1.0/testfixtures/resolve.py` & `testfixtures-8.2.0/testfixtures/resolve.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/rmtree.py` & `testfixtures-8.2.0/testfixtures/rmtree.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/shouldraise.py` & `testfixtures-8.2.0/testfixtures/shouldraise.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/shouldwarn.py` & `testfixtures-8.2.0/testfixtures/shouldwarn.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/sybil.py` & `testfixtures-8.2.0/testfixtures/sybil.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tempdirectory.py` & `testfixtures-8.2.0/testfixtures/tempdirectory.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/configparser-read.txt` & `testfixtures-8.2.0/testfixtures/tests/configparser-read.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/configparser-write.txt` & `testfixtures-8.2.0/testfixtures/tests/configparser-write.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/directory-contents.txt` & `testfixtures-8.2.0/testfixtures/tests/directory-contents.txt`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/sample1.py` & `testfixtures-8.2.0/testfixtures/tests/sample1.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_compare.py` & `testfixtures-8.2.0/testfixtures/tests/test_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -2129,14 +2129,23 @@
     def test_ignore_list_context_list_param(self):
         def compare_thing(x, y, context):
             return compare_object(x, y, context, ignore_attributes=['y'])
         compare(self.Thing(x=1, y=2, z=3), self.Thing(x=1, y=4, z=5),
                 comparers={self.Thing: compare_thing},
                 ignore_attributes=['z'])
 
+    def test_strict_respected_when_nested(self):
+        with ShouldAssert(
+            "Thing not as expected:\n\n"
+            "attributes differ:\n"
+            "'x': datetime.time(0, 0) != datetime.time(0, 0, fold=1)\n\n"
+            "While comparing .x: datetime.time(0, 0) != datetime.time(0, 0, fold=1)",
+        ):
+            compare(self.Thing(x=time()), self.Thing(x=time(fold=1)), strict=True)
+
 
 class BaseClass(ABC):
     pass
 
 
 class MyDerivedClass(BaseClass):
 
@@ -2217,7 +2226,19 @@
             compare(datetime(2000, 1, 1, fold=1), datetime(2000, 1, 1, fold=0), strict=True)
 
     def test_time_with_different_fold_strict(self):
         with ShouldAssert(
                 'datetime.time(0, 0, fold=1) != datetime.time(0, 0)'
         ):
             compare(time(fold=1), time(fold=0), strict=True)
+
+    def test_datetime_with_different_fold_strict_but_identical_repr(self):
+        class PandasDatetime(datetime):
+            def __repr__(self):
+                return f'<DT{self.year}-{self.day}-{self.month}>'
+
+        with ShouldAssert(
+                '<DT2000-1-1> (fold=1) != <DT2000-1-1> (fold=0)'
+        ):
+            compare(
+                PandasDatetime(2000, 1, 1, fold=1), PandasDatetime(2000, 1, 1, fold=0), strict=True
+            )
```

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_comparison.py` & `testfixtures-8.2.0/testfixtures/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_date.py` & `testfixtures-8.2.0/testfixtures/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_datetime.py` & `testfixtures-8.2.0/testfixtures/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_diff.py` & `testfixtures-8.2.0/testfixtures/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_django/test_compare.py` & `testfixtures-8.2.0/testfixtures/tests/test_django/test_compare.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_django/test_shouldraise.py` & `testfixtures-8.2.0/testfixtures/tests/test_django/test_shouldraise.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_log_capture.py` & `testfixtures-8.2.0/testfixtures/tests/test_log_capture.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_logcapture.py` & `testfixtures-8.2.0/testfixtures/tests/test_logcapture.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_mappingcomparison.py` & `testfixtures-8.2.0/testfixtures/tests/test_mappingcomparison.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_mock.py` & `testfixtures-8.2.0/testfixtures/tests/test_mock.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_outputcapture.py` & `testfixtures-8.2.0/testfixtures/tests/test_outputcapture.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_popen.py` & `testfixtures-8.2.0/testfixtures/tests/test_popen.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_popen_docs.py` & `testfixtures-8.2.0/testfixtures/tests/test_popen_docs.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_rangecomparison.py` & `testfixtures-8.2.0/testfixtures/tests/test_rangecomparison.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_replace.py` & `testfixtures-8.2.0/testfixtures/tests/test_replace.py`

 * *Files 17% similar despite different names*

```diff
@@ -263,22 +263,17 @@
         def test_something(obj):
             sample1.foo = 'bar'
 
         test_something()
         self.assertFalse(hasattr(sample1, 'foo'))
 
     def test_replace_delattr_cant_remove(self):
-        if PY_310_PLUS:
-            message = "cannot set 'today' attribute of " \
-                      "immutable type 'datetime.datetime'"
-        else:
-            message = "can't set attributes of " \
-                      "built-in/extension type 'datetime.datetime'"
+        message = "<class 'datetime.datetime'> has __dict__ but 'today' is not in it"
         with Replacer() as r:
-            with ShouldRaise(TypeError(message)):
+            with ShouldRaise(AttributeError(message)):
                 r.replace('datetime.datetime.today', not_there)
 
     def test_replace_delattr_cant_remove_not_strict(self):
         if PY_310_PLUS:
             message = "cannot set 'today' attribute of " \
                       "immutable type 'datetime.datetime'"
         else:
@@ -568,18 +563,21 @@
             def a(self):
                 return 1
 
             def b(self):
                 return 2
 
         sample_obj = SampleClass()
+        s_repr = repr(SampleClass)
         a_repr = repr(SampleClass.a)
         b_repr = repr(SampleClass.b)
         replacer = Replacer()
-        with ShouldRaise(AssertionError(f"'b' resolved to {b_repr}, expected {a_repr}")):
+        with ShouldRaise(AssertionError(
+                f"<built-in function getattr> of 'b' from {s_repr} gave {b_repr}, expected {a_repr}"
+        )):
             replacer(SampleClass.a, lambda self: 3,
                      container=SampleClass, name='b', accessor=getattr)
 
         compare(sample_obj.a(), expected=1)
         compare(sample_obj.b(), expected=2)
 
     def test_traverse_from_container(self):
@@ -620,23 +618,14 @@
         environ = {}
 
         with Replace('.MY_ENV_VAR', 'True', container=environ, strict=False):
             compare(environ, expected={'MY_ENV_VAR': 'True'})
 
         compare(environ, expected={})
 
-    def test_obj_and_name(self):
-        my_obj = Mock()
-        foo = my_obj.foo
-
-        with Replace(my_obj, name='foo', replacement=42, strict=False):
-            compare(my_obj.foo, expected=42)
-
-        assert my_obj.foo is foo
-
     def test_non_string_target_and_no_name(self):
         my_dict = {}
 
         replacer = Replacer()
         with ShouldRaise(TypeError('name must be specified when target is not a string')):
             replacer(my_dict, replacement=42, strict=False)
 
@@ -789,14 +778,15 @@
             compare(sample.method_a(1), expected=4)
             compare(sample.method_b(1), expected=5)
 
         compare(sample.method_a(1), expected=2)
         compare(sample.method_b(1), expected=3)
         assert SampleClass.__dict__['method_a'] is original_a
         assert SampleSubClass.__dict__['method_b'] is original_b
+        assert 'method_a' not in SampleSubClass.__dict__
 
     def test_attributes_on_class(self):
 
         class SampleClass:
             x = 1
             y = 'a'
 
@@ -1054,7 +1044,365 @@
             from .sample3 import z as sample3_z
             compare(sample1_z(), expected='original z')
             compare(sample3_z(), expected='all new z')
         from .sample1 import z as sample1_z
         from .sample3 import z as sample3_z
         compare(sample1_z(), expected='original z')
         compare(sample3_z(), expected='original z')
+
+
+class OriginA:
+
+    bar = 13
+
+    def __init__(self):
+        self.foo = 43
+
+    def method(self, x):
+        return x * 2
+
+    original = method
+
+
+class UseB(OriginA):
+    pass
+
+
+class UseC(OriginA):
+    pass
+
+
+class OriginD:
+
+    def __init__(self, attrs):
+        self.attrs = attrs
+
+    def __getattr__(self, item):
+        return self.attrs[item]
+
+
+class OriginE:
+    __slots__ = 'attr',
+
+    def method(self, x):
+        return x * 2
+
+    original = method
+
+
+class UseF(OriginE):
+    __slots__ = 'attr',
+
+
+class UseG(OriginE):
+    __slots__ = 'attr',
+
+
+def check_originals_not_modified():
+    assert OriginA.__dict__['method'] is OriginA.original
+    assert OriginA.__dict__['bar'] == 13
+    assert 'method' not in UseB.__dict__
+    assert 'method' not in UseC.__dict__
+    assert OriginE.method is OriginE.original
+
+
+def check_behaviour_is_unchanged(*callables):
+    for c in callables:
+        compare(c(1), expected=2, prefix=repr(c))
+
+
+class TestReplaceWithInterestingOriginsStrict:
+
+    strict = True
+
+    def test_class_attribute_on_class(self):
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        with Replace(OriginA.bar, name='bar', replacement=31, strict=self.strict, container=OriginA):
+            compare(sample_a.bar, expected=31)
+            compare(sample_b.bar, expected=31)
+            compare(sample_c.bar, expected=31)
+
+        compare(sample_a.bar, expected=13)
+        compare(sample_b.bar, expected=13)
+        compare(sample_c.bar, expected=13)
+
+        check_originals_not_modified()
+
+    def test_class_attribute_on_subclass(self):
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError(f"{UseB!r} has __dict__ but 'bar' is not in it")):
+            replace_(UseB.bar, name='bar', replacement=31, strict=self.strict, container=UseB)
+
+        compare(sample_a.bar, expected=13)
+        compare(sample_b.bar, expected=13)
+        compare(sample_c.bar, expected=13)
+
+        check_originals_not_modified()
+
+    def test_method_on_subclass(self):
+
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError(f"{UseB!r} has __dict__ but 'method' is not in it")):
+            replace_(
+                UseB.method, lambda self_, x: x*4, name='method', container=UseB, strict=self.strict
+            )
+
+        check_behaviour_is_unchanged(sample_a.method, sample_b.method, sample_c.method)
+        check_originals_not_modified()
+
+    def test_class_attribute_on_instance_of_class(self):
+        obj = OriginA()
+        bar = obj.bar
+
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError(f"{obj!r} has __dict__ but 'bar' is not in it")):
+            replace_(obj, name='bar', replacement=31, strict=self.strict)
+            compare(obj.bar, expected=31)
+
+        assert obj.bar is bar
+
+    def test_instance_attribute_on_instance_of_class(self):
+        obj = OriginA()
+        foo = obj.foo
+
+        with Replace(obj, name='foo', replacement=42, strict=self.strict):
+            compare(obj.foo, expected=42)
+
+        assert obj.foo is foo
+
+    def test_method_on_instance_of_class(self):
+
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        replace = Replacer()
+        with ShouldRaise(TypeError(
+                "Cannot replace methods on instances with strict=True, "
+                "replace on class or use strict=False")
+        ):
+            replace(
+                sample_a.method, lambda self_, x: x*4, name='method', container=sample_a,
+                strict=self.strict
+            )
+
+        check_behaviour_is_unchanged(sample_a.method, sample_b.method, sample_c.method)
+        check_originals_not_modified()
+
+    def test_method_on_instance_of_subclass(self):
+        obj = UseB()
+        replace = Replacer()
+        with ShouldRaise(TypeError(
+                "Cannot replace methods on instances with strict=True, "
+                "replace on class or use strict=False")
+        ):
+            replace(
+                obj.method, lambda self_, x: x*4, name='method', container=obj, strict=self.strict
+            )
+        check_behaviour_is_unchanged(obj.method)
+        check_originals_not_modified()
+
+    def test_valid_attribute_on_instance_of_slotted_class(self):
+
+        obj = OriginE()
+        assert not hasattr(obj, '__dict__')
+        obj.attr = 41
+
+        with Replace(obj, name='attr', replacement=42, strict=self.strict):
+            compare(obj.attr, expected=42)
+
+        assert obj.attr == 41
+
+    def test_invalid_attribute_on_instance_of_slotted_class(self):
+        obj = OriginE()
+        assert not hasattr(obj, '__dict__')
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError("Original 'bad' not found")):
+            replace_(obj, name='bad', replacement=42, strict=self.strict)
+
+    def test_method_on_instance_of_slotted_subclass(self):
+
+        sample_e = OriginE()
+        sample_f = UseF()
+        sample_g = UseG()
+
+        obj = UseF()
+
+        assert not hasattr(obj, '__dict__')
+
+        replace_ = Replacer()
+        with ShouldRaise(TypeError(
+                "Cannot replace methods on instances with strict=True, "
+                "replace on class or use strict=False"
+        )):
+            replace_(
+                obj.method, lambda self_, x: x*4, name='method', container=obj, strict=self.strict
+            )
+
+        check_behaviour_is_unchanged(sample_e.method, sample_f.method, sample_g.method)
+        check_behaviour_is_unchanged()
+
+    def test_interesting_container(self):
+        replace_ = Replacer()
+        sample = OriginD({'foo': 'bar'})
+        with ShouldRaise(AttributeError(f"{sample!r} has __dict__ but 'foo' is not in it")):
+            replace_(sample.foo, 'baz', name='foo', container=sample, strict=self.strict)
+        compare(sample.foo, expected='bar')
+        assert 'foo' not in sample.__dict__
+
+    def test_mock_and_name(self):
+        my_obj = Mock()
+        foo = my_obj.foo
+
+        # Mock instances are tricky in that they have a __dict__ but
+        # their attributes are not in it:
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError(f"{my_obj!r} has __dict__ but 'foo' is not in it")):
+            replace_(my_obj, name='foo', replacement=42, strict=self.strict)
+
+        assert my_obj.foo is foo
+
+
+class TestReplaceWithInterestingOriginsNotStrict(TestReplaceWithInterestingOriginsStrict):
+    # This subclasses TestReplaceWithInterestingOriginsStrict to ensure we check all the same cases
+    strict = False
+
+    def test_class_attribute_on_subclass(self):
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        with Replace(UseB.bar, name='bar', replacement=31, strict=self.strict, container=UseB):
+            compare(sample_a.bar, expected=13)
+            compare(sample_b.bar, expected=31)
+            compare(sample_c.bar, expected=13)
+
+        compare(sample_a.bar, expected=13)
+        compare(sample_b.bar, expected=13)
+        compare(sample_c.bar, expected=13)
+
+        check_originals_not_modified()
+
+    def test_method_on_subclass(self):
+
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        with Replace(
+                UseB.method, lambda self_, x: x*4, name='method', container=UseB, strict=self.strict
+        ):
+            compare(sample_b.method(1), expected=4)
+            check_behaviour_is_unchanged(sample_a.method, sample_c.method)
+
+        check_behaviour_is_unchanged(sample_a.method, sample_b.method, sample_c.method)
+        check_originals_not_modified()
+
+    def test_class_attribute_on_instance_of_class(self):
+        obj = OriginA()
+        bar = obj.bar
+
+        with Replace(obj, name='bar', replacement=31, strict=self.strict):
+            compare(obj.bar, expected=31)
+
+        assert obj.bar is bar
+
+    def test_instance_attribute_on_instance_of_class(self):
+        obj = OriginA()
+        foo = obj.foo
+
+        with Replace(obj, name='foo', replacement=42, strict=self.strict):
+            compare(obj.foo, expected=42)
+
+        assert obj.foo is foo
+
+    def test_method_on_instance_of_class(self):
+
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        with Replace(
+                sample_a.method, lambda x: x*4, name='method', container=sample_a,
+                strict=self.strict
+        ):
+            compare(sample_a.method(1), expected=4)
+            check_behaviour_is_unchanged(sample_b.method, sample_c.method)
+
+        check_behaviour_is_unchanged(sample_a.method, sample_b.method, sample_c.method)
+        check_originals_not_modified()
+
+    def test_method_on_instance_of_subclass(self):
+
+        sample_a = OriginA()
+        sample_b = UseB()
+        sample_c = UseC()
+
+        with Replace(
+                sample_b.method, lambda x: x*4, name='method', container=sample_b,
+                strict=self.strict
+        ):
+            compare(sample_b.method(1), expected=4)
+            check_behaviour_is_unchanged(sample_a.method, sample_c.method)
+
+        check_behaviour_is_unchanged(sample_a.method, sample_b.method, sample_c.method)
+        check_originals_not_modified()
+
+    def test_invalid_attribute_on_instance_of_slotted_class(self):
+        obj = OriginE()
+        assert not hasattr(obj, '__dict__')
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError("'OriginE' object has no attribute 'bad'")):
+            replace_(obj, name='bad', replacement=42, strict=self.strict)
+
+    def test_method_on_instance_of_slotted_subclass(self):
+
+        sample_e = OriginE()
+        sample_f = UseF()
+        sample_g = UseG()
+
+        obj = UseF()
+
+        assert not hasattr(obj, '__dict__')
+
+        replace_ = Replacer()
+        with ShouldRaise(AttributeError("'UseF' object attribute 'method' is read-only")):
+            replace_(
+                obj.method, lambda self_, x: x*4, name='method', container=obj, strict=self.strict
+            )
+
+        check_behaviour_is_unchanged(sample_e.method, sample_f.method, sample_g.method)
+        check_behaviour_is_unchanged()
+
+    def test_interesting_container(self):
+        sample = OriginD({'foo': 'bar'})
+        with Replace(sample.foo, 'baz', name='foo', container=sample, strict=self.strict):
+            compare(sample.foo, expected='baz')
+        compare(sample.foo, expected='bar')
+        assert 'foo' not in sample.__dict__
+
+    def test_mock_and_name(self):
+        my_obj = Mock()
+        foo = my_obj.foo
+
+        assert hasattr(my_obj, 'foo')
+        assert getattr(my_obj, 'foo', None)
+
+        with Replace(my_obj, name='foo', replacement=42, strict=self.strict):
+            compare(my_obj.foo, expected=42)
+
+        with ShouldRaise(AttributeError('foo')):
+            # Mock instances are tricky in that they have a __dict__ but
+            # their attributes are not in it, confusing Replace, which deletes
+            # the attribute on restore as a result:
+            assert my_obj.foo is foo
```

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_replacer.py` & `testfixtures-8.2.0/testfixtures/tests/test_replacer.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_roundcomparison.py` & `testfixtures-8.2.0/testfixtures/tests/test_roundcomparison.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_sequencecomparison.py` & `testfixtures-8.2.0/testfixtures/tests/test_sequencecomparison.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_should_raise.py` & `testfixtures-8.2.0/testfixtures/tests/test_should_raise.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_shouldwarn.py` & `testfixtures-8.2.0/testfixtures/tests/test_shouldwarn.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_stringcomparison.py` & `testfixtures-8.2.0/testfixtures/tests/test_stringcomparison.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_sybil.py` & `testfixtures-8.2.0/testfixtures/tests/test_sybil.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_tempdir.py` & `testfixtures-8.2.0/testfixtures/tests/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_tempdirectory.py` & `testfixtures-8.2.0/testfixtures/tests/test_tempdirectory.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_time.py` & `testfixtures-8.2.0/testfixtures/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_twisted.py` & `testfixtures-8.2.0/testfixtures/tests/test_twisted.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/tests/test_wrap.py` & `testfixtures-8.2.0/testfixtures/tests/test_wrap.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/twisted.py` & `testfixtures-8.2.0/testfixtures/twisted.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures/utils.py` & `testfixtures-8.2.0/testfixtures/utils.py`

 * *Files identical despite different names*

### Comparing `testfixtures-8.1.0/testfixtures.egg-info/PKG-INFO` & `testfixtures-8.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 Metadata-Version: 2.1
 Name: testfixtures
-Version: 8.1.0
+Version: 8.2.0
 Summary: A collection of helpers and mock objects for unit tests and doc tests.
 Home-page: https://github.com/Simplistix/testfixtures
 Author: Chris Withers
 Author-email: chris@simplistix.co.uk
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+License-File: LICENSE.txt
 Provides-Extra: test
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: pytest>=7.1; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-django; extra == "test"
+Requires-Dist: django; extra == "test"
+Requires-Dist: sybil>=6; extra == "test"
+Requires-Dist: twisted; extra == "test"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: django; extra == "docs"
+Requires-Dist: sybil>=6; extra == "docs"
+Requires-Dist: twisted; extra == "docs"
 Provides-Extra: build
-License-File: LICENSE.txt
+Requires-Dist: setuptools-git; extra == "build"
+Requires-Dist: wheel; extra == "build"
+Requires-Dist: twine; extra == "build"
 
 Testfixtures
 ============
 
 |CircleCI|_ |Docs|_
 
 .. |CircleCI| image:: https://circleci.com/gh/simplistix/testfixtures/tree/master.svg?style=shield
```

### Comparing `testfixtures-8.1.0/testfixtures.egg-info/SOURCES.txt` & `testfixtures-8.2.0/testfixtures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

