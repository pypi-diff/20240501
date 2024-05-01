# Comparing `tmp/nmbrs-0.2.0.tar.gz` & `tmp/nmbrs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-0.2.0.tar", last modified: Sun Apr 28 18:06:29 2024, max compression
+gzip compressed data, was "nmbrs-1.0.2.tar", last modified: Wed May  1 11:33:45 2024, max compression
```

## Comparing `nmbrs-0.2.0.tar` & `nmbrs-1.0.2.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.209584 nmbrs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-28 18:06:16.000000 nmbrs-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 18:06:16.000000 nmbrs-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-28 18:06:29.209584 nmbrs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-28 18:06:16.000000 nmbrs-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-28 18:06:16.000000 nmbrs-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:06:29.209584 nmbrs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-28 18:06:16.000000 nmbrs-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.193584 nmbrs-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.193584 nmbrs-0.2.0/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-28 18:06:27.000000 nmbrs-0.2.0/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/auth/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14957 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.201584 nmbrs-0.2.0/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.201584 nmbrs-0.2.0/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.201584 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.205584 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.209584 nmbrs-0.2.0/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.209584 nmbrs-0.2.0/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.331218 nmbrs-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-01 11:33:32.000000 nmbrs-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 11:33:32.000000 nmbrs-1.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-01 11:33:45.331218 nmbrs-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-05-01 11:33:32.000000 nmbrs-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 11:33:32.000000 nmbrs-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:33:45.331218 nmbrs-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-01 11:33:32.000000 nmbrs-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.311218 nmbrs-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.315218 nmbrs-1.0.2/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/__logging__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-01 11:33:43.000000 nmbrs-1.0.2/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.315218 nmbrs-1.0.2/src/nmbrs/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/auth/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.315218 nmbrs-1.0.2/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.319218 nmbrs-1.0.2/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.319218 nmbrs-1.0.2/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.319218 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/background_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13509 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.319218 nmbrs-1.0.2/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.319218 nmbrs-1.0.2/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.323218 nmbrs-1.0.2/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.323218 nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.331218 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/report_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.331218 nmbrs-1.0.2/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/utils/get_module_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 11:33:32.000000 nmbrs-1.0.2/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:33:45.331218 nmbrs-1.0.2/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-01 11:33:45.000000 nmbrs-1.0.2/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-01 11:33:45.000000 nmbrs-1.0.2/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:33:45.000000 nmbrs-1.0.2/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 11:33:45.000000 nmbrs-1.0.2/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 11:33:45.000000 nmbrs-1.0.2/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-0.2.0/LICENSE` & `nmbrs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/setup.py` & `nmbrs-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/__version__.py` & `nmbrs-1.0.2/src/nmbrs/__version__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Versioning details."""
 
 __title__ = "nmbrs"
-__version__ = '0.2.0'
+__version__ = '1.0.2'
 __author__ = "Lars Kluijtmans"
 __author_email__ = "info@lk-software.com"
 __maintainer__ = "Lars Kluijtmans"
 __maintainer_email__ = "info@lk-software.com"
 __description__ = "Python SDK for the Visma Nmbrs SOAP API."
 __license__ = "Lars Kluijtmans"
```

### Comparing `nmbrs-0.2.0/src/nmbrs/api.py` & `nmbrs-1.0.2/src/nmbrs/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 """Main class provided by the package."""
 
+import logging
 from .auth.token_manager import AuthManager
 from .exceptions import ParameterMissingError
 from .service.company_service import CompanyService
 from .service.debtor_service import DebtorService
 from .service.employee_service import EmployeeService
-from .service.sso_service import SingleSingOnService
+from .service.report_service import ReportService
 from .utils.find_empty_params import find_empty_params
 
+logger = logging.getLogger(__name__)
+
 
 class Nmbrs:
     """
     A class representing the Nmbrs SOAP API.
 
     This class provides an interface to interact with various Nmbrs SOAP API services.
 
     [Nmbrs SOAP API](https://api.nmbrs.nl/soap/v3/)
     """
 
     def __init__(
         self,
-        username: str = None,
-        token: str = None,
+        username: str,
+        token: str,
+        auth_type: str = "token",
         domain: str = None,
         sandbox: bool = True,
-        auth_type: str = None,
     ):
         """
         Initializes a Nmbrs SOAP API instance with authentication details and settings.
 
         Args:
-            username (str, optional): Username for Nmbrs.
-            token (str, optional): Token for the Nmbrs SOAP API.
-            domain (str, optional): Nmbrs environment subdomain.
+            username (str): Username for Nmbrs.
+            token (str): Token for the Nmbrs SOAP API.
+            auth_type (str): The type of authentication to be used. Options: "token", "domain". Default "token"
+            domain (str, optional): Nmbrs environment subdomain (used when the auth_type paramater is set to "domain").
             sandbox (bool, optional): A boolean indicating whether to use the sandbox environment. Default is True.
-            auth_type (str, optional): The type of authentication to be used. Options: "token", "domain", None (default).
         """
+        if not sandbox:
+            logger.warning("Live environment is activated")  # pragma: no cover
+
         self.sandbox = sandbox
         self.auth_manager = AuthManager()
-        self.sso = SingleSingOnService(self.auth_manager, self.sandbox)
         self.debtor = DebtorService(self.auth_manager, self.sandbox)
         self.company = CompanyService(self.auth_manager, self.sandbox)
         self.employee = EmployeeService(self.auth_manager, self.sandbox)
+        self.report = ReportService(self.auth_manager, self.sandbox)
 
         if auth_type == "token":
             self.auth_with_token(username, token)
         elif auth_type == "domain":
             self.auth_with_domain(username, token, domain)
 
-    def auth_with_token(self, username: str, token: str) -> None:
+    def auth_with_token(self, username: str, token: str):
         """
         Perform standard authentication using token and initialize related services.
 
         Args:
             username (str): Username for Nmbrs.
             token (str): Token for the Nmbrs SOAP API.
         """
         params = find_empty_params(**{"username": username, "token": token})
         if params:
+            logger.error("Parameter missing: %s", params)
             raise ParameterMissingError(params=params)
         domain = self.debtor.get_domain(username, token)
         self.auth_manager.set_auth_header(username, token, domain.sub_domain)
+        logger.info("Authentication with token successful")
 
-    def auth_with_domain(self, username: str, token: str, domain: str) -> None:
+    def auth_with_domain(self, username: str, token: str, domain: str):
         """
         Create the auth header with domain object and initialize related services.
         Note: The username, token, and domain are not validated in this routine.
 
         Args:
             username (str): Username for Nmbrs.
             token (str): Token for the Nmbrs SOAP API.
             domain (str): Nmbrs environment subdomain.
         """
         params = find_empty_params(**{"username": username, "token": token, "domain": domain})
         if params:
+            logger.error("Parameter missing: %s", params)
             raise ParameterMissingError(params=params)
         self.auth_manager.set_auth_header(username, token, domain)
+        logger.info("Authentication with domain successful")
```

### Comparing `nmbrs-0.2.0/src/nmbrs/auth/token_manager.py` & `nmbrs-1.0.2/src/nmbrs/auth/token_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """
 A class for managing the Nmbrs authentication header.
 """
 
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 class AuthManager:
     """
     A class for managing the Nmbrs authentication header.
     """
 
     def __init__(self):
@@ -23,40 +27,44 @@
         self.header = {
             "AuthHeaderWithDomain": {
                 "Username": username,
                 "Token": token,
                 "Domain": domain,
             }
         }
+        logger.info("Authentication header set successfully.")
 
     def get_username(self) -> str:
         """
         Gets the username from the authentication header.
 
         Returns:
             str: The username or None if the authentication header is not set.
         """
         if self.header:
             return self.header["AuthHeaderWithDomain"]["Username"]
+        logger.warning("Authentication header is not set.")
         return ""
 
     def get_token(self) -> str:
         """
         Gets the authentication token from the authentication header.
 
         Returns:
             str: The authentication token or None if the authentication header is not set.
         """
         if self.header:
             return self.header["AuthHeaderWithDomain"]["Token"]
+        logger.warning("Authentication header is not set.")
         return ""
 
     def get_domain(self) -> str:
         """
         Gets the domain from the authentication header.
 
         Returns:
             str: The domain or None if the authentication header is not set.
         """
         if self.header:
             return self.header["AuthHeaderWithDomain"]["Domain"]
+        logger.warning("Authentication header is not set.")
         return ""
```

### Comparing `nmbrs-0.2.0/src/nmbrs/data_classes/company.py` & `nmbrs-1.0.2/src/nmbrs/data_classes/company.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/data_classes/data_class.py` & `nmbrs-1.0.2/src/nmbrs/data_classes/data_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 """A base class for data classes that automatically initializes instance variables from a dictionary."""
 
 import json
 from abc import ABC, abstractmethod
 from decimal import Decimal
 
 
-def serialize(obj: any, target_cls=dict) -> float | dict | list[dict]:
-    """Serialize DataClass objects to native python data structures"""
-    if isinstance(obj, list):
-        return [serialize(sub, target_cls) for sub in obj]
-
-    if isinstance(obj, Decimal):
-        return float(obj)
-
-    if isinstance(obj, (dict, DataClass)):
-        obj = obj.__dict__
-        result = target_cls()
-        for key in obj:
-            result[key] = serialize(obj[key], target_cls)
-        return result
-    return obj
-
-
 class DataClass(ABC):
     """A base class for data classes that automatically initializes instance variables from a dictionary."""
 
     @abstractmethod
     def __init__(self) -> None:
         """Initializes instance variables based on the provided dictionary."""
 
     def to_dict(self) -> dict:
         """Convert the instance to a dictionary."""
-        return serialize(self)
+        return self._serialize_str(self)
+
+    def _serialize_str(self, obj, decimal=False):
+        """
+        Serialize DataClass objects be suitable to format to string
+
+        Args:
+            obj (any): The object to be converted into a dict.
+            decimal (bool, optional): When true all the decimals will be changed to floats.
+        """
+        if isinstance(obj, list):
+            return [self._serialize_str(sub) for sub in obj]
+
+        if decimal:
+            if isinstance(obj, Decimal):
+                return float(obj)  # pragma: no cover
+
+        if isinstance(obj, (dict, DataClass)):
+            obj = obj.__dict__
+            result = {}
+            for key in obj:
+                result[key] = self._serialize_str(obj[key])
+            return result
+        return obj
 
     def __str__(self):
         """Returns a JSON representation of the instance."""
-        obj = self.to_dict()
+        obj = self._serialize_str(self, True)
         return json.dumps(obj)
 
     def __getattr__(self, name):
         """Implement custom __getattr__ to access instance variables directly."""
         try:
             return self.__dict__[name]
         except KeyError as e:
```

### Comparing `nmbrs-0.2.0/src/nmbrs/data_classes/debtor.py` & `nmbrs-1.0.2/src/nmbrs/data_classes/debtor.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/data_classes/employee.py` & `nmbrs-1.0.2/src/nmbrs/data_classes/employee.py`

 * *Files 6% similar despite different names*

```diff
@@ -404,7 +404,26 @@
         self.sector_code = sector.get("SectorCode")
         self.sector_description = sector.get("SectorDescription")
 
         wage_cost_benefit = data.get("WageCostBenefit")
         self.wage_cost_benefit_code = wage_cost_benefit.get("WageCostBenefitCode")
         self.wage_cost_benefit_end_period = wage_cost_benefit.get("EndPeriod")
         self.wage_cost_benefit_end_year = wage_cost_benefit.get("EndYear")
+
+
+class VariableDaysWorked:
+    """A class used to insert days worked to a employee."""
+
+    def __init__(self, employee_id: int, data: dict):
+        self.employee_id = employee_id
+        self.days: int = data.get("Days")
+        self.plus_min_days_for_wage_comp: int = data.get("PlusMinusDaysForWageComp")
+
+
+class DaysWorked:
+    """A class used to insert days worked to a employee."""
+
+    def __init__(self, employee_id: int, days: int, period: int, year: int):
+        self.employee_id = employee_id
+        self.days = days
+        self.period = period
+        self.year = year
```

### Comparing `nmbrs-0.2.0/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-1.0.2/src/nmbrs/data_classes/utils/xml.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,31 +6,35 @@
         If parsing fails, return the original XML string.
     get_xml(xml: str) -> dict | None: Retrieve XML data as a dictionary.
 
 Dependencies:
     xmltodict: A library for parsing XML into Python dictionaries.
 """
 
+import logging
 import xmltodict
 
+logger = logging.getLogger(__name__)
+
 
 def parse_xml_to_dict(xml: str) -> dict | str:
     """
     Try to parse the XML string into a dictionary.
     If parsing fails, return the original XML string.
 
     Args:
         xml (str): A string that contains an XML document.
 
     Returns:
         dict | str: A dictionary representation of the XML or the original XML string.
     """
     try:
         return xmltodict.parse(xml)
-    except Exception:
+    except Exception as e:
+        logger.error("Error parsing XML: %s", e)
         return xml
 
 
 def get_xml(xml: str) -> dict | None:
     """
     Method to retrieve XML data as a dictionary.
 
@@ -38,9 +42,10 @@
         xml (str): A string that contains an XML document.
 
     Returns:
         dict | None: A dictionary representation of the XML data, or None if parsing fails.
     """
     xml = parse_xml_to_dict(xml)
     if not isinstance(xml, dict):
+        logger.warning("Failed to parse XML into dictionary.")
         return None
     return xml
```

### Comparing `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py` & `nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py` & `nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py` & `nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py` & `nmbrs-1.0.2/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -213,15 +213,26 @@
             case 2046:
                 self.title = "Not Found"
                 self.cause = "Could not find the requested resource"
                 self.solution = "Input a valid resource, use a GET call to retrieve the data."
             case 9999:
                 self.unknown_error()
                 self.title = "Unkown"  # Actual title returned by nmbrs
+            case 10001:
+                # Special errors for background tasks
+                self.title = "Error Retrieving Background Report"
+                self.cause = "The 'Error' was returned when retrieving the background report from the Nmbrs API."
+                self.solution = "Please check your network connection and try again. If the issue persists, contact nmbrs support"
+            case 10002:
+                # Special errors for background tasks
+                self.title = "Unknown Error Retrieving Background Report"
+                self.cause = "The 'Unknown' was returned when retrieving the background report from the Nmbrs API."
+                self.solution = "¯_(ツ)_/¯"
             case _:
+                # Exception for unknown nmbrs errors
                 self.unknown_error()
 
     def unknown_error(self):
         """Unknown error, No documentation found"""
         self.title = "Unknown Nmbrs error"
         self.cause = "Unknown"
         self.solution = f"Create a issue on our git page: {__git_issues__}"
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/company_service.py` & `nmbrs-1.0.2/src/nmbrs/service/company_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Module for handling the Company Nmbrs services."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from .microservices.company import (
     CompanyAddressService,
     CompanyBankAccountService,
     CompanyCostCenterService,
@@ -31,14 +33,16 @@
     ContactPerson,
     GuidConvertor,
     DefaultEmployeeTemplate,
     FulltimeSchedules,
     PayrollWorkflowTrack,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyService(Service):
     """A class representing Company Service for interacting with Nmbrs company-related functionalities."""
 
     def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
         super().__init__(auth_manager, sandbox)
 
@@ -59,14 +63,16 @@
         self.salary_table = CompanySalaryTableService(self.auth_manager, self.client)
         self.svw = CompanySvwService(self.auth_manager, self.client)
         self.wage_component = CompanyWageComponentService(self.auth_manager, self.client)
         self.wage_cost = CompanyWageCostService(self.auth_manager, self.client)
         self.wage_model = CompanyWageModelService(self.auth_manager, self.client)
         self.wage_tax = CompanyWageTaxService(self.auth_manager, self.client)
 
+        logger.info("CompanyService initialized.")
+
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:List_GetAll")
     def get_all(self) -> list[Company]:
         """
         Retrieve all companies.
 
         For more information, refer to the official documentation:
@@ -110,14 +116,15 @@
             employee_id (int): The ID of the employee.
 
         Returns:
             Company: A list of Company objects.
         """
         company = self.client.service.Company_GetCurrentByEmployeeId(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         if company is None:
+            logger.debug("No company found, for employee, ID: %s.", employee_id)
             return None
         return Company(serialize_object(company))
 
     @nmbrs_exception_handler(resource="CompanyService:Company_GetCurrentPeriod")
     def get_current_period(self, company_id: int) -> Period | None:
         """
         Get the current period of the company.
@@ -129,14 +136,15 @@
             company_id (int): The ID of the company.
 
         Returns:
             Period: year, period and period type and the company.
         """
         period = self.client.service.Company_GetCurrentPeriod(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         if period is None:
+            logger.debug("No current period found, for company, ID: %s.", company_id)
             return None
         return Period(company_id=company_id, data=serialize_object(period))
 
     @nmbrs_exception_handler(resource="CompanyService:Company_Insert")
     def post(
         self, debtor_id: int, name: str, period_type: int, default_id: int, labour_agreement_group_id: str, pay_in_advance: bool
     ) -> int:
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/debtor_service.py` & `nmbrs-1.0.2/src/nmbrs/service/debtor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Module for handling the Debtor Nmbrs services.
 """
 
+import logging
 from datetime import datetime
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from .microservices.debtor import DebtorDepartmentService, DebtorFunctionService, DebtorTitleService, DebtorWebHooksService
 from .service import Service
 from ..auth.token_manager import AuthManager
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
@@ -20,14 +22,16 @@
     LabourAgreementSettings,
     Manager,
     ServiceLevel,
     Tag,
     Domain,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class DebtorService(Service):
     """
     A class representing Debtor Service for interacting with Nmbrs debtor-related functionalities.
 
     Not implemented calls:
         1 [Converter_GetDebtors_IntToGuid](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Converter_GetDebtors_IntToGuid)
@@ -41,14 +45,16 @@
 
         # Micro services
         self.department = DebtorDepartmentService(self.auth_manager, self.client)
         self.function = DebtorFunctionService(self.auth_manager, self.client)
         self.webhook = DebtorWebHooksService(self.auth_manager, self.client)
         self.title = DebtorTitleService(self.auth_manager, self.client)
 
+        logger.info("DebtorService initialized.")
+
     @nmbrs_exception_handler(resource="DebtorService:Environment_Get")
     def get_domain(self, username: str, token: str) -> Domain:
         """
         Generate authentication header for standard token-based authentication.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Environment_Get)
@@ -110,14 +116,15 @@
             debtor_id (int): The ID of the debtor.
 
         Returns:
             Debtor | None: A Debtor object representing the debtor if found, otherwise None.
         """
         debtor = self.client.service.Debtor_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if debtor is None:
+            logger.debug("No debtor found, ID: %s.", debtor_id)
             return None
         return Debtor(serialize_object(debtor))
 
     @nmbrs_exception_handler(resource="DebtorService:Debtor_Insert")
     def post(self, debtor_id: int, number: str, name: str) -> int:
         """
         Insert a new debtor.
@@ -206,14 +213,15 @@
             debtor_id (int): The ID of the debtor.
 
         Returns:
             Address | None: An Address object representing the address if found, otherwise None.
         """
         address = self.client.service.Address_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if address is None:
+            logger.debug("No address found for debtor, ID: %s.", debtor_id)
             return None
         return Address(debtor_id=debtor_id, data=serialize_object(address))
 
     @nmbrs_exception_handler(resource="DebtorService:BankAccount_Get")
     def get_bank_account(self, debtor_id: int) -> BankAccount | None:
         """
         Retrieve bank account information for a debtor.
@@ -225,14 +233,15 @@
             debtor_id (int): The ID of the debtor.
 
         Returns:
             BankAccount | None: A BankAccount object representing the bank account if found, otherwise None.
         """
         bank_account = self.client.service.BankAccount_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if bank_account is None:
+            logger.debug("No bank account found for debtor, ID: %s.", debtor_id)
             return None
         return BankAccount(debtor_id=debtor_id, data=serialize_object(bank_account))
 
     @nmbrs_exception_handler(resource="DebtorService:ContactPerson_Get")
     def get_contact_person(self, debtor_id: int) -> ContactInfo | None:
         """
         Retrieve contact person information for a debtor.
@@ -244,14 +253,15 @@
             debtor_id (int): The ID of the debtor.
 
         Returns:
             ContactInfo | None: A ContactInfo object representing the contact person if found, otherwise None.
         """
         contact_person = self.client.service.ContactPerson_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if contact_person is None:
+            logger.debug("No contact person found for debtor, ID: %s.", debtor_id)
             return None
         return ContactInfo(debtor_id=debtor_id, data=serialize_object(contact_person))
 
     @nmbrs_exception_handler(resource="DebtorService:Debtor_IsOwner")
     def is_owner(self) -> bool:
         """
         Check if the current user is the owner of the debtor.
@@ -323,14 +333,15 @@
 
         Returns:
             ServiceLevel | None: A ServiceLevel object representing the service level information if found, otherwise
             None.
         """
         service_level = self.client.service.ServiceLevel_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if service_level is None:
+            logger.debug("No service level found for debtor, ID: %s.", debtor_id)
             return None
         return ServiceLevel(debtor_id=debtor_id, data=serialize_object(service_level))
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:Tags_Get")
     def get_tags(self, debtor_id: int) -> list[Tag]:
         """
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/employee_service.py` & `nmbrs-1.0.2/src/nmbrs/service/employee_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-# pylint: disable=line-too-long
 """
 Module for handling the Employee Nmbrs services.
 """
+
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from .microservices.employee import (
     EmployeeWageTaxService,
     EmployeeWageComponentsService,
     EmployeeAbsenceService,
@@ -38,14 +40,17 @@
 from .service import Service
 from ..auth.token_manager import AuthManager
 from ..data_classes.employee import EmployeeTypes, Employee, Period
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..utils.return_list import return_list
 
 
+logger = logging.getLogger(__name__)
+
+
 class EmployeeService(Service):
     """A class representing Employee Service for interacting with Nmbrs employee-related functionalities."""
 
     def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
         super().__init__(auth_manager, sandbox)
 
         # Initialize nmbrs services
@@ -77,14 +82,16 @@
         self.spaarloon = EmployeeSpaarloonService(self.auth_manager, self.client)  # TO BE implemented
         self.svw = EmployeeSvwService(self.auth_manager, self.client)  # TO BE implemented
         self.time_registration = EmployeeTimeRegistrationService(self.auth_manager, self.client)  # TO BE implemented
         self.time_schedule = EmployeeTimeScheduleService(self.auth_manager, self.client)  # TO BE implemented
         self.wage_component = EmployeeWageComponentsService(self.auth_manager, self.client)  # TO BE implemented
         self.wage_tax = EmployeeWageTaxService(self.auth_manager, self.client)  # TO BE implemented
 
+        logger.info("EmployeeService initialized.")
+
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:EmployeeType_GetList")
     def get_types(self) -> list[EmployeeTypes]:
         """
         Get the list of all employee types available.
 
         For more information, refer to the official documentation:
@@ -109,14 +116,15 @@
             employee_id (int): The ID of the employee.
 
         Returns:
             Period: year, period and period type and the company.
         """
         period = self.client.service.Employee_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         if period is None:
+            logger.debug("No current period found for employee, ID: %s.", employee_id)
             return None
         return Period(employee_id=employee_id, data=serialize_object(period))
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:List_GetByCompany")
     def get_by_company(self, company_id: int, employee_type: int) -> list[Employee]:
         """
@@ -182,15 +190,16 @@
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Employee_InsertByEmployeeType")
     def post_with_type(self):
         """
         Create a new employee based on the employee type and returns the Id of this employee.
-        If the date is before the company's current period, unprotected mode flag is required.
+        If the date is before th
+        e company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_InsertByEmployeeType](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_InsertByEmployeeType)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Employee_Transition")
@@ -250,20 +259,20 @@
 
         For more information, refer to the official documentation:
             [PerformanceReview_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:PerformanceReview_GetAll_AllEmployeesByCompany")
-    def get_all_performance_reviewa_by_company(self):
+    def get_all_performance_review_by_company(self):
         """
         Get the HR Performance Reviews for all the employees in the given Company ID.
 
         For more information, refer to the official documentation:
-            [PerformanceReview_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_GetAll_AllEmployeesByCompany)
+            [PerformanceReview_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_GetAll_AllEmployeesByCompany)  # pylint: disable=line-too-long
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Reports_GetJournalsReportByEmployee")
     def get_journal(self):
         """
         Returns the Journal Report for Employee.
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/address.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/address.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Microservice responsible for address-related actions on the company level."""
 
+import logging
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import Address
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..micro_service import MicroService
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyAddressService(MicroService):
     """Microservice responsible for address-related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
 
@@ -27,14 +30,15 @@
             company_id (int): The ID of the company.
 
         Returns:
             Address | None: An Address object if found, otherwise None.
         """
         address = self.client.service.Address_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         if address is None:
+            logger.debug("No address found, for company, ID: %s.", company_id)
             return None
         return Address(company_id=company_id, data=serialize_object(address))
 
     @nmbrs_exception_handler(resource="CompanyService:Address_Insert")
     def post(
         self,
         company_id: int,
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Microservice responsible for bank account related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import BankAccount
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyBankAccountService(MicroService):
     """Microservice responsible for bank account related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
 
@@ -27,14 +31,15 @@
             company_id (int): The ID of the company.
 
         Returns:
             BankAccount: An BankAccount object.
         """
         bank_account = self.client.service.BankAccount_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         if bank_account is None:
+            logger.debug("No bank account found, for company, ID: %s.", company_id)
             return None
         return BankAccount(company_id=company_id, data=serialize_object(bank_account))
 
     @nmbrs_exception_handler(resource="CompanyService:BankAccount_Insert")
     def post(
         self,
         company_id: int,
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for managing cost centers at the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import CostCenter
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyCostCenterService(MicroService):
     """Microservice responsible for managing cost centers at the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for cost unit related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import CostUnit
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyCostUnitService(MicroService):
     """Microservice responsible for cost unit related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for hour model related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import HourCode
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyHourModelService(MicroService):
     """Microservice responsible for hour model related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/journal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for journal related actions on the company level."""
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyJournalService(MicroService):
     """Microservice responsible for journal related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for labour agreement related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import LabourAgreement, LeaveTypeGroup
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyLabourAgreementService(MicroService):
     """
     Microservice responsible for labour agreement related actions on the company level.
     """
 
     def __init__(self, auth_manager: AuthManager, client: Client):
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/pension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for pension related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import Pension, PensionXML
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyPensionService(MicroService):
     """Microservice responsible for pension related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/run.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Microservice responsible for run related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import RunRequest, RunInfo
 from ....data_classes.employee import Employee
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyRunService(MicroService):
     """Microservice responsible for run related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for salary documents related actions on the company level."""
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class CompanySalaryDocumentService(MicroService):
     """Microservice responsible for salary documents related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for salary table related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import SalaryTable, SalaryTableScale, SalaryTableStep
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanySalaryTableService(MicroService):
     """Microservice responsible for salary table related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/svw.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Microservice responsible for svw related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import SVW
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class CompanySvwService(MicroService):
     """Microservice responsible for svw related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for wage component related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageComponent
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyWageComponentService(MicroService):
     """Microservice responsible for wage component related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_cost.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for managing wage cost related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageCost
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyWageCostService(MicroService):
     """Microservice responsible for managing wage cost related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_model.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for managing wage model related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageModel
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyWageModelService(MicroService):
     """Microservice responsible for managing wage model related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for managing wage tax-related actions on the company level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageTax, WageTaxXML
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class CompanyWageTaxService(MicroService):
     """Microservice responsible for managing wage tax-related actions on the company level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/department.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for department related actions on the debtor level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....auth.token_manager import AuthManager
 from ....data_classes.debtor import Department
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class DebtorDepartmentService(MicroService):
     """Microservice responsible for department related actions on the debtor level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for function related actions on the debtor level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....auth.token_manager import AuthManager
 from ....data_classes.debtor import Function
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class DebtorFunctionService(MicroService):
     """Microservice responsible for function related actions on the debtor level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/title.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Microservice responsible for title related actions on the debtor level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class DebtorTitleService(MicroService):
     """Microservice responsible for title related actions on the debtor level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for webhooks related actions on the debtor level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ....auth.token_manager import AuthManager
 from ....data_classes.debtor import WebhookSetting, Event
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class DebtorWebHooksService(MicroService):
     """Microservice responsible for webhooks related actions on the debtor level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/absence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Microservice responsible for absence related actions on the employee level."""
 
+import logging
 from datetime import datetime
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Absence
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeAbsenceService(MicroService):
     """Microservice responsible for absence related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for address related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Address
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeAddressService(MicroService):
     """Microservice responsible for address related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/bank_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for bank account related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import BankAccount
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeBankAccountService(MicroService):
     """Microservice responsible for bank account related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/child.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for child related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Child
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeChildService(MicroService):
     """Microservice responsible for child related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for contract related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Contract
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeContractService(MicroService):
     """Microservice responsible for contract related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for cost center related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import CostCenter
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeCostCenterService(MicroService):
     """Microservice responsible for cost center related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/department.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for departments related actions on the employee level."""
+import logging
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Department, DepartmentAll
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeDepartmentsService(MicroService):
     """Microservice responsible for departments related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
 
@@ -56,15 +59,21 @@
         _departments = []
         for employee in departments:
             for department in employee["EmployeeDepartments"]["Department_V2"]:
                 _departments.append(DepartmentAll(employee_id=employee["EmployeeId"], data=department))
         return _departments
 
     @nmbrs_exception_handler(resource="EmployeeService:Department_UpdateCurrent")
-    def update_current(self):
+    def update_current(self, employee_id: int, department_id: int):
         """
         Update the department starting the current period.
 
         For more information, refer to the official documentation:
             [Department_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Department_UpdateCurrent)
+
+        Args:
+            employee_id (int): The ID of the employee.
+            department_id (int): The ID of the employees new department.
         """
-        raise NotImplementedError()  # pragma: no cover
+        self.client.service.Department_UpdateCurrent(
+            EmployeeId=employee_id, DepartmentId=department_id, _soapheaders=self.auth_manager.header
+        )
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Microservice responsible for document related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeDocumentService(MicroService):
     """Microservice responsible for document related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/employment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for employment related actions on the employee level."""
+import logging
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Employment
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeEmploymentService(MicroService):
     """Microservice responsible for employment related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for function related actions on the employee level."""
+import logging
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Function, FunctionAll
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeFunctionService(MicroService):
     """Microservice responsible for function related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for hour component related actions on the employee level."""
+import logging
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeHourComponentFixedService(MicroService):
     """Microservice responsible for hour component related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Microservice responsible for labour agreement related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeLabourAgreementService(MicroService):
     """Microservice responsible for labour agreement related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for lease car related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import LeaseCar
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeLeaseCarService(MicroService):
     """Microservice responsible for lease car related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/leave.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Microservice responsible for leave related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeLeaveService(MicroService):
     """Microservice responsible for leave related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Microservice responsible for levens loop related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeLevensLoopService(MicroService):
     """Microservice responsible for levens loop related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/manager.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Microservice responsible for manager related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Manager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeManagerService(MicroService):
     """Microservice responsible for manager related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/partner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for partner related actions on the employee level."""
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 from ....data_classes.employee import Partner
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeePartnerService(MicroService):
     """Microservice responsible for partner related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/personal_info.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/personal_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for personal info related actions on the employee level."""
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import PersonalInfo, PersonalInfoContractSalaryAddress
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeePersonalInfoService(MicroService):
     """Microservice responsible for personal info related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/salary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for salary related actions on the employee level."""
+import logging
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Salary
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeSalaryService(MicroService):
     """Microservice responsible for salary related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/schedule.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # pylint: disable=line-too-long
 """Microservice responsible for schedule related actions on the employee level."""
+import logging
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Schedule
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeScheduleService(MicroService):
     """Microservice responsible for schedule related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for service related actions on the employee level."""
+import logging
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeServiceService(MicroService):
     """Microservice responsible for service related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for spaarloon related actions on the employee level."""
+import logging
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeSpaarloonService(MicroService):
     """Microservice responsible for spaarloon related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/svw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Microservice responsible for svw related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....data_classes.employee import SVW
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeSvwService(MicroService):
     """Microservice responsible for svw related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for time registration related actions on the employee level."""
+import logging
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeTimeRegistrationService(MicroService):
     """Microservice responsible for time registration related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_schedule.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/time_schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # pylint: disable=line-too-long
 """Microservice responsible for time schedule related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeTimeScheduleService(MicroService):
     """Microservice responsible for time schedule related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_component.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=line-too-long
 """Microservice responsible for wage components related actions on the employee level."""
+import logging
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeWageComponentsService(MicroService):
     """Microservice responsible for wage components related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_tax.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Microservice responsible for wage tax related actions on the employee level."""
 
+import logging
+
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class EmployeeWageTaxService(MicroService):
     """Microservice responsible for wage tax related actions on the employee level."""
 
     def __init__(self, auth_manager: AuthManager, client: Client):
         super().__init__(auth_manager, client)
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-1.0.2/src/nmbrs/service/microservices/micro_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Abstract base class for defining microservice interfaces.
 """
 
 from abc import ABC, abstractmethod
 
 from zeep import Client
 
-from src.nmbrs.auth.token_manager import AuthManager
+from ...auth.token_manager import AuthManager
 
 
 class MicroService(ABC):
     """
     Abstract base class for defining microservice interfaces.
 
     This class defines the common structure and methods required for interacting with microservices.
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/service.py` & `nmbrs-1.0.2/src/nmbrs/service/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Abstract base class for defining service interfaces."""
 
 from abc import ABC, abstractmethod
-from src.nmbrs.auth.token_manager import AuthManager
+from ..auth.token_manager import AuthManager
 
 
 class Service(ABC):
     """
     Abstract base class for defining service interfaces.
 
     This class serves as an abstract base class for defining interfaces for Nmbrs SOAP API services.
```

### Comparing `nmbrs-0.2.0/src/nmbrs/service/sso_service.py` & `nmbrs-1.0.2/src/nmbrs/service/sso_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Module for handling Single Sign-On (SSO) for Nmbrs services.
 """
 
+import logging
+
 from zeep import Client
 
 from .service import Service
-from ..auth.token_manager import AuthManager
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
 
+logger = logging.getLogger(__name__)
+
 
 class SingleSingOnService(Service):
     """
     A class responsible for managing Single Sign-On (SSO) for Nmbrs services.
     """
 
-    def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
-        super().__init__(auth_manager, sandbox)
+    def __init__(self, sandbox: bool = True):
+        super().__init__(None, sandbox)
 
         # Initialize nmbrs services
         self.sso_service = Client(f"{self.base_uri}{self.sso_uri}")
+        logger.info("SingleSignOnService initialized.")
 
     def get_sso_url(self, token: str, nmbrs_env: str, target: str = "nmbrs") -> str:
         """
         Generate the Single Sign-On (SSO) URL.
 
         Args:
             token (str): The authentication token.
@@ -30,15 +34,17 @@
             target (str, (optional)): The target application. Defaults to "nmbrs".
 
         Returns:
             str: The generated Single Sign-On URL.
         """
         if self.sso_url not in nmbrs_env:
             nmbrs_env = f"{nmbrs_env}{self.sso_url}"
-        return f"https://{nmbrs_env}/applications/common/externalactions.aspx?login={target}&ID={token}"
+        url = f"https://{nmbrs_env}/applications/common/externalactions.aspx?login={target}&ID={token}"
+        logger.debug("Generated SSO URL: %s", url)
+        return url
 
     @nmbrs_exception_handler(resource="SingleSignOn:GetToken")
     def get_token_with_password(self, username: str, password: str) -> str:
         """
         Get token for user. Valid for 30 seconds
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.2.0/src/nmbrs/utils/find_empty_params.py` & `nmbrs-1.0.2/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs/utils/return_list.py` & `nmbrs-1.0.2/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.2.0/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-1.0.2/src/nmbrs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 NOTICE
 README.md
 pyproject.toml
 setup.py
 src/nmbrs/__init__.py
+src/nmbrs/__logging__.py
 src/nmbrs/__version__.py
 src/nmbrs/api.py
 src/nmbrs.egg-info/PKG-INFO
 src/nmbrs.egg-info/SOURCES.txt
 src/nmbrs.egg-info/dependency_links.txt
 src/nmbrs.egg-info/requires.txt
 src/nmbrs.egg-info/top_level.txt
@@ -15,28 +16,31 @@
 src/nmbrs/auth/token_manager.py
 src/nmbrs/data_classes/__init__.py
 src/nmbrs/data_classes/company.py
 src/nmbrs/data_classes/data_class.py
 src/nmbrs/data_classes/debtor.py
 src/nmbrs/data_classes/employee.py
 src/nmbrs/data_classes/general.py
+src/nmbrs/data_classes/serialize.py
 src/nmbrs/data_classes/utils/__init__.py
 src/nmbrs/data_classes/utils/xml.py
 src/nmbrs/exceptions/__init__.py
 src/nmbrs/exceptions/exceptions.py
 src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+src/nmbrs/exceptions/nmbrs_exceptions/background_task.py
 src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
 src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
 src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
 src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
 src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
 src/nmbrs/service/__init__.py
 src/nmbrs/service/company_service.py
 src/nmbrs/service/debtor_service.py
 src/nmbrs/service/employee_service.py
+src/nmbrs/service/report_service.py
 src/nmbrs/service/service.py
 src/nmbrs/service/sso_service.py
 src/nmbrs/service/microservices/__init__.py
 src/nmbrs/service/microservices/micro_service.py
 src/nmbrs/service/microservices/company/__init__.py
 src/nmbrs/service/microservices/company/address.py
 src/nmbrs/service/microservices/company/bank_account.py
@@ -86,9 +90,10 @@
 src/nmbrs/service/microservices/employee/svw.py
 src/nmbrs/service/microservices/employee/time_registration.py
 src/nmbrs/service/microservices/employee/time_schedule.py
 src/nmbrs/service/microservices/employee/wage_component.py
 src/nmbrs/service/microservices/employee/wage_tax.py
 src/nmbrs/utils/__init__.py
 src/nmbrs/utils/find_empty_params.py
+src/nmbrs/utils/get_module_path.py
 src/nmbrs/utils/nmbrs_exception_handler.py
 src/nmbrs/utils/return_list.py
```

