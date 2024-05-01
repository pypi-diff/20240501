# Comparing `tmp/trytond_account_invoice-7.2.0.tar.gz` & `tmp/trytond_account_invoice-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice-7.2.0.tar", last modified: Mon Apr 29 15:33:33 2024, max compression
+gzip compressed data, was "trytond_account_invoice-7.2.1.tar", last modified: Wed May  1 12:21:41 2024, max compression
```

## Comparing `trytond_account_invoice-7.2.0.tar` & `trytond_account_invoice-7.2.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.430225 trytond_account_invoice-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     8135 2024-04-29 15:14:14.000000 trytond_account_invoice-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:14:13.000000 trytond_account_invoice-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-29 15:33:33.430225 trytond_account_invoice-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1977 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14844 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4877 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.420225 trytond_account_invoice-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:54.000000 trytond_account_invoice-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.420225 trytond_account_invoice-7.2.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/amend.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/prepare.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.420225 trytond_account_invoice-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/icons/tryton-invoice.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    94000 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/invoice.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)   139705 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23815 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.423559 trytond_account_invoice-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    38393 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39802 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33224 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40399 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39520 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34147 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37479 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41650 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33185 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40336 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35842 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35712 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36471 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39045 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37221 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39539 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33850 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38882 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39056 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38148 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33167 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31749 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38154 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6873 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3324 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2389 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-04-13 17:12:23.000000 trytond_account_invoice-7.2.0/payment_term.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/payment_term.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:33.430225 trytond_account_invoice-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.423559 trytond_account_invoice-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3122 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_cancelling_invoice_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4010 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_credit_note.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    13167 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6057 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_exchange.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_lower_rate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3488 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_rate_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternative_payee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2666 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_customer_sequential.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_group_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2581 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_manual_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3501 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_overpayment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_report_revision.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2989 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_reschedule_lines.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7240 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3373 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier_post_paid.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3986 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_tax_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3349 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_with_credit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3632 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:54.000000 trytond_account_invoice-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-29 15:14:09.000000 trytond_account_invoice-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.426892 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     6312 2024-04-29 15:33:33.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.426892 trytond_account_invoice-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-07-26 15:07:10.000000 trytond_account_invoice-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4830 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-03-15 08:41:28.000000 trytond_account_invoice-7.2.0/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/invoice_report_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/invoice_report_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/invoice_sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/invoice_sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/invoice_sequence_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_tax_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_tax_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-28 07:43:48.000000 trytond_account_invoice-7.2.0/view/invoice_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/move_line_list_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-26 15:26:42.000000 trytond_account_invoice-7.2.0/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/pay_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_method_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2024-03-17 11:01:36.000000 trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-03-17 11:01:36.000000 trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-03-17 11:01:36.000000 trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8236 2024-05-01 12:21:38.000000 trytond_account_invoice-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:21:38.000000 trytond_account_invoice-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1977 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14844 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4877 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.902370 trytond_account_invoice-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7303 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.902370 trytond_account_invoice-7.2.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/amend.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/prepare.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.902370 trytond_account_invoice-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/icons/tryton-invoice.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    94000 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/invoice.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)   139705 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23815 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.905703 trytond_account_invoice-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    38545 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40107 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33376 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40811 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39814 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34299 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37631 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41802 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33337 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40567 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35994 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35962 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36623 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39197 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37373 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39770 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34002 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36946 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39091 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39208 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38359 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33319 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31901 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38369 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6873 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3324 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2389 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/payment_term.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/payment_term.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.909037 trytond_account_invoice-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3122 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_cancelling_invoice_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4010 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_credit_note.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    13167 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6057 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_exchange.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_lower_rate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3488 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_rate_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternative_payee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2666 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_customer_sequential.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_group_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2581 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_manual_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3501 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_overpayment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_report_revision.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2989 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_reschedule_lines.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7240 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3373 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier_post_paid.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3986 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_tax_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3349 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_with_credit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3632 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11545 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-30 17:21:06.000000 trytond_account_invoice-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     6312 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4830 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_report_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_report_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_sequence_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tax_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tax_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_list_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/pay_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_method_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_tree.xml
```

### Comparing `trytond_account_invoice-7.2.0/CHANGELOG` & `trytond_account_invoice-7.2.1/CHANGELOG`

 * *Files 1% similar despite different names*

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
 * Raise a warning when validating invoice with non default taxes
 * Book currency exchange amount in dedicated account
 
 Version 7.0.0 - 2023-10-30
```

### Comparing `trytond_account_invoice-7.2.0/COPYRIGHT` & `trytond_account_invoice-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/LICENSE` & `trytond_account_invoice-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/PKG-INFO` & `trytond_account_invoice-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice-7.2.0/__init__.py` & `trytond_account_invoice-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/account.py` & `trytond_account_invoice-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/account.xml` & `trytond_account_invoice-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/company.py` & `trytond_account_invoice-7.2.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/doc/conf.py` & `trytond_account_invoice-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/doc/configuration.rst` & `trytond_account_invoice-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/doc/design.rst` & `trytond_account_invoice-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/doc/usage/amend.inc.rst` & `trytond_account_invoice-7.2.1/doc/usage/amend.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/doc/usage/prepare.inc.rst` & `trytond_account_invoice-7.2.1/doc/usage/prepare.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/doc/usage/process.inc.rst` & `trytond_account_invoice-7.2.1/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/exceptions.py` & `trytond_account_invoice-7.2.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/icons/LICENSE` & `trytond_account_invoice-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/invoice.fodt` & `trytond_account_invoice-7.2.1/invoice.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/invoice.py` & `trytond_account_invoice-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/invoice.xml` & `trytond_account_invoice-7.2.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/locale/bg.po` & `trytond_account_invoice-7.2.1/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -1053,14 +1053,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/ca.po` & `trytond_account_invoice-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -924,15 +924,15 @@
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
 msgid "Pending"
 msgstr "Pendent"
 
 msgctxt "model:ir.message,text:msg_cancel_invoice_move"
 msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
 msgstr ""
-"Els assentaments \"%(moves)s\" tenen com origen les factures "
+"Els assentaments \"%(moves)s\" tenen com a origen les factures "
 "comptabilitzades \"%(invoices)s\"."
 
 msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
 msgid ""
 "Cancelling them will reconcile the move lines thus paying the invoices. You "
 "might want to cancel the invoices first."
 msgstr ""
@@ -953,46 +953,50 @@
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "No podeu abonar la factura rectificativa \"%(invoice)s\" perquè no està "
 "comptabilitzada."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a currency exchange credit "
 "account for \"%(company)s\"."
 msgstr ""
-"Per poder comptabilitzar la factura \"%(invoice)s\" heu de definir una "
-"seqüència per l'exercici fical \"%(fiscalyear)s\"."
+"Per poder comptabilitzar la factura \"%(invoice)s\" heu de definir un compte"
+" haver de diferencies de canvi per l'empresa \"%(company)s\"."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a currency exchange debit "
 "account for \"%(company)s\"."
 msgstr ""
-"Per poder comptabilitzar la factura \"%(invoice)s\" heu de definir una "
-"seqüència per l'exercici fical \"%(fiscalyear)s\"."
+"Per poder comptabilitzar la factura \"%(invoice)s\" heu de definir un compte"
+" deure de diferencies de canvi per l'empresa \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "No podeu cancel·lar la factura de client \"%(invoice)s\" perquè està "
 "comptabilitzada i la configuració de l'empresa no ho permet."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "Les factures \"%(invoices)s\" tenen una data de facturació en el futur."
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+"Les factures \"%(invoices)s\" no tenen els impostos per defecte per les "
+"línies %(lines)s."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Heu de cancel·lar la factura \"%(invoice)s\" per poder-la eliminar."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "No podeu la factura \"%(invoice)s\" perquè està numerada."
@@ -1397,15 +1401,15 @@
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "view:account.invoice.payment_term.line.delta:"
 msgid "Operations are applied in this displayed order."
-msgstr ""
+msgstr "Les operacions s'apliquen en l'ordre mostrat."
 
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.2.0/locale/cs.po` & `trytond_account_invoice-7.2.1/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -511,31 +511,29 @@
 msgid "Debit Account"
 msgstr ""
 
 msgctxt "field:account.invoice.payment.method,journal:"
 msgid "Journal"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.payment.method,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:account.invoice.payment_term,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.payment_term,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:account.invoice.payment_term.line,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term.line,currency:"
 msgid "Currency"
@@ -623,18 +621,17 @@
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.invoice.report.revision,date:"
 msgid "Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,filename:"
 msgid "File Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.report.revision,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
 #, fuzzy
@@ -1007,14 +1004,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
@@ -1221,15 +1222,14 @@
 msgstr "Payment Terms"
 
 #, fuzzy
 msgctxt "model:party.party.payment_term,name:"
 msgid "Party Payment Term"
 msgstr "Test Payment Term"
 
-#, fuzzy
 msgctxt "report:account.invoice:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:account.invoice:"
 msgid "Amount"
 msgstr ""
@@ -1402,15 +1402,14 @@
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:account.invoice.payment_term.line.delta:"
 msgid "Operations are applied in this displayed order."
 msgstr ""
 
-#, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/de.po` & `trytond_account_invoice-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -957,47 +957,53 @@
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "Rechnung \"%(invoice)s\" kann nicht verrechnet werden, da sie noch nicht "
 "festgeschrieben wurde."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a currency exchange credit "
 "account for \"%(company)s\"."
 msgstr ""
-"Um Rechnung invoice \"%(invoice)s\" festschreiben zu können, muss ein "
-"Nummernkreis für das Geschäftsjahr \"%(fiscalyear)s\" definiert sein."
+"Um die Rechnung invoice \"%(invoice)s\" festschreiben zu können, muss für "
+"das Unternehmen \"%(company)s\" ein Habenkonto für Differenzen aus der "
+"Währungsumrechnung definiert sein."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a currency exchange debit "
 "account for \"%(company)s\"."
 msgstr ""
-"Um Rechnung invoice \"%(invoice)s\" festschreiben zu können, muss ein "
-"Nummernkreis für das Geschäftsjahr \"%(fiscalyear)s\" definiert sein."
+"Um die Rechnung invoice \"%(invoice)s\" festschreiben zu können, muss für "
+"das Unternehmen \"%(company)s\" ein Sollkonto für Differenzen aus der "
+"Währungsumrechnung definiert sein."
 
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Rechnung \"%(invoice)s\" kann nicht annulliert werden, da sie "
 "festgeschrieben ist und das Annullieren für das Unternehmen nicht zulässig "
 "ist."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "Die Rechnungen \"%(invoices)s\" haben ein Rechnungsdatum in der Zukunft."
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+"Bei der Rechnungsposition %(line)s der Rechnung \"%(invoices)s\" weichen die"
+" Steuern vom Standard ab."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 "Rechnung \"%(invoice)s\" muss annulliert werden, damit sie gelöscht werden "
 "kann."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
@@ -1063,16 +1069,16 @@
 "möglich."
 
 msgctxt "model:ir.message,text:msg_invoice_pay_amount_greater_amount_to_pay"
 msgid ""
 "You cannot add a partial payment on invoice \"%(invoice)s\" with an amount "
 "greater than the amount to pay \"%(amount_to_pay)s\"."
 msgstr ""
-"Für Rechnung \"%(invoice)s\" kann keine Teilzahlung mit einem Betrag erfasst"
-" werden, der höher ist als der zu zahlende Betrag."
+"Sie können keine Teilzahlung zur Rechnung \"%(invoice)s\" hinzufügen, wenn "
+"der Betrag höher ist als der zu zahlende Betrag \"%(amount_to_pay)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_line_unique"
 msgid "A payment line can be linked to only one invoice."
 msgstr ""
 "Eine Zahlungsposition kann nur einer einzigen Rechnung zugeordnet werden."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_lines_add_remove_paid"
@@ -1139,15 +1145,15 @@
 
 msgctxt "model:ir.message,text:msg_payment_term_missing_remainder"
 msgid ""
 "To compute terms, you must append a remainder line on payment term "
 "\"%(payment_term)s\"."
 msgstr ""
 "Damit die Berechnung durchgeführt werden kann, muss eine Position für den "
-"Restbetrag auf Zahlungsbedingung \"%(paxment_term)s\" erfasst werden."
+"Restbetrag auf der Zahlungsbedingung \"%(payment_term)s\" erfasst werden."
 
 msgctxt "model:ir.model.button,confirm:invoice_cancel_button"
 msgid "Are you sure you want to cancel the invoices?"
 msgstr "Wollen Sie die Rechnungen wirklich stornieren?"
 
 msgctxt "model:ir.model.button,confirm:invoice_post_button"
 msgid "Are you sure you want to post the invoices?"
@@ -1191,27 +1197,27 @@
 
 msgctxt "model:ir.model.button,string:invoice_validate_button"
 msgid "Validate"
 msgstr "Prüfen"
 
 msgctxt "model:ir.rule.group,name:rule_group_invoice_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_invoice_line_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_invoice_sequence_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_method_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_account_invoice"
 msgid "Invoice"
 msgstr "Rechnung"
 
 msgctxt "model:ir.ui.menu,name:menu_invoice_in_form"
 msgid "Supplier Invoices"
@@ -1411,15 +1417,15 @@
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notizen"
 
 msgctxt "view:account.invoice.payment_term.line.delta:"
 msgid "Operations are applied in this displayed order."
-msgstr ""
+msgstr "Die Angaben werden in der angezeigten Reihenfolge angewandt."
 
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.2.0/locale/es.po` & `trytond_account_invoice-7.2.1/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -924,16 +924,16 @@
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
 msgid "Pending"
 msgstr "Pendiente"
 
 msgctxt "model:ir.message,text:msg_cancel_invoice_move"
 msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
 msgstr ""
-"Los asientos \"(moves)s\" tiene como origen las facturas contabilizadas "
-"\"%(facturas)s\"."
+"Los asientos \"%(moves)s\" tiene como origen las facturas contabilizadas "
+"\"%(invoices)s\"."
 
 msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
 msgid ""
 "Cancelling them will reconcile the move lines thus paying the invoices. You "
 "might want to cancel the invoices first."
 msgstr ""
 "Al cancelar-los se conciliaran los apuntes i se pagaran las facturas. Quizas"
@@ -951,47 +951,51 @@
 "No puede eliminar el tercero \"%(party)s\" mientras tenga facturas "
 "pendientes con la companía \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr "No puede abonar la factura \"%(invoice)s\" porque no está contabilizada."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a currency exchange credit "
 "account for \"%(company)s\"."
 msgstr ""
-"Para contabilizar la factura \"%(invoice)s\", debe definir una secuencia "
-"para el ejercicio fiscal \"%(fiscalyear)s\"."
+"Para contabilizar la factura \"%(invoice)s\", debe definir una Cuenta haber "
+"diferencias de cambio para la empresa \"%(company)s\"."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a currency exchange debit "
 "account for \"%(company)s\"."
 msgstr ""
-"Para contabilizar la factura \"%(invoice)s\", debe definir una secuencia "
-"para el ejercicio fiscal \"%(fiscalyear)s\"."
+"Para contabilizar la factura \"%(invoice)s\", debe definir una Cuenta debe "
+"diferencias de cambio para la empresa \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "No puede cancelar la factura de cliente \"%(invoice)s\" porque está "
 "contabilizada y la configuración de la empresa no lo permite."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 "Las facturas \"%(invoices)s\" tienen una fecha de facturación en el futuro."
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+"Las facturas \"%(invoices)s\" no tiene los impuestos por defecto para "
+"%(lines)s."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Para eliminar la factura \"%(invoice)s\" debe cancelarla."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "No puede eliminar la factura \"%(invoice)s\" porque está numerada."
@@ -1396,15 +1400,15 @@
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notas"
 
 msgctxt "view:account.invoice.payment_term.line.delta:"
 msgid "Operations are applied in this displayed order."
-msgstr ""
+msgstr "La operaciones se ejecutan en el orden mostrado."
 
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.2.0/locale/es_419.po` & `trytond_account_invoice-7.2.1/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -994,14 +994,18 @@
 "No puede agregar el impuesto a la factura \"%(invoice)s\" porque está "
 "contabilizada, pagada o cancelada."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/et.po` & `trytond_account_invoice-7.2.1/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -1014,14 +1014,18 @@
 "company setup does not allow it."
 msgstr "Kliendiarvet \"%(arve)id\" ei saa tühistada, kuna need on postitatud."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Arve \"%(arve)te\" kustutamiseks tuleb see tühistada."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Arvet \"%(arve)id\" ei saa kustutada, kuna sellel on number."
```

### Comparing `trytond_account_invoice-7.2.0/locale/fa.po` & `trytond_account_invoice-7.2.1/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -1020,14 +1020,18 @@
 "شما نمیتوانید صورتحساب مشتری : \"%(invoice)s\" را لغو کنید، چراکه آن ارسال "
 "شده است."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "برای حذف صورتحساب : \"%(invoice)s\" شما باید آنرا لغو کنید."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/fi.po` & `trytond_account_invoice-7.2.1/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -1004,14 +1004,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/fr.po` & `trytond_account_invoice-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -983,15 +983,20 @@
 "company setup does not allow it."
 msgstr ""
 "Vous ne pouvez pas annuler la facture client « %(invoice)s » car elle est "
 "comptabilisée et la configuration de la société ne le permet pas."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
-msgstr "La facture « %(invoice)s » a une date de facture dans le futur."
+msgstr "La facture « %(invoices)s » a une date de facture dans le futur."
+
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+"La facture « %(invoice)s » n'a pas les taxes par défaut pour %(line)s."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Pour supprimer la facture « %(invoice)s », vous devez l'annuler."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
```

### Comparing `trytond_account_invoice-7.2.0/locale/hu.po` & `trytond_account_invoice-7.2.1/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,14 +999,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/id.po` & `trytond_account_invoice-7.2.1/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -999,14 +999,21 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 "Faktur \"%(invoice)s\" menghasilkan tanggal pembayaran \"%(date)s\" di masa "
 "lampau."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+"Faktur \"%(invoice)s\" menghasilkan tanggal pembayaran \"%(date)s\" di masa "
+"lampau."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Untuk menghapus faktur \"%(invoice)s\" Anda harus membatalkannya."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Anda tidak dapat menghapus faktur \"%(invoice)s\" karena memiliki nomor."
```

### Comparing `trytond_account_invoice-7.2.0/locale/it.po` & `trytond_account_invoice-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -1021,14 +1021,18 @@
 "Non puoi aggiungere/variare l'imposta nella fattura \"%(invoice)s\" perché è"
 " stata registrata, pagata o cancellata."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/lo.po` & `trytond_account_invoice-7.2.1/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -1070,14 +1070,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/lt.po` & `trytond_account_invoice-7.2.1/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -1005,14 +1005,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/nl.po` & `trytond_account_invoice-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -944,16 +944,16 @@
 msgstr "Om de periodes af te sluiten moet u de facturen \"%(invoices)s\" boeken."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
 "company \"%(company)s\"."
 msgstr ""
-"U kunt de relatie \"% (party)s\" niet verwijderen terwijl ze facturen hebben"
-" die in behandeling zijn bij bedrijf \"%(company)s\"."
+"U kunt de relatie \"%(party)s\" niet verwijderen terwijl ze facturen hebben "
+"die in behandeling zijn bij bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "U kunt de factuur \"%(invoice)s\" niet terugbetalen omdat ze niet geboekt "
 "is."
 
@@ -976,24 +976,30 @@
 "grootboekrekening voor de wisselkoers definiëren voor \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
-"U kunt klant factuur \"% (invoice)s\" niet annuleren omdat deze is geboekt "
-"en de bedrijfsinstellingen dit niet toelaten."
+"U kunt klant factuur \"%(invoice)s\" niet annuleren omdat deze is geboekt en"
+" de bedrijfsinstellingen dit niet toelaten."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "De facturen \"%(invoices)s\" hebben een factuurdatum in de toekomst."
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+"De factuur \"%(invoice)s\" heeft niet de standaard belastingen voor "
+"%(lines)s."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
-msgstr "Om de factuur \"% (invoice)s\" te verwijderen, moet u deze annuleren."
+msgstr "Om de factuur \"%(invoice)s\" te verwijderen, moet u deze annuleren."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 "U kunt factuur \"%(invoice)s\" niet verwijderen omdat deze een nummer heeft."
 
 msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
@@ -1027,15 +1033,15 @@
 
 msgctxt "model:ir.message,text:msg_invoice_no_sequence"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a sequence on fiscal year "
 "\"%(fiscalyear)s\"."
 msgstr ""
 "Om factuur \"%(invoice)s\" te kunnen boeken, moet u een reeks definiëren in "
-"het fiscale jaar \"% (fiscaal jaar)\"."
+"het fiscale jaar \"%(fiscalyear)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_number_after"
 msgid ""
 "To number the invoice \"%(invoice)s\", you must set an invoice date after "
 "\"%(date)s\" because the sequence \"%(sequence)s\" has already been used for"
 " invoice \"%(after_invoice)s\"."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/pl.po` & `trytond_account_invoice-7.2.1/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -1024,14 +1024,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/pt.po` & `trytond_account_invoice-7.2.1/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1034,14 +1034,18 @@
 "Você não pode adicionar a linha \"%(line)s\" à fatura \"%(invoice)s\" porque"
 " ela já foi confirmada, paga ou cancelada."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/ro.po` & `trytond_account_invoice-7.2.1/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -981,14 +981,19 @@
 "Nu se poate anula factura de client \"%(invoice)s\" pentru că este postata "
 "şi configurarea companiei nu permite acest lucru."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "Facturile \"%(invoices)s\" au o data în viitor."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr "Facturile \"%(invoices)s\" au o data în viitor."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Pentru a şterge factura \"%(invoice)s\" trebuie anulata."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Nu se poate şterge factura \"%(invoice)s\" pentru că are un număr."
```

### Comparing `trytond_account_invoice-7.2.0/locale/ru.po` & `trytond_account_invoice-7.2.1/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -1057,14 +1057,18 @@
 "Вы не можете добавить строчку \"%(line)s\" в инвойс \"%(invoice)s\" так как "
 "он \"Отправлен\", \"Оплачен\" или \"Отменен\"."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/sl.po` & `trytond_account_invoice-7.2.1/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -993,14 +993,19 @@
 "Ni mogoče preklicati fakture kupca \"%(invoice)s\", saj je knjižena. "
 "Nastavitve podjetja ne dovoljujejo preklica faktur."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "Fakture \"%(invoice)s\" imajo datum v prihodnosti."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr "Fakture \"%(invoice)s\" imajo datum v prihodnosti."
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 "Fakturo \"%(invoice)s\" je potrebno preklicati, preden jo je mogoče brisati."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
```

### Comparing `trytond_account_invoice-7.2.0/locale/tr.po` & `trytond_account_invoice-7.2.1/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -511,29 +511,31 @@
 msgid "Debit Account"
 msgstr ""
 
 msgctxt "field:account.invoice.payment.method,journal:"
 msgid "Journal"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.payment.method,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:account.invoice.payment_term,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.payment_term,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:account.invoice.payment_term.line,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term.line,currency:"
 msgid "Currency"
@@ -621,17 +623,18 @@
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.invoice.report.revision,date:"
 msgid "Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.report.revision,filename:"
 msgid "File Name"
-msgstr ""
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:account.invoice.report.revision,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
 #, fuzzy
@@ -1004,14 +1007,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
@@ -1218,14 +1225,15 @@
 msgstr "Payment Terms"
 
 #, fuzzy
 msgctxt "model:party.party.payment_term,name:"
 msgid "Party Payment Term"
 msgstr "Test Payment Term"
 
+#, fuzzy
 msgctxt "report:account.invoice:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:account.invoice:"
 msgid "Amount"
 msgstr ""
@@ -1398,14 +1406,15 @@
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:account.invoice.payment_term.line.delta:"
 msgid "Operations are applied in this displayed order."
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/uk.po` & `trytond_account_invoice-7.2.1/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -965,14 +965,18 @@
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
```

### Comparing `trytond_account_invoice-7.2.0/locale/zh_CN.po` & `trytond_account_invoice-7.2.1/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -971,14 +971,19 @@
 "company setup does not allow it."
 msgstr "无法取消客户原始凭证 \"%(invoice)s\"，因为它已过帐并且公司设置不允许。"
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "原始凭证 \"%(invoices)s\" 的日期指向未来。"
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_default_taxes"
+msgid "The invoice \"%(invoice)s\" does not have the default taxes for %(lines)s."
+msgstr "原始凭证 \"%(invoices)s\" 的日期指向未来。"
+
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "删除原始凭证 \"%(invoice)s\" 之前必须先取消它。"
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "无法删除原始凭证 \"%(invoice)s\" ，因为它包含序号。"
```

### Comparing `trytond_account_invoice-7.2.0/message.xml` & `trytond_account_invoice-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/party.py` & `trytond_account_invoice-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/party.xml` & `trytond_account_invoice-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/payment_term.py` & `trytond_account_invoice-7.2.1/payment_term.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/payment_term.xml` & `trytond_account_invoice-7.2.1/payment_term.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/setup.py` & `trytond_account_invoice-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_cancelling_invoice_move.rst` & `trytond_account_invoice-7.2.1/tests/scenario_cancelling_invoice_move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_credit_note.rst` & `trytond_account_invoice-7.2.1/tests/scenario_credit_note.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_exchange.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_exchange.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_lower_rate.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_lower_rate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_rate_change.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_rate_change.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternative_payee.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternative_payee.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_customer_sequential.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_customer_sequential.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_group_line.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_group_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_in_future.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_in_future.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_manual_tax.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_manual_tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_overpayment.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_overpayment.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_report_revision.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_report_revision.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_reschedule_lines.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_reschedule_lines.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier_post_paid.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier_post_paid.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_tax_deductible.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_tax_deductible.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_invoice_with_credit.rst` & `trytond_account_invoice-7.2.1/tests/scenario_invoice_with_credit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/scenario_renew_fiscalyear.rst` & `trytond_account_invoice-7.2.1/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/test_module.py` & `trytond_account_invoice-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tests/tools.py` & `trytond_account_invoice-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/tox.ini` & `trytond_account_invoice-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/PKG-INFO` & `trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/SOURCES.txt` & `trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/credit_start_form.xml` & `trytond_account_invoice-7.2.1/view/credit_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_form.xml` & `trytond_account_invoice-7.2.1/view/invoice_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_line_form.xml` & `trytond_account_invoice-7.2.1/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_line_tree.xml` & `trytond_account_invoice-7.2.1/view/invoice_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_line_tree_sequence.xml` & `trytond_account_invoice-7.2.1/view/invoice_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_sequence_form.xml` & `trytond_account_invoice-7.2.1/view/invoice_sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_tax_form.xml` & `trytond_account_invoice-7.2.1/view/invoice_tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_tax_tree_sequence.xml` & `trytond_account_invoice-7.2.1/view/invoice_tax_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/invoice_tree.xml` & `trytond_account_invoice-7.2.1/view/invoice_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/move_line_list_payment.xml` & `trytond_account_invoice-7.2.1/view/move_line_list_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/party_form.xml` & `trytond_account_invoice-7.2.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/pay_ask_form.xml` & `trytond_account_invoice-7.2.1/view/pay_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/pay_start_form.xml` & `trytond_account_invoice-7.2.1/view/pay_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/payment_method_form.xml` & `trytond_account_invoice-7.2.1/view/payment_method_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/payment_term_form.xml` & `trytond_account_invoice-7.2.1/view/payment_term_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/payment_term_line_form.xml` & `trytond_account_invoice-7.2.1/view/payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_form.xml` & `trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_form.xml`

 * *Files identical despite different names*

