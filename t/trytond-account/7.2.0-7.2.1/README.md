# Comparing `tmp/trytond_account-7.2.0.tar.gz` & `tmp/trytond_account-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account-7.2.0.tar", last modified: Mon Apr 29 15:31:25 2024, max compression
+gzip compressed data, was "trytond_account-7.2.1.tar", last modified: Wed May  1 12:38:35 2024, max compression
```

## Comparing `trytond_account-7.2.0.tar` & `trytond_account-7.2.1.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.416906 trytond_account-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)    10737 2024-04-29 15:12:38.000000 trytond_account-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:12:38.000000 trytond_account-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-29 15:31:25.413573 trytond_account-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-25 11:39:10.000000 trytond_account-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-01-27 09:58:52.000000 trytond_account-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)   129467 2024-04-27 16:30:39.000000 trytond_account-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46672 2024-04-27 16:30:39.000000 trytond_account-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-01-16 14:00:20.000000 trytond_account-7.2.0/aged_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-04-15 07:12:14.000000 trytond_account-7.2.0/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6045 2024-01-27 09:58:52.000000 trytond_account-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3024 2024-04-27 16:30:39.000000 trytond_account-7.2.0/company.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8831 2024-01-27 09:58:52.000000 trytond_account-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-27 16:30:39.000000 trytond_account-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.396907 trytond_account-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-15 07:12:14.000000 trytond_account-7.2.0/doc/configuration.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.396907 trytond_account-7.2.0/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/account.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/configuration.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/fiscal-year.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2246 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/journal.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/move.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/tax.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/template.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-25 11:39:10.000000 trytond_account-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-04-15 07:12:14.000000 trytond_account-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.396907 trytond_account-7.2.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/close.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/create.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/report.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/structure.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/view.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2024-04-22 12:14:36.000000 trytond_account-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26581 2024-03-17 11:01:35.000000 trytond_account-7.2.0/fiscalyear.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7424 2024-04-27 16:30:39.000000 trytond_account-7.2.0/fiscalyear.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-04-15 07:12:14.000000 trytond_account-7.2.0/general_journal.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81559 2024-02-04 18:51:26.000000 trytond_account-7.2.0/general_ledger.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.400240 trytond_account-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/tryton-account-block.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/tryton-account-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/tryton-account-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-01-16 14:00:20.000000 trytond_account-7.2.0/icons/tryton-account.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13491 2024-04-27 16:30:39.000000 trytond_account-7.2.0/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12289 2024-04-27 16:30:39.000000 trytond_account-7.2.0/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.400240 trytond_account-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   130819 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130189 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)   114018 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   133816 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130504 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118696 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)   126852 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   138321 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)   117810 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132544 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125268 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)   116922 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122609 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)   142915 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)   134510 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130863 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122016 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125178 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   129562 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132756 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122826 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   113850 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   147710 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125787 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account-7.2.0/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)    17448 2024-03-17 11:01:36.000000 trytond_account-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22110 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11303 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11058 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11004 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11069 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11050 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11083 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11090 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11405 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11056 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   116642 2024-04-27 16:37:33.000000 trytond_account-7.2.0/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26295 2024-04-27 16:30:39.000000 trytond_account-7.2.0/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15750 2024-02-04 18:51:26.000000 trytond_account-7.2.0/move_template.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6717 2024-04-27 16:30:39.000000 trytond_account-7.2.0/move_template.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13726 2024-04-27 16:30:39.000000 trytond_account-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4156 2024-04-27 16:30:39.000000 trytond_account-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16319 2024-03-17 11:01:36.000000 trytond_account-7.2.0/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4083 2024-04-27 16:30:39.000000 trytond_account-7.2.0/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:25.416906 trytond_account-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-04-27 16:30:39.000000 trytond_account-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    70885 2024-04-27 16:30:39.000000 trytond_account-7.2.0/tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24263 2024-04-27 16:30:39.000000 trytond_account-7.2.0/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.403574 trytond_account-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4618 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_active.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-03-17 11:01:36.000000 trytond_account-7.2.0/tests/scenario_account_reconcile.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3995 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconcile.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconcile_automatic.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-02-04 18:51:26.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-02-04 18:51:26.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency_write_off.json
--rw-r--r--   0 ced       (1000) ced       (1000)     4420 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4736 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_close_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_cancel.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_line_delegate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5021 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_line_group.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4907 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_line_reschedule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4796 2024-04-27 16:37:33.000000 trytond_account-7.2.0/tests/scenario_move_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10860 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_reports.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_tax_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    80138 2024-04-27 16:30:39.000000 trytond_account-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-07-29 12:33:26.000000 trytond_account-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4788 2024-01-27 09:58:52.000000 trytond_account-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-04-15 07:12:14.000000 trytond_account-7.2.0/trial_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-29 15:12:34.000000 trytond_account-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.413573 trytond_account-7.2.0/trytond_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    12499 2024-04-29 15:31:25.000000 trytond_account-7.2.0/trytond_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account-7.2.0/trytond_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-04-15 07:12:14.000000 trytond_account-7.2.0/type_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.413573 trytond_account-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_deferral_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_deferral_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_list_balance_sheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/aged_balance_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/aged_balance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/balance_sheet_context_comparison_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1353 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/create_chart_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/create_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/fiscalyear_balance_non_deferral_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/general_ledger_account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/general_ledger_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/general_ledger_account_party_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/general_ledger_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/general_ledger_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-02-12 22:20:37.000000 trytond_account-7.2.0/view/journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/journal_list_cash.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_list_matching_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/journal_open_cash_context.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_cancel_default_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_delegate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1753 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_group_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_list_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_list_reconcile.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_line_receivable_payable_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_reschedule_preview_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_reschedule_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_reschedule_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1026 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      636 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_tree_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_reconciliation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_reconciliation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_template_create_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      857 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_template_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_template_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_template_keyword_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/open_journal_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/reconcile_lines_writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      755 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/reconcile_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/reconcile_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/renew_fiscalyear_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_group_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_rule_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/update_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/update_chart_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/writeoff_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.875851 trytond_account-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10838 2024-05-01 12:38:32.000000 trytond_account-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:38:32.000000 trytond_account-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-05-01 12:38:35.875851 trytond_account-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-04-30 17:20:59.000000 trytond_account-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   129467 2024-04-30 17:20:59.000000 trytond_account-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46672 2024-04-30 17:20:59.000000 trytond_account-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    51736 2024-04-30 17:20:59.000000 trytond_account-7.2.1/aged_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:20:59.000000 trytond_account-7.2.1/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6045 2024-04-30 17:20:59.000000 trytond_account-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3024 2024-04-30 17:20:59.000000 trytond_account-7.2.1/company.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8831 2024-04-30 17:20:59.000000 trytond_account-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-30 17:20:59.000000 trytond_account-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/configuration.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/account.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/configuration.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/fiscal-year.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2246 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/journal.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/move.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/tax.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/template.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1558 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/close.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/create.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/report.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/structure.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/view.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1808 2024-04-30 17:20:59.000000 trytond_account-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26581 2024-04-30 17:20:59.000000 trytond_account-7.2.1/fiscalyear.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7424 2024-04-30 17:20:59.000000 trytond_account-7.2.1/fiscalyear.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52160 2024-04-30 17:20:59.000000 trytond_account-7.2.1/general_journal.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81559 2024-04-30 17:20:59.000000 trytond_account-7.2.1/general_ledger.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account-block.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13491 2024-04-30 17:20:59.000000 trytond_account-7.2.1/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12289 2024-04-30 17:20:59.000000 trytond_account-7.2.1/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.862517 trytond_account-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   131048 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130583 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   114241 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   134193 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130891 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   118935 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   127139 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   138558 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   118048 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132823 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125558 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   117226 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122882 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   143189 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   134790 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   131232 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122265 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125426 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129848 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   133001 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   123107 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   114073 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   148010 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   126059 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2024-04-30 17:20:59.000000 trytond_account-7.2.1/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)    17448 2024-04-30 17:21:06.000000 trytond_account-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22110 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11303 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11058 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11004 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11069 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11050 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11083 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11090 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11405 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11056 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   116642 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26295 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15750 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move_template.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6717 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move_template.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13726 2024-04-30 17:20:59.000000 trytond_account-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4156 2024-04-30 17:20:59.000000 trytond_account-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16319 2024-04-30 17:20:59.000000 trytond_account-7.2.1/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4083 2024-04-30 17:20:59.000000 trytond_account-7.2.1/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:38:35.875851 trytond_account-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-04-30 17:20:59.000000 trytond_account-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    70885 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24263 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.865851 trytond_account-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4618 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_active.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconcile.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3995 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconcile.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconcile_automatic.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency_write_off.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     4420 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4736 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_close_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_cancel.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_line_delegate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5021 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_line_group.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4907 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_line_reschedule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4796 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10860 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_reports.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_tax_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    80138 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4788 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)    47972 2024-04-30 17:20:59.000000 trytond_account-7.2.1/trial_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:06.000000 trytond_account-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.875851 trytond_account-7.2.1/trytond_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    12499 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    54595 2024-04-30 17:20:59.000000 trytond_account-7.2.1/type_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.875851 trytond_account-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_deferral_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_deferral_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_list_balance_sheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1074 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/aged_balance_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/aged_balance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/balance_sheet_context_comparison_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      710 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1353 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/create_chart_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/create_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_balance_non_deferral_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      910 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_account_party_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1138 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_list_cash.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_list_matching_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_open_cash_context.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_cancel_default_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_delegate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1753 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1241 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_group_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_list_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_list_reconcile.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_receivable_payable_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_reschedule_preview_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_reschedule_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_reschedule_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1026 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      636 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_tree_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_reconciliation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_reconciliation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_create_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      857 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_keyword_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/open_journal_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/reconcile_lines_writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      755 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/reconcile_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/reconcile_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/renew_fiscalyear_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_group_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2101 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      250 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/update_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/update_chart_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/writeoff_tree.xml
```

### Comparing `trytond_account-7.2.0/CHANGELOG` & `trytond_account-7.2.1/CHANGELOG`

 * *Files 2% similar despite different names*

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
 * Convert recursive calls of reconcile accounts wizard into loop
 * Remove active field on journal - period
 * Allow modifying period dates with moves
```

### Comparing `trytond_account-7.2.0/COPYRIGHT` & `trytond_account-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/LICENSE` & `trytond_account-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/PKG-INFO` & `trytond_account-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account-7.2.0/__init__.py` & `trytond_account-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/account.py` & `trytond_account-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/account.xml` & `trytond_account-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/aged_balance.fodt` & `trytond_account-7.2.1/aged_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/common.py` & `trytond_account-7.2.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/company.py` & `trytond_account-7.2.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/company.xml` & `trytond_account-7.2.1/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/configuration.py` & `trytond_account-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/configuration.xml` & `trytond_account-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/conf.py` & `trytond_account-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/configuration.rst` & `trytond_account-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/account.inc.rst` & `trytond_account-7.2.1/doc/design/account.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/configuration.inc.rst` & `trytond_account-7.2.1/doc/design/configuration.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/fiscal-year.inc.rst` & `trytond_account-7.2.1/doc/design/fiscal-year.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/journal.inc.rst` & `trytond_account-7.2.1/doc/design/journal.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/move.inc.rst` & `trytond_account-7.2.1/doc/design/move.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/tax.inc.rst` & `trytond_account-7.2.1/doc/design/tax.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/design/template.inc.rst` & `trytond_account-7.2.1/doc/design/template.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/reference.rst` & `trytond_account-7.2.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/setup.rst` & `trytond_account-7.2.1/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/usage/close.inc.rst` & `trytond_account-7.2.1/doc/usage/close.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/usage/create.inc.rst` & `trytond_account-7.2.1/doc/usage/create.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/usage/process.inc.rst` & `trytond_account-7.2.1/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/usage/report.inc.rst` & `trytond_account-7.2.1/doc/usage/report.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/usage/structure.inc.rst` & `trytond_account-7.2.1/doc/usage/structure.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/doc/usage/view.inc.rst` & `trytond_account-7.2.1/doc/usage/view.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/exceptions.py` & `trytond_account-7.2.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/fiscalyear.py` & `trytond_account-7.2.1/fiscalyear.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/fiscalyear.xml` & `trytond_account-7.2.1/fiscalyear.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/general_journal.fodt` & `trytond_account-7.2.1/general_journal.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/general_ledger.fodt` & `trytond_account-7.2.1/general_ledger.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/icons/LICENSE` & `trytond_account-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/journal.py` & `trytond_account-7.2.1/journal.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/journal.xml` & `trytond_account-7.2.1/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/locale/bg.po` & `trytond_account-7.2.1/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -1326,14 +1326,19 @@
 msgstr "Крайна дата"
 
 #, fuzzy
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Начална дата"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Фирма"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Икона"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Дневник"
@@ -4054,14 +4059,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -4099,14 +4113,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5227,24 +5245,14 @@
 msgid "Periods"
 msgstr "Периоди"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Последователности"
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Затваряне"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/ca.po` & `trytond_account-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:account.account,active:"
 msgid "Active"
 msgstr "Actiu"
 
 msgctxt "field:account.account,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.account,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account,childs:"
 msgid "Children"
@@ -104,15 +104,15 @@
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Dreta"
 
 msgctxt "field:account.account,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data inicial"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -152,15 +152,15 @@
 
 msgctxt "field:account.account.deferral,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.account.deferral,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.account.deferral,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account.deferral,credit:"
 msgid "Credit"
@@ -180,27 +180,27 @@
 
 msgctxt "field:account.account.deferral,line_count:"
 msgid "Line Count"
 msgstr "Nombre de línies"
 
 msgctxt "field:account.account.deferral,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.account.party,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.account.party,active:"
 msgid "Active"
 msgstr "Actiu"
 
 msgctxt "field:account.account.party,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.account.party,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account.party,closed:"
 msgid "Closed"
@@ -248,15 +248,15 @@
 
 msgctxt "field:account.account.party,party:"
 msgid "Party"
 msgstr "Tercer"
 
 msgctxt "field:account.account.party,second_currency:"
 msgid "Secondary Currency"
-msgstr "Moneda secundària"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.account.party,start_date:"
 msgid "Start Date"
 msgstr "Data inicial"
 
 msgctxt "field:account.account.party,type:"
 msgid "Type"
@@ -937,15 +937,15 @@
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Compte del tercer"
 
 msgctxt "field:account.general_ledger.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
@@ -1001,15 +1001,15 @@
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliació"
 
 msgctxt "field:account.general_ledger.line,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
@@ -1143,14 +1143,18 @@
 msgid "End Date"
 msgstr "Data final"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Data inicial"
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Empresa"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Icona"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Diari"
@@ -1241,15 +1245,15 @@
 
 msgctxt "field:account.move.line,amount_currency:"
 msgid "Amount Currency"
 msgstr "Moneda de l'import"
 
 msgctxt "field:account.move.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.move.line,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.move.line,credit:"
 msgid "Credit"
@@ -1333,19 +1337,19 @@
 
 msgctxt "field:account.move.line,reconciliations_delegated:"
 msgid "Reconciliations Delegated"
 msgstr "Conciliacions delegades"
 
 msgctxt "field:account.move.line,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.move.line,second_currency_required:"
 msgid "Second Currency Required"
-msgstr "Segona moneda obligatòria"
+msgstr "Moneda secundaria obligatòria"
 
 msgctxt "field:account.move.line,state:"
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:account.move.line,tax_lines:"
 msgid "Tax Lines"
@@ -2332,15 +2336,15 @@
 msgstr ""
 "Força a tots els assentaments d'aquest compte a tenir aquesta moneda "
 "secundària."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default taxes for documents to be applied when there is no other source."
-msgstr ""
+msgstr "Impostos per defecte que s'aplicaran quan no hi hagi una altra font."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Marca per sobreescriure la definició de la plantilla"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -2442,23 +2446,23 @@
 
 msgctxt "help:account.move.cancel.default,reversal:"
 msgid "Reverse debit and credit."
 msgstr "Inverteix deure i haber."
 
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
-msgstr "L'import expressat en la segona moneda."
+msgstr "L'import expressat en la moneda secundaria."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Establiu una data per fer el apunt pagable o cobrable."
 
 msgctxt "help:account.move.line,second_currency:"
 msgid "The second currency."
-msgstr "La segona moneda."
+msgstr "La moneda secundaria."
 
 msgctxt "help:account.move.line.reschedule.start,interval:"
 msgid "The length of each period, in months."
 msgstr "La longitud en mesos de cada període."
 
 msgctxt "help:account.move.line.template,amount:"
 msgid "A python expression that will be evaluated with the keywords."
@@ -3177,32 +3181,32 @@
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr "No podeu tancar el compte \"%(account)s\" perquè té apunts."
 
 msgctxt "model:ir.message,text:msg_account_invalid_deferral_second_currency"
 msgid "To set a second currency for account \"%(account)s\", it must be deferral."
 msgstr ""
-"Per establir una segona divisa al compte \"%(account)s\", ha de ser de "
+"Per establir una moneda secundaria al compte \"%(account)s\", ha de ser de "
 "tancament."
 
 msgctxt "model:ir.message,text:msg_account_invalid_lines_second_currency"
 msgid ""
 "To set a second currency for account \"%(account)s\", its lines must have "
 "the same second currency \"%(currency)s\"."
 msgstr ""
-"Per establir una segona divisa al compte \"%(account)s\", els seus apunts "
-"han de tenir la mateixa segona divisa \"%(currency)s\"."
+"Per establir una moneda secundaria al compte \"%(account)s\", els seus "
+"apunts han de tenir la mateixa segona divisa \"%(currency)s\"."
 
 msgctxt "model:ir.message,text:msg_account_invalid_type_second_currency"
 msgid ""
 "To set a second currency for account \"%(account)s\", it must not have a "
 "type \"payable\", \"revenue\", \"receivable\" nor \"expense\"."
 msgstr ""
-"Per assignar una segona moneda al compte \"%(account)s\", aquest no ha de "
-"ser del tipus \"A pagar\", \"Ingressos\", \"A cobrar\" o \"Despeses\"."
+"Per assignar una moneda secundaria al compte \"%(account)s\", aquest no ha "
+"de ser del tipus \"A pagar\", \"Ingressos\", \"A cobrar\" o \"Despeses\"."
 
 msgctxt "model:ir.message,text:msg_account_no_type_lines"
 msgid ""
 "You cannot remove type of account \"%(account)s\" because it has move lines."
 msgstr "No podeu eliminar el tipus de compte \"%(account)s\" perquè té apunts."
 
 msgctxt "model:ir.message,text:msg_cancel_line_delegated"
@@ -3332,15 +3336,15 @@
 
 msgctxt "model:ir.message,text:msg_group_line_same_company"
 msgid "You cannot group lines of different companies."
 msgstr "No podeu agrupar línies d'empreses diferents."
 
 msgctxt "model:ir.message,text:msg_group_line_same_second_currency"
 msgid "You cannot group lines of different second currencies."
-msgstr "No podeu agrupar línies amb segones monedes diferents."
+msgstr "No podeu agrupar línies amb monedes secundaries diferents."
 
 msgctxt "model:ir.message,text:msg_group_line_single"
 msgid "You cannot group a single line."
 msgstr "No podeu agrupar una sola línia."
 
 msgctxt "model:ir.message,text:msg_journal_account_moves"
 msgid ""
@@ -3387,15 +3391,16 @@
 " línia \"%(line)s\"."
 
 msgctxt "model:ir.message,text:msg_line_second_currency_sign"
 msgid ""
 "You must set the sign for second currency to match the sign of debit - "
 "credit."
 msgstr ""
-"El signe de la segona moneda ha de coincidir amb el signe del deure - haver."
+"El signe de la moneda secundaria ha de coincidir amb el signe del deure - "
+"haver."
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "No es pot modificar o eliminar el diari-període \"%(journal_period)s\" "
@@ -3529,22 +3534,21 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Les dates del període \"%(period)s\" ha d'estar dins de les dates del seu "
 "exercici fiscal \"%(fiscalyear)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_period_move_dates"
 msgid ""
 "The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
 "of move \"%(move)s\"."
 msgstr ""
-"Les dates del període \"%(period)s\" ha d'estar dins de les dates del seu "
-"exercici fiscal \"%(fiscalyear)s\"."
+"Les dates del període \"%(period)s\" han d'incloure la data "
+"\"%(move_date)s\" del assentament \"%(move)s\"."
 
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "El períodes \"%(first)s\" i \"%(second)s\" es sobreposen, heu d'utilitzar "
@@ -3725,14 +3729,22 @@
 msgid "Lock"
 msgstr "Bloqueja"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Torna a obrir"
 
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Tanca"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr "Torna a obrir"
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Comptabilitza"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Tanca"
@@ -3770,14 +3782,18 @@
 msgid "User in companies"
 msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Usuari a les empreses"
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Usuari a les empreses"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "Usuari a les empreses"
@@ -4759,22 +4775,14 @@
 msgid "Periods"
 msgstr "Períodes"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Seqüències"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Tanca"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Torna a obrir"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "cada"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "mesos"
```

### Comparing `trytond_account-7.2.0/locale/cs.po` & `trytond_account-7.2.1/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -1224,14 +1224,18 @@
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr ""
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr ""
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
@@ -3831,14 +3835,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -3876,14 +3889,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -4922,24 +4939,14 @@
 msgid "Periods"
 msgstr "Periods"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr ""
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Close"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr ""
```

### Comparing `trytond_account-7.2.0/locale/de.po` & `trytond_account-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 msgctxt "field:account.account,end_date:"
 msgid "End Date"
 msgstr "Enddatum"
 
 msgctxt "field:account.account,general_ledger_balance:"
 msgid "General Ledger Balance"
-msgstr "Kontenblattsaldo"
+msgstr "Saldoanzeige Kontenblätter"
 
 msgctxt "field:account.account,left:"
 msgid "Left"
 msgstr "Links"
 
 msgctxt "field:account.account,line_count:"
 msgid "Line Count"
@@ -288,15 +288,15 @@
 
 msgctxt "field:account.account.template,end_date:"
 msgid "End Date"
 msgstr "Enddatum"
 
 msgctxt "field:account.account.template,general_ledger_balance:"
 msgid "General Ledger Balance"
-msgstr "Kontenblattsaldo"
+msgstr "Saldoanzeige Kontenblätter"
 
 msgctxt "field:account.account.template,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:account.account.template,parent:"
 msgid "Parent"
@@ -801,15 +801,15 @@
 
 msgctxt "field:account.general_ledger.account,end_debit:"
 msgid "End Debit"
 msgstr "Soll bei Ende"
 
 msgctxt "field:account.general_ledger.account,general_ledger_balance:"
 msgid "General Ledger Balance"
-msgstr "Kontenblattsaldo"
+msgstr "Saldoanzeige Kontenblätter"
 
 msgctxt "field:account.general_ledger.account,line_count:"
 msgid "Line Count"
 msgstr "Anzahl Buchungspositionen"
 
 msgctxt "field:account.general_ledger.account,lines:"
 msgid "Lines"
@@ -1143,14 +1143,18 @@
 msgid "End Date"
 msgstr "Enddatum"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Startdatum"
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Unternehmen"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Icon"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Journal"
@@ -2317,28 +2321,30 @@
 msgid "The type used if not empty and debit > credit."
 msgstr ""
 "Dieser Typ wird genutzt, sofern er erfasst wurde und der Kontensaldo im Soll"
 " steht."
 
 msgctxt "help:account.account,general_ledger_balance:"
 msgid "Display only the balance in the general ledger report."
-msgstr "Nur Salden in Kontenblättern anzeigen."
+msgstr "Nur Salden auf Kontenblättern anzeigen."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Buchungszeilen dieses Kontos können abgestimmt werden."
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "Für alle Buchungen auf dieses Konto diese Fremdwährung verwenden."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default taxes for documents to be applied when there is no other source."
 msgstr ""
+"Standardsteuern, die dann zur Anwendung kommen, wenn keine anderen Quellen "
+"zur Verfügung stehen."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Aktivieren um die Vorlage zu überschreiben"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3258,21 +3264,21 @@
 "früheren Geschäftsjahre abgeschlossen werden."
 
 msgctxt "model:ir.message,text:msg_close_period_inactive_accounts"
 msgid ""
 "To close period \"%(period)s\", you must balance the inactive account "
 "\"%(account)s\"."
 msgstr ""
-"Damit der Buchungszeitraum \"$(period)s\" geschlossen werden kann, muss "
+"Damit der Buchungszeitraum \"%(period)s\" geschlossen werden kann, muss "
 "zuerst das inaktive Konto \"%(account)s\" ausgeglichen werden."
 
 msgctxt "model:ir.message,text:msg_close_period_non_posted_moves"
 msgid "To close period \"%(period)s\" you must post the moves \"%(moves)s\"."
 msgstr ""
-"Um den Buchungszeitraum \"$(period)s\" zu schließen, müssen zuerst die "
+"Um den Buchungszeitraum \"%(period)s\" zu schließen, müssen zuerst die "
 "Buchungssätze \"%(moves)s\" festgeschrieben werden."
 
 msgctxt "model:ir.message,text:msg_company_change_currency"
 msgid ""
 "You cannot change the currency of a company which is associated with account"
 " moves."
 msgstr ""
@@ -3569,22 +3575,21 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Die Daten für den Buchungszeitraum \"%(period)s\" müssen zwischen den Daten "
 "des zugehörigen Geschäftsjahres \"%(fiscalyear)s\" liegen."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_period_move_dates"
 msgid ""
 "The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
 "of move \"%(move)s\"."
 msgstr ""
-"Die Daten für den Buchungszeitraum \"%(period)s\" müssen zwischen den Daten "
-"des zugehörigen Geschäftsjahres \"%(fiscalyear)s\" liegen."
+"Die Daten für den Buchungszeitraum \"%(period)s\" müssen das Datum "
+"\"%(move_date)s\" des Buchungsatzes \"%(move)s\" enthalten."
 
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Die Buchungszeiträume \"%(first)s\" und \"%(second)s\" dürfen sich zeitlich "
@@ -3776,14 +3781,22 @@
 msgid "Lock"
 msgstr "Schließen"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Wieder öffnen"
 
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Schließen"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr "Wieder öffnen"
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Festschreiben"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Schließen"
@@ -3794,72 +3807,76 @@
 
 msgctxt "model:ir.model.button,string:period_reopen_button"
 msgid "Re-Open"
 msgstr "Wieder öffnen"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_type_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_aged_balance_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_fiscalyear_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_account_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_general_ledger_account_party_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
+
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_template_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_period_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reconcile_writeoff_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_tax_code_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_tax_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_tax_rule_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_account_journal"
 msgid "Default Account Journal"
 msgstr "Standard Journal"
 
 msgctxt "model:ir.sequence,name:sequence_account_move_reconciliation"
 msgid "Default Account Move Reconciliation"
@@ -4476,15 +4493,15 @@
 
 msgctxt "selection:account.fiscalyear,state:"
 msgid "Locked"
 msgstr "Geschlossen"
 
 msgctxt "selection:account.fiscalyear,state:"
 msgid "Open"
-msgstr "Geöffnet"
+msgstr "Offen"
 
 msgctxt "selection:account.fiscalyear.create_periods.start,frequency:"
 msgid "Monthly"
 msgstr "Monatlich"
 
 msgctxt "selection:account.fiscalyear.create_periods.start,frequency:"
 msgid "Other"
@@ -4528,15 +4545,15 @@
 
 msgctxt "selection:account.journal.period,state:"
 msgid "Closed"
 msgstr "Geschlossen"
 
 msgctxt "selection:account.journal.period,state:"
 msgid "Open"
-msgstr "Geöffnet"
+msgstr "Offen"
 
 msgctxt "selection:account.move,state:"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "selection:account.move,state:"
 msgid "Posted"
@@ -4592,15 +4609,15 @@
 
 msgctxt "selection:account.period,state:"
 msgid "Locked"
 msgstr "Geschlossen"
 
 msgctxt "selection:account.period,state:"
 msgid "Open"
-msgstr "Geöffnet"
+msgstr "Offen"
 
 msgctxt "selection:account.period,type:"
 msgid "Adjustment"
 msgstr "Berichtigung"
 
 msgctxt "selection:account.period,type:"
 msgid "Standard"
@@ -4810,22 +4827,14 @@
 msgid "Periods"
 msgstr "Buchungszeiträume"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Nummernkreise"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Abschließen"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Wieder öffnen"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "alle"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "Monate"
```

### Comparing `trytond_account-7.2.0/locale/es.po` & `trytond_account-7.2.1/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:account.account,active:"
 msgid "Active"
 msgstr "Activo"
 
 msgctxt "field:account.account,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Importe segunda moneda"
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.account,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account,childs:"
 msgid "Children"
@@ -104,15 +104,15 @@
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Derecha"
 
 msgctxt "field:account.account,second_currency:"
 msgid "Second Currency"
-msgstr "Segunda moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Fecha inicial"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -152,15 +152,15 @@
 
 msgctxt "field:account.account.deferral,account:"
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.account.deferral,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Importe segunda moneda"
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.account.deferral,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account.deferral,credit:"
 msgid "Credit"
@@ -180,27 +180,27 @@
 
 msgctxt "field:account.account.deferral,line_count:"
 msgid "Line Count"
 msgstr "Número de líneas"
 
 msgctxt "field:account.account.deferral,second_currency:"
 msgid "Second Currency"
-msgstr "Segunda moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.account.party,account:"
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.account.party,active:"
 msgid "Active"
 msgstr "Activo"
 
 msgctxt "field:account.account.party,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Importe segunda moneda"
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.account.party,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account.party,closed:"
 msgid "Closed"
@@ -937,15 +937,15 @@
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Cuenta del tercero"
 
 msgctxt "field:account.general_ledger.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Importe segunda moneda"
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
@@ -1001,15 +1001,15 @@
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliación"
 
 msgctxt "field:account.general_ledger.line,second_currency:"
 msgid "Second Currency"
-msgstr "Segunda moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
@@ -1143,14 +1143,18 @@
 msgid "End Date"
 msgstr "Fecha final"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Fecha inicial"
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Empresa"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Icono"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Diario"
@@ -1333,19 +1337,19 @@
 
 msgctxt "field:account.move.line,reconciliations_delegated:"
 msgid "Reconciliations Delegated"
 msgstr "Conciliaciones delegadas"
 
 msgctxt "field:account.move.line,second_currency:"
 msgid "Second Currency"
-msgstr "Segunda moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.move.line,second_currency_required:"
 msgid "Second Currency Required"
-msgstr "Segunda moneda obligatoria"
+msgstr "Moneda secundaria obligatoria"
 
 msgctxt "field:account.move.line,state:"
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.move.line,tax_lines:"
 msgid "Tax Lines"
@@ -2330,14 +2334,16 @@
 msgstr ""
 "Fuerza todos los asientos de esta cuenta a tener esta moneda secundaria."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default taxes for documents to be applied when there is no other source."
 msgstr ""
+"Impuestos por defecto que se aplicaran a los documentos cuando no hay otro "
+"origen."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Marcar para sobrescribir la definición de la plantilla"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -2439,23 +2445,23 @@
 
 msgctxt "help:account.move.cancel.default,reversal:"
 msgid "Reverse debit and credit."
 msgstr "Invertir debe y haber."
 
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
-msgstr "El importe expresado en la segunda moneda."
+msgstr "El importe expresado en la moneda secundaria."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Establecer una fecha para hacer el apunte pagable o cobrable."
 
 msgctxt "help:account.move.line,second_currency:"
 msgid "The second currency."
-msgstr "La segunda moneda."
+msgstr "La moneda secundaria."
 
 msgctxt "help:account.move.line.reschedule.start,interval:"
 msgid "The length of each period, in months."
 msgstr "La longitud en meses de cada periodo."
 
 msgctxt "help:account.move.line.template,amount:"
 msgid "A python expression that will be evaluated with the keywords."
@@ -3176,24 +3182,24 @@
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr "No se puede cerrar la cuenta \"%(account)s\" porque tiene apuntes."
 
 msgctxt "model:ir.message,text:msg_account_invalid_deferral_second_currency"
 msgid "To set a second currency for account \"%(account)s\", it must be deferral."
 msgstr ""
-"Para establecer una segunda divisa en la cuenta \"%(account)s\", esta debe "
-"ser de cierre."
+"Para establecer una moneda secundaria en la cuenta \"%(account)s\", esta "
+"debe ser de cierre."
 
 msgctxt "model:ir.message,text:msg_account_invalid_lines_second_currency"
 msgid ""
 "To set a second currency for account \"%(account)s\", its lines must have "
 "the same second currency \"%(currency)s\"."
 msgstr ""
-"Para establecer una segunda divisa en la cuenta \"%(account)s\", sus apuntes"
-" deben tener la misma segunda divisa \"%(currency)s\"."
+"Para establecer una moneda secundaria en la cuenta \"%(account)s\", sus "
+"apuntes deben tener la misma segunda divisa \"%(currency)s\"."
 
 msgctxt "model:ir.message,text:msg_account_invalid_type_second_currency"
 msgid ""
 "To set a second currency for account \"%(account)s\", it must not have a "
 "type \"payable\", \"revenue\", \"receivable\" nor \"expense\"."
 msgstr ""
 "Para establecer una moneda secundaria de la cuenta \"%(account)s\", no debe "
@@ -3331,15 +3337,15 @@
 
 msgctxt "model:ir.message,text:msg_group_line_same_company"
 msgid "You cannot group lines of different companies."
 msgstr "No se pueden agrupar líneas de diferentes compañías."
 
 msgctxt "model:ir.message,text:msg_group_line_same_second_currency"
 msgid "You cannot group lines of different second currencies."
-msgstr "No se pueden agrupar líneas con segundas monedas diferentes."
+msgstr "No se pueden agrupar líneas con monedas secundarias distintas."
 
 msgctxt "model:ir.message,text:msg_group_line_single"
 msgid "You cannot group a single line."
 msgstr "No se puede agrupar una sola línea."
 
 msgctxt "model:ir.message,text:msg_journal_account_moves"
 msgid ""
@@ -3386,15 +3392,16 @@
 "tercero en el apunte \"%(line)s\"."
 
 msgctxt "model:ir.message,text:msg_line_second_currency_sign"
 msgid ""
 "You must set the sign for second currency to match the sign of debit - "
 "credit."
 msgstr ""
-"El signo de la segunda moneda debe coincidir con el signo del debe - haber."
+"El signo de la moneda secundaria debe coincidir con el signo del debe - "
+"haber."
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "No puede modificar o eliminar el diario periodo \"%(journal_period)s\" "
@@ -3532,22 +3539,21 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Las fechas del periodo \"%(period)s\" deben estar dentro de las fechas de su"
 " ejercicio fiscal \"%(fiscalyear)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_period_move_dates"
 msgid ""
 "The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
 "of move \"%(move)s\"."
 msgstr ""
-"Las fechas del periodo \"%(period)s\" deben estar dentro de las fechas de su"
-" ejercicio fiscal \"%(fiscalyear)s\"."
+"Las fechas del periodo \"%(period)s\" deben incluir la fechas "
+"\"%(move_date)s\" del asiento \"%(move)s\"."
 
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Los periodos \"%(first)s\" y \"%(second)s\" se superponen, debe usar fechas "
@@ -3727,14 +3733,22 @@
 msgid "Lock"
 msgstr "Bloquear"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Volver a abrir"
 
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Cerrar"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr "Volver a abrir"
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Contabilizar"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Cerrar"
@@ -3772,14 +3786,18 @@
 msgid "User in companies"
 msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Usuario en las empresas"
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Usuario en las empresas"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "Usuario en las empresas"
@@ -4761,22 +4779,14 @@
 msgid "Periods"
 msgstr "Periodos"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Secuencias"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Cerrar"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Volver a abrir"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "cada"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "meses"
```

### Comparing `trytond_account-7.2.0/locale/es_419.po` & `trytond_account-7.2.1/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -1229,14 +1229,18 @@
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr ""
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr ""
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr ""
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Libro diario"
@@ -3887,14 +3891,23 @@
 msgid "Lock"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
@@ -3933,14 +3946,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -4989,23 +5006,14 @@
 msgstr "Periods"
 
 #, fuzzy
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Secuencia"
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Close"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr ""
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr ""
```

### Comparing `trytond_account-7.2.0/locale/et.po` & `trytond_account-7.2.1/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -1224,14 +1224,19 @@
 msgid "End Date"
 msgstr "Lõppkuupäev"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Alguskuupäev"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Ettevõte"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Ikoon"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Andmik"
@@ -3881,14 +3886,23 @@
 msgid "Lock"
 msgstr "Lukusta"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Ava uuesti"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Sulge"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Postita"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Sulge"
@@ -3934,14 +3948,19 @@
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Kasutaja ettevõttes"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Kasutaja ettevõttes"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Kasutaja ettevõttes"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
@@ -4978,22 +4997,14 @@
 msgid "Periods"
 msgstr "Perioodid"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Järjestused"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Sulge"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Taas-ava"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/fa.po` & `trytond_account-7.2.1/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -1236,14 +1236,19 @@
 msgid "End Date"
 msgstr "تاریخ پایان"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "تاریخ شروع"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "شرکت"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "آیکون"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "روزنامه"
@@ -3928,14 +3933,23 @@
 msgid "Lock"
 msgstr "قفل"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "بازگشایی"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "بسته"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "صدور"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "بسته"
@@ -3973,14 +3987,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5012,22 +5030,14 @@
 msgid "Periods"
 msgstr "دوره ها"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "ترتیب ها"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "بسته"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "دوباره باز کردن"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/fi.po` & `trytond_account-7.2.1/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -1341,14 +1341,19 @@
 msgstr "eräpäivä"
 
 #, fuzzy
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Aloitus päivä"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Yritys"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
@@ -4026,14 +4031,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -4071,14 +4085,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5140,24 +5158,14 @@
 msgid "Periods"
 msgstr "Periods"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr ""
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Close"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr ""
```

### Comparing `trytond_account-7.2.0/locale/fr.po` & `trytond_account-7.2.1/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1143,14 +1143,18 @@
 msgid "End Date"
 msgstr "Date de fin"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Date de début"
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Société"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Icône"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Journal"
@@ -3751,14 +3755,22 @@
 msgid "Lock"
 msgstr "Verrouiller"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Rouvrir"
 
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Clôturer"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr "Rouvrir"
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Fermer"
@@ -3796,14 +3808,18 @@
 msgid "User in companies"
 msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Utilisateur dans les sociétés"
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Utilisateur dans les sociétés"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "Utilisateur dans les sociétés"
@@ -4785,22 +4801,14 @@
 msgid "Periods"
 msgstr "Périodes"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Séquences"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Clôturer"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Rouvrir"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "tous les"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "mois"
```

### Comparing `trytond_account-7.2.0/locale/hu.po` & `trytond_account-7.2.1/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -1176,14 +1176,19 @@
 msgid "End Date"
 msgstr "Befejező dátum"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Kezdődátum"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Cég"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Ikon"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Napló"
@@ -3782,14 +3787,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Visszanyitás"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Lezárás"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Rögzítés"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Lezárás"
@@ -3835,14 +3849,19 @@
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Felhasználó a cég alkalmazotta"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Felhasználó a cég alkalmazotta"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Felhasználó a cég alkalmazotta"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
@@ -4869,22 +4888,14 @@
 msgid "Periods"
 msgstr "Periódusok"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Sorszámozások"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Lezárás"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Visszanyitás"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/id.po` & `trytond_account-7.2.1/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -1164,14 +1164,19 @@
 msgid "End Date"
 msgstr "Tanggal Akhir"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Tanggal Awal"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Perusahaan"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr ""
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Jurnal"
@@ -3709,14 +3714,23 @@
 msgid "Lock"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Tutup"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Tutup"
@@ -3762,14 +3776,19 @@
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Pengguna di dalam perusahaan"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Pengguna di dalam perusahaan"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Pengguna di dalam perusahaan"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
@@ -4779,22 +4798,14 @@
 msgid "Periods"
 msgstr "Periode"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Urutan-Urutan"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Tutup"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr ""
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr ""
```

### Comparing `trytond_account-7.2.0/locale/it.po` & `trytond_account-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -1243,14 +1243,19 @@
 msgid "End Date"
 msgstr "Data fine"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Data inizio"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Azienda"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Icona"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Registro"
@@ -3921,14 +3926,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Chiudi"
@@ -3974,14 +3988,19 @@
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Utente in azienda"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Utente in azienda"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Utente in azienda"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
@@ -5077,23 +5096,14 @@
 msgstr "Periodi"
 
 #, fuzzy
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Sequenze"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Chiudi"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/lo.po` & `trytond_account-7.2.1/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -1261,14 +1261,19 @@
 msgid "End Date"
 msgstr "ວັນທີສິ້ນສຸດ"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "ວັນທີເລີ່ມ"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "ສຳນັກງານ/ຫ້ອງການ"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "ປຸ່ມລັດ"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "ບັນຊີປະຈໍາວັນ"
@@ -3961,14 +3966,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -4006,14 +4020,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5114,24 +5132,14 @@
 msgid "Periods"
 msgstr "ໄລຍະ"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "ລຳດັບ"
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "ອັດ"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/lt.po` & `trytond_account-7.2.1/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1214,14 +1214,19 @@
 msgid "End Date"
 msgstr "Pabaigos data"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Pradžios data"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Organizacija"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Ikona"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Žurnalas"
@@ -3891,14 +3896,23 @@
 msgid "Lock"
 msgstr "Užrakinti"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Iš naujo atverti"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Užverti"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Įtraukti į apskaitą"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Užverti"
@@ -3944,14 +3958,19 @@
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Organizacijos naudotojas"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Organizacijos naudotojas"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Organizacijos naudotojas"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
@@ -5010,24 +5029,14 @@
 msgid "Periods"
 msgstr "Periods"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Numeruotės"
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Close"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/nl.po` & `trytond_account-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1143,14 +1143,18 @@
 msgid "End Date"
 msgstr "Eind datum"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Start datum"
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Bedrijf"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Pictogram"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Dagboek"
@@ -2329,14 +2333,16 @@
 "Forceer alle boekingen voor deze grootboekrekening om deze secundaire valuta"
 " te gebruiken."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default taxes for documents to be applied when there is no other source."
 msgstr ""
+"Standaard belastingen die moeten worden toegepast op documenten als er geen "
+"andere bron is."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Vink aan om de template te overschrijven"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3165,15 +3171,15 @@
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Grootboekschema actualiseren"
 
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
-msgstr "Er bestaat al een rekeningschema voor bedrijf \"% (company)s\"."
+msgstr "Er bestaat al een rekeningschema voor bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
 "U kunt de grootboekrekening \"%(account)s\" niet sluiten omdat er boekingen "
 "op gedaan zijn."
 
@@ -3403,28 +3409,28 @@
 "debet - credit."
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
-"U kunt de journaalperiode \"% (journal_period) s\" niet wijzigen of "
+"U kunt periode \"%(journal_period)s\" van het dagboek niet wijzigen of "
 "verwijderen omdat deze boekingen bevat."
 
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "U kunt geen regels toevoegen / wijzigen / verwijderen in de gesloten dagboek"
 " periode \"%(journal_period)s\"."
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
 msgid "You cannot modify line \"%(line)s\" from posted move \"%(move)s\"."
-msgstr "U kunt regel \"%(line)s\" van geboekte boeking \"%(line)s\" niet wijzigen."
+msgstr "U kunt regel \"%(line)s\" van geboekte boeking \"%(move)s\" niet wijzigen."
 
 msgctxt "model:ir.message,text:msg_modify_line_reconciled"
 msgid "You cannot modify reconciled line \"%(line)s\"."
 msgstr "U kunt de afgeletterde regel \"%(line)s\" niet aanpassen."
 
 msgctxt "model:ir.message,text:msg_modify_posted_moved"
 msgid "You cannot modify posted move \"%(move)s\"."
@@ -3738,14 +3744,22 @@
 msgid "Lock"
 msgstr "Vergrendel"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Heropen"
 
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Sluiten"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr "Heropenen"
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Boeken"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Sluiten"
@@ -3783,14 +3797,18 @@
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Gebruiker in bedrijven"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
@@ -4772,22 +4790,14 @@
 msgid "Periods"
 msgstr "Periodes"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Reeksen"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Sluiten"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Heropen"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "elke"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "maanden"
```

### Comparing `trytond_account-7.2.0/locale/pl.po` & `trytond_account-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1244,14 +1244,19 @@
 msgid "End Date"
 msgstr "Data ukończenia"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Data rozpoczęcia"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Firma"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Ikona"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Rejestr"
@@ -3940,14 +3945,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Zamknij"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Zamknij"
@@ -3985,14 +3999,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -4209,15 +4227,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_renew_fiscalyear"
 msgid "Renew Fiscal Year"
 msgstr "Otworzenie na nowo roku podatkowego"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Raportowanie"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tax_code_list"
 msgid "Codes"
 msgstr "Kod"
 
 #, fuzzy
@@ -5069,22 +5087,14 @@
 msgid "Periods"
 msgstr "Okresy"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Sekwencje"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Zamknij"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Otwórz ponownie"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/pt.po` & `trytond_account-7.2.1/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1234,14 +1234,19 @@
 msgid "End Date"
 msgstr "Data de fim"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Data inicial"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Empresa"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Ícone"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Diário"
@@ -3933,14 +3938,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -3978,14 +3992,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5081,22 +5099,14 @@
 msgid "Periods"
 msgstr "Períodos"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Sequências"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Fechar"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Abrir Novamente"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/ro.po` & `trytond_account-7.2.1/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -1169,14 +1169,19 @@
 msgid "End Date"
 msgstr "Data de încheiere"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Data de început"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Companie"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Pictogramă"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Jurnal"
@@ -3778,14 +3783,23 @@
 msgid "Lock"
 msgstr "Blocare"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Deschide"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Închidere"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Postare"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Închidere"
@@ -3823,14 +3837,19 @@
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Utilizator în companii"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
@@ -4818,22 +4837,14 @@
 msgid "Periods"
 msgstr "Perioade"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Secvenţe"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Închidere"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Deschide"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "fiecare"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "luni"
```

### Comparing `trytond_account-7.2.0/locale/ru.po` & `trytond_account-7.2.1/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -1326,14 +1326,19 @@
 msgstr "Дата окончания"
 
 #, fuzzy
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Дата начала"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Организация"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Иконка"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Журнал"
@@ -4063,14 +4068,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -4108,14 +4122,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5223,24 +5241,14 @@
 msgid "Periods"
 msgstr "Периоды"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Нумерации"
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Закрыть"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/sl.po` & `trytond_account-7.2.1/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1249,14 +1249,19 @@
 msgid "End Date"
 msgstr "Končni datum"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Začetni datum"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Družba"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Ikona"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Dnevnik"
@@ -3933,14 +3938,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Zapri"
@@ -3978,14 +3992,19 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Uporabnik v družbah"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -5078,22 +5097,14 @@
 msgid "Periods"
 msgstr "Obdobja"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Šifranti"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Zaprto"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Znova odpri"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
```

### Comparing `trytond_account-7.2.0/locale/tr.po` & `trytond_account-7.2.1/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1221,14 +1221,18 @@
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr ""
 
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr ""
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
@@ -3824,14 +3828,23 @@
 msgid "Lock"
 msgstr "Lock"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Re-Open"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Close"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Post"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Close"
@@ -3869,14 +3882,18 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr ""
@@ -4909,24 +4926,14 @@
 msgid "Periods"
 msgstr "Periods"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr ""
 
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Close"
-
-#, fuzzy
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Re-Open"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr ""
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr ""
```

### Comparing `trytond_account-7.2.0/locale/uk.po` & `trytond_account-7.2.1/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -1160,14 +1160,19 @@
 msgid "End Date"
 msgstr "Кінцева дата"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "Початкова дата"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "Компанія"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "Піктограма"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "Журнал"
@@ -3788,14 +3793,23 @@
 msgid "Lock"
 msgstr "Заблокувати"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Перевідкрити"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "Закрити"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Провести"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Закрити"
@@ -3833,14 +3847,19 @@
 msgid "User in companies"
 msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "Користувач у компаніях"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "Користувач у компаніях"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "Користувач у компаніях"
@@ -4838,22 +4857,14 @@
 msgid "Periods"
 msgstr "Періоди"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "Послідовності"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "Закрити"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "Перевідкрити"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "кожні"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "місяці"
```

### Comparing `trytond_account-7.2.0/locale/zh_CN.po` & `trytond_account-7.2.1/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -1143,14 +1143,19 @@
 msgid "End Date"
 msgstr "结账日期"
 
 msgctxt "field:account.journal.open_cash.context,start_date:"
 msgid "Start Date"
 msgstr "开始日期"
 
+#, fuzzy
+msgctxt "field:account.journal.period,company:"
+msgid "Company"
+msgstr "公司"
+
 msgctxt "field:account.journal.period,icon:"
 msgid "Icon"
 msgstr "图标"
 
 msgctxt "field:account.journal.period,journal:"
 msgid "Journal"
 msgstr "日记账"
@@ -3612,14 +3617,23 @@
 msgid "Lock"
 msgstr "锁定"
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "重新打开"
 
+#, fuzzy
+msgctxt "model:ir.model.button,string:journal_period_close_button"
+msgid "Close"
+msgstr "结账"
+
+msgctxt "model:ir.model.button,string:journal_period_reopen_button"
+msgid "Reopen"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "登记入账"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "结账"
@@ -3657,14 +3671,19 @@
 msgid "User in companies"
 msgstr "公司用户"
 
 msgctxt "model:ir.rule.group,name:rule_group_general_ledger_line_companies"
 msgid "User in companies"
 msgstr "公司用户"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_journal_period_companies"
+msgid "User in companies"
+msgstr "公司用户"
+
 msgctxt "model:ir.rule.group,name:rule_group_move_companies"
 msgid "User in companies"
 msgstr "公司中的用户"
 
 msgctxt "model:ir.rule.group,name:rule_group_move_reconciliation_companies"
 msgid "User in companies"
 msgstr "公司用户"
@@ -4644,22 +4663,14 @@
 msgid "Periods"
 msgstr "分期"
 
 msgctxt "view:account.fiscalyear:"
 msgid "Sequences"
 msgstr "序列"
 
-msgctxt "view:account.journal.period:"
-msgid "Close"
-msgstr "结账"
-
-msgctxt "view:account.journal.period:"
-msgid "Re-Open"
-msgstr "重新打开"
-
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "每"
 
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "月"
```

### Comparing `trytond_account-7.2.0/localize.xsl` & `trytond_account-7.2.1/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/message.xml` & `trytond_account-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart.xml` & `trytond_account-7.2.1/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_bg.xml` & `trytond_account-7.2.1/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_ca.xml` & `trytond_account-7.2.1/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_de.xml` & `trytond_account-7.2.1/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_en.xml` & `trytond_account-7.2.1/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_es.xml` & `trytond_account-7.2.1/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_fr.xml` & `trytond_account-7.2.1/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_nl.xml` & `trytond_account-7.2.1/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_pt.xml` & `trytond_account-7.2.1/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_ru.xml` & `trytond_account-7.2.1/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/minimal_chart_sl.xml` & `trytond_account-7.2.1/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/move.py` & `trytond_account-7.2.1/move.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/move.xml` & `trytond_account-7.2.1/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/move_template.py` & `trytond_account-7.2.1/move_template.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/move_template.xml` & `trytond_account-7.2.1/move_template.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/party.py` & `trytond_account-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/party.xml` & `trytond_account-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/period.py` & `trytond_account-7.2.1/period.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/period.xml` & `trytond_account-7.2.1/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/setup.py` & `trytond_account-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tax.py` & `trytond_account-7.2.1/tax.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tax.xml` & `trytond_account-7.2.1/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_account_active.rst` & `trytond_account-7.2.1/tests/scenario_account_active.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_account_reconcile.rst` & `trytond_account-7.2.1/tests/scenario_account_reconcile.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_account_reconcile_automatic.rst` & `trytond_account-7.2.1/tests/scenario_account_reconcile_automatic.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_account_reconciliation.rst` & `trytond_account-7.2.1/tests/scenario_account_reconciliation.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency.rst` & `trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst` & `trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency_write_off.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_close_fiscalyear.rst` & `trytond_account-7.2.1/tests/scenario_close_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_move_cancel.rst` & `trytond_account-7.2.1/tests/scenario_move_cancel.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_move_line_delegate.rst` & `trytond_account-7.2.1/tests/scenario_move_line_delegate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_move_line_group.rst` & `trytond_account-7.2.1/tests/scenario_move_line_group.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_move_line_reschedule.rst` & `trytond_account-7.2.1/tests/scenario_move_line_reschedule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_move_template.rst` & `trytond_account-7.2.1/tests/scenario_move_template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_renew_fiscalyear.rst` & `trytond_account-7.2.1/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_reports.rst` & `trytond_account-7.2.1/tests/scenario_reports.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/scenario_tax_code.rst` & `trytond_account-7.2.1/tests/scenario_tax_code.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/test_module.py` & `trytond_account-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tests/tools.py` & `trytond_account-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tox.ini` & `trytond_account-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/trial_balance.fodt` & `trytond_account-7.2.1/trial_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/tryton.cfg` & `trytond_account-7.2.1/tryton.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tryton]
-version=7.2.0
+version=7.2.1
 depends:
     company
     currency
     ir
     party
     res
 xml:
```

### Comparing `trytond_account-7.2.0/trytond_account.egg-info/PKG-INFO` & `trytond_account-7.2.1/trytond_account.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account-7.2.0/trytond_account.egg-info/SOURCES.txt` & `trytond_account-7.2.1/trytond_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/type_statement.fodt` & `trytond_account-7.2.1/type_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/account_deferral_form.xml` & `trytond_account-7.2.1/view/account_deferral_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/account_form.xml` & `trytond_account-7.2.1/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/account_template_form.xml` & `trytond_account-7.2.1/view/account_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/account_type_form.xml` & `trytond_account-7.2.1/view/account_type_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/account_type_template_form.xml` & `trytond_account-7.2.1/view/account_type_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/aged_balance_context_form.xml` & `trytond_account-7.2.1/view/aged_balance_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/company_form.xml` & `trytond_account-7.2.1/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/configuration_form.xml` & `trytond_account-7.2.1/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/fiscalyear_balance_non_deferral_start_form.xml` & `trytond_account-7.2.1/view/fiscalyear_balance_non_deferral_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/fiscalyear_create_periods_start_form.xml` & `trytond_account-7.2.1/view/fiscalyear_create_periods_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/fiscalyear_form.xml` & `trytond_account-7.2.1/view/fiscalyear_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/general_ledger_account_context_form.xml` & `trytond_account-7.2.1/view/general_ledger_account_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/general_ledger_line_list.xml` & `trytond_account-7.2.1/view/general_ledger_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/income_statement_context_form.xml` & `trytond_account-7.2.1/view/income_statement_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/journal_form.xml` & `trytond_account-7.2.1/view/journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/journal_period_form.xml` & `trytond_account-7.2.1/view/journal_period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_form.xml` & `trytond_account-7.2.1/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_form.xml` & `trytond_account-7.2.1/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_form_move.xml` & `trytond_account-7.2.1/view/move_line_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_list_payable_receivable.xml` & `trytond_account-7.2.1/view/move_line_list_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_reschedule_start_form.xml` & `trytond_account-7.2.1/view/move_line_reschedule_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_template_form.xml` & `trytond_account-7.2.1/view/move_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_tree.xml` & `trytond_account-7.2.1/view/move_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_line_tree_move.xml` & `trytond_account-7.2.1/view/move_line_tree_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_template_form.xml` & `trytond_account-7.2.1/view/move_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_template_keyword_form.xml` & `trytond_account-7.2.1/view/move_template_keyword_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/move_tree.xml` & `trytond_account-7.2.1/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/party_form.xml` & `trytond_account-7.2.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/period_form.xml` & `trytond_account-7.2.1/view/period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/reconcile_show_form.xml` & `trytond_account-7.2.1/view/reconcile_show_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/renew_fiscalyear_start_form.xml` & `trytond_account-7.2.1/view/renew_fiscalyear_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_code_context_form.xml` & `trytond_account-7.2.1/view/tax_code_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_code_form.xml` & `trytond_account-7.2.1/view/tax_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_code_template_form.xml` & `trytond_account-7.2.1/view/tax_code_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_form.xml` & `trytond_account-7.2.1/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_rule_form.xml` & `trytond_account-7.2.1/view/tax_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_rule_line_form.xml` & `trytond_account-7.2.1/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_rule_line_template_form.xml` & `trytond_account-7.2.1/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_template_form.xml` & `trytond_account-7.2.1/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/tax_test_form.xml` & `trytond_account-7.2.1/view/tax_test_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.0/view/writeoff_form.xml` & `trytond_account-7.2.1/view/writeoff_form.xml`

 * *Files identical despite different names*

