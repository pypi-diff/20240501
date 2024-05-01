# Comparing `tmp/recharge-api-1.4.1.tar.gz` & `tmp/recharge_api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recharge-api-1.4.1.tar", last modified: Fri Jul 23 09:08:08 2021, max compression
+gzip compressed data, was "recharge_api-1.5.0.tar", last modified: Wed May  1 13:04:48 2024, max compression
```

## Comparing `recharge-api-1.4.1.tar` & `recharge_api-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-07-23 09:08:08.722215 recharge-api-1.4.1/
--rw-rw-rw-   0        0        0     1072 2021-07-07 15:01:43.000000 recharge-api-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     2487 2021-07-23 09:08:08.721216 recharge-api-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2021-07-07 15:02:58.000000 recharge-api-1.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-07-23 09:08:08.716216 recharge-api-1.4.1/recharge/
--rw-rw-rw-   0        0        0     1192 2021-07-23 09:07:24.000000 recharge-api-1.4.1/recharge/__init__.py
--rw-rw-rw-   0        0        0    15661 2021-07-23 08:59:26.000000 recharge-api-1.4.1/recharge/resources.py
-drwxrwxrwx   0        0        0        0 2021-07-23 09:08:08.720218 recharge-api-1.4.1/recharge_api.egg-info/
--rw-rw-rw-   0        0        0     2487 2021-07-23 09:08:08.000000 recharge-api-1.4.1/recharge_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2021-07-23 09:08:08.000000 recharge-api-1.4.1/recharge_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-23 09:08:08.000000 recharge-api-1.4.1/recharge_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-07-07 15:24:16.000000 recharge-api-1.4.1/recharge_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2021-07-23 09:08:08.000000 recharge-api-1.4.1/recharge_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-07-23 09:08:08.000000 recharge-api-1.4.1/recharge_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-23 09:08:08.722215 recharge-api-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1165 2021-07-23 09:07:44.000000 recharge-api-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.223780 recharge_api-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-01 13:04:44.000000 recharge_api-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-01 13:04:48.223780 recharge_api-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 13:04:44.000000 recharge_api-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 13:04:44.000000 recharge_api-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.219780 recharge_api-1.5.0/recharge/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.219780 recharge_api-1.5.0/recharge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.223780 recharge_api-1.5.0/recharge/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8728 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.223780 recharge_api-1.5.0/recharge_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-01 13:04:48.227780 recharge_api-1.5.0/setup.cfg
```

### Comparing `recharge-api-1.4.1/LICENSE` & `recharge_api-1.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2021 Joe Tebbett
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+Copyright (c) 2021 Joe Tebbett
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

