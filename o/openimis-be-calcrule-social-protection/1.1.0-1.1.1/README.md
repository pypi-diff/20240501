# Comparing `tmp/openimis_be_calcrule_social_protection-1.1.0.tar.gz` & `tmp/openimis_be_calcrule_social_protection-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis_be_calcrule_social_protection-1.1.0.tar", last modified: Tue Apr 30 08:29:47 2024, max compression
+gzip compressed data, was "openimis_be_calcrule_social_protection-1.1.1.tar", last modified: Wed May  1 05:27:07 2024, max compression
```

## Comparing `openimis_be_calcrule_social_protection-1.1.0.tar` & `openimis_be_calcrule_social_protection-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_base_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_group_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_individual_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_strategy_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_strategy_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.755780 openimis_be_calcrule_social_protection-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-01 05:27:07.755780 openimis_be_calcrule_social_protection-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.751780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.751780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.751780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/beneficiary/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/beneficiary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/beneficiary/beneficiary_to_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.751780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/builder_to_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/builder_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/builder_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.751780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/group_beneficiary/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/group_beneficiary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/group_beneficiary/group_to_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/group_beneficiary/group_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/group_beneficiary/group_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.751780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.755780 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_base_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_group_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_individual_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_strategy_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_strategy_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 05:26:59.000000 openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:27:07.755780 openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-01 05:27:07.000000 openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-01 05:27:07.000000 openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:27:07.000000 openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 05:27:07.000000 openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 05:27:07.000000 openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:27:07.755780 openimis_be_calcrule_social_protection-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-01 05:27:07.000000 openimis_be_calcrule_social_protection-1.1.1/setup.py
```

### Comparing `openimis_be_calcrule_social_protection-1.1.0/LICENSE.md` & `openimis_be_calcrule_social_protection-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/PKG-INFO` & `openimis_be_calcrule_social_protection-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_social_protection
-Version: 1.1.0
+Version: 1.1.1
 Summary: The openIMIS Backend calcrule_social_protection reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/apps.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/apps.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/calculation_rule.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/config.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/config.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_benefit.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/builder_to_benefit.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/builder_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill_item.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/builder/builder_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_benefit.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/converters/group_beneficiary/group_to_benefit.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/signals.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/signals.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/__init__.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_base_strategy.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_base_strategy.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_group_strategy.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_group_strategy.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_individual_strategy.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_individual_strategy.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_strategy_storage.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/strategies/benefit_package_strategy_storage.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/utils.py` & `openimis_be_calcrule_social_protection-1.1.1/calcrule_social_protection/utils.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/PKG-INFO` & `openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_social_protection
-Version: 1.1.0
+Version: 1.1.1
 Summary: The openIMIS Backend calcrule_social_protection reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt` & `openimis_be_calcrule_social_protection-1.1.1/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis_be_calcrule_social_protection-1.1.0/setup.py` & `openimis_be_calcrule_social_protection-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_social_protection',
-    version='1.1.0',
+    version='v1.1.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calcrule_social_protection reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

