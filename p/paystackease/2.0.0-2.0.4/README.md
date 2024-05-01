# Comparing `tmp/paystackease-2.0.0.tar.gz` & `tmp/paystackease-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystackease-2.0.0.tar", max compression
+gzip compressed data, was "paystackease-2.0.4.tar", max compression
```

## Comparing `paystackease-2.0.0.tar` & `paystackease-2.0.4.tar`

### file list

```diff
@@ -1,65 +1,69 @@
--rwxr-xr-x   0        0        0     1090 2024-02-21 14:06:29.101210 paystackease-2.0.0/LICENSE
--rwxr-xr-x   0        0        0     4989 2024-04-19 08:56:04.255180 paystackease-2.0.0/README.md
--rwxr-xr-x   0        0        0     1407 2024-04-19 07:37:11.942415 paystackease-2.0.0/paystackease/__init__.py
--rwxr-xr-x   0        0        0     5768 2024-04-19 07:37:11.944394 paystackease-2.0.0/paystackease/apaystack.py
--rwxr-xr-x   0        0        0     1041 2024-04-19 07:37:11.946391 paystackease-2.0.0/paystackease/apis/__init__.py
--rwxr-xr-x   0        0        0        0 2024-04-19 07:37:11.946391 paystackease-2.0.0/paystackease/apis/async_apis/__init__.py
--rwxr-xr-x   0        0        0     2208 2024-04-19 07:37:11.947568 paystackease-2.0.0/paystackease/apis/async_apis/aapple_pay.py
--rwxr-xr-x   0        0        0     4498 2024-04-19 07:37:11.949191 paystackease-2.0.0/paystackease/apis/async_apis/abulk_charges.py
--rwxr-xr-x   0        0        0     6009 2024-04-19 07:37:11.949414 paystackease-2.0.0/paystackease/apis/async_apis/acharges.py
--rwxr-xr-x   0        0        0     6947 2024-04-19 07:37:11.951390 paystackease-2.0.0/paystackease/apis/async_apis/acustomers.py
--rwxr-xr-x   0        0        0     9518 2024-04-19 07:37:11.952391 paystackease-2.0.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py
--rwxr-xr-x   0        0        0     8198 2024-04-19 07:37:11.953392 paystackease-2.0.0/paystackease/apis/async_apis/adisputes.py
--rwxr-xr-x   0        0        0     1185 2024-04-19 07:37:11.954391 paystackease-2.0.0/paystackease/apis/async_apis/aintegration.py
--rwxr-xr-x   0        0        0     4426 2024-04-19 07:37:11.955392 paystackease-2.0.0/paystackease/apis/async_apis/amiscellaneous.py
--rwxr-xr-x   0        0        0     5801 2024-04-19 07:37:11.956393 paystackease-2.0.0/paystackease/apis/async_apis/apayment_pages.py
--rwxr-xr-x   0        0        0    10076 2024-04-19 07:37:11.957476 paystackease-2.0.0/paystackease/apis/async_apis/apayment_requests.py
--rwxr-xr-x   0        0        0     4690 2024-04-19 07:37:11.958390 paystackease-2.0.0/paystackease/apis/async_apis/aplans.py
--rwxr-xr-x   0        0        0     4381 2024-04-19 07:37:11.959391 paystackease-2.0.0/paystackease/apis/async_apis/aproducts.py
--rwxr-xr-x   0        0        0     3332 2024-04-19 07:37:11.960391 paystackease-2.0.0/paystackease/apis/async_apis/arefund.py
--rwxr-xr-x   0        0        0     3340 2024-04-19 07:37:11.961390 paystackease-2.0.0/paystackease/apis/async_apis/asettlements.py
--rwxr-xr-x   0        0        0     6387 2024-04-19 07:37:11.962392 paystackease-2.0.0/paystackease/apis/async_apis/asubaccounts.py
--rwxr-xr-x   0        0        0     4528 2024-04-19 07:37:11.963391 paystackease-2.0.0/paystackease/apis/async_apis/asubscriptions.py
--rwxr-xr-x   0        0        0     5537 2024-04-19 07:37:11.964391 paystackease-2.0.0/paystackease/apis/async_apis/aterminal.py
--rwxr-xr-x   0        0        0     6009 2024-04-19 07:37:11.965390 paystackease-2.0.0/paystackease/apis/async_apis/atransaction_splits.py
--rwxr-xr-x   0        0        0    12878 2024-04-19 07:37:11.966390 paystackease-2.0.0/paystackease/apis/async_apis/atransactions.py
--rwxr-xr-x   0        0        0     5418 2024-04-19 07:37:11.967390 paystackease-2.0.0/paystackease/apis/async_apis/atransfer_recipients.py
--rwxr-xr-x   0        0        0     4957 2024-04-19 07:37:11.968390 paystackease-2.0.0/paystackease/apis/async_apis/atransfers.py
--rwxr-xr-x   0        0        0     2795 2024-04-19 07:37:11.969390 paystackease-2.0.0/paystackease/apis/async_apis/atransfers_control.py
--rwxr-xr-x   0        0        0     2878 2024-04-19 07:37:11.970390 paystackease-2.0.0/paystackease/apis/async_apis/averification.py
--rwxr-xr-x   0        0        0        0 2024-04-19 07:37:11.971391 paystackease-2.0.0/paystackease/apis/sync_apis/__init__.py
--rwxr-xr-x   0        0        0     2154 2024-04-19 07:37:11.972390 paystackease-2.0.0/paystackease/apis/sync_apis/apple_pay.py
--rwxr-xr-x   0        0        0     4405 2024-04-19 07:37:11.973390 paystackease-2.0.0/paystackease/apis/sync_apis/bulk_charges.py
--rwxr-xr-x   0        0        0     5913 2024-04-19 07:37:11.975391 paystackease-2.0.0/paystackease/apis/sync_apis/charges.py
--rwxr-xr-x   0        0        0     6848 2024-04-19 07:37:11.976390 paystackease-2.0.0/paystackease/apis/sync_apis/customers.py
--rwxr-xr-x   0        0        0     9390 2024-04-19 07:37:11.977390 paystackease-2.0.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
--rwxr-xr-x   0        0        0     8082 2024-04-19 07:37:11.978395 paystackease-2.0.0/paystackease/apis/sync_apis/disputes.py
--rwxr-xr-x   0        0        0     1149 2024-04-19 07:37:11.979583 paystackease-2.0.0/paystackease/apis/sync_apis/integration.py
--rwxr-xr-x   0        0        0     4381 2024-04-19 07:37:11.980986 paystackease-2.0.0/paystackease/apis/sync_apis/miscellaneous.py
--rwxr-xr-x   0        0        0     5717 2024-04-19 07:37:11.982162 paystackease-2.0.0/paystackease/apis/sync_apis/payment_pages.py
--rwxr-xr-x   0        0        0     9948 2024-04-19 07:37:11.983416 paystackease-2.0.0/paystackease/apis/sync_apis/payment_requests.py
--rwxr-xr-x   0        0        0     4622 2024-04-19 07:37:11.984565 paystackease-2.0.0/paystackease/apis/sync_apis/plans.py
--rwxr-xr-x   0        0        0     4313 2024-04-19 07:37:11.985391 paystackease-2.0.0/paystackease/apis/sync_apis/products.py
--rwxr-xr-x   0        0        0     3276 2024-04-19 07:37:11.986391 paystackease-2.0.0/paystackease/apis/sync_apis/refund.py
--rwxr-xr-x   0        0        0     3304 2024-04-19 07:37:11.987391 paystackease-2.0.0/paystackease/apis/sync_apis/settlements.py
--rwxr-xr-x   0        0        0     6313 2024-04-19 07:37:11.988571 paystackease-2.0.0/paystackease/apis/sync_apis/subaccounts.py
--rwxr-xr-x   0        0        0     4437 2024-04-19 07:37:11.989391 paystackease-2.0.0/paystackease/apis/sync_apis/subscriptions.py
--rwxr-xr-x   0        0        0     5424 2024-04-19 07:37:11.990390 paystackease-2.0.0/paystackease/apis/sync_apis/terminal.py
--rwxr-xr-x   0        0        0     5913 2024-04-19 07:37:11.992392 paystackease-2.0.0/paystackease/apis/sync_apis/transaction_splits.py
--rwxr-xr-x   0        0        0    12740 2024-04-19 07:37:11.993390 paystackease-2.0.0/paystackease/apis/sync_apis/transactions.py
--rwxr-xr-x   0        0        0     5326 2024-04-19 07:37:11.995392 paystackease-2.0.0/paystackease/apis/sync_apis/transfer_recipients.py
--rwxr-xr-x   0        0        0     4865 2024-04-19 07:37:11.996436 paystackease-2.0.0/paystackease/apis/sync_apis/transfers.py
--rwxr-xr-x   0        0        0     2703 2024-04-19 07:37:11.997390 paystackease-2.0.0/paystackease/apis/sync_apis/transfers_control.py
--rwxr-xr-x   0        0        0     2822 2024-04-19 07:37:11.998390 paystackease-2.0.0/paystackease/apis/sync_apis/verification.py
--rwxr-xr-x   0        0        0      490 2024-04-19 07:37:11.999391 paystackease-2.0.0/paystackease/core/__init__.py
--rwxr-xr-x   0        0        0     3921 2024-04-19 07:37:12.001391 paystackease-2.0.0/paystackease/core/_api_base.py
--rwxr-xr-x   0        0        0     5859 2024-04-19 07:37:12.002463 paystackease-2.0.0/paystackease/core/_api_base_client.py
--rwxr-xr-x   0        0        0     4845 2024-04-19 07:37:12.003393 paystackease-2.0.0/paystackease/core/_api_client_requests.py
--rwxr-xr-x   0        0        0      683 2024-04-19 07:37:12.004392 paystackease-2.0.0/paystackease/core/_api_client_response.py
--rwxr-xr-x   0        0        0     1009 2024-04-19 07:37:12.006389 paystackease-2.0.0/paystackease/core/_api_errors.py
--rwxr-xr-x   0        0        0      582 2024-04-05 08:20:03.238175 paystackease-2.0.0/paystackease/helpers/__init__.py
--rwxr-xr-x   0        0        0      768 2024-04-03 01:47:46.289946 paystackease-2.0.0/paystackease/helpers/convert.py
--rwxr-xr-x   0        0        0     3756 2024-04-04 20:07:23.519543 paystackease-2.0.0/paystackease/helpers/tool_kit.py
--rwxr-xr-x   0        0        0     3064 2024-04-19 07:37:12.008473 paystackease-2.0.0/paystackease/paystack.py
--rwxr-xr-x   0        0        0     2035 2024-04-19 08:11:17.248078 paystackease-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-01 16:47:07.083210 paystackease-2.0.4/LICENSE
+-rw-r--r--   0        0        0     4802 2024-05-01 16:47:07.083210 paystackease-2.0.4/README.md
+-rw-r--r--   0        0        0     1335 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/__init__.py
+-rw-r--r--   0        0        0     5713 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apaystack.py
+-rw-r--r--   0        0        0      988 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/aapple_pay.py
+-rw-r--r--   0        0        0     4355 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/abulk_charges.py
+-rw-r--r--   0        0        0     5820 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/acharges.py
+-rw-r--r--   0        0        0     6762 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/acustomers.py
+-rw-r--r--   0        0        0     9269 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/adedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7980 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/adisputes.py
+-rw-r--r--   0        0        0     1146 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/aintegration.py
+-rw-r--r--   0        0        0     4327 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/amiscellaneous.py
+-rw-r--r--   0        0        0     5644 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/apayment_pages.py
+-rw-r--r--   0        0        0     9834 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/apayment_requests.py
+-rw-r--r--   0        0        0     4547 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/aplans.py
+-rw-r--r--   0        0        0     4253 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/aproducts.py
+-rw-r--r--   0        0        0     3233 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/arefund.py
+-rw-r--r--   0        0        0     3250 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/asettlements.py
+-rw-r--r--   0        0        0     6232 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/asubaccounts.py
+-rw-r--r--   0        0        0     4396 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/asubscriptions.py
+-rw-r--r--   0        0        0     5399 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/aterminal.py
+-rw-r--r--   0        0        0     5844 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/atransaction_splits.py
+-rw-r--r--   0        0        0    12559 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/atransactions.py
+-rw-r--r--   0        0        0     5281 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/atransfer_recipients.py
+-rw-r--r--   0        0        0     4822 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/atransfers.py
+-rw-r--r--   0        0        0     2717 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/atransfers_control.py
+-rw-r--r--   0        0        0     2802 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/async_apis/averification.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/__init__.py
+-rw-r--r--   0        0        0     2084 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/apple_pay.py
+-rw-r--r--   0        0        0     4263 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/bulk_charges.py
+-rw-r--r--   0        0        0     5724 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/charges.py
+-rw-r--r--   0        0        0     6663 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/customers.py
+-rw-r--r--   0        0        0     9141 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7864 2024-05-01 16:47:07.087210 paystackease-2.0.4/paystackease/apis/sync_apis/disputes.py
+-rw-r--r--   0        0        0     1110 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/integration.py
+-rw-r--r--   0        0        0     4283 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/miscellaneous.py
+-rw-r--r--   0        0        0     5560 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/payment_pages.py
+-rw-r--r--   0        0        0     9706 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/payment_requests.py
+-rw-r--r--   0        0        0     4479 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/plans.py
+-rw-r--r--   0        0        0     4185 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/products.py
+-rw-r--r--   0        0        0     3177 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/refund.py
+-rw-r--r--   0        0        0     3214 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/settlements.py
+-rw-r--r--   0        0        0     6158 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/subaccounts.py
+-rw-r--r--   0        0        0     4305 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/subscriptions.py
+-rw-r--r--   0        0        0     5285 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/terminal.py
+-rw-r--r--   0        0        0     5747 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/transaction_splits.py
+-rw-r--r--   0        0        0    12421 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/transactions.py
+-rw-r--r--   0        0        0     5189 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/transfer_recipients.py
+-rw-r--r--   0        0        0     4730 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/transfers.py
+-rw-r--r--   0        0        0     2625 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/transfers_control.py
+-rw-r--r--   0        0        0     2746 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/apis/sync_apis/verification.py
+-rw-r--r--   0        0        0      479 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/core/__init__.py
+-rw-r--r--   0        0        0     3805 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/core/_api_base.py
+-rw-r--r--   0        0        0     5696 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/core/_api_base_client.py
+-rw-r--r--   0        0        0     4680 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/core/_api_client_requests.py
+-rw-r--r--   0        0        0      660 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/core/_api_client_response.py
+-rw-r--r--   0        0        0      983 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/core/_api_errors.py
+-rw-r--r--   0        0        0      552 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/helpers/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/helpers/convert.py
+-rw-r--r--   0        0        0     3566 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/helpers/tool_kit.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/metadata/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/metadata/__version__.py
+-rw-r--r--   0        0        0     3074 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/paystack.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/utils/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-01 16:47:07.091210 paystackease-2.0.4/paystackease/utils/_compact.py
+-rw-r--r--   0        0        0     2259 2024-05-01 16:47:08.323217 paystackease-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.0.4/PKG-INFO
```

### Comparing `paystackease-2.0.0/LICENSE` & `paystackease-2.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 PETER MBACHU
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 PETER MBACHU
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `paystackease-2.0.0/README.md` & `paystackease-2.0.4/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-# PayStackEase Library  
-
---------------
-
-![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease.svg) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
-
-
-**PayStackEase API Library**  is a Python library that simplifies interacting with the Paystack API. 
-It provides both asynchronous and synchronous wrappers for various Paystack functionalities, 
-making it easier to integrate payment processing into your Python projects.
-
-> 📝: Read more on paystack api documentation: [Paystack API DOCUMENTATION](https://paystack.com/docs/api/)
-
-> 📝: Read more on paystackease api documentation: [PayStackEase DOCUMENTATION](https://paystackease.readthedocs.io/en/latest/)
-
-
-## Getting Started
-
-You should create a Paystack account to generate a **Paystack Secret Key**. You can see this in the *settings page >> API keys and Webhook section*.
-
-> ⚠️: **Warning:** Do not expose your secret key or commit your secret key to git, or use them in client-side code.
-
-> 💡: **Take Note:**  Public key is to be used from your front-end when integrating using Paystack Inline. In this case you have to use you secret key
-
-> ✅: **Good**: Set your secret key in environment variables as seen: *PAYSTACK_SECRET_KEY=your-secret-key*
-
-
-## Create a Virtual Environment
-
-1. For Windows:
-
-    * Create virtual environment
-
-        ```
-            py -m venv <environment_name>
-       ```
-    * Activate the virtual environment
-
-        ```
-            <environment_name>\Scripts\activate
-       ```
-
-2. For Unix/macOS
-
-    * Create virtual environment
-
-        ```
-            python3 -m venv <environment_name>
-       ```
-    * Activate the virtual environment
-
-        ```
-            <environment_name>/bin/activate
-       ```
-
-----------------------------------------------------------------------
-
-## Install paystackease library:
-
-
-* #### Install paystackease using pip.
-
-> pip install paystackease
-
-* #### Install paystackease using pipx.
-
-> pipx install paystackease
-
-* #### Install paystackease using poetry.
-
-> poetry add paystackease
-
-
-## If you want to download the sdist packages directly:
-
-Download the wheel distribution file and install using pip
-
->  pip install paystackease-2.0.0-py3-none-any.whl 
-
-Download the source distribution file, and install using pip
-
-> pip install paystackease-2.0.0.tar.gz 
-
-
-## To get a development version of paystackease
-
-Clone from the ``dev`` branch GitHub repository, unzip and install:
-
-> git clone -b dev https://github.com/cla-bit/PayStackEase.git
-
-> cd PayStackEase
-
-> pip install paystackease
-
-----------------------------------------------------------------------
-
-## API usage
-
--------------------------------------------------------
-
-### Making a Transaction [Synchronous]
-
-If after setting your secret key in environment variables, for a synchronous transaction process 
-all you need to do is use the transaction API to make a transaction. 
-
-To create a transaction or initialize a transaction:
-
-* import the Paystack API wrapper.
-
-```apacheconf
-    from paystackease import PayStackBase
-```
-
-* Create an instance to use the PaystackBase wrapper to interact with the Transaction API.
-
-```apacheconf
-    paystack_client = PayStackBase()
-```
-
-* Use the instance and call the transaction method to initialize a transaction
-
-```apacheconf
-    create_transaction = paystack_client.transactions.initialize(
-        email="johndoe@email.com",
-        amount=10000000)
-    
-    print(f"Transaction Created: {create_transaction}")
-```
-
-> ✅: **Good**: You can check your Paystack account, go to the Transaction page, and you will see the transaction just created.
-
-
-# Other Tools
-Similar to calling the PayStackBase, you can also call other tools to make your work easy. For example:
-
-* ### Account Type
-```apacheconf
-    from paystackease import AccountType
-    
-    val1 = AccountType.PERSONAL.value
-    
-    print(val1)
-```
-> "personal"
-
-* ### Convert units to subunits:
-```apacheconf
-    from paystackease import convert_to_subunit
-    
-    # amount should be in subunit in this case 10000 kobo = 100 naira
-    money = convert_to_subunit(100, Currency.NGN)
-    print(money)
-```
-> 10000
-
-* ### Channels
-```apacheconf
-    from paystackease import Channels
-    
-    bank = Channels.BANK.value
-    
-    print(bank)
-```
-> "bank"
-
-* ### Currency
-```apacheconf
-    from paystackease import Currency
-    
-    val1 = Currency.NGN.value
-    
-    print(val1)
-```
-> "NGN"
-
-* ### Document Type
-```apacheconf
-    from paystackease import DocumentType
-    
-    val1 = DocumentType.IDENTITY_NUMBER.value
-    
-    print(val1)
-```
-
-> "identityNumber"
-
-Others are: ***EventType, Interval, MobileMoney, PWT, QRCODE, RecipientType, ResendOTP, Resolution, RiskAction, SplitType, STATUS, etc***.
+# PayStackEase Library  
+
+--------------
+
+![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease.svg) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
+
+
+**PayStackEase API Library**  is a Python library that simplifies interacting with the Paystack API. 
+It provides both asynchronous and synchronous wrappers for various Paystack functionalities, 
+making it easier to integrate payment processing into your Python projects.
+
+> 📝: Read more on paystack api documentation: [Paystack API DOCUMENTATION](https://paystack.com/docs/api/)
+
+> 📝: Read more on paystackease api documentation: [PayStackEase DOCUMENTATION](https://paystackease.readthedocs.io/en/latest/)
+
+
+## Getting Started
+
+You should create a Paystack account to generate a **Paystack Secret Key**. You can see this in the *settings page >> API keys and Webhook section*.
+
+> ⚠️: **Warning:** Do not expose your secret key or commit your secret key to git, or use them in client-side code.
+
+> 💡: **Take Note:**  Public key is to be used from your front-end when integrating using Paystack Inline. In this case you have to use you secret key
+
+> ✅: **Good**: Set your secret key in environment variables as seen: *PAYSTACK_SECRET_KEY=your-secret-key*
+
+
+## Create a Virtual Environment
+
+1. For Windows:
+
+    * Create virtual environment
+
+        ```
+            py -m venv <environment_name>
+       ```
+    * Activate the virtual environment
+
+        ```
+            <environment_name>\Scripts\activate
+       ```
+
+2. For Unix/macOS
+
+    * Create virtual environment
+
+        ```
+            python3 -m venv <environment_name>
+       ```
+    * Activate the virtual environment
+
+        ```
+            <environment_name>/bin/activate
+       ```
+
+----------------------------------------------------------------------
+
+## Install paystackease library:
+
+
+* #### Install paystackease using pip.
+
+> pip install paystackease
+
+* #### Install paystackease using pipx.
+
+> pipx install paystackease
+
+* #### Install paystackease using poetry.
+
+> poetry add paystackease
+
+
+## If you want to download the sdist packages directly:
+
+Download the wheel distribution file and install using pip
+
+>  pip install paystackease-2.0.0-py3-none-any.whl 
+
+Download the source distribution file, and install using pip
+
+> pip install paystackease-2.0.0.tar.gz 
+
+
+## To get a development version of paystackease
+
+Clone from the ``dev`` branch GitHub repository, unzip and install:
+
+> git clone -b dev https://github.com/cla-bit/PayStackEase.git
+
+> cd PayStackEase
+
+> pip install paystackease
+
+----------------------------------------------------------------------
+
+## API usage
+
+-------------------------------------------------------
+
+### Making a Transaction [Synchronous]
+
+If after setting your secret key in environment variables, for a synchronous transaction process 
+all you need to do is use the transaction API to make a transaction. 
+
+To create a transaction or initialize a transaction:
+
+* import the Paystack API wrapper.
+
+```apacheconf
+    from paystackease import PayStackBase
+```
+
+* Create an instance to use the PaystackBase wrapper to interact with the Transaction API.
+
+```apacheconf
+    paystack_client = PayStackBase()
+```
+
+* Use the instance and call the transaction method to initialize a transaction
+
+```apacheconf
+    create_transaction = paystack_client.transactions.initialize(
+        email="johndoe@email.com",
+        amount=10000000)
+    
+    print(f"Transaction Created: {create_transaction}")
+```
+
+> ✅: **Good**: You can check your Paystack account, go to the Transaction page, and you will see the transaction just created.
+
+
+# Other Tools
+Similar to calling the PayStackBase, you can also call other tools to make your work easy. For example:
+
+* ### Account Type
+```apacheconf
+    from paystackease import AccountType
+    
+    val1 = AccountType.PERSONAL.value
+    
+    print(val1)
+```
+> "personal"
+
+* ### Convert units to subunits:
+```apacheconf
+    from paystackease import convert_to_subunit
+    
+    # amount should be in subunit in this case 10000 kobo = 100 naira
+    money = convert_to_subunit(100, Currency.NGN)
+    print(money)
+```
+> 10000
+
+* ### Channels
+```apacheconf
+    from paystackease import Channels
+    
+    bank = Channels.BANK.value
+    
+    print(bank)
+```
+> "bank"
+
+* ### Currency
+```apacheconf
+    from paystackease import Currency
+    
+    val1 = Currency.NGN.value
+    
+    print(val1)
+```
+> "NGN"
+
+* ### Document Type
+```apacheconf
+    from paystackease import DocumentType
+    
+    val1 = DocumentType.IDENTITY_NUMBER.value
+    
+    print(val1)
+```
+
+> "identityNumber"
+
+Others are: ***EventType, Interval, MobileMoney, PWT, QRCODE, RecipientType, ResendOTP, Resolution, RiskAction, SplitType, STATUS, etc***.
```

### Comparing `paystackease-2.0.0/paystackease/__init__.py` & `paystackease-2.0.4/paystackease/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-""" Wrappers for Paystack API calls"""
-from paystackease.core import (
-    PayStackError,
-    SecretKeyError,
-    TypeValueError,
-    InvalidRequestMethodError
-)
-from paystackease.apaystack import AsyncPayStackBase
-from paystackease.paystack import PayStackBase
-from paystackease.helpers import (
-    convert_to_subunit,
-    AccountType,
-    Bearer,
-    Currency,
-    Channels,
-    DisputeStatus,
-    DocumentType,
-    DVABank,
-    EFT,
-    EventAction,
-    EventType,
-    GateWay,
-    Interval,
-    MobileMoney,
-    PayMentRequestStatus,
-    PWT,
-    QRCODE,
-    RecipientType,
-    ResendOTP,
-    Resolution,
-    RiskAction,
-    SettlementSchedule,
-    SplitType,
-    STATUS,
-    TransactionStatus,
-    USSD,
-)
-
-__all__ = [
-    'PayStackBase',
-    'AsyncPayStackBase',
-    'PayStackError',
-    'SecretKeyError',
-    'TypeValueError',
-    'InvalidRequestMethodError',
-    'convert_to_subunit',
-    'AccountType',
-    'Bearer',
-    'Currency',
-    'Channels',
-    'DisputeStatus',
-    'DocumentType',
-    'DVABank',
-    'EFT',
-    'EventAction',
-    'EventType',
-    'GateWay',
-    'Interval',
-    'MobileMoney',
-    'PayMentRequestStatus',
-    'PWT',
-    'QRCODE',
-    'RecipientType',
-    'ResendOTP',
-    'Resolution',
-    'RiskAction',
-    'SettlementSchedule',
-    'SplitType',
-    'STATUS',
-    'TransactionStatus',
-    'USSD',
-]
+""" Wrappers for Paystack API calls"""
+from paystackease.core import (
+    PayStackError,
+    SecretKeyError,
+    TypeValueError,
+    InvalidRequestMethodError
+)
+from paystackease.apaystack import AsyncPayStackBase
+from paystackease.paystack import PayStackBase
+from paystackease.helpers import (
+    convert_to_subunit,
+    AccountType,
+    Bearer,
+    Currency,
+    Channels,
+    DisputeStatus,
+    DocumentType,
+    DVABank,
+    EFT,
+    EventAction,
+    EventType,
+    GateWay,
+    Interval,
+    MobileMoney,
+    PayMentRequestStatus,
+    PWT,
+    QRCODE,
+    RecipientType,
+    ResendOTP,
+    Resolution,
+    RiskAction,
+    SettlementSchedule,
+    SplitType,
+    STATUS,
+    TransactionStatus,
+    USSD,
+)
+
+__all__ = [
+    'PayStackBase',
+    'AsyncPayStackBase',
+    'PayStackError',
+    'SecretKeyError',
+    'TypeValueError',
+    'InvalidRequestMethodError',
+    'convert_to_subunit',
+    'AccountType',
+    'Bearer',
+    'Currency',
+    'Channels',
+    'DisputeStatus',
+    'DocumentType',
+    'DVABank',
+    'EFT',
+    'EventAction',
+    'EventType',
+    'GateWay',
+    'Interval',
+    'MobileMoney',
+    'PayMentRequestStatus',
+    'PWT',
+    'QRCODE',
+    'RecipientType',
+    'ResendOTP',
+    'Resolution',
+    'RiskAction',
+    'SettlementSchedule',
+    'SplitType',
+    'STATUS',
+    'TransactionStatus',
+    'USSD',
+]
```

### Comparing `paystackease-2.0.0/paystackease/apaystack.py` & `paystackease-2.0.4/paystackease/apaystack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,143 @@
-""" Wrapper classes for various Asynchronous Paystack API endpoints,
-providing simplified access to functionality in Paystack
-"""
-
-from paystackease.apis.async_apis import (
-    aapple_pay,
-    abulk_charges,
-    acharges,
-    acustomers,
-    adedicated_virtual_accounts,
-    adisputes,
-    aintegration,
-    amiscellaneous,
-    apayment_pages,
-    apayment_requests,
-    aplans,
-    aproducts,
-    arefund,
-    asettlements,
-    asubaccounts,
-    asubscriptions,
-    aterminal,
-    atransaction_splits,
-    atransactions,
-    atransfer_recipients,
-    atransfers,
-    atransfers_control,
-    averification,
-)
-from paystackease.core import AsyncRequestAPI
-
-
-class AsyncPayStackBase(AsyncRequestAPI):
-    """AsyncPayStackBase acts as a wrapper around various client APIs to
-    interact with the PayStack API
-    """
-
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, secret_key=None):
-        super().__init__(secret_key)
-        self.apple_pay = aapple_pay.AsyncApplePayClientAPI(secret_key=secret_key)
-        self.bulk_charges = abulk_charges.AsyncBulkChargesClientAPI(
-            secret_key=secret_key
-        )
-        self.charges = acharges.AsyncChargesClientAPI(secret_key=secret_key)
-        self.customers = acustomers.AsyncCustomerClientAPI(secret_key=secret_key)
-        self.dedicated_virtual_accounts = (
-            adedicated_virtual_accounts.AsyncDedicatedVirtualAccountClientAPI(
-                secret_key=secret_key
-            )
-        )
-        self.disputes = adisputes.AsyncDisputesClientAPI(secret_key=secret_key)
-        self.integration = aintegration.AsyncIntegrationClientAPI(secret_key=secret_key)
-        self.miscellaneous = amiscellaneous.AsyncMiscellaneousClientAPI(
-            secret_key=secret_key
-        )
-        self.payment_pages = apayment_pages.AsyncPaymentPagesClientAPI(
-            secret_key=secret_key
-        )
-        self.payment_requests = apayment_requests.AsyncPaymentRequestClientAPI(
-            secret_key=secret_key
-        )
-        self.plans = aplans.AsyncPlanClientAPI(secret_key=secret_key)
-        self.products = aproducts.AsyncProductClientAPI(secret_key=secret_key)
-        self.refund = arefund.AsyncRefundClientAPI(secret_key=secret_key)
-        self.settlements = asettlements.AsyncSettlementClientAPI(secret_key=secret_key)
-        self.subaccounts = asubaccounts.AsyncSubAccountClientAPI(secret_key=secret_key)
-        self.subscriptions = asubscriptions.AsyncSubscriptionClientAPI(
-            secret_key=secret_key
-        )
-        self.terminal = aterminal.AsyncTerminalClientAPI(secret_key=secret_key)
-        self.transaction_splits = atransaction_splits.AsyncTransactionSplitClientAPI(
-            secret_key=secret_key
-        )
-        self.transactions = atransactions.AsyncTransactionClientAPI(
-            secret_key=secret_key
-        )
-        self.transfer_recipients = (
-            atransfer_recipients.AsyncTransferRecipientsClientAPI(secret_key=secret_key)
-        )
-        self.transfers = atransfers.AsyncTransfersClientAPI(secret_key=secret_key)
-        self.transfer_control = atransfers_control.AsyncTransferControlClientAPI(
-            secret_key=secret_key
-        )
-        self.verification = averification.AsyncVerificationClientAPI(
-            secret_key=secret_key
-        )
-
-    async def __aenter__(self):
-        await super().__aenter__()
-        await self.apple_pay.__aenter__()
-        await self.bulk_charges.__aenter__()
-        await self.charges.__aenter__()
-        await self.customers.__aenter__()
-        await self.dedicated_virtual_accounts.__aenter__()
-        await self.disputes.__aenter__()
-        await self.integration.__aenter__()
-        await self.miscellaneous.__aenter__()
-        await self.payment_pages.__aenter__()
-        await self.payment_requests.__aenter__()
-        await self.plans.__aenter__()
-        await self.products.__aenter__()
-        await self.refund.__aenter__()
-        await self.settlements.__aenter__()
-        await self.subaccounts.__aenter__()
-        await self.subscriptions.__aenter__()
-        await self.terminal.__aenter__()
-        await self.transaction_splits.__aenter__()
-        await self.transactions.__aenter__()
-        await self.transfer_recipients.__aenter__()
-        await self.transfers.__aenter__()
-        await self.transfer_control.__aenter__()
-        await self.verification.__aenter__()
-        return self
-
-    async def __aexit__(self, *args):
-        await self.apple_pay.__aexit__(*args)
-        await self.bulk_charges.__aexit__(*args)
-        await self.charges.__aexit__(*args)
-        await self.customers.__aexit__(*args)
-        await self.dedicated_virtual_accounts.__aexit__(*args)
-        await self.disputes.__aexit__(*args)
-        await self.integration.__aexit__(*args)
-        await self.miscellaneous.__aexit__(*args)
-        await self.payment_pages.__aexit__(*args)
-        await self.payment_requests.__aexit__(*args)
-        await self.plans.__aexit__(*args)
-        await self.products.__aexit__(*args)
-        await self.refund.__aexit__(*args)
-        await self.settlements.__aexit__(*args)
-        await self.subaccounts.__aexit__(*args)
-        await self.subscriptions.__aexit__(*args)
-        await self.terminal.__aexit__(*args)
-        await self.transaction_splits.__aexit__(*args)
-        await self.transactions.__aexit__(*args)
-        await self.transfer_recipients.__aexit__(*args)
-        await self.transfers.__aexit__(*args)
-        await self.transfer_control.__aexit__(*args)
-        await self.verification.__aexit__(*args)
-        await super().__aexit__(*args)
+""" Wrapper classes for various Asynchronous Paystack API endpoints,
+providing simplified access to functionality in Paystack
+"""
+
+from paystackease.apis.async_apis import (
+    aapple_pay,
+    abulk_charges,
+    acharges,
+    acustomers,
+    adedicated_virtual_accounts,
+    adisputes,
+    aintegration,
+    amiscellaneous,
+    apayment_pages,
+    apayment_requests,
+    aplans,
+    aproducts,
+    arefund,
+    asettlements,
+    asubaccounts,
+    asubscriptions,
+    aterminal,
+    atransaction_splits,
+    atransactions,
+    atransfer_recipients,
+    atransfers,
+    atransfers_control,
+    averification,
+)
+from paystackease.core import AsyncRequestAPI
+from paystackease.metadata.__version__ import __version__
+
+
+class AsyncPayStackBase(AsyncRequestAPI):
+    """AsyncPayStackBase acts as a wrapper around various client APIs to
+    interact with the PayStack API
+    """
+
+    VERSION = __version__
+
+    # pylint: disable=too-many-instance-attributes
+    def __init__(self, secret_key=None):
+        super().__init__(secret_key)
+        self.apple_pay = aapple_pay.AsyncApplePayClientAPI(secret_key=secret_key)
+        self.bulk_charges = abulk_charges.AsyncBulkChargesClientAPI(
+            secret_key=secret_key
+        )
+        self.charges = acharges.AsyncChargesClientAPI(secret_key=secret_key)
+        self.customers = acustomers.AsyncCustomerClientAPI(secret_key=secret_key)
+        self.dedicated_virtual_accounts = (
+            adedicated_virtual_accounts.AsyncDedicatedVirtualAccountClientAPI(
+                secret_key=secret_key
+            )
+        )
+        self.disputes = adisputes.AsyncDisputesClientAPI(secret_key=secret_key)
+        self.integration = aintegration.AsyncIntegrationClientAPI(secret_key=secret_key)
+        self.miscellaneous = amiscellaneous.AsyncMiscellaneousClientAPI(
+            secret_key=secret_key
+        )
+        self.payment_pages = apayment_pages.AsyncPaymentPagesClientAPI(
+            secret_key=secret_key
+        )
+        self.payment_requests = apayment_requests.AsyncPaymentRequestClientAPI(
+            secret_key=secret_key
+        )
+        self.plans = aplans.AsyncPlanClientAPI(secret_key=secret_key)
+        self.products = aproducts.AsyncProductClientAPI(secret_key=secret_key)
+        self.refund = arefund.AsyncRefundClientAPI(secret_key=secret_key)
+        self.settlements = asettlements.AsyncSettlementClientAPI(secret_key=secret_key)
+        self.subaccounts = asubaccounts.AsyncSubAccountClientAPI(secret_key=secret_key)
+        self.subscriptions = asubscriptions.AsyncSubscriptionClientAPI(
+            secret_key=secret_key
+        )
+        self.terminal = aterminal.AsyncTerminalClientAPI(secret_key=secret_key)
+        self.transaction_splits = atransaction_splits.AsyncTransactionSplitClientAPI(
+            secret_key=secret_key
+        )
+        self.transactions = atransactions.AsyncTransactionClientAPI(
+            secret_key=secret_key
+        )
+        self.transfer_recipients = (
+            atransfer_recipients.AsyncTransferRecipientsClientAPI(secret_key=secret_key)
+        )
+        self.transfers = atransfers.AsyncTransfersClientAPI(secret_key=secret_key)
+        self.transfer_control = atransfers_control.AsyncTransferControlClientAPI(
+            secret_key=secret_key
+        )
+        self.verification = averification.AsyncVerificationClientAPI(
+            secret_key=secret_key
+        )
+
+    async def __aenter__(self):
+        await super().__aenter__()
+        await self.apple_pay.__aenter__()
+        await self.bulk_charges.__aenter__()
+        await self.charges.__aenter__()
+        await self.customers.__aenter__()
+        await self.dedicated_virtual_accounts.__aenter__()
+        await self.disputes.__aenter__()
+        await self.integration.__aenter__()
+        await self.miscellaneous.__aenter__()
+        await self.payment_pages.__aenter__()
+        await self.payment_requests.__aenter__()
+        await self.plans.__aenter__()
+        await self.products.__aenter__()
+        await self.refund.__aenter__()
+        await self.settlements.__aenter__()
+        await self.subaccounts.__aenter__()
+        await self.subscriptions.__aenter__()
+        await self.terminal.__aenter__()
+        await self.transaction_splits.__aenter__()
+        await self.transactions.__aenter__()
+        await self.transfer_recipients.__aenter__()
+        await self.transfers.__aenter__()
+        await self.transfer_control.__aenter__()
+        await self.verification.__aenter__()
+        return self
+
+    async def __aexit__(self, *args):
+        await self.apple_pay.__aexit__(*args)
+        await self.bulk_charges.__aexit__(*args)
+        await self.charges.__aexit__(*args)
+        await self.customers.__aexit__(*args)
+        await self.dedicated_virtual_accounts.__aexit__(*args)
+        await self.disputes.__aexit__(*args)
+        await self.integration.__aexit__(*args)
+        await self.miscellaneous.__aexit__(*args)
+        await self.payment_pages.__aexit__(*args)
+        await self.payment_requests.__aexit__(*args)
+        await self.plans.__aexit__(*args)
+        await self.products.__aexit__(*args)
+        await self.refund.__aexit__(*args)
+        await self.settlements.__aexit__(*args)
+        await self.subaccounts.__aexit__(*args)
+        await self.subscriptions.__aexit__(*args)
+        await self.terminal.__aexit__(*args)
+        await self.transaction_splits.__aexit__(*args)
+        await self.transactions.__aexit__(*args)
+        await self.transfer_recipients.__aexit__(*args)
+        await self.transfers.__aexit__(*args)
+        await self.transfer_control.__aexit__(*args)
+        await self.verification.__aexit__(*args)
+        await super().__aexit__(*args)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/aapple_pay.py` & `paystackease-2.0.4/paystackease/apis/async_apis/aapple_pay.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-"""
-Wrapper class for Asynchronous Paystack Apple Pay API.
-
-The Apple Pay API allows you register your application's top-level domain or subdomain.
-"""
-
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-
-
-class AsyncApplePayClientAPI(AsyncRequestAPI):
-    """
-    Paystack Apple Pay API
-    Reference: https://paystack.com/docs/api/apple-pay/
-    """
-
-    async def register_domain(self, domain_name: str) -> PayStackResponse:
-        """
-        Register a domain or subdomain for Apple Pay
-
-        :param: domain_name  # domain name or subdomain
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "domainName": domain_name,
-        }
-        return await self._post_request("/apple-pay/domain", data=data)
-
-    async def list_domains(
-        self,
-            use_cursor: Optional[Union[bool, None]] = False,
-            next_page: Optional[Union[int, None]] = None,
-            previous_page: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all registered domains
-
-        :param: use_cursor  # use cursor for pagination
-        :param: next_page  # next page
-        :param: previous_page  # previous page
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        use_cursor = self._convert_to_string(use_cursor)
-
-        params = {
-            "use_cursor": use_cursor,
-            "next": next_page,
-            "previous": previous_page,
-        }
-        return await self._get_request("/apple-pay/domain", params=params)
-
-    async def unregister_domain(self, domain_name: str) -> PayStackResponse:
-        """
-        Unregister a domain or subdomain for Apple Pay
-
-        :param: domain_name  # domain name or subdomain
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "domainName": domain_name,
-        }
-        return await self._delete_request("/apple-pay/domain", data=data)
+"""
+Wrapper class for Asynchronous Paystack Apple Pay API.
+
+The Apple Pay API allows you register your application's top-level domain or subdomain.
+"""
+
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+
+
+class AsyncApplePayClientAPI(AsyncRequestAPI):
+    """
+    Paystack Apple Pay API
+    Reference: https://paystack.com/docs/api/apple-pay/
+    """
+
+    async def register_domain(self, domain_name: str) -> PayStackResponse:
+        """
+        Register a domain or subdomain for Apple Pay
+
+        :param: domain_name  # domain name or subdomain
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "domainName": domain_name,
+        }
+        return await self._post_request("/apple-pay/domain", data=data)
+
+    async def list_domains(
+        self,
+            use_cursor: Optional[Union[bool, None]] = False,
+            next_page: Optional[Union[int, None]] = None,
+            previous_page: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all registered domains
+
+        :param: use_cursor  # use cursor for pagination
+        :param: next_page  # next page
+        :param: previous_page  # previous page
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        use_cursor = self._convert_to_string(use_cursor)
+
+        params = {
+            "use_cursor": use_cursor,
+            "next": next_page,
+            "previous": previous_page,
+        }
+        return await self._get_request("/apple-pay/domain", params=params)
+
+    async def unregister_domain(self, domain_name: str) -> PayStackResponse:
+        """
+        Unregister a domain or subdomain for Apple Pay
+
+        :param: domain_name  # domain name or subdomain
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "domainName": domain_name,
+        }
+        return await self._delete_request("/apple-pay/domain", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/abulk_charges.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/bulk_charges.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,142 @@
-"""
-Wrapper for Asynchronous Paystack Bulk Charges API.
-
-The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
-"""
-
-from datetime import date
-from typing import List, Dict, Optional, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import STATUS
-
-
-class AsyncBulkChargesClientAPI(AsyncRequestAPI):
-    """
-    Paystack Bulk Charges API
-    Reference: https://paystack.com/docs/api/bulk-charge/
-    """
-
-    async def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> PayStackResponse:
-        """
-        Send an array of objects with authorization codes and amount
-
-        :param: objects
-
-        note::
-
-            A list of dictionary with authorization codes, amount and reference as keys
-            [{"authorization": "123456", "amount": 1000, "reference": "123456" }]
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._post_request("/bulkcharge", data=objects)
-
-    async def list_bulk_charge_batches(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all bulk charges
-
-        :param: per_page
-        :param: page
-        :param: from_date
-        :param: to_date
-
-        note::
-
-            Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # Convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/bulkcharge", params=params)
-
-    async def fetch_bulk_charge_batch(self, id_or_code: str) -> PayStackResponse:
-        """
-        Fetch a bulk charge of a specific batch
-
-        :param: id_or_code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/bulkcharge/{id_or_code}")
-
-    async def fetch_charge_bulk_batch(
-            self,
-            id_or_code: str,
-            status: Optional[Union[STATUS, None]] = None,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Fetch a bulk charge of a specific batch
-
-        :param: id_or_code
-        :param: status:  {STATUS.value.value}
-        :param: per_page
-        :param: page
-        :param: from_date
-        :param: to_date
-
-        note::
-
-            Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
-            status: STATUS.value.value
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # Convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "status": status,
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
-
-    async def pause_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
-        """
-        Pause a bulk charge of a specific batch
-
-        :param: batch_code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/bulkcharge/pause/{batch_code}")
-
-    async def resume_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
-        """
-        Resume a bulk charge of a specific batch
-
-        :param: batch_code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/bulkcharge/resume/{batch_code}")
+""" Wrapper for Paystack Bulk Charges API.
+
+The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
+"""
+
+from datetime import date
+from typing import List, Dict, Optional, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import STATUS
+
+
+class BulkChargesClientAPI(SyncRequestAPI):
+    """
+    Paystack Bulk Charges API
+    Reference: https://paystack.com/docs/api/bulk-charge/
+    """
+
+    def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> PayStackResponse:
+        """
+        Send an array of objects with authorization codes and amount
+
+        :param: objects
+
+        note::
+
+            A list of dictionary with authorization codes, amount and reference as keys
+            [{"authorization": "123456", "amount": 1000, "reference": "123456" }]
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request("/bulkcharge", data=objects)
+
+    def list_bulk_charge_batches(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all bulk charges
+
+        :param: per_page
+        :param: page
+        :param: from_date
+        :param: to_date
+
+        note::
+
+            Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # Convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/bulkcharge", params=params)
+
+    def fetch_bulk_charge_batch(self, id_or_code: str) -> PayStackResponse:
+        """
+        Fetch a bulk charge of a specific batch
+
+        :param: id_or_code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/bulkcharge/{id_or_code}")
+
+    def fetch_charge_bulk_batch(
+            self,
+            id_or_code: str,
+            status: Optional[Union[STATUS, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Fetch a bulk charge of a specific batch
+
+        :param: id_or_code
+        :param: status:  {STATUS.value.value}
+        :param: per_page
+        :param: page
+        :param: from_date
+        :param: to_date
+
+        note::
+
+            Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
+            status: STATUS.value.value
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # Convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "status": status,
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
+
+    def pause_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
+        """
+        Pause a bulk charge of a specific batch
+
+        :param: batch_code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/bulkcharge/pause/{batch_code}")
+
+    def resume_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
+        """
+        Resume a bulk charge of a specific batch
+
+        :param: batch_code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/bulkcharge/resume/{batch_code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/acharges.py` & `paystackease-2.0.4/paystackease/apis/async_apis/acharges.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-"""
-Wrapper for Asynchronous Paystack Charges API.
-
-The Charge API allows you to configure payment channel of your choice when initiating a payment.
-"""
-
-from datetime import date
-from typing import Optional, Dict, Any, List, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import PWT
-
-
-class AsyncChargesClientAPI(AsyncRequestAPI):
-    """
-    Paystack Charges API
-    Reference: https://paystack.com/docs/api/charge/
-    """
-
-    async def create_charge(
-        self,
-            email: str,
-            amount: int,
-            metadata: Dict[str, List[Dict[str, Any]]],
-            authorization_code: Optional[Union[str, None]] = None,
-            pin: Optional[Union[int, None]] = None,
-            reference: Optional[Union[str, None]] = None,
-            device_id: Optional[Union[str, None]] = None,
-            bank: Optional[Union[Dict[str, str], None]] = None,
-            bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
-            qr: Optional[Union[Dict[str, str], None]] = None,
-            ussd: Optional[Union[Dict[str, str], None]] = None,
-            mobile_money: Optional[Union[Dict[str, str], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a charge
-
-        :param: email
-        :param: amount
-        :param: bank. (Set key ass: {code, account_number})
-        :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
-        :param: qr (Set key as: {provider})
-        :param: authorization_code
-        :param: pin
-        :param: reference
-        :param: ussd (Set key as: {type})
-        :param: mobile_money (Set Keys as: {phone, provider}, and value {phone_number, MobileMoney.value.value})
-        :param: device_id
-        :param: metadata A JSON object, which is passed as-is to your integration API
-
-        note::
-
-            Do not send or use the following if charging an authorization code:
-            * bank
-            * ussd
-            * mobile_money
-
-            Do not send or use the following if charging an authorization code, bank or card:
-            * ussd
-            * mobile_money
-
-            Send with a non-reusable authorization code:
-            * pin
-
-            mobile_money is only available in Ghana and Kenya
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "amount": amount,
-            "metadata": metadata,
-            "authorization_code": authorization_code,
-            "bank": bank,
-            "bank_transfer": bank_transfer,
-            "qr": qr,
-            "pin": pin,
-            "reference": reference,
-            "ussd": ussd,
-            "mobile_money": mobile_money,
-            "device_id": device_id,
-        }
-        return await self._post_request("/charge", data=data)
-
-    async def submit_pin(self, pin: int, reference: str) -> PayStackResponse:
-        """
-        Submit a PIN for a charge
-
-        :param: pin
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "pin": pin,
-            "reference": reference,
-        }
-        return await self._post_request("/charge/submit_pin", data=data)
-
-    async def submit_otp(self, otp: int, reference: str) -> PayStackResponse:
-        """
-        Submit OTP to complete a charge
-
-        :param: otp
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "otp": otp,
-            "reference": reference,
-        }
-        return await self._post_request("/charge/submit_otp", data=data)
-
-    async def submit_phone(self, phone: str, reference: str) -> PayStackResponse:
-        """
-        Submit a phone number to complete a charge
-
-        :param: phone
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "phone": phone,
-            "reference": reference,
-        }
-        return await self._post_request("/charge/submit_phone", data=data)
-
-    async def submit_birthday(self, birthday: date, reference: str) -> PayStackResponse:
-        """
-        Submit birthday when required
-
-        :param: birthday
-        :param: reference
-
-        note::
-
-            Birthday submitted by user e.g. 2016-09-21
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        birthday = self._convert_to_string(birthday)
-
-        data = {
-            "birthday": birthday,
-            "reference": reference,
-        }
-        return await self._post_request("/charge/submit_birthday", data=data)
-
-    async def submit_address(
-        self, reference: str, address: str, city: str, state: str, zipcode: str
-    ) -> PayStackResponse:
-        """
-        Submit address to continue a charge
-
-        :param: reference
-        :param: address
-        :param: city
-        :param: state
-        :param: zipcode
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "reference": reference,
-            "address": address,
-            "city": city,
-            "state": state,
-            "zip_code": zipcode,
-        }
-        return await self._post_request("/charge/submit_address", data=data)
-
-    async def check_pending_charge(self, reference: str) -> PayStackResponse:
-        """
-        Check pending charge
-
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/charge/{reference}")
+"""
+Wrapper for Asynchronous Paystack Charges API.
+
+The Charge API allows you to configure payment channel of your choice when initiating a payment.
+"""
+
+from datetime import date
+from typing import Optional, Dict, Any, List, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import PWT
+
+
+class AsyncChargesClientAPI(AsyncRequestAPI):
+    """
+    Paystack Charges API
+    Reference: https://paystack.com/docs/api/charge/
+    """
+
+    async def create_charge(
+        self,
+            email: str,
+            amount: int,
+            metadata: Dict[str, List[Dict[str, Any]]],
+            authorization_code: Optional[Union[str, None]] = None,
+            pin: Optional[Union[int, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+            device_id: Optional[Union[str, None]] = None,
+            bank: Optional[Union[Dict[str, str], None]] = None,
+            bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
+            qr: Optional[Union[Dict[str, str], None]] = None,
+            ussd: Optional[Union[Dict[str, str], None]] = None,
+            mobile_money: Optional[Union[Dict[str, str], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a charge
+
+        :param: email
+        :param: amount
+        :param: bank. (Set key ass: {code, account_number})
+        :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
+        :param: qr (Set key as: {provider})
+        :param: authorization_code
+        :param: pin
+        :param: reference
+        :param: ussd (Set key as: {type})
+        :param: mobile_money (Set Keys as: {phone, provider}, and value {phone_number, MobileMoney.value.value})
+        :param: device_id
+        :param: metadata A JSON object, which is passed as-is to your integration API
+
+        note::
+
+            Do not send or use the following if charging an authorization code:
+            * bank
+            * ussd
+            * mobile_money
+
+            Do not send or use the following if charging an authorization code, bank or card:
+            * ussd
+            * mobile_money
+
+            Send with a non-reusable authorization code:
+            * pin
+
+            mobile_money is only available in Ghana and Kenya
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "amount": amount,
+            "metadata": metadata,
+            "authorization_code": authorization_code,
+            "bank": bank,
+            "bank_transfer": bank_transfer,
+            "qr": qr,
+            "pin": pin,
+            "reference": reference,
+            "ussd": ussd,
+            "mobile_money": mobile_money,
+            "device_id": device_id,
+        }
+        return await self._post_request("/charge", data=data)
+
+    async def submit_pin(self, pin: int, reference: str) -> PayStackResponse:
+        """
+        Submit a PIN for a charge
+
+        :param: pin
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "pin": pin,
+            "reference": reference,
+        }
+        return await self._post_request("/charge/submit_pin", data=data)
+
+    async def submit_otp(self, otp: int, reference: str) -> PayStackResponse:
+        """
+        Submit OTP to complete a charge
+
+        :param: otp
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "otp": otp,
+            "reference": reference,
+        }
+        return await self._post_request("/charge/submit_otp", data=data)
+
+    async def submit_phone(self, phone: str, reference: str) -> PayStackResponse:
+        """
+        Submit a phone number to complete a charge
+
+        :param: phone
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "phone": phone,
+            "reference": reference,
+        }
+        return await self._post_request("/charge/submit_phone", data=data)
+
+    async def submit_birthday(self, birthday: date, reference: str) -> PayStackResponse:
+        """
+        Submit birthday when required
+
+        :param: birthday
+        :param: reference
+
+        note::
+
+            Birthday submitted by user e.g. 2016-09-21
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        birthday = self._convert_to_string(birthday)
+
+        data = {
+            "birthday": birthday,
+            "reference": reference,
+        }
+        return await self._post_request("/charge/submit_birthday", data=data)
+
+    async def submit_address(
+        self, reference: str, address: str, city: str, state: str, zipcode: str
+    ) -> PayStackResponse:
+        """
+        Submit address to continue a charge
+
+        :param: reference
+        :param: address
+        :param: city
+        :param: state
+        :param: zipcode
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "reference": reference,
+            "address": address,
+            "city": city,
+            "state": state,
+            "zip_code": zipcode,
+        }
+        return await self._post_request("/charge/submit_address", data=data)
+
+    async def check_pending_charge(self, reference: str) -> PayStackResponse:
+        """
+        Check pending charge
+
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/charge/{reference}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/acustomers.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/customers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-"""
-Wrapper for Asynchronous Paystack Customers API.
-
-The Customers API allows you to create and manage customers on your integration.
-"""
-
-from datetime import date
-from typing import Optional, Dict, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import RiskAction
-
-
-class AsyncCustomerClientAPI(AsyncRequestAPI):
-    """
-    Paystack Customer API
-    Reference: https://paystack.com/docs/api/customer/
-    """
-
-    async def create_customer(
-            self,
-            email: str,
-            first_name: str,
-            last_name: str,
-            phone: str,
-            metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> PayStackResponse:
-        """
-        Create a customer
-
-        :param: email: The email associated with the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: phone: The phone number of the customer.
-        :param: metadata: The metadata of the customer in JSON format.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-            "metadata": metadata,
-        }
-        return await self._post_request("/customer", data=data)
-
-    async def validate_customer(
-            self,
-            email_or_code: str,
-            first_name: str,
-            last_name: str,
-            account_type: str,
-            country: str,
-            bank_code: str,
-            account_number: str,
-            bvn: str,
-            customer_id_num: Optional[Union[str, None]] = None,
-            middle_name: Optional[Union[str, None]] = None
-    ) -> PayStackResponse:
-        """
-        Validate a customer's identity
-
-        :param: email_or_code: The email or code of the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: middle_name: The middle name of the customer.
-        :param: account_type: The type of account. Only bank_account is currently supported.
-        :param: customer_id_num: The customer identification number
-        :param: country: The country of the customer. 2-letter country code of identification issuer
-        :param: bvn: The Bank Verification Number
-        :param: bank_code: The bank code of the customer
-        :param: account_number: The account number of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "first_name": first_name,
-            "last_name": last_name,
-            "middle_name": middle_name,
-            "type": account_type,
-            "value": customer_id_num,
-            "country": country,
-            "bvn": bvn,
-            "bank_code": bank_code,
-            "account_number": account_number,
-        }
-        return await self._post_request(f"customer/{email_or_code}/identification", data=data)
-
-    async def whitelist_blacklist_customer(
-            self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
-    ) -> PayStackResponse:
-        """
-        Whitelist or blacklist a customer
-
-        :param: email_or_code: The code or email of the customer.
-        :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "customer": email_or_code,
-            "risk_action": risk_action
-        }
-        return await self._post_request("/customer/set_risk_action", data=data)
-
-    async def deactivate_authorization(self, authorization_code: str) -> PayStackResponse:
-        """
-        Deactivate an authorization when the card needs to be forgotten
-
-        :param: authorization_code: The authorization code to be deactivated.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"authorization_code": authorization_code}
-        return await self._post_request("/customer/deactivate_authorization", data=data)
-
-    async def update_customer(
-            self,
-            customer_code: str,
-            first_name: Optional[Union[str, None]] = None,
-            last_name: Optional[Union[str, None]] = None,
-            phone: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> PayStackResponse:
-        """
-        Update a customer
-
-        :param: customer_code: The code of the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: phone: The phone number of the customer.
-        :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-            "metadata": metadata,
-        }
-        return await self._put_request(f"/customer/{customer_code}", data=data)
-
-    async def fetch_customer(self, email_or_code: str) -> PayStackResponse:
-        """
-        Fetch details of a specific customer
-
-        :param: email_or_code: The email or code of the customer.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/customer/{email_or_code}")
-
-    async def list_customers(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all customers
-
-        :param: per_page: The number of records to return.
-        :param: page: The page number to return.
-        :param: from_date: The date to start returning customers from
-        :param: to_date: The date to stop returning customers from
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date  to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/customer", params=params)
+"""
+Wrapper for Paystack Customers API.
+
+The Customers API allows you to create and manage customers on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Dict, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import RiskAction
+
+
+class CustomerClientAPI(SyncRequestAPI):
+    """
+    Paystack Customer API
+    Reference: https://paystack.com/docs/api/customer/
+    """
+
+    def create_customer(
+            self, 
+            email: str, 
+            first_name: str, 
+            last_name: str, 
+            phone: str, 
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> PayStackResponse:
+        """
+        Create a customer
+
+        :param: email: The email associated with the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: phone: The phone number of the customer.
+        :param: metadata: The metadata of the customer in JSON format.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+            "metadata": metadata,
+        }
+        return self._post_request("/customer", data=data)
+
+    def validate_customer(
+            self,
+            email_or_code: str,
+            first_name: str,
+            last_name: str,
+            account_type: str,
+            country: str,
+            bank_code: str,
+            account_number: str,
+            bvn: str,
+            customer_id_num: Optional[Union[str, None]] = None,
+            middle_name: Optional[Union[str, None]] = None
+    ) -> PayStackResponse:
+        """
+        Validate a customer's identity
+
+        :param: email_or_code: The email or code of the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: middle_name: The middle name of the customer.
+        :param: account_type: The type of account. Only bank_account is currently supported.
+        :param: customer_id_num: The customer identification number
+        :param: country: The country of the customer. 2-letter country code of identification issuer
+        :param: bvn: The Bank Verification Number
+        :param: bank_code: The bank code of the customer
+        :param: account_number: The account number of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "first_name": first_name,
+            "last_name": last_name,
+            "middle_name": middle_name,
+            "type": account_type,
+            "value": customer_id_num,
+            "country": country,
+            "bvn": bvn,
+            "bank_code": bank_code,
+            "account_number": account_number,
+        }
+        return self._post_request(f"customer/{email_or_code}/identification", data=data)
+
+    def whitelist_blacklist_customer(
+            self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
+    ) -> PayStackResponse:
+        """
+        Whitelist or blacklist a customer
+
+        :param: email_or_code: The code or email of the customer.
+        :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "customer": email_or_code,
+            "risk_action": risk_action
+        }
+        return self._post_request("/customer/set_risk_action", data=data)
+
+    def deactivate_authorization(self, authorization_code: str) -> PayStackResponse:
+        """
+        Deactivate an authorization when the card needs to be forgotten
+
+        :param: authorization_code: The authorization code to be deactivated.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"authorization_code": authorization_code}
+        return self._post_request("/customer/deactivate_authorization", data=data)
+
+    def update_customer(
+            self,
+            customer_code: str,
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> PayStackResponse:
+        """
+        Update a customer
+
+        :param: customer_code: The code of the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: phone: The phone number of the customer.
+        :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+            "metadata": metadata,
+        }
+        return self._put_request(f"/customer/{customer_code}", data=data)
+
+    def fetch_customer(self, email_or_code: str) -> PayStackResponse:
+        """
+        Fetch details of a specific customer
+
+        :param: email_or_code: The email or code of the customer.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/customer/{email_or_code}")
+
+    def list_customers(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all customers
+
+        :param: per_page: The number of records to return.
+        :param: page: The page number to return.
+        :param: from_date: The date to start returning customers from
+        :param: to_date: The date to stop returning customers from
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date  to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return self._get_request("/customer", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py` & `paystackease-2.0.4/paystackease/apis/async_apis/adedicated_virtual_accounts.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-"""
-Wrapper for Asynchronous Paystack Dedicated Virtual Account API
-
-The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import Currency
-
-
-class AsyncDedicatedVirtualAccountClientAPI(AsyncRequestAPI):
-    """
-    Paystack Dedicated Virtual Account API
-    Reference: https://paystack.com/docs/api/dedicated-virtual-account/
-
-    note::
-        Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
-    """
-
-    async def create_virtual_account(
-            self,
-            customer_id_or_code: str,
-            preferred_bank: Optional[Union[str, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            first_name: Optional[Union[str, None]] = None,
-            last_name: Optional[Union[str, None]] = None,
-            phone: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a dedicated virtual account for existing customers.
-        Currently, support Wema Bank and Titan Paystack.
-
-        :param: customer_id_or_code: The customer's ID or Code
-        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
-
-        note::
-
-             currently support Wema Bank and Titan Paystack.
-
-        :param: subaccount: Subaccount code of the account you want to split the transaction.
-        :param: split_code: Split code
-        :param: first_name: First name of the customer
-        :param: last_name: Last name of the customer
-        :param: phone: Phone number of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "customer": customer_id_or_code,
-            "preferred_bank": preferred_bank,
-            "subaccount": subaccount,
-            "split_code": split_code,
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-        }
-        return await self._post_request("/dedicated_account", data=data)
-
-    async def assign_dedicated_virtual_account(
-            self,
-            email: str,
-            first_name: str,
-            last_name: str,
-            phone: str,
-            preferred_bank: str,
-            country: str,
-            account_number: Optional[Union[str, None]] = None,
-            bvn: Optional[Union[str, None]] = None,
-            bank_code: Optional[Union[str, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        create a customer, validate the customer, and assign a DVA to the customer
-
-        :param: email: The email associated with the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: phone: The phone number of the customer.
-        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
-
-        note::
-
-             currently support Wema Bank and Titan Paystack.
-
-        :param: country: The country of the customer. 2-letter country code of identification issuer
-
-        note::
-
-             currently accepts NG only.
-
-        :param: account_number: The account number of the customer
-        :param: bvn: The Bank Verification Number
-        :param: bank_code: The bank code of the customer
-        :param: subaccount: Subaccount code of the account you want to split the transaction.
-        :param: split_code: Split code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-            "preferred_bank": preferred_bank,
-            "country": country,
-            "account_number": account_number,
-            "bvn": bvn,
-            "bank_code": bank_code,
-            "subaccount": subaccount,
-            "split_code": split_code,
-        }
-        return await self._post_request("/dedicated_account", data=data)
-
-    async def list_dedicated_account(
-            self,
-            active: Optional[Union[bool, None]] = True,
-            currency: Optional[Union[Currency, None]] = None,
-            provider_slug: Optional[Union[str, None]] = None,
-            bank_id: Optional[Union[str, None]] = None,
-            customer_id: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List dedicated accounts
-
-        :param: active: Shows the status of the dedicated virtual account
-        :param: currency: Currency of the dedicated virtual account
-        :param: provider_slug: Provider slug in lowercase eg: wema-bank
-        :param: bank_id: Bank ID of the dedicated virtual account eg: 035
-        :param: customer_id: Customer ID of the dedicated virtual account
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert date to string
-        active = self._convert_to_string(active)
-
-        params = {
-            "active": active,
-            "currency": currency,
-            "provider_slug": provider_slug,
-            "bank_id": bank_id,
-            "customer": customer_id,
-        }
-        return await self._get_request("/dedicated_account", params=params)
-
-    async def fetch_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
-        """
-        Get details of a dedicated virtual account
-
-        :param: dedicated_account_id: Dedicated account ID
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/dedicated_account/{dedicated_account_id}")
-
-    async def requery_dedicated_account(
-            self,
-            account_number: Optional[Union[str, None]] = None,
-            provider_slug: Optional[Union[str, None]] = None,
-            date_transfer: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Requery a dedicated virtual account for new transactions
-
-        :param: account_number: Virtual Account number to requery
-        :param: provider_slug: Provider slug in lowercase eg: wema-bank
-        :param: date_transfer: Date of when the transfer was made
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        date_transfer = self._convert_to_string(date_transfer)
-
-        params = {
-            "account_number": account_number,
-            "provider_slug": provider_slug,
-            "date": date_transfer,
-        }
-        return await self._get_request("/dedicated_account/requery", params=params)
-
-    async def deactivate_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
-        """
-        Deactivate a dedicated virtual account
-
-        :param: dedicated_account_id: Dedicated account ID
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._delete_request(f"/dedicated_account/{dedicated_account_id}")
-
-    async def split_dedicated_account(
-            self,
-            customer_id_or_code: str,
-            subaccount: Optional[Union[str, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            preferred_bank: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Split a dedicated virtual account transaction with one or more accounts
-
-        :param: customer_id_or_code: Customer's ID or Code
-        :param: subaccount: Subaccount code of the account you want to split the transaction
-        :param: split_code: Split code
-        :param: preferred_bank: Preferred bank for the virtual account
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "customer": customer_id_or_code,
-            "preferred_bank": preferred_bank,
-            "subaccount": subaccount,
-            "split_code": split_code,
-        }
-        return await self._post_request("/dedicated_account/split", data=data)
-
-    async def remove_split_dedicated_account(self, account_number: str) -> PayStackResponse:
-        """
-        Remove a split dedicated virtual account
-
-        :param: account_number: the account number of the dedicated virtual account
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "account_number": account_number,
-        }
-        return await self._delete_request("/dedicated_account/split", data=data)
-
-    async def fetch_bank_providers(self) -> PayStackResponse:
-        """
-        Fetch bank providers
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request("/dedicated_account/available_providers")
+"""
+Wrapper for Asynchronous Paystack Dedicated Virtual Account API
+
+The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
+
+
+class AsyncDedicatedVirtualAccountClientAPI(AsyncRequestAPI):
+    """
+    Paystack Dedicated Virtual Account API
+    Reference: https://paystack.com/docs/api/dedicated-virtual-account/
+
+    note::
+        Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
+    """
+
+    async def create_virtual_account(
+            self,
+            customer_id_or_code: str,
+            preferred_bank: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a dedicated virtual account for existing customers.
+        Currently, support Wema Bank and Titan Paystack.
+
+        :param: customer_id_or_code: The customer's ID or Code
+        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
+
+        note::
+
+             currently support Wema Bank and Titan Paystack.
+
+        :param: subaccount: Subaccount code of the account you want to split the transaction.
+        :param: split_code: Split code
+        :param: first_name: First name of the customer
+        :param: last_name: Last name of the customer
+        :param: phone: Phone number of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "customer": customer_id_or_code,
+            "preferred_bank": preferred_bank,
+            "subaccount": subaccount,
+            "split_code": split_code,
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+        }
+        return await self._post_request("/dedicated_account", data=data)
+
+    async def assign_dedicated_virtual_account(
+            self,
+            email: str,
+            first_name: str,
+            last_name: str,
+            phone: str,
+            preferred_bank: str,
+            country: str,
+            account_number: Optional[Union[str, None]] = None,
+            bvn: Optional[Union[str, None]] = None,
+            bank_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        create a customer, validate the customer, and assign a DVA to the customer
+
+        :param: email: The email associated with the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: phone: The phone number of the customer.
+        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
+
+        note::
+
+             currently support Wema Bank and Titan Paystack.
+
+        :param: country: The country of the customer. 2-letter country code of identification issuer
+
+        note::
+
+             currently accepts NG only.
+
+        :param: account_number: The account number of the customer
+        :param: bvn: The Bank Verification Number
+        :param: bank_code: The bank code of the customer
+        :param: subaccount: Subaccount code of the account you want to split the transaction.
+        :param: split_code: Split code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+            "preferred_bank": preferred_bank,
+            "country": country,
+            "account_number": account_number,
+            "bvn": bvn,
+            "bank_code": bank_code,
+            "subaccount": subaccount,
+            "split_code": split_code,
+        }
+        return await self._post_request("/dedicated_account", data=data)
+
+    async def list_dedicated_account(
+            self,
+            active: Optional[Union[bool, None]] = True,
+            currency: Optional[Union[Currency, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            bank_id: Optional[Union[str, None]] = None,
+            customer_id: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List dedicated accounts
+
+        :param: active: Shows the status of the dedicated virtual account
+        :param: currency: Currency of the dedicated virtual account
+        :param: provider_slug: Provider slug in lowercase eg: wema-bank
+        :param: bank_id: Bank ID of the dedicated virtual account eg: 035
+        :param: customer_id: Customer ID of the dedicated virtual account
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert date to string
+        active = self._convert_to_string(active)
+
+        params = {
+            "active": active,
+            "currency": currency,
+            "provider_slug": provider_slug,
+            "bank_id": bank_id,
+            "customer": customer_id,
+        }
+        return await self._get_request("/dedicated_account", params=params)
+
+    async def fetch_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
+        """
+        Get details of a dedicated virtual account
+
+        :param: dedicated_account_id: Dedicated account ID
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/dedicated_account/{dedicated_account_id}")
+
+    async def requery_dedicated_account(
+            self,
+            account_number: Optional[Union[str, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            date_transfer: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Requery a dedicated virtual account for new transactions
+
+        :param: account_number: Virtual Account number to requery
+        :param: provider_slug: Provider slug in lowercase eg: wema-bank
+        :param: date_transfer: Date of when the transfer was made
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        date_transfer = self._convert_to_string(date_transfer)
+
+        params = {
+            "account_number": account_number,
+            "provider_slug": provider_slug,
+            "date": date_transfer,
+        }
+        return await self._get_request("/dedicated_account/requery", params=params)
+
+    async def deactivate_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
+        """
+        Deactivate a dedicated virtual account
+
+        :param: dedicated_account_id: Dedicated account ID
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._delete_request(f"/dedicated_account/{dedicated_account_id}")
+
+    async def split_dedicated_account(
+            self,
+            customer_id_or_code: str,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            preferred_bank: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Split a dedicated virtual account transaction with one or more accounts
+
+        :param: customer_id_or_code: Customer's ID or Code
+        :param: subaccount: Subaccount code of the account you want to split the transaction
+        :param: split_code: Split code
+        :param: preferred_bank: Preferred bank for the virtual account
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "customer": customer_id_or_code,
+            "preferred_bank": preferred_bank,
+            "subaccount": subaccount,
+            "split_code": split_code,
+        }
+        return await self._post_request("/dedicated_account/split", data=data)
+
+    async def remove_split_dedicated_account(self, account_number: str) -> PayStackResponse:
+        """
+        Remove a split dedicated virtual account
+
+        :param: account_number: the account number of the dedicated virtual account
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "account_number": account_number,
+        }
+        return await self._delete_request("/dedicated_account/split", data=data)
+
+    async def fetch_bank_providers(self) -> PayStackResponse:
+        """
+        Fetch bank providers
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request("/dedicated_account/available_providers")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/aintegration.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-Wrapper for Asynchronous Paystack Integration API
-
-The Integration API allows you manage some settings on your integration.
-"""
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-
-
-class AsyncIntegrationClientAPI(AsyncRequestAPI):
-    """
-    Paystack Integration API
-    Reference: https://paystack.com/docs/api/integration/
-    """
-
-    async def fetch_timeout(self) -> PayStackResponse:
-        """
-        Fetch payment session timeout
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request("/integration/payment_session_timeout")
-
-    async def update_timeout(self, timeout: int) -> PayStackResponse:
-        """
-        Update payment session timeout
-
-        :param: timeout: The new payment session timeout before session
-
-        note::
-
-            timeout is in seconds. Set 0 to cancel the timeout
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        data = {"timeout": timeout}
-        return await self._put_request("/integration/payment_session_timeout", data=data)
+"""
+Wrapper for Paystack Integration API
+
+The Integration API allows you manage some settings on your integration.
+"""
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class IntegrationClientAPI(SyncRequestAPI):
+    """
+    Paystack Integration API
+    Reference: https://paystack.com/docs/api/integration/
+    """
+
+    def fetch_timeout(self) -> PayStackResponse:
+        """
+        Fetch payment session timeout
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request("/integration/payment_session_timeout")
+
+    def update_timeout(self, timeout: int) -> PayStackResponse:
+        """
+        Update payment session timeout
+
+        :param: timeout: The new payment session timeout before session
+        
+        note::
+
+            timeout is in seconds. Set 0 to cancel the timeout
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        data = {"timeout": timeout}
+        return self._put_request("/integration/payment_session_timeout", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/amiscellaneous.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/miscellaneous.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,98 @@
-"""
-Wrapper for Paystack Miscellaneous API.
-
-The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
-"""
-
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import GateWay, Channels, Currency
-
-
-class AsyncMiscellaneousClientAPI(AsyncRequestAPI):
-    """
-    Paystack Miscellaneous API
-    Reference: https://paystack.com/docs/api/miscellaneous/
-    """
-
-    async def list_banks(
-            self,
-            country: Optional[Union[str, None]] = None,
-            use_cursor: Optional[Union[bool, None]] = False,
-            per_page: Optional[Union[int, None]] = 50,
-            pay_with_bank_transfer: Optional[Union[bool, None]] = False,
-            pay_with_bank: Optional[Union[bool, None]] = False,
-            enabled_for_verification: Optional[Union[bool, None]] = False,
-            next_cursor: Optional[Union[str, None]] = None,
-            previous_cursor: Optional[Union[str, None]] = None,
-            gateway: Optional[Union[GateWay, None]] = None,
-            channel_type: Optional[Union[Channels, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Get a list of all supported banks and their properties
-
-        :param: country: The country to obtain the list of supported banks.
-                        Values { country=ghana or country=nigeria }
-        :param: use_cursor: Use cursor to paginate through the list of supported banks
-        :param: per_page: The number of records to return per page: 10, 20 or 50
-        :param: pay_with_bank_transfer: filter for available banks a customer can make a transfer to complete a payment
-        :param: pay_with_bank: filter for banks a customer can pay directly from
-        :param: enabled_for_verification: filter the banks that are supported for account
-                                            verification in South Africa. Combine with currency or country filter
-        :param: next_cursor: The cursor for the next page of results
-        :param: previous_cursor: The cursor for the previous page of results
-        :param: gateway: filters for banks that support a specific payment gateway:
-                        { emandate or digitalbankmandate }
-        :param: currency: filter for banks that support a specific currency
-        :param: channel_type: Type of financial channel. { Channels.value.value}
-
-        **note::**
-
-        For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert to strings
-        use_cursor = self._convert_to_string(use_cursor)
-        pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
-        pay_with_bank = self._convert_to_string(pay_with_bank)
-        enabled_for_verification = self._convert_to_string(enabled_for_verification)
-
-        params = {
-            "country": country,
-            "use_cursor": use_cursor,
-            "perPage": per_page,
-            "supports_transfer": pay_with_bank_transfer,
-            "pay_with_bank": pay_with_bank,
-            "enabled_for_verification": enabled_for_verification,
-            "next": next_cursor,
-            "previous": previous_cursor,
-            "gateway": gateway,
-            "type": channel_type,
-            "currency": currency,
-        }
-        return await self._get_request("/bank", params=params)
-
-    async def list_countries(self) -> PayStackResponse:
-        """
-        Get a list of all supported countries and their properties
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request("/country")
-
-    async def list_states(self, country: str) -> PayStackResponse:
-        """
-        Get a list of all supported states and their properties
-
-        :param: country: The country code from which to obtain the list of supported states
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {"country": country}
-        return await self._get_request("/address_verification/states", params=params)
+"""
+Wrapper for Paystack Miscellaneous API.
+
+The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
+"""
+
+from typing import Optional, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import GateWay, Channels, Currency
+
+
+class MiscellaneousClientAPI(SyncRequestAPI):
+    """
+    Paystack Miscellaneous API
+    Reference: https://paystack.com/docs/api/miscellaneous/
+    """
+
+    def list_banks(
+            self,
+            country: Optional[Union[str, None]] = None,
+            use_cursor: Optional[Union[bool, None]] = False,
+            per_page: Optional[Union[int, None]] = 50,
+            pay_with_bank_transfer: Optional[Union[bool, None]] = False,
+            pay_with_bank: Optional[Union[bool, None]] = False,
+            enabled_for_verification: Optional[Union[bool, None]] = False,
+            next_cursor: Optional[Union[str, None]] = None,
+            previous_cursor: Optional[Union[str, None]] = None,
+            gateway: Optional[Union[GateWay, None]] = None,
+            channel_type: Optional[Union[Channels, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Get a list of all supported banks and their properties
+
+        :param: country: The country to obtain the list of supported banks.
+                        Values { country=ghana or country=nigeria }
+        :param: use_cursor: Use cursor to paginate through the list of supported banks
+        :param: per_page: The number of records to return per page: 10, 20 or 50
+        :param: pay_with_bank_transfer: filter for available banks a customer can make a transfer to complete a payment
+        :param: pay_with_bank: filter for banks a customer can pay directly from
+        :param: enabled_for_verification: filter the banks that are supported for account
+                                            verification in South Africa. Combine with currency or country filter
+        :param: next_cursor: The cursor for the next page of results
+        :param: previous_cursor: The cursor for the previous page of results
+        :param: gateway: filters for banks that support a specific payment gateway:
+                        { emandate or digitalbankmandate }
+        :param: currency: filter for banks that support a specific currency
+        :param: channel_type: Type of financial channel. { Channels.value.value}
+
+        **note::**
+
+        For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        use_cursor = self._convert_to_string(use_cursor)
+        pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
+        pay_with_bank = self._convert_to_string(pay_with_bank)
+        enabled_for_verification = self._convert_to_string(enabled_for_verification)
+
+        params = {
+            "country": country,
+            "use_cursor": use_cursor,
+            "perPage": per_page,
+            "supports_transfer": pay_with_bank_transfer,
+            "pay_with_bank": pay_with_bank,
+            "enabled_for_verification": enabled_for_verification,
+            "next": next_cursor,
+            "previous": previous_cursor,
+            "gateway": gateway,
+            "type": channel_type,
+            "currency": currency,
+        }
+        return self._get_request("/bank", params=params)
+
+    def list_countries(self) -> PayStackResponse:
+        """
+        Get a list of all supported countries and their properties
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request("/country")
+
+    def list_states(self, country: str) -> PayStackResponse:
+        """
+        Get a list of all supported states and their properties
+
+        :param: country: The country code from which to obtain the list of supported states
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {"country": country}
+        return self._get_request("/address_verification/states", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/apayment_pages.py` & `paystackease-2.0.4/paystackease/apis/async_apis/apayment_pages.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-"""
-Wrapper for Asynchronous Paystack Payment Pages API.
-
-The Payment Pages API provides a quick and secure way to collect payment for products.
-"""
-
-from datetime import date
-from typing import Optional, Dict, List, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-
-
-class AsyncPaymentPagesClientAPI(AsyncRequestAPI):
-    """
-    Paystack Payment Pages API
-    Reference: https://paystack.com/docs/api/page/
-    """
-
-    async def create_payment_page(
-            self,
-            name: str,
-            description: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            page_slug: Optional[Union[str, None]] = None,
-            redirect_url: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-            custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a payment page
-
-        :param: name: Name of the page
-        :param: description: Description of the page
-        :param: amount: Amount of the page
-        :param: split_code: Split code of the transaction split
-        :param: page_slug: URL slug you would like to be associated with this page.
-
-        note::
-
-            Page will be accessible at https://paystack.com/pay/page_slug
-
-        :param: redirect_url: If you would like Paystack to redirect someplace
-                                upon successful payment, specify the URL here.
-        :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
-        :param: custom_fields: If you would like to accept custom fields, specify them here.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "name": name,
-            "description": description,
-            "amount": amount,
-            "split_code": split_code,
-            "slug": page_slug,
-            "redirect_url": redirect_url,
-            "metadata": metadata,
-            "custom_fields": custom_fields,
-        }
-        return await self._post_request("/page", data=data)
-
-    async def list_payment_pages(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the payment pages
-
-        :param: per_page: Number of records to return
-        :param: page: number to return
-        :param: from_date: A timestamp from which to start listing page
-        :param: to_date: A timestamp from which to start listing page
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-
-        note::
-            Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/page", params=params)
-
-    async def fetch_payment_page(self, page_id_or_slug: str) -> PayStackResponse:
-        """
-        Get details of a payment page
-
-        :param: page_id_or_slug: ID or slug of the payment page
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/page/{page_id_or_slug}")
-
-    async def update_payment_page(
-            self,
-            page_id_or_slug: str,
-            name: Optional[Union[str, None]] = None,
-            description: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            active: Optional[Union[bool, None]] = True,
-    ) -> PayStackResponse:
-        """
-        Update a payment page detail
-
-        :param: page_id_or_slug: ID or slug of the payment page
-        :param: name: Name of the page
-        :param: description: Description of the page
-        :param: amount: Amount of the page
-        :param: active: Set false to deactivate the page url
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "name": name,
-            "description": description,
-            "amount": amount,
-            "active": active,
-        }
-        return await self._put_request(f"/page/{page_id_or_slug}", data=data)
-
-    async def check_slug_available(self, page_slug: str) -> PayStackResponse:
-        """
-        Check if a slug is available
-
-        :param: page_slug: URL slug you would like to be associated with this page.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/page/check_slug_availability/{page_slug}")
-
-    async def add_products(self, payment_id: int, product: List[int]) -> PayStackResponse:
-        """
-        Add products to a payment page
-
-        :param: payment_id: ID of the payment page
-        :param: product: List of IDS of all the products
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"product": product}
-        return await self._post_request(f"/page/{payment_id}/product", data=data)
+"""
+Wrapper for Asynchronous Paystack Payment Pages API.
+
+The Payment Pages API provides a quick and secure way to collect payment for products.
+"""
+
+from datetime import date
+from typing import Optional, Dict, List, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+
+
+class AsyncPaymentPagesClientAPI(AsyncRequestAPI):
+    """
+    Paystack Payment Pages API
+    Reference: https://paystack.com/docs/api/page/
+    """
+
+    async def create_payment_page(
+            self,
+            name: str,
+            description: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            page_slug: Optional[Union[str, None]] = None,
+            redirect_url: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+            custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a payment page
+
+        :param: name: Name of the page
+        :param: description: Description of the page
+        :param: amount: Amount of the page
+        :param: split_code: Split code of the transaction split
+        :param: page_slug: URL slug you would like to be associated with this page.
+
+        note::
+
+            Page will be accessible at https://paystack.com/pay/page_slug
+
+        :param: redirect_url: If you would like Paystack to redirect someplace
+                                upon successful payment, specify the URL here.
+        :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
+        :param: custom_fields: If you would like to accept custom fields, specify them here.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "name": name,
+            "description": description,
+            "amount": amount,
+            "split_code": split_code,
+            "slug": page_slug,
+            "redirect_url": redirect_url,
+            "metadata": metadata,
+            "custom_fields": custom_fields,
+        }
+        return await self._post_request("/page", data=data)
+
+    async def list_payment_pages(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the payment pages
+
+        :param: per_page: Number of records to return
+        :param: page: number to return
+        :param: from_date: A timestamp from which to start listing page
+        :param: to_date: A timestamp from which to start listing page
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+
+        note::
+            Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return await self._get_request("/page", params=params)
+
+    async def fetch_payment_page(self, page_id_or_slug: str) -> PayStackResponse:
+        """
+        Get details of a payment page
+
+        :param: page_id_or_slug: ID or slug of the payment page
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/page/{page_id_or_slug}")
+
+    async def update_payment_page(
+            self,
+            page_id_or_slug: str,
+            name: Optional[Union[str, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+    ) -> PayStackResponse:
+        """
+        Update a payment page detail
+
+        :param: page_id_or_slug: ID or slug of the payment page
+        :param: name: Name of the page
+        :param: description: Description of the page
+        :param: amount: Amount of the page
+        :param: active: Set false to deactivate the page url
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        active = self._convert_to_string(active)
+
+        data = {
+            "name": name,
+            "description": description,
+            "amount": amount,
+            "active": active,
+        }
+        return await self._put_request(f"/page/{page_id_or_slug}", data=data)
+
+    async def check_slug_available(self, page_slug: str) -> PayStackResponse:
+        """
+        Check if a slug is available
+
+        :param: page_slug: URL slug you would like to be associated with this page.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/page/check_slug_availability/{page_slug}")
+
+    async def add_products(self, payment_id: int, product: List[int]) -> PayStackResponse:
+        """
+        Add products to a payment page
+
+        :param: payment_id: ID of the payment page
+        :param: product: List of IDS of all the products
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"product": product}
+        return await self._post_request(f"/page/{payment_id}/product", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/apayment_requests.py` & `paystackease-2.0.4/paystackease/apis/async_apis/apayment_requests.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-"""
-Wrapper for Asynchronous Paystack Payment Requests API.
-
-The Payment Requests API allows you manage requests for payment of goods and services.
-"""
-
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import PayMentRequestStatus, Currency
-
-
-class AsyncPaymentRequestClientAPI(AsyncRequestAPI):
-    """
-    Paystack Payment Request API
-    Reference: https://paystack.com/docs/api/payment-request/
-    """
-
-    async def create_payment_request(
-            self,
-            customer: str,
-            amount: int,
-            draft: bool,
-            has_invoice: bool,
-            send_notification: bool,
-            due_date: Optional[Union[date, None]] = None,
-            description: Optional[Union[str, Any]] = None,
-            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
-            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
-            currency: Optional[Union[Currency, Any]] = None,
-            invoice_number: Optional[Union[int, Any]] = None,
-            split_code: Optional[Union[str, Any]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a payment request for a transaction
-
-        :param: customer: Customer ID of the customer
-        :param: amount: Amount of the payment request
-        :param: due_date: Due date of the payment request
-        :param: description: Description of the payment request
-        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
-        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
-        :param: currency: Currency of the payment request
-        :param: send_notification: Set true if you want to send a notification to the customer email
-        :param: draft: Set true if you want to create a draft payment request
-        :param: has_invoice: Set true if you want to create a draft payment request
-        :param: invoice_number: Invoice number of the payment request
-        :param: split_code: split code of the transaction split
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert date and bool to string
-        due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        has_invoice = self._convert_to_string(has_invoice)
-        send_notification = self._convert_to_string(send_notification)
-
-        data = {
-            "customer": customer,
-            "amount": amount,
-            "due_date": due_date,
-            "description": description,
-            "line_items": line_items,
-            "tax": tax,
-            "currency": currency,
-            "send_notification": send_notification,
-            "draft": draft,
-            "has_invoice": has_invoice,
-            "invoice_number": invoice_number,
-            "split_code": split_code,
-        }
-        return await self._post_request("/paymentrequest", data=data)
-
-    async def list_payment_requests(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[str, None]] = None,
-            status: Optional[Union[PayMentRequestStatus, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            include_archive: Optional[Union[bool, None]] = True,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the payment requests
-
-        :param: per_page: Number of records to return
-        :param: page:  number to return
-        :param: customer: Filter by customer ID
-        :param: status: Filter by payment request status
-        :param: currency:
-        :param: include_archive: Show archived payment requests
-        :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
-        :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-        include_archive = self._convert_to_string(include_archive)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "status": status,
-            "currency": currency,
-            "include_archive": include_archive,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/paymentrequest", params=params)
-
-    async def fetch_payment_request(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a payment request on your integration
-
-        :param: id_or_code: ID or Code of the payment request
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/paymentrequest/{id_or_code}")
-
-    async def verify_payment_request(self, code: str) -> PayStackResponse:
-        """
-        Verify details of a payment request on your integration
-
-        :param: code: Payment request code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/paymentrequest/verify/{code}")
-
-    async def send_notification(self, code: str) -> PayStackResponse:
-        """
-        Send notification of a payment request to a customer
-
-        :param: code: Payment request code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._post_request(f"/paymentrequest/notify/{code}")
-
-    async def payment_request_total(self) -> PayStackResponse:
-        """
-        Get total of a payment request metric
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request("/paymentrequest/totals")
-
-    async def finalize_payment_request(self, code: str, send_notification: bool) -> PayStackResponse:
-        """
-        Finalize a draft payment request
-
-        :param: code: Payment request code
-        :param: send_notification: Set true if you want to send a notification to the customer email
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        send_notification = self._convert_to_string(send_notification)
-
-        data = {"send_notification": send_notification}
-        return await self._post_request(f"/paymentrequest/finalize/{code}", data=data)
-
-    async def update_payment_request(
-            self,
-            id_or_code: str,
-            customer: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            description: Optional[Union[str, None]] = None,
-            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
-            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            due_date: Optional[Union[date, None]] = None,
-            send_notification: Optional[Union[bool, None]] = True,
-            draft: Optional[Union[bool, None]] = True,
-            invoice_number: Optional[Union[int, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a payment request
-
-        :param: id_or_code: ID or Code of the payment request
-        :param: customer: Customer ID or code of the customer
-        :param: amount: Amount of the payment request
-        :param: due_date: Due date of the payment request
-        :param: description: Description of the payment request
-        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
-        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
-        :param: currency: Currency of the payment request
-        :param: send_notification: Set true if you want to send a notification to the customer email
-        :param: draft: Set true if you want to create a draft payment request
-        :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
-        :param: split_code: split code of the transaction split
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date and bool to string
-        due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        send_notification = self._convert_to_string(send_notification)
-
-        data = {
-            "customer": customer,
-            "amount": amount,
-            "due_date": due_date,
-            "description": description,
-            "line_items": line_items,
-            "tax": tax,
-            "currency": currency,
-            "send_notification": send_notification,
-            "draft": draft,
-            "invoice_number": invoice_number,
-            "split_code": split_code,
-        }
-        return await self._put_request(f"/paymentrequest/{id_or_code}", data=data)
-
-    async def archive_payment_request(self, code: str) -> PayStackResponse:
-        """
-        Archive a payment request
-
-        :param: code: Payment request code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._post_request(f"/paymentrequest/archive/{code}")
+"""
+Wrapper for Asynchronous Paystack Payment Requests API.
+
+The Payment Requests API allows you manage requests for payment of goods and services.
+"""
+
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import PayMentRequestStatus, Currency
+
+
+class AsyncPaymentRequestClientAPI(AsyncRequestAPI):
+    """
+    Paystack Payment Request API
+    Reference: https://paystack.com/docs/api/payment-request/
+    """
+
+    async def create_payment_request(
+            self,
+            customer: str,
+            amount: int,
+            draft: bool,
+            has_invoice: bool,
+            send_notification: bool,
+            due_date: Optional[Union[date, None]] = None,
+            description: Optional[Union[str, Any]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, Any]] = None,
+            invoice_number: Optional[Union[int, Any]] = None,
+            split_code: Optional[Union[str, Any]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a payment request for a transaction
+
+        :param: customer: Customer ID of the customer
+        :param: amount: Amount of the payment request
+        :param: due_date: Due date of the payment request
+        :param: description: Description of the payment request
+        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
+        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
+        :param: currency: Currency of the payment request
+        :param: send_notification: Set true if you want to send a notification to the customer email
+        :param: draft: Set true if you want to create a draft payment request
+        :param: has_invoice: Set true if you want to create a draft payment request
+        :param: invoice_number: Invoice number of the payment request
+        :param: split_code: split code of the transaction split
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert date and bool to string
+        due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        has_invoice = self._convert_to_string(has_invoice)
+        send_notification = self._convert_to_string(send_notification)
+
+        data = {
+            "customer": customer,
+            "amount": amount,
+            "due_date": due_date,
+            "description": description,
+            "line_items": line_items,
+            "tax": tax,
+            "currency": currency,
+            "send_notification": send_notification,
+            "draft": draft,
+            "has_invoice": has_invoice,
+            "invoice_number": invoice_number,
+            "split_code": split_code,
+        }
+        return await self._post_request("/paymentrequest", data=data)
+
+    async def list_payment_requests(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[str, None]] = None,
+            status: Optional[Union[PayMentRequestStatus, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            include_archive: Optional[Union[bool, None]] = True,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the payment requests
+
+        :param: per_page: Number of records to return
+        :param: page:  number to return
+        :param: customer: Filter by customer ID
+        :param: status: Filter by payment request status
+        :param: currency:
+        :param: include_archive: Show archived payment requests
+        :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
+        :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+        include_archive = self._convert_to_string(include_archive)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "status": status,
+            "currency": currency,
+            "include_archive": include_archive,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/paymentrequest", params=params)
+
+    async def fetch_payment_request(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a payment request on your integration
+
+        :param: id_or_code: ID or Code of the payment request
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/paymentrequest/{id_or_code}")
+
+    async def verify_payment_request(self, code: str) -> PayStackResponse:
+        """
+        Verify details of a payment request on your integration
+
+        :param: code: Payment request code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/paymentrequest/verify/{code}")
+
+    async def send_notification(self, code: str) -> PayStackResponse:
+        """
+        Send notification of a payment request to a customer
+
+        :param: code: Payment request code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._post_request(f"/paymentrequest/notify/{code}")
+
+    async def payment_request_total(self) -> PayStackResponse:
+        """
+        Get total of a payment request metric
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request("/paymentrequest/totals")
+
+    async def finalize_payment_request(self, code: str, send_notification: bool) -> PayStackResponse:
+        """
+        Finalize a draft payment request
+
+        :param: code: Payment request code
+        :param: send_notification: Set true if you want to send a notification to the customer email
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        send_notification = self._convert_to_string(send_notification)
+
+        data = {"send_notification": send_notification}
+        return await self._post_request(f"/paymentrequest/finalize/{code}", data=data)
+
+    async def update_payment_request(
+            self,
+            id_or_code: str,
+            customer: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            due_date: Optional[Union[date, None]] = None,
+            send_notification: Optional[Union[bool, None]] = True,
+            draft: Optional[Union[bool, None]] = True,
+            invoice_number: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a payment request
+
+        :param: id_or_code: ID or Code of the payment request
+        :param: customer: Customer ID or code of the customer
+        :param: amount: Amount of the payment request
+        :param: due_date: Due date of the payment request
+        :param: description: Description of the payment request
+        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
+        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
+        :param: currency: Currency of the payment request
+        :param: send_notification: Set true if you want to send a notification to the customer email
+        :param: draft: Set true if you want to create a draft payment request
+        :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
+        :param: split_code: split code of the transaction split
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date and bool to string
+        due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        send_notification = self._convert_to_string(send_notification)
+
+        data = {
+            "customer": customer,
+            "amount": amount,
+            "due_date": due_date,
+            "description": description,
+            "line_items": line_items,
+            "tax": tax,
+            "currency": currency,
+            "send_notification": send_notification,
+            "draft": draft,
+            "invoice_number": invoice_number,
+            "split_code": split_code,
+        }
+        return await self._put_request(f"/paymentrequest/{id_or_code}", data=data)
+
+    async def archive_payment_request(self, code: str) -> PayStackResponse:
+        """
+        Archive a payment request
+
+        :param: code: Payment request code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._post_request(f"/paymentrequest/archive/{code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/aplans.py` & `paystackease-2.0.4/paystackease/apis/async_apis/aplans.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""
-Wrapper for Asynchronous Paystack Plans API
-
-The Plans API allows you to create and manage installment payment options on your integration.
-"""
-
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import Interval
-
-
-class AsyncPlanClientAPI(AsyncRequestAPI):
-    """
-    Paystack Plan API
-    Reference: https://paystack.com/docs/api/plan/
-    """
-
-    async def create_plan(
-            self,
-            name: str,
-            amount: int,
-            interval: Interval,
-            currency: str,
-            invoice_limit: int,
-            send_invoices: bool,
-            send_sms: bool,
-            description: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a plan
-
-        :param: name: Name of the plan
-        :param: amount: Amount of the plan
-        :param: interval: Interval of the plan. Values [Interval.value.value]
-        :param: description: Description of the plan
-        :param: send_invoices: Send invoices to customer
-        :param: send_sms: Send SMS to customer
-        :param: currency: Currency of the plan
-        :param: invoice_limit: Invoice limit of the plan
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
-        data = {
-            "name": name,
-            "amount": amount,
-            "interval": interval,
-            "description": description,
-            "send_invoices": send_invoices,
-            "send_sms": send_sms,
-            "currency": currency,
-            "invoice_limit": invoice_limit,
-        }
-        return await self._post_request("/plan", data=data)
-
-    async def list_plans(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            status: Optional[Union[str, None]] = None,
-            interval: Optional[Union[Interval, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the plans
-
-        :param: per_page: Number of records to return
-        :param: page:  number to return
-        :param: status: Filter list by plans with specified status
-        :param: interval: Filter list by plans with specified interval
-        :param: amount
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "status": status,
-            "interval": interval,
-            "amount": amount,
-        }
-        return await self._get_request("/plan", params=params)
-
-    async def fetch_plan(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a plan
-
-        :param: id_or_code: ID or Code of the plan
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/plan/{id_or_code}")
-
-    async def update_plan(
-            self,
-            id_or_code: str,
-            name: str,
-            amount: int,
-            interval: Interval,
-            send_invoices: bool,
-            send_sms: bool,
-            currency: str,
-            invoice_limit: int,
-            description: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a plan detail
-
-        :param: id_or_code: ID or Code of the plan
-        :param: name: Name of the plan
-        :param: amount: Amount of the plan
-        :param: interval: Interval of the plan. [Interval.value.value]
-        :param: description:
-        :param: send_invoices:
-        :param: send_sms:
-        :param: currency:
-        :param: invoice_limit:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
-        data = {
-            "name": name,
-            "amount": amount,
-            "interval": interval,
-            "description": description,
-            "send_invoices": send_invoices,
-            "send_sms": send_sms,
-            "currency": currency,
-            "invoice_limit": invoice_limit,
-        }
-        return await self._put_request(f"/plan/{id_or_code}", data=data)
+"""
+Wrapper for Asynchronous Paystack Plans API
+
+The Plans API allows you to create and manage installment payment options on your integration.
+"""
+
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Interval
+
+
+class AsyncPlanClientAPI(AsyncRequestAPI):
+    """
+    Paystack Plan API
+    Reference: https://paystack.com/docs/api/plan/
+    """
+
+    async def create_plan(
+            self,
+            name: str,
+            amount: int,
+            interval: Interval,
+            currency: str,
+            invoice_limit: int,
+            send_invoices: bool,
+            send_sms: bool,
+            description: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a plan
+
+        :param: name: Name of the plan
+        :param: amount: Amount of the plan
+        :param: interval: Interval of the plan. Values [Interval.value.value]
+        :param: description: Description of the plan
+        :param: send_invoices: Send invoices to customer
+        :param: send_sms: Send SMS to customer
+        :param: currency: Currency of the plan
+        :param: invoice_limit: Invoice limit of the plan
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        send_invoices = self._convert_to_string(send_invoices)
+        send_sms = self._convert_to_string(send_sms)
+
+        data = {
+            "name": name,
+            "amount": amount,
+            "interval": interval,
+            "description": description,
+            "send_invoices": send_invoices,
+            "send_sms": send_sms,
+            "currency": currency,
+            "invoice_limit": invoice_limit,
+        }
+        return await self._post_request("/plan", data=data)
+
+    async def list_plans(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            status: Optional[Union[str, None]] = None,
+            interval: Optional[Union[Interval, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the plans
+
+        :param: per_page: Number of records to return
+        :param: page:  number to return
+        :param: status: Filter list by plans with specified status
+        :param: interval: Filter list by plans with specified interval
+        :param: amount
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "status": status,
+            "interval": interval,
+            "amount": amount,
+        }
+        return await self._get_request("/plan", params=params)
+
+    async def fetch_plan(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a plan
+
+        :param: id_or_code: ID or Code of the plan
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/plan/{id_or_code}")
+
+    async def update_plan(
+            self,
+            id_or_code: str,
+            name: str,
+            amount: int,
+            interval: Interval,
+            send_invoices: bool,
+            send_sms: bool,
+            currency: str,
+            invoice_limit: int,
+            description: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a plan detail
+
+        :param: id_or_code: ID or Code of the plan
+        :param: name: Name of the plan
+        :param: amount: Amount of the plan
+        :param: interval: Interval of the plan. [Interval.value.value]
+        :param: description:
+        :param: send_invoices:
+        :param: send_sms:
+        :param: currency:
+        :param: invoice_limit:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        send_invoices = self._convert_to_string(send_invoices)
+        send_sms = self._convert_to_string(send_sms)
+
+        data = {
+            "name": name,
+            "amount": amount,
+            "interval": interval,
+            "description": description,
+            "send_invoices": send_invoices,
+            "send_sms": send_sms,
+            "currency": currency,
+            "invoice_limit": invoice_limit,
+        }
+        return await self._put_request(f"/plan/{id_or_code}", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/aproducts.py` & `paystackease-2.0.4/paystackease/apis/async_apis/aproducts.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-"""
-Wrapper for Asynchronous Paystack Products API
-
-The Products API allows you to create and manage inventories on your integration.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-
-
-class AsyncProductClientAPI(AsyncRequestAPI):
-    """
-    Paystack Product API
-    Reference: https://paystack.com/docs/api/product/
-    """
-
-    async def create_product(
-            self,
-            name: str,
-            description: str,
-            amount: int,
-            currency: str,
-            unlimited: Optional[Union[bool, None]] = True,
-            quantity: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a product
-
-        :param: name: Name of the product
-        :param: description: Description of the product
-        :param: amount: Price of the product
-        :param: currency: Currency of the product
-        :param: unlimited: Set true if the product has unlimited stock,
-        :param: quantity: Quantity of the product in stock Use if unlimited is false
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        unlimited = self._convert_to_string(unlimited)
-
-        data = {
-            "name": name,
-            "description": description,
-            "price": amount,
-            "currency": currency,
-            "unlimited": unlimited,
-            "quantity": quantity,
-        }
-        return await self._post_request("/product", data=data)
-
-    async def list_products(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the products
-
-        :param: per_page: Number of records to return
-        :param: page:  number to return
-        :param: from_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        :param: to_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to strings
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/product", params=params)
-
-    async def fetch_product(self, product_id: str) -> PayStackResponse:
-        """
-        Get details of a product
-
-        :param: product_id: ID or Code of the product
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/product/{product_id}")
-
-    async def update_product(
-            self,
-            product_id: str,
-            name: str,
-            description: str,
-            amount: int,
-            currency: str,
-            unlimited: Optional[Union[bool, None]] = True,
-            quantity: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a product detail
-
-        :param: product_id: ID or Code of the product
-        :param: name: Name of the product
-        :param: description: Description of the product
-        :param: amount: Price of the product
-        :param: currency: Currency of the product
-        :param: unlimited: Set true if the product has unlimited stock,
-        :param: quantity: Quantity of the product in stock Use if unlimited is false
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        unlimited = self._convert_to_string(unlimited)
-
-        data = {
-            "name": name,
-            "description": description,
-            "price": amount,
-            "currency": currency,
-            "unlimited": unlimited,
-            "quantity": quantity,
-        }
-        return await self._put_request(f"/product/{product_id}", data=data)
+"""
+Wrapper for Asynchronous Paystack Products API
+
+The Products API allows you to create and manage inventories on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+
+
+class AsyncProductClientAPI(AsyncRequestAPI):
+    """
+    Paystack Product API
+    Reference: https://paystack.com/docs/api/product/
+    """
+
+    async def create_product(
+            self,
+            name: str,
+            description: str,
+            amount: int,
+            currency: str,
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a product
+
+        :param: name: Name of the product
+        :param: description: Description of the product
+        :param: amount: Price of the product
+        :param: currency: Currency of the product
+        :param: unlimited: Set true if the product has unlimited stock,
+        :param: quantity: Quantity of the product in stock Use if unlimited is false
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        unlimited = self._convert_to_string(unlimited)
+
+        data = {
+            "name": name,
+            "description": description,
+            "price": amount,
+            "currency": currency,
+            "unlimited": unlimited,
+            "quantity": quantity,
+        }
+        return await self._post_request("/product", data=data)
+
+    async def list_products(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the products
+
+        :param: per_page: Number of records to return
+        :param: page:  number to return
+        :param: from_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+        :param: to_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to strings
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return await self._get_request("/product", params=params)
+
+    async def fetch_product(self, product_id: str) -> PayStackResponse:
+        """
+        Get details of a product
+
+        :param: product_id: ID or Code of the product
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/product/{product_id}")
+
+    async def update_product(
+            self,
+            product_id: str,
+            name: str,
+            description: str,
+            amount: int,
+            currency: str,
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a product detail
+
+        :param: product_id: ID or Code of the product
+        :param: name: Name of the product
+        :param: description: Description of the product
+        :param: amount: Price of the product
+        :param: currency: Currency of the product
+        :param: unlimited: Set true if the product has unlimited stock,
+        :param: quantity: Quantity of the product in stock Use if unlimited is false
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        unlimited = self._convert_to_string(unlimited)
+
+        data = {
+            "name": name,
+            "description": description,
+            "price": amount,
+            "currency": currency,
+            "unlimited": unlimited,
+            "quantity": quantity,
+        }
+        return await self._put_request(f"/product/{product_id}", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/arefund.py` & `paystackease-2.0.4/paystackease/apis/async_apis/arefund.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""
-Wrapper for Asynchronous Paystack Refund API
-
-The Refunds API allows you to create and manage transaction refunds.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import Currency
-
-
-class AsyncRefundClientAPI(AsyncRequestAPI):
-    """
-    Paystack Refund API
-    Reference: https://paystack.com/docs/api/refund/
-    """
-
-    async def create_refund(
-            self,
-            transaction_ref_or_id: str,
-            amount: Optional[Union[int, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            customer_note: Optional[Union[str, None]] = None,
-            merchant_note: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a refund
-
-        :param: transaction_ref_or_id: The transaction id or reference to fetch
-        :param: amount: The amount to refund
-        :param: currency: The currency to refund { Currency.value.value }
-        :param: customer_note: The customer note or reason
-        :param: merchant_note: The merchant note or reason
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "transaction": transaction_ref_or_id,
-            "amount": amount,
-            "currency": currency,
-            "customer_note": customer_note,
-            "merchant_note": merchant_note,
-        }
-        return await self._post_request("/refund", data=data)
-
-    async def list_refunds(
-            self,
-            reference: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List refunds
-
-        :param: reference: The transaction reference to fetch for the refund
-        :param: currency: The currency to refund
-        :param: per_page
-        :param: page
-        :param: from_date: A timestamp at which to stop listing refund
-        :param: to_date: A timestamp at which to stop listing refund
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-
-        note::
-
-            Date time format: 2016-09-21
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "reference": reference,
-            "currency": currency,
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/refund", params=params)
-
-    async def fetch_refund(self, reference: str) -> PayStackResponse:
-        """
-        Fetch a refund
-
-        :param: reference: The transaction reference to fetch for the refund
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/refund/{reference}")
+"""
+Wrapper for Asynchronous Paystack Refund API
+
+The Refunds API allows you to create and manage transaction refunds.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
+
+
+class AsyncRefundClientAPI(AsyncRequestAPI):
+    """
+    Paystack Refund API
+    Reference: https://paystack.com/docs/api/refund/
+    """
+
+    async def create_refund(
+            self,
+            transaction_ref_or_id: str,
+            amount: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            customer_note: Optional[Union[str, None]] = None,
+            merchant_note: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a refund
+
+        :param: transaction_ref_or_id: The transaction id or reference to fetch
+        :param: amount: The amount to refund
+        :param: currency: The currency to refund { Currency.value.value }
+        :param: customer_note: The customer note or reason
+        :param: merchant_note: The merchant note or reason
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "transaction": transaction_ref_or_id,
+            "amount": amount,
+            "currency": currency,
+            "customer_note": customer_note,
+            "merchant_note": merchant_note,
+        }
+        return await self._post_request("/refund", data=data)
+
+    async def list_refunds(
+            self,
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List refunds
+
+        :param: reference: The transaction reference to fetch for the refund
+        :param: currency: The currency to refund
+        :param: per_page
+        :param: page
+        :param: from_date: A timestamp at which to stop listing refund
+        :param: to_date: A timestamp at which to stop listing refund
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+
+        note::
+
+            Date time format: 2016-09-21
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "reference": reference,
+            "currency": currency,
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/refund", params=params)
+
+    async def fetch_refund(self, reference: str) -> PayStackResponse:
+        """
+        Fetch a refund
+
+        :param: reference: The transaction reference to fetch for the refund
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/refund/{reference}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/asettlements.py` & `paystackease-2.0.4/paystackease/apis/async_apis/asettlements.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-"""
-Wrapper for Asynchronous Paystack Settlements API
-
-The Settlements API allows you to gain insights into payouts made by Paystack to your bank account.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import STATUS
-
-
-class AsyncSettlementClientAPI(AsyncRequestAPI):
-    """
-    Paystack Settlement API
-    Reference: https://paystack.com/docs/api/settlement/
-    """
-
-    async def list_settlements(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            status: Optional[Union[STATUS, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List settlements made to your settlement accounts
-
-        :param: per_page: The number of records to return per page.
-        :param: page: the number to retrieve.
-        :param: status: Value can be one of success, processing, pending or failed.
-        :param: subaccount:
-        :param: from_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        :param: to_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "status": status,
-            "subaccount": subaccount,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/settlement", params=params)
-
-    async def list_settlement_transactions(
-            self,
-            settlement_id: int,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Get the transactions that make up a particular settlement
-
-        :param: settlement_id: The id of the settlement.
-        :param: per_page: The number of records to return per page.
-        :param: page: the number to retrieve.
-        :param: from_date: A timestamp from which to start listing settlements
-        :param: to_date: A timestamp from which to start listing settlements
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-
-        note::
-
-            Date and time format: 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request(
-            f"/settlement/{settlement_id}/transactions", params=params
-        )
+"""
+Wrapper for Asynchronous Paystack Settlements API
+
+The Settlements API allows you to gain insights into payouts made by Paystack to your bank account.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import STATUS
+
+
+class AsyncSettlementClientAPI(AsyncRequestAPI):
+    """
+    Paystack Settlement API
+    Reference: https://paystack.com/docs/api/settlement/
+    """
+
+    async def list_settlements(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            status: Optional[Union[STATUS, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List settlements made to your settlement accounts
+
+        :param: per_page: The number of records to return per page.
+        :param: page: the number to retrieve.
+        :param: status: Value can be one of success, processing, pending or failed.
+        :param: subaccount:
+        :param: from_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+        :param: to_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "status": status,
+            "subaccount": subaccount,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/settlement", params=params)
+
+    async def list_settlement_transactions(
+            self,
+            settlement_id: int,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Get the transactions that make up a particular settlement
+
+        :param: settlement_id: The id of the settlement.
+        :param: per_page: The number of records to return per page.
+        :param: page: the number to retrieve.
+        :param: from_date: A timestamp from which to start listing settlements
+        :param: to_date: A timestamp from which to start listing settlements
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+
+        note::
+
+            Date and time format: 2016-09-24T00:00:05.000Z, 2016-09-21
+
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return await self._get_request(
+            f"/settlement/{settlement_id}/transactions", params=params
+        )
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/asubaccounts.py` & `paystackease-2.0.4/paystackease/apis/async_apis/asubaccounts.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-"""
-Wrapper for Asynchronous Paystack SubAccounts API
-
-The Subaccounts API allows you to create and manage subaccounts on your integration.
-Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
-"""
-
-from datetime import date
-from typing import Optional, Dict, List, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import SettlementSchedule
-
-
-class AsyncSubAccountClientAPI(AsyncRequestAPI):
-    """
-    Paystack SubAccount API
-    Reference: https://paystack.com/docs/api/subaccount/
-    """
-
-    async def create_subaccount(
-            self,
-            business_name: str,
-            settlement_bank: str,
-            account_number: str,
-            percentage_charge: float,
-            description: str,
-            primary_contact_email: Optional[Union[str, None]] = None,
-            primary_contact_name: Optional[Union[str, None]] = None,
-            primary_contact_phone: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a subaccount
-
-        :param: business_name: The business name of the subaccount.
-        :param: settlement_bank: Bank Code for the bank
-        :param: account_number: The account number of the subaccount.
-        :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
-        :param: description: The description of the subaccount.
-        :param: primary_contact_email: A contact email for the subaccount
-        :param: primary_contact_name: A name for the contact person for this subaccount
-        :param: primary_contact_phone: A phone number to call for this subaccount
-        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "business_name": business_name,
-            "settlement_bank": settlement_bank,
-            "account_number": account_number,
-            "percentage_charge": percentage_charge,
-            "description": description,
-            "primary_contact_email": primary_contact_email,
-            "primary_contact_name": primary_contact_name,
-            "primary_contact_phone": primary_contact_phone,
-            "metadata": metadata,
-        }
-        return await self._post_request("/subaccount", data=data)
-
-    async def update_subaccount(
-            self,
-            id_or_code: str,
-            business_name: str,
-            settlement_bank: str,
-            account_number: str,
-            active: Optional[Union[bool, None]] = True,
-            percentage_charge: Optional[Union[float, None]] = None,
-            description: Optional[Union[str, None]] = None,
-            primary_contact_email: Optional[Union[str, None]] = None,
-            primary_contact_name: Optional[Union[str, None]] = None,
-            primary_contact_phone: Optional[Union[str, None]] = None,
-            settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a subaccount
-
-        :param: id_or_code: The id or code of the subaccount.
-        :param: business_name: The business name of the subaccount.
-        :param: settlement_bank: The settlement bank of the subaccount.
-        :param: account_number
-        :param: active: [ True or False ]
-        :param: percentage_charge
-        :param: description
-        :param: primary_contact_email
-        :param: primary_contact_name
-        :param: primary_contact_phone
-        :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
-
-        note::
-            Auto means payout is T+1
-            Manual means payout to the subaccount should only be made when requested. async defaults to auto
-
-        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "business_name": business_name,
-            "settlement_bank": settlement_bank,
-            "account_number": account_number,
-            "active": active,
-            "percentage_charge": percentage_charge,
-            "description": description,
-            "primary_contact_email": primary_contact_email,
-            "primary_contact_name": primary_contact_name,
-            "primary_contact_phone": primary_contact_phone,
-            "settlement_schedule": settlement_schedule,
-            "metadata": metadata,
-        }
-        return await self._put_request(f"/subaccount/{id_or_code}", data=data)
-
-    async def list_subaccounts(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all subaccounts
-
-        :param: per_page: The number of records to return per page.
-        :param: page: The number to retrieve.
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/subaccount", params=params)
-
-    async def fetch_subaccount(self, id_or_code: str) -> PayStackResponse:
-        """
-        Fetch details of a specific subaccount
-
-        :param: id_or_code: The id or code of the subaccount.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/subaccount/{id_or_code}")
+"""
+Wrapper for Asynchronous Paystack SubAccounts API
+
+The Subaccounts API allows you to create and manage subaccounts on your integration.
+Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
+"""
+
+from datetime import date
+from typing import Optional, Dict, List, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import SettlementSchedule
+
+
+class AsyncSubAccountClientAPI(AsyncRequestAPI):
+    """
+    Paystack SubAccount API
+    Reference: https://paystack.com/docs/api/subaccount/
+    """
+
+    async def create_subaccount(
+            self,
+            business_name: str,
+            settlement_bank: str,
+            account_number: str,
+            percentage_charge: float,
+            description: str,
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a subaccount
+
+        :param: business_name: The business name of the subaccount.
+        :param: settlement_bank: Bank Code for the bank
+        :param: account_number: The account number of the subaccount.
+        :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
+        :param: description: The description of the subaccount.
+        :param: primary_contact_email: A contact email for the subaccount
+        :param: primary_contact_name: A name for the contact person for this subaccount
+        :param: primary_contact_phone: A phone number to call for this subaccount
+        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "business_name": business_name,
+            "settlement_bank": settlement_bank,
+            "account_number": account_number,
+            "percentage_charge": percentage_charge,
+            "description": description,
+            "primary_contact_email": primary_contact_email,
+            "primary_contact_name": primary_contact_name,
+            "primary_contact_phone": primary_contact_phone,
+            "metadata": metadata,
+        }
+        return await self._post_request("/subaccount", data=data)
+
+    async def update_subaccount(
+            self,
+            id_or_code: str,
+            business_name: str,
+            settlement_bank: str,
+            account_number: str,
+            active: Optional[Union[bool, None]] = True,
+            percentage_charge: Optional[Union[float, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a subaccount
+
+        :param: id_or_code: The id or code of the subaccount.
+        :param: business_name: The business name of the subaccount.
+        :param: settlement_bank: The settlement bank of the subaccount.
+        :param: account_number
+        :param: active: [ True or False ]
+        :param: percentage_charge
+        :param: description
+        :param: primary_contact_email
+        :param: primary_contact_name
+        :param: primary_contact_phone
+        :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
+
+        note::
+            Auto means payout is T+1
+            Manual means payout to the subaccount should only be made when requested. async defaults to auto
+
+        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        active = self._convert_to_string(active)
+
+        data = {
+            "business_name": business_name,
+            "settlement_bank": settlement_bank,
+            "account_number": account_number,
+            "active": active,
+            "percentage_charge": percentage_charge,
+            "description": description,
+            "primary_contact_email": primary_contact_email,
+            "primary_contact_name": primary_contact_name,
+            "primary_contact_phone": primary_contact_phone,
+            "settlement_schedule": settlement_schedule,
+            "metadata": metadata,
+        }
+        return await self._put_request(f"/subaccount/{id_or_code}", data=data)
+
+    async def list_subaccounts(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all subaccounts
+
+        :param: per_page: The number of records to return per page.
+        :param: page: The number to retrieve.
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return await self._get_request("/subaccount", params=params)
+
+    async def fetch_subaccount(self, id_or_code: str) -> PayStackResponse:
+        """
+        Fetch details of a specific subaccount
+
+        :param: id_or_code: The id or code of the subaccount.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/subaccount/{id_or_code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/asubscriptions.py` & `paystackease-2.0.4/paystackease/apis/async_apis/asubscriptions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""
-Wrapper for Paystack Subscriptions API
-
-The Subscriptions API allows you to create and manage recurring payment on your integration.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-
-
-class AsyncSubscriptionClientAPI(AsyncRequestAPI):
-    """
-    Paystack Subscription API
-    Reference: https://paystack.com/docs/api/subscription/
-    """
-
-    async def create_subscription(
-            self,
-            customer: str,
-            plan_code: str,
-            authorization: str,
-            start_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a subscription
-
-        :param: customer: Email or Code of the customer
-        :param: plan_code: Code of the plan
-        :param: authorization: Code of the authorization
-        :param: start_date: Start date of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        start_date = self._convert_to_string(start_date)
-
-        data = {
-            "customer": customer,
-            "plan": plan_code,
-            "authorization": authorization,
-            "start_date": start_date,
-        }
-        return await self._post_request("/subscription", data=data)
-
-    async def list_subscriptions(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[int, None]] = None,
-            plan_code: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the subscriptions
-
-        :param: per_page: Number of records to return per page.
-        :param: page: THe number to return
-        :param: customer:
-        :param: plan_code:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "plan": plan_code,
-        }
-        return await self._get_request("/subscription", params=params)
-
-    async def fetch_subscription(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a subscription
-
-        :param: id_or_code: ID or Code of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/subscription/{id_or_code}")
-
-    async def enable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
-        """
-        Enable a subscription
-
-        :param: subscription_code: Code of the subscription
-        :param: token: Email token of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"code": subscription_code, "token": token}
-        return await self._post_request("/subscription/enable", data=data)
-
-    async def disable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
-        """
-        Disable a subscription
-
-        :param: subscription_code: Code of the subscription
-        :param: token: Email token of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"code": subscription_code, "token": token}
-        return await self._post_request("/subscription/disable", data=data)
-
-    async def generate_update_subscription(self, subscription_code: str) -> PayStackResponse:
-        """
-        Generate a link for updating the card on subscription
-
-        :param: subscription_code: Code of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._post_request(f"/subscription/{subscription_code}/manage/link")
-
-    async def send_update_subscription_link(self, subscription_code: str) -> PayStackResponse:
-        """
-        Email a customer a link for updating the card on their subscription
-
-        :param: subscription_code: Code of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._post_request(f"/subscription/{subscription_code}/manage/email")
+"""
+Wrapper for Paystack Subscriptions API
+
+The Subscriptions API allows you to create and manage recurring payment on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+
+
+class AsyncSubscriptionClientAPI(AsyncRequestAPI):
+    """
+    Paystack Subscription API
+    Reference: https://paystack.com/docs/api/subscription/
+    """
+
+    async def create_subscription(
+            self,
+            customer: str,
+            plan_code: str,
+            authorization: str,
+            start_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a subscription
+
+        :param: customer: Email or Code of the customer
+        :param: plan_code: Code of the plan
+        :param: authorization: Code of the authorization
+        :param: start_date: Start date of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        start_date = self._convert_to_string(start_date)
+
+        data = {
+            "customer": customer,
+            "plan": plan_code,
+            "authorization": authorization,
+            "start_date": start_date,
+        }
+        return await self._post_request("/subscription", data=data)
+
+    async def list_subscriptions(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            plan_code: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the subscriptions
+
+        :param: per_page: Number of records to return per page.
+        :param: page: THe number to return
+        :param: customer:
+        :param: plan_code:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "plan": plan_code,
+        }
+        return await self._get_request("/subscription", params=params)
+
+    async def fetch_subscription(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a subscription
+
+        :param: id_or_code: ID or Code of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/subscription/{id_or_code}")
+
+    async def enable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
+        """
+        Enable a subscription
+
+        :param: subscription_code: Code of the subscription
+        :param: token: Email token of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"code": subscription_code, "token": token}
+        return await self._post_request("/subscription/enable", data=data)
+
+    async def disable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
+        """
+        Disable a subscription
+
+        :param: subscription_code: Code of the subscription
+        :param: token: Email token of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"code": subscription_code, "token": token}
+        return await self._post_request("/subscription/disable", data=data)
+
+    async def generate_update_subscription(self, subscription_code: str) -> PayStackResponse:
+        """
+        Generate a link for updating the card on subscription
+
+        :param: subscription_code: Code of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._post_request(f"/subscription/{subscription_code}/manage/link")
+
+    async def send_update_subscription_link(self, subscription_code: str) -> PayStackResponse:
+        """
+        Email a customer a link for updating the card on their subscription
+
+        :param: subscription_code: Code of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._post_request(f"/subscription/{subscription_code}/manage/email")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/atransaction_splits.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/transaction_splits.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,166 @@
-"""
-Wrapper for Asynchronous Paystack Transaction Splits APIs
-
-The Transaction Splits API enables merchants split the settlement for a transaction
-across their payout account, and one or more subaccounts.
-"""
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import Currency
-
-
-class AsyncTransactionSplitClientAPI(AsyncRequestAPI):
-    """
-    Paystack Transaction Split API
-    Reference: https://paystack.com/docs/api/split/
-    """
-
-    async def create_split(
-            self,
-            transaction_split_name: str,
-            transaction_split_type: str,
-            currency: Currency,
-            subaccounts: List[Dict[str, Any]],
-            bearer_type: str,
-            bearer_subaccount: str,
-    ) -> PayStackResponse:
-        """
-        Create a split payment on your integration
-
-        :param: transaction_split_name: Name of the transaction split
-        :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
-        :param: currency: [ Currency.value.value ]
-        :param: subaccounts: A list of object containing subaccount code and number of shares
-                            [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
-        :param: bearer_type: Any of subaccount | account | all-proportional | all
-        :param: bearer_subaccount: Subaccount code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "name": transaction_split_name,
-            "type": transaction_split_type,
-            "currency": currency,
-            "subaccounts": subaccounts,
-            "bearer_type": bearer_type,
-            "bearer_subaccount": bearer_subaccount,
-        }
-        return await self._post_request("/split", data=data)
-
-    async def add_or_update_subaccount_split(
-            self, split_id: str, subaccount: str, transaction_share: int
-    ) -> PayStackResponse:
-        """
-        Add a Subaccount to a Transaction Split, or update the share of
-        an existing Subaccount in a Transaction Split
-
-        :param: split_id: The split ID
-        :param: subaccount: The subaccount code
-        :param: transaction_share: The number of shares
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"subaccount": subaccount, "share": transaction_share}
-        return await self._post_request(f"/split/{split_id}/subaccount/add", data=data)
-
-    async def remove_sub_account_split(self, split_id: str, subaccount: str) -> PayStackResponse:
-        """
-        Remove a Sub Account from a transaction split
-
-        :param: split_id: The split ID
-        :param: subaccount: The subaccount code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"subaccount": subaccount}
-        return await self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
-
-    async def update_split(
-            self,
-            split_id: str,
-            transaction_split_name: str,
-            active: bool,
-            bearer_type: Optional[Union[str, None]] = None,
-            bearer_subaccount: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a specific transaction split details
-
-        :param: split_id: The split ID
-        :param: transaction_split_name: Name of the transaction split
-        :param: active: True or False
-        :param: bearer_type:
-        :param: bearer_subaccount:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "name": transaction_split_name,
-            "active": active,
-            "bearer_type": bearer_type,
-            "bearer_subaccount": bearer_subaccount,
-        }
-        return await self._put_request(f"/split/{split_id}", data=data)
-
-    async def list_split(
-            self,
-            split_name: Optional[Union[str, None]] = None,
-            active: Optional[Union[bool, None]] = True,
-            sort_by: Optional[Union[str, None]] = None,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the transaction splits
-
-        :param: split_name: Name of the transaction split
-        :param: active: True or False
-        :param: sort_by: Sort by name, async defaults to createdAt date,
-        :param: per_page:
-        :param: page:
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date and bool to string
-        active = self._convert_to_string(active)
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "name": split_name,
-            "active": active,
-            "sort_by": sort_by,
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/split", params=params)
-
-    async def fetch_split(self, split_id: str) -> PayStackResponse:
-        """
-        Fetch details of a specific transaction split
-
-        :param: split_id: The split ID
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/split/{split_id}")
+"""
+Wrapper for Paystack Transaction Splits APIs
+
+The Transaction Splits API enables merchants split the settlement for a transaction
+across their payout account, and one or more subaccounts.
+"""
+
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
+
+
+class TransactionSplitClientAPI(SyncRequestAPI):
+    """
+    Paystack Transaction Split API
+    Reference: https://paystack.com/docs/api/split/
+    """
+
+    def create_split(
+            self,
+            transaction_split_name: str,
+            transaction_split_type: str,
+            currency: Currency,
+            subaccounts: List[Dict[str, Any]],
+            bearer_type: str,
+            bearer_subaccount: str,
+    ) -> PayStackResponse:
+        """
+        Create a split payment on your integration
+
+        :param: transaction_split_name: Name of the transaction split
+        :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
+        :param: currency: [ Currency.value.value ]
+        :param: subaccounts: A list of object containing subaccount code and number of shares
+                            [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
+        :param: bearer_type: Any of subaccount | account | all-proportional | all
+        :param: bearer_subaccount: Subaccount code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "name": transaction_split_name,
+            "type": transaction_split_type,
+            "currency": currency,
+            "subaccounts": subaccounts,
+            "bearer_type": bearer_type,
+            "bearer_subaccount": bearer_subaccount,
+        }
+        return self._post_request("/split", data=data)
+
+    def add_or_update_subaccount_split(
+            self, split_id: str, subaccount: str, transaction_share: int
+    ) -> PayStackResponse:
+        """
+        Add a Subaccount to a Transaction Split, or update the share of
+        an existing Subaccount in a Transaction Split
+
+        :param: split_id: The split ID
+        :param: subaccount: The subaccount code
+        :param: transaction_share: The number of shares
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"subaccount": subaccount, "share": transaction_share}
+        return self._post_request(f"/split/{split_id}/subaccount/add", data=data)
+
+    def remove_sub_account_split(self, split_id: str, subaccount: str) -> PayStackResponse:
+        """
+        Remove a Sub Account from a transaction split
+
+        :param: split_id: The split ID
+        :param: subaccount: The subaccount code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"subaccount": subaccount}
+        return self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
+
+    def update_split(
+            self,
+            split_id: str,
+            transaction_split_name: str,
+            active: bool,
+            bearer_type: Optional[Union[str, None]] = None,
+            bearer_subaccount: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a specific transaction split details
+
+        :param: split_id: The split ID
+        :param: transaction_split_name: Name of the transaction split
+        :param: active: True or False
+        :param: bearer_type:
+        :param: bearer_subaccount:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        active = self._convert_to_string(active)
+
+        data = {
+            "name": transaction_split_name,
+            "active": active,
+            "bearer_type": bearer_type,
+            "bearer_subaccount": bearer_subaccount,
+        }
+        return self._put_request(f"/split/{split_id}", data=data)
+
+    def list_split(
+            self,
+            split_name: Optional[Union[str, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+            sort_by: Optional[Union[str, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the transaction splits
+
+        :param: split_name: Name of the transaction split
+        :param: active: True or False
+        :param: sort_by: Sort by name, defaults to createdAt date,
+        :param: per_page:
+        :param: page:
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date and bool to string
+        active = self._convert_to_string(active)
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "name": split_name,
+            "active": active,
+            "sort_by": sort_by,
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/split", params=params)
+
+    def fetch_split(self, split_id: str) -> PayStackResponse:
+        """
+        Fetch details of a specific transaction split
+
+        :param: split_id: The split ID
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/split/{split_id}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/atransactions.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,319 +1,319 @@
-"""
-Wrapper for Asynchronous Paystack Transactions API
-
-The Transactions API allows you to create and manage payments on your integration.
-"""
-
-from datetime import date
-from typing import List, Optional, Dict, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import TransactionStatus, Channels, Bearer, Currency
-
-
-class AsyncTransactionClientAPI(AsyncRequestAPI):
-    """
-    Paystack Transaction API
-    Reference: https://paystack.com/docs/api/transaction/
-    """
-
-    async def initialize(
-            self,
-            email: str,
-            amount: int,
-            currency: Optional[Union[Currency, None]] = Currency.NGN.value,
-            reference: Optional[Union[str, None]] = None,
-            callback_url: Optional[Union[str, None]] = None,
-            plan: Optional[Union[str, None]] = None,
-            invoice_limit: Optional[Union[int, None]] = None,
-            channels: Optional[Union[List[Channels], None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            transaction_charge: Optional[Union[int, None]] = None,
-            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Initialize a transaction
-
-        :param: email:
-        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
-                        Use convert_currency() to convert to subunit
-        :param: currency:  # Currency.value.value
-        :param: reference:
-        :param: callback_url: # Use this to override the callback url provided on the  dashboard
-                                # https://example.com/callback
-        :param: plan:  # If transaction is to create a subscription to a preasync defined plan, provide plan code here.
-        :param: invoice_limit:  # Number of times to charge customer during subscription to plan
-        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
-        :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
-        :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
-        :param: transaction_charge: # An amount used to override the split configuration for a
-                                    # single split payment
-        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
-        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "amount": amount,
-            "currency": currency,
-            "reference": reference,
-            "callback_url": callback_url,
-            "plan": plan,
-            "invoice_limit": invoice_limit,
-            "channels": channels,
-            "split_code": split_code,
-            "subaccount": subaccount,
-            "transaction_charge": transaction_charge,
-            "bearer": bearer,
-            "metadata": metadata,
-        }
-        return await self._post_request("/transaction/initialize", data=data)
-
-    async def charge_authorization(
-            self,
-            email: str,
-            amount: int,
-            authorization_code: str,
-            reference: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            channels: Optional[Union[List[Channels], None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            transaction_charge: Optional[int] = None,
-            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
-            queue: Optional[Union[bool, None]] = True,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Charge an authorization transaction
-
-        :param: email:
-        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
-                        Use convert_currency() to convert to subunit
-        :param: authorization_code:  # value = AUTH_1234234WRFW
-        :param: reference:
-        :param: currency:  # value = Currency.value.value
-        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
-        :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
-        :param: transaction_charge:
-        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
-        :param: queue:  # If set to true, the transaction will be queued for processing
-        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        queue = self._convert_to_string(queue)
-
-        data = {
-            "email": email,
-            "amount": amount,
-            "authorization_code": authorization_code,
-            "reference": reference,
-            "currency": currency,
-            "channels": channels,
-            "subaccount": subaccount,
-            "transaction_charge": transaction_charge,
-            "bearer": bearer,
-            "queue": queue,
-            "metadata": metadata,
-        }
-        return await self._post_request("/transaction/charge_authorization", data=data)
-
-    async def partial_debit(
-            self,
-            email: str,
-            authorization_code: str,
-            amount: int,
-            currency: str,
-            reference: Optional[Union[str, None]] = None,
-            at_least: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Charge a partial debit transaction
-
-        :param: email:
-        :param: authorization_code:  # value = AUTH_1234234WRFW
-        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
-                        Use convert_currency() to convert to subunit
-        :param: currency:  # value = Currency.value.value
-        :param: reference:  # Unique transaction reference.
-        :param: at_least:  # Minimum amount to charge
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "authorization_code": authorization_code,
-            "amount": amount,
-            "currency": currency,
-            "reference": reference,
-            "at_least": at_least,
-        }
-        return await self._post_request("/transaction/partial_debit", data=data)
-
-    async def list_transactions(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[int, None]] = None,
-            terminal_id: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            status: Optional[Union[TransactionStatus, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all transactions
-
-        :param: per_page:  # Specify how many records you want to retrieve per page.
-        :param: page:  # Specify a page number to retrieve
-        :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
-        :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
-        :param: amount:  # Specify an amount for the transactions you want to retrieve
-        :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
-        :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
-        :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "terminalid": terminal_id,
-            "amount": amount,
-            "status": status,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/transaction", params=params)
-
-    async def verify_transaction(self, reference: str) -> PayStackResponse:
-        """
-        Verify a transaction by reference
-
-        :param: reference:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/transaction/verify/{reference}")
-
-    async def fetch_transaction(self, transaction_id: int) -> PayStackResponse:
-        """
-        Fetch details of a specific transaction
-
-        :param: transaction_id:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/transaction/{transaction_id}")
-
-    async def transaction_timeline(self, id_or_reference: str) -> PayStackResponse:
-        """
-        Get the timeline of a transaction
-
-        :param: id_or_reference:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/transaction/timeline/{id_or_reference}")
-
-    async def transaction_totals(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Get totals of all transactions
-
-        :param: per_page:
-        :param: page:
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/transaction/totals", params=params)
-
-    async def export_transactions(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[int, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            status: Optional[Union[TransactionStatus, None]] = None,
-            settled: Optional[Union[bool, None]] = True,
-            settlement: Optional[Union[int, None]] = None,
-            payment_page: Optional[Union[int, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Export transactions
-
-        :param: per_page:
-        :param: page:
-        :param: customer:
-        :param: currency:  # value = Currency.value.value
-        :param: amount:
-        :param: status:
-        :param: settled:  # true or false
-        :param: settlement:
-        :param: payment_page:
-        :param: from_date:  # 2016-09-24T00:00:05.000Z
-        :param: to_date:  # 2016-09-24T00:00:05.000Z
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date and bool to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-        settled = self._convert_to_string(settled)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "currency": currency,
-            "amount": amount,
-            "status": status,
-            "settled": settled,
-            "settlement": settlement,
-            "payment_page": payment_page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/transaction/export", params=params)
+"""
+Wrapper for Paystack Transactions API
+
+The Transactions API allows you to create and manage payments on your integration.
+"""
+
+from datetime import date
+from typing import List, Optional, Dict, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Channels, Currency, Bearer, TransactionStatus
+
+
+class TransactionClientAPI(SyncRequestAPI):
+    """
+    Paystack Transaction API
+    Reference: https://paystack.com/docs/api/transaction/
+    """
+
+    def initialize(
+            self,
+            email: str,
+            amount: int,
+            currency: Optional[Union[Currency, None]] = Currency.NGN.value,
+            reference: Optional[Union[str, None]] = None,
+            callback_url: Optional[Union[str, None]] = None,
+            plan: Optional[Union[str, None]] = None,
+            invoice_limit: Optional[Union[int, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            transaction_charge: Optional[Union[int, None]] = None,
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Initialize a transaction
+
+        :param: email:
+        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
+                        Use convert_currency() to convert to subunit
+        :param: currency:  # Currency.value.value
+        :param: reference:
+        :param: callback_url: # Use this to override the callback url provided on the  dashboard
+                            # https://example.com/callback
+        :param: plan:  # If transaction is to create a subscription to a predefined plan, provide plan code here.
+        :param: invoice_limit:  # Number of times to charge customer during subscription to plan
+        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
+        :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
+        :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
+        :param: transaction_charge: # An amount used to override the split configuration for a
+                                    # single split payment
+        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
+        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "amount": amount,
+            "currency": currency,
+            "reference": reference,
+            "callback_url": callback_url,
+            "plan": plan,
+            "invoice_limit": invoice_limit,
+            "channels": channels,
+            "split_code": split_code,
+            "subaccount": subaccount,
+            "transaction_charge": transaction_charge,
+            "bearer": bearer,
+            "metadata": metadata,
+        }
+        return self._post_request("/transaction/initialize", data=data)
+
+    def charge_authorization(
+            self,
+            email: str,
+            amount: int,
+            authorization_code: str,
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            transaction_charge: Optional[int] = None,
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            queue: Optional[Union[bool, None]] = True,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Charge an authorization transaction
+
+        :param: email:
+        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
+                        Use convert_currency() to convert to subunit
+        :param: authorization_code:  # value = AUTH_1234234WRFW
+        :param: reference:
+        :param: currency:  # value = Currency.value.value
+        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
+        :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
+        :param: transaction_charge:
+        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
+        :param: queue:  # If set to true, the transaction will be queued for processing
+        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        queue = self._convert_to_string(queue)
+
+        data = {
+            "email": email,
+            "amount": amount,
+            "authorization_code": authorization_code,
+            "reference": reference,
+            "currency": currency,
+            "channels": channels,
+            "subaccount": subaccount,
+            "transaction_charge": transaction_charge,
+            "bearer": bearer,
+            "queue": queue,
+            "metadata": metadata,
+        }
+        return self._post_request("/transaction/charge_authorization", data=data)
+
+    def partial_debit(
+            self,
+            email: str,
+            authorization_code: str,
+            amount: int,
+            currency: str,
+            reference: Optional[Union[str, None]] = None,
+            at_least: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Charge a partial debit transaction
+
+        :param: email:
+        :param: authorization_code:  # value = AUTH_1234234WRFW
+        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
+                        Use convert_currency() to convert to subunit
+        :param: currency:  # value = Currency.value.value
+        :param: reference:  # Unique transaction reference.
+        :param: at_least:  # Minimum amount to charge
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "authorization_code": authorization_code,
+            "amount": amount,
+            "currency": currency,
+            "reference": reference,
+            "at_least": at_least,
+        }
+        return self._post_request("/transaction/partial_debit", data=data)
+
+    def list_transactions(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            terminal_id: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all transactions
+
+        :param: per_page:  # Specify how many records you want to retrieve per page.
+        :param: page:  # Specify a page number to retrieve
+        :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
+        :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
+        :param: amount:  # Specify an amount for the transactions you want to retrieve
+        :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
+        :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
+        :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "terminalid": terminal_id,
+            "amount": amount,
+            "status": status,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/transaction", params=params)
+
+    def verify_transaction(self, reference: str) -> PayStackResponse:
+        """
+        Verify a transaction by reference
+
+        :param: reference:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/transaction/verify/{reference}")
+
+    def fetch_transaction(self, transaction_id: int) -> PayStackResponse:
+        """
+        Fetch details of a specific transaction
+
+        :param: transaction_id:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/transaction/{transaction_id}")
+
+    def transaction_timeline(self, id_or_reference: str) -> PayStackResponse:
+        """
+        Get the timeline of a transaction
+
+        :param: id_or_reference:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/transaction/timeline/{id_or_reference}")
+
+    def transaction_totals(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Get totals of all transactions
+
+        :param: per_page:
+        :param: page:
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/transaction/totals", params=params)
+
+    def export_transactions(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            settled: Optional[Union[bool, None]] = True,
+            settlement: Optional[Union[int, None]] = None,
+            payment_page: Optional[Union[int, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Export transactions
+
+        :param: per_page:
+        :param: page:
+        :param: customer:
+        :param: currency:  # value = Currency.value.value
+        :param: amount:
+        :param: status:
+        :param: settled:  # true or false
+        :param: settlement:
+        :param: payment_page:
+        :param: from_date:  # 2016-09-24T00:00:05.000Z
+        :param: to_date:  # 2016-09-24T00:00:05.000Z
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date and bool to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+        settled = self._convert_to_string(settled)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "currency": currency,
+            "amount": amount,
+            "status": status,
+            "settled": settled,
+            "settlement": settlement,
+            "payment_page": payment_page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/transaction/export", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/atransfer_recipients.py` & `paystackease-2.0.4/paystackease/apis/async_apis/atransfer_recipients.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-"""
-Wrapper for Asynchronous Paystack Transfer Recipient APIs
-
-The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
-"""
-
-from datetime import date
-from typing import Optional, Dict, List, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import Currency
-
-
-class AsyncTransferRecipientsClientAPI(AsyncRequestAPI):
-    """
-    Paystack Transfer Recipients API
-    Reference: https://paystack.com/docs/api/transfer-recipient/
-    """
-
-    async def create_transfer_recipients(
-            self,
-            recipient_type: str,
-            recipient_name: str,
-            account_number: str,
-            bank_code: str,
-            description: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            authorization_code: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a transfer recipient
-
-        :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
-        :param: recipient_name: The name of the transfer recipient according to their account registration
-        :param: account_number: transfer recipient's account number.
-                                Required for all recipient types except authorization
-        :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
-        :param: description:
-        :param: currency: transfer recipient's currency. [Currency.value.value ]
-        :param: authorization_code: transfer recipient's authorization code from previous transaction
-        :param: metadata: transfer recipient's metadata
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "type": recipient_type,
-            "name": recipient_name,
-            "account_number": account_number,
-            "bank_code": bank_code,
-            "description": description,
-            "currency": currency,
-            "authorization_code": authorization_code,
-            "metadata": metadata,
-        }
-        return await self._post_request("/transferrecipient", data=data)
-
-    async def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> PayStackResponse:
-        """
-        Create multiple transfer recipients in batches.
-
-        :param: batch: A list of transfer recipient object
-                        keys [ { type, name, account_number, bank_code, currency etc. }]
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"batch": batch}
-        return await self._post_request("/transferrecipient/bulk", data=data)
-
-    async def list_transfer_recipients(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List transfer recipients
-
-        :param: per_page: The number of records to return per page.
-        :param: page: The page number to retrieve.
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to strings
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/transferrecipient", params=params)
-
-    async def fetch_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
-        """
-        Fetch details of a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/transferrecipient/{id_or_code}")
-
-    async def update_transfer_recipient(
-            self,
-            id_or_code: str,
-            recipient_name: str,
-            recipient_email: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-        :param: recipient_name: The name of the transfer recipient
-        :param: recipient_email: The email of the transfer recipient
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"name": recipient_name, "email": recipient_email}
-        return await self._put_request(f"/transferrecipient/{id_or_code}", data=data)
-
-    async def delete_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
-        """
-        Delete a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._delete_request(f"/transferrecipient/{id_or_code}")
+"""
+Wrapper for Asynchronous Paystack Transfer Recipient APIs
+
+The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
+"""
+
+from datetime import date
+from typing import Optional, Dict, List, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
+
+
+class AsyncTransferRecipientsClientAPI(AsyncRequestAPI):
+    """
+    Paystack Transfer Recipients API
+    Reference: https://paystack.com/docs/api/transfer-recipient/
+    """
+
+    async def create_transfer_recipients(
+            self,
+            recipient_type: str,
+            recipient_name: str,
+            account_number: str,
+            bank_code: str,
+            description: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            authorization_code: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a transfer recipient
+
+        :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
+        :param: recipient_name: The name of the transfer recipient according to their account registration
+        :param: account_number: transfer recipient's account number.
+                                Required for all recipient types except authorization
+        :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
+        :param: description:
+        :param: currency: transfer recipient's currency. [Currency.value.value ]
+        :param: authorization_code: transfer recipient's authorization code from previous transaction
+        :param: metadata: transfer recipient's metadata
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "type": recipient_type,
+            "name": recipient_name,
+            "account_number": account_number,
+            "bank_code": bank_code,
+            "description": description,
+            "currency": currency,
+            "authorization_code": authorization_code,
+            "metadata": metadata,
+        }
+        return await self._post_request("/transferrecipient", data=data)
+
+    async def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> PayStackResponse:
+        """
+        Create multiple transfer recipients in batches.
+
+        :param: batch: A list of transfer recipient object
+                        keys [ { type, name, account_number, bank_code, currency etc. }]
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"batch": batch}
+        return await self._post_request("/transferrecipient/bulk", data=data)
+
+    async def list_transfer_recipients(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List transfer recipients
+
+        :param: per_page: The number of records to return per page.
+        :param: page: The page number to retrieve.
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to strings
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return await self._get_request("/transferrecipient", params=params)
+
+    async def fetch_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
+        """
+        Fetch details of a transfer recipient
+
+        :param: id_or_code: The id or code of the transfer recipient
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/transferrecipient/{id_or_code}")
+
+    async def update_transfer_recipient(
+            self,
+            id_or_code: str,
+            recipient_name: str,
+            recipient_email: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a transfer recipient
+
+        :param: id_or_code: The id or code of the transfer recipient
+        :param: recipient_name: The name of the transfer recipient
+        :param: recipient_email: The email of the transfer recipient
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"name": recipient_name, "email": recipient_email}
+        return await self._put_request(f"/transferrecipient/{id_or_code}", data=data)
+
+    async def delete_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
+        """
+        Delete a transfer recipient
+
+        :param: id_or_code: The id or code of the transfer recipient
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._delete_request(f"/transferrecipient/{id_or_code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/atransfers.py` & `paystackease-2.0.4/paystackease/apis/async_apis/atransfers.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-"""
-Wrapper for Asynchronous Paystack Transfers APIs
-
-The Transfers API allows you to automate sending money to your customers.
-"""
-
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-from paystackease.helpers import Currency
-
-
-class AsyncTransfersClientAPI(AsyncRequestAPI):
-    """
-    Paystack Transfers API
-    Reference: https://paystack.com/docs/api/transfer/
-    """
-
-    async def initiate_transfer(
-            self,
-            transfer_source: str,
-            amount: int,
-            transfer_recipient: str,
-            reason: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            reference: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Initiate a transfer. Upgrade your business to a Registered Business to use
-
-        :param: transfer_source: Where should we transfer from? Only balance for now
-        :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
-        :param: transfer_recipient: The code of the recipient
-        :param: currency: The currency of the transfer
-        :param: reason: The reason for the transfer
-        :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
-                            Only -,_ and alphanumeric characters allowed.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "source": transfer_source,
-            "amount": amount,
-            "recipient": transfer_recipient,
-            "reason": reason,
-            "currency": currency,
-            "reference": reference,
-        }
-        return await self._post_request("/transfer", data=data)
-
-    async def finalize_transfer(self, transfer_code: str, otp: str) -> PayStackResponse:
-        """
-        Finalize an initiated transfer
-
-        :param: transfer_code: The code of the transfer to finalize
-        :param: otp: The OTP sent to the business phone to verify transfer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"transfer_code": transfer_code, "otp": otp}
-        return await self._post_request("/transfer/finalize_transfer", data=data)
-
-    async def initiate_bulk_transfer(
-            self, transfer_source: str, transfers: List[Dict[str, Any]]
-    ) -> PayStackResponse:
-        """
-        Batch multiple transfers in a single request
-
-        :param: transfer_source: Where should we transfer from? Only balance for now
-        :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"source": transfer_source, "transfers": transfers}
-        return await self._post_request("/transfer/bulk", data=data)
-
-    async def list_transfers(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer_id: Optional[Union[str, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List transfers
-
-        :param: per_page: The number of records to return per page.
-        :param: page: The page number to retrieve.
-        :param: customer_id
-        :param: from_date
-        :param: to_date
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer_id,
-            "from": from_date,
-            "to": to_date,
-        }
-        return await self._get_request("/transfer", params=params)
-
-    async def fetch_transfer(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a transfer
-
-        :param: id_or_code: The id or code of the transfer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/transfer/{id_or_code}")
-
-    async def verify_transfer(self, reference: str) -> PayStackResponse:
-        """
-        Verify a transfer
-
-        :param: reference: The reference of the transfer to verify
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._post_request(f"/transfer/verify/{reference}")
+"""
+Wrapper for Asynchronous Paystack Transfers APIs
+
+The Transfers API allows you to automate sending money to your customers.
+"""
+
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
+
+
+class AsyncTransfersClientAPI(AsyncRequestAPI):
+    """
+    Paystack Transfers API
+    Reference: https://paystack.com/docs/api/transfer/
+    """
+
+    async def initiate_transfer(
+            self,
+            transfer_source: str,
+            amount: int,
+            transfer_recipient: str,
+            reason: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Initiate a transfer. Upgrade your business to a Registered Business to use
+
+        :param: transfer_source: Where should we transfer from? Only balance for now
+        :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
+        :param: transfer_recipient: The code of the recipient
+        :param: currency: The currency of the transfer
+        :param: reason: The reason for the transfer
+        :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
+                            Only -,_ and alphanumeric characters allowed.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "source": transfer_source,
+            "amount": amount,
+            "recipient": transfer_recipient,
+            "reason": reason,
+            "currency": currency,
+            "reference": reference,
+        }
+        return await self._post_request("/transfer", data=data)
+
+    async def finalize_transfer(self, transfer_code: str, otp: str) -> PayStackResponse:
+        """
+        Finalize an initiated transfer
+
+        :param: transfer_code: The code of the transfer to finalize
+        :param: otp: The OTP sent to the business phone to verify transfer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"transfer_code": transfer_code, "otp": otp}
+        return await self._post_request("/transfer/finalize_transfer", data=data)
+
+    async def initiate_bulk_transfer(
+            self, transfer_source: str, transfers: List[Dict[str, Any]]
+    ) -> PayStackResponse:
+        """
+        Batch multiple transfers in a single request
+
+        :param: transfer_source: Where should we transfer from? Only balance for now
+        :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"source": transfer_source, "transfers": transfers}
+        return await self._post_request("/transfer/bulk", data=data)
+
+    async def list_transfers(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer_id: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List transfers
+
+        :param: per_page: The number of records to return per page.
+        :param: page: The page number to retrieve.
+        :param: customer_id
+        :param: from_date
+        :param: to_date
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer_id,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/transfer", params=params)
+
+    async def fetch_transfer(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a transfer
+
+        :param: id_or_code: The id or code of the transfer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/transfer/{id_or_code}")
+
+    async def verify_transfer(self, reference: str) -> PayStackResponse:
+        """
+        Verify a transfer
+
+        :param: reference: The reference of the transfer to verify
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._post_request(f"/transfer/verify/{reference}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/async_apis/averification.py` & `paystackease-2.0.4/paystackease/apis/async_apis/averification.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""
-Wrapper for Asynchronous Paystack Verification APIs
-
-The Verification API allows you to perform KYC processes.
-"""
-
-from paystackease.core import AsyncRequestAPI, PayStackResponse
-
-
-class AsyncVerificationClientAPI(AsyncRequestAPI):
-    """
-    Paystack Verification API
-    Reference: https://paystack.com/docs/api/verification/
-    """
-
-    async def resolve_account(self, account_number: str, bank_code: str) -> PayStackResponse:
-        """
-        Confirm an account belongs to the right customer.
-        This feature is available to business in Nigeria and Ghana.
-
-        :param: account_number: The account number to verify
-        :param: bank_code: The bank code to verify
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {"account_number": account_number, "bank_code": bank_code}
-        return await self._get_request("/bank/resolve", params=params)
-
-    async def validate_account(
-            self,
-            account_name: str,
-            account_number: str,
-            account_type: str,
-            bank_code: str,
-            country_code: str,
-            document_type: str,
-            document_number: str,
-    ) -> PayStackResponse:
-        """
-        Confirm the authenticity of a customer's account number before sending money.
-        This feature is only available to businesses in South Africa.
-
-        :param: account_name: The account name to validate: first and last name
-        :param: account_number: The account number to validate
-        :param: account_type: The account type to validate: personal or business
-        :param: bank_code: The bank code to validate
-        :param: country_code: The country code to validate
-        :param: document_type: The customer's mode of identity:
-                                identityNumber, passportNumber or businessRegistrationNumber
-        :param: document_number: The customer's document number
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "account_name": account_name,
-            "account_number": account_number,
-            "account_type": account_type,
-            "bank_code": bank_code,
-            "country_code": country_code,
-            "document_type": document_type,
-            "document_number": document_number,
-        }
-        return await self._post_request("/bank/validate", data=data)
-
-    async def resolve_card_bin(self, bin_code: str) -> PayStackResponse:
-        """
-        Resolve a card BIN
-
-        :param: bin_code: First 6 characters of card
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return await self._get_request(f"/decision/bin/{bin_code}")
+"""
+Wrapper for Asynchronous Paystack Verification APIs
+
+The Verification API allows you to perform KYC processes.
+"""
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+
+
+class AsyncVerificationClientAPI(AsyncRequestAPI):
+    """
+    Paystack Verification API
+    Reference: https://paystack.com/docs/api/verification/
+    """
+
+    async def resolve_account(self, account_number: str, bank_code: str) -> PayStackResponse:
+        """
+        Confirm an account belongs to the right customer.
+        This feature is available to business in Nigeria and Ghana.
+
+        :param: account_number: The account number to verify
+        :param: bank_code: The bank code to verify
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {"account_number": account_number, "bank_code": bank_code}
+        return await self._get_request("/bank/resolve", params=params)
+
+    async def validate_account(
+            self,
+            account_name: str,
+            account_number: str,
+            account_type: str,
+            bank_code: str,
+            country_code: str,
+            document_type: str,
+            document_number: str,
+    ) -> PayStackResponse:
+        """
+        Confirm the authenticity of a customer's account number before sending money.
+        This feature is only available to businesses in South Africa.
+
+        :param: account_name: The account name to validate: first and last name
+        :param: account_number: The account number to validate
+        :param: account_type: The account type to validate: personal or business
+        :param: bank_code: The bank code to validate
+        :param: country_code: The country code to validate
+        :param: document_type: The customer's mode of identity:
+                                identityNumber, passportNumber or businessRegistrationNumber
+        :param: document_number: The customer's document number
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "account_name": account_name,
+            "account_number": account_number,
+            "account_type": account_type,
+            "bank_code": bank_code,
+            "country_code": country_code,
+            "document_type": document_type,
+            "document_number": document_number,
+        }
+        return await self._post_request("/bank/validate", data=data)
+
+    async def resolve_card_bin(self, bin_code: str) -> PayStackResponse:
+        """
+        Resolve a card BIN
+
+        :param: bin_code: First 6 characters of card
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/decision/bin/{bin_code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/apple_pay.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/apple_pay.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-"""
-Wrapper class for Paystack Apple Pay API.
-
-The Apple Pay API allows you register your application's top-level domain or subdomain.
-"""
-
-from typing import Optional, Union
-from paystackease.core import PayStackResponse, SyncRequestAPI
-
-
-class ApplePayClientAPI(SyncRequestAPI):
-    """
-    Paystack Apple Pay API
-    Reference: https://paystack.com/docs/api/apple-pay/
-    """
-
-    def register_domain(self, domain_name: str) -> PayStackResponse:
-        """
-        Register a domain or subdomain for Apple Pay
-
-        :param: domain_name  # domain name or subdomain
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "domainName": domain_name,
-        }
-        return self._post_request("/apple-pay/domain", data=data)
-
-    def list_domains(
-            self,
-            use_cursor: Optional[Union[bool, None]] = False,
-            next_page: Optional[Union[int, None]] = None,
-            previous_page: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all registered domains
-
-        :param: use_cursor  # use cursor for pagination
-        :param: next_page  # next page
-        :param: previous_page  # previous page
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        use_cursor = self._convert_to_string(use_cursor)
-
-        params = {
-            "use_cursor": use_cursor,
-            "next": next_page,
-            "previous": previous_page,
-        }
-        return self._get_request("/apple-pay/domain", params=params)
-
-    def unregister_domain(self, domain_name: str) -> PayStackResponse:
-        """
-        Unregister a domain or subdomain for Apple Pay
-
-        :param: domain_name  # domain name or subdomain
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "domainName": domain_name,
-        }
-        return self._delete_request("/apple-pay/domain", data=data)
+"""
+Wrapper class for Paystack Apple Pay API.
+
+The Apple Pay API allows you register your application's top-level domain or subdomain.
+"""
+
+from typing import Optional, Union
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class ApplePayClientAPI(SyncRequestAPI):
+    """
+    Paystack Apple Pay API
+    Reference: https://paystack.com/docs/api/apple-pay/
+    """
+
+    def register_domain(self, domain_name: str) -> PayStackResponse:
+        """
+        Register a domain or subdomain for Apple Pay
+
+        :param: domain_name  # domain name or subdomain
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "domainName": domain_name,
+        }
+        return self._post_request("/apple-pay/domain", data=data)
+
+    def list_domains(
+            self,
+            use_cursor: Optional[Union[bool, None]] = False,
+            next_page: Optional[Union[int, None]] = None,
+            previous_page: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all registered domains
+
+        :param: use_cursor  # use cursor for pagination
+        :param: next_page  # next page
+        :param: previous_page  # previous page
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        use_cursor = self._convert_to_string(use_cursor)
+
+        params = {
+            "use_cursor": use_cursor,
+            "next": next_page,
+            "previous": previous_page,
+        }
+        return self._get_request("/apple-pay/domain", params=params)
+
+    def unregister_domain(self, domain_name: str) -> PayStackResponse:
+        """
+        Unregister a domain or subdomain for Apple Pay
+
+        :param: domain_name  # domain name or subdomain
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "domainName": domain_name,
+        }
+        return self._delete_request("/apple-pay/domain", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/bulk_charges.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/products.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,142 +1,128 @@
-""" Wrapper for Paystack Bulk Charges API.
-
-The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
-"""
-
-from datetime import date
-from typing import List, Dict, Optional, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import STATUS
-
-
-class BulkChargesClientAPI(SyncRequestAPI):
-    """
-    Paystack Bulk Charges API
-    Reference: https://paystack.com/docs/api/bulk-charge/
-    """
-
-    def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> PayStackResponse:
-        """
-        Send an array of objects with authorization codes and amount
-
-        :param: objects
-
-        note::
-
-            A list of dictionary with authorization codes, amount and reference as keys
-            [{"authorization": "123456", "amount": 1000, "reference": "123456" }]
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request("/bulkcharge", data=objects)
-
-    def list_bulk_charge_batches(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all bulk charges
-
-        :param: per_page
-        :param: page
-        :param: from_date
-        :param: to_date
-
-        note::
-
-            Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # Convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/bulkcharge", params=params)
-
-    def fetch_bulk_charge_batch(self, id_or_code: str) -> PayStackResponse:
-        """
-        Fetch a bulk charge of a specific batch
-
-        :param: id_or_code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/bulkcharge/{id_or_code}")
-
-    def fetch_charge_bulk_batch(
-            self,
-            id_or_code: str,
-            status: Optional[Union[STATUS, None]] = None,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Fetch a bulk charge of a specific batch
-
-        :param: id_or_code
-        :param: status:  {STATUS.value.value}
-        :param: per_page
-        :param: page
-        :param: from_date
-        :param: to_date
-
-        note::
-
-            Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
-            status: STATUS.value.value
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # Convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "status": status,
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
-
-    def pause_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
-        """
-        Pause a bulk charge of a specific batch
-
-        :param: batch_code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/bulkcharge/pause/{batch_code}")
-
-    def resume_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
-        """
-        Resume a bulk charge of a specific batch
-
-        :param: batch_code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/bulkcharge/resume/{batch_code}")
+"""
+Wrapper for Paystack Products API
+
+The Products API allows you to create and manage inventories on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class ProductClientAPI(SyncRequestAPI):
+    """
+    Paystack Product API
+    Reference: https://paystack.com/docs/api/product/
+    """
+
+    def create_product(
+            self,
+            name: str,
+            description: str,
+            amount: int,
+            currency: str,
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a product
+
+        :param: name: Name of the product
+        :param: description: Description of the product
+        :param: amount: Price of the product
+        :param: currency: Currency of the product
+        :param: unlimited: Set true if the product has unlimited stock,
+        :param: quantity: Quantity of the product in stock Use if unlimited is false
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        unlimited = self._convert_to_string(unlimited)
+
+        data = {
+            "name": name,
+            "description": description,
+            "price": amount,
+            "currency": currency,
+            "unlimited": unlimited,
+            "quantity": quantity,
+        }
+        return self._post_request("/product", data=data)
+
+    def list_products(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the products
+
+        :param: per_page: Number of records to return
+        :param: page:  number to return
+        :param: from_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+        :param: to_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to strings
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return self._get_request("/product", params=params)
+
+    def fetch_product(self, product_id: str) -> PayStackResponse:
+        """
+        Get details of a product
+
+        :param: product_id: ID or Code of the product
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/product/{product_id}")
+
+    def update_product(
+            self,
+            product_id: str,
+            name: str,
+            description: str,
+            amount: int,
+            currency: str,
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a product detail
+
+        :param: product_id: ID or Code of the product
+        :param: name: Name of the product
+        :param: description: Description of the product
+        :param: amount: Price of the product
+        :param: currency: Currency of the product
+        :param: unlimited: Set true if the product has unlimited stock,
+        :param: quantity: Quantity of the product in stock Use if unlimited is false
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        unlimited = self._convert_to_string(unlimited)
+
+        data = {
+            "name": name,
+            "description": description,
+            "price": amount,
+            "currency": currency,
+            "unlimited": unlimited,
+            "quantity": quantity,
+        }
+        return self._put_request(f"/product/{product_id}", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/charges.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/charges.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-"""
-Wrapper for Paystack Charges API.
-
-The Charge API allows you to configure payment channel of your choice when initiating a payment.
-"""
-
-from datetime import date
-from typing import Optional, Dict, Any, List, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import PWT
-
-
-class ChargesClientAPI(SyncRequestAPI):
-    """
-    Paystack Charges API
-    Reference: https://paystack.com/docs/api/charge/
-    """
-
-    def create_charge(
-            self,
-            email: str,
-            amount: int,
-            metadata: Dict[str, List[Dict[str, Any]]],
-            authorization_code: Optional[Union[str, None]] = None,
-            pin: Optional[Union[int, None]] = None,
-            reference: Optional[Union[str, None]] = None,
-            device_id: Optional[Union[str, None]] = None,
-            bank: Optional[Union[Dict[str, str], None]] = None,
-            bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
-            qr: Optional[Union[Dict[str, str], None]] = None,
-            ussd: Optional[Union[Dict[str, str], None]] = None,
-            mobile_money: Optional[Union[Dict[str, str], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a charge
-
-        :param: email
-        :param: amount
-        :param: bank. (Set key ass: {code, account_number})
-        :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
-        :param: qr (Set key as: {provider})
-        :param: authorization_code
-        :param: pin
-        :param: reference
-        :param: ussd (Set key as: {type})
-        :param: mobile_money (Set Keys as: {phone, provider}, and value {phone_number, MobileMoney.value.value})
-        :param: device_id
-        :param: metadata A JSON object, which is passed as-is to your integration API
-
-        note::
-
-            Do not send or use the following if charging an authorization code:
-            * bank
-            * ussd
-            * mobile_money
-
-            Do not send or use the following if charging an authorization code, bank or card:
-            * ussd
-            * mobile_money
-
-            Send with a non-reusable authorization code:
-            * pin
-
-            mobile_money is only available in Ghana and Kenya
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "amount": amount,
-            "metadata": metadata,
-            "authorization_code": authorization_code,
-            "bank": bank,
-            "bank_transfer": bank_transfer,
-            "qr": qr,
-            "pin": pin,
-            "reference": reference,
-            "ussd": ussd,
-            "mobile_money": mobile_money,
-            "device_id": device_id,
-        }
-        return self._post_request("/charge", data=data)
-
-    def submit_pin(self, pin: int, reference: str) -> PayStackResponse:
-        """
-        Submit a PIN for a charge
-
-        :param: pin
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "pin": pin,
-            "reference": reference,
-        }
-        return self._post_request("/charge/submit_pin", data=data)
-
-    def submit_otp(self, otp: int, reference: str) -> PayStackResponse:
-        """
-        Submit OTP to complete a charge
-
-        :param: otp
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "otp": otp,
-            "reference": reference,
-        }
-        return self._post_request("/charge/submit_otp", data=data)
-
-    def submit_phone(self, phone: str, reference: str) -> PayStackResponse:
-        """
-        Submit a phone number to complete a charge
-
-        :param: phone
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "phone": phone,
-            "reference": reference,
-        }
-        return self._post_request("/charge/submit_phone", data=data)
-
-    def submit_birthday(self, birthday: date, reference: str) -> PayStackResponse:
-        """
-        Submit birthday when required
-
-        :param: birthday
-        :param: reference
-
-        note::
-
-            Birthday submitted by user e.g. 2016-09-21
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        birthday = self._convert_to_string(birthday)
-
-        data = {
-            "birthday": birthday,
-            "reference": reference,
-        }
-        return self._post_request("/charge/submit_birthday", data=data)
-
-    def submit_address(
-            self, reference: str, address: str, city: str, state: str, zipcode: str
-    ) -> PayStackResponse:
-        """
-        Submit address to continue a charge
-
-        :param: reference
-        :param: address
-        :param: city
-        :param: state
-        :param: zipcode
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "reference": reference,
-            "address": address,
-            "city": city,
-            "state": state,
-            "zip_code": zipcode,
-        }
-        return self._post_request("/charge/submit_address", data=data)
-
-    def check_pending_charge(self, reference: str) -> PayStackResponse:
-        """
-        Check pending charge
-
-        :param: reference
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/charge/{reference}")
+"""
+Wrapper for Paystack Charges API.
+
+The Charge API allows you to configure payment channel of your choice when initiating a payment.
+"""
+
+from datetime import date
+from typing import Optional, Dict, Any, List, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import PWT
+
+
+class ChargesClientAPI(SyncRequestAPI):
+    """
+    Paystack Charges API
+    Reference: https://paystack.com/docs/api/charge/
+    """
+
+    def create_charge(
+            self,
+            email: str,
+            amount: int,
+            metadata: Dict[str, List[Dict[str, Any]]],
+            authorization_code: Optional[Union[str, None]] = None,
+            pin: Optional[Union[int, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+            device_id: Optional[Union[str, None]] = None,
+            bank: Optional[Union[Dict[str, str], None]] = None,
+            bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
+            qr: Optional[Union[Dict[str, str], None]] = None,
+            ussd: Optional[Union[Dict[str, str], None]] = None,
+            mobile_money: Optional[Union[Dict[str, str], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a charge
+
+        :param: email
+        :param: amount
+        :param: bank. (Set key ass: {code, account_number})
+        :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
+        :param: qr (Set key as: {provider})
+        :param: authorization_code
+        :param: pin
+        :param: reference
+        :param: ussd (Set key as: {type})
+        :param: mobile_money (Set Keys as: {phone, provider}, and value {phone_number, MobileMoney.value.value})
+        :param: device_id
+        :param: metadata A JSON object, which is passed as-is to your integration API
+
+        note::
+
+            Do not send or use the following if charging an authorization code:
+            * bank
+            * ussd
+            * mobile_money
+
+            Do not send or use the following if charging an authorization code, bank or card:
+            * ussd
+            * mobile_money
+
+            Send with a non-reusable authorization code:
+            * pin
+
+            mobile_money is only available in Ghana and Kenya
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "amount": amount,
+            "metadata": metadata,
+            "authorization_code": authorization_code,
+            "bank": bank,
+            "bank_transfer": bank_transfer,
+            "qr": qr,
+            "pin": pin,
+            "reference": reference,
+            "ussd": ussd,
+            "mobile_money": mobile_money,
+            "device_id": device_id,
+        }
+        return self._post_request("/charge", data=data)
+
+    def submit_pin(self, pin: int, reference: str) -> PayStackResponse:
+        """
+        Submit a PIN for a charge
+
+        :param: pin
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "pin": pin,
+            "reference": reference,
+        }
+        return self._post_request("/charge/submit_pin", data=data)
+
+    def submit_otp(self, otp: int, reference: str) -> PayStackResponse:
+        """
+        Submit OTP to complete a charge
+
+        :param: otp
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "otp": otp,
+            "reference": reference,
+        }
+        return self._post_request("/charge/submit_otp", data=data)
+
+    def submit_phone(self, phone: str, reference: str) -> PayStackResponse:
+        """
+        Submit a phone number to complete a charge
+
+        :param: phone
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "phone": phone,
+            "reference": reference,
+        }
+        return self._post_request("/charge/submit_phone", data=data)
+
+    def submit_birthday(self, birthday: date, reference: str) -> PayStackResponse:
+        """
+        Submit birthday when required
+
+        :param: birthday
+        :param: reference
+
+        note::
+
+            Birthday submitted by user e.g. 2016-09-21
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        birthday = self._convert_to_string(birthday)
+
+        data = {
+            "birthday": birthday,
+            "reference": reference,
+        }
+        return self._post_request("/charge/submit_birthday", data=data)
+
+    def submit_address(
+            self, reference: str, address: str, city: str, state: str, zipcode: str
+    ) -> PayStackResponse:
+        """
+        Submit address to continue a charge
+
+        :param: reference
+        :param: address
+        :param: city
+        :param: state
+        :param: zipcode
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "reference": reference,
+            "address": address,
+            "city": city,
+            "state": state,
+            "zip_code": zipcode,
+        }
+        return self._post_request("/charge/submit_address", data=data)
+
+    def check_pending_charge(self, reference: str) -> PayStackResponse:
+        """
+        Check pending charge
+
+        :param: reference
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/charge/{reference}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/customers.py` & `paystackease-2.0.4/paystackease/apis/async_apis/acustomers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-"""
-Wrapper for Paystack Customers API.
-
-The Customers API allows you to create and manage customers on your integration.
-"""
-
-from datetime import date
-from typing import Optional, Dict, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import RiskAction
-
-
-class CustomerClientAPI(SyncRequestAPI):
-    """
-    Paystack Customer API
-    Reference: https://paystack.com/docs/api/customer/
-    """
-
-    def create_customer(
-            self, 
-            email: str, 
-            first_name: str, 
-            last_name: str, 
-            phone: str, 
-            metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> PayStackResponse:
-        """
-        Create a customer
-
-        :param: email: The email associated with the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: phone: The phone number of the customer.
-        :param: metadata: The metadata of the customer in JSON format.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-            "metadata": metadata,
-        }
-        return self._post_request("/customer", data=data)
-
-    def validate_customer(
-            self,
-            email_or_code: str,
-            first_name: str,
-            last_name: str,
-            account_type: str,
-            country: str,
-            bank_code: str,
-            account_number: str,
-            bvn: str,
-            customer_id_num: Optional[Union[str, None]] = None,
-            middle_name: Optional[Union[str, None]] = None
-    ) -> PayStackResponse:
-        """
-        Validate a customer's identity
-
-        :param: email_or_code: The email or code of the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: middle_name: The middle name of the customer.
-        :param: account_type: The type of account. Only bank_account is currently supported.
-        :param: customer_id_num: The customer identification number
-        :param: country: The country of the customer. 2-letter country code of identification issuer
-        :param: bvn: The Bank Verification Number
-        :param: bank_code: The bank code of the customer
-        :param: account_number: The account number of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "first_name": first_name,
-            "last_name": last_name,
-            "middle_name": middle_name,
-            "type": account_type,
-            "value": customer_id_num,
-            "country": country,
-            "bvn": bvn,
-            "bank_code": bank_code,
-            "account_number": account_number,
-        }
-        return self._post_request(f"customer/{email_or_code}/identification", data=data)
-
-    def whitelist_blacklist_customer(
-            self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
-    ) -> PayStackResponse:
-        """
-        Whitelist or blacklist a customer
-
-        :param: email_or_code: The code or email of the customer.
-        :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "customer": email_or_code,
-            "risk_action": risk_action
-        }
-        return self._post_request("/customer/set_risk_action", data=data)
-
-    def deactivate_authorization(self, authorization_code: str) -> PayStackResponse:
-        """
-        Deactivate an authorization when the card needs to be forgotten
-
-        :param: authorization_code: The authorization code to be deactivated.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"authorization_code": authorization_code}
-        return self._post_request("/customer/deactivate_authorization", data=data)
-
-    def update_customer(
-            self,
-            customer_code: str,
-            first_name: Optional[Union[str, None]] = None,
-            last_name: Optional[Union[str, None]] = None,
-            phone: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> PayStackResponse:
-        """
-        Update a customer
-
-        :param: customer_code: The code of the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: phone: The phone number of the customer.
-        :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-            "metadata": metadata,
-        }
-        return self._put_request(f"/customer/{customer_code}", data=data)
-
-    def fetch_customer(self, email_or_code: str) -> PayStackResponse:
-        """
-        Fetch details of a specific customer
-
-        :param: email_or_code: The email or code of the customer.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/customer/{email_or_code}")
-
-    def list_customers(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all customers
-
-        :param: per_page: The number of records to return.
-        :param: page: The page number to return.
-        :param: from_date: The date to start returning customers from
-        :param: to_date: The date to stop returning customers from
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date  to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/customer", params=params)
+"""
+Wrapper for Asynchronous Paystack Customers API.
+
+The Customers API allows you to create and manage customers on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Dict, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import RiskAction
+
+
+class AsyncCustomerClientAPI(AsyncRequestAPI):
+    """
+    Paystack Customer API
+    Reference: https://paystack.com/docs/api/customer/
+    """
+
+    async def create_customer(
+            self,
+            email: str,
+            first_name: str,
+            last_name: str,
+            phone: str,
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> PayStackResponse:
+        """
+        Create a customer
+
+        :param: email: The email associated with the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: phone: The phone number of the customer.
+        :param: metadata: The metadata of the customer in JSON format.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+            "metadata": metadata,
+        }
+        return await self._post_request("/customer", data=data)
+
+    async def validate_customer(
+            self,
+            email_or_code: str,
+            first_name: str,
+            last_name: str,
+            account_type: str,
+            country: str,
+            bank_code: str,
+            account_number: str,
+            bvn: str,
+            customer_id_num: Optional[Union[str, None]] = None,
+            middle_name: Optional[Union[str, None]] = None
+    ) -> PayStackResponse:
+        """
+        Validate a customer's identity
+
+        :param: email_or_code: The email or code of the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: middle_name: The middle name of the customer.
+        :param: account_type: The type of account. Only bank_account is currently supported.
+        :param: customer_id_num: The customer identification number
+        :param: country: The country of the customer. 2-letter country code of identification issuer
+        :param: bvn: The Bank Verification Number
+        :param: bank_code: The bank code of the customer
+        :param: account_number: The account number of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "first_name": first_name,
+            "last_name": last_name,
+            "middle_name": middle_name,
+            "type": account_type,
+            "value": customer_id_num,
+            "country": country,
+            "bvn": bvn,
+            "bank_code": bank_code,
+            "account_number": account_number,
+        }
+        return await self._post_request(f"customer/{email_or_code}/identification", data=data)
+
+    async def whitelist_blacklist_customer(
+            self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
+    ) -> PayStackResponse:
+        """
+        Whitelist or blacklist a customer
+
+        :param: email_or_code: The code or email of the customer.
+        :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "customer": email_or_code,
+            "risk_action": risk_action
+        }
+        return await self._post_request("/customer/set_risk_action", data=data)
+
+    async def deactivate_authorization(self, authorization_code: str) -> PayStackResponse:
+        """
+        Deactivate an authorization when the card needs to be forgotten
+
+        :param: authorization_code: The authorization code to be deactivated.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"authorization_code": authorization_code}
+        return await self._post_request("/customer/deactivate_authorization", data=data)
+
+    async def update_customer(
+            self,
+            customer_code: str,
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> PayStackResponse:
+        """
+        Update a customer
+
+        :param: customer_code: The code of the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: phone: The phone number of the customer.
+        :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+            "metadata": metadata,
+        }
+        return await self._put_request(f"/customer/{customer_code}", data=data)
+
+    async def fetch_customer(self, email_or_code: str) -> PayStackResponse:
+        """
+        Fetch details of a specific customer
+
+        :param: email_or_code: The email or code of the customer.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/customer/{email_or_code}")
+
+    async def list_customers(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all customers
+
+        :param: per_page: The number of records to return.
+        :param: page: The page number to return.
+        :param: from_date: The date to start returning customers from
+        :param: to_date: The date to stop returning customers from
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date  to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return await self._get_request("/customer", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/dedicated_virtual_accounts.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-"""
-Wrapper for Paystack Dedicated Virtual Account API
-
-The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import Currency
-
-
-class DedicatedVirtualAccountClientAPI(SyncRequestAPI):
-    """
-    Paystack Dedicated Virtual Account API
-    Reference: https://paystack.com/docs/api/dedicated-virtual-account/
-
-    note::
-        Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
-    """
-
-    def create_virtual_account(
-            self,
-            customer_id_or_code: str,
-            preferred_bank: Optional[Union[str, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            first_name: Optional[Union[str, None]] = None,
-            last_name: Optional[Union[str, None]] = None,
-            phone: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a dedicated virtual account for existing customers.
-        Currently, support Wema Bank and Titan Paystack.
-
-        :param: customer_id_or_code: The customer's ID or Code
-        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
-
-        note::
-
-             currently support Wema Bank and Titan Paystack.
-
-        :param: subaccount: Subaccount code of the account you want to split the transaction.
-        :param: split_code: Split code
-        :param: first_name: First name of the customer
-        :param: last_name: Last name of the customer
-        :param: phone: Phone number of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "customer": customer_id_or_code,
-            "preferred_bank": preferred_bank,
-            "subaccount": subaccount,
-            "split_code": split_code,
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-        }
-        return self._post_request("/dedicated_account", data=data)
-
-    def assign_dedicated_virtual_account(
-            self,
-            email: str,
-            first_name: str,
-            last_name: str,
-            phone: str,
-            preferred_bank: str,
-            country: str,
-            account_number: Optional[Union[str, None]] = None,
-            bvn: Optional[Union[str, None]] = None,
-            bank_code: Optional[Union[str, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        create a customer, validate the customer, and assign a DVA to the customer
-
-        :param: email: The email associated with the customer.
-        :param: first_name: The first name of the customer.
-        :param: last_name: The last name of the customer.
-        :param: phone: The phone number of the customer.
-        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
-
-        note::
-
-             currently support Wema Bank and Titan Paystack.
-
-        :param: country: The country of the customer. 2-letter country code of identification issuer
-
-        note::
-
-             currently accepts NG only.
-
-        :param: account_number: The account number of the customer
-        :param: bvn: The Bank Verification Number
-        :param: bank_code: The bank code of the customer
-        :param: subaccount: Subaccount code of the account you want to split the transaction.
-        :param: split_code: Split code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "first_name": first_name,
-            "last_name": last_name,
-            "phone": phone,
-            "preferred_bank": preferred_bank,
-            "country": country,
-            "account_number": account_number,
-            "bvn": bvn,
-            "bank_code": bank_code,
-            "subaccount": subaccount,
-            "split_code": split_code,
-        }
-        return self._post_request("/dedicated_account", data=data)
-
-    def list_dedicated_account(
-            self,
-            active: Optional[Union[bool, None]] = True,
-            currency: Optional[Union[Currency, None]] = None,
-            provider_slug: Optional[Union[str, None]] = None,
-            bank_id: Optional[Union[str, None]] = None,
-            customer_id: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List dedicated accounts
-
-        :param: active: Shows the status of the dedicated virtual account
-        :param: currency: Currency of the dedicated virtual account
-        :param: provider_slug: Provider slug in lowercase eg: wema-bank
-        :param: bank_id: Bank ID of the dedicated virtual account eg: 035
-        :param: customer_id: Customer ID of the dedicated virtual account
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert date to string
-        active = self._convert_to_string(active)
-
-        params = {
-            "active": active,
-            "currency": currency,
-            "provider_slug": provider_slug,
-            "bank_id": bank_id,
-            "customer": customer_id,
-        }
-        return self._get_request("/dedicated_account", params=params)
-
-    def fetch_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
-        """
-        Get details of a dedicated virtual account
-
-        :param: dedicated_account_id: Dedicated account ID
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/dedicated_account/{dedicated_account_id}")
-
-    def requery_dedicated_account(
-            self,
-            account_number: Optional[Union[str, None]] = None,
-            provider_slug: Optional[Union[str, None]] = None,
-            date_transfer: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Requery a dedicated virtual account for new transactions
-
-        :param: account_number: Virtual Account number to requery
-        :param: provider_slug: Provider slug in lowercase eg: wema-bank
-        :param: date_transfer: Date of when the transfer was made
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        date_transfer = self._convert_to_string(date_transfer)
-
-        params = {
-            "account_number": account_number,
-            "provider_slug": provider_slug,
-            "date": date_transfer,
-        }
-        return self._get_request("/dedicated_account/requery", params=params)
-
-    def deactivate_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
-        """
-        Deactivate a dedicated virtual account
-
-        :param: dedicated_account_id: Dedicated account ID
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._delete_request(f"/dedicated_account/{dedicated_account_id}")
-
-    def split_dedicated_account(
-            self,
-            customer_id_or_code: str,
-            subaccount: Optional[Union[str, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            preferred_bank: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Split a dedicated virtual account transaction with one or more accounts
-
-        :param: customer_id_or_code: Customer's ID or Code
-        :param: subaccount: Subaccount code of the account you want to split the transaction
-        :param: split_code: Split code
-        :param: preferred_bank: Preferred bank for the virtual account
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "customer": customer_id_or_code,
-            "preferred_bank": preferred_bank,
-            "subaccount": subaccount,
-            "split_code": split_code,
-        }
-        return self._post_request("/dedicated_account/split", data=data)
-
-    def remove_split_dedicated_account(self, account_number: str) -> PayStackResponse:
-        """
-        Remove a split dedicated virtual account
-
-        :param: account_number: the account number of the dedicated virtual account
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "account_number": account_number,
-        }
-        return self._delete_request("/dedicated_account/split", data=data)
-
-    def fetch_bank_providers(self) -> PayStackResponse:
-        """
-        Fetch bank providers
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request("/dedicated_account/available_providers")
+"""
+Wrapper for Paystack Dedicated Virtual Account API
+
+The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
+
+
+class DedicatedVirtualAccountClientAPI(SyncRequestAPI):
+    """
+    Paystack Dedicated Virtual Account API
+    Reference: https://paystack.com/docs/api/dedicated-virtual-account/
+
+    note::
+        Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
+    """
+
+    def create_virtual_account(
+            self,
+            customer_id_or_code: str,
+            preferred_bank: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a dedicated virtual account for existing customers.
+        Currently, support Wema Bank and Titan Paystack.
+
+        :param: customer_id_or_code: The customer's ID or Code
+        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
+
+        note::
+
+             currently support Wema Bank and Titan Paystack.
+
+        :param: subaccount: Subaccount code of the account you want to split the transaction.
+        :param: split_code: Split code
+        :param: first_name: First name of the customer
+        :param: last_name: Last name of the customer
+        :param: phone: Phone number of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "customer": customer_id_or_code,
+            "preferred_bank": preferred_bank,
+            "subaccount": subaccount,
+            "split_code": split_code,
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+        }
+        return self._post_request("/dedicated_account", data=data)
+
+    def assign_dedicated_virtual_account(
+            self,
+            email: str,
+            first_name: str,
+            last_name: str,
+            phone: str,
+            preferred_bank: str,
+            country: str,
+            account_number: Optional[Union[str, None]] = None,
+            bvn: Optional[Union[str, None]] = None,
+            bank_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        create a customer, validate the customer, and assign a DVA to the customer
+
+        :param: email: The email associated with the customer.
+        :param: first_name: The first name of the customer.
+        :param: last_name: The last name of the customer.
+        :param: phone: The phone number of the customer.
+        :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
+
+        note::
+
+             currently support Wema Bank and Titan Paystack.
+
+        :param: country: The country of the customer. 2-letter country code of identification issuer
+
+        note::
+
+             currently accepts NG only.
+
+        :param: account_number: The account number of the customer
+        :param: bvn: The Bank Verification Number
+        :param: bank_code: The bank code of the customer
+        :param: subaccount: Subaccount code of the account you want to split the transaction.
+        :param: split_code: Split code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "first_name": first_name,
+            "last_name": last_name,
+            "phone": phone,
+            "preferred_bank": preferred_bank,
+            "country": country,
+            "account_number": account_number,
+            "bvn": bvn,
+            "bank_code": bank_code,
+            "subaccount": subaccount,
+            "split_code": split_code,
+        }
+        return self._post_request("/dedicated_account", data=data)
+
+    def list_dedicated_account(
+            self,
+            active: Optional[Union[bool, None]] = True,
+            currency: Optional[Union[Currency, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            bank_id: Optional[Union[str, None]] = None,
+            customer_id: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List dedicated accounts
+
+        :param: active: Shows the status of the dedicated virtual account
+        :param: currency: Currency of the dedicated virtual account
+        :param: provider_slug: Provider slug in lowercase eg: wema-bank
+        :param: bank_id: Bank ID of the dedicated virtual account eg: 035
+        :param: customer_id: Customer ID of the dedicated virtual account
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert date to string
+        active = self._convert_to_string(active)
+
+        params = {
+            "active": active,
+            "currency": currency,
+            "provider_slug": provider_slug,
+            "bank_id": bank_id,
+            "customer": customer_id,
+        }
+        return self._get_request("/dedicated_account", params=params)
+
+    def fetch_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
+        """
+        Get details of a dedicated virtual account
+
+        :param: dedicated_account_id: Dedicated account ID
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/dedicated_account/{dedicated_account_id}")
+
+    def requery_dedicated_account(
+            self,
+            account_number: Optional[Union[str, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            date_transfer: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Requery a dedicated virtual account for new transactions
+
+        :param: account_number: Virtual Account number to requery
+        :param: provider_slug: Provider slug in lowercase eg: wema-bank
+        :param: date_transfer: Date of when the transfer was made
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        date_transfer = self._convert_to_string(date_transfer)
+
+        params = {
+            "account_number": account_number,
+            "provider_slug": provider_slug,
+            "date": date_transfer,
+        }
+        return self._get_request("/dedicated_account/requery", params=params)
+
+    def deactivate_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
+        """
+        Deactivate a dedicated virtual account
+
+        :param: dedicated_account_id: Dedicated account ID
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._delete_request(f"/dedicated_account/{dedicated_account_id}")
+
+    def split_dedicated_account(
+            self,
+            customer_id_or_code: str,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            preferred_bank: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Split a dedicated virtual account transaction with one or more accounts
+
+        :param: customer_id_or_code: Customer's ID or Code
+        :param: subaccount: Subaccount code of the account you want to split the transaction
+        :param: split_code: Split code
+        :param: preferred_bank: Preferred bank for the virtual account
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "customer": customer_id_or_code,
+            "preferred_bank": preferred_bank,
+            "subaccount": subaccount,
+            "split_code": split_code,
+        }
+        return self._post_request("/dedicated_account/split", data=data)
+
+    def remove_split_dedicated_account(self, account_number: str) -> PayStackResponse:
+        """
+        Remove a split dedicated virtual account
+
+        :param: account_number: the account number of the dedicated virtual account
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "account_number": account_number,
+        }
+        return self._delete_request("/dedicated_account/split", data=data)
+
+    def fetch_bank_providers(self) -> PayStackResponse:
+        """
+        Fetch bank providers
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request("/dedicated_account/available_providers")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/disputes.py` & `paystackease-2.0.4/paystackease/apis/async_apis/adisputes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-"""
-Wrapper for Paystack Disputes API
-
-The Disputes API allows you manage transaction disputes on your integration.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import DisputeStatus, Resolution
-
-
-class DisputesClientAPI(SyncRequestAPI):
-    """
-    Paystack Disputes API
-    Reference: https://paystack.com/docs/api/dispute/
-    """
-
-    def list_disputes(
-            self,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            transaction_id: Optional[Union[str, None]] = None,
-            status: Optional[Union[DisputeStatus, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List disputes filed against you
-
-        :param: from_date: A timestamp from which to start listing dispute e.g. 2016-09-21
-        :param: to_date: A timestamp from which to start listing dispute e.g. 2016-09-21
-        :param: per_page:
-        :param: page:
-        :param: transaction_id:
-        :param: status: Dispute Status. Acceptable values:
-                        { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-            "transaction": transaction_id,
-            "status": status,
-        }
-        return self._get_request("/dispute", params=params)
-
-    def fetch_dispute(self, dispute_id: str) -> PayStackResponse:
-        """
-        Fetch details about a dispute
-
-        :param: dispute_id: The dispute ID to fetch
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/dispute/{dispute_id}")
-
-    def list_transaction_disputes(self, transaction_id: str) -> PayStackResponse:
-        """
-        List disputes for a transaction
-
-        :param: transaction_id: The transaction id to fetch
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/dispute/transaction/{transaction_id}")
-
-    def update_dispute(
-            self,
-            dispute_id: str,
-            refund_amount: int,
-            uploaded_filename: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update details of a dispute
-
-        :param: dispute_id: The dispute id to fetch
-        :param: refund_amount: The amount to refund to the customer
-        :param: uploaded_filename: filename of attachment returned via
-                                    PayStackResponse from upload url(GET /dispute/:id/upload_url)
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"refund_amount": refund_amount, "uploaded_filename": uploaded_filename}
-        return self._put_request(f"/dispute/{dispute_id}", data=data)
-
-    def add_evidence(
-            self,
-            dispute_id: str,
-            customer_email: str,
-            customer_name: str,
-            customer_phone: str,
-            service_details: str,
-            delivery_address: Optional[Union[str, None]] = None,
-            delivery_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Add evidence to a dispute
-
-        :param: dispute_id: The dispute id to fetch
-        :param: customer_email: The customer email
-        :param: customer_name: The customer name
-        :param: customer_phone: The customer phone
-        :param: service_details: The service details
-        :param: delivery_address: The delivery address
-        :param: delivery_date: The delivery date: YYYY-MM-DD
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        delivery_date = self._convert_to_string(delivery_date)
-
-        data = {
-            "customer_email": customer_email,
-            "customer_name": customer_name,
-            "customer_phone": customer_phone,
-            "service_details": service_details,
-            "delivery_address": delivery_address,
-            "delivery_date": delivery_date,
-        }
-        return self._post_request(f"/dispute/{dispute_id}/evidence", data=data)
-
-    def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> PayStackResponse:
-        """
-        Get upload url for dispute evidence
-
-        :param: dispute_id: The dispute id to fetch
-        :param: uploaded_filename: The file name, with its extension, that you want to upload. e.g. filename.pdf
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {"uploaded_filename": uploaded_filename}
-        return self._get_request(f"/dispute/{dispute_id}/upload_url", params=params)
-
-    def resolve_dispute(
-            self,
-            dispute_id: str,
-            resolution: Resolution,
-            message: str,
-            refund_amount: int,
-            uploaded_filename: str,
-            evidence: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Resolve a dispute
-
-        :param: dispute_id: The dispute id to fetch
-        :param: resolution: The resolution to resolve the dispute: Accepted values: { merchant-accepted | declined }.
-        :param: message: The message for resolution
-        :param: refund_amount: The amount to refund to the customer
-        :param: uploaded_filename: filename of attachment returned via PayStackResponse from method get_upload_url
-        :param: evidence: The evidence id for fraud claims
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "resolution": resolution,
-            "message": message,
-            "refund_amount": refund_amount,
-            "uploaded_filename": uploaded_filename,
-            "evidence": evidence,
-        }
-        return self._put_request(f"/dispute/{dispute_id}/resolve", data=data)
-
-    def export_disputes(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-            transaction_id: Optional[Union[str, None]] = None,
-            status: Optional[Union[DisputeStatus, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Export disputes
-
-        :param: per_page:
-        :param: page:
-        :param: from_date: The start date to fetch disputes from
-        :param: to_date: The end date to fetch disputes from
-        :param: transaction_id: The transaction ID
-        :param: status: The dispute status:
-                        Acceptable values: { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-            "transaction": transaction_id,
-            "status": status,
-        }
-        return self._get_request("/dispute/export", params=params)
+"""
+Wrapper for Asynchronous Paystack Disputes API
+
+The Disputes API allows you manage transaction disputes on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import DisputeStatus, Resolution
+
+
+class AsyncDisputesClientAPI(AsyncRequestAPI):
+    """
+    Paystack Disputes API
+    Reference: https://paystack.com/docs/api/dispute/
+    """
+
+    async def list_disputes(
+            self,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List disputes filed against you
+
+        :param: from_date: A timestamp from which to start listing dispute e.g. 2016-09-21
+        :param: to_date: A timestamp from which to start listing dispute e.g. 2016-09-21
+        :param: per_page:
+        :param: page:
+        :param: transaction_id:
+        :param: status: Dispute Status. Acceptable values:
+                        { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+            "transaction": transaction_id,
+            "status": status,
+        }
+        return await self._get_request("/dispute", params=params)
+
+    async def fetch_dispute(self, dispute_id: str) -> PayStackResponse:
+        """
+        Fetch details about a dispute
+
+        :param: dispute_id: The dispute ID to fetch
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/dispute/{dispute_id}")
+
+    async def list_transaction_disputes(self, transaction_id: str) -> PayStackResponse:
+        """
+        List disputes for a transaction
+
+        :param: transaction_id: The transaction id to fetch
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/dispute/transaction/{transaction_id}")
+
+    async def update_dispute(
+            self,
+            dispute_id: str,
+            refund_amount: int,
+            uploaded_filename: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update details of a dispute
+
+        :param: dispute_id: The dispute id to fetch
+        :param: refund_amount: The amount to refund to the customer
+        :param: uploaded_filename: filename of attachment returned via
+                                    PayStackResponse from upload url(GET /dispute/:id/upload_url)
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"refund_amount": refund_amount, "uploaded_filename": uploaded_filename}
+        return await self._put_request(f"/dispute/{dispute_id}", data=data)
+
+    async def add_evidence(
+            self,
+            dispute_id: str,
+            customer_email: str,
+            customer_name: str,
+            customer_phone: str,
+            service_details: str,
+            delivery_address: Optional[Union[str, None]] = None,
+            delivery_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Add evidence to a dispute
+
+        :param: dispute_id: The dispute id to fetch
+        :param: customer_email: The customer email
+        :param: customer_name: The customer name
+        :param: customer_phone: The customer phone
+        :param: service_details: The service details
+        :param: delivery_address: The delivery address
+        :param: delivery_date: The delivery date: YYYY-MM-DD
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        delivery_date = self._convert_to_string(delivery_date)
+
+        data = {
+            "customer_email": customer_email,
+            "customer_name": customer_name,
+            "customer_phone": customer_phone,
+            "service_details": service_details,
+            "delivery_address": delivery_address,
+            "delivery_date": delivery_date,
+        }
+        return await self._post_request(f"/dispute/{dispute_id}/evidence", data=data)
+
+    async def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> PayStackResponse:
+        """
+        Get upload url for dispute evidence
+
+        :param: dispute_id: The dispute id to fetch
+        :param: uploaded_filename: The file name, with its extension, that you want to upload. e.g. filename.pdf
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {"uploaded_filename": uploaded_filename}
+        return await self._get_request(f"/dispute/{dispute_id}/upload_url", params=params)
+
+    async def resolve_dispute(
+            self,
+            dispute_id: str,
+            resolution: Resolution,
+            message: str,
+            refund_amount: int,
+            uploaded_filename: str,
+            evidence: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Resolve a dispute
+
+        :param: dispute_id: The dispute id to fetch
+        :param: resolution: The resolution to resolve the dispute: Accepted values: { merchant-accepted | declined }.
+        :param: message: The message for resolution
+        :param: refund_amount: The amount to refund to the customer
+        :param: uploaded_filename: filename of attachment returned via PayStackResponse from method get_upload_url
+        :param: evidence: The evidence id for fraud claims
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "resolution": resolution,
+            "message": message,
+            "refund_amount": refund_amount,
+            "uploaded_filename": uploaded_filename,
+            "evidence": evidence,
+        }
+        return await self._put_request(f"/dispute/{dispute_id}/resolve", data=data)
+
+    async def export_disputes(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Export disputes
+
+        :param: per_page:
+        :param: page:
+        :param: from_date: The start date to fetch disputes from
+        :param: to_date: The end date to fetch disputes from
+        :param: transaction_id: The transaction ID
+        :param: status: The dispute status:
+                        Acceptable values: { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+            "transaction": transaction_id,
+            "status": status,
+        }
+        return await self._get_request("/dispute/export", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/miscellaneous.py` & `paystackease-2.0.4/paystackease/apis/async_apis/amiscellaneous.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,99 @@
-"""
-Wrapper for Paystack Miscellaneous API.
-
-The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
-"""
-
-from typing import Optional, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import GateWay, Channels, Currency
-
-
-class MiscellaneousClientAPI(SyncRequestAPI):
-    """
-    Paystack Miscellaneous API
-    Reference: https://paystack.com/docs/api/miscellaneous/
-    """
-
-    def list_banks(
-            self,
-            country: Optional[Union[str, None]] = None,
-            use_cursor: Optional[Union[bool, None]] = False,
-            per_page: Optional[Union[int, None]] = 50,
-            pay_with_bank_transfer: Optional[Union[bool, None]] = False,
-            pay_with_bank: Optional[Union[bool, None]] = False,
-            enabled_for_verification: Optional[Union[bool, None]] = False,
-            next_cursor: Optional[Union[str, None]] = None,
-            previous_cursor: Optional[Union[str, None]] = None,
-            gateway: Optional[Union[GateWay, None]] = None,
-            channel_type: Optional[Union[Channels, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Get a list of all supported banks and their properties
-
-        :param: country: The country to obtain the list of supported banks.
-                        Values { country=ghana or country=nigeria }
-        :param: use_cursor: Use cursor to paginate through the list of supported banks
-        :param: per_page: The number of records to return per page: 10, 20 or 50
-        :param: pay_with_bank_transfer: filter for available banks a customer can make a transfer to complete a payment
-        :param: pay_with_bank: filter for banks a customer can pay directly from
-        :param: enabled_for_verification: filter the banks that are supported for account
-                                            verification in South Africa. Combine with currency or country filter
-        :param: next_cursor: The cursor for the next page of results
-        :param: previous_cursor: The cursor for the previous page of results
-        :param: gateway: filters for banks that support a specific payment gateway:
-                        { emandate or digitalbankmandate }
-        :param: currency: filter for banks that support a specific currency
-        :param: channel_type: Type of financial channel. { Channels.value.value}
-
-        **note::**
-
-        For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        use_cursor = self._convert_to_string(use_cursor)
-        pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
-        pay_with_bank = self._convert_to_string(pay_with_bank)
-        enabled_for_verification = self._convert_to_string(enabled_for_verification)
-
-        params = {
-            "country": country,
-            "use_cursor": use_cursor,
-            "perPage": per_page,
-            "supports_transfer": pay_with_bank_transfer,
-            "pay_with_bank": pay_with_bank,
-            "enabled_for_verification": enabled_for_verification,
-            "next": next_cursor,
-            "previous": previous_cursor,
-            "gateway": gateway,
-            "type": channel_type,
-            "currency": currency,
-        }
-        return self._get_request("/bank", params=params)
-
-    def list_countries(self) -> PayStackResponse:
-        """
-        Get a list of all supported countries and their properties
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request("/country")
-
-    def list_states(self, country: str) -> PayStackResponse:
-        """
-        Get a list of all supported states and their properties
-
-        :param: country: The country code from which to obtain the list of supported states
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {"country": country}
-        return self._get_request("/address_verification/states", params=params)
+"""
+Wrapper for Paystack Miscellaneous API.
+
+The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
+"""
+
+from typing import Optional, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import GateWay, Channels, Currency
+
+
+class AsyncMiscellaneousClientAPI(AsyncRequestAPI):
+    """
+    Paystack Miscellaneous API
+    Reference: https://paystack.com/docs/api/miscellaneous/
+    """
+
+    async def list_banks(
+            self,
+            country: Optional[Union[str, None]] = None,
+            use_cursor: Optional[Union[bool, None]] = False,
+            per_page: Optional[Union[int, None]] = 50,
+            pay_with_bank_transfer: Optional[Union[bool, None]] = False,
+            pay_with_bank: Optional[Union[bool, None]] = False,
+            enabled_for_verification: Optional[Union[bool, None]] = False,
+            next_cursor: Optional[Union[str, None]] = None,
+            previous_cursor: Optional[Union[str, None]] = None,
+            gateway: Optional[Union[GateWay, None]] = None,
+            channel_type: Optional[Union[Channels, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Get a list of all supported banks and their properties
+
+        :param: country: The country to obtain the list of supported banks.
+                        Values { country=ghana or country=nigeria }
+        :param: use_cursor: Use cursor to paginate through the list of supported banks
+        :param: per_page: The number of records to return per page: 10, 20 or 50
+        :param: pay_with_bank_transfer: filter for available banks a customer can make a transfer to complete a payment
+        :param: pay_with_bank: filter for banks a customer can pay directly from
+        :param: enabled_for_verification: filter the banks that are supported for account
+                                            verification in South Africa. Combine with currency or country filter
+        :param: next_cursor: The cursor for the next page of results
+        :param: previous_cursor: The cursor for the previous page of results
+        :param: gateway: filters for banks that support a specific payment gateway:
+                        { emandate or digitalbankmandate }
+        :param: currency: filter for banks that support a specific currency
+        :param: channel_type: Type of financial channel. { Channels.value.value}
+
+        **note::**
+
+        For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert to strings
+        use_cursor = self._convert_to_string(use_cursor)
+        pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
+        pay_with_bank = self._convert_to_string(pay_with_bank)
+        enabled_for_verification = self._convert_to_string(enabled_for_verification)
+
+        params = {
+            "country": country,
+            "use_cursor": use_cursor,
+            "perPage": per_page,
+            "supports_transfer": pay_with_bank_transfer,
+            "pay_with_bank": pay_with_bank,
+            "enabled_for_verification": enabled_for_verification,
+            "next": next_cursor,
+            "previous": previous_cursor,
+            "gateway": gateway,
+            "type": channel_type,
+            "currency": currency,
+        }
+        return await self._get_request("/bank", params=params)
+
+    async def list_countries(self) -> PayStackResponse:
+        """
+        Get a list of all supported countries and their properties
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request("/country")
+
+    async def list_states(self, country: str) -> PayStackResponse:
+        """
+        Get a list of all supported states and their properties
+
+        :param: country: The country code from which to obtain the list of supported states
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {"country": country}
+        return await self._get_request("/address_verification/states", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/payment_pages.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/payment_pages.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-"""
-Wrapper for Paystack Payment Pages API.
-
-The Payment Pages API provides a quick and secure way to collect payment for products.
-"""
-
-from datetime import date
-from typing import Optional, Dict, List, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-
-
-class PaymentPagesClientAPI(SyncRequestAPI):
-    """
-    Paystack Payment Pages API
-    Reference: https://paystack.com/docs/api/page/
-    """
-
-    def create_payment_page(
-            self,
-            name: str,
-            description: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            page_slug: Optional[Union[str, None]] = None,
-            redirect_url: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-            custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a payment page
-
-        :param: name: Name of the page
-        :param: description: Description of the page
-        :param: amount: Amount of the page
-        :param: split_code: Split code of the transaction split
-        :param: page_slug: URL slug you would like to be associated with this page.
-        
-        note::
-
-            Page will be accessible at https://paystack.com/pay/page_slug
-
-        :param: redirect_url: If you would like Paystack to redirect someplace
-                                upon successful payment, specify the URL here.
-        :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
-        :param: custom_fields: If you would like to accept custom fields, specify them here.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "name": name,
-            "description": description,
-            "amount": amount,
-            "split_code": split_code,
-            "slug": page_slug,
-            "redirect_url": redirect_url,
-            "metadata": metadata,
-            "custom_fields": custom_fields,
-        }
-        return self._post_request("/page", data=data)
-
-    def list_payment_pages(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the payment pages
-
-        :param: per_page: Number of records to return
-        :param: page: number to return
-        :param: from_date: A timestamp from which to start listing page
-        :param: to_date: A timestamp from which to start listing page
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-
-        note::
-            Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/page", params=params)
-
-    def fetch_payment_page(self, page_id_or_slug: str) -> PayStackResponse:
-        """
-        Get details of a payment page
-
-        :param: page_id_or_slug: ID or slug of the payment page
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/page/{page_id_or_slug}")
-
-    def update_payment_page(
-            self,
-            page_id_or_slug: str,
-            name: Optional[Union[str, None]] = None,
-            description: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            active: Optional[Union[bool, None]] = True,
-    ) -> PayStackResponse:
-        """
-        Update a payment page detail
-
-        :param: page_id_or_slug: ID or slug of the payment page
-        :param: name: Name of the page
-        :param: description: Description of the page
-        :param: amount: Amount of the page
-        :param: active: Set false to deactivate the page url
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "name": name,
-            "description": description,
-            "amount": amount,
-            "active": active,
-        }
-        return self._put_request(f"/page/{page_id_or_slug}", data=data)
-
-    def check_slug_available(self, page_slug: str) -> PayStackResponse:
-        """
-        Check if a slug is available
-
-        :param: page_slug: URL slug you would like to be associated with this page.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/page/check_slug_availability/{page_slug}")
-
-    def add_products(self, payment_id: int, product: List[int]) -> PayStackResponse:
-        """
-        Add products to a payment page
-
-        :param: payment_id: ID of the payment page
-        :param: product: List of IDS of all the products
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"product": product}
-        return self._post_request(f"/page/{payment_id}/product", data=data)
+"""
+Wrapper for Paystack Payment Pages API.
+
+The Payment Pages API provides a quick and secure way to collect payment for products.
+"""
+
+from datetime import date
+from typing import Optional, Dict, List, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class PaymentPagesClientAPI(SyncRequestAPI):
+    """
+    Paystack Payment Pages API
+    Reference: https://paystack.com/docs/api/page/
+    """
+
+    def create_payment_page(
+            self,
+            name: str,
+            description: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            page_slug: Optional[Union[str, None]] = None,
+            redirect_url: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+            custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a payment page
+
+        :param: name: Name of the page
+        :param: description: Description of the page
+        :param: amount: Amount of the page
+        :param: split_code: Split code of the transaction split
+        :param: page_slug: URL slug you would like to be associated with this page.
+        
+        note::
+
+            Page will be accessible at https://paystack.com/pay/page_slug
+
+        :param: redirect_url: If you would like Paystack to redirect someplace
+                                upon successful payment, specify the URL here.
+        :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
+        :param: custom_fields: If you would like to accept custom fields, specify them here.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "name": name,
+            "description": description,
+            "amount": amount,
+            "split_code": split_code,
+            "slug": page_slug,
+            "redirect_url": redirect_url,
+            "metadata": metadata,
+            "custom_fields": custom_fields,
+        }
+        return self._post_request("/page", data=data)
+
+    def list_payment_pages(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the payment pages
+
+        :param: per_page: Number of records to return
+        :param: page: number to return
+        :param: from_date: A timestamp from which to start listing page
+        :param: to_date: A timestamp from which to start listing page
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+
+        note::
+            Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return self._get_request("/page", params=params)
+
+    def fetch_payment_page(self, page_id_or_slug: str) -> PayStackResponse:
+        """
+        Get details of a payment page
+
+        :param: page_id_or_slug: ID or slug of the payment page
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/page/{page_id_or_slug}")
+
+    def update_payment_page(
+            self,
+            page_id_or_slug: str,
+            name: Optional[Union[str, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+    ) -> PayStackResponse:
+        """
+        Update a payment page detail
+
+        :param: page_id_or_slug: ID or slug of the payment page
+        :param: name: Name of the page
+        :param: description: Description of the page
+        :param: amount: Amount of the page
+        :param: active: Set false to deactivate the page url
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        active = self._convert_to_string(active)
+
+        data = {
+            "name": name,
+            "description": description,
+            "amount": amount,
+            "active": active,
+        }
+        return self._put_request(f"/page/{page_id_or_slug}", data=data)
+
+    def check_slug_available(self, page_slug: str) -> PayStackResponse:
+        """
+        Check if a slug is available
+
+        :param: page_slug: URL slug you would like to be associated with this page.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/page/check_slug_availability/{page_slug}")
+
+    def add_products(self, payment_id: int, product: List[int]) -> PayStackResponse:
+        """
+        Add products to a payment page
+
+        :param: payment_id: ID of the payment page
+        :param: product: List of IDS of all the products
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"product": product}
+        return self._post_request(f"/page/{payment_id}/product", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/payment_requests.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/payment_requests.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-"""
-Wrapper for Paystack Payment Requests API.
-
-The Payment Requests API allows you manage requests for payment of goods and services.
-"""
-
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import PayMentRequestStatus, Currency
-
-
-class PaymentRequestClientAPI(SyncRequestAPI):
-    """
-    Paystack Payment Request API
-    Reference: https://paystack.com/docs/api/payment-request/
-    """
-
-    def create_payment_request(
-            self,
-            customer: str,
-            amount: int,
-            draft: bool,
-            has_invoice: bool,
-            send_notification: bool,
-            due_date: Optional[Union[date, None]] = None,
-            description: Optional[Union[str, Any]] = None,
-            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
-            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
-            currency: Optional[Union[Currency, Any]] = None,
-            invoice_number: Optional[Union[int, Any]] = None,
-            split_code: Optional[Union[str, Any]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a payment request for a transaction
-
-        :param: customer: Customer ID of the customer
-        :param: amount: Amount of the payment request
-        :param: due_date: Due date of the payment request
-        :param: description: Description of the payment request
-        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
-        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
-        :param: currency: Currency of the payment request
-        :param: send_notification: Set true if you want to send a notification to the customer email
-        :param: draft: Set true if you want to create a draft payment request
-        :param: has_invoice: Set true if you want to create a draft payment request
-        :param: invoice_number: Invoice number of the payment request
-        :param: split_code: split code of the transaction split
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert date and bool to string
-        due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        has_invoice = self._convert_to_string(has_invoice)
-        send_notification = self._convert_to_string(send_notification)
-
-        data = {
-            "customer": customer,
-            "amount": amount,
-            "due_date": due_date,
-            "description": description,
-            "line_items": line_items,
-            "tax": tax,
-            "currency": currency,
-            "send_notification": send_notification,
-            "draft": draft,
-            "has_invoice": has_invoice,
-            "invoice_number": invoice_number,
-            "split_code": split_code,
-        }
-        return self._post_request("/paymentrequest", data=data)
-
-    def list_payment_requests(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[str, None]] = None,
-            status: Optional[Union[PayMentRequestStatus, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            include_archive: Optional[Union[bool, None]] = True,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the payment requests
-
-        :param: per_page: Number of records to return
-        :param: page:  number to return
-        :param: customer: Filter by customer ID
-        :param: status: Filter by payment request status
-        :param: currency:
-        :param: include_archive: Show archived payment requests
-        :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
-        :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-        include_archive = self._convert_to_string(include_archive)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "status": status,
-            "currency": currency,
-            "include_archive": include_archive,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/paymentrequest", params=params)
-
-    def fetch_payment_request(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a payment request on your integration
-
-        :param: id_or_code: ID or Code of the payment request
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/paymentrequest/{id_or_code}")
-
-    def verify_payment_request(self, code: str) -> PayStackResponse:
-        """
-        Verify details of a payment request on your integration
-
-        :param: code: Payment request code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/paymentrequest/verify/{code}")
-
-    def send_notification(self, code: str) -> PayStackResponse:
-        """
-        Send notification of a payment request to a customer
-
-        :param: code: Payment request code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request(f"/paymentrequest/notify/{code}")
-
-    def payment_request_total(self) -> PayStackResponse:
-        """
-        Get total of a payment request metric
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request("/paymentrequest/totals")
-
-    def finalize_payment_request(self, code: str, send_notification: bool) -> PayStackResponse:
-        """
-        Finalize a draft payment request
-
-        :param: code: Payment request code
-        :param: send_notification: Set true if you want to send a notification to the customer email
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        send_notification = self._convert_to_string(send_notification)
-
-        data = {"send_notification": send_notification}
-        return self._post_request(f"/paymentrequest/finalize/{code}", data=data)
-
-    def update_payment_request(
-            self,
-            id_or_code: str,
-            customer: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            description: Optional[Union[str, None]] = None,
-            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
-            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            due_date: Optional[Union[date, None]] = None,
-            send_notification: Optional[Union[bool, None]] = True,
-            draft: Optional[Union[bool, None]] = True,
-            invoice_number: Optional[Union[int, None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a payment request
-
-        :param: id_or_code: ID or Code of the payment request
-        :param: customer: Customer ID or code of the customer
-        :param: amount: Amount of the payment request
-        :param: due_date: Due date of the payment request
-        :param: description: Description of the payment request
-        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
-        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
-        :param: currency: Currency of the payment request
-        :param: send_notification: Set true if you want to send a notification to the customer email
-        :param: draft: Set true if you want to create a draft payment request
-        :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
-        :param: split_code: split code of the transaction split
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date and bool to string
-        due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        send_notification = self._convert_to_string(send_notification)
-
-        data = {
-            "customer": customer,
-            "amount": amount,
-            "due_date": due_date,
-            "description": description,
-            "line_items": line_items,
-            "tax": tax,
-            "currency": currency,
-            "send_notification": send_notification,
-            "draft": draft,
-            "invoice_number": invoice_number,
-            "split_code": split_code,
-        }
-        return self._put_request(f"/paymentrequest/{id_or_code}", data=data)
-
-    def archive_payment_request(self, code: str) -> PayStackResponse:
-        """
-        Archive a payment request
-
-        :param: code: Payment request code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request(f"/paymentrequest/archive/{code}")
+"""
+Wrapper for Paystack Payment Requests API.
+
+The Payment Requests API allows you manage requests for payment of goods and services.
+"""
+
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import PayMentRequestStatus, Currency
+
+
+class PaymentRequestClientAPI(SyncRequestAPI):
+    """
+    Paystack Payment Request API
+    Reference: https://paystack.com/docs/api/payment-request/
+    """
+
+    def create_payment_request(
+            self,
+            customer: str,
+            amount: int,
+            draft: bool,
+            has_invoice: bool,
+            send_notification: bool,
+            due_date: Optional[Union[date, None]] = None,
+            description: Optional[Union[str, Any]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, Any]] = None,
+            invoice_number: Optional[Union[int, Any]] = None,
+            split_code: Optional[Union[str, Any]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a payment request for a transaction
+
+        :param: customer: Customer ID of the customer
+        :param: amount: Amount of the payment request
+        :param: due_date: Due date of the payment request
+        :param: description: Description of the payment request
+        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
+        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
+        :param: currency: Currency of the payment request
+        :param: send_notification: Set true if you want to send a notification to the customer email
+        :param: draft: Set true if you want to create a draft payment request
+        :param: has_invoice: Set true if you want to create a draft payment request
+        :param: invoice_number: Invoice number of the payment request
+        :param: split_code: split code of the transaction split
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert date and bool to string
+        due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        has_invoice = self._convert_to_string(has_invoice)
+        send_notification = self._convert_to_string(send_notification)
+
+        data = {
+            "customer": customer,
+            "amount": amount,
+            "due_date": due_date,
+            "description": description,
+            "line_items": line_items,
+            "tax": tax,
+            "currency": currency,
+            "send_notification": send_notification,
+            "draft": draft,
+            "has_invoice": has_invoice,
+            "invoice_number": invoice_number,
+            "split_code": split_code,
+        }
+        return self._post_request("/paymentrequest", data=data)
+
+    def list_payment_requests(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[str, None]] = None,
+            status: Optional[Union[PayMentRequestStatus, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            include_archive: Optional[Union[bool, None]] = True,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the payment requests
+
+        :param: per_page: Number of records to return
+        :param: page:  number to return
+        :param: customer: Filter by customer ID
+        :param: status: Filter by payment request status
+        :param: currency:
+        :param: include_archive: Show archived payment requests
+        :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
+        :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+        include_archive = self._convert_to_string(include_archive)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "status": status,
+            "currency": currency,
+            "include_archive": include_archive,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/paymentrequest", params=params)
+
+    def fetch_payment_request(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a payment request on your integration
+
+        :param: id_or_code: ID or Code of the payment request
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/paymentrequest/{id_or_code}")
+
+    def verify_payment_request(self, code: str) -> PayStackResponse:
+        """
+        Verify details of a payment request on your integration
+
+        :param: code: Payment request code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/paymentrequest/verify/{code}")
+
+    def send_notification(self, code: str) -> PayStackResponse:
+        """
+        Send notification of a payment request to a customer
+
+        :param: code: Payment request code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request(f"/paymentrequest/notify/{code}")
+
+    def payment_request_total(self) -> PayStackResponse:
+        """
+        Get total of a payment request metric
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request("/paymentrequest/totals")
+
+    def finalize_payment_request(self, code: str, send_notification: bool) -> PayStackResponse:
+        """
+        Finalize a draft payment request
+
+        :param: code: Payment request code
+        :param: send_notification: Set true if you want to send a notification to the customer email
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        send_notification = self._convert_to_string(send_notification)
+
+        data = {"send_notification": send_notification}
+        return self._post_request(f"/paymentrequest/finalize/{code}", data=data)
+
+    def update_payment_request(
+            self,
+            id_or_code: str,
+            customer: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            due_date: Optional[Union[date, None]] = None,
+            send_notification: Optional[Union[bool, None]] = True,
+            draft: Optional[Union[bool, None]] = True,
+            invoice_number: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a payment request
+
+        :param: id_or_code: ID or Code of the payment request
+        :param: customer: Customer ID or code of the customer
+        :param: amount: Amount of the payment request
+        :param: due_date: Due date of the payment request
+        :param: description: Description of the payment request
+        :param: line_items: Array of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
+        :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
+        :param: currency: Currency of the payment request
+        :param: send_notification: Set true if you want to send a notification to the customer email
+        :param: draft: Set true if you want to create a draft payment request
+        :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
+        :param: split_code: split code of the transaction split
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date and bool to string
+        due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        send_notification = self._convert_to_string(send_notification)
+
+        data = {
+            "customer": customer,
+            "amount": amount,
+            "due_date": due_date,
+            "description": description,
+            "line_items": line_items,
+            "tax": tax,
+            "currency": currency,
+            "send_notification": send_notification,
+            "draft": draft,
+            "invoice_number": invoice_number,
+            "split_code": split_code,
+        }
+        return self._put_request(f"/paymentrequest/{id_or_code}", data=data)
+
+    def archive_payment_request(self, code: str) -> PayStackResponse:
+        """
+        Archive a payment request
+
+        :param: code: Payment request code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request(f"/paymentrequest/archive/{code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/plans.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/plans.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""
-Wrapper for Paystack Plans API
-
-The Plans API allows you to create and manage installment payment options on your integration.
-"""
-
-from typing import Optional, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import Interval
-
-
-class PlanClientAPI(SyncRequestAPI):
-    """
-    Paystack Plan API
-    Reference: https://paystack.com/docs/api/plan/
-    """
-
-    def create_plan(
-            self,
-            name: str,
-            amount: int,
-            interval: Interval,
-            currency: str,
-            invoice_limit: int,
-            send_invoices: bool,
-            send_sms: bool,
-            description: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a plan
-
-        :param: name: Name of the plan
-        :param: amount: Amount of the plan
-        :param: interval: Interval of the plan. Values [Interval.value.value]
-        :param: description: Description of the plan
-        :param: send_invoices: Send invoices to customer
-        :param: send_sms: Send SMS to customer
-        :param: currency: Currency of the plan
-        :param: invoice_limit: Invoice limit of the plan
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
-        data = {
-            "name": name,
-            "amount": amount,
-            "interval": interval,
-            "description": description,
-            "send_invoices": send_invoices,
-            "send_sms": send_sms,
-            "currency": currency,
-            "invoice_limit": invoice_limit,
-        }
-        return self._post_request("/plan", data=data)
-
-    def list_plans(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            status: Optional[Union[str, None]] = None,
-            interval: Optional[Union[Interval, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the plans
-
-        :param: per_page: Number of records to return
-        :param: page:  number to return
-        :param: status: Filter list by plans with specified status
-        :param: interval: Filter list by plans with specified interval
-        :param: amount
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "status": status,
-            "interval": interval,
-            "amount": amount,
-        }
-        return self._get_request("/plan", params=params)
-
-    def fetch_plan(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a plan
-
-        :param: id_or_code: ID or Code of the plan
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/plan/{id_or_code}")
-
-    def update_plan(
-            self,
-            id_or_code: str,
-            name: str,
-            amount: int,
-            interval: Interval,
-            send_invoices: bool,
-            send_sms: bool,
-            currency: str,
-            invoice_limit: int,
-            description: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a plan detail
-
-        :param: id_or_code: ID or Code of the plan
-        :param: name: Name of the plan
-        :param: amount: Amount of the plan
-        :param: interval: Interval of the plan. [Interval.value.value]
-        :param: description:
-        :param: send_invoices:
-        :param: send_sms:
-        :param: currency:
-        :param: invoice_limit:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
-        data = {
-            "name": name,
-            "amount": amount,
-            "interval": interval,
-            "description": description,
-            "send_invoices": send_invoices,
-            "send_sms": send_sms,
-            "currency": currency,
-            "invoice_limit": invoice_limit,
-        }
-        return self._put_request(f"/plan/{id_or_code}", data=data)
+"""
+Wrapper for Paystack Plans API
+
+The Plans API allows you to create and manage installment payment options on your integration.
+"""
+
+from typing import Optional, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Interval
+
+
+class PlanClientAPI(SyncRequestAPI):
+    """
+    Paystack Plan API
+    Reference: https://paystack.com/docs/api/plan/
+    """
+
+    def create_plan(
+            self,
+            name: str,
+            amount: int,
+            interval: Interval,
+            currency: str,
+            invoice_limit: int,
+            send_invoices: bool,
+            send_sms: bool,
+            description: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a plan
+
+        :param: name: Name of the plan
+        :param: amount: Amount of the plan
+        :param: interval: Interval of the plan. Values [Interval.value.value]
+        :param: description: Description of the plan
+        :param: send_invoices: Send invoices to customer
+        :param: send_sms: Send SMS to customer
+        :param: currency: Currency of the plan
+        :param: invoice_limit: Invoice limit of the plan
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        send_invoices = self._convert_to_string(send_invoices)
+        send_sms = self._convert_to_string(send_sms)
+
+        data = {
+            "name": name,
+            "amount": amount,
+            "interval": interval,
+            "description": description,
+            "send_invoices": send_invoices,
+            "send_sms": send_sms,
+            "currency": currency,
+            "invoice_limit": invoice_limit,
+        }
+        return self._post_request("/plan", data=data)
+
+    def list_plans(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            status: Optional[Union[str, None]] = None,
+            interval: Optional[Union[Interval, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the plans
+
+        :param: per_page: Number of records to return
+        :param: page:  number to return
+        :param: status: Filter list by plans with specified status
+        :param: interval: Filter list by plans with specified interval
+        :param: amount
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "status": status,
+            "interval": interval,
+            "amount": amount,
+        }
+        return self._get_request("/plan", params=params)
+
+    def fetch_plan(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a plan
+
+        :param: id_or_code: ID or Code of the plan
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/plan/{id_or_code}")
+
+    def update_plan(
+            self,
+            id_or_code: str,
+            name: str,
+            amount: int,
+            interval: Interval,
+            send_invoices: bool,
+            send_sms: bool,
+            currency: str,
+            invoice_limit: int,
+            description: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a plan detail
+
+        :param: id_or_code: ID or Code of the plan
+        :param: name: Name of the plan
+        :param: amount: Amount of the plan
+        :param: interval: Interval of the plan. [Interval.value.value]
+        :param: description:
+        :param: send_invoices:
+        :param: send_sms:
+        :param: currency:
+        :param: invoice_limit:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        # convert to strings
+        send_invoices = self._convert_to_string(send_invoices)
+        send_sms = self._convert_to_string(send_sms)
+
+        data = {
+            "name": name,
+            "amount": amount,
+            "interval": interval,
+            "description": description,
+            "send_invoices": send_invoices,
+            "send_sms": send_sms,
+            "currency": currency,
+            "invoice_limit": invoice_limit,
+        }
+        return self._put_request(f"/plan/{id_or_code}", data=data)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/subaccounts.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/subaccounts.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-"""
-Wrapper for Paystack SubAccounts API
-
-The Subaccounts API allows you to create and manage subaccounts on your integration.
-Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
-"""
-
-from datetime import date
-from typing import Optional, Dict, List, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import SettlementSchedule
-
-
-class SubAccountClientAPI(SyncRequestAPI):
-    """
-    Paystack SubAccount API
-    Reference: https://paystack.com/docs/api/subaccount/
-    """
-
-    def create_subaccount(
-            self,
-            business_name: str,
-            settlement_bank: str,
-            account_number: str,
-            percentage_charge: float,
-            description: str,
-            primary_contact_email: Optional[Union[str, None]] = None,
-            primary_contact_name: Optional[Union[str, None]] = None,
-            primary_contact_phone: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a subaccount
-
-        :param: business_name: The business name of the subaccount.
-        :param: settlement_bank: Bank Code for the bank
-        :param: account_number: The account number of the subaccount.
-        :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
-        :param: description: The description of the subaccount.
-        :param: primary_contact_email: A contact email for the subaccount
-        :param: primary_contact_name: A name for the contact person for this subaccount
-        :param: primary_contact_phone: A phone number to call for this subaccount
-        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "business_name": business_name,
-            "settlement_bank": settlement_bank,
-            "account_number": account_number,
-            "percentage_charge": percentage_charge,
-            "description": description,
-            "primary_contact_email": primary_contact_email,
-            "primary_contact_name": primary_contact_name,
-            "primary_contact_phone": primary_contact_phone,
-            "metadata": metadata,
-        }
-        return self._post_request("/subaccount", data=data)
-
-    def update_subaccount(
-            self,
-            id_or_code: str,
-            business_name: str,
-            settlement_bank: str,
-            account_number: str,
-            active: Optional[Union[bool, None]] = True,
-            percentage_charge: Optional[Union[float, None]] = None,
-            description: Optional[Union[str, None]] = None,
-            primary_contact_email: Optional[Union[str, None]] = None,
-            primary_contact_name: Optional[Union[str, None]] = None,
-            primary_contact_phone: Optional[Union[str, None]] = None,
-            settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a subaccount
-
-        :param: id_or_code: The id or code of the subaccount.
-        :param: business_name: The business name of the subaccount.
-        :param: settlement_bank: The settlement bank of the subaccount.
-        :param: account_number
-        :param: active: [ True or False ]
-        :param: percentage_charge
-        :param: description
-        :param: primary_contact_email
-        :param: primary_contact_name
-        :param: primary_contact_phone
-        :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
-
-        note::
-            Auto means payout is T+1
-            Manual means payout to the subaccount should only be made when requested. Defaults to auto
-
-        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "business_name": business_name,
-            "settlement_bank": settlement_bank,
-            "account_number": account_number,
-            "active": active,
-            "percentage_charge": percentage_charge,
-            "description": description,
-            "primary_contact_email": primary_contact_email,
-            "primary_contact_name": primary_contact_name,
-            "primary_contact_phone": primary_contact_phone,
-            "settlement_schedule": settlement_schedule,
-            "metadata": metadata,
-        }
-        return self._put_request(f"/subaccount/{id_or_code}", data=data)
-
-    def list_subaccounts(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all subaccounts
-
-        :param: per_page: The number of records to return per page.
-        :param: page: The number to retrieve.
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/subaccount", params=params)
-
-    def fetch_subaccount(self, id_or_code: str) -> PayStackResponse:
-        """
-        Fetch details of a specific subaccount
-
-        :param: id_or_code: The id or code of the subaccount.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/subaccount/{id_or_code}")
+"""
+Wrapper for Paystack SubAccounts API
+
+The Subaccounts API allows you to create and manage subaccounts on your integration.
+Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
+"""
+
+from datetime import date
+from typing import Optional, Dict, List, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import SettlementSchedule
+
+
+class SubAccountClientAPI(SyncRequestAPI):
+    """
+    Paystack SubAccount API
+    Reference: https://paystack.com/docs/api/subaccount/
+    """
+
+    def create_subaccount(
+            self,
+            business_name: str,
+            settlement_bank: str,
+            account_number: str,
+            percentage_charge: float,
+            description: str,
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a subaccount
+
+        :param: business_name: The business name of the subaccount.
+        :param: settlement_bank: Bank Code for the bank
+        :param: account_number: The account number of the subaccount.
+        :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
+        :param: description: The description of the subaccount.
+        :param: primary_contact_email: A contact email for the subaccount
+        :param: primary_contact_name: A name for the contact person for this subaccount
+        :param: primary_contact_phone: A phone number to call for this subaccount
+        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "business_name": business_name,
+            "settlement_bank": settlement_bank,
+            "account_number": account_number,
+            "percentage_charge": percentage_charge,
+            "description": description,
+            "primary_contact_email": primary_contact_email,
+            "primary_contact_name": primary_contact_name,
+            "primary_contact_phone": primary_contact_phone,
+            "metadata": metadata,
+        }
+        return self._post_request("/subaccount", data=data)
+
+    def update_subaccount(
+            self,
+            id_or_code: str,
+            business_name: str,
+            settlement_bank: str,
+            account_number: str,
+            active: Optional[Union[bool, None]] = True,
+            percentage_charge: Optional[Union[float, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a subaccount
+
+        :param: id_or_code: The id or code of the subaccount.
+        :param: business_name: The business name of the subaccount.
+        :param: settlement_bank: The settlement bank of the subaccount.
+        :param: account_number
+        :param: active: [ True or False ]
+        :param: percentage_charge
+        :param: description
+        :param: primary_contact_email
+        :param: primary_contact_name
+        :param: primary_contact_phone
+        :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
+
+        note::
+            Auto means payout is T+1
+            Manual means payout to the subaccount should only be made when requested. Defaults to auto
+
+        :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        active = self._convert_to_string(active)
+
+        data = {
+            "business_name": business_name,
+            "settlement_bank": settlement_bank,
+            "account_number": account_number,
+            "active": active,
+            "percentage_charge": percentage_charge,
+            "description": description,
+            "primary_contact_email": primary_contact_email,
+            "primary_contact_name": primary_contact_name,
+            "primary_contact_phone": primary_contact_phone,
+            "settlement_schedule": settlement_schedule,
+            "metadata": metadata,
+        }
+        return self._put_request(f"/subaccount/{id_or_code}", data=data)
+
+    def list_subaccounts(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all subaccounts
+
+        :param: per_page: The number of records to return per page.
+        :param: page: The number to retrieve.
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return self._get_request("/subaccount", params=params)
+
+    def fetch_subaccount(self, id_or_code: str) -> PayStackResponse:
+        """
+        Fetch details of a specific subaccount
+
+        :param: id_or_code: The id or code of the subaccount.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/subaccount/{id_or_code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/subscriptions.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/subscriptions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""
-Wrapper for Paystack Subscriptions API
-
-The Subscriptions API allows you to create and manage recurring payment on your integration.
-"""
-
-from datetime import date
-from typing import Optional, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-
-
-class SubscriptionClientAPI(SyncRequestAPI):
-    """
-    Paystack Subscription API
-    Reference: https://paystack.com/docs/api/subscription/
-    """
-
-    def create_subscription(
-            self,
-            customer: str,
-            plan_code: str,
-            authorization: str,
-            start_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a subscription
-
-        :param: customer: Email or Code of the customer
-        :param: plan_code: Code of the plan
-        :param: authorization: Code of the authorization
-        :param: start_date: Start date of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        start_date = self._convert_to_string(start_date)
-
-        data = {
-            "customer": customer,
-            "plan": plan_code,
-            "authorization": authorization,
-            "start_date": start_date,
-        }
-        return self._post_request("/subscription", data=data)
-
-    def list_subscriptions(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[int, None]] = None,
-            plan_code: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the subscriptions
-
-        :param: per_page: Number of records to return per page.
-        :param: page: THe number to return
-        :param: customer:
-        :param: plan_code:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "plan": plan_code,
-        }
-        return self._get_request("/subscription", params=params)
-
-    def fetch_subscription(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a subscription
-
-        :param: id_or_code: ID or Code of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/subscription/{id_or_code}")
-
-    def enable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
-        """
-        Enable a subscription
-
-        :param: subscription_code: Code of the subscription
-        :param: token: Email token of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"code": subscription_code, "token": token}
-        return self._post_request("/subscription/enable", data=data)
-
-    def disable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
-        """
-        Disable a subscription
-
-        :param: subscription_code: Code of the subscription
-        :param: token: Email token of the customer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"code": subscription_code, "token": token}
-        return self._post_request("/subscription/disable", data=data)
-
-    def generate_update_subscription(self, subscription_code: str) -> PayStackResponse:
-        """
-        Generate a link for updating the card on subscription
-
-        :param: subscription_code: Code of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request(f"/subscription/{subscription_code}/manage/link")
-
-    def send_update_subscription_link(self, subscription_code: str) -> PayStackResponse:
-        """
-        Email a customer a link for updating the card on their subscription
-
-        :param: subscription_code: Code of the subscription
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request(f"/subscription/{subscription_code}/manage/email")
+"""
+Wrapper for Paystack Subscriptions API
+
+The Subscriptions API allows you to create and manage recurring payment on your integration.
+"""
+
+from datetime import date
+from typing import Optional, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class SubscriptionClientAPI(SyncRequestAPI):
+    """
+    Paystack Subscription API
+    Reference: https://paystack.com/docs/api/subscription/
+    """
+
+    def create_subscription(
+            self,
+            customer: str,
+            plan_code: str,
+            authorization: str,
+            start_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a subscription
+
+        :param: customer: Email or Code of the customer
+        :param: plan_code: Code of the plan
+        :param: authorization: Code of the authorization
+        :param: start_date: Start date of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        start_date = self._convert_to_string(start_date)
+
+        data = {
+            "customer": customer,
+            "plan": plan_code,
+            "authorization": authorization,
+            "start_date": start_date,
+        }
+        return self._post_request("/subscription", data=data)
+
+    def list_subscriptions(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            plan_code: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the subscriptions
+
+        :param: per_page: Number of records to return per page.
+        :param: page: THe number to return
+        :param: customer:
+        :param: plan_code:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "plan": plan_code,
+        }
+        return self._get_request("/subscription", params=params)
+
+    def fetch_subscription(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a subscription
+
+        :param: id_or_code: ID or Code of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/subscription/{id_or_code}")
+
+    def enable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
+        """
+        Enable a subscription
+
+        :param: subscription_code: Code of the subscription
+        :param: token: Email token of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"code": subscription_code, "token": token}
+        return self._post_request("/subscription/enable", data=data)
+
+    def disable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
+        """
+        Disable a subscription
+
+        :param: subscription_code: Code of the subscription
+        :param: token: Email token of the customer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"code": subscription_code, "token": token}
+        return self._post_request("/subscription/disable", data=data)
+
+    def generate_update_subscription(self, subscription_code: str) -> PayStackResponse:
+        """
+        Generate a link for updating the card on subscription
+
+        :param: subscription_code: Code of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request(f"/subscription/{subscription_code}/manage/link")
+
+    def send_update_subscription_link(self, subscription_code: str) -> PayStackResponse:
+        """
+        Email a customer a link for updating the card on their subscription
+
+        :param: subscription_code: Code of the subscription
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request(f"/subscription/{subscription_code}/manage/email")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/transaction_splits.py` & `paystackease-2.0.4/paystackease/apis/async_apis/atransaction_splits.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,165 @@
-"""
-Wrapper for Paystack Transaction Splits APIs
-
-The Transaction Splits API enables merchants split the settlement for a transaction
-across their payout account, and one or more subaccounts.
-"""
-
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import Currency
-
-
-class TransactionSplitClientAPI(SyncRequestAPI):
-    """
-    Paystack Transaction Split API
-    Reference: https://paystack.com/docs/api/split/
-    """
-
-    def create_split(
-            self,
-            transaction_split_name: str,
-            transaction_split_type: str,
-            currency: Currency,
-            subaccounts: List[Dict[str, Any]],
-            bearer_type: str,
-            bearer_subaccount: str,
-    ) -> PayStackResponse:
-        """
-        Create a split payment on your integration
-
-        :param: transaction_split_name: Name of the transaction split
-        :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
-        :param: currency: [ Currency.value.value ]
-        :param: subaccounts: A list of object containing subaccount code and number of shares
-                            [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
-        :param: bearer_type: Any of subaccount | account | all-proportional | all
-        :param: bearer_subaccount: Subaccount code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "name": transaction_split_name,
-            "type": transaction_split_type,
-            "currency": currency,
-            "subaccounts": subaccounts,
-            "bearer_type": bearer_type,
-            "bearer_subaccount": bearer_subaccount,
-        }
-        return self._post_request("/split", data=data)
-
-    def add_or_update_subaccount_split(
-            self, split_id: str, subaccount: str, transaction_share: int
-    ) -> PayStackResponse:
-        """
-        Add a Subaccount to a Transaction Split, or update the share of
-        an existing Subaccount in a Transaction Split
-
-        :param: split_id: The split ID
-        :param: subaccount: The subaccount code
-        :param: transaction_share: The number of shares
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"subaccount": subaccount, "share": transaction_share}
-        return self._post_request(f"/split/{split_id}/subaccount/add", data=data)
-
-    def remove_sub_account_split(self, split_id: str, subaccount: str) -> PayStackResponse:
-        """
-        Remove a Sub Account from a transaction split
-
-        :param: split_id: The split ID
-        :param: subaccount: The subaccount code
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"subaccount": subaccount}
-        return self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
-
-    def update_split(
-            self,
-            split_id: str,
-            transaction_split_name: str,
-            active: bool,
-            bearer_type: Optional[Union[str, None]] = None,
-            bearer_subaccount: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a specific transaction split details
-
-        :param: split_id: The split ID
-        :param: transaction_split_name: Name of the transaction split
-        :param: active: True or False
-        :param: bearer_type:
-        :param: bearer_subaccount:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "name": transaction_split_name,
-            "active": active,
-            "bearer_type": bearer_type,
-            "bearer_subaccount": bearer_subaccount,
-        }
-        return self._put_request(f"/split/{split_id}", data=data)
-
-    def list_split(
-            self,
-            split_name: Optional[Union[str, None]] = None,
-            active: Optional[Union[bool, None]] = True,
-            sort_by: Optional[Union[str, None]] = None,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all the transaction splits
-
-        :param: split_name: Name of the transaction split
-        :param: active: True or False
-        :param: sort_by: Sort by name, defaults to createdAt date,
-        :param: per_page:
-        :param: page:
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date and bool to string
-        active = self._convert_to_string(active)
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "name": split_name,
-            "active": active,
-            "sort_by": sort_by,
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/split", params=params)
-
-    def fetch_split(self, split_id: str) -> PayStackResponse:
-        """
-        Fetch details of a specific transaction split
-
-        :param: split_id: The split ID
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/split/{split_id}")
+"""
+Wrapper for Asynchronous Paystack Transaction Splits APIs
+
+The Transaction Splits API enables merchants split the settlement for a transaction
+across their payout account, and one or more subaccounts.
+"""
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
+
+
+class AsyncTransactionSplitClientAPI(AsyncRequestAPI):
+    """
+    Paystack Transaction Split API
+    Reference: https://paystack.com/docs/api/split/
+    """
+
+    async def create_split(
+            self,
+            transaction_split_name: str,
+            transaction_split_type: str,
+            currency: Currency,
+            subaccounts: List[Dict[str, Any]],
+            bearer_type: str,
+            bearer_subaccount: str,
+    ) -> PayStackResponse:
+        """
+        Create a split payment on your integration
+
+        :param: transaction_split_name: Name of the transaction split
+        :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
+        :param: currency: [ Currency.value.value ]
+        :param: subaccounts: A list of object containing subaccount code and number of shares
+                            [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
+        :param: bearer_type: Any of subaccount | account | all-proportional | all
+        :param: bearer_subaccount: Subaccount code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "name": transaction_split_name,
+            "type": transaction_split_type,
+            "currency": currency,
+            "subaccounts": subaccounts,
+            "bearer_type": bearer_type,
+            "bearer_subaccount": bearer_subaccount,
+        }
+        return await self._post_request("/split", data=data)
+
+    async def add_or_update_subaccount_split(
+            self, split_id: str, subaccount: str, transaction_share: int
+    ) -> PayStackResponse:
+        """
+        Add a Subaccount to a Transaction Split, or update the share of
+        an existing Subaccount in a Transaction Split
+
+        :param: split_id: The split ID
+        :param: subaccount: The subaccount code
+        :param: transaction_share: The number of shares
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"subaccount": subaccount, "share": transaction_share}
+        return await self._post_request(f"/split/{split_id}/subaccount/add", data=data)
+
+    async def remove_sub_account_split(self, split_id: str, subaccount: str) -> PayStackResponse:
+        """
+        Remove a Sub Account from a transaction split
+
+        :param: split_id: The split ID
+        :param: subaccount: The subaccount code
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"subaccount": subaccount}
+        return await self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
+
+    async def update_split(
+            self,
+            split_id: str,
+            transaction_split_name: str,
+            active: bool,
+            bearer_type: Optional[Union[str, None]] = None,
+            bearer_subaccount: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a specific transaction split details
+
+        :param: split_id: The split ID
+        :param: transaction_split_name: Name of the transaction split
+        :param: active: True or False
+        :param: bearer_type:
+        :param: bearer_subaccount:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        active = self._convert_to_string(active)
+
+        data = {
+            "name": transaction_split_name,
+            "active": active,
+            "bearer_type": bearer_type,
+            "bearer_subaccount": bearer_subaccount,
+        }
+        return await self._put_request(f"/split/{split_id}", data=data)
+
+    async def list_split(
+            self,
+            split_name: Optional[Union[str, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+            sort_by: Optional[Union[str, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all the transaction splits
+
+        :param: split_name: Name of the transaction split
+        :param: active: True or False
+        :param: sort_by: Sort by name, async defaults to createdAt date,
+        :param: per_page:
+        :param: page:
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date and bool to string
+        active = self._convert_to_string(active)
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "name": split_name,
+            "active": active,
+            "sort_by": sort_by,
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/split", params=params)
+
+    async def fetch_split(self, split_id: str) -> PayStackResponse:
+        """
+        Fetch details of a specific transaction split
+
+        :param: split_id: The split ID
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/split/{split_id}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/transactions.py` & `paystackease-2.0.4/paystackease/apis/async_apis/atransactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,319 +1,319 @@
-"""
-Wrapper for Paystack Transactions API
-
-The Transactions API allows you to create and manage payments on your integration.
-"""
-
-from datetime import date
-from typing import List, Optional, Dict, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import Channels, Currency, Bearer, TransactionStatus
-
-
-class TransactionClientAPI(SyncRequestAPI):
-    """
-    Paystack Transaction API
-    Reference: https://paystack.com/docs/api/transaction/
-    """
-
-    def initialize(
-            self,
-            email: str,
-            amount: int,
-            currency: Optional[Union[Currency, None]] = Currency.NGN.value,
-            reference: Optional[Union[str, None]] = None,
-            callback_url: Optional[Union[str, None]] = None,
-            plan: Optional[Union[str, None]] = None,
-            invoice_limit: Optional[Union[int, None]] = None,
-            channels: Optional[Union[List[Channels], None]] = None,
-            split_code: Optional[Union[str, None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            transaction_charge: Optional[Union[int, None]] = None,
-            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Initialize a transaction
-
-        :param: email:
-        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
-                        Use convert_currency() to convert to subunit
-        :param: currency:  # Currency.value.value
-        :param: reference:
-        :param: callback_url: # Use this to override the callback url provided on the  dashboard
-                            # https://example.com/callback
-        :param: plan:  # If transaction is to create a subscription to a predefined plan, provide plan code here.
-        :param: invoice_limit:  # Number of times to charge customer during subscription to plan
-        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
-        :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
-        :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
-        :param: transaction_charge: # An amount used to override the split configuration for a
-                                    # single split payment
-        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
-        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "amount": amount,
-            "currency": currency,
-            "reference": reference,
-            "callback_url": callback_url,
-            "plan": plan,
-            "invoice_limit": invoice_limit,
-            "channels": channels,
-            "split_code": split_code,
-            "subaccount": subaccount,
-            "transaction_charge": transaction_charge,
-            "bearer": bearer,
-            "metadata": metadata,
-        }
-        return self._post_request("/transaction/initialize", data=data)
-
-    def charge_authorization(
-            self,
-            email: str,
-            amount: int,
-            authorization_code: str,
-            reference: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            channels: Optional[Union[List[Channels], None]] = None,
-            subaccount: Optional[Union[str, None]] = None,
-            transaction_charge: Optional[int] = None,
-            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
-            queue: Optional[Union[bool, None]] = True,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Charge an authorization transaction
-
-        :param: email:
-        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
-                        Use convert_currency() to convert to subunit
-        :param: authorization_code:  # value = AUTH_1234234WRFW
-        :param: reference:
-        :param: currency:  # value = Currency.value.value
-        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
-        :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
-        :param: transaction_charge:
-        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
-        :param: queue:  # If set to true, the transaction will be queued for processing
-        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert bool to string
-        queue = self._convert_to_string(queue)
-
-        data = {
-            "email": email,
-            "amount": amount,
-            "authorization_code": authorization_code,
-            "reference": reference,
-            "currency": currency,
-            "channels": channels,
-            "subaccount": subaccount,
-            "transaction_charge": transaction_charge,
-            "bearer": bearer,
-            "queue": queue,
-            "metadata": metadata,
-        }
-        return self._post_request("/transaction/charge_authorization", data=data)
-
-    def partial_debit(
-            self,
-            email: str,
-            authorization_code: str,
-            amount: int,
-            currency: str,
-            reference: Optional[Union[str, None]] = None,
-            at_least: Optional[Union[int, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Charge a partial debit transaction
-
-        :param: email:
-        :param: authorization_code:  # value = AUTH_1234234WRFW
-        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
-                        Use convert_currency() to convert to subunit
-        :param: currency:  # value = Currency.value.value
-        :param: reference:  # Unique transaction reference.
-        :param: at_least:  # Minimum amount to charge
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "email": email,
-            "authorization_code": authorization_code,
-            "amount": amount,
-            "currency": currency,
-            "reference": reference,
-            "at_least": at_least,
-        }
-        return self._post_request("/transaction/partial_debit", data=data)
-
-    def list_transactions(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[int, None]] = None,
-            terminal_id: Optional[Union[str, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            status: Optional[Union[TransactionStatus, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List all transactions
-
-        :param: per_page:  # Specify how many records you want to retrieve per page.
-        :param: page:  # Specify a page number to retrieve
-        :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
-        :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
-        :param: amount:  # Specify an amount for the transactions you want to retrieve
-        :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
-        :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
-        :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "terminalid": terminal_id,
-            "amount": amount,
-            "status": status,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/transaction", params=params)
-
-    def verify_transaction(self, reference: str) -> PayStackResponse:
-        """
-        Verify a transaction by reference
-
-        :param: reference:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/transaction/verify/{reference}")
-
-    def fetch_transaction(self, transaction_id: int) -> PayStackResponse:
-        """
-        Fetch details of a specific transaction
-
-        :param: transaction_id:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/transaction/{transaction_id}")
-
-    def transaction_timeline(self, id_or_reference: str) -> PayStackResponse:
-        """
-        Get the timeline of a transaction
-
-        :param: id_or_reference:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/transaction/timeline/{id_or_reference}")
-
-    def transaction_totals(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Get totals of all transactions
-
-        :param: per_page:
-        :param: page:
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/transaction/totals", params=params)
-
-    def export_transactions(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer: Optional[Union[int, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            amount: Optional[Union[int, None]] = None,
-            status: Optional[Union[TransactionStatus, None]] = None,
-            settled: Optional[Union[bool, None]] = True,
-            settlement: Optional[Union[int, None]] = None,
-            payment_page: Optional[Union[int, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Export transactions
-
-        :param: per_page:
-        :param: page:
-        :param: customer:
-        :param: currency:  # value = Currency.value.value
-        :param: amount:
-        :param: status:
-        :param: settled:  # true or false
-        :param: settlement:
-        :param: payment_page:
-        :param: from_date:  # 2016-09-24T00:00:05.000Z
-        :param: to_date:  # 2016-09-24T00:00:05.000Z
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date and bool to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-        settled = self._convert_to_string(settled)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer,
-            "currency": currency,
-            "amount": amount,
-            "status": status,
-            "settled": settled,
-            "settlement": settlement,
-            "payment_page": payment_page,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/transaction/export", params=params)
+"""
+Wrapper for Asynchronous Paystack Transactions API
+
+The Transactions API allows you to create and manage payments on your integration.
+"""
+
+from datetime import date
+from typing import List, Optional, Dict, Any, Union
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import TransactionStatus, Channels, Bearer, Currency
+
+
+class AsyncTransactionClientAPI(AsyncRequestAPI):
+    """
+    Paystack Transaction API
+    Reference: https://paystack.com/docs/api/transaction/
+    """
+
+    async def initialize(
+            self,
+            email: str,
+            amount: int,
+            currency: Optional[Union[Currency, None]] = Currency.NGN.value,
+            reference: Optional[Union[str, None]] = None,
+            callback_url: Optional[Union[str, None]] = None,
+            plan: Optional[Union[str, None]] = None,
+            invoice_limit: Optional[Union[int, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            transaction_charge: Optional[Union[int, None]] = None,
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Initialize a transaction
+
+        :param: email:
+        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
+                        Use convert_currency() to convert to subunit
+        :param: currency:  # Currency.value.value
+        :param: reference:
+        :param: callback_url: # Use this to override the callback url provided on the  dashboard
+                                # https://example.com/callback
+        :param: plan:  # If transaction is to create a subscription to a preasync defined plan, provide plan code here.
+        :param: invoice_limit:  # Number of times to charge customer during subscription to plan
+        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
+        :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
+        :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
+        :param: transaction_charge: # An amount used to override the split configuration for a
+                                    # single split payment
+        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
+        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "amount": amount,
+            "currency": currency,
+            "reference": reference,
+            "callback_url": callback_url,
+            "plan": plan,
+            "invoice_limit": invoice_limit,
+            "channels": channels,
+            "split_code": split_code,
+            "subaccount": subaccount,
+            "transaction_charge": transaction_charge,
+            "bearer": bearer,
+            "metadata": metadata,
+        }
+        return await self._post_request("/transaction/initialize", data=data)
+
+    async def charge_authorization(
+            self,
+            email: str,
+            amount: int,
+            authorization_code: str,
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            transaction_charge: Optional[int] = None,
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            queue: Optional[Union[bool, None]] = True,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Charge an authorization transaction
+
+        :param: email:
+        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
+                        Use convert_currency() to convert to subunit
+        :param: authorization_code:  # value = AUTH_1234234WRFW
+        :param: reference:
+        :param: currency:  # value = Currency.value.value
+        :param: channels:  # [Channels.value.value, Channels.value.value, ...]
+        :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
+        :param: transaction_charge:
+        :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
+        :param: queue:  # If set to true, the transaction will be queued for processing
+        :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert bool to string
+        queue = self._convert_to_string(queue)
+
+        data = {
+            "email": email,
+            "amount": amount,
+            "authorization_code": authorization_code,
+            "reference": reference,
+            "currency": currency,
+            "channels": channels,
+            "subaccount": subaccount,
+            "transaction_charge": transaction_charge,
+            "bearer": bearer,
+            "queue": queue,
+            "metadata": metadata,
+        }
+        return await self._post_request("/transaction/charge_authorization", data=data)
+
+    async def partial_debit(
+            self,
+            email: str,
+            authorization_code: str,
+            amount: int,
+            currency: str,
+            reference: Optional[Union[str, None]] = None,
+            at_least: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Charge a partial debit transaction
+
+        :param: email:
+        :param: authorization_code:  # value = AUTH_1234234WRFW
+        :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
+                        Use convert_currency() to convert to subunit
+        :param: currency:  # value = Currency.value.value
+        :param: reference:  # Unique transaction reference.
+        :param: at_least:  # Minimum amount to charge
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "email": email,
+            "authorization_code": authorization_code,
+            "amount": amount,
+            "currency": currency,
+            "reference": reference,
+            "at_least": at_least,
+        }
+        return await self._post_request("/transaction/partial_debit", data=data)
+
+    async def list_transactions(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            terminal_id: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List all transactions
+
+        :param: per_page:  # Specify how many records you want to retrieve per page.
+        :param: page:  # Specify a page number to retrieve
+        :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
+        :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
+        :param: amount:  # Specify an amount for the transactions you want to retrieve
+        :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
+        :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
+        :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "terminalid": terminal_id,
+            "amount": amount,
+            "status": status,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/transaction", params=params)
+
+    async def verify_transaction(self, reference: str) -> PayStackResponse:
+        """
+        Verify a transaction by reference
+
+        :param: reference:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/transaction/verify/{reference}")
+
+    async def fetch_transaction(self, transaction_id: int) -> PayStackResponse:
+        """
+        Fetch details of a specific transaction
+
+        :param: transaction_id:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/transaction/{transaction_id}")
+
+    async def transaction_timeline(self, id_or_reference: str) -> PayStackResponse:
+        """
+        Get the timeline of a transaction
+
+        :param: id_or_reference:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/transaction/timeline/{id_or_reference}")
+
+    async def transaction_totals(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Get totals of all transactions
+
+        :param: per_page:
+        :param: page:
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/transaction/totals", params=params)
+
+    async def export_transactions(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            settled: Optional[Union[bool, None]] = True,
+            settlement: Optional[Union[int, None]] = None,
+            payment_page: Optional[Union[int, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Export transactions
+
+        :param: per_page:
+        :param: page:
+        :param: customer:
+        :param: currency:  # value = Currency.value.value
+        :param: amount:
+        :param: status:
+        :param: settled:  # true or false
+        :param: settlement:
+        :param: payment_page:
+        :param: from_date:  # 2016-09-24T00:00:05.000Z
+        :param: to_date:  # 2016-09-24T00:00:05.000Z
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date and bool to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+        settled = self._convert_to_string(settled)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer,
+            "currency": currency,
+            "amount": amount,
+            "status": status,
+            "settled": settled,
+            "settlement": settlement,
+            "payment_page": payment_page,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/transaction/export", params=params)
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/transfer_recipients.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/transfer_recipients.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-"""
-Wrapper for Paystack Transfer Recipient APIs
-
-The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
-"""
-
-from datetime import date
-from typing import Optional, Dict, List, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import Currency
-
-
-class TransferRecipientsClientAPI(SyncRequestAPI):
-    """
-    Paystack Transfer Recipients API
-    Reference: https://paystack.com/docs/api/transfer-recipient/
-    """
-
-    def create_transfer_recipients(
-            self,
-            recipient_type: str,
-            recipient_name: str,
-            account_number: str,
-            bank_code: str,
-            description: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            authorization_code: Optional[Union[str, None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> PayStackResponse:
-        """
-        Create a transfer recipient
-
-        :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
-        :param: recipient_name: The name of the transfer recipient according to their account registration
-        :param: account_number: transfer recipient's account number.
-                                Required for all recipient types except authorization
-        :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
-        :param: description:
-        :param: currency: transfer recipient's currency. [Currency.value.value ]
-        :param: authorization_code: transfer recipient's authorization code from previous transaction
-        :param: metadata: transfer recipient's metadata
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "type": recipient_type,
-            "name": recipient_name,
-            "account_number": account_number,
-            "bank_code": bank_code,
-            "description": description,
-            "currency": currency,
-            "authorization_code": authorization_code,
-            "metadata": metadata,
-        }
-        return self._post_request("/transferrecipient", data=data)
-
-    def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> PayStackResponse:
-        """
-        Create multiple transfer recipients in batches.
-
-        :param: batch: A list of transfer recipient object
-                        keys [ { type, name, account_number, bank_code, currency etc. }]
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"batch": batch}
-        return self._post_request("/transferrecipient/bulk", data=data)
-
-    def list_transfer_recipients(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List transfer recipients
-
-        :param: per_page: The number of records to return per page.
-        :param: page: The page number to retrieve.
-        :param: from_date:
-        :param: to_date:
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to strings
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/transferrecipient", params=params)
-
-    def fetch_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
-        """
-        Fetch details of a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/transferrecipient/{id_or_code}")
-
-    def update_transfer_recipient(
-            self,
-            id_or_code: str,
-            recipient_name: str,
-            recipient_email: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Update a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-        :param: recipient_name: The name of the transfer recipient
-        :param: recipient_email: The email of the transfer recipient
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"name": recipient_name, "email": recipient_email}
-        return self._put_request(f"/transferrecipient/{id_or_code}", data=data)
-
-    def delete_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
-        """
-        Delete a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._delete_request(f"/transferrecipient/{id_or_code}")
+"""
+Wrapper for Paystack Transfer Recipient APIs
+
+The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
+"""
+
+from datetime import date
+from typing import Optional, Dict, List, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
+
+
+class TransferRecipientsClientAPI(SyncRequestAPI):
+    """
+    Paystack Transfer Recipients API
+    Reference: https://paystack.com/docs/api/transfer-recipient/
+    """
+
+    def create_transfer_recipients(
+            self,
+            recipient_type: str,
+            recipient_name: str,
+            account_number: str,
+            bank_code: str,
+            description: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            authorization_code: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> PayStackResponse:
+        """
+        Create a transfer recipient
+
+        :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
+        :param: recipient_name: The name of the transfer recipient according to their account registration
+        :param: account_number: transfer recipient's account number.
+                                Required for all recipient types except authorization
+        :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
+        :param: description:
+        :param: currency: transfer recipient's currency. [Currency.value.value ]
+        :param: authorization_code: transfer recipient's authorization code from previous transaction
+        :param: metadata: transfer recipient's metadata
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "type": recipient_type,
+            "name": recipient_name,
+            "account_number": account_number,
+            "bank_code": bank_code,
+            "description": description,
+            "currency": currency,
+            "authorization_code": authorization_code,
+            "metadata": metadata,
+        }
+        return self._post_request("/transferrecipient", data=data)
+
+    def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> PayStackResponse:
+        """
+        Create multiple transfer recipients in batches.
+
+        :param: batch: A list of transfer recipient object
+                        keys [ { type, name, account_number, bank_code, currency etc. }]
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"batch": batch}
+        return self._post_request("/transferrecipient/bulk", data=data)
+
+    def list_transfer_recipients(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List transfer recipients
+
+        :param: per_page: The number of records to return per page.
+        :param: page: The page number to retrieve.
+        :param: from_date:
+        :param: to_date:
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to strings
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
+        return self._get_request("/transferrecipient", params=params)
+
+    def fetch_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
+        """
+        Fetch details of a transfer recipient
+
+        :param: id_or_code: The id or code of the transfer recipient
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/transferrecipient/{id_or_code}")
+
+    def update_transfer_recipient(
+            self,
+            id_or_code: str,
+            recipient_name: str,
+            recipient_email: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update a transfer recipient
+
+        :param: id_or_code: The id or code of the transfer recipient
+        :param: recipient_name: The name of the transfer recipient
+        :param: recipient_email: The email of the transfer recipient
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"name": recipient_name, "email": recipient_email}
+        return self._put_request(f"/transferrecipient/{id_or_code}", data=data)
+
+    def delete_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
+        """
+        Delete a transfer recipient
+
+        :param: id_or_code: The id or code of the transfer recipient
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._delete_request(f"/transferrecipient/{id_or_code}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/transfers.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/transfers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-"""
-Wrapper for Paystack Transfers APIs
-
-The Transfers API allows you to automate sending money to your customers.
-"""
-
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-from paystackease.helpers import Currency
-
-
-class TransfersClientAPI(SyncRequestAPI):
-    """
-    Paystack Transfers API
-    Reference: https://paystack.com/docs/api/transfer/
-    """
-
-    def initiate_transfer(
-            self,
-            transfer_source: str,
-            amount: int,
-            transfer_recipient: str,
-            reason: Optional[Union[str, None]] = None,
-            currency: Optional[Union[Currency, None]] = None,
-            reference: Optional[Union[str, None]] = None,
-    ) -> PayStackResponse:
-        """
-        Initiate a transfer. Upgrade your business to a Registered Business to use
-
-        :param: transfer_source: Where should we transfer from? Only balance for now
-        :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
-        :param: transfer_recipient: The code of the recipient
-        :param: currency: The currency of the transfer
-        :param: reason: The reason for the transfer
-        :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
-                            Only -,_ and alphanumeric characters allowed.
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "source": transfer_source,
-            "amount": amount,
-            "recipient": transfer_recipient,
-            "reason": reason,
-            "currency": currency,
-            "reference": reference,
-        }
-        return self._post_request("/transfer", data=data)
-
-    def finalize_transfer(self, transfer_code: str, otp: str) -> PayStackResponse:
-        """
-        Finalize an initiated transfer
-
-        :param: transfer_code: The code of the transfer to finalize
-        :param: otp: The OTP sent to the business phone to verify transfer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"transfer_code": transfer_code, "otp": otp}
-        return self._post_request("/transfer/finalize_transfer", data=data)
-
-    def initiate_bulk_transfer(
-            self, transfer_source: str, transfers: List[Dict[str, Any]]
-    ) -> PayStackResponse:
-        """
-        Batch multiple transfers in a single request
-
-        :param: transfer_source: Where should we transfer from? Only balance for now
-        :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"source": transfer_source, "transfers": transfers}
-        return self._post_request("/transfer/bulk", data=data)
-
-    def list_transfers(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page: Optional[Union[int, None]] = 1,
-            customer_id: Optional[Union[str, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> PayStackResponse:
-        """
-        List transfers
-
-        :param: per_page: The number of records to return per page.
-        :param: page: The page number to retrieve.
-        :param: customer_id
-        :param: from_date
-        :param: to_date
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-
-        # convert date to string
-        from_date = self._convert_to_string(from_date)
-        to_date = self._convert_to_string(to_date)
-
-        params = {
-            "perPage": per_page,
-            "page": page,
-            "customer": customer_id,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get_request("/transfer", params=params)
-
-    def fetch_transfer(self, id_or_code: str) -> PayStackResponse:
-        """
-        Get details of a transfer
-
-        :param: id_or_code: The id or code of the transfer
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/transfer/{id_or_code}")
-
-    def verify_transfer(self, reference: str) -> PayStackResponse:
-        """
-        Verify a transfer
-
-        :param: reference: The reference of the transfer to verify
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request(f"/transfer/verify/{reference}")
+"""
+Wrapper for Paystack Transfers APIs
+
+The Transfers API allows you to automate sending money to your customers.
+"""
+
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
+
+
+class TransfersClientAPI(SyncRequestAPI):
+    """
+    Paystack Transfers API
+    Reference: https://paystack.com/docs/api/transfer/
+    """
+
+    def initiate_transfer(
+            self,
+            transfer_source: str,
+            amount: int,
+            transfer_recipient: str,
+            reason: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Initiate a transfer. Upgrade your business to a Registered Business to use
+
+        :param: transfer_source: Where should we transfer from? Only balance for now
+        :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
+        :param: transfer_recipient: The code of the recipient
+        :param: currency: The currency of the transfer
+        :param: reason: The reason for the transfer
+        :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
+                            Only -,_ and alphanumeric characters allowed.
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "source": transfer_source,
+            "amount": amount,
+            "recipient": transfer_recipient,
+            "reason": reason,
+            "currency": currency,
+            "reference": reference,
+        }
+        return self._post_request("/transfer", data=data)
+
+    def finalize_transfer(self, transfer_code: str, otp: str) -> PayStackResponse:
+        """
+        Finalize an initiated transfer
+
+        :param: transfer_code: The code of the transfer to finalize
+        :param: otp: The OTP sent to the business phone to verify transfer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"transfer_code": transfer_code, "otp": otp}
+        return self._post_request("/transfer/finalize_transfer", data=data)
+
+    def initiate_bulk_transfer(
+            self, transfer_source: str, transfers: List[Dict[str, Any]]
+    ) -> PayStackResponse:
+        """
+        Batch multiple transfers in a single request
+
+        :param: transfer_source: Where should we transfer from? Only balance for now
+        :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"source": transfer_source, "transfers": transfers}
+        return self._post_request("/transfer/bulk", data=data)
+
+    def list_transfers(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer_id: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List transfers
+
+        :param: per_page: The number of records to return per page.
+        :param: page: The page number to retrieve.
+        :param: customer_id
+        :param: from_date
+        :param: to_date
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer_id,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get_request("/transfer", params=params)
+
+    def fetch_transfer(self, id_or_code: str) -> PayStackResponse:
+        """
+        Get details of a transfer
+
+        :param: id_or_code: The id or code of the transfer
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/transfer/{id_or_code}")
+
+    def verify_transfer(self, reference: str) -> PayStackResponse:
+        """
+        Verify a transfer
+
+        :param: reference: The reference of the transfer to verify
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request(f"/transfer/verify/{reference}")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/transfers_control.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/transfers_control.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""
-Wrapper for Paystack Transfer Control APIs
-
-The Transfers Control API allows you manage settings of your transfers.
-"""
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-
-
-class TransferControlClientAPI(SyncRequestAPI):
-    """
-    Paystack Transfers Control API
-    Reference: https://paystack.com/docs/api/transfer-control/
-    """
-
-    def check_balance(self) -> PayStackResponse:
-        """
-        Get the available balance
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request("/balance")
-
-    def fetch_balance_ledger(self) -> PayStackResponse:
-        """
-        Fetch all pay-ins and pay-outs that occurred on your integration
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request("/balance/ledger")
-
-    def resend_otp(self, transfer_code: str, reason: str) -> PayStackResponse:
-        """
-        Generates a new OTP and sends to customer in the event
-        they are having trouble receiving one.
-
-        :param: transfer_code: The code of the transfer to finalize
-        :param: reason: Either resend_otp or transfer as the value of this field
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"transfer_code": transfer_code, "reason": reason}
-        return self._post_request("/transfer/resend_otp", data=data)
-
-    def disable_otp(self) -> PayStackResponse:
-        """
-        This is used in the event that you want to be able to
-         complete transfers programmatically without use of OTPs
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request("/transfer/disable_otp")
-
-    def finalize_disable_otp(self, otp: str) -> PayStackResponse:
-        """
-        Finalize the request to disable OTP on your transfers.
-
-        :param: otp: The OTP sent to the business phone to verify disabling of OTP
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {"otp": otp}
-        return self._post_request("/transfer/disable_otp_finalize", data=data)
-
-    def enable_otp(self) -> PayStackResponse:
-        """
-        This is used in the event that you want to stop
-        being able to complete transfers programmatically with use of OTPs
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._post_request("/transfer/enable_otp")
+"""
+Wrapper for Paystack Transfer Control APIs
+
+The Transfers Control API allows you manage settings of your transfers.
+"""
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class TransferControlClientAPI(SyncRequestAPI):
+    """
+    Paystack Transfers Control API
+    Reference: https://paystack.com/docs/api/transfer-control/
+    """
+
+    def check_balance(self) -> PayStackResponse:
+        """
+        Get the available balance
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request("/balance")
+
+    def fetch_balance_ledger(self) -> PayStackResponse:
+        """
+        Fetch all pay-ins and pay-outs that occurred on your integration
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request("/balance/ledger")
+
+    def resend_otp(self, transfer_code: str, reason: str) -> PayStackResponse:
+        """
+        Generates a new OTP and sends to customer in the event
+        they are having trouble receiving one.
+
+        :param: transfer_code: The code of the transfer to finalize
+        :param: reason: Either resend_otp or transfer as the value of this field
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"transfer_code": transfer_code, "reason": reason}
+        return self._post_request("/transfer/resend_otp", data=data)
+
+    def disable_otp(self) -> PayStackResponse:
+        """
+        This is used in the event that you want to be able to
+         complete transfers programmatically without use of OTPs
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request("/transfer/disable_otp")
+
+    def finalize_disable_otp(self, otp: str) -> PayStackResponse:
+        """
+        Finalize the request to disable OTP on your transfers.
+
+        :param: otp: The OTP sent to the business phone to verify disabling of OTP
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"otp": otp}
+        return self._post_request("/transfer/disable_otp_finalize", data=data)
+
+    def enable_otp(self) -> PayStackResponse:
+        """
+        This is used in the event that you want to stop
+        being able to complete transfers programmatically with use of OTPs
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._post_request("/transfer/enable_otp")
```

### Comparing `paystackease-2.0.0/paystackease/apis/sync_apis/verification.py` & `paystackease-2.0.4/paystackease/apis/sync_apis/verification.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""
-Wrapper for Paystack Verification APIs
-
-The Verification API allows you to perform KYC processes.
-"""
-
-from paystackease.core import PayStackResponse, SyncRequestAPI
-
-
-class VerificationClientAPI(SyncRequestAPI):
-    """
-    Paystack Verification API
-    Reference: https://paystack.com/docs/api/verification/
-    """
-
-    def resolve_account(self, account_number: str, bank_code: str) -> PayStackResponse:
-        """
-        Confirm an account belongs to the right customer.
-        This feature is available to business in Nigeria and Ghana.
-
-        :param: account_number: The account number to verify
-        :param: bank_code: The bank code to verify
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        params = {"account_number": account_number, "bank_code": bank_code}
-        return self._get_request("/bank/resolve", params=params)
-
-    def validate_account(
-            self,
-            account_name: str,
-            account_number: str,
-            account_type: str,
-            bank_code: str,
-            country_code: str,
-            document_type: str,
-            document_number: str,
-    ) -> PayStackResponse:
-        """
-        Confirm the authenticity of a customer's account number before sending money.
-        This feature is only available to businesses in South Africa.
-
-        :param: account_name: The account name to validate: first and last name
-        :param: account_number: The account number to validate
-        :param: account_type: The account type to validate: personal or business
-        :param: bank_code: The bank code to validate
-        :param: country_code: The country code to validate
-        :param: document_type: The customer's mode of identity:
-                                identityNumber, passportNumber or businessRegistrationNumber
-        :param: document_number: The customer's document number
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        data = {
-            "account_name": account_name,
-            "account_number": account_number,
-            "account_type": account_type,
-            "bank_code": bank_code,
-            "country_code": country_code,
-            "document_type": document_type,
-            "document_number": document_number,
-        }
-        return self._post_request("/bank/validate", data=data)
-
-    def resolve_card_bin(self, bin_code: str) -> PayStackResponse:
-        """
-        Resolve a card BIN
-
-        :param: bin_code: First 6 characters of card
-
-        :return: The PayStackResponse from the API
-        :rtype: PayStackResponse object
-        """
-        return self._get_request(f"/decision/bin/{bin_code}")
+"""
+Wrapper for Paystack Verification APIs
+
+The Verification API allows you to perform KYC processes.
+"""
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+
+
+class VerificationClientAPI(SyncRequestAPI):
+    """
+    Paystack Verification API
+    Reference: https://paystack.com/docs/api/verification/
+    """
+
+    def resolve_account(self, account_number: str, bank_code: str) -> PayStackResponse:
+        """
+        Confirm an account belongs to the right customer.
+        This feature is available to business in Nigeria and Ghana.
+
+        :param: account_number: The account number to verify
+        :param: bank_code: The bank code to verify
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {"account_number": account_number, "bank_code": bank_code}
+        return self._get_request("/bank/resolve", params=params)
+
+    def validate_account(
+            self,
+            account_name: str,
+            account_number: str,
+            account_type: str,
+            bank_code: str,
+            country_code: str,
+            document_type: str,
+            document_number: str,
+    ) -> PayStackResponse:
+        """
+        Confirm the authenticity of a customer's account number before sending money.
+        This feature is only available to businesses in South Africa.
+
+        :param: account_name: The account name to validate: first and last name
+        :param: account_number: The account number to validate
+        :param: account_type: The account type to validate: personal or business
+        :param: bank_code: The bank code to validate
+        :param: country_code: The country code to validate
+        :param: document_type: The customer's mode of identity:
+                                identityNumber, passportNumber or businessRegistrationNumber
+        :param: document_number: The customer's document number
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "account_name": account_name,
+            "account_number": account_number,
+            "account_type": account_type,
+            "bank_code": bank_code,
+            "country_code": country_code,
+            "document_type": document_type,
+            "document_number": document_number,
+        }
+        return self._post_request("/bank/validate", data=data)
+
+    def resolve_card_bin(self, bin_code: str) -> PayStackResponse:
+        """
+        Resolve a card BIN
+
+        :param: bin_code: First 6 characters of card
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return self._get_request(f"/decision/bin/{bin_code}")
```

### Comparing `paystackease-2.0.0/paystackease/core/_api_base.py` & `paystackease-2.0.4/paystackease/core/_api_base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""
-BaseAPI serves as the base for creating client APIs to interact with the Paystack API
-with methods for handling HTTP requests, authentication using a secret key,
-constructing HTTP headers, joining URLs with the API base URL, and logging response information.
-"""
-
-import logging
-from abc import ABC, abstractmethod
-
-from datetime import datetime, date
-from typing import Union, Dict, List, Any, Optional
-from urllib.parse import urljoin
-from decouple import config
-
-from paystackease.core._api_client_response import PayStackResponse
-from paystackease.core._api_errors import SecretKeyError, TypeValueError
-
-logger = logging.getLogger(__name__)
-
-PAYSTACK_SECRET_KEY = config("PAYSTACK_SECRET_KEY")
-
-
-class BaseAPI(ABC):
-    """Base Client API for Paystack API"""
-
-    _PAYSTACK_API_URL: str = "https://api.paystack.co/"
-    _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
-
-    # pylint: disable=too-few-public-methods
-    def __init__(self, secret_key: str = None) -> None:
-        self._secret_key = secret_key
-
-        # Default to PAYSTACK_SECRET_KEY if not provided in the instance
-        if not self._secret_key:
-            self._secret_key = PAYSTACK_SECRET_KEY  # or environment variables
-
-        # Raise an error if PAYSTACK_SECRET_KEY is not set in the instance or environment variables
-        if not self._secret_key:
-            error_message = "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
-            logger.error(error_message)
-            raise SecretKeyError(error_message)
-
-        self._headers = self._make_paystack_http_headers()
-
-    @classmethod
-    def _set_secret_key(cls, secret_key: str) -> None:
-        """Set the secret key for all instances of this class"""
-        cls._secret_key = secret_key
-
-    def _join_url(self, path: str) -> str:
-        """
-        Join URL with Paystack API URL
-        :param path:
-        :return:
-        """
-        if path.startswith("/"):
-            path = path[1:]
-        return urljoin(self._PAYSTACK_API_URL, path)
-
-    def _make_paystack_http_headers(self) -> dict:
-        """
-        Make Paystack HTTP Headers
-        :return:
-        """
-        return {
-            "Authorization": f"Bearer {self._secret_key}",
-            "content-type": "application/json",
-        }
-
-    @staticmethod
-    def _convert_to_string(
-        value: Union[bool, date, datetime, None]
-    ) -> Union[str, int, None]:
-        """
-        Convert the type of value to a string
-        :param value: The value to be converted
-
-        :raise TypeError: if the value is not a supported type
-
-        :return: The value as a string
-        :rtype: str
-        """
-        # each supported type is mapped to its corresponding conversion function
-        conversion_functions = {
-            bool: lambda val: str(val),
-            date: lambda val: val.strftime("%Y-%m-%d"),
-            datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),  # Added a datetime
-        }
-
-        if value is None:
-            return None
-        if type(value) in conversion_functions:
-            return conversion_functions[type(value)](value)
-        error_message = f"Unsupported type: {type(value)}. Expected type -bool, -date, -datetime"
-        logger.error(error_message)
-        raise TypeValueError(error_message)
-
-    @abstractmethod
-    def _request_url(
-        self,
-        method: str,
-        url: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Handles the request to Paystack API
-        :param method:
-        :param url:
-        :param data:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        pass
+"""
+BaseAPI serves as the base for creating client APIs to interact with the Paystack API
+with methods for handling HTTP requests, authentication using a secret key,
+constructing HTTP headers, joining URLs with the API base URL, and logging response information.
+"""
+
+import logging
+from abc import ABC, abstractmethod
+
+from datetime import datetime, date
+from typing import Union, Dict, List, Any, Optional
+from urllib.parse import urljoin
+from decouple import config
+
+from paystackease.core._api_client_response import PayStackResponse
+from paystackease.core._api_errors import SecretKeyError, TypeValueError
+
+logger = logging.getLogger(__name__)
+
+PAYSTACK_SECRET_KEY = config("PAYSTACK_SECRET_KEY")
+
+
+class BaseAPI(ABC):
+    """Base Client API for Paystack API"""
+
+    _PAYSTACK_API_URL: str = "https://api.paystack.co/"
+    _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
+
+    # pylint: disable=too-few-public-methods
+    def __init__(self, secret_key: str = None) -> None:
+        self._secret_key = secret_key
+
+        # Default to PAYSTACK_SECRET_KEY if not provided in the instance
+        if not self._secret_key:
+            self._secret_key = PAYSTACK_SECRET_KEY  # or environment variables
+
+        # Raise an error if PAYSTACK_SECRET_KEY is not set in the instance or environment variables
+        if not self._secret_key:
+            error_message = "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
+            logger.error(error_message)
+            raise SecretKeyError(error_message)
+
+        self._headers = self._make_paystack_http_headers()
+
+    @classmethod
+    def _set_secret_key(cls, secret_key: str) -> None:
+        """Set the secret key for all instances of this class"""
+        cls._secret_key = secret_key
+
+    def _join_url(self, path: str) -> str:
+        """
+        Join URL with Paystack API URL
+        :param path:
+        :return:
+        """
+        if path.startswith("/"):
+            path = path[1:]
+        return urljoin(self._PAYSTACK_API_URL, path)
+
+    def _make_paystack_http_headers(self) -> dict:
+        """
+        Make Paystack HTTP Headers
+        :return:
+        """
+        return {
+            "Authorization": f"Bearer {self._secret_key}",
+            "content-type": "application/json",
+        }
+
+    @staticmethod
+    def _convert_to_string(
+        value: Union[bool, date, datetime, None]
+    ) -> Union[str, int, None]:
+        """
+        Convert the type of value to a string
+        :param value: The value to be converted
+
+        :raise TypeError: if the value is not a supported type
+
+        :return: The value as a string
+        :rtype: str
+        """
+        # each supported type is mapped to its corresponding conversion function
+        conversion_functions = {
+            bool: lambda val: str(val),
+            date: lambda val: val.strftime("%Y-%m-%d"),
+            datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),  # Added a datetime
+        }
+
+        if value is None:
+            return None
+        if type(value) in conversion_functions:
+            return conversion_functions[type(value)](value)
+        error_message = f"Unsupported type: {type(value)}. Expected type -bool, -date, -datetime"
+        logger.error(error_message)
+        raise TypeValueError(error_message)
+
+    @abstractmethod
+    def _request_url(
+        self,
+        method: str,
+        url: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Handles the request to Paystack API
+        :param method:
+        :param url:
+        :param data:
+        :param params:
+        :param kwargs:
+        :return:
+        """
+        pass
```

### Comparing `paystackease-2.0.0/paystackease/core/_api_client_requests.py` & `paystackease-2.0.4/paystackease/core/_api_client_requests.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-"""
-Paystackease HTTP requests and aiohttp handlers This aims to simplify the process of making requests
-to the Paystack API by providing higher-level methods for different HTTP methods,
-"""
-
-from typing import Optional, Any, Union, List, Dict
-
-from paystackease.core._api_base_client import SyncBaseClientAPI, AsyncBaseClientAPI
-from paystackease.core._api_client_response import PayStackResponse
-
-
-class SyncRequestAPI(SyncBaseClientAPI):
-    """Requests methods to Paystack API"""
-
-    def _request(
-        self,
-        method: str,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Handles the request to Paystack API
-        :param method:
-        :param endpoint:
-        :param data:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        return self._request_url(method, endpoint, data=data, params=params, **kwargs)
-
-    def _get_request(
-        self,
-        endpoint: str,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Makes the GET request to Paystack API
-        :param endpoint:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        return self._request("GET", endpoint, params=params, **kwargs)
-
-    def _post_request(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Makes the POST request to Paystack API
-        :param endpoint:
-        :param data:
-        :param kwargs:
-        :return:
-        """
-        return self._request("POST", endpoint, data=data, **kwargs)
-
-    def _put_request(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Makes the PUT request to Paystack API
-        :param endpoint:
-        :param data:
-        :param kwargs:
-        :return:
-        """
-        return self._request("PUT", endpoint, data=data, **kwargs)
-
-    def _delete_request(self, endpoint: str, **kwargs) -> PayStackResponse:
-        """
-        Makes the DELETE request to Paystack API
-        :param endpoint:
-        :param kwargs:
-        :return:
-        """
-        return self._request("DELETE", endpoint, **kwargs)
-
-
-class AsyncRequestAPI(AsyncBaseClientAPI):
-    """Requests methods to Paystack API"""
-
-    async def _request(
-        self,
-        method: str,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Handles the request to Paystack API
-        :param method:
-        :param endpoint:
-        :param data:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        return await self._request_url(
-            method, endpoint, data=data, params=params, **kwargs
-        )
-
-    async def _get_request(
-        self,
-        endpoint: str,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Makes the GET request to Paystack API
-        :param endpoint:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("GET", endpoint, params=params, **kwargs)
-
-    async def _post_request(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Makes the POST request to Paystack API
-        :param endpoint:
-        :param data:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("POST", endpoint, data=data, **kwargs)
-
-    async def _put_request(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> PayStackResponse:
-        """
-        Makes the PUT request to Paystack API
-        :param endpoint:
-        :param data:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("PUT", endpoint, data=data, **kwargs)
-
-    async def _delete_request(self, endpoint: str, **kwargs) -> PayStackResponse:
-        """
-        Makes the DELETE request to Paystack API
-        :param endpoint:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("DELETE", endpoint, **kwargs)
+"""
+Paystackease HTTP requests and aiohttp handlers This aims to simplify the process of making requests
+to the Paystack API by providing higher-level methods for different HTTP methods,
+"""
+
+from typing import Optional, Any, Union, List, Dict
+
+from paystackease.core._api_base_client import SyncBaseClientAPI, AsyncBaseClientAPI
+from paystackease.core._api_client_response import PayStackResponse
+
+
+class SyncRequestAPI(SyncBaseClientAPI):
+    """Requests methods to Paystack API"""
+
+    def _request(
+        self,
+        method: str,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Handles the request to Paystack API
+        :param method:
+        :param endpoint:
+        :param data:
+        :param params:
+        :param kwargs:
+        :return:
+        """
+        return self._request_url(method, endpoint, data=data, params=params, **kwargs)
+
+    def _get_request(
+        self,
+        endpoint: str,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Makes the GET request to Paystack API
+        :param endpoint:
+        :param params:
+        :param kwargs:
+        :return:
+        """
+        return self._request("GET", endpoint, params=params, **kwargs)
+
+    def _post_request(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Makes the POST request to Paystack API
+        :param endpoint:
+        :param data:
+        :param kwargs:
+        :return:
+        """
+        return self._request("POST", endpoint, data=data, **kwargs)
+
+    def _put_request(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Makes the PUT request to Paystack API
+        :param endpoint:
+        :param data:
+        :param kwargs:
+        :return:
+        """
+        return self._request("PUT", endpoint, data=data, **kwargs)
+
+    def _delete_request(self, endpoint: str, **kwargs) -> PayStackResponse:
+        """
+        Makes the DELETE request to Paystack API
+        :param endpoint:
+        :param kwargs:
+        :return:
+        """
+        return self._request("DELETE", endpoint, **kwargs)
+
+
+class AsyncRequestAPI(AsyncBaseClientAPI):
+    """Requests methods to Paystack API"""
+
+    async def _request(
+        self,
+        method: str,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Handles the request to Paystack API
+        :param method:
+        :param endpoint:
+        :param data:
+        :param params:
+        :param kwargs:
+        :return:
+        """
+        return await self._request_url(
+            method, endpoint, data=data, params=params, **kwargs
+        )
+
+    async def _get_request(
+        self,
+        endpoint: str,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Makes the GET request to Paystack API
+        :param endpoint:
+        :param params:
+        :param kwargs:
+        :return:
+        """
+        return await self._request("GET", endpoint, params=params, **kwargs)
+
+    async def _post_request(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Makes the POST request to Paystack API
+        :param endpoint:
+        :param data:
+        :param kwargs:
+        :return:
+        """
+        return await self._request("POST", endpoint, data=data, **kwargs)
+
+    async def _put_request(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> PayStackResponse:
+        """
+        Makes the PUT request to Paystack API
+        :param endpoint:
+        :param data:
+        :param kwargs:
+        :return:
+        """
+        return await self._request("PUT", endpoint, data=data, **kwargs)
+
+    async def _delete_request(self, endpoint: str, **kwargs) -> PayStackResponse:
+        """
+        Makes the DELETE request to Paystack API
+        :param endpoint:
+        :param kwargs:
+        :return:
+        """
+        return await self._request("DELETE", endpoint, **kwargs)
```

### Comparing `paystackease-2.0.0/paystackease/core/_api_client_response.py` & `paystackease-2.0.4/paystackease/core/_api_client_response.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""  This represents the response from the Paystack API server after making HTTP requests. """
-
-from typing import NamedTuple, Optional, Union, Dict, Any
-
-
-class PayStackResponse(NamedTuple):
-    """
-    PaystackEase API Response from the server after HTTP requests have been made
-    """
-
-    status_code: int
-    status: bool
-    message: str
-    data: Optional[Union[Dict[str, Any], None]]
-
-    @property
-    def url(self) -> Optional[Union[str, None]]:
-        """
-        URL of the request
-        """
-        if self.status_code == 200 and self.data and isinstance(self.data, dict):
-            return self.data["authorization_url"]
-        return None
+"""  This represents the response from the Paystack API server after making HTTP requests. """
+
+from typing import NamedTuple, Optional, Union, Dict, Any
+
+
+class PayStackResponse(NamedTuple):
+    """
+    PaystackEase API Response from the server after HTTP requests have been made
+    """
+
+    status_code: int
+    status: bool
+    message: str
+    data: Optional[Union[Dict[str, Any], None]]
+
+    @property
+    def url(self) -> Optional[Union[str, None]]:
+        """
+        URL of the request
+        """
+        if self.status_code == 200 and self.data and isinstance(self.data, dict):
+            return self.data["authorization_url"]
+        return None
```

### Comparing `paystackease-2.0.0/paystackease/core/_api_errors.py` & `paystackease-2.0.4/paystackease/core/_api_errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-""" Paystack Error Message"""
-
-
-class PayStackError(Exception):
-    """
-    Base exception class for Paystack API errors
-    """
-
-    def __init__(self, message: str, status_code: int = None) -> None:
-        self.message = message
-        self.status_code = status_code
-        super(PayStackError, self).__init__(f"\nError Message: {message} \nError Status Code: {status_code}")
-
-
-class SecretKeyError(PayStackError):
-    """
-    Secret Key Error
-    """
-    def __init__(self, message: str, status_code: int = 401) -> None:
-        super().__init__(message, status_code)
-
-
-class TypeValueError(PayStackError):
-    """
-    Type Value Error
-    """
-    def __init__(self, message: str, status_code: int = 400) -> None:
-        super().__init__(message, status_code)
-
-
-class InvalidRequestMethodError(PayStackError):
-    """
-    Request Time Error
-    """
-    def __init__(self, message: str, status_code: int = 400) -> None:
-        super().__init__(message, status_code)
+""" Paystack Error Message"""
+
+
+class PayStackError(Exception):
+    """
+    Base exception class for Paystack API errors
+    """
+
+    def __init__(self, message: str, status_code: int = None) -> None:
+        self.message = message
+        self.status_code = status_code
+        super(PayStackError, self).__init__(f"\nError Message: {self.message} \nError Status Code: {self.status_code}")
+
+
+class SecretKeyError(PayStackError):
+    """
+    Secret Key Error
+    """
+    def __init__(self, message: str, status_code: int = 401) -> None:
+        super().__init__(message, status_code)
+
+
+class TypeValueError(PayStackError):
+    """
+    Type Value Error
+    """
+    def __init__(self, message: str, status_code: int = 400) -> None:
+        super().__init__(message, status_code)
+
+
+class InvalidRequestMethodError(PayStackError):
+    """
+    Request Time Error
+    """
+    def __init__(self, message: str, status_code: int = 400) -> None:
+        super().__init__(message, status_code)
```

### Comparing `paystackease-2.0.0/paystackease/helpers/convert.py` & `paystackease-2.0.4/paystackease/helpers/convert.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""
-This holds function to convert to subunits in NGN, GHS, USD, ZAR and KES
-"""
-from typing import Union
-from paystackease.helpers.tool_kit import Currency
-
-
-def convert_to_subunit(amount: int, currency: Union[Currency, None] = Currency.NGN) -> int:
-    """
-    Convert a subunit amount to a base amount
-    :param amount:
-    :param currency:
-    :return:
-    """
-    subunit_multipliers = {
-        currency.NGN: 100,
-        currency.GHS: 100,
-        currency.USD: 100,
-        currency.ZAR: 100,
-        currency.KES: 100,
-    }
-    subunit_multiplier = subunit_multipliers.get(currency)
-    if not subunit_multiplier:
-        raise ValueError(f"Invalid currency: {currency}")
-    amount = amount * subunit_multiplier
-    return amount
+"""
+This holds function to convert to subunits in NGN, GHS, USD, ZAR and KES
+"""
+from typing import Union
+from paystackease.helpers.tool_kit import Currency
+
+
+def convert_to_subunit(amount: int, currency: Union[Currency, None] = Currency.NGN) -> int:
+    """
+    Convert a subunit amount to a base amount
+    :param amount:
+    :param currency:
+    :return:
+    """
+    subunit_multipliers = {
+        currency.NGN: 100,
+        currency.GHS: 100,
+        currency.USD: 100,
+        currency.ZAR: 100,
+        currency.KES: 100,
+    }
+    subunit_multiplier = subunit_multipliers.get(currency)
+    if not subunit_multiplier:
+        raise ValueError(f"Invalid currency: {currency}")
+    amount = amount * subunit_multiplier
+    return amount
```

### Comparing `paystackease-2.0.0/paystackease/helpers/tool_kit.py` & `paystackease-2.0.4/paystackease/helpers/tool_kit.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-"""
-Enums for Currency and Channels with predefined values.
-"""
-
-from enum import Enum
-
-
-class AccountType(Enum):
-    """Customer’s type of Account."""
-
-    PERSONAL = "personal"
-    BUSINESS = "business"
-
-
-class Bearer(Enum):
-    """Bearer supported by Paystack."""
-    ACCOUNT = "account"
-    SUB_ACCOUNT = "subaccount"
-
-
-class Currency(Enum):
-    """Currencies supported by Paystack."""
-
-    GHS = "GHS"
-    KES = "KES"
-    NGN = "NGN"
-    USD = "USD"
-    ZAR = "ZAR"
-
-
-class Channels(Enum):
-    """Channels supported by Paystack."""
-
-    BANK = "bank"
-    BANK_TRANSFER = "bank_transfer"
-    CARD = "card"
-    ETF = "etf"
-    MOBILE_MONEY = "mobile_money"
-    QR = "qr"
-    USSD = "ussd"
-
-
-class DisputeStatus(Enum):
-    """Dispute status."""
-    MERCHANT_FEEDBACK = "awaiting-merchant-feedback"
-    BANK_FEEDBACK = "awaiting-bank-feedback"
-    PENDING = "pending"
-    RESOLVED = "resolved"
-
-
-class DocumentType(Enum):
-    """Customer’s mode of identity."""
-
-    IDENTITY_NUMBER = "identityNumber"
-    PASSPORT_NUMBER = "passportNumber"
-    BUSINESS_REG_NUMBER = "businessRegistrationNumber"
-
-
-class DVABank(Enum):
-    """DVA_BANK supported by Paystack."""
-    WEMA_BANK = "wema-bank"
-    TITAN = "titan-paystack"
-
-
-class EFT(Enum):
-    """EFT supported by Paystack."""
-
-    OZOW = "ozow"
-
-
-class EventAction(Enum):
-    """Event action supported by Paystack."""
-    PROCESS = "process"
-    VIEW = "view"
-    PRINT = "print"
-
-
-class EventType(Enum):
-    INVOICE = "invoice"
-    TRANSACTION = "transaction"
-
-
-class GateWay(Enum):
-    """ Gateway supported bt Paystack"""
-    E_MANDATE = "emandate"
-    DIGITAL_BANK_MANDATE = "digitalbankmandate"
-
-
-class Interval(Enum):
-    """Interval supported by Paystack."""
-
-    DAILY = "daily"
-    WEEKLY = "weekly"
-    MONTHLY = "monthly"
-    QUARTERLY = "quarterly"
-    BIANNUALLY = "biannually"
-    ANNUALLY = "annually"
-
-
-class MobileMoney(Enum):
-    """Mobile Money supported by Paystack.
-    Only available to businesses in Ghana and Kenya.
-    """
-
-    MTN = "mtn"
-    AIRTEL_TIGO = "atl"
-    VODAFONE = "vod"
-    M_PESA = "mpesa"
-
-
-class PayMentRequestStatus(Enum):
-    """ Payment request status supported by Paystack"""
-    DRAFT = "draft"
-    PENDING = "pending"
-
-
-class PWT(Enum):
-    """PWT supported by Paystack."""
-
-    ACCOUNT_EXPIRES_AT = "account_expires_at"
-
-
-class QRCODE(Enum):
-    """QR Codes supported by Paystack."""
-
-    SCAN_TO_PAY = "scan-to-pay"
-    VISA = "visa"
-
-
-class RecipientType(Enum):
-    BASE = "base"
-    GHIPSS = "ghipss"
-    MOBILE_MONEY = "mobile_money"
-    NUBAN = "nuban"
-
-
-class ResendOTP(Enum):
-    RESEND_OTP = "resend_otp"
-    TRANSFER = "transfer"
-
-
-class Resolution(Enum):
-    MERCHANT = "merchant-accepted"
-    DECLINED = "declined"
-
-
-class RiskAction(Enum):
-    """Risk Action supported by Paystack."""
-
-    ALLOW = "allow"
-    DEFAULT = "default"
-    DENY = "deny"
-
-
-class SettlementSchedule(Enum):
-    """ Schedule"""
-    AUTO = "auto"
-    WEEKLY = "weekly"
-    MANUAL = "manual"
-    MONTHLY = "monthly"
-
-
-class SplitType(Enum):
-    PERCENTAGE = "percentage"
-    FLAT = "flat"
-
-
-class STATUS(Enum):
-    """Status supported by Paystack."""
-
-    SUCCESS = "success"
-    FAILED = "failed"
-    PENDING = "pending"
-    PROCESSING = "processing"
-
-
-class TransactionStatus(Enum):
-    """Transaction status supported by Paystack."""
-    FAILED = "failed"
-    SUCCESS = "success"
-    ABANDONED = "abandoned"
-
-
-class USSD(Enum):
-    """USSD supported by Paystack."""
-
-    GUARANTY_BANK = "737"
-    UNITED_BANK_OF_AFRICA = "919"
-    STERLING_BANK = "822"
-    ZENITH_BANK = "966"
+"""
+Enums for Currency and Channels with predefined values.
+"""
+
+from enum import Enum
+
+
+class AccountType(Enum):
+    """Customer’s type of Account."""
+
+    PERSONAL = "personal"
+    BUSINESS = "business"
+
+
+class Bearer(Enum):
+    """Bearer supported by Paystack."""
+    ACCOUNT = "account"
+    SUB_ACCOUNT = "subaccount"
+
+
+class Currency(Enum):
+    """Currencies supported by Paystack."""
+
+    GHS = "GHS"
+    KES = "KES"
+    NGN = "NGN"
+    USD = "USD"
+    ZAR = "ZAR"
+
+
+class Channels(Enum):
+    """Channels supported by Paystack."""
+
+    BANK = "bank"
+    BANK_TRANSFER = "bank_transfer"
+    CARD = "card"
+    ETF = "etf"
+    MOBILE_MONEY = "mobile_money"
+    QR = "qr"
+    USSD = "ussd"
+
+
+class DisputeStatus(Enum):
+    """Dispute status."""
+    MERCHANT_FEEDBACK = "awaiting-merchant-feedback"
+    BANK_FEEDBACK = "awaiting-bank-feedback"
+    PENDING = "pending"
+    RESOLVED = "resolved"
+
+
+class DocumentType(Enum):
+    """Customer’s mode of identity."""
+
+    IDENTITY_NUMBER = "identityNumber"
+    PASSPORT_NUMBER = "passportNumber"
+    BUSINESS_REG_NUMBER = "businessRegistrationNumber"
+
+
+class DVABank(Enum):
+    """DVA_BANK supported by Paystack."""
+    WEMA_BANK = "wema-bank"
+    TITAN = "titan-paystack"
+
+
+class EFT(Enum):
+    """EFT supported by Paystack."""
+
+    OZOW = "ozow"
+
+
+class EventAction(Enum):
+    """Event action supported by Paystack."""
+    PROCESS = "process"
+    VIEW = "view"
+    PRINT = "print"
+
+
+class EventType(Enum):
+    INVOICE = "invoice"
+    TRANSACTION = "transaction"
+
+
+class GateWay(Enum):
+    """ Gateway supported bt Paystack"""
+    E_MANDATE = "emandate"
+    DIGITAL_BANK_MANDATE = "digitalbankmandate"
+
+
+class Interval(Enum):
+    """Interval supported by Paystack."""
+
+    DAILY = "daily"
+    WEEKLY = "weekly"
+    MONTHLY = "monthly"
+    QUARTERLY = "quarterly"
+    BIANNUALLY = "biannually"
+    ANNUALLY = "annually"
+
+
+class MobileMoney(Enum):
+    """Mobile Money supported by Paystack.
+    Only available to businesses in Ghana and Kenya.
+    """
+
+    MTN = "mtn"
+    AIRTEL_TIGO = "atl"
+    VODAFONE = "vod"
+    M_PESA = "mpesa"
+
+
+class PayMentRequestStatus(Enum):
+    """ Payment request status supported by Paystack"""
+    DRAFT = "draft"
+    PENDING = "pending"
+
+
+class PWT(Enum):
+    """PWT supported by Paystack."""
+
+    ACCOUNT_EXPIRES_AT = "account_expires_at"
+
+
+class QRCODE(Enum):
+    """QR Codes supported by Paystack."""
+
+    SCAN_TO_PAY = "scan-to-pay"
+    VISA = "visa"
+
+
+class RecipientType(Enum):
+    BASE = "base"
+    GHIPSS = "ghipss"
+    MOBILE_MONEY = "mobile_money"
+    NUBAN = "nuban"
+
+
+class ResendOTP(Enum):
+    RESEND_OTP = "resend_otp"
+    TRANSFER = "transfer"
+
+
+class Resolution(Enum):
+    MERCHANT = "merchant-accepted"
+    DECLINED = "declined"
+
+
+class RiskAction(Enum):
+    """Risk Action supported by Paystack."""
+
+    ALLOW = "allow"
+    DEFAULT = "default"
+    DENY = "deny"
+
+
+class SettlementSchedule(Enum):
+    """ Schedule"""
+    AUTO = "auto"
+    WEEKLY = "weekly"
+    MANUAL = "manual"
+    MONTHLY = "monthly"
+
+
+class SplitType(Enum):
+    PERCENTAGE = "percentage"
+    FLAT = "flat"
+
+
+class STATUS(Enum):
+    """Status supported by Paystack."""
+
+    SUCCESS = "success"
+    FAILED = "failed"
+    PENDING = "pending"
+    PROCESSING = "processing"
+
+
+class TransactionStatus(Enum):
+    """Transaction status supported by Paystack."""
+    FAILED = "failed"
+    SUCCESS = "success"
+    ABANDONED = "abandoned"
+
+
+class USSD(Enum):
+    """USSD supported by Paystack."""
+
+    GUARANTY_BANK = "737"
+    UNITED_BANK_OF_AFRICA = "919"
+    STERLING_BANK = "822"
+    ZENITH_BANK = "966"
```

### Comparing `paystackease-2.0.0/pyproject.toml` & `paystackease-2.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,84 @@
-[tool.poetry]
-name = "paystackease"
-version = "2.0.0"
-description = "This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs."
-authors = ["Peter Mbachu <doublep098@gmail.com>"]
-maintainers = []
-license = "MIT"
-readme = "README.md"
-keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
-classifiers = [
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Development Status :: 5 - Production/Stable",
-    "Natural Language :: English",
-    "Topic :: Software Development :: Libraries :: Python Modules"
-]
-packages = [{include = "paystackease"}]
-
-
-[license]
-text = "Copyright ©2024 Peter Mbachu"
-
-
-[tool.poetry.urls]
-"Homepage" = "https://github.com/cla-bit/PayStackEase"
-"Source Code" = "https://github.com/cla-bit/PayStackEase"
-"Documentation" = "https://paystackease.readthedocs.io/en/latest/"
-"Bug Tracker" = "https://github.com/cla-bit/PayStackEase/issues"
-
-
-[tool.poetry.dependencies]
-python = "^3.9"
-aiohttp = "^3.8"
-requests = "^2.31"
-python-decouple = "^3.8"
-
-
-[tool.poetry.group.docs.dependencies]
-pdflatex = "^0.1.3"
-sphinx = "^7.2.6"
-sphinx-rtd-theme = "^2.0.0"
-sphinxawesome-theme = "^5.1.1"
-sphinx-autobuild = "^2024.2.4"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^24.2"
-pylint = "^3.1"
-twine = "^5.0"
-
-
-[tool.poetry.group.test.dependencies]
-pytest = "^8.0"
-responses = "^0.25"
-pytest-asyncio = "^0.23"
-aioresponses = "^0.7"
-
-
-[tool.pytest.ini_options]
-testpaths = ["tests"]
-addopts = "--doctest-modules"
-
-
-[tool.black]
-target-version = ['py310', 'py311']
-include = '\.pyi?$'
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "paystackease"
+version = "2.0.4"
+description = "This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs."
+authors = ["Peter Mbachu <doublep098@gmail.com>"]
+maintainers = []
+license = "MIT"
+readme = "README.md"
+keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
+classifiers = [
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Development Status :: 5 - Production/Stable",
+    "Natural Language :: English",
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
+packages = [{include = "paystackease"}]
+
+
+[license]
+text = "Copyright ©2024 Peter Mbachu"
+
+
+[tool.poetry.urls]
+"Homepage" = "https://github.com/cla-bit/PayStackEase"
+"Source Code" = "https://github.com/cla-bit/PayStackEase"
+"Documentation" = "https://paystackease.readthedocs.io/en/latest/"
+"Bug Tracker" = "https://github.com/cla-bit/PayStackEase/issues"
+
+
+[tool.poetry.dependencies]
+python = "^3.9"
+aiohttp = "^3.8"
+requests = "^2.31"
+python-decouple = "^3.8"
+
+
+[tool.poetry.group.docs.dependencies]
+pdflatex = "^0.1.3"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
+sphinxawesome-theme = "^5.1.1"
+sphinx-autobuild = "^2024.2.4"
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^24.2"
+pylint = "^3.1"
+python-semantic-release = "^9.0"
+
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.0"
+pytest-cov = "^5.0"
+responses = "^0.25"
+pytest-asyncio = "^0.23"
+aioresponses = "^0.7"
+
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+addopts = "--doctest-modules"
+
+
+[tool.black]
+target-version = ['py310', 'py311']
+include = '\.pyi?$'
+
+
+[tool.semantic_release]
+version_toml = ["pyproject.toml:tool.poetry.version"]  # version location
+branch = "main"  # branch to make release of
+changelog_file = "CHANGELOG.md"  # changelog file
+build_command = "pip install poetry && poetry build"  # build dist
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `paystackease-2.0.0/PKG-INFO` & `paystackease-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paystackease
-Version: 2.0.0
+Version: 2.0.4
 Summary: This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs.
 License: MIT
 Keywords: paystack,paystackease,python,api,payment integration
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

