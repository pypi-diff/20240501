# Comparing `tmp/airbyte-source-kyriba-0.1.1.tar.gz` & `tmp/airbyte_source_kyriba-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-kyriba-0.1.1.tar", last modified: Thu Feb  1 18:02:08 2024, max compression
+gzip compressed data, was "airbyte_source_kyriba-0.1.3.tar", max compression
```

## Comparing `airbyte-source-kyriba-0.1.1.tar` & `airbyte_source_kyriba-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.096959 airbyte-source-kyriba-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     7437 2024-02-01 18:02:08.096959 airbyte-source-kyriba-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7984 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.092960 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7437 2024-02-01 18:02:08.000000 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1222 2024-02-01 18:02:08.000000 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 18:02:08.000000 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-02-01 18:02:08.000000 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 18:02:08.000000 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-02-01 18:02:08.000000 airbyte-source-kyriba-0.1.1/airbyte_source_kyriba.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.088959 airbyte-source-kyriba-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     2036 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      144 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      144 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     7378 2024-02-01 18:02:08.096959 airbyte-source-kyriba-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      916 2024-02-01 18:02:05.000000 airbyte-source-kyriba-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.088959 airbyte-source-kyriba-0.1.1/source_kyriba/
--rw-r--r--   0 root         (0) root         (0)      124 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/__init__.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.092960 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/
--rw-r--r--   0 root         (0) root         (0)     5529 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/accounts.json
--rw-r--r--   0 root         (0) root         (0)      867 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/bank_balances_eod.json
--rw-r--r--   0 root         (0) root         (0)      901 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/bank_balances_intraday.json
--rw-r--r--   0 root         (0) root         (0)     1431 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/cash_balances_eod.json
--rw-r--r--   0 root         (0) root         (0)     1469 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/cash_balances_intraday.json
--rw-r--r--   0 root         (0) root         (0)     1632 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/cash_flows.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.092960 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/shared/
--rw-r--r--   0 root         (0) root         (0)    26897 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/schemas/shared/_definitions.json
--rw-r--r--   0 root         (0) root         (0)    11774 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/source.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/source_kyriba/spec.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 18:02:08.092960 airbyte-source-kyriba-0.1.1/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_account_sub_stream.py
--rw-r--r--   0 root         (0) root         (0)     1944 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_bank_balances_stream.py
--rw-r--r--   0 root         (0) root         (0)     2247 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_cash_balances_stream.py
--rw-r--r--   0 root         (0) root         (0)     2956 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_cash_flows.py
--rw-r--r--   0 root         (0) root         (0)     2867 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     4001 2024-02-01 17:40:59.000000 airbyte-source-kyriba-0.1.1/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4496 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/README.md
+-rw-r--r--   0        0        0      743 2024-05-01 18:56:56.054655 airbyte_source_kyriba-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/run.py
+-rw-r--r--   0        0        0    10240 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/accounts.json
+-rw-r--r--   0        0        0     1524 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/bank_balances_eod.json
+-rw-r--r--   0        0        0     1516 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/bank_balances_intraday.json
+-rw-r--r--   0        0        0     2541 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/cash_balances_eod.json
+-rw-r--r--   0        0        0     2076 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/cash_balances_intraday.json
+-rw-r--r--   0        0        0     2589 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/cash_flows.json
+-rw-r--r--   0        0        0    26897 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/schemas/shared/_definitions.json
+-rw-r--r--   0        0        0    11774 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/source.py
+-rw-r--r--   0        0        0     1513 2024-05-01 18:53:12.802788 airbyte_source_kyriba-0.1.3/source_kyriba/spec.json
+-rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 airbyte_source_kyriba-0.1.3/PKG-INFO
```

### Comparing `airbyte-source-kyriba-0.1.1/source_kyriba/schemas/cash_balances_intraday.json` & `airbyte_source_kyriba-0.1.3/source_kyriba/schemas/cash_balances_intraday.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'properties'": "{'account': {'properties': {'code': {'description': 'The identifier code for the "*

 * *                 "account.'}, 'statementIdentifier': {'description': 'The identifier for the cash "*

 * *                 "flow statement.'}, 'uuid': {'description': 'The universally unique identifier "*

 * *                 "for the account.'}}, 'description': 'Details about the account associated with "*

 * *                 "the cash balance data.'}, 'cashFlowStatus': {'properties': {'actual': "*

 * *                 "{'desc […]*

```diff
@@ -1,25 +1,29 @@
 {
     "$schema": "http://json-schema.org/schema#",
     "properties": {
         "account": {
+            "description": "Details about the account associated with the cash balance data.",
             "properties": {
                 "code": {
+                    "description": "The identifier code for the account.",
                     "type": [
                         "string",
                         "null"
                     ]
                 },
                 "statementIdentifier": {
+                    "description": "The identifier for the cash flow statement.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "uuid": {
+                    "description": "The universally unique identifier for the account.",
                     "type": [
                         "string",
                         "null"
                     ]
                 }
             },
             "type": [
@@ -71,34 +75,39 @@
             },
             "type": [
                 "array",
                 "null"
             ]
         },
         "cashFlowStatus": {
+            "description": "The current status of cash flow.",
             "properties": {
                 "actual": {
+                    "description": "The actual cash flow status.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
                 "confirmedForecasts": {
+                    "description": "The confirmed cash flow forecasts.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
                 "estimatedForecasts": {
+                    "description": "The estimated cash flow forecasts.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
                 "intraday": {
+                    "description": "The intraday cash balance status.",
                     "type": [
                         "boolean",
                         "null"
                     ]
                 }
             },
             "type": [
```

### Comparing `airbyte-source-kyriba-0.1.1/source_kyriba/schemas/shared/_definitions.json` & `airbyte_source_kyriba-0.1.3/source_kyriba/schemas/shared/_definitions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-kyriba-0.1.1/source_kyriba/source.py` & `airbyte_source_kyriba-0.1.3/source_kyriba/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-kyriba-0.1.1/source_kyriba/spec.json` & `airbyte_source_kyriba-0.1.3/source_kyriba/spec.json`

 * *Files identical despite different names*

