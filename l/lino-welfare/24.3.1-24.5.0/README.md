# Comparing `tmp/lino-welfare-24.3.1.tar.gz` & `tmp/lino-welfare-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-welfare-24.3.1.tar", last modified: Thu Mar 14 17:48:56 2024, max compression
+gzip compressed data, was "lino-welfare-24.5.0.tar", last modified: Wed May  1 06:05:11 2024, max compression
```

## Comparing `lino-welfare-24.3.1.tar` & `lino-welfare-24.5.0.tar`

### file list

```diff
@@ -1,535 +1,533 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:53.000000 lino-welfare-24.3.1/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      239 2023-08-07 14:42:11.000000 lino-welfare-24.3.1/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     2187 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1130 2023-03-17 19:57:59.000000 lino-welfare-24.3.1/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.503755 lino-welfare-24.3.1/lino_welfare/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      687 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    23396 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)   230878 2024-02-14 17:29:48.000000 lino-welfare-24.3.1/lino_welfare/migrate_old.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.503755 lino-welfare-24.3.1/lino_welfare/modlib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      659 2017-06-14 02:24:21.000000 lino-welfare-24.3.1/lino_welfare/modlib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.503755 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      561 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.503755 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1050 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-24.3.1/lino_welfare/modlib/active_job_search__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.503755 lino-welfare-24.3.1/lino_welfare/modlib/aids/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1537 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2392 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1142 2020-07-22 09:24:05.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2019-08-01 14:29:04.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       65 2015-09-19 03:53:59.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/default.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      713 2015-09-19 03:53:59.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      863 2023-10-19 09:52:50.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      803 2023-10-19 09:49:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-10-19 09:58:10.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      564 2018-05-25 10:09:23.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      763 2015-09-19 03:53:59.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5158 2024-01-29 19:47:15.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html
--rw-rw-r--   0 luc       (1000) www-data    (33)      966 2023-10-19 13:58:36.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/aids/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:00.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6792 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6710 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    11656 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    28023 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      365 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/aids/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/art60/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1137 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/art60/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/art60/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/art60/config/art60/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/art60/config/art60/Contract/
--rw-rw-r--   0 luc       (1000) www-data    (33)    46358 2022-10-05 09:08:36.000000 lino-welfare-24.3.1/lino_welfare/modlib/art60/config/art60/Contract/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/art60/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/art60/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      813 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/art60/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11511 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/art60/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/art61/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      982 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/art61/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1702 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/art61/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/art61/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/art61/config/art61/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/art61/config/art61/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8721 2015-09-19 03:53:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/art61/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/art61/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      346 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/art61/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8571 2024-02-20 04:55:13.000000 lino-welfare-24.3.1/lino_welfare/modlib/art61/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/badges/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1240 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/badges/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1525 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/badges/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/cal/
--rw-rw-r--   0 luc       (1000) www-data    (33)      537 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cal/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/Guest/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1249 2015-09-19 03:53:48.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2015-09-19 03:53:48.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/Guest/Visitor.eml.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1700 2016-03-11 22:32:06.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:48.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       44 2016-02-22 08:52:32.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      826 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       43 2016-02-22 08:52:32.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    14228 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.507755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8464 2016-11-17 14:00:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4120 2017-04-21 06:04:21.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3740 2019-10-02 18:54:22.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2846 2015-09-19 03:53:40.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.511755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    23800 2016-07-01 08:28:52.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    15771 2016-05-18 07:19:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3353 2016-05-18 07:19:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2075 2015-09-19 03:53:40.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.511755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.511755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/20190612/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11616 2016-09-30 09:59:39.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)   139908 2016-09-30 09:59:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    16746 2013-12-23 11:43:40.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1639 2013-11-06 13:08:24.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)      154 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/README.txt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.511755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8507 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)      777 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)      933 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4198 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.511755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9867 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7931 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1042 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.511755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5622 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13874 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5569 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5699 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9421 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    19800 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1600 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4063 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5074 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3334 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2591 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1460 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3450 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3938 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11981 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5436 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6504 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3332 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1119 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1969 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1044 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4562 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3627 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6440 2015-09-19 03:53:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3491 2019-03-22 11:35:44.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2902 2019-03-22 11:35:44.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    26504 2019-03-22 11:35:44.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/
--rw-rw-rw-   0 luc       (1000) www-data    (33)   121083 2019-03-22 11:35:44.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4940 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3228 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    21764 2015-09-19 03:53:40.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    15865 2015-09-19 03:53:40.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      537 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/cbss.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3647 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/cbss_demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1961 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2109 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2579 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4542 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1826 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11618 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    24155 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    26292 2015-11-29 20:09:07.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      618 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/democfg.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6231 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/garble_tx25.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    20869 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9316 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/purposes.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2507 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/sectors.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    16822 2016-09-29 13:14:34.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    23231 2016-09-30 11:44:50.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    25160 2016-09-30 11:41:01.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/cbss/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1894 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    23988 2024-03-14 04:37:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    24524 2024-03-14 04:38:33.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      402 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/roles.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    37719 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/tx25.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9240 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/ui.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2469 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/cbss/utils.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.515756 lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      653 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3858 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1808 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2016-07-06 14:59:14.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-07-06 14:59:14.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/fixtures/std.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/contacts/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:26:17.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/contacts/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:27:23.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10075 2024-02-20 08:22:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/cv/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      477 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/cv/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      969 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5613 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/props.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-02-22 08:56:29.000000 lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5590 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/cv/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/debts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1585 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4438 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/debts/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.495755 lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    17514 2018-09-28 15:27:47.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/Default.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    24679 2015-09-19 03:53:44.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    19964 2015-09-19 03:53:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      661 2023-04-01 16:59:59.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/fields.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:44.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4835 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    18261 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/minimal.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      576 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1888 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    22758 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      350 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/roles.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    21587 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/debts/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      814 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:03.000000 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      420 2021-04-14 07:26:11.000000 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1924 2021-04-07 10:22:54.000000 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1695 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/esf/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      848 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6435 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/Client/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      742 2020-11-20 03:16:25.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/ClientSummary/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      905 2016-06-07 02:40:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      620 2018-03-08 12:32:06.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/esf/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-01-19 01:49:31.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      360 2018-05-25 08:15:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      465 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     5668 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/esf/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/finan/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      379 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/finan/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.519755 lino-welfare-24.3.1/lino_welfare/modlib/finan/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-12-12 21:53:36.000000 lino-welfare-24.3.1/lino_welfare/modlib/finan/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      465 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/finan/fixtures/payments.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1994 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/finan/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/households/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      305 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/households/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/households/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/households/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-02-22 08:57:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/households/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       50 2016-02-22 08:57:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/households/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3744 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/households/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/immersion/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1105 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/immersion/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/immersion/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)   667935 2018-05-10 19:37:42.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5587 2016-02-11 13:18:18.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/immersion/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:47.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1454 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3677 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3923 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/immersion/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/integ/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2373 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/integ/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/integ/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:46.000000 lino-welfare-24.3.1/lino_welfare/modlib/integ/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8535 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/integ/fixtures/demo.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2927 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/integ/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    24402 2024-02-19 04:11:43.000000 lino-welfare-24.3.1/lino_welfare/modlib/integ/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      377 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/integ/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/isip/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      350 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/isip/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      725 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/isip/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/isip/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/isip/config/isip/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/isip/config/isip/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    55172 2016-08-02 05:50:22.000000 lino-welfare-24.3.1/lino_welfare/modlib/isip/config/isip/Contract/Default.odt
--rw-rw-r--   0 luc       (1000) www-data    (33)    18379 2024-03-14 04:51:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/isip/mixins.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    12092 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/isip/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      902 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    94813 2015-09-19 03:54:01.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9896 2015-09-19 03:54:01.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9876 2015-09-19 03:54:01.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/jobs/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      834 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2955 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13624 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      328 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/template_messages.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    17473 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/jobs/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/ledger/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      418 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/ledger/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      550 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2746 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3082 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/std_journals.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/ledger/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.523755 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      995 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3551 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/fixtures/demo.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    17187 2024-02-27 09:05:10.000000 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      415 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/newcomers/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/notes/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      281 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/notes/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/notes/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:57.000000 lino-welfare-24.3.1/lino_welfare/modlib/notes/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      888 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/notes/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 09:05:22.000000 lino-welfare-24.3.1/lino_welfare/modlib/notes/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2531 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/notes/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1513 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     4553 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/actions.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2556 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/choicelists.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      363 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/client_address.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    32053 2015-09-19 03:53:51.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)   157223 2015-09-19 03:53:51.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    31905 2015-09-19 03:53:51.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      373 2015-09-19 03:53:51.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/pac.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2015-09-19 03:53:51.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/welcome.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2589 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1629 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    37817 2024-02-20 22:33:59.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      510 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/pcsw/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/polls/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      334 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/polls/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/polls/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:39.000000 lino-welfare-24.3.1/lino_welfare/modlib/polls/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5826 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/polls/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      326 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/polls/fixtures/jobsearch.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-07-06 15:15:32.000000 lino-welfare-24.3.1/lino_welfare/modlib/polls/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/polls/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/projects/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      617 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/projects/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1960 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/projects/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/reception/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      531 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/reception/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    15233 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/reception/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/sales/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-24.3.1/lino_welfare/modlib/sales/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      467 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/sales/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/sepa/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      303 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/sepa/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/sepa/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-24.3.1/lino_welfare/modlib/sepa/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4141 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/sepa/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1576 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/sepa/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/system/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      216 2021-04-07 10:22:54.000000 lino-welfare-24.3.1/lino_welfare/modlib/system/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4120 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/system/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      339 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:57:01.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:57:01.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2699 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1111 2024-02-27 09:00:59.000000 lino-welfare-24.3.1/lino_welfare/modlib/users/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      406 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.527756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)   672907 2021-02-18 17:59:31.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      511 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/TasksByClient.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1221 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      533 2015-10-21 13:33:32.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       40 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/default.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      624 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      800 2021-02-03 10:12:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/base.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/integ/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/integ/ActivityReport/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11787 2015-09-19 03:53:54.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      585 2021-02-18 18:02:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/letter_margin_bottom.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/notes/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/notes/Note/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    50685 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:55.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    44275 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1026 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    30606 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/pp2lino.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4488 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3698 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/std2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    26063 2024-03-13 04:13:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/help_texts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    38160 2024-02-20 08:34:16.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 luc       (1000) www-data    (33)   131735 2024-02-20 08:34:16.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.531756 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    35510 2024-03-03 14:31:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 luc       (1000) www-data    (33)   130540 2024-03-03 14:31:45.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/nl/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    18043 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/cpas2lino.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4782 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/garble.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4526 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/gd2lino.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    14714 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/initdb_tim.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    35617 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/watch_tim.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5553 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     6237 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6974 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1636 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/lino_welfare/modlib/welfare/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1054 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/courses/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/courses/Course/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    12127 2015-09-19 03:53:49.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    12100 2015-09-19 03:53:49.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:49.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3041 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    20712 2024-02-14 17:29:27.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      363 2021-04-07 10:22:54.000000 lino-welfare-24.3.1/lino_welfare/modlib/xcourses/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      204 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/gerd/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      296 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      416 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/django110_isnull.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      278 2023-01-10 07:35:10.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/manage.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1372 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/print_tx25.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      342 2021-04-16 02:21:20.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      837 2024-02-21 14:55:09.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      389 2024-02-14 17:29:45.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/doctests.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/beid/
--rw-rw-r--   0 luc       (1000) www-data    (33)     3046 2024-03-14 05:47:20.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
--rw-rw-r--   0 luc       (1000) www-data    (33)     7615 2024-03-14 05:47:20.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/webdav/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/webdav/userdocs/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/
--rw-rw-r--   0 luc       (1000) www-data    (33)    13378 2024-03-14 05:51:38.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       86 2024-02-14 17:29:45.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/memory.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1039 2024-02-14 17:29:45.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/mysql.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2610 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_aids.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2756 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_broken_gfks.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8257 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_cbss.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2944 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_clients.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4184 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_debts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      253 2021-02-15 14:17:17.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_restore.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    35711 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_watchtim.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.535755 lino-welfare-24.3.1/lino_welfare/projects/mathieu/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      364 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      280 2023-01-10 07:35:10.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/manage.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      280 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      512 2024-02-27 08:51:22.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/doctests.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.499755 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/media/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/media/beid/
--rw-rw-r--   0 luc       (1000) www-data    (33)     3046 2024-03-14 05:48:10.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
--rw-rw-r--   0 luc       (1000) www-data    (33)     7615 2024-03-14 05:48:10.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
--rw-rw-rw-   0 luc       (1000) www-data    (33)       86 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/memory.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/projects/mathieu/t/
--rw-rw-r--   0 luc       (1000) www-data    (33)      244 2024-02-26 06:37:02.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/t/restore.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/projects/mathieu/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-02-06 12:35:36.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/tests/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7316 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/tests/test_chatelet.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    19006 2024-02-14 17:29:29.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/tests/test_notify.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/projects/mathieu/tmp/
--rw-rw-r--   0 luc       (1000) www-data    (33)      244 2024-02-26 06:37:19.000000 lino-welfare-24.3.1/lino_welfare/projects/mathieu/tmp/restore.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/projects/weleup1r/
--rw-rw-r--   0 luc       (1000) www-data    (33)        0 2023-12-04 12:57:37.000000 lino-welfare-24.3.1/lino_welfare/projects/weleup1r/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      276 2023-12-03 15:07:00.000000 lino-welfare-24.3.1/lino_welfare/projects/weleup1r/manage.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      433 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/projects/weleup1r/settings.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare/scripts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:30.000000 lino-welfare-24.3.1/lino_welfare/scripts/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7378 2024-02-14 17:29:28.000000 lino-welfare-24.3.1/lino_welfare/scripts/load_plp.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7896 2024-03-14 17:48:43.000000 lino-welfare-24.3.1/lino_welfare/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/lino_welfare.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     2187 2024-03-14 17:48:56.000000 lino-welfare-24.3.1/lino_welfare.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)    18264 2024-03-14 17:48:56.000000 lino-welfare-24.3.1/lino_welfare.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-03-14 17:48:56.000000 lino-welfare-24.3.1/lino_welfare.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-09-02 10:20:26.000000 lino-welfare-24.3.1/lino_welfare.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2024-03-14 17:48:56.000000 lino-welfare-24.3.1/lino_welfare.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       13 2024-03-14 17:48:56.000000 lino-welfare-24.3.1/lino_welfare.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)      149 2023-08-17 15:07:46.000000 lino-welfare-24.3.1/requirements-install.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)      349 2024-03-03 14:33:45.000000 lino-welfare-24.3.1/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      164 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      617 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-14 17:48:56.539756 lino-welfare-24.3.1/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      558 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/tests/test_demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      162 2024-02-14 17:29:26.000000 lino-welfare-24.3.1/tests/test_docs.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.525815 lino-welfare-24.5.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:53.000000 lino-welfare-24.5.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      239 2023-08-07 14:42:11.000000 lino-welfare-24.5.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     2187 2024-05-01 06:05:11.525815 lino-welfare-24.5.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1130 2023-03-17 19:57:59.000000 lino-welfare-24.5.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.489816 lino-welfare-24.5.0/lino_welfare/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      687 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    23396 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   230878 2024-02-14 17:29:48.000000 lino-welfare-24.5.0/lino_welfare/migrate_old.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.489816 lino-welfare-24.5.0/lino_welfare/modlib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      657 2024-03-25 11:24:31.000000 lino-welfare-24.5.0/lino_welfare/modlib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.489816 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      561 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.489816 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1050 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-24.5.0/lino_welfare/modlib/active_job_search__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.489816 lino-welfare-24.5.0/lino_welfare/modlib/aids/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1537 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2392 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1142 2020-07-22 09:24:05.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2019-08-01 14:29:04.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       65 2015-09-19 03:53:59.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/default.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      713 2015-09-19 03:53:59.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      863 2023-10-19 09:52:50.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      803 2023-10-19 09:49:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-10-19 09:58:10.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      564 2018-05-25 10:09:23.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      763 2015-09-19 03:53:59.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5158 2024-01-29 19:47:15.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)      966 2023-10-19 13:58:36.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/aids/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:00.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6792 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6710 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    11656 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    28073 2024-03-24 06:41:17.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      365 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/aids/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/art60/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1137 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/art60/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/art60/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/art60/config/art60/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/art60/config/art60/Contract/
+-rw-rw-r--   0 luc       (1000) www-data    (33)    46358 2022-10-05 09:08:36.000000 lino-welfare-24.5.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/art60/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-24.5.0/lino_welfare/modlib/art60/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      813 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/art60/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11592 2024-04-30 13:14:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/art60/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/art61/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      982 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/art61/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1702 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/art61/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/art61/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/art61/config/art61/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/art61/config/art61/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8721 2015-09-19 03:53:45.000000 lino-welfare-24.5.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/art61/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-24.5.0/lino_welfare/modlib/art61/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      346 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/art61/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8596 2024-03-24 06:41:34.000000 lino-welfare-24.5.0/lino_welfare/modlib/art61/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/badges/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1240 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/badges/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1525 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/badges/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/cal/
+-rw-rw-r--   0 luc       (1000) www-data    (33)      537 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cal/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/Guest/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1249 2015-09-19 03:53:48.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2015-09-19 03:53:48.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/Guest/Visitor.eml.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1700 2016-03-11 22:32:06.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:48.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       44 2016-02-22 08:52:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      826 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       43 2016-02-22 08:52:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    14251 2024-03-25 03:50:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8464 2016-11-17 14:00:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4120 2017-04-21 06:04:21.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3740 2019-10-02 18:54:22.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2846 2015-09-19 03:53:40.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.493816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    23800 2016-07-01 08:28:52.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    15771 2016-05-18 07:19:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3353 2016-05-18 07:19:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2075 2015-09-19 03:53:40.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.497815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.497815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/20190612/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11616 2016-09-30 09:59:39.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   139908 2016-09-30 09:59:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    16746 2013-12-23 11:43:40.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1639 2013-11-06 13:08:24.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      154 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/README.txt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.497815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8507 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      777 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      933 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4198 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.497815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9867 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7931 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1042 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.497815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5622 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13874 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5569 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5699 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9421 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    19800 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.497815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1600 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4063 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5074 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3334 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2591 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1460 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3450 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3938 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11981 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5436 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6504 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3332 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1119 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1969 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1044 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4562 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3627 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6440 2015-09-19 03:53:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3491 2019-03-22 11:35:44.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2902 2019-03-22 11:35:44.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    26504 2019-03-22 11:35:44.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   121083 2019-03-22 11:35:44.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4940 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3228 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    21764 2015-09-19 03:53:40.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    15865 2015-09-19 03:53:40.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      537 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/cbss.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3647 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1961 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2109 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2579 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4542 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1826 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11618 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    24155 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    26292 2015-11-29 20:09:07.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      618 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/democfg.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6231 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    20869 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9316 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/purposes.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2507 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/sectors.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    16822 2016-09-29 13:14:34.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    23231 2016-09-30 11:44:50.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    25160 2016-09-30 11:41:01.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/cbss/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1894 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    23988 2024-03-14 04:37:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    24524 2024-03-14 04:38:33.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      402 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/roles.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    37719 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/tx25.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9240 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/ui.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2469 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/cbss/utils.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      653 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3858 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1810 2024-03-25 11:04:19.000000 lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.501815 lino-welfare-24.5.0/lino_welfare/modlib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2016-07-06 14:59:14.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-07-06 14:59:14.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/fixtures/std.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/contacts/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:26:17.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/contacts/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:27:23.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10259 2024-04-30 19:18:49.000000 lino-welfare-24.5.0/lino_welfare/modlib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/cv/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      477 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/cv/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      969 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5613 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/props.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-02-22 08:56:29.000000 lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5590 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/cv/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/debts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1585 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4438 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/debts/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    17514 2018-09-28 15:27:47.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    24679 2015-09-19 03:53:44.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    19964 2015-09-19 03:53:43.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      661 2023-04-01 16:59:59.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/fields.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:44.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4835 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    18261 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/minimal.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      576 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1888 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    22758 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      350 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/roles.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    21587 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/debts/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      814 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:03.000000 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      420 2021-04-14 07:26:11.000000 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1924 2021-04-07 10:22:54.000000 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1695 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/esf/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      848 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6435 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/Client/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      742 2020-11-20 03:16:25.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/ClientSummary/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      905 2016-06-07 02:40:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      620 2018-03-08 12:32:06.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/esf/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-01-19 01:49:31.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      360 2018-05-25 08:15:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      465 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     5668 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/esf/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.505815 lino-welfare-24.5.0/lino_welfare/modlib/finan/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      379 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/finan/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/finan/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-12-12 21:53:36.000000 lino-welfare-24.5.0/lino_welfare/modlib/finan/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      465 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/finan/fixtures/payments.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1994 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/finan/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/households/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      305 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/households/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/households/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-24.5.0/lino_welfare/modlib/households/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-02-22 08:57:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/households/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       50 2016-02-22 08:57:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/households/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3744 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/households/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/immersion/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1105 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/immersion/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/immersion/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   667935 2018-05-10 19:37:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5587 2016-02-11 13:18:18.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/immersion/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:47.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1454 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3677 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3948 2024-03-24 06:42:10.000000 lino-welfare-24.5.0/lino_welfare/modlib/immersion/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/integ/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2373 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/integ/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/integ/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:46.000000 lino-welfare-24.5.0/lino_welfare/modlib/integ/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8558 2024-04-30 07:49:15.000000 lino-welfare-24.5.0/lino_welfare/modlib/integ/fixtures/demo.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2927 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/integ/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    24284 2024-03-24 06:43:20.000000 lino-welfare-24.5.0/lino_welfare/modlib/integ/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      377 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/integ/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/isip/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      350 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/isip/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      725 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/isip/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/isip/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.481816 lino-welfare-24.5.0/lino_welfare/modlib/isip/config/isip/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/isip/config/isip/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    55172 2016-08-02 05:50:22.000000 lino-welfare-24.5.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    18404 2024-03-24 06:43:31.000000 lino-welfare-24.5.0/lino_welfare/modlib/isip/mixins.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    12117 2024-03-24 06:43:42.000000 lino-welfare-24.5.0/lino_welfare/modlib/isip/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/jobs/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      902 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    94813 2015-09-19 03:54:01.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9896 2015-09-19 03:54:01.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9876 2015-09-19 03:54:01.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/jobs/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      834 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2955 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14082 2024-04-30 10:36:15.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      328 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/template_messages.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    18488 2024-05-01 01:55:34.000000 lino-welfare-24.5.0/lino_welfare/modlib/jobs/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/ledger/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      418 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/ledger/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.509815 lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      550 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2746 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3082 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/std_journals.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/ledger/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      995 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3551 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/fixtures/demo.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    17244 2024-03-24 06:45:29.000000 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      415 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/newcomers/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/notes/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      281 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/notes/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/notes/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:57.000000 lino-welfare-24.5.0/lino_welfare/modlib/notes/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      888 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/notes/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 09:05:22.000000 lino-welfare-24.5.0/lino_welfare/modlib/notes/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2531 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/notes/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1513 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4553 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/actions.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2556 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/choicelists.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      363 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/client_address.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    32053 2015-09-19 03:53:51.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   157223 2015-09-19 03:53:51.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    31905 2015-09-19 03:53:51.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      373 2015-09-19 03:53:51.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/pac.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2015-09-19 03:53:51.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/welcome.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2589 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1629 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    37842 2024-03-24 06:45:54.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      510 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/pcsw/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/polls/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      334 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/polls/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/polls/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:39.000000 lino-welfare-24.5.0/lino_welfare/modlib/polls/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5826 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/polls/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      326 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/polls/fixtures/jobsearch.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-07-06 15:15:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/polls/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/polls/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/projects/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      617 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/projects/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1960 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/projects/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/reception/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      531 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/reception/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    15233 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/reception/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/sepa/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      303 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/sepa/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/sepa/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/sepa/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4141 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/sepa/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1576 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/sepa/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/system/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      216 2021-04-07 10:22:54.000000 lino-welfare-24.5.0/lino_welfare/modlib/system/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4120 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/system/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/trading/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-24.5.0/lino_welfare/modlib/trading/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      390 2024-03-25 11:24:57.000000 lino-welfare-24.5.0/lino_welfare/modlib/trading/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      339 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.513815 lino-welfare-24.5.0/lino_welfare/modlib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:57:01.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:57:01.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2699 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1111 2024-02-27 09:00:59.000000 lino-welfare-24.5.0/lino_welfare/modlib/users/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      406 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   672907 2021-02-18 17:59:31.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      511 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/TasksByClient.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1221 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      533 2015-10-21 13:33:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       40 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/default.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      624 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      800 2021-02-03 10:12:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/integ/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11787 2015-09-19 03:53:54.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      585 2021-02-18 18:02:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/notes/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/notes/Note/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    50685 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    44866 2024-04-30 08:35:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1026 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    30606 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4488 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3698 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/std2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    27345 2024-04-30 23:56:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/help_texts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    38160 2024-04-08 10:14:32.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)   132194 2024-04-30 10:49:37.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    35592 2024-04-30 10:49:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)   130844 2024-04-30 10:49:58.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/nl/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.517815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    18043 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4782 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/garble.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4526 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    14714 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    35617 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5553 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     6245 2024-03-27 08:42:23.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6974 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1636 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/lino_welfare/modlib/welfare/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1054 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/courses/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/courses/Course/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    12127 2015-09-19 03:53:49.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    12100 2015-09-19 03:53:49.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:49.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3041 2024-02-14 17:29:27.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    20643 2024-03-24 06:46:55.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      363 2021-04-07 10:22:54.000000 lino-welfare-24.5.0/lino_welfare/modlib/xcourses/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      204 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/gerd/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      296 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      416 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/django110_isnull.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      278 2023-01-10 07:35:10.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/manage.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1372 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/print_tx25.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      342 2021-04-16 02:21:20.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      837 2024-02-21 14:55:09.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      389 2024-02-14 17:29:45.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/doctests.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/beid/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3046 2024-05-01 01:57:36.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7615 2024-05-01 01:57:36.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/webdav/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/
+-rw-rw-r--   0 luc       (1000) www-data    (33)    13381 2024-05-01 02:01:59.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       86 2024-02-14 17:29:45.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/memory.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1039 2024-02-14 17:29:45.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/mysql.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2610 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_aids.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2756 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8257 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_cbss.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2944 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_clients.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4184 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_debts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      253 2021-02-15 14:17:17.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_restore.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    35711 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_watchtim.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/mathieu/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      364 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      280 2023-01-10 07:35:10.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/manage.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      280 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      512 2024-03-21 08:57:59.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/doctests.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.485816 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/media/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/media/beid/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3046 2024-05-01 01:58:25.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7615 2024-05-01 01:58:25.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       86 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/memory.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/mathieu/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-02-06 12:35:36.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/tests/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7316 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/tests/test_chatelet.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    19006 2024-02-14 17:29:29.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/tests/test_notify.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/mathieu/tmp/
+-rw-rw-r--   0 luc       (1000) www-data    (33)      244 2024-02-26 06:37:19.000000 lino-welfare-24.5.0/lino_welfare/projects/mathieu/tmp/restore.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.521815 lino-welfare-24.5.0/lino_welfare/projects/weleup1r/
+-rw-rw-r--   0 luc       (1000) www-data    (33)        0 2023-12-04 12:57:37.000000 lino-welfare-24.5.0/lino_welfare/projects/weleup1r/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      276 2023-12-03 15:07:00.000000 lino-welfare-24.5.0/lino_welfare/projects/weleup1r/manage.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      433 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/projects/weleup1r/settings.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.525815 lino-welfare-24.5.0/lino_welfare/scripts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:30.000000 lino-welfare-24.5.0/lino_welfare/scripts/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7378 2024-02-14 17:29:28.000000 lino-welfare-24.5.0/lino_welfare/scripts/load_plp.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7898 2024-05-01 06:04:58.000000 lino-welfare-24.5.0/lino_welfare/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.525815 lino-welfare-24.5.0/lino_welfare.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     2187 2024-05-01 06:05:11.000000 lino-welfare-24.5.0/lino_welfare.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    18225 2024-05-01 06:05:11.000000 lino-welfare-24.5.0/lino_welfare.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-05-01 06:05:11.000000 lino-welfare-24.5.0/lino_welfare.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-09-02 10:20:26.000000 lino-welfare-24.5.0/lino_welfare.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2024-05-01 06:05:11.000000 lino-welfare-24.5.0/lino_welfare.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       13 2024-05-01 06:05:11.000000 lino-welfare-24.5.0/lino_welfare.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)      149 2023-08-17 15:07:46.000000 lino-welfare-24.5.0/requirements-install.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)      349 2024-03-03 14:33:45.000000 lino-welfare-24.5.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-05-01 06:05:11.525815 lino-welfare-24.5.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      164 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      617 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:05:11.525815 lino-welfare-24.5.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      558 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/tests/test_demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      162 2024-02-14 17:29:26.000000 lino-welfare-24.5.0/tests/test_docs.py
```

### Comparing `lino-welfare-24.3.1/COPYING` & `lino-welfare-24.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/PKG-INFO` & `lino-welfare-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-welfare
-Version: 24.3.1
+Version: 24.5.0
 Summary: A Lino plugin library for Belgian PCSWs
 Home-page: https://gitlab.com/lino-framework/welfare
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lino-welfare-24.3.1/README.rst` & `lino-welfare-24.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/__init__.py` & `lino-welfare-24.5.0/lino_welfare/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/migrate.py` & `lino-welfare-24.5.0/lino_welfare/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/migrate_old.py` & `lino-welfare-24.5.0/lino_welfare/migrate_old.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,26 +23,26 @@
     aids
     badges
     immersion
     esf
 
 The following plugins are extensions of their respective version in
 :mod:`lino.modlib`:
-    
+
 .. autosummary::
    :toctree:
 
 
     cal
     cv
     households
     notes
     polls
     ledger
-    sales
+    trading
     sepa
     system
     users
 
 The following plugins are not being used:
 
 .. autosummary::
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/active_job_search/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/active_job_search/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/mixins.py` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/aids/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/aids/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     )
 
     params_layout = "board aid_type user signer state"
 
     @classmethod
     def get_request_queryset(self, ar):
         qs = super(Grantings, self).get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         if pv.aid_type:
             qs = qs.filter(aid_type=pv.aid_type)
         if pv.board:
             qs = qs.filter(board=pv.board)
         # if pv.user:
         #     qs = qs.filter(user=pv.user)
         # if pv.signer:
@@ -392,15 +392,15 @@
 
     params_layout = """start_date end_date observed_event board signer user
     aid_type state client gender"""
 
     @classmethod
     def get_request_queryset(self, ar):
         qs = super(Confirmations, self).get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         if pv.observed_event:
             qs = pv.observed_event.add_filter(qs, pv)
         if pv.aid_type:
             qs = qs.filter(granting__aid_type=pv.aid_type)
         if pv.gender:
             qs = qs.filter(client__gender=pv.gender)
         if pv.board:
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art60/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/art60/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art60/config/art60/Contract/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art60/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/art60/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art60/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/art60/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2015-2022 Rumma & Ko Ltd
+# Copyright 2015-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 from lino import logger
 
 from django.conf import settings
 from django.db import models
 from django.db.models import Q
@@ -97,15 +97,15 @@
 
 class Convention(ContractPartnerBase, UploadController):
 
     class Meta:
         verbose_name = _("Art60§7 convention")
         verbose_name_plural = _('Art60§7 conventions')
 
-    company = dd.ForeignKey(
+    company = dd.ForeignKey(  # ContractPartnerBase requires a field "company"
         "jobs.JobProvider",
         related_name="%(app_label)s_%(class)s_set_by_company",
         blank=True,
         null=True)
 
     contract = dd.ForeignKey("art60.Contract")
     job = dd.ForeignKey("jobs.Job")
@@ -122,17 +122,17 @@
     refund_rate = models.CharField(_("refund rate"),
                                    max_length=200,
                                    blank=True)
 
     def __str__(self):
         return "{} {}".format(dd.fds(self.start_date), self.job)
 
-    @dd.chooser()
-    def company_choices(cls):
-        return rt.models.jobs.JobProvider.objects.all()
+    # @dd.chooser()
+    # def company_choices(cls):
+    #     return rt.models.jobs.JobProvider.objects.all()
 
     def full_clean(self, *args, **kw):
         if self.job_id is not None:
             if self.job.provider is not None:
                 self.company = self.job.provider
             if self.job.contract_type is not None:
                 self.type = self.job.contract_type
@@ -253,15 +253,15 @@
         yield 'convention__company__type'
         yield 'convention__company'
         yield 'convention__job'
 
     @classmethod
     def get_request_queryset(cls, ar):
         qs = super().get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         if pv.company:
             qs = qs.filter(convention__company=pv.company)
         if pv.start_monthly_refund:
             qs = qs.filter(
                 convention__monthly_refund__gte=pv.start_monthly_refund)
         if pv.end_monthly_refund:
             qs = qs.filter(
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art61/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/art61/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art61/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/art61/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/art61/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/art61/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     user type start_date end_date observed_event
     company ending_success ending
     """
 
     @classmethod
     def get_request_queryset(cls, ar):
         qs = super(Contracts, cls).get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         if pv.company:
             qs = qs.filter(company=pv.company)
         return qs
 
 
 class ContractsByClient(Contracts):
     required_roles = dd.login_required((IntegUser, SocialCoordinator))
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/badges/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/badges/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/badges/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/badges/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cal/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cal/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html` & `lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cal/fixtures/demo2.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cal/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cal/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cal/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,17 +183,15 @@
                         role=settings.SITE.site_config.client_guestrole)
 
 
 dd.update_field(Event, 'user', verbose_name=_("Managed by"))
 
 
 class EntriesByClient(Events):
-    """
-    Events where :attr:`Event.project` **or** one guest is this client.
-    """
+    # Events where :attr:`Event.project` **or** one guest is this client.
     required_roles = dd.login_required((OfficeUser, OfficeOperator))
     # master_key = 'project'
     # master = 'cal.Event'
     order_by = ["-start_date", "-start_time", "id"]
     master = 'pcsw.Client'
     auto_fit_column_widths = True
     column_names = 'when_text user summary workflow_buttons *'
@@ -201,20 +199,21 @@
     insert_layout = """
     event_type
     summary
     start_date start_time end_date end_time
     """
 
     @classmethod
-    def get_queryset(self, ar):
+    def get_request_queryset(cls, ar):
+        qs = super().get_request_queryset(ar)
         mi = ar.master_instance
         if mi is None:
             return None
         flt = Q(project=mi) | Q(guest__partner=mi)
-        qs = self.model.objects.filter(flt).distinct()
+        qs = qs.filter(flt).distinct()
         # logger.info("20140314 %s", qs.query)
         return qs
 
     @classmethod
     def create_instance(cls, ar, **kw):
         mi = ar.master_instance
         if mi is not None:
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/cbss.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/cbss.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/cbss_demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/democfg.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/democfg.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/garble_tx25.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/purposes.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/purposes.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/sectors.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/sectors.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/mixins.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/tx25.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/ui.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cbss/utils.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cbss/utils.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/client_vouchers/ui.py` & `lino-welfare-24.5.0/lino_welfare/modlib/client_vouchers/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     date amount
     """
 
 
 class ClientVouchersByJournal(ByJournal, ClientVouchers):
     """Shows all simple invoices of a given journal (whose
     :attr:`Journal.voucher_type` must be
-    :class:`lino_xl.lib.sales.models.ClientVoucher`).
+    :class:`lino_xl.lib.trading.models.ClientVoucher`).
 
     """
     params_layout = "project partner state year"
     column_names = "number date project amount user workflow_buttons *"
     insert_layout = """
     project
     date amount
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/contacts/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/contacts/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/contacts/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,18 @@
 
     class Meta(Person.Meta):
         verbose_name = _("Person")  # :doc:`/tickets/14`
         verbose_name_plural = _("Persons")  # :doc:`/tickets/14`
         #~ ordering = ['last_name','first_name']
         abstract = dd.is_abstract_model(__name__, 'Person')
 
-    @classmethod
-    def get_request_queryset(cls, *args, **kwargs):
-        qs = super().get_request_queryset(*args, **kwargs)
-        return qs.select_related('country', 'city')
+    # @classmethod
+    # def get_request_queryset(cls, *args, **kwargs):
+    #     qs = super().get_request_queryset(*args, **kwargs)
+    #     return qs.select_related('country', 'city')
 
     def get_print_language(self):
         "Used by DirectPrintAction"
         return self.language
 
     @classmethod
     def on_analyze(cls, site):
@@ -290,14 +290,19 @@
     class Meta(Company.Meta):
         # verbose_name = _("Organisation")
         # verbose_name_plural = _("Organisations")
         abstract = dd.is_abstract_model(__name__, 'Company')
 
     vat_id = models.CharField(_("VAT id"), max_length=200, blank=True)
 
+    if dd.is_installed("art60"):
+        job_provider = dd.ForeignKey('jobs.JobProvider', blank=True, null=True)
+    else:
+        job_provider = dd.DummyField()
+
     @classmethod
     def on_analyze(cls, site):
         #~ if cls.model is None:
         #~ raise Exception("%r.model is None" % cls)
         super().on_analyze(site)
         cls.declare_imported_fields(
             '''name vat_id prefix phone fax email activity''')
@@ -311,16 +316,16 @@
     overview:30 general2:45 general3:30
     contacts.RolesByCompany
     """, label=_("General"))
 
     general2 = """
     prefix:20 name:40
     type vat_id
-    client_contact_type
     url
+    client_contact_type job_provider
     """
 
     general3 = """
     email:40
     phone
     gsm
     fax
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cv/fixtures/props.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cv/fixtures/props.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/cv/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/cv/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/fields.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/fields.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/minimal.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/minimal.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/mixins.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/debts/ui.py` & `lino-welfare-24.5.0/lino_welfare/modlib/debts/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/mixins.py` & `lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/dupable_clients/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/dupable_clients/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/esf/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/esf/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/esf/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/esf/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html` & `lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html` & `lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html` & `lino-welfare-24.5.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/esf/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/esf/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/finan/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/finan/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/households/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/households/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/immersion/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/immersion/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/immersion/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/immersion/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/immersion/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/immersion/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/immersion/ui.py` & `lino-welfare-24.5.0/lino_welfare/modlib/immersion/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     user type start_date end_date observed_event
     company ending_success ending
     """
 
     @classmethod
     def get_request_queryset(cls, ar):
         qs = super(Contracts, cls).get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         if pv.company:
             qs = qs.filter(company=pv.company)
         return qs
 
 
 class ContractsByClient(Contracts):
     required_roles = dd.login_required((IntegUser, SocialCoordinator))
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/integ/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/integ/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/integ/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/integ/fixtures/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 cv = dd.resolve_app('cv')
 
 ONE_DAY = datetime.timedelta(days=1)
 
 
 def objects():
 
+    Company = rt.models.contacts.Company
+
     DSBE = rt.models.coachings.CoachingType.objects.get(
         id=isip.COACHINGTYPE_DSBE)
 
     # isip (VSE)
     ISIP_DURATIONS = Cycler(312, 480, 312, 480, 30)
 
     JOBS = Cycler(jobs.Job.objects.all())
 
     STUDY_TYPES = Cycler(cv.StudyType.objects.all())
 
-    COMPANIES = Cycler(rt.models.contacts.Company.objects.all()[:5])
+    COMPANIES = Cycler(Company.objects.all()[:5])
     if dd.get_plugin_setting('jobs', 'with_employer_model'):
         EMPLOYERS = Cycler(rt.models.jobs.Employer.objects.all()[:5])
     else:
         EMPLOYERS = Cycler(rt.models.jobs.JobProvider.objects.all()[:5])
     NORMAL_CONTRACT_ENDINGS = Cycler(
         isip.ContractEnding.objects.filter(needs_date_ended=False))
     PREMATURE_CONTRACT_ENDINGS = Cycler(
@@ -72,18 +74,18 @@
 
     def jobs_contract(**kw):
         kw.update(type=JOBS_CONTRACT_TYPES.pop(),
                   duration=JOBS_CONTRACT_DURATIONS.pop())
         if not 'type' in kw:
             raise Exception("20150711, %s" % kw)
         if dd.is_installed("art60"):
-            job = JOBS.pop()
             ctr = art60.Contract(**kw)
             ctr.full_clean()
             ctr.save()
+            job = JOBS.pop()
             cv = art60.Convention(contract=ctr, job=job)
             cv.full_clean()
             cv.save()
             return ctr
         else:
             kw.update(job=JOBS.pop())
             return jobs.Contract(**kw)
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/integ/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/integ/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/integ/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/integ/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,24 +125,24 @@
         # kw.update(only_primary=True)
         return kw
 
     @classmethod
     def get_request_queryset(self, ar):
         #~ ar.param_values.update(client_state = ClientStates.coached)
         qs = super(Clients, self).get_request_queryset(ar)
-        if ar.param_values.language:
-            qs = qs.filter(languageknowledge__language=ar.param_values.language
+        if (pv := ar.param_values) is None: return qs
+        if pv.language:
+            qs = qs.filter(languageknowledge__language=pv.language
                            ).distinct()
-        if ar.param_values.wanted_property:
-            qs = qs.filter(personproperty__property=ar.param_values.
-                           wanted_property).distinct()
+        if pv.wanted_property:
+            qs = qs.filter(personproperty__property=pv.wanted_property).distinct()
 
-        if ar.param_values.group:
-            qs = qs.filter(group=ar.param_values.group)
-        if ar.param_values.only_active:
+        if pv.group:
+            qs = qs.filter(group=pv.group)
+        if pv.only_active:
             qs = qs.filter(group__active=True)
         return qs
 
     @classmethod
     def get_title_tags(self, ar):
         for t in super(Clients, self).get_title_tags(ar):
             yield t
@@ -528,15 +528,15 @@
     help_text = _("""Nombre de PIIS actifs par
     type de formation et type de contrat.""")
     contracts_table = isip.Contracts
 
     @classmethod
     def get_request_queryset(cls, ar):
         #~ logger.info("20120608.get_request_queryset param_values = %r",ar.param_values)
-        qs = super(StudyTypesAndContracts, cls).get_request_queryset(ar)
+        qs = super().get_request_queryset(ar)
         qs = qs.annotate(count=models.Count('contract'))
         return qs.filter(count__gte=1)
         #~ return qs
 
     @dd.virtualfield(
         dd.ForeignKey('cv.StudyType'))  # , verbose_name=_("Description")))
     def description(self, obj, ar):
@@ -571,15 +571,15 @@
     organisation externe et type de contrat.""")
     contracts_table = isip.Contracts
     contract_types = isip.ContractType
     hide_zero_rows = True
 
     @classmethod
     def get_request_queryset(cls, ar):
-        qs = super(CompaniesAndContracts, cls).get_request_queryset(ar)
+        qs = super().get_request_queryset(ar)
         qs = qs.annotate(
             count=models.Count('isip_contractpartner_set_by_company'))
         return qs.filter(count__gte=1)
 
     @dd.virtualfield(dd.ForeignKey('contacts.Company'))
     def description(self, obj, ar):
         return obj
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/isip/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/isip/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/isip/config/isip/Contract/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/isip/mixins.py` & `lino-welfare-24.5.0/lino_welfare/modlib/isip/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,15 @@
         kw.update(start_date=dd.today())
         # kw.update(end_date=dd.today())
         return kw
 
     @classmethod
     def get_request_queryset(cls, ar):
         qs = super().get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         #~ logger.info("20120608.get_request_queryset param_values = %r", pv)
         if pv.user:
             qs = qs.filter(user=pv.user)
         if pv.user_asd:
             qs = qs.filter(user_asd=pv.user_asd)
         if pv.type:
             qs = qs.filter(type=pv.type)
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/isip/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/isip/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
     company:20 study_type:15 ending_success:20 ending
     """
 
     @classmethod
     def get_request_queryset(cls, ar):
         #~ logger.info("20120608.get_request_queryset param_values = %r",ar.param_values)
         qs = super(Contracts, cls).get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         if pv.company:
             qs = qs.filter(contractpartner__company=pv.company)
         if pv.study_type:
             qs = qs.filter(study_type=pv.study_type)
         return qs
 
     @classmethod
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/mixins.py` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         ordering = ['name']
 
     # ref = models.CharField(_("Reference"), max_length=20, blank=True)
 
 
 if not dd.is_installed("art60"):
 
+    # Remains here for backward compat. Still used in weleup.
+
     class Contract(ContractPartnerBase, ContractBase, JobSupplyment):
         """An **Art60§7 job supplyment** is a contract bla bla...
 
 .. attribute:: duration
 
     If :attr:`applies_from` and :attr:`duration` are set, then the
     default value for :attr:`applies_until` is computed assuming 26
@@ -234,15 +236,15 @@
     remark = dd.RichTextField(blank=True,
                               verbose_name=_("Remark"),
                               format='plain')
 
     def __str__(self):
         if self.name:
             return self.name
-        return u'%s @ %s' % (self.function, self.provider)
+        return '%s @ %s' % (self.function, self.provider)
 
 
 class Job(SectorFunction):
     """
     A **job** is a place where a Client can work.
 
     """
@@ -256,28 +258,40 @@
 
     name = models.CharField(max_length=100, verbose_name=_("Name"))
     type = dd.ForeignKey("jobs.JobType",
                          verbose_name=_("Job Type"),
                          blank=True,
                          null=True)
     provider = dd.ForeignKey('jobs.JobProvider', blank=True, null=True)
+    if dd.is_installed("art60"):
+        workplace = dd.ForeignKey("contacts.Company",
+            verbose_name=_("Workplace"),
+            related_name="art60_workplaces",
+            blank=True, null=True)
+    else:
+        workplace = dd.DummyField()
+
     contract_type = dd.ForeignKey('jobs.ContractType',
                                   verbose_name=_("Contract Type"),
                                   blank=True,
                                   null=True)
     hourly_rate = dd.PriceField(_("hourly rate"), blank=True, null=True)
     capacity = models.IntegerField(_("capacity"), default=1)
     remark = models.TextField(blank=True, verbose_name=_("Remark"))
 
     def __str__(self):
         if self.provider:
             return _('%(job)s at %(provider)s') % dict(
                 job=self.name, provider=self.provider.name)
         return self.name
 
+    @dd.chooser()
+    def workplace_choices(cls, provider):
+        return rt.models.contacts.Company.objects.filter(job_provider=provider)
+
     def unused_disabled_fields(self, ar):
         # disabled 20140519. must convert this to Certifiable
         if self.contract_set.filter(build_time__isnull=False).count():
             return set(('contract_type', 'provider'))
         return set()
 
     #~ @dd.chooser()
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/jobs/ui.py` & `lino-welfare-24.5.0/lino_welfare/modlib/jobs/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import pgettext_lazy as pgettext
 from django.utils.encoding import force_str
 
 from lino.api import dd, rt
 from lino import mixins
+from lino.core import constants
 
 from etgen.html import E
 from lino.utils.report import Report
 
 from lino_xl.lib.cv.mixins import SectorFunction
 
 from lino_xl.lib.coachings.utils import only_coached_on, has_contracts_filter
@@ -64,14 +65,19 @@
     - add a new tab `jobs`
     - add the UploadsByController panel
 
     """
 
     main = "general notes jobs"
 
+    general = dd.Panel("""
+    overview:30 general2:45 general3:30
+    contacts.RolesByCompany:30 jobs.WorkplacesByProvider:30
+    """, label=_("General"))
+
     general2 = """
     prefix:20 name:40
     type vat_id
     client_contact_type is_social
     url
     """
 
@@ -90,17 +96,43 @@
 
 class JobProviders(contacts.Companies, dd.Table):
     required_roles = dd.login_required(IntegUser)
     model = 'jobs.JobProvider'
     detail_layout = JobProviderDetail()
 
 
+if dd.is_installed("art60"):
+
+    class WorkplacesByProvider(contacts.Companies):
+        required_roles = dd.login_required(IntegUser)
+        master_key = "job_provider"
+        label = _("Workplaces")
+        column_names = "name_column:20 address_column phone * id"
+        display_mode = (
+            (None, constants.DISPLAY_MODE_SUMMARY),
+        )
+
+        @classmethod
+        def param_defaults(self, ar, **kw):
+            kw = super().param_defaults(ar, **kw)
+            kw['also_obsolete'] = True
+            return kw
+
+else:
+    class WorkplacesByProvider(dd.Dummy):
+        pass
+
 if dd.get_plugin_setting('jobs', 'with_employer_model'):
 
     class EmployerDetail(JobProviderDetail):
+        general = dd.Panel("""
+        overview:30 general2:45 general3:30
+        contacts.RolesByCompany:30
+        """, label=_("General"))
+
         jobs = dd.Panel("""
         art61.ContractsByProvider
         """,
                         label=_("Jobs"))
 
     class Employers(contacts.Companies, dd.Table):
         required_roles = dd.login_required(IntegUser)
@@ -177,15 +209,15 @@
     user type start_date end_date observed_event
     company ending_success ending
     """
 
         @classmethod
         def get_request_queryset(cls, ar):
             qs = super(Contracts, cls).get_request_queryset(ar)
-            pv = ar.param_values
+            if (pv := ar.param_values) is None: return qs
             if pv.company:
                 qs = qs.filter(company=pv.company)
             return qs
 
     class ContractsByClient(Contracts):
         """Shows the *Art60§7 job supplyments* for this client.
     """
@@ -369,15 +401,16 @@
 class Jobs(dd.Table):
     model = 'jobs.Job'
     required_roles = dd.login_required(IntegUser)
     #~ order_by = ['start_date']
     column_names = 'name provider * id'
 
     detail_layout = """
-    name provider contract_type type id
+    name provider workplace
+    contract_type type id
     sector function capacity hourly_rate
     remark CandidaturesByJob
     ContractsByJob
     """
     insert_layout = """
     name provider
     contract_type type
@@ -394,14 +427,15 @@
     id name is_social
     JobsByType
     """
 
 
 class JobsByProvider(Jobs):
     master_key = 'provider'
+    column_names = 'name type workplace * id'
 
 
 class JobsByType(Jobs):
     master_key = 'type'
 
 
 class JobsOverviewByType(Jobs):
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/ledger/fixtures/std_journals.py` & `lino-welfare-24.5.0/lino_welfare/modlib/ledger/fixtures/std_journals.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/ledger/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/ledger/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/newcomers/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/newcomers/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/newcomers/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/newcomers/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/newcomers/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/newcomers/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,15 +238,16 @@
         kw.update(client_state=ClientStates.newcomer)
         # kw.update(new_since=amonthago())
         return kw
 
     @classmethod
     def get_request_queryset(self, ar):
         qs = super(NewClients, self).get_request_queryset(ar)
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
+        if (pv := ar.param_values) is None: return qs
         if pv.new_since:
             qs = qs.filter(coachings_by_client__start_date__gte=pv.new_since)
         return qs
 
     @classmethod
     def get_title_tags(self, ar):
         for t in super(NewClients, self).get_title_tags(ar):
@@ -289,16 +290,15 @@
         return NewClients.request().data_iterator
 
     @classmethod
     def get_request_queryset(self, ar):
         user_types = [
             p for p in UserTypes.items() if isinstance(p.role, SocialUser)
         ]
-        return super(AvailableCoaches, self,
-                     ar).filter(models.Q(user_type__in=user_types))
+        return super().get_request_queryset(ar).filter(models.Q(user_type__in=user_types))
 
     @classmethod
     def get_data_rows(self, ar):
         client = ar.param_values.for_client
         if client:
             # if client.client_state != ClientStates.newcomer:
             #     raise Warning(_("Only for newcomers"))
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/notes/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/notes/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/notes/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/notes/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/actions.py` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/actions.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/choicelists.py` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/fixtures/demo2.py` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/pcsw/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/pcsw/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,15 @@
         - some explicit date range is specified
         - `observed_event` is set to "active" (which means "All those
           who have some active coaching".
 
         """
         qs = super().get_request_queryset(ar)
 
-        pv = ar.param_values
+        if (pv := ar.param_values) is None: return qs
         period = [pv.start_date, pv.end_date]
         if period[0] is None:
             period[0] = period[1] or dd.today()
         if period[1] is None:
             period[1] = period[0]
 
         ce = pv.observed_event
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/polls/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/polls/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/projects/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/projects/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/projects/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/reception/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/reception/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/reception/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/reception/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/sepa/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/sepa/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/sepa/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/sepa/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/system/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/system/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/users/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/users/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/users/ui.py` & `lino-welfare-24.5.0/lino_welfare/modlib/users/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/excerpts/base.body.html` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/letter_margin_bottom.html` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -709,16 +709,16 @@
         country='BE',
         gender=dd.Genders.male)
     yield gerd
     yield role(company=cpas, person=gerd, type=4)
 
     # see :blogentry:`20111007`
     tatjana = client(
-        first_name=u"Tatjana",
-        last_name=u"Kasennova",
+        first_name="Tatjana",
+        last_name="Kasennova",
         #~ first_name=u"Татьяна",last_name=u"Казеннова",
         city=kettenis,
         country='BE',
         #~ national_id='1237',
         birth_place="Moskau",  # birth_country='SUHH',
         client_state=ClientStates.newcomer,
         #~ newcomer=True,
@@ -894,15 +894,15 @@
     for i in range(10):
         yield Note(user=USERS.pop(),
                    date=settings.SITE.demo_date(days=i),
                    subject=SUBJECTS.pop())
 
     schule = StudyType.objects.get(pk=1)
     # uni = StudyType.objects.get(pk=4)
-    abi = u"Abitur"
+    abi = "Abitur"
     study = Instantiator('cv.Study').build
 
     gerd = CLIENTS.pop()
     luc = CLIENTS.pop()
     ly = CLIENTS.pop()
     mari = CLIENTS.pop()
     iiris = CLIENTS.pop()
@@ -951,29 +951,35 @@
 
     yield langk(person=luc, language='est', written='3', spoken='3')
     yield langk(person=ly, language='est', written='4', spoken='4')
     yield langk(person=mari, language='est', written='3', spoken='4')
     yield langk(person=iiris, language='est', written='0', spoken='3')
 
     jobtype = Instantiator(jobs.JobType, 'name').build
-    art607 = jobtype(u'Sozialwirtschaft = "majorés"')
+    art607 = jobtype('Sozialwirtschaft = "majorés"')
     yield art607
     yield jobtype('Intern')
     yield jobtype('Extern (Öffentl. VoE mit Kostenrückerstattung)')
     yield jobtype('Extern (Privat Kostenrückerstattung)')
     #~ yield jobtype(u'VSE')
     yield jobtype('Sonstige')
 
     rcycle = mti.insert_child(rcycle, jobs.JobProvider)
     yield rcycle
     bisa = mti.insert_child(bisa, jobs.JobProvider)
     yield bisa
     proaktiv = mti.insert_child(proaktiv, jobs.JobProvider)
     yield proaktiv
 
+    if dd.is_installed("art60"):
+        kw = dict(job_provider=proaktiv, country=belgium, city=eupen)
+        yield Company(name="Pro Aktiv Unterstadt", **kw)
+        yield Company(name="Pro Aktiv Noereth", **kw)
+        yield Company(name="Pro Aktiv Nispert", **kw)
+
     if dd.get_plugin_setting('jobs', 'with_employer_model'):
         cardijn = mti.insert_child(cardijn, jobs.Employer)
         yield cardijn
         bwe = mti.insert_child(bwe, jobs.Employer)
         yield bwe
 
     # jobs (Art.60-7)
@@ -983,24 +989,36 @@
 
     PROVIDERS = Cycler(jobs.JobProvider.objects.all())
     SECTORS = Cycler(cv.Sector.objects.all())
     FUNCTIONS = Cycler(cv.Function.objects.all())
     REMARKS = Cycler(_("A very hard job."), '',
                      _("No supervisor. Only for independent people."), '', '',
                      '')
+    WORKPLACES = {}  # maps job provider to cycler on workplaces
 
     for i in range(8):
         f = FUNCTIONS.pop()
-        yield jobs.Job(provider=PROVIDERS.pop(),
-                       type=JTYPES.pop(),
-                       contract_type=JOBS_CONTRACT_TYPES.pop(),
-                       name=str(f),
-                       remark=REMARKS.pop(),
-                       sector=SECTORS.pop(),
-                       function=f)
+        p = PROVIDERS.pop()
+
+        kw = dict(provider=p,
+            type=JTYPES.pop(),
+            contract_type=JOBS_CONTRACT_TYPES.pop(),
+            name=str(f),
+            remark=REMARKS.pop(),
+            sector=SECTORS.pop(),
+            function=f)
+
+        if dd.is_installed("art60"):
+            workplaces = WORKPLACES.get(p, None)
+            if workplaces is None:
+                workplaces = Cycler(Company.objects.filter(job_provider=p))
+            WORKPLACES[p] = workplaces
+            kw.update(workplace=workplaces.pop())
+
+        yield jobs.Job(**kw)
 
     JOBS = Cycler(jobs.Job.objects.all())
 
     for i in range(40):
         yield jobs.Candidature(job=JOBS.pop(),
                                person=CLIENTS.pop(),
                                state=CSTATES.pop(),
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/demo2.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/pp2lino.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/std.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/fixtures/std2.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/fixtures/std2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/help_texts.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/help_texts.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,27 +79,35 @@
     'lino_welfare.modlib.aids.Granting.category' : _("""Currently only used for printing an isip.Contract."""),
     'lino_welfare.modlib.aids.Confirmation' : _("""Base class for all aid confirmations."""),
     'lino_welfare.modlib.aids.Confirmation.get_date_range_veto' : _("""Return an error message if this confirmation lies outside of granted period."""),
     'lino_welfare.modlib.aids.Confirmable' : _("""Base class for both Granting and Confirmation."""),
     'lino_welfare.modlib.aids.Confirmable.state' : _("""The confirmation state of this object. Pointer to ConfirmationStates."""),
     'lino_welfare.modlib.aids.Confirmable.sign' : _("""Sign this granting or confirmation, making most fields read-only."""),
     'lino_welfare.modlib.aids.Confirmable.revoke' : _("""Revoke your signature of this granting or confirmation."""),
+    'lino_welfare.modlib.art61.Contract' : _("""The database model used to represent an article 61 job supplyment."""),
+    'lino_welfare.modlib.art61.Contract.get_subsidizations' : _("""Yield a list of all subsidizations activated for this contract."""),
+    'lino_welfare.modlib.art61.ContractsByClient' : _("""Shows the Art61 job supplyments for this client."""),
+    'lino_welfare.modlib.art61.ContractType' : _("""This is the homologue of isip.ContractType (see there for general documentation)."""),
+    'lino_welfare.modlib.art61.Activation.company' : _("""The employer or job provider."""),
+    'lino_welfare.modlib.art61.Subsidizations' : _("""The choicelist with available subsidization formulas."""),
     'lino_welfare.modlib.cal.EventType' : _("""Adds two fields."""),
     'lino_welfare.modlib.cal.EventType.esf_field' : _("""How to summarize entries of this type in the ESF summary."""),
     'lino_welfare.modlib.cal.Guest' : _("""Adds a virtual field client."""),
     'lino_welfare.modlib.cal.Guest.client' : _("""Virtual field which returns the partner if it is a client."""),
+    'lino_welfare.modlib.cal.EntriesByClient' : _("""Shows calendar entries having either project or one guest pointing to this client."""),
     'lino_welfare.modlib.cbss.Sector' : _("""Default values filled from lino_welfare.modlib.cbss.fixtures.sectors."""),
     'lino_welfare.modlib.cbss.Purpose' : _("""Codes qualité (Hoedanigheidscodes). This table is usually filled with the official codes by lino_welfare.modlib.cbss.fixtures.purposes."""),
     'lino_welfare.modlib.cbss.IdentifyPersonRequest' : _("""A request to the IdentifyPerson service."""),
     'lino_welfare.modlib.cbss.ManageAccessRequest' : _("""A request to the ManageAccess service."""),
     'lino_welfare.modlib.cbss.ManageAccessRequest.sector' : _("""Pointer to Sector."""),
     'lino_welfare.modlib.cbss.ManageAccessRequest.purpose' : _("""Pointer to Purpose."""),
     'lino_welfare.modlib.cbss.ManageAccessRequest.action' : _("""The action to perform. This must be one of the values in lino_welfare.modlib.cbss.choicelists.ManageActions"""),
     'lino_welfare.modlib.cbss.ManageAccessRequest.query_register' : _("""The register to be query. This must be one of the values in lino_welfare.modlib.cbss.choicelists.QueryRegisters"""),
     'lino_welfare.modlib.cbss.RetrieveTIGroupsRequest' : _("""A request to the RetrieveTIGroups service (aka Tx25)"""),
+    'lino_welfare.modlib.contacts.Company.job_provider' : _("""The job provider for whom this company acts as a workplace."""),
     'lino_welfare.modlib.debts.Budget.print_empty_rows' : _("""Whether to print empty rows."""),
     'lino_welfare.modlib.debts.Budget.ignore_yearly_incomes' : _("""Whether to ignore yearly incomes."""),
     'lino_welfare.modlib.debts.Budget.entry_groups' : _("""Yield the entry groups for this budget, i.e. one item for each account group for which this budget has some data."""),
     'lino_welfare.modlib.debts.Actor' : _("""The database model used to represent a budget actor."""),
     'lino_welfare.modlib.debts.Entry' : _("""A detail row of a Budget."""),
     'lino_welfare.modlib.debts.Entry.actor' : _("""Optionally specify a budget actor who contributes this entry. Leave empty when the entry refers to the entire household."""),
     'lino_welfare.modlib.debts.Entry.amount' : _("""The amount of money. An empty amount is different from a zero amount in that the latter will be printed while the former not."""),
@@ -170,15 +178,21 @@
     'lino_welfare.modlib.isip.ContractTypeBase.full_name' : _("""The full description of this contract type as used in printed documents."""),
     'lino_welfare.modlib.isip.ContractTypeBase.exam_policy' : _("""The default examination policy to be used for contracts of this type."""),
     'lino_welfare.modlib.isip.ContractTypeBase.overlap_group' : _("""The overlap group to use when checking whether two contracts are overlapping or not. If this field is empty, Lino does not check at all for overlapping contracts."""),
     'lino_welfare.modlib.isip.ContractTypeBase.template' : _("""The main template to use instead of the default template defined on the excerpt type."""),
     'lino_welfare.modlib.isip.OverlapGroups' : _("""The list of all known overlap groups to be selected for the overlap_group of a contract type."""),
     'lino_welfare.modlib.isip.OverlappingContractsTest' : _("""Volatile object used to test for overlapping contracts. It is responsible for issuing the following error messages:"""),
     'lino_welfare.modlib.isip.OverlappingContractsChecker' : _("""A given client cannot have two active contracts at the same time."""),
-    'lino_welfare.modlib.jobs.JobProvider.is_social' : _("""Organisation bénéficiant de l’agrément « Initiative d’économie sociale » octroyé par la Wallonie."""),
+    'lino_welfare.modlib.jobs.Job.provider' : _("""The job provider for this job."""),
+    'lino_welfare.modlib.jobs.Job.workplace' : _("""The workplace for this job if the job provider has multiple workplaces. See art60_workplace."""),
+    'lino_welfare.modlib.jobs.JobProvider' : _("""Database model used to represent a job provider."""),
+    'lino_welfare.modlib.jobs.JobProvider.is_social' : _("""Whether this is a recognized social economy project."""),
+    'lino_welfare.modlib.jobs.WorkplacesByProvider' : _("""Shows the companies that act as workplaces for this job provider."""),
+    'lino_welfare.modlib.jobs.Employer' : _("""Database model used to represent an employer."""),
+    'lino_welfare.modlib.jobs.Employer.is_social' : _("""Whether this is a recognized social economy project."""),
     'lino_welfare.modlib.jobs.Contracts' : _("""Shows all Art60 job supplyments."""),
     'lino_welfare.modlib.jobs.ContractsByClient' : _("""Shows the Art60 job supplyments for this client."""),
     'lino_welfare.modlib.jobs.JobSupplyment' : _("""Model mixin for jobs.Contract and art61.Contract. And also for art60.Contract."""),
     'lino_welfare.modlib.jobs.JobSupplyment.duration' : _("""The duration of this job supplyment (number of working days)."""),
     'lino_welfare.modlib.pcsw.Client' : _("""Django model used to represent a beneficiary."""),
     'lino_welfare.modlib.pcsw.Client.has_esf' : _("""Whether Lino should make ESF summaries for this client."""),
     'lino_welfare.modlib.pcsw.Client.overview' : _("""A panel with general information about this client."""),
@@ -189,11 +203,8 @@
     'lino_welfare.modlib.pcsw.Client.client_state' : _("""Pointer to ClientStates."""),
     'lino_welfare.modlib.pcsw.Client.unemployed_since' : _("""The date when this client got unemployed and stopped to have a regular work."""),
     'lino_welfare.modlib.pcsw.Client.seeking_since' : _("""The date when this client registered as unemployed and started to look for a new job."""),
     'lino_welfare.modlib.pcsw.Client.get_first_meeting' : _("""Return the last note of type “First meeting” for this client. Usage example see debts and notes."""),
     'lino_welfare.modlib.pcsw.Clients' : _("""The list that opens by Contacts ‣ Clients."""),
     'lino_welfare.modlib.pcsw.Clients.client_state' : _("""If not empty, show only Clients whose client_state equals the specified value."""),
     'lino_welfare.modlib.cbss.tx25.RetrieveTIGroupsResult' : _("""Displays the response of an RetrieveTIGroupsRequest as a table."""),
-    'lino_welfare.modlib.art61.Contract' : _("""The Django database model."""),
-    'lino_welfare.modlib.art61.Contract.get_subsidizations' : _("""Yield a list of all subsidizations activated for this contract."""),
-    'lino_welfare.modlib.art61.ContractsByClient' : _("""Shows the Art61 job supplyments for this client."""),
 }
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Lino-DSBE\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-02-20 10:34+0200\n"
+"PO-Revision-Date: 2024-04-08 13:14+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
 "Language-Team: de <luc.saffre@gmail.com>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 # Copyright (C) 2016 ORGANIZATION
 # This file is distributed under the same license as the lino-welfare
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Lino-DSBE\n"
+"Project-Id-Version:  Lino-DSBE\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-02-20 10:31+0200\n"
-"PO-Revision-Date: 2024-02-20 10:34+0200\n"
+"POT-Creation-Date: 2024-04-30 13:49+0300\n"
+"PO-Revision-Date: 2024-04-08 13:14+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
-"Language-Team: de <luc.saffre@gmail.com>\n"
 "Language: de\n"
+"Language-Team: de <luc.saffre@gmail.com>\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Generated-By: Babel 2.12.1\n"
-"X-Generator: Poedit 3.0.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:18
 #, fuzzy
 msgid "Active Job Search"
 msgstr "Arbeitssuche"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:19
@@ -37,21 +36,21 @@
 
 #: lino_welfare/modlib/active_job_search/models.py:23
 #, fuzzy
 msgid "Proofs of search"
 msgstr "Arbeitssuche"
 
 #: lino_welfare/modlib/active_job_search/models.py:27
-#: lino_welfare/modlib/badges/models.py:38 lino_welfare/modlib/cal/models.py:348
-#: lino_welfare/modlib/cbss/tx25.py:315 lino_welfare/modlib/cbss/tx25.py:362
-#: lino_welfare/modlib/cbss/tx25.py:371 lino_welfare/modlib/cbss/tx25.py:383
-#: lino_welfare/modlib/cbss/tx25.py:476 lino_welfare/modlib/cbss/tx25.py:488
-#: lino_welfare/modlib/debts/models.py:104 lino_welfare/modlib/isip/models.py:376
-#: lino_welfare/modlib/jobs/ui.py:416 lino_welfare/modlib/jobs/ui.py:536
-#: lino_welfare/modlib/pcsw/models.py:1046
+#: lino_welfare/modlib/badges/models.py:38
+#: lino_welfare/modlib/cal/models.py:347 lino_welfare/modlib/cbss/tx25.py:315
+#: lino_welfare/modlib/cbss/tx25.py:362 lino_welfare/modlib/cbss/tx25.py:371
+#: lino_welfare/modlib/cbss/tx25.py:383 lino_welfare/modlib/cbss/tx25.py:476
+#: lino_welfare/modlib/cbss/tx25.py:488 lino_welfare/modlib/debts/models.py:104
+#: lino_welfare/modlib/isip/models.py:376 lino_welfare/modlib/jobs/ui.py:430
+#: lino_welfare/modlib/jobs/ui.py:550 lino_welfare/modlib/pcsw/models.py:1048
 msgid "Date"
 msgstr "Datum"
 
 #: lino_welfare/modlib/active_job_search/models.py:29
 #, fuzzy
 msgid "Spontaneous"
 msgstr "Kontakte"
@@ -77,16 +76,17 @@
 msgid "Child custody"
 msgstr ""
 
 #: lino_welfare/modlib/active_job_search/models.py:76
 msgid "Notes concerning child custody."
 msgstr ""
 
-#: lino_welfare/modlib/aids/__init__.py:13 lino_welfare/modlib/ledger/models.py:49
-#: lino_welfare/modlib/pcsw/models.py:531
+#: lino_welfare/modlib/aids/__init__.py:13
+#: lino_welfare/modlib/ledger/models.py:49
+#: lino_welfare/modlib/pcsw/models.py:533
 msgid "Aids"
 msgstr "Hilfen"
 
 #: lino_welfare/modlib/aids/choicelists.py:47
 msgid "Aid confirmation type"
 msgstr "Hilfebescheinigungsart"
 
@@ -148,50 +148,58 @@
 msgstr "Entstätigen"
 
 #: lino_welfare/modlib/aids/mixins.py:104
 #, python-format
 msgid "You revoke your confirmation that %(client)s %(text)s"
 msgstr "Sie annulieren Ihre Bestätigung, dass %(client)s %(text)s"
 
-#: lino_welfare/modlib/aids/mixins.py:118 lino_welfare/modlib/aids/mixins.py:143
+#: lino_welfare/modlib/aids/mixins.py:118
+#: lino_welfare/modlib/aids/mixins.py:143
 msgctxt "aids"
 msgid "Signer"
 msgstr "Bestätiger"
 
 #: lino_welfare/modlib/aids/mixins.py:188
 #, python-format
 msgid "receives %(what)s %(when)s."
 msgstr "%(when)s %(what)s erhält."
 
-#: lino_welfare/modlib/aids/mixins.py:217 lino_welfare/modlib/art61/models.py:248
+#: lino_welfare/modlib/aids/mixins.py:217
+#: lino_welfare/modlib/art61/models.py:248
 #: lino_welfare/modlib/badges/models.py:40 lino_welfare/modlib/cv/models.py:46
-#: lino_welfare/modlib/debts/models.py:399 lino_welfare/modlib/debts/models.py:435
-#: lino_welfare/modlib/esf/models.py:37
+#: lino_welfare/modlib/debts/models.py:399
+#: lino_welfare/modlib/debts/models.py:435 lino_welfare/modlib/esf/models.py:37
 #: lino_welfare/modlib/immersion/models.py:102
-#: lino_welfare/modlib/jobs/mixins.py:45 lino_welfare/modlib/jobs/models.py:235
-#: lino_welfare/modlib/jobs/models.py:269 lino_welfare/modlib/jobs/models.py:336
-#: lino_welfare/modlib/jobs/models.py:409 lino_welfare/modlib/pcsw/actions.py:39
-#: lino_welfare/modlib/pcsw/models.py:952 lino_welfare/modlib/pcsw/models.py:1012
+#: lino_welfare/modlib/jobs/mixins.py:45 lino_welfare/modlib/jobs/models.py:237
+#: lino_welfare/modlib/jobs/models.py:279
+#: lino_welfare/modlib/jobs/models.py:350
+#: lino_welfare/modlib/jobs/models.py:423
+#: lino_welfare/modlib/pcsw/actions.py:39
+#: lino_welfare/modlib/pcsw/models.py:954
+#: lino_welfare/modlib/pcsw/models.py:1014
 #: lino_welfare/modlib/projects/models.py:40
 #: lino_welfare/modlib/xcourses/models.py:177
 #: lino_welfare/modlib/xcourses/models.py:354
 msgid "Remark"
 msgstr "Bemerkung"
 
 #: lino_welfare/modlib/aids/mixins.py:249
 #, python-format
 msgid "Date range %(p1)s lies outside of granted period %(p2)s."
 msgstr "Datumsbereich %(p1)s außerhalb der Laufzeit des Beschlusses %(p2)s."
 
-#: lino_welfare/modlib/aids/mixins.py:322 lino_welfare/modlib/cbss/models.py:283
+#: lino_welfare/modlib/aids/mixins.py:322
+#: lino_welfare/modlib/cbss/models.py:283
 msgid "Period from"
 msgstr "Periode vom"
 
-#: lino_welfare/modlib/aids/mixins.py:326 lino_welfare/modlib/aids/models.py:221
-#: lino_welfare/modlib/pcsw/models.py:956 lino_welfare/modlib/pcsw/models.py:1011
+#: lino_welfare/modlib/aids/mixins.py:326
+#: lino_welfare/modlib/aids/models.py:221
+#: lino_welfare/modlib/pcsw/models.py:958
+#: lino_welfare/modlib/pcsw/models.py:1013
 msgid "until"
 msgstr "bis"
 
 #: lino_welfare/modlib/aids/mixins.py:330
 msgid "Recipient (Organization)"
 msgstr "Empfänger (Organisation)"
 
@@ -229,16 +237,16 @@
 
 #: lino_welfare/modlib/aids/models.py:71
 msgid "Integration duty"
 msgstr "Verpflichtung DSBE"
 
 #: lino_welfare/modlib/aids/models.py:73
 msgid ""
-"Whether aid grantings of this type are considered as duty for integration "
-"contract."
+"Whether aid grantings of this type are considered as duty for integration"
+" contract."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:77
 msgid "Urgent"
 msgstr "Dringend"
 
 #: lino_welfare/modlib/aids/models.py:79
@@ -247,22 +255,22 @@
 
 #: lino_welfare/modlib/aids/models.py:83
 msgid "Confirmed by primary coach"
 msgstr "Primärbegleiter bestätigt"
 
 #: lino_welfare/modlib/aids/models.py:86
 msgid ""
-"Whether grantings for this aid type are to be signed by the client's primary "
-"coach."
+"Whether grantings for this aid type are to be signed by the client's "
+"primary coach."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:96
 msgid ""
-"Which client address to print on confirmations. If this is empty, Lino will use "
-"the primary address."
+"Which client address to print on confirmations. If this is empty, Lino "
+"will use the primary address."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:101
 msgid "Body template"
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:157
@@ -287,19 +295,21 @@
 msgid "Create confirmation"
 msgstr "Bescheinigung ausstellen"
 
 #: lino_welfare/modlib/aids/models.py:217
 msgid "Applies from"
 msgstr "Laufzeit von"
 
-#: lino_welfare/modlib/aids/models.py:248 lino_welfare/modlib/aids/models.py:371
+#: lino_welfare/modlib/aids/models.py:248
+#: lino_welfare/modlib/aids/models.py:371
 msgid "Only rows decided by this board."
 msgstr ""
 
-#: lino_welfare/modlib/aids/models.py:253 lino_welfare/modlib/aids/models.py:381
+#: lino_welfare/modlib/aids/models.py:253
+#: lino_welfare/modlib/aids/models.py:381
 msgid "Only confirmations about this aid type."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:310
 msgid "Grantings to confirm"
 msgstr "Zu bestätigende Hilfebeschlüsse"
 
@@ -343,29 +353,31 @@
 #: lino_welfare/modlib/aids/models.py:609
 msgid "Income confirmations"
 msgstr "Einkommensbescheinigungen"
 
 #: lino_welfare/modlib/aids/models.py:613
 #: lino_welfare/modlib/client_vouchers/models.py:36
 #: lino_welfare/modlib/client_vouchers/models.py:110
-#: lino_welfare/modlib/debts/models.py:155 lino_welfare/modlib/debts/models.py:423
-#: lino_welfare/modlib/debts/ui.py:487 lino_welfare/modlib/debts/ui.py:491
-#: lino_welfare/modlib/debts/ui.py:495 lino_welfare/modlib/debts/ui.py:499
-#: lino_welfare/modlib/debts/ui.py:503 lino_welfare/modlib/debts/ui.py:523
+#: lino_welfare/modlib/debts/models.py:155
+#: lino_welfare/modlib/debts/models.py:423 lino_welfare/modlib/debts/ui.py:487
+#: lino_welfare/modlib/debts/ui.py:491 lino_welfare/modlib/debts/ui.py:495
+#: lino_welfare/modlib/debts/ui.py:499 lino_welfare/modlib/debts/ui.py:503
+#: lino_welfare/modlib/debts/ui.py:523
 #: lino_welfare/modlib/households/models.py:73
 msgid "Amount"
 msgstr "Betrag"
 
 #: lino_welfare/modlib/aids/models.py:681
 msgid "Can refund"
 msgstr "Kostenrückerstattung"
 
 #: lino_welfare/modlib/aids/models.py:683
 msgid ""
-"Whether persons of this type can be used as doctor of a refund confirmation."
+"Whether persons of this type can be used as doctor of a refund "
+"confirmation."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:719
 msgid "Refund confirmation"
 msgstr "Kostenübernahmeschein"
 
 #: lino_welfare/modlib/aids/models.py:720
@@ -444,25 +456,27 @@
 msgstr "Art.61-Konvention"
 
 #: lino_welfare/modlib/art60/models.py:33
 #, fuzzy
 msgid "Art60 job supplyment"
 msgstr "Art.60§7-Konvention"
 
-#: lino_welfare/modlib/art60/models.py:48 lino_welfare/modlib/jobs/models.py:116
-#: lino_welfare/modlib/jobs/ui.py:37
+#: lino_welfare/modlib/art60/models.py:48
+#: lino_welfare/modlib/jobs/models.py:118 lino_welfare/modlib/jobs/ui.py:37
 msgid "Art60§7 job supplyment"
 msgstr "Art.60§7-Konvention"
 
-#: lino_welfare/modlib/art60/models.py:49 lino_welfare/modlib/jobs/models.py:117
+#: lino_welfare/modlib/art60/models.py:49
+#: lino_welfare/modlib/jobs/models.py:119
 msgid "Art60§7 job supplyments"
 msgstr "Art.60§7-Konventionen"
 
-#: lino_welfare/modlib/art60/models.py:55 lino_welfare/modlib/art61/models.py:76
-#: lino_welfare/modlib/jobs/models.py:131
+#: lino_welfare/modlib/art60/models.py:55
+#: lino_welfare/modlib/art61/models.py:76
+#: lino_welfare/modlib/jobs/models.py:133
 #, fuzzy
 msgid "Type"
 msgstr "Typ "
 
 #: lino_welfare/modlib/art60/models.py:85
 #, fuzzy
 msgid "Active convention"
@@ -479,40 +493,46 @@
 msgstr "Vorstrafen"
 
 #: lino_welfare/modlib/art60/models.py:114
 #, fuzzy
 msgid "Start date"
 msgstr "Beginndatum"
 
-#: lino_welfare/modlib/art60/models.py:120 lino_welfare/modlib/art60/models.py:237
+#: lino_welfare/modlib/art60/models.py:120
+#: lino_welfare/modlib/art60/models.py:237
 #, fuzzy
 msgid "Monthly refund"
 msgstr "Monatsrate"
 
-#: lino_welfare/modlib/art60/models.py:121 lino_welfare/modlib/jobs/models.py:141
-#: lino_welfare/modlib/jobs/models.py:267
+#: lino_welfare/modlib/art60/models.py:121
+#: lino_welfare/modlib/jobs/models.py:143
+#: lino_welfare/modlib/jobs/models.py:277
 msgid "hourly rate"
 msgstr "Stundensatz"
 
-#: lino_welfare/modlib/art60/models.py:122 lino_welfare/modlib/jobs/models.py:142
+#: lino_welfare/modlib/art60/models.py:122
+#: lino_welfare/modlib/jobs/models.py:144
 msgid "refund rate"
 msgstr "Rückzahlung"
 
-#: lino_welfare/modlib/art60/models.py:175 lino_welfare/modlib/jobs/models.py:186
+#: lino_welfare/modlib/art60/models.py:175
+#: lino_welfare/modlib/jobs/models.py:188
 #, python-format
 msgid "(%d candidatures have been marked inactive)"
 msgstr "( %d Kandidaturen wurden als inaktiv markiert)"
 
-#: lino_welfare/modlib/art60/models.py:177 lino_welfare/modlib/isip/models.py:117
-#: lino_welfare/modlib/jobs/models.py:188 lino_welfare/modlib/pcsw/actions.py:85
+#: lino_welfare/modlib/art60/models.py:177
+#: lino_welfare/modlib/isip/models.py:117
+#: lino_welfare/modlib/jobs/models.py:190
+#: lino_welfare/modlib/pcsw/actions.py:85
 #: lino_welfare/modlib/pcsw/actions.py:118
 msgid "Success"
 msgstr "Abschluss"
 
-#: lino_welfare/modlib/art60/models.py:241 lino_welfare/modlib/jobs/ui.py:173
+#: lino_welfare/modlib/art60/models.py:241 lino_welfare/modlib/jobs/ui.py:185
 msgid "Only contracts of type"
 msgstr "Vertragsart"
 
 #: lino_welfare/modlib/art60/models.py:297
 #: lino_welfare/modlib/isip/choicelists.py:27
 msgid "Conventions"
 msgstr "Vorstrafen"
@@ -556,15 +576,16 @@
 msgid "Tutorate"
 msgstr ""
 
 #: lino_welfare/modlib/art61/choicelists.py:48
 msgid "Walloon Region"
 msgstr ""
 
-#: lino_welfare/modlib/art61/models.py:29 lino_welfare/modlib/art61/models.py:66
+#: lino_welfare/modlib/art61/models.py:29
+#: lino_welfare/modlib/art61/models.py:66
 msgid "Art61 job supplyment"
 msgstr "Art.61-Konvention"
 
 #: lino_welfare/modlib/art61/models.py:47
 msgid "Art61 job supplyment type"
 msgstr "Art.61-Konventionsart"
 
@@ -621,20 +642,22 @@
 msgid "Badge Awards"
 msgstr "Badgeprüfungen"
 
 #: lino_welfare/modlib/badges/models.py:36
 msgid "Holder"
 msgstr ""
 
-#: lino_welfare/modlib/badges/models.py:39 lino_welfare/modlib/cbss/mixins.py:282
+#: lino_welfare/modlib/badges/models.py:39
+#: lino_welfare/modlib/cbss/mixins.py:282
 #: lino_welfare/modlib/projects/models.py:41
 msgid "Result"
 msgstr "Resultat"
 
-#: lino_welfare/modlib/badges/models.py:49 lino_welfare/modlib/badges/models.py:57
+#: lino_welfare/modlib/badges/models.py:49
+#: lino_welfare/modlib/badges/models.py:57
 msgid "Awards"
 msgstr "Badgeprüfungen"
 
 #: lino_welfare/modlib/cal/models.py:33
 msgid "You are busy in "
 msgstr "Du bist beschäftigt in "
 
@@ -692,62 +715,64 @@
 msgid "at"
 msgstr "um"
 
 #: lino_welfare/modlib/cal/models.py:186
 msgid "Managed by"
 msgstr "Verwaltet durch"
 
-#: lino_welfare/modlib/cal/models.py:241
+#: lino_welfare/modlib/cal/models.py:240
 #, fuzzy
 msgid "Notes"
 msgstr "Notiz"
 
-#: lino_welfare/modlib/cal/models.py:326
+#: lino_welfare/modlib/cal/models.py:325
 #: lino_welfare/modlib/client_vouchers/ui.py:38
 #: lino_welfare/modlib/contacts/models.py:139
 #: lino_welfare/modlib/contacts/models.py:227
-#: lino_welfare/modlib/contacts/models.py:313 lino_welfare/modlib/debts/ui.py:125
-#: lino_welfare/modlib/finan/models.py:19 lino_welfare/modlib/isip/models.py:263
+#: lino_welfare/modlib/contacts/models.py:318
+#: lino_welfare/modlib/debts/ui.py:125 lino_welfare/modlib/finan/models.py:19
+#: lino_welfare/modlib/isip/models.py:263 lino_welfare/modlib/jobs/ui.py:74
 #: lino_welfare/modlib/system/models.py:103 lino_welfare/modlib/users/ui.py:24
 #: lino_welfare/modlib/welfare/workflows.py:49
 msgid "General"
 msgstr "Allgemein"
 
-#: lino_welfare/modlib/cal/models.py:331 lino_welfare/modlib/finan/models.py:25
+#: lino_welfare/modlib/cal/models.py:330 lino_welfare/modlib/finan/models.py:25
 msgid "More"
 msgstr "Mehr"
 
-#: lino_welfare/modlib/cal/models.py:346
+#: lino_welfare/modlib/cal/models.py:345
 #: lino_welfare/modlib/integ/fixtures/std.py:30
 msgid "Appointment"
 msgstr "Termin"
 
-#: lino_welfare/modlib/cal/models.py:352
+#: lino_welfare/modlib/cal/models.py:351
 msgid "Summary"
 msgstr "Zusammenfassung"
 
-#: lino_welfare/modlib/cal/models.py:367
+#: lino_welfare/modlib/cal/models.py:366
 #, python-format
 msgid "Created appointment for %(user)s with %(partner)s"
 msgstr ""
 
-#: lino_welfare/modlib/cal/models.py:408
+#: lino_welfare/modlib/cal/models.py:407
 #, fuzzy
 msgid "Task"
 msgstr "Status"
 
-#: lino_welfare/modlib/cal/models.py:409
+#: lino_welfare/modlib/cal/models.py:408
 msgid "Tasks"
 msgstr ""
 
-#: lino_welfare/modlib/cal/models.py:412
+#: lino_welfare/modlib/cal/models.py:411
 msgid "Delegated to client"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/__init__.py:37 lino_welfare/modlib/pcsw/models.py:419
+#: lino_welfare/modlib/cbss/__init__.py:37
+#: lino_welfare/modlib/pcsw/models.py:421
 msgid "CBSS"
 msgstr "ZDSS"
 
 #: lino_welfare/modlib/cbss/choicelists.py:20
 #: lino_welfare/modlib/cbss/mixins.py:74
 msgid "Sent"
 msgstr "Abgeschickt"
@@ -937,15 +962,16 @@
 msgid "Tx25 Request"
 msgstr "Tx25-Anfrage"
 
 #: lino_welfare/modlib/cbss/models.py:410
 msgid "Tx25 Requests"
 msgstr "Tx25-Anfragen"
 
-#: lino_welfare/modlib/cbss/models.py:415 lino_welfare/modlib/pcsw/models.py:539
+#: lino_welfare/modlib/cbss/models.py:415
+#: lino_welfare/modlib/pcsw/models.py:541
 msgid "History"
 msgstr "Historie"
 
 #: lino_welfare/modlib/cbss/models.py:562
 msgid "Requesting organisation"
 msgstr "Anfragende Organisation"
 
@@ -1105,16 +1131,18 @@
 msgid "produced "
 msgstr "produziert"
 
 #: lino_welfare/modlib/cbss/tx25.py:710 lino_welfare/modlib/cbss/tx25.py:752
 msgid "SSIN "
 msgstr "NR-Nr. "
 
-#: lino_welfare/modlib/cbss/tx25.py:730 lino_welfare/modlib/immersion/models.py:86
-#: lino_welfare/modlib/isip/models.py:150 lino_welfare/modlib/jobs/models.py:125
+#: lino_welfare/modlib/cbss/tx25.py:730
+#: lino_welfare/modlib/immersion/models.py:86
+#: lino_welfare/modlib/isip/models.py:150
+#: lino_welfare/modlib/jobs/models.py:127
 msgid "Organization"
 msgstr "Organisation"
 
 #: lino_welfare/modlib/cbss/tx25.py:811 lino_welfare/modlib/isip/models.py:54
 msgid "Reference"
 msgstr "Referenz"
 
@@ -1356,15 +1384,16 @@
 msgstr "Führerscheine"
 
 #: lino_welfare/modlib/cbss/tx25.py:1211
 msgid "Identity Cards"
 msgstr "Personalausweise"
 
 #: lino_welfare/modlib/cbss/tx25.py:1228 lino_welfare/modlib/pcsw/models.py:131
-#: lino_welfare/modlib/pcsw/models.py:951 lino_welfare/modlib/pcsw/models.py:1003
+#: lino_welfare/modlib/pcsw/models.py:953
+#: lino_welfare/modlib/pcsw/models.py:1005
 #: lino_welfare/modlib/reception/models.py:106
 #: lino_welfare/modlib/reception/models.py:133
 msgid "Reason"
 msgstr "Begründung"
 
 #: lino_welfare/modlib/cbss/tx25.py:1241
 msgid "Legal cohabitations"
@@ -1439,15 +1468,16 @@
 msgid "Birth location"
 msgstr "Geburtsort"
 
 #: lino_welfare/modlib/cbss/ui.py:208
 msgid "Civil state"
 msgstr "Zivilstand"
 
-#: lino_welfare/modlib/cbss/ui.py:212 lino_welfare/modlib/xcourses/models.py:604
+#: lino_welfare/modlib/cbss/ui.py:212
+#: lino_welfare/modlib/xcourses/models.py:605
 msgid "Address"
 msgstr "Adresse"
 
 #: lino_welfare/modlib/cbss/ui.py:223 lino_welfare/modlib/cbss/ui.py:245
 msgid "Requested action"
 msgstr "Angefragte Aktion"
 
@@ -1499,28 +1529,28 @@
 
 #: lino_welfare/modlib/contacts/models.py:118
 msgid "Cannot delete companies and persons imported from TIM"
 msgstr "Aus TIM importierte Partner dürfen nicht gelöscht werden."
 
 #: lino_welfare/modlib/contacts/models.py:159
 #: lino_welfare/modlib/contacts/models.py:247
-#: lino_welfare/modlib/contacts/models.py:332
+#: lino_welfare/modlib/contacts/models.py:337
 msgid "Contact"
 msgstr "Kontakt"
 
 #: lino_welfare/modlib/contacts/models.py:172
 #: lino_welfare/modlib/contacts/models.py:260
-#: lino_welfare/modlib/contacts/models.py:347
-#: lino_welfare/modlib/pcsw/models.py:561
+#: lino_welfare/modlib/contacts/models.py:352
+#: lino_welfare/modlib/pcsw/models.py:563
 msgid "Miscellaneous"
 msgstr "Sonstiges"
 
 #: lino_welfare/modlib/contacts/models.py:181
 #: lino_welfare/modlib/households/models.py:80
-#: lino_welfare/modlib/pcsw/models.py:468
+#: lino_welfare/modlib/pcsw/models.py:470
 msgid "Person"
 msgstr ""
 
 #: lino_welfare/modlib/contacts/models.py:182
 msgid "Persons"
 msgstr "Personen"
 
@@ -1592,19 +1622,21 @@
 msgstr ""
 
 #: lino_welfare/modlib/debts/choicelists.py:67
 #, fuzzy
 msgid "Sheet"
 msgstr "eID-Inhalt"
 
-#: lino_welfare/modlib/debts/choicelists.py:77 lino_welfare/modlib/debts/ui.py:627
+#: lino_welfare/modlib/debts/choicelists.py:77
+#: lino_welfare/modlib/debts/ui.py:627
 msgid "Assets"
 msgstr "Vermögen"
 
-#: lino_welfare/modlib/debts/choicelists.py:88 lino_welfare/modlib/debts/ui.py:602
+#: lino_welfare/modlib/debts/choicelists.py:88
+#: lino_welfare/modlib/debts/ui.py:602
 msgid "Liabilities"
 msgstr "Verpflichtungen"
 
 #: lino_welfare/modlib/debts/choicelists.py:99
 #, fuzzy
 msgid "Capital"
 msgstr "Kapazität"
@@ -1688,15 +1720,16 @@
 msgid "Required for Households"
 msgstr "verpflichtend für Haushalte"
 
 #: lino_welfare/modlib/debts/models.py:76
 msgid "Required for Persons"
 msgstr "verpflichtend für Personen"
 
-#: lino_welfare/modlib/debts/models.py:78 lino_welfare/modlib/debts/models.py:449
+#: lino_welfare/modlib/debts/models.py:78
+#: lino_welfare/modlib/debts/models.py:449
 msgid "Periods"
 msgstr "Perioden"
 
 #: lino_welfare/modlib/debts/models.py:79
 msgid "Default amount"
 msgstr "Standard-Betrag"
 
@@ -1732,18 +1765,20 @@
 
 #: lino_welfare/modlib/debts/models.py:121
 msgid "Include yearly incomes"
 msgstr "Jährliche Einkommen berücksichtigen"
 
 #: lino_welfare/modlib/debts/models.py:123
 msgid ""
-"Check this to include yearly incomes in the Debts Overview table of this Budget."
+"Check this to include yearly incomes in the Debts Overview table of this "
+"Budget."
 msgstr ""
 
-#: lino_welfare/modlib/debts/models.py:125 lino_welfare/modlib/integ/models.py:654
+#: lino_welfare/modlib/debts/models.py:125
+#: lino_welfare/modlib/integ/models.py:654
 msgid "Introduction"
 msgstr "Einleitung"
 
 #: lino_welfare/modlib/debts/models.py:126
 #: lino_welfare/modlib/jobs/template_messages.py:8
 msgid "Conclusion"
 msgstr "Schlussfolgerung"
@@ -1822,35 +1857,36 @@
 msgid "Distribute"
 msgstr "Verteilen"
 
 #: lino_welfare/modlib/debts/models.py:431
 msgid "To Do"
 msgstr "to do"
 
-#: lino_welfare/modlib/debts/models.py:439 lino_welfare/modlib/debts/models.py:502
-#: lino_welfare/modlib/debts/ui.py:440 lino_welfare/modlib/debts/ui.py:449
-#: lino_welfare/modlib/debts/ui.py:518 lino_welfare/modlib/debts/ui.py:706
-#: lino_welfare/modlib/integ/models.py:276 lino_welfare/modlib/integ/models.py:339
+#: lino_welfare/modlib/debts/models.py:439
+#: lino_welfare/modlib/debts/models.py:502 lino_welfare/modlib/debts/ui.py:440
+#: lino_welfare/modlib/debts/ui.py:449 lino_welfare/modlib/debts/ui.py:518
+#: lino_welfare/modlib/debts/ui.py:706 lino_welfare/modlib/integ/models.py:276
+#: lino_welfare/modlib/integ/models.py:339
 #: lino_welfare/modlib/xcourses/models.py:122
 msgid "Description"
 msgstr "Beschreibung"
 
 #: lino_welfare/modlib/debts/models.py:454 lino_welfare/modlib/debts/ui.py:481
 msgid "Monthly rate"
 msgstr "Monatsrate"
 
-#: lino_welfare/modlib/debts/models.py:463 lino_welfare/modlib/debts/models.py:577
-#: lino_welfare/modlib/debts/ui.py:477
+#: lino_welfare/modlib/debts/models.py:463
+#: lino_welfare/modlib/debts/models.py:577 lino_welfare/modlib/debts/ui.py:477
 msgid "Debt collection agency"
 msgstr "Schuldeneintreiber"
 
 #: lino_welfare/modlib/debts/models.py:464
 msgid ""
-"Leave empty for simple debts, otherwise select         here the responsible "
-"bailiff or collection agency"
+"Leave empty for simple debts, otherwise select         here the "
+"responsible bailiff or collection agency"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:531
 msgid "Periods must be > 0"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:535
@@ -1905,16 +1941,18 @@
 msgstr "Vorschau"
 
 #: lino_welfare/modlib/debts/ui.py:204
 msgid "Is partner of these budgets:"
 msgstr "Ist Hauptpartner in folgenden Budgets:"
 
 #: lino_welfare/modlib/debts/ui.py:436 lino_welfare/modlib/integ/models.py:206
-#: lino_welfare/modlib/integ/models.py:429 lino_welfare/modlib/integ/models.py:457
-#: lino_welfare/modlib/integ/models.py:491 lino_welfare/modlib/integ/models.py:565
+#: lino_welfare/modlib/integ/models.py:429
+#: lino_welfare/modlib/integ/models.py:457
+#: lino_welfare/modlib/integ/models.py:491
+#: lino_welfare/modlib/integ/models.py:565
 #: lino_welfare/modlib/integ/models.py:608
 msgid "Total"
 msgstr ""
 
 #: lino_welfare/modlib/debts/ui.py:457 lino_welfare/modlib/debts/ui.py:463
 msgid "Yearly amount"
 msgstr "Jährl. Betrag"
@@ -1970,19 +2008,20 @@
 
 #: lino_welfare/modlib/debts/ui.py:653
 #, fuzzy
 msgid ""
 "Répartition au marc-le-franc.\n"
 "A table with one row per entry in Liabilities which has \"distribute\" "
 "checked,\n"
-"proportionally distributing the `Distributable amount` among the debtors.\n"
+"proportionally distributing the `Distributable amount` among the debtors."
+"\n"
 msgstr ""
 "Répartition au marc-le-franc.\n"
-"Tabelle mit einer Zeile pro Eintrag in \"Verpflichtungen\", dessen Option "
-"\"verteilen\" angekreuzt ist. \n"
+"Tabelle mit einer Zeile pro Eintrag in \"Verpflichtungen\", dessen Option"
+" \"verteilen\" angekreuzt ist. \n"
 "Der verfügbare Betrag wird dabei proportional zum geschuldeten Betrag "
 "aufgeteilt.\n"
 
 #: lino_welfare/modlib/debts/ui.py:691
 msgid "%"
 msgstr ""
 
@@ -2159,15 +2198,16 @@
 msgid "Disbursement orders"
 msgstr "Ausgabeanweisungen"
 
 #: lino_welfare/modlib/finan/models.py:59
 msgid "Internal reference"
 msgstr "Interne Referenz"
 
-#: lino_welfare/modlib/finan/models.py:60 lino_welfare/modlib/finan/models.py:64
+#: lino_welfare/modlib/finan/models.py:60
+#: lino_welfare/modlib/finan/models.py:64
 msgid "External reference"
 msgstr "Externe Referenz"
 
 #: lino_welfare/modlib/households/models.py:130
 #, python-format
 msgid "%(count)d adult"
 msgid_plural "%(count)d adults"
@@ -2220,15 +2260,16 @@
 
 #: lino_welfare/modlib/immersion/models.py:98
 #: lino_welfare/modlib/isip/mixins.py:326
 msgid "responsibilities"
 msgstr "Aufgabenbereich"
 
 #: lino_welfare/modlib/immersion/models.py:118
-#: lino_welfare/modlib/isip/mixins.py:315 lino_welfare/modlib/isip/mixins.py:416
+#: lino_welfare/modlib/isip/mixins.py:315
+#: lino_welfare/modlib/isip/mixins.py:416
 #: lino_welfare/modlib/isip/models.py:221
 msgid "Responsible (IS)"
 msgstr "Verantwortlicher (DSBE)"
 
 #: lino_welfare/modlib/immersion/ui.py:97
 #, fuzzy
 msgid "Only immersion trainings of type"
@@ -2270,16 +2311,16 @@
 msgid "Available"
 msgstr "Verfügbar"
 
 #: lino_welfare/modlib/integ/models.py:77
 msgid "Integration Clients"
 msgstr "DSBE-Klienten"
 
-#: lino_welfare/modlib/integ/models.py:106 lino_welfare/modlib/pcsw/models.py:88
-#: lino_welfare/modlib/pcsw/models.py:867
+#: lino_welfare/modlib/integ/models.py:106
+#: lino_welfare/modlib/pcsw/models.py:88 lino_welfare/modlib/pcsw/models.py:869
 msgid "Integration phase"
 msgstr "Integrationsphase"
 
 #: lino_welfare/modlib/integ/models.py:108
 msgid "Language knowledge"
 msgstr "Sprachkenntnis"
 
@@ -2375,16 +2416,18 @@
 msgid "Job providers and contrats"
 msgstr ""
 
 #: lino_welfare/modlib/integ/models.py:632
 msgid "Activity Report"
 msgstr "Tätigkeitsbericht"
 
-#: lino_welfare/modlib/integ/models.py:639 lino_welfare/modlib/isip/__init__.py:13
-#: lino_welfare/modlib/isip/models.py:187 lino_welfare/modlib/isip/models.py:269
+#: lino_welfare/modlib/integ/models.py:639
+#: lino_welfare/modlib/isip/__init__.py:13
+#: lino_welfare/modlib/isip/models.py:187
+#: lino_welfare/modlib/isip/models.py:269
 msgid "ISIP"
 msgstr "VSE"
 
 #: lino_welfare/modlib/integ/models.py:664
 msgid "Indicateurs généraux"
 msgstr "Allgemeine Indikatoren"
 
@@ -2568,16 +2611,18 @@
 msgid "Reason of termination"
 msgstr "Beendigungsgrund"
 
 #: lino_welfare/modlib/isip/models.py:112
 msgid "Contract termination reasons"
 msgstr "Vertragsbeendigungsgründe"
 
-#: lino_welfare/modlib/isip/models.py:114 lino_welfare/modlib/jobs/models.py:407
-#: lino_welfare/modlib/pcsw/models.py:871 lino_welfare/modlib/pcsw/models.py:1048
+#: lino_welfare/modlib/isip/models.py:114
+#: lino_welfare/modlib/jobs/models.py:421
+#: lino_welfare/modlib/pcsw/models.py:873
+#: lino_welfare/modlib/pcsw/models.py:1050
 msgid "Designation"
 msgstr "Bezeichnung"
 
 #: lino_welfare/modlib/isip/models.py:118
 msgid "Require date ended"
 msgstr "erfordert Enddatum"
 
@@ -2593,15 +2638,16 @@
 msgid "duties company"
 msgstr "Verpflichtungen Firma"
 
 #: lino_welfare/modlib/isip/models.py:188
 msgid "ISIPs"
 msgstr "VSEs"
 
-#: lino_welfare/modlib/isip/models.py:192 lino_welfare/modlib/jobs/models.py:264
+#: lino_welfare/modlib/isip/models.py:192
+#: lino_welfare/modlib/jobs/models.py:274
 msgid "Contract Type"
 msgstr "Vertragsart"
 
 #: lino_welfare/modlib/isip/models.py:197
 msgid "stages"
 msgstr "Etappen"
 
@@ -2623,16 +2669,16 @@
 
 #: lino_welfare/modlib/isip/models.py:214
 msgid "duties person"
 msgstr "Verpflichtungen Person"
 
 #: lino_welfare/modlib/isip/models.py:246
 msgid ""
-"Cannot print {} because there is no active aid confirmation and Duties (PCSW) "
-"is empty."
+"Cannot print {} because there is no active aid confirmation and Duties "
+"(PCSW) is empty."
 msgstr ""
 "Kann {} nicht drucken, weil es keine aktive Hilfebestätigung gibt und "
 "Verpflichtungen ÖSHZ leer ist."
 
 #: lino_welfare/modlib/isip/models.py:365
 #, fuzzy
 msgid "Proceedings"
@@ -2655,23 +2701,23 @@
 msgstr "Kandidatur-Zustände"
 
 #: lino_welfare/modlib/jobs/mixins.py:26
 msgctxt "jobs"
 msgid "Active"
 msgstr "Aktiv"
 
-#: lino_welfare/modlib/jobs/mixins.py:27 lino_welfare/modlib/jobs/ui.py:443
+#: lino_welfare/modlib/jobs/mixins.py:27 lino_welfare/modlib/jobs/ui.py:457
 msgid "Probation"
 msgstr "Probezeit"
 
 #: lino_welfare/modlib/jobs/mixins.py:28
 msgid "Probation failed"
 msgstr "Probezeit ohne Erfolg"
 
-#: lino_welfare/modlib/jobs/mixins.py:29 lino_welfare/modlib/jobs/ui.py:435
+#: lino_welfare/modlib/jobs/mixins.py:29 lino_welfare/modlib/jobs/ui.py:449
 msgctxt "jobs"
 msgid "Working"
 msgstr "Arbeitet"
 
 #: lino_welfare/modlib/jobs/mixins.py:30
 msgctxt "jobs"
 msgid "Inactive"
@@ -2694,15 +2740,15 @@
 msgstr "Stellenanbieter"
 
 #: lino_welfare/modlib/jobs/models.py:52
 msgid "Job providers"
 msgstr "Stellenanbieter"
 
 #: lino_welfare/modlib/jobs/models.py:54 lino_welfare/modlib/jobs/models.py:70
-#: lino_welfare/modlib/jobs/models.py:410
+#: lino_welfare/modlib/jobs/models.py:424
 msgid "Social economy"
 msgstr "Sozialökonomie"
 
 #: lino_welfare/modlib/jobs/models.py:67
 msgid "Employer"
 msgstr "Arbeitgeber"
 
@@ -2714,103 +2760,110 @@
 msgid "Art60§7 job supplyment type"
 msgstr "Art.60§7-Konventionsart"
 
 #: lino_welfare/modlib/jobs/models.py:92
 msgid "Art60§7 job supplyment types"
 msgstr "Art.60§7-Konventionsarten"
 
-#: lino_welfare/modlib/jobs/models.py:218
+#: lino_welfare/modlib/jobs/models.py:220
 msgid "Job Offer"
 msgstr "Stellenangebot"
 
-#: lino_welfare/modlib/jobs/models.py:219
+#: lino_welfare/modlib/jobs/models.py:221
 msgid "Job Offers"
 msgstr "Stellenangebote"
 
-#: lino_welfare/modlib/jobs/models.py:222 lino_welfare/modlib/jobs/models.py:257
+#: lino_welfare/modlib/jobs/models.py:224
+#: lino_welfare/modlib/jobs/models.py:259
 #: lino_welfare/modlib/xcourses/models.py:71
 #: lino_welfare/modlib/xcourses/models.py:99
 #: lino_welfare/modlib/xcourses/models.py:170
 msgid "Name"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:226
+#: lino_welfare/modlib/jobs/models.py:228
 msgid "selection from"
 msgstr "Beginn Auswahl"
 
-#: lino_welfare/modlib/jobs/models.py:229
+#: lino_welfare/modlib/jobs/models.py:231
 msgid "selection until"
 msgstr "Ende Auswahl"
 
-#: lino_welfare/modlib/jobs/models.py:232
+#: lino_welfare/modlib/jobs/models.py:234
 #: lino_welfare/modlib/xcourses/models.py:172
 msgid "start date"
 msgstr "Beginndatum"
 
-#: lino_welfare/modlib/jobs/models.py:253 lino_welfare/modlib/jobs/ui.py:424
+#: lino_welfare/modlib/jobs/models.py:255 lino_welfare/modlib/jobs/ui.py:438
 msgid "Job"
 msgstr "Stelle"
 
-#: lino_welfare/modlib/jobs/models.py:254 lino_welfare/modlib/jobs/ui.py:82
-#: lino_welfare/modlib/jobs/ui.py:103
+#: lino_welfare/modlib/jobs/models.py:256 lino_welfare/modlib/jobs/ui.py:87
+#: lino_welfare/modlib/jobs/ui.py:115
 msgid "Jobs"
 msgstr "Stellen"
 
-#: lino_welfare/modlib/jobs/models.py:259 lino_welfare/modlib/jobs/models.py:402
+#: lino_welfare/modlib/jobs/models.py:261
+#: lino_welfare/modlib/jobs/models.py:416
 msgid "Job Type"
 msgstr "Stellenart"
 
-#: lino_welfare/modlib/jobs/models.py:268
+#: lino_welfare/modlib/jobs/models.py:267
+#, fuzzy
+msgid "Workplace"
+msgstr "Arbeit"
+
+#: lino_welfare/modlib/jobs/models.py:278
 msgid "capacity"
 msgstr "Kapazität"
 
-#: lino_welfare/modlib/jobs/models.py:273
+#: lino_welfare/modlib/jobs/models.py:283
 #, python-format
 msgid "%(job)s at %(provider)s"
 msgstr "%(job)s bei %(provider)s"
 
-#: lino_welfare/modlib/jobs/models.py:324
+#: lino_welfare/modlib/jobs/models.py:338
 msgid "Job Candidature"
 msgstr "Stellenanfrage"
 
-#: lino_welfare/modlib/jobs/models.py:325
+#: lino_welfare/modlib/jobs/models.py:339
 msgid "Job Candidatures"
 msgstr "Stellenanfragen"
 
-#: lino_welfare/modlib/jobs/models.py:333
+#: lino_welfare/modlib/jobs/models.py:347
 #: lino_welfare/modlib/xcourses/models.py:334
 msgid "date submitted"
 msgstr "Anfragedatum"
 
-#: lino_welfare/modlib/jobs/models.py:334
+#: lino_welfare/modlib/jobs/models.py:348
 msgid "Date when the IA introduced this candidature."
 msgstr "Datum wann der SA die Kandidatur erfasst hat."
 
-#: lino_welfare/modlib/jobs/models.py:341
+#: lino_welfare/modlib/jobs/models.py:355
 msgid "Art.60"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:343
+#: lino_welfare/modlib/jobs/models.py:357
 msgid "Whether an art.60 contract can satisfy this candidature."
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:347
+#: lino_welfare/modlib/jobs/models.py:361
 msgid "Art.61"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:349
+#: lino_welfare/modlib/jobs/models.py:363
 msgid "Whether an art.61 contract can satisfy this candidature."
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:374
+#: lino_welfare/modlib/jobs/models.py:388
 #, python-format
 msgid "Candidature by %(person)s"
 msgstr "Kandidatur von %(person)s"
 
-#: lino_welfare/modlib/jobs/models.py:403
+#: lino_welfare/modlib/jobs/models.py:417
 msgid "Job Types"
 msgstr "Stellenarten"
 
 #: lino_welfare/modlib/jobs/template_messages.py:6
 msgid "Renseignements généraux"
 msgstr "Allgemeine Auskünfte"
 
@@ -2818,37 +2871,42 @@
 msgid "Situation financière"
 msgstr "Finanzielle Situation"
 
 #: lino_welfare/modlib/jobs/template_messages.py:9
 msgid "Nom du médiateur de dettes"
 msgstr "Name des Schuldnerberaters"
 
-#: lino_welfare/modlib/jobs/ui.py:88
+#: lino_welfare/modlib/jobs/ui.py:93
 #, fuzzy
 msgid "Documents"
 msgstr "Dokumentarten"
 
-#: lino_welfare/modlib/jobs/ui.py:256
+#: lino_welfare/modlib/jobs/ui.py:105
+#, fuzzy
+msgid "Workplaces"
+msgstr "Arbeit"
+
+#: lino_welfare/modlib/jobs/ui.py:268
 msgid "Job Contracts Search"
 msgstr "Suche Art.60§7-Konventionen"
 
-#: lino_welfare/modlib/jobs/ui.py:359 lino_welfare/modlib/jobs/ui.py:439
-#: lino_welfare/modlib/xcourses/models.py:506
+#: lino_welfare/modlib/jobs/ui.py:371 lino_welfare/modlib/jobs/ui.py:453
+#: lino_welfare/modlib/xcourses/models.py:507
 msgid "Candidates"
 msgstr "Kandidaten"
 
-#: lino_welfare/modlib/jobs/ui.py:365
+#: lino_welfare/modlib/jobs/ui.py:377
 msgid "Experiences"
 msgstr "Erfahrungen"
 
-#: lino_welfare/modlib/jobs/ui.py:411 lino_welfare/modlib/jobs/ui.py:533
+#: lino_welfare/modlib/jobs/ui.py:425 lino_welfare/modlib/jobs/ui.py:547
 msgid "Contracts Situation"
 msgstr "Übersicht Art.60§7-Konventionen"
 
-#: lino_welfare/modlib/jobs/ui.py:427
+#: lino_welfare/modlib/jobs/ui.py:441
 msgctxt "(place)"
 msgid " at "
 msgstr " bei "
 
 #: lino_welfare/modlib/ledger/models.py:15
 msgid "Disbursement orders to execute"
 msgstr "Auszuführende Ausgabeanweisungen"
@@ -3015,47 +3073,47 @@
 msgstr "Aufwand"
 
 #: lino_welfare/modlib/newcomers/models.py:123
 msgid "Competence"
 msgstr "Kompetenz"
 
 #: lino_welfare/modlib/newcomers/models.py:124
-#: lino_welfare/modlib/pcsw/models.py:582
+#: lino_welfare/modlib/pcsw/models.py:584
 msgid "Competences"
 msgstr "Kompetenzen"
 
 #: lino_welfare/modlib/newcomers/models.py:143
 #, fuzzy
 msgid "User"
 msgstr "Ablehnen"
 
 #: lino_welfare/modlib/newcomers/models.py:213
 #: lino_welfare/modlib/newcomers/models.py:365
 msgid "New Clients"
 msgstr "Neue Klienten"
 
 #: lino_welfare/modlib/newcomers/models.py:229
-#: lino_welfare/modlib/newcomers/models.py:278
+#: lino_welfare/modlib/newcomers/models.py:279
 msgid "New clients since"
 msgstr "Neue Klienten seit"
 
-#: lino_welfare/modlib/newcomers/models.py:267
+#: lino_welfare/modlib/newcomers/models.py:268
 msgid "List of users available for new coachings"
 msgstr ""
 
-#: lino_welfare/modlib/newcomers/models.py:272
+#: lino_welfare/modlib/newcomers/models.py:273
 #: lino_welfare/modlib/newcomers/models.py:485
 msgid "Available Coaches"
 msgstr "Verfügbare Begleiter"
 
-#: lino_welfare/modlib/newcomers/models.py:276
+#: lino_welfare/modlib/newcomers/models.py:277
 msgid "Show suggested agents for"
 msgstr "Zeige Vorschläge für"
 
-#: lino_welfare/modlib/newcomers/models.py:281
+#: lino_welfare/modlib/newcomers/models.py:282
 msgid "New clients are those whose coaching started after this date"
 msgstr "Neue Klienten sind die, deren Begleitung nach diesem Datum beginnt"
 
 #: lino_welfare/modlib/newcomers/models.py:306
 #, fuzzy
 msgid "Only for clients with given `faculty`."
 msgstr "Nur für Neuanträge mit Angabe in `Fachbereich`."
@@ -3138,15 +3196,15 @@
 
 #: lino_welfare/modlib/pcsw/actions.py:145
 #, python-format
 msgid "This will end %(count)d coachings of %(client)s."
 msgstr "Hierdurch werden %(count)d Begleitungen von %(client)s beendet."
 
 #: lino_welfare/modlib/pcsw/choicelists.py:15
-#: lino_welfare/modlib/pcsw/models.py:946
+#: lino_welfare/modlib/pcsw/models.py:948
 msgid "Dispense"
 msgstr "Dispenz"
 
 #: lino_welfare/modlib/pcsw/choicelists.py:27
 msgid "Penalty"
 msgstr "AG-Sperre"
 
@@ -3235,224 +3293,224 @@
 msgid "Contact person at local job office"
 msgstr "Kontaktperson ADG"
 
 #: lino_welfare/modlib/pcsw/models.py:236
 msgid "Circular reference"
 msgstr "Redundanter RÜckbezug"
 
-#: lino_welfare/modlib/pcsw/models.py:262
+#: lino_welfare/modlib/pcsw/models.py:264
 msgid "eID card expires in 2 months"
 msgstr "eID-Karte läuft in 2 Monaten ab"
 
-#: lino_welfare/modlib/pcsw/models.py:264
+#: lino_welfare/modlib/pcsw/models.py:266
 msgid "becomes available again in 1 month"
 msgstr "wird wieder verfügbar in 1 Monat"
 
-#: lino_welfare/modlib/pcsw/models.py:267
+#: lino_welfare/modlib/pcsw/models.py:269
 msgid "work permit suspension ends in 1 month"
 msgstr "Arbeitslosen-Wartezeit endet in 1 Monat"
 
-#: lino_welfare/modlib/pcsw/models.py:350
+#: lino_welfare/modlib/pcsw/models.py:352
 msgid "Contract starts"
 msgstr "Vertrag beginnt"
 
-#: lino_welfare/modlib/pcsw/models.py:356
+#: lino_welfare/modlib/pcsw/models.py:358
 msgid "Contract ends"
 msgstr "Vertrag endet"
 
-#: lino_welfare/modlib/pcsw/models.py:365
+#: lino_welfare/modlib/pcsw/models.py:367
 msgid "Working at "
 msgstr "Arbeitet bei"
 
-#: lino_welfare/modlib/pcsw/models.py:372
+#: lino_welfare/modlib/pcsw/models.py:374
 #, fuzzy
 msgid "Active contract"
 msgstr "erlaubt in Verträgen"
 
-#: lino_welfare/modlib/pcsw/models.py:491
+#: lino_welfare/modlib/pcsw/models.py:493
 msgid "Human Links"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:497
+#: lino_welfare/modlib/pcsw/models.py:499
 msgid "Coaches"
 msgstr "Begleiter"
 
-#: lino_welfare/modlib/pcsw/models.py:523
+#: lino_welfare/modlib/pcsw/models.py:525
 msgid "Job search"
 msgstr "Arbeitssuche"
 
-#: lino_welfare/modlib/pcsw/models.py:552
+#: lino_welfare/modlib/pcsw/models.py:554
 msgid "Calendar"
 msgstr "Kalender"
 
-#: lino_welfare/modlib/pcsw/models.py:569
+#: lino_welfare/modlib/pcsw/models.py:571
 msgid "Career"
 msgstr "Lebenslauf"
 
-#: lino_welfare/modlib/pcsw/models.py:576
+#: lino_welfare/modlib/pcsw/models.py:578
 msgid "Languages"
 msgstr "Sprachen"
 
-#: lino_welfare/modlib/pcsw/models.py:590
+#: lino_welfare/modlib/pcsw/models.py:592
 msgid "Contracts"
 msgstr "Verträge"
 
-#: lino_welfare/modlib/pcsw/models.py:635
+#: lino_welfare/modlib/pcsw/models.py:637
 msgid "Coached by"
 msgstr "Begleitet durch"
 
-#: lino_welfare/modlib/pcsw/models.py:641
+#: lino_welfare/modlib/pcsw/models.py:643
 msgid "and by"
 msgstr "und durch"
 
-#: lino_welfare/modlib/pcsw/models.py:647
+#: lino_welfare/modlib/pcsw/models.py:649
 msgid "Nationality"
 msgstr "Staatsangehörigkeit"
 
-#: lino_welfare/modlib/pcsw/models.py:651
+#: lino_welfare/modlib/pcsw/models.py:653
 msgid "Extended filter criteria, e.g.:"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:652
+#: lino_welfare/modlib/pcsw/models.py:654
 msgid "Active: All those who have some active coaching."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:653
+#: lino_welfare/modlib/pcsw/models.py:655
 msgid "Only primary clients"
 msgstr "Nur primäre Begleitungen"
 
-#: lino_welfare/modlib/pcsw/models.py:782
+#: lino_welfare/modlib/pcsw/models.py:784
 msgid "and"
 msgstr "und"
 
-#: lino_welfare/modlib/pcsw/models.py:786
+#: lino_welfare/modlib/pcsw/models.py:788
 #, python-format
 msgid " on %(date)s"
 msgstr " am %(date)s"
 
-#: lino_welfare/modlib/pcsw/models.py:790
+#: lino_welfare/modlib/pcsw/models.py:792
 #, python-format
 msgid "Coached on %s"
 msgstr "Begleitet am %s"
 
-#: lino_welfare/modlib/pcsw/models.py:841
+#: lino_welfare/modlib/pcsw/models.py:843
 msgid "Check for valid identification"
 msgstr "Auf gültige Identifizierungsangaben prüfen"
 
-#: lino_welfare/modlib/pcsw/models.py:850
+#: lino_welfare/modlib/pcsw/models.py:852
 msgid "Neither valid eId data nor alternative identifying document."
 msgstr "Weder gültige eID-Daten noch identifizierendes Dokument."
 
-#: lino_welfare/modlib/pcsw/models.py:868
+#: lino_welfare/modlib/pcsw/models.py:870
 msgid "Integration phases"
 msgstr "Integrationsphasen"
 
-#: lino_welfare/modlib/pcsw/models.py:872
+#: lino_welfare/modlib/pcsw/models.py:874
 msgid "Reference name"
 msgstr "Referenzname"
 
-#: lino_welfare/modlib/pcsw/models.py:873
+#: lino_welfare/modlib/pcsw/models.py:875
 msgid "Considered active"
 msgstr "aktive Phase"
 
-#: lino_welfare/modlib/pcsw/models.py:898
+#: lino_welfare/modlib/pcsw/models.py:900
 msgid "activity"
 msgstr "Beruf"
 
-#: lino_welfare/modlib/pcsw/models.py:899
+#: lino_welfare/modlib/pcsw/models.py:901
 msgid "activities"
 msgstr "Berufe"
 
-#: lino_welfare/modlib/pcsw/models.py:902
+#: lino_welfare/modlib/pcsw/models.py:904
 msgid "Appears in Listing 104"
 msgstr "Listing 104"
 
-#: lino_welfare/modlib/pcsw/models.py:909
+#: lino_welfare/modlib/pcsw/models.py:911
 msgid "Liste des \"activités\" ou \"codes profession\"."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:925
+#: lino_welfare/modlib/pcsw/models.py:927
 msgid "Dispense reason"
 msgstr "Dispenzgrund"
 
-#: lino_welfare/modlib/pcsw/models.py:926
+#: lino_welfare/modlib/pcsw/models.py:928
 msgid "Dispense reasons"
 msgstr "Dispenzgründe"
 
-#: lino_welfare/modlib/pcsw/models.py:935
+#: lino_welfare/modlib/pcsw/models.py:937
 msgid "A list of reasons for being dispensed"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:947
+#: lino_welfare/modlib/pcsw/models.py:949
 msgid "Dispenses"
 msgstr "Dispenzen"
 
-#: lino_welfare/modlib/pcsw/models.py:955
+#: lino_welfare/modlib/pcsw/models.py:957
 msgid "Dispensed from"
 msgstr "Dispenziert seit"
 
-#: lino_welfare/modlib/pcsw/models.py:961
+#: lino_welfare/modlib/pcsw/models.py:963
 msgid "Liste de dispenses"
 msgstr "Liste aller Dispenzen"
 
-#: lino_welfare/modlib/pcsw/models.py:978
+#: lino_welfare/modlib/pcsw/models.py:980
 msgid "Unemployment exclusion type"
 msgstr "AG-Sperrgrund"
 
-#: lino_welfare/modlib/pcsw/models.py:979
+#: lino_welfare/modlib/pcsw/models.py:981
 msgid "Unemployment exclusion types"
 msgstr "AG-Sperrgründe"
 
-#: lino_welfare/modlib/pcsw/models.py:988
+#: lino_welfare/modlib/pcsw/models.py:990
 msgid ""
 "Liste des raisons possibles d'arrêter temporairement\n"
 "    le paiement d'une aide financière prévue."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:998
+#: lino_welfare/modlib/pcsw/models.py:1000
 msgid "Exclusion from unemployment"
 msgstr "AG-Sperre"
 
-#: lino_welfare/modlib/pcsw/models.py:999
+#: lino_welfare/modlib/pcsw/models.py:1001
 msgid "Exclusions from unemployment"
 msgstr "AG-Sperren"
 
-#: lino_welfare/modlib/pcsw/models.py:1008
+#: lino_welfare/modlib/pcsw/models.py:1010
 msgid "Excluded from"
 msgstr "AG-Sperre seit"
 
-#: lino_welfare/modlib/pcsw/models.py:1025
+#: lino_welfare/modlib/pcsw/models.py:1027
 msgid "Liste des exclusions."
 msgstr "Liste der Arbeitslosengeld-Sperren"
 
-#: lino_welfare/modlib/pcsw/models.py:1031
+#: lino_welfare/modlib/pcsw/models.py:1033
 msgid "Unemployment situation"
 msgstr "AG-Sperren"
 
-#: lino_welfare/modlib/pcsw/models.py:1042
+#: lino_welfare/modlib/pcsw/models.py:1044
 msgid "Conviction"
 msgstr "Vorstrafe"
 
-#: lino_welfare/modlib/pcsw/models.py:1043
+#: lino_welfare/modlib/pcsw/models.py:1045
 msgid "Convictions"
 msgstr "Vorstrafen"
 
-#: lino_welfare/modlib/pcsw/models.py:1047
+#: lino_welfare/modlib/pcsw/models.py:1049
 msgid "Prejudicial"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:1083
+#: lino_welfare/modlib/pcsw/models.py:1085
 msgid "aid type"
 msgstr "Sozialhilfeart"
 
-#: lino_welfare/modlib/pcsw/models.py:1084
+#: lino_welfare/modlib/pcsw/models.py:1086
 msgid "aid types"
 msgstr "Sozialhilfearten"
 
-#: lino_welfare/modlib/pcsw/models.py:1088
+#: lino_welfare/modlib/pcsw/models.py:1090
 msgid "Liste des types d'aide financière."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/fixtures/std.py:24
 msgid "Formation"
 msgstr "Ausbildung"
 
@@ -3658,891 +3716,907 @@
 msgid "Lino Welfare"
 msgstr "Lino für ÖSHZ"
 
 #: lino_welfare/modlib/welfare/help_texts.py:7
 msgid "The standard migrator for welfare."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:9
+#: lino_welfare/modlib/welfare/help_texts.py:8
 msgid "The plugin."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:11
+#: lino_welfare/modlib/welfare/help_texts.py:9
 msgid ""
-"Optionally specify the primary key (an integer) of the last granting for which "
-"you want to deactivate date range validation in confirmations. This is useful "
-"for keeping legacy confirmations that have been issued before the rule was "
-"activated."
+"Optionally specify the primary key (an integer) of the last granting for "
+"which you want to deactivate date range validation in confirmations. This"
+" is useful for keeping legacy confirmations that have been issued before "
+"the rule was activated."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:14
-#: lino_welfare/modlib/welfare/help_texts.py:19
-#: lino_welfare/modlib/welfare/help_texts.py:94
-#: lino_welfare/modlib/welfare/help_texts.py:96
-#: lino_welfare/modlib/welfare/help_texts.py:104
-#: lino_welfare/modlib/welfare/help_texts.py:106
-#: lino_welfare/modlib/welfare/help_texts.py:108
-#: lino_welfare/modlib/welfare/help_texts.py:117
-#: lino_welfare/modlib/welfare/help_texts.py:119
-#: lino_welfare/modlib/welfare/help_texts.py:121
-#: lino_welfare/modlib/welfare/help_texts.py:123
+#: lino_welfare/modlib/welfare/help_texts.py:10
+#: lino_welfare/modlib/welfare/help_texts.py:12
+#: lino_welfare/modlib/welfare/help_texts.py:43
+#: lino_welfare/modlib/welfare/help_texts.py:44
+#: lino_welfare/modlib/welfare/help_texts.py:47
+#: lino_welfare/modlib/welfare/help_texts.py:48
+#: lino_welfare/modlib/welfare/help_texts.py:49
+#: lino_welfare/modlib/welfare/help_texts.py:53
+#: lino_welfare/modlib/welfare/help_texts.py:54
+#: lino_welfare/modlib/welfare/help_texts.py:55
+#: lino_welfare/modlib/welfare/help_texts.py:56
 msgid "See lino.core.plugin.Plugin."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:16
+#: lino_welfare/modlib/welfare/help_texts.py:11
 msgid ""
-"A string referring to the model which represents the badge holder in your "
-"application. Default value is 'contacts.Person'."
+"A string referring to the model which represents the badge holder in your"
+" application. Default value is 'contacts.Person'."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:21
+#: lino_welfare/modlib/welfare/help_texts.py:13
 msgid "The descriptor for this plugin. See lino.core.plugin.Plugin."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:23
+#: lino_welfare/modlib/welfare/help_texts.py:14
 msgid ""
-"Whether executing requests should try to really connect to the CBSS. Real "
-"requests would fail with a timeout if run from behind an IP address that is not "
-"registered at the CBSS."
+"Whether executing requests should try to really connect to the CBSS. Real"
+" requests would fail with a timeout if run from behind an IP address that"
+" is not registered at the CBSS."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:26
+#: lino_welfare/modlib/welfare/help_texts.py:15
 msgid "Either None or one of ‘test’, ‘acpt’ or ‘prod’."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:28
+#: lino_welfare/modlib/welfare/help_texts.py:16
 #, fuzzy
 msgid "The status of a CBSSRequest."
 msgstr "Antragsdatum"
 
-#: lino_welfare/modlib/welfare/help_texts.py:30
+#: lino_welfare/modlib/welfare/help_texts.py:17
 msgid ""
-"Possible values for the action field of a lino_welfare.modlib.cbss.models."
-"ManageAccessRequest."
+"Possible values for the action field of a "
+"lino_welfare.modlib.cbss.models.ManageAccessRequest."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:33
+#: lino_welfare/modlib/welfare/help_texts.py:18
 msgid ""
-"Ce service est sollicité au moment du démarrage de l’enquête sociale. Le CPAS "
-"déclare au réseau de la sécurité sociale qu’il possède un dossier pour lequel "
-"il a l’autorisation (dispositions légales et réglementaires) d’obtenir des "
-"informations des autres institutions en vue de compléter son enquête dans le "
-"cadre de l’octroi du revenu d’intégration. Cette déclaration concerne le "
-"répertoire sectoriel des CPAS à la SmalS-MvM et peut concerner plusieurs "
-"catégories de personnes : le demandeur, les cohabitants et les tiers concernés "
-"et ce, pour des finalités différentes."
+"Ce service est sollicité au moment du démarrage de l’enquête sociale. Le "
+"CPAS déclare au réseau de la sécurité sociale qu’il possède un dossier "
+"pour lequel il a l’autorisation (dispositions légales et réglementaires) "
+"d’obtenir des informations des autres institutions en vue de compléter "
+"son enquête dans le cadre de l’octroi du revenu d’intégration. Cette "
+"déclaration concerne le répertoire sectoriel des CPAS à la SmalS-MvM et "
+"peut concerner plusieurs catégories de personnes : le demandeur, les "
+"cohabitants et les tiers concernés et ce, pour des finalités différentes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:36
+#: lino_welfare/modlib/welfare/help_texts.py:19
 msgid "L’opération contraire est aussi mise à disposition."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:38
+#: lino_welfare/modlib/welfare/help_texts.py:20
 msgid ""
 "Il est en plus possible d’obtenir une liste des enregistrements dans le "
-"répertoire sectoriel des CPAS à la SmalS-MvM ainsi qu’au sein du réseau BCSS."
+"répertoire sectoriel des CPAS à la SmalS-MvM ainsi qu’au sein du réseau "
+"BCSS."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:41
+#: lino_welfare/modlib/welfare/help_texts.py:21
 msgid ""
-"Possible values for the query_register field of a lino_welfare.modlib.cbss."
-"models.ManageAccessRequest."
+"Possible values for the query_register field of a "
+"lino_welfare.modlib.cbss.models.ManageAccessRequest."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:44
+#: lino_welfare/modlib/welfare/help_texts.py:22
 msgid "Query only the primary register."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:46
+#: lino_welfare/modlib/welfare/help_texts.py:23
 msgid "Query only the secondary register."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:48
+#: lino_welfare/modlib/welfare/help_texts.py:24
 #, fuzzy
 msgid "Query both registers."
 msgstr "Abfrageregister"
 
-#: lino_welfare/modlib/welfare/help_texts.py:50
+#: lino_welfare/modlib/welfare/help_texts.py:25
 msgid "Common Abstract Base Class for SSDNRequest and NewStyleRequest"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:52
+#: lino_welfare/modlib/welfare/help_texts.py:26
 msgid "alias of NotImplementedError"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:54
+#: lino_welfare/modlib/welfare/help_texts.py:27
 msgid ""
-"When duplicating a CBSS request, we want re-execute it. So please duplicate "
-"only the parameters, not the execution data like ticket, sent and status. Note "
-"that also the user will be set to the user who asked to duplicate (because this "
-"is a subclass of UserAuthored."
+"When duplicating a CBSS request, we want re-execute it. So please "
+"duplicate only the parameters, not the execution data like ticket, sent "
+"and status. Note that also the user will be set to the user who asked to "
+"duplicate (because this is a subclass of UserAuthored."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:57
+#: lino_welfare/modlib/welfare/help_texts.py:28
 msgid "CBSS requests that have a ticket may never be modified."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:59
-#: lino_welfare/modlib/welfare/help_texts.py:83
+#: lino_welfare/modlib/welfare/help_texts.py:29
+#: lino_welfare/modlib/welfare/help_texts.py:38
 msgid "Called when a successful reply has been received."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:61
+#: lino_welfare/modlib/welfare/help_texts.py:30
 msgid "This is the common part of a request for both classic and new-style."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:64
+#: lino_welfare/modlib/welfare/help_texts.py:31
 msgid ""
 "When we print a request, the resulting excerpt should go to the client’s "
 "history."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:67
+#: lino_welfare/modlib/welfare/help_texts.py:32
 msgid "Abstract Base Class for Models that represent SSDN (“classic”) requests."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:70
+#: lino_welfare/modlib/welfare/help_texts.py:33
 msgid ""
-"Validates the generated XML against the XSD files. Used by test suite. It is "
-"not necessary to validate each real request before actually sending it."
+"Validates the generated XML against the XSD files. Used by test suite. It"
+" is not necessary to validate each real request before actually sending "
+"it."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:73
+#: lino_welfare/modlib/welfare/help_texts.py:34
 msgid "SSDN specific part of a request."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:75
+#: lino_welfare/modlib/welfare/help_texts.py:35
 msgid ""
-"Wrap the given service request into the SSDN envelope by adding AuthorizedUser "
-"and other information common the all SSDN requests)."
+"Wrap the given service request into the SSDN envelope by adding "
+"AuthorizedUser and other information common the all SSDN requests)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:78
+#: lino_welfare/modlib/welfare/help_texts.py:36
 msgid ""
-"Abstract Base Class for Models that represent “new style” requests to the CBSS "
-"(and responses)."
+"Abstract Base Class for Models that represent “new style” requests to the"
+" CBSS (and responses)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:81
+#: lino_welfare/modlib/welfare/help_texts.py:37
 msgid "NewStyle specific part of a request."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:85
+#: lino_welfare/modlib/welfare/help_texts.py:39
 msgid ""
 "Abstract base for Requests that have a field national_id and a method "
 "get_ssin()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:88
+#: lino_welfare/modlib/welfare/help_texts.py:40
 msgid "Mixin for models that have certain fields"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:90
+#: lino_welfare/modlib/welfare/help_texts.py:41
 msgid "Space-separated list of all first names."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:92
+#: lino_welfare/modlib/welfare/help_texts.py:42
 msgid "Last name (family name)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:98
+#: lino_welfare/modlib/welfare/help_texts.py:45
 msgid ""
-"Model mixin to add to the base classes of your application’s pcsw.Client model."
+"Model mixin to add to the base classes of your application’s pcsw.Client "
+"model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:101
+#: lino_welfare/modlib/welfare/help_texts.py:46
 msgid ""
-"Overrides lino.mixins.dupable.Dupable.find_similar_instances(), adding some "
-"additional rules."
+"Overrides lino.mixins.dupable.Dupable.find_similar_instances(), adding "
+"some additional rules."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:110
+#: lino_welfare/modlib/welfare/help_texts.py:50
 msgid ""
 "Whether to show only primary coachings in the columns (coachings per "
 "Integration phase table."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:113
+#: lino_welfare/modlib/welfare/help_texts.py:51
 msgid "Has access to data used by integration agents."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:115
+#: lino_welfare/modlib/welfare/help_texts.py:52
 msgid "Can configure social integration functionality."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:125
+#: lino_welfare/modlib/welfare/help_texts.py:57
 msgid "Refuse this newcomer request."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:127
+#: lino_welfare/modlib/welfare/help_texts.py:58
 msgid ""
-"Change client’s state to ‘former’. This will also end any active coachings."
+"Change client’s state to ‘former’. This will also end any active "
+"coachings."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:130
+#: lino_welfare/modlib/welfare/help_texts.py:59
 msgid "Has limited access to data of social workers. Can see contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:132
+#: lino_welfare/modlib/welfare/help_texts.py:60
 msgid "Can access data managed by general social workers."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:134
+#: lino_welfare/modlib/welfare/help_texts.py:61
 msgid "Can configure general social work functionality."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:136
+#: lino_welfare/modlib/welfare/help_texts.py:62
 msgid "Can manage external courses."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:138
+#: lino_welfare/modlib/welfare/help_texts.py:63
 msgid "Can manage and configure external courses."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:140
+#: lino_welfare/modlib/welfare/help_texts.py:64
 msgid "The Django model representing an aid type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:142
+#: lino_welfare/modlib/welfare/help_texts.py:65
 msgid ""
-"The short name for internal use, e.g. when a user must select an aid type from "
-"a combobox."
+"The short name for internal use, e.g. when a user must select an aid type"
+" from a combobox."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:145
+#: lino_welfare/modlib/welfare/help_texts.py:66
 msgid ""
-"The database model to use for issuing an aid confirmation of this type. This is "
-"a mandatory pointer to ConfirmationTypes."
+"The database model to use for issuing an aid confirmation of this type. "
+"This is a mandatory pointer to ConfirmationTypes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:148
+#: lino_welfare/modlib/welfare/help_texts.py:67
 msgid ""
-"The designation of this aid type as seen by the user e.g. when selecting an aid "
-"type."
+"The designation of this aid type as seen by the user e.g. when selecting "
+"an aid type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:151
+#: lino_welfare/modlib/welfare/help_texts.py:68
 msgid ""
-"The text to print as title in confirmations. See also lino_xl.lib.excerpts."
-"mixins.ExcerptTitle.excerpt_title."
+"The text to print as title in confirmations. See also "
+"lino_xl.lib.excerpts.mixins.ExcerptTitle.excerpt_title."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:154
+#: lino_welfare/modlib/welfare/help_texts.py:69
 msgid ""
-"The body template to use when printing a confirmation of this type. If this "
-"field is empty, Lino uses the excerpt type’s body_template. See also lino.admin."
-"printing."
+"The body template to use when printing a confirmation of this type. If "
+"this field is empty, Lino uses the excerpt type’s body_template. See also"
+" lino.admin.printing."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:157
+#: lino_welfare/modlib/welfare/help_texts.py:70
 msgid ""
-"Whether aid grantings of this type are considered as urgent. This is used by "
-"Confirmation.get_urgent_granting()"
+"Whether aid grantings of this type are considered as urgent. This is used"
+" by Confirmation.get_urgent_granting()"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:160
+#: lino_welfare/modlib/welfare/help_texts.py:71
 msgid ""
-"Pointer to the default lino_xl.lib.boards.models.Board for aid projects of this "
-"type."
+"Pointer to the default lino_xl.lib.boards.models.Board for aid projects "
+"of this type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:163
+#: lino_welfare/modlib/welfare/help_texts.py:72
 msgid ""
-"Whether grantings for this aid type are to be signed by the client’s primary "
-"coach (see Client.get_primary_coach)."
+"Whether grantings for this aid type are to be signed by the client’s "
+"primary coach (see Client.get_primary_coach)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:166
+#: lino_welfare/modlib/welfare/help_texts.py:73
 msgid ""
-"A pointer to the ClientContactType to be used when selecting the pharmacy of a "
-"refund confirmation (RefundConfirmation.pharmacy)."
+"A pointer to the ClientContactType to be used when selecting the pharmacy"
+" of a refund confirmation (RefundConfirmation.pharmacy)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:169
+#: lino_welfare/modlib/welfare/help_texts.py:74
 msgid "The Django model representing an aid granting."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:171
+#: lino_welfare/modlib/welfare/help_texts.py:75
 msgid "Pointer to the lino_welfare.modlib.pcsw.models.Client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:173
+#: lino_welfare/modlib/welfare/help_texts.py:76
 msgid "The type of aid being granted. Mandatory. Pointer to the AidType."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:175
+#: lino_welfare/modlib/welfare/help_texts.py:77
 msgid ""
-"Pointer to the user who is expected to “sign” this granting (i.e. to confirm "
-"that it is real)."
+"Pointer to the user who is expected to “sign” this granting (i.e. to "
+"confirm that it is real)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:178
+#: lino_welfare/modlib/welfare/help_texts.py:78
 msgid "Pointer to the Board which decided to allocate this aid project."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:180
+#: lino_welfare/modlib/welfare/help_texts.py:79
 msgid "Currently only used for printing an isip.Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:182
+#: lino_welfare/modlib/welfare/help_texts.py:80
 msgid "Base class for all aid confirmations."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:184
+#: lino_welfare/modlib/welfare/help_texts.py:81
 #, fuzzy
 msgid ""
-"Return an error message if this confirmation lies outside of granted period."
+"Return an error message if this confirmation lies outside of granted "
+"period."
 msgstr "Datumsbereich %(p1)s außerhalb der Laufzeit des Beschlusses %(p2)s."
 
-#: lino_welfare/modlib/welfare/help_texts.py:187
+#: lino_welfare/modlib/welfare/help_texts.py:82
 msgid "Base class for both Granting and Confirmation."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:189
+#: lino_welfare/modlib/welfare/help_texts.py:83
 msgid "The confirmation state of this object. Pointer to ConfirmationStates."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:192
+#: lino_welfare/modlib/welfare/help_texts.py:84
 msgid "Sign this granting or confirmation, making most fields read-only."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:194
+#: lino_welfare/modlib/welfare/help_texts.py:85
 msgid "Revoke your signature of this granting or confirmation."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:196
+#: lino_welfare/modlib/welfare/help_texts.py:86
 msgid "Adds two fields."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:198
+#: lino_welfare/modlib/welfare/help_texts.py:87
 msgid "How to summarize entries of this type in the ESF summary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:200
+#: lino_welfare/modlib/welfare/help_texts.py:88
 msgid "Adds a virtual field client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:202
+#: lino_welfare/modlib/welfare/help_texts.py:89
 msgid "Virtual field which returns the partner if it is a client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:204
+#: lino_welfare/modlib/welfare/help_texts.py:90
+msgid ""
+"Shows calendar entries having either project or one guest pointing to "
+"this client."
+msgstr ""
+
+#: lino_welfare/modlib/welfare/help_texts.py:91
 msgid "Default values filled from lino_welfare.modlib.cbss.fixtures.sectors."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:207
+#: lino_welfare/modlib/welfare/help_texts.py:92
 msgid ""
-"Codes qualité (Hoedanigheidscodes). This table is usually filled with the "
-"official codes by lino_welfare.modlib.cbss.fixtures.purposes."
+"Codes qualité (Hoedanigheidscodes). This table is usually filled with the"
+" official codes by lino_welfare.modlib.cbss.fixtures.purposes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:210
+#: lino_welfare/modlib/welfare/help_texts.py:93
 msgid "A request to the IdentifyPerson service."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:212
+#: lino_welfare/modlib/welfare/help_texts.py:94
 msgid "A request to the ManageAccess service."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:214
+#: lino_welfare/modlib/welfare/help_texts.py:95
 msgid "Pointer to Sector."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:216
+#: lino_welfare/modlib/welfare/help_texts.py:96
 msgid "Pointer to Purpose."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:218
+#: lino_welfare/modlib/welfare/help_texts.py:97
 msgid ""
-"The action to perform. This must be one of the values in lino_welfare.modlib."
-"cbss.choicelists.ManageActions"
+"The action to perform. This must be one of the values in "
+"lino_welfare.modlib.cbss.choicelists.ManageActions"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:221
+#: lino_welfare/modlib/welfare/help_texts.py:98
 msgid ""
-"The register to be query. This must be one of the values in lino_welfare.modlib."
-"cbss.choicelists.QueryRegisters"
+"The register to be query. This must be one of the values in "
+"lino_welfare.modlib.cbss.choicelists.QueryRegisters"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:224
+#: lino_welfare/modlib/welfare/help_texts.py:99
 msgid "A request to the RetrieveTIGroups service (aka Tx25)"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:226
+#: lino_welfare/modlib/welfare/help_texts.py:100
 #, fuzzy
 msgid "Whether to print empty rows."
 msgstr "Auch leere Einträge drucken"
 
-#: lino_welfare/modlib/welfare/help_texts.py:228
+#: lino_welfare/modlib/welfare/help_texts.py:101
 #, fuzzy
 msgid "Whether to ignore yearly incomes."
 msgstr "Jährliche Einkommen berücksichtigen"
 
-#: lino_welfare/modlib/welfare/help_texts.py:230
+#: lino_welfare/modlib/welfare/help_texts.py:102
 msgid ""
-"Yield the entry groups for this budget, i.e. one item for each account group "
-"for which this budget has some data."
+"Yield the entry groups for this budget, i.e. one item for each account "
+"group for which this budget has some data."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:233
+#: lino_welfare/modlib/welfare/help_texts.py:103
 msgid "The database model used to represent a budget actor."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:235
+#: lino_welfare/modlib/welfare/help_texts.py:104
 msgid "A detail row of a Budget."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:237
+#: lino_welfare/modlib/welfare/help_texts.py:105
 msgid ""
-"Optionally specify a budget actor who contributes this entry. Leave empty when "
-"the entry refers to the entire household."
+"Optionally specify a budget actor who contributes this entry. Leave empty"
+" when the entry refers to the entire household."
 msgstr ""
-"Hier optional den Akteur angeben, der diesen Eintrag beiträgt. Leer lassen, "
-"wenn der Eintrag sich auf den Gesamthaushalt bezieht."
+"Hier optional den Akteur angeben, der diesen Eintrag beiträgt. Leer "
+"lassen, wenn der Eintrag sich auf den Gesamthaushalt bezieht."
 
-#: lino_welfare/modlib/welfare/help_texts.py:240
+#: lino_welfare/modlib/welfare/help_texts.py:106
 msgid ""
-"The amount of money. An empty amount is different from a zero amount in that "
-"the latter will be printed while the former not."
+"The amount of money. An empty amount is different from a zero amount in "
+"that the latter will be printed while the former not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:243
+#: lino_welfare/modlib/welfare/help_texts.py:107
 msgid "The related Account."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:245
+#: lino_welfare/modlib/welfare/help_texts.py:108
 msgid ""
-"An account is an item of an account chart used to collect ledger transactions "
-"or other accountable items."
+"An account is an item of an account chart used to collect ledger "
+"transactions or other accountable items."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:248
+#: lino_welfare/modlib/welfare/help_texts.py:109
 msgid "The multilingual designation of this account, as the users see it."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:251
+#: lino_welfare/modlib/welfare/help_texts.py:110
 msgid ""
-"The account group to which this account belongs. This must point to an instance "
-"of Group."
+"The account group to which this account belongs. This must point to an "
+"instance of Group."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:254
+#: lino_welfare/modlib/welfare/help_texts.py:111
 msgid "The sequence number of this account within its group."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:256
+#: lino_welfare/modlib/welfare/help_texts.py:112
 msgid "An optional unique name which can be used to reference a given account."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:259
+#: lino_welfare/modlib/welfare/help_texts.py:113
 msgid ""
-"The account type of this account. This must point to an item of lino_welfare."
-"modlib.debts.AccountTypes."
+"The account type of this account. This must point to an item of "
+"lino_welfare.modlib.debts.AccountTypes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:262
+#: lino_welfare/modlib/welfare/help_texts.py:114
 msgid "Base class for both the volatile MainActor and the Actor model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:264
+#: lino_welfare/modlib/welfare/help_texts.py:115
 msgid "A volatile object that represents the budget partner as actor"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:266
+#: lino_welfare/modlib/welfare/help_texts.py:116
 msgid ""
-"Used for Entry.periods and Account.periods (the latter holds simply the default "
-"value for the former). It means: for how many months the entered amount counts. "
-"Default value is 1. For yearly amounts set it to 12."
+"Used for Entry.periods and Account.periods (the latter holds simply the "
+"default value for the former). It means: for how many months the entered "
+"amount counts. Default value is 1. For yearly amounts set it to 12."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:269
+#: lino_welfare/modlib/welfare/help_texts.py:117
 msgid "The Django model that represents a client summary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:271
+#: lino_welfare/modlib/welfare/help_texts.py:118
 msgid "Base class for all tables on ClientSummary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:273
+#: lino_welfare/modlib/welfare/help_texts.py:119
 msgid "Lists all ESF summaries for all clients."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:275
+#: lino_welfare/modlib/welfare/help_texts.py:120
 msgid "Lists the ESF summaries for a given client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:277
+#: lino_welfare/modlib/welfare/help_texts.py:121
 msgid "Base class for all statistical fields."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:279
+#: lino_welfare/modlib/welfare/help_texts.py:122
 msgid "Used as the verbose_name of field."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:281
+#: lino_welfare/modlib/welfare/help_texts.py:123
 msgid "The internal field name."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:283
+#: lino_welfare/modlib/welfare/help_texts.py:124
 msgid "The field descriptor (an instance of a Django Field)"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:285
+#: lino_welfare/modlib/welfare/help_texts.py:125
 msgid "Count the number of presences."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:287
+#: lino_welfare/modlib/welfare/help_texts.py:126
 msgid "Count the real hours of presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:289
+#: lino_welfare/modlib/welfare/help_texts.py:127
 msgid "Count the event’s duration for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:291
+#: lino_welfare/modlib/welfare/help_texts.py:128
 msgid "Count a fixed time for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:293
+#: lino_welfare/modlib/welfare/help_texts.py:129
 msgid ""
-"Shows the members of the primary household of this person together with an "
-"amount which depends on whether that member is adult or not."
+"Shows the members of the primary household of this person together with "
+"an amount which depends on whether that member is adult or not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:296
+#: lino_welfare/modlib/welfare/help_texts.py:130
 msgid ""
-"The amount to refund for children (household members less than lino_xl.lib."
-"households.Plugin.adult_age years old)."
+"The amount to refund for children (household members less than "
+"lino_xl.lib.households.Plugin.adult_age years old)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:299
+#: lino_welfare/modlib/welfare/help_texts.py:131
 msgid ""
-"The amount to refund for children (household members who are lino_xl.lib."
-"households.Plugin.adult_age years or older)."
+"The amount to refund for children (household members who are "
+"lino_xl.lib.households.Plugin.adult_age years or older)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:302
+#: lino_welfare/modlib/welfare/help_texts.py:132
 msgid "The full name of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:304
+#: lino_welfare/modlib/welfare/help_texts.py:133
 msgid ""
-"The amount to pay. This is either child_tariff or adult_tarif depending on the "
-"age of the household member."
+"The amount to pay. This is either child_tariff or adult_tarif depending "
+"on the age of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:307
+#: lino_welfare/modlib/welfare/help_texts.py:134
 msgid "Model mixin for all integration contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:309
+#: lino_welfare/modlib/welfare/help_texts.py:135
 msgid "The person who created this contract."
 msgstr "Die Person, die diesen Vertrag erstellt hat."
 
-#: lino_welfare/modlib/welfare/help_texts.py:311
+#: lino_welfare/modlib/welfare/help_texts.py:136
 msgid "The responsible person at the general social service."
 msgstr "Die verantwortliche Person im allgemeinen Sozialdienst."
 
-#: lino_welfare/modlib/welfare/help_texts.py:313
+#: lino_welfare/modlib/welfare/help_texts.py:137
 msgid "The client for whom this contract is done."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:315
+#: lino_welfare/modlib/welfare/help_texts.py:138
 msgid "The start date of the contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:317
+#: lino_welfare/modlib/welfare/help_texts.py:139
 msgid "The planned end date of this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:319
+#: lino_welfare/modlib/welfare/help_texts.py:140
 msgid ""
-"The date when this contract was effectively ended. This field is set to the "
-"same value as applies_until."
+"The date when this contract was effectively ended. This field is set to "
+"the same value as applies_until."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:322
+#: lino_welfare/modlib/welfare/help_texts.py:141
 msgid "The reason of prematured ending. Pointer to ContractEnding"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:324
+#: lino_welfare/modlib/welfare/help_texts.py:142
 msgid "When the contract was issued to the client and signed by them."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:326
+#: lino_welfare/modlib/welfare/help_texts.py:143
 msgid "When the contract was ratified by the responsible board."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:328
+#: lino_welfare/modlib/welfare/help_texts.py:144
 msgid "The language of this contract. Default value is the client’s language."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:331
+#: lino_welfare/modlib/welfare/help_texts.py:145
 msgid "The type of this contract. Pointer to a subclass of ContractTypeBase."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:334
+#: lino_welfare/modlib/welfare/help_texts.py:146
 msgid ""
-"The printed title of a contract specifies just the contract type (not the "
-"number and name of client)."
+"The printed title of a contract specifies just the contract type (not the"
+" number and name of client)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:337
+#: lino_welfare/modlib/welfare/help_texts.py:147
 msgid "Overrides lino_xl.lib.excerpts.Certifiable.get_excerpt_templates()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:340
+#: lino_welfare/modlib/welfare/help_texts.py:148
 msgid ""
-"If the contract’s author is the client’s primary coach, then set user_asd to "
-"None, otherwise set user_asd to the primary coach. We no longer suppose that "
-"only integration agents write contracts."
+"If the contract’s author is the client’s primary coach, then set user_asd"
+" to None, otherwise set user_asd to the primary coach. We no longer "
+"suppose that only integration agents write contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:343
+#: lino_welfare/modlib/welfare/help_texts.py:149
 msgid "Checks for the following error conditions:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:345
+#: lino_welfare/modlib/welfare/help_texts.py:150
 msgid ""
-"Returns the last aid confirmation that has been issued for this contract. May "
-"be used in .odt template."
+"Returns the last aid confirmation that has been issued for this contract."
+" May be used in .odt template."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:348
+#: lino_welfare/modlib/welfare/help_texts.py:151
 msgid ""
-"Automatic evaluation events have the client as mandatory participant, plus "
-"possibly some other coach."
+"Automatic evaluation events have the client as mandatory participant, "
+"plus possibly some other coach."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:351
+#: lino_welfare/modlib/welfare/help_texts.py:152
 msgid ""
-"All contracts of a demo project (not only one) are being printed. Overrides "
-"lino.modlib.printing.Printable.get_printable_demo_objects()."
+"All contracts of a demo project (not only one) are being printed. "
+"Overrides lino.modlib.printing.Printable.get_printable_demo_objects()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:354
+#: lino_welfare/modlib/welfare/help_texts.py:153
 msgid "Model mixin for integration contracts that have a single partner."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:356
+#: lino_welfare/modlib/welfare/help_texts.py:154
 msgid "Base for contract tables. Defines the following parameter fields:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:358
+#: lino_welfare/modlib/welfare/help_texts.py:155
 #, fuzzy
 msgid "See ContractEvents."
 msgstr "erlaubt in Verträgen"
 
-#: lino_welfare/modlib/welfare/help_texts.py:360
+#: lino_welfare/modlib/welfare/help_texts.py:156
 msgid "Show only contracts with the specified ContractEnding."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:362
+#: lino_welfare/modlib/welfare/help_texts.py:157
 msgid ""
-"Select “Yes” to show only contracts whose ending ContractEnding has is_success "
-"checked."
+"Select “Yes” to show only contracts whose ending ContractEnding has "
+"is_success checked."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:365
+#: lino_welfare/modlib/welfare/help_texts.py:158
 msgid "The Django model representing an ISIP."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:367
+#: lino_welfare/modlib/welfare/help_texts.py:159
 msgid "The type of this contract. Pointer to ContractType."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:369
+#: lino_welfare/modlib/welfare/help_texts.py:160
 msgid "The type of study that is going to be followed during this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:372
+#: lino_welfare/modlib/welfare/help_texts.py:161
 msgid "The table of all ISIP contract types."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:374
+#: lino_welfare/modlib/welfare/help_texts.py:162
 msgid "The type of a Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:376
+#: lino_welfare/modlib/welfare/help_texts.py:163
 msgid "Whether contracts of this type need their study_type field filled in."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:379
+#: lino_welfare/modlib/welfare/help_texts.py:164
 msgid "Django model to represent an examination policy."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:381
+#: lino_welfare/modlib/welfare/help_texts.py:165
 msgid "A possible reason for premature termination of a contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:383
+#: lino_welfare/modlib/welfare/help_texts.py:166
 msgid ""
-"Represents a third-party external partner who participates in this contract. "
-"For every partner there is a rich text field describing their duties."
+"Represents a third-party external partner who participates in this "
+"contract. For every partner there is a rich text field describing their "
+"duties."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:386
+#: lino_welfare/modlib/welfare/help_texts.py:167
 msgid ""
-"A list of observable events for filtering contracts (ContractBaseTable."
-"observed_event)."
+"A list of observable events for filtering contracts "
+"(ContractBaseTable.observed_event)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:389
+#: lino_welfare/modlib/welfare/help_texts.py:168
 msgid ""
-"Whether the client has at least one ISIP contact during the observed date range."
+"Whether the client has at least one ISIP contact during the observed date"
+" range."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:392
+#: lino_welfare/modlib/welfare/help_texts.py:169
 msgid "To see this table you need either IntegrationAgent or SocialCoordinator."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:395
+#: lino_welfare/modlib/welfare/help_texts.py:170
 msgid "Base class for all ContractType models."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:397
+#: lino_welfare/modlib/welfare/help_texts.py:171
 msgid "The full description of this contract type as used in printed documents."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:400
+#: lino_welfare/modlib/welfare/help_texts.py:172
 msgid "The default examination policy to be used for contracts of this type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:403
+#: lino_welfare/modlib/welfare/help_texts.py:173
 msgid ""
-"The overlap group to use when checking whether two contracts are overlapping or "
-"not. If this field is empty, Lino does not check at all for overlapping "
-"contracts."
+"The overlap group to use when checking whether two contracts are "
+"overlapping or not. If this field is empty, Lino does not check at all "
+"for overlapping contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:406
+#: lino_welfare/modlib/welfare/help_texts.py:174
 msgid ""
-"The main template to use instead of the default template defined on the excerpt "
-"type."
+"The main template to use instead of the default template defined on the "
+"excerpt type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:409
+#: lino_welfare/modlib/welfare/help_texts.py:175
 msgid ""
-"The list of all known overlap groups to be selected for the overlap_group of a "
-"contract type."
+"The list of all known overlap groups to be selected for the overlap_group"
+" of a contract type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:412
+#: lino_welfare/modlib/welfare/help_texts.py:176
 msgid ""
-"Volatile object used to test for overlapping contracts. It is responsible for "
-"issuing the following error messages:"
+"Volatile object used to test for overlapping contracts. It is responsible"
+" for issuing the following error messages:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:415
+#: lino_welfare/modlib/welfare/help_texts.py:177
 msgid "A given client cannot have two active contracts at the same time."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:417
+#: lino_welfare/modlib/welfare/help_texts.py:178
 msgid ""
 "Organisation bénéficiant de l’agrément « Initiative d’économie sociale » "
 "octroyé par la Wallonie."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:420
+#: lino_welfare/modlib/welfare/help_texts.py:179
 #, fuzzy
 msgid "Shows all Art60 job supplyments."
 msgstr "Art.60§7-Konvention"
 
-#: lino_welfare/modlib/welfare/help_texts.py:422
+#: lino_welfare/modlib/welfare/help_texts.py:180
 #, fuzzy
 msgid "Shows the Art60 job supplyments for this client."
 msgstr "Art.61-Konventionsart"
 
-#: lino_welfare/modlib/welfare/help_texts.py:424
+#: lino_welfare/modlib/welfare/help_texts.py:181
 msgid ""
-"Model mixin for jobs.Contract and art61.Contract. And also for art60.Contract."
+"Model mixin for jobs.Contract and art61.Contract. And also for "
+"art60.Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:427
+#: lino_welfare/modlib/welfare/help_texts.py:182
 msgid "The duration of this job supplyment (number of working days)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:429
+#: lino_welfare/modlib/welfare/help_texts.py:183
 msgid "Django model used to represent a beneficiary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:431
+#: lino_welfare/modlib/welfare/help_texts.py:184
 msgid "Whether Lino should make ESF summaries for this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:433
+#: lino_welfare/modlib/welfare/help_texts.py:185
 msgid "A panel with general information about this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:435
+#: lino_welfare/modlib/welfare/help_texts.py:186
 msgid ""
 "A virtual field displaying a group of shortcut links for managing CVs "
 "(Curriculum Vitaes)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:438
+#: lino_welfare/modlib/welfare/help_texts.py:187
 msgid ""
-"A virtual field displaying a group of buttons for managing the “identifying "
-"document”, i.e. an uploaded document which has been used as alternative to the "
-"eID card."
+"A virtual field displaying a group of buttons for managing the "
+"“identifying document”, i.e. an uploaded document which has been used as "
+"alternative to the eID card."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:441
+#: lino_welfare/modlib/welfare/help_texts.py:188
 msgid "Pointer to PersonGroup. The intergration phase of this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:443
+#: lino_welfare/modlib/welfare/help_texts.py:189
 msgid "The civil state of this client. Allowed choices are defined in CivilState."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:446
+#: lino_welfare/modlib/welfare/help_texts.py:190
 #, fuzzy
 msgid "Pointer to ClientStates."
 msgstr "DSBE-Klienten"
 
-#: lino_welfare/modlib/welfare/help_texts.py:448
+#: lino_welfare/modlib/welfare/help_texts.py:191
 msgid ""
-"The date when this client got unemployed and stopped to have a regular work."
+"The date when this client got unemployed and stopped to have a regular "
+"work."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:451
+#: lino_welfare/modlib/welfare/help_texts.py:192
 msgid ""
-"The date when this client registered as unemployed and started to look for a "
-"new job."
+"The date when this client registered as unemployed and started to look "
+"for a new job."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:454
+#: lino_welfare/modlib/welfare/help_texts.py:193
 msgid ""
-"Return the last note of type “First meeting” for this client. Usage example see "
-"debts and notes."
+"Return the last note of type “First meeting” for this client. Usage "
+"example see debts and notes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:457
+#: lino_welfare/modlib/welfare/help_texts.py:194
 #, fuzzy
 msgid "The list that opens by Contacts ‣ Clients."
 msgstr "Liste der Klientenkontakte"
 
-#: lino_welfare/modlib/welfare/help_texts.py:459
+#: lino_welfare/modlib/welfare/help_texts.py:195
 msgid ""
-"If not empty, show only Clients whose client_state equals the specified value."
+"If not empty, show only Clients whose client_state equals the specified "
+"value."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:462
+#: lino_welfare/modlib/welfare/help_texts.py:196
 msgid "Displays the response of an RetrieveTIGroupsRequest as a table."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:464
+#: lino_welfare/modlib/welfare/help_texts.py:197
 msgid "The Django database model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:466
+#: lino_welfare/modlib/welfare/help_texts.py:198
 msgid "Yield a list of all subsidizations activated for this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:468
+#: lino_welfare/modlib/welfare/help_texts.py:199
 #, fuzzy
 msgid "Shows the Art61 job supplyments for this client."
 msgstr "Art.61-Konventionsart"
 
 #: lino_welfare/modlib/welfare/models.py:35
 msgid "Local job office"
 msgstr "Lokales Arbeitsamt"
@@ -4561,15 +4635,16 @@
 
 #: lino_welfare/modlib/welfare/models.py:71
 msgid "usable in contracts"
 msgstr "erlaubt in Verträgen"
 
 #: lino_welfare/modlib/welfare/models.py:73
 msgid ""
-"Whether Links of this type can be used as contact person of a job contract."
+"Whether Links of this type can be used as contact person of a job "
+"contract."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/user_types.py:155
 msgid "Anonymous"
 msgstr "Anonym"
 
 #: lino_welfare/modlib/welfare/user_types.py:160
@@ -4731,31 +4806,31 @@
 msgid "Dentist"
 msgstr "Zahnarzt"
 
 #: lino_welfare/modlib/welfare/fixtures/demo.py:781
 msgid "Pediatrician"
 msgstr "Kinderarzt"
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:987
+#: lino_welfare/modlib/welfare/fixtures/demo.py:993
 msgid "A very hard job."
 msgstr "Sehr harte Stelle"
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:988
+#: lino_welfare/modlib/welfare/fixtures/demo.py:994
 msgid "No supervisor. Only for independent people."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:1197
+#: lino_welfare/modlib/welfare/fixtures/demo.py:1215
 msgid "Urgent problem"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:1197
+#: lino_welfare/modlib/welfare/fixtures/demo.py:1215
 msgid "Complain"
 msgstr "Beschwerde"
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:1197
+#: lino_welfare/modlib/welfare/fixtures/demo.py:1215
 #, fuzzy
 msgid "Information"
 msgstr "Ausbildung"
 
 #: lino_welfare/modlib/welfare/fixtures/std.py:83
 msgid "Normal"
 msgstr "Normal"
@@ -4930,27 +5005,27 @@
 msgid "The course which satisfies this request. Leave blank on open requests."
 msgstr ""
 
 #: lino_welfare/modlib/xcourses/models.py:352
 msgid "Course found"
 msgstr "Kurs gefunden"
 
-#: lino_welfare/modlib/xcourses/models.py:496
+#: lino_welfare/modlib/xcourses/models.py:497
 msgid "Participants"
 msgstr "Teilnehmer"
 
-#: lino_welfare/modlib/xcourses/models.py:534
+#: lino_welfare/modlib/xcourses/models.py:535
 msgid "Pending Course Requests"
 msgstr "Offene Kursanfragen"
 
-#: lino_welfare/modlib/xcourses/models.py:600
+#: lino_welfare/modlib/xcourses/models.py:601
 msgid "Age"
 msgstr "Alter"
 
-#: lino_welfare/modlib/xcourses/models.py:614
+#: lino_welfare/modlib/xcourses/models.py:615
 msgid "unknown age"
 msgstr "unbek. Alter"
 
 #~ msgid "reason"
 #~ msgstr "Begründung"
 
 #~ msgid "eID card expires"
@@ -5026,7 +5101,8 @@
 #~ msgstr "Auch veraltete Daten"
 
 #~ msgid "Show also obsolete records."
 #~ msgstr "Auch veraltete Daten"
 
 #~ msgid "Art61 job supplyments and activations"
 #~ msgstr "Art.61-Konventionsarten"
+
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: lino_welfare\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-03-03 16:31+0200\n"
+"PO-Revision-Date: 2024-04-30 13:49+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
 "Language-Team: fr <info@lino-framework.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n>1;\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 "X-Generator: Poedit 3.0.1\n"
 
 msgid " and "
 msgstr " et "
 
 msgid " born "
 msgstr " né(e) "
@@ -1547,15 +1547,15 @@
 msgid "Success"
 msgstr "Réussi"
 
 msgid "Successfully ended"
 msgstr "Terminé avec succès"
 
 msgid "Summary"
-msgstr "Sommaire"
+msgstr "Résumé"
 
 msgid "Technical"
 msgstr "Technique"
 
 msgid "Temporary absences"
 msgstr "Absences temporaires"
 
@@ -1666,14 +1666,20 @@
 
 msgid "Work Schedule"
 msgstr "Horaire"
 
 msgid "Work Schedules"
 msgstr "Horaires"
 
+msgid "Workplace"
+msgstr "Lieu de travail"
+
+msgid "Workplaces"
+msgstr "Lieux de travail"
+
 msgid "Yearly amount"
 msgstr "Montant annuel"
 
 msgid "Yearly incomes ({0} / 12)"
 msgstr "Revenus annuels ({0} / 12)"
 
 msgid "Yes/Maybe/No"
@@ -1897,15 +1903,15 @@
 msgid "suspended until"
 msgstr "Suspendu jusque"
 
 msgid "unknown age"
 msgstr "age inconnu"
 
 msgid "until"
-msgstr "jusque"
+msgstr "au"
 
 msgid "until "
 msgstr "jusque "
 
 msgid "usable in contracts"
 msgstr "utilisable dans contrats"
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: lino_welfare\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-02-20 10:31+0200\n"
-"PO-Revision-Date: 2024-03-03 16:31+0200\n"
+"POT-Creation-Date: 2024-04-30 13:49+0300\n"
+"PO-Revision-Date: 2024-04-30 13:49+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
 "Language-Team: fr <info@lino-framework.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n>1;\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 "X-Generator: Poedit 3.0.1\n"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:18
 msgid "Active Job Search"
 msgstr "Recherche active d'emploi"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:19
@@ -33,21 +33,21 @@
 msgstr "Preuve de recherche"
 
 #: lino_welfare/modlib/active_job_search/models.py:23
 msgid "Proofs of search"
 msgstr "Preuves de recherche"
 
 #: lino_welfare/modlib/active_job_search/models.py:27
-#: lino_welfare/modlib/badges/models.py:38 lino_welfare/modlib/cal/models.py:348
+#: lino_welfare/modlib/badges/models.py:38 lino_welfare/modlib/cal/models.py:347
 #: lino_welfare/modlib/cbss/tx25.py:315 lino_welfare/modlib/cbss/tx25.py:362
 #: lino_welfare/modlib/cbss/tx25.py:371 lino_welfare/modlib/cbss/tx25.py:383
 #: lino_welfare/modlib/cbss/tx25.py:476 lino_welfare/modlib/cbss/tx25.py:488
 #: lino_welfare/modlib/debts/models.py:104 lino_welfare/modlib/isip/models.py:376
-#: lino_welfare/modlib/jobs/ui.py:416 lino_welfare/modlib/jobs/ui.py:536
-#: lino_welfare/modlib/pcsw/models.py:1046
+#: lino_welfare/modlib/jobs/ui.py:430 lino_welfare/modlib/jobs/ui.py:550
+#: lino_welfare/modlib/pcsw/models.py:1048
 msgid "Date"
 msgstr ""
 
 #: lino_welfare/modlib/active_job_search/models.py:29
 msgid "Spontaneous"
 msgstr "Spontanée"
 
@@ -73,15 +73,15 @@
 msgstr "Garde d'enfant"
 
 #: lino_welfare/modlib/active_job_search/models.py:76
 msgid "Notes concerning child custody."
 msgstr ""
 
 #: lino_welfare/modlib/aids/__init__.py:13 lino_welfare/modlib/ledger/models.py:49
-#: lino_welfare/modlib/pcsw/models.py:531
+#: lino_welfare/modlib/pcsw/models.py:533
 msgid "Aids"
 msgstr "Aides"
 
 #: lino_welfare/modlib/aids/choicelists.py:47
 msgid "Aid confirmation type"
 msgstr "Type de confirmation d'aide"
 
@@ -159,18 +159,18 @@
 msgstr "béneficie d'une aide %(what)s %(when)s."
 
 #: lino_welfare/modlib/aids/mixins.py:217 lino_welfare/modlib/art61/models.py:248
 #: lino_welfare/modlib/badges/models.py:40 lino_welfare/modlib/cv/models.py:46
 #: lino_welfare/modlib/debts/models.py:399 lino_welfare/modlib/debts/models.py:435
 #: lino_welfare/modlib/esf/models.py:37
 #: lino_welfare/modlib/immersion/models.py:102
-#: lino_welfare/modlib/jobs/mixins.py:45 lino_welfare/modlib/jobs/models.py:235
-#: lino_welfare/modlib/jobs/models.py:269 lino_welfare/modlib/jobs/models.py:336
-#: lino_welfare/modlib/jobs/models.py:409 lino_welfare/modlib/pcsw/actions.py:39
-#: lino_welfare/modlib/pcsw/models.py:952 lino_welfare/modlib/pcsw/models.py:1012
+#: lino_welfare/modlib/jobs/mixins.py:45 lino_welfare/modlib/jobs/models.py:237
+#: lino_welfare/modlib/jobs/models.py:279 lino_welfare/modlib/jobs/models.py:350
+#: lino_welfare/modlib/jobs/models.py:423 lino_welfare/modlib/pcsw/actions.py:39
+#: lino_welfare/modlib/pcsw/models.py:954 lino_welfare/modlib/pcsw/models.py:1014
 #: lino_welfare/modlib/projects/models.py:40
 #: lino_welfare/modlib/xcourses/models.py:177
 #: lino_welfare/modlib/xcourses/models.py:354
 msgid "Remark"
 msgstr "Remarque"
 
 #: lino_welfare/modlib/aids/mixins.py:249
@@ -179,17 +179,17 @@
 msgstr "Période %(p1)s hors de la période d'ocroi %(p2)s."
 
 #: lino_welfare/modlib/aids/mixins.py:322 lino_welfare/modlib/cbss/models.py:283
 msgid "Period from"
 msgstr "Période du"
 
 #: lino_welfare/modlib/aids/mixins.py:326 lino_welfare/modlib/aids/models.py:221
-#: lino_welfare/modlib/pcsw/models.py:956 lino_welfare/modlib/pcsw/models.py:1011
+#: lino_welfare/modlib/pcsw/models.py:958 lino_welfare/modlib/pcsw/models.py:1013
 msgid "until"
-msgstr "jusque"
+msgstr "au"
 
 #: lino_welfare/modlib/aids/mixins.py:330
 msgid "Recipient (Organization)"
 msgstr "Destinataire (Organisation)"
 
 #: lino_welfare/modlib/aids/mixins.py:333
 msgid "Recipient (Person)"
@@ -448,25 +448,25 @@
 msgid "Art60 job supplying"
 msgstr "Mise à l'emploi art60"
 
 #: lino_welfare/modlib/art60/models.py:33
 msgid "Art60 job supplyment"
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:48 lino_welfare/modlib/jobs/models.py:116
+#: lino_welfare/modlib/art60/models.py:48 lino_welfare/modlib/jobs/models.py:118
 #: lino_welfare/modlib/jobs/ui.py:37
 msgid "Art60§7 job supplyment"
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:49 lino_welfare/modlib/jobs/models.py:117
+#: lino_welfare/modlib/art60/models.py:49 lino_welfare/modlib/jobs/models.py:119
 msgid "Art60§7 job supplyments"
 msgstr "Mises à l'emploi art60§7"
 
 #: lino_welfare/modlib/art60/models.py:55 lino_welfare/modlib/art61/models.py:76
-#: lino_welfare/modlib/jobs/models.py:131
+#: lino_welfare/modlib/jobs/models.py:133
 #, fuzzy
 msgid "Type"
 msgstr "Type d'aide sociale"
 
 #: lino_welfare/modlib/art60/models.py:85
 msgid "Active convention"
 msgstr "Convention active"
@@ -483,35 +483,35 @@
 msgid "Start date"
 msgstr "Date de début"
 
 #: lino_welfare/modlib/art60/models.py:120 lino_welfare/modlib/art60/models.py:237
 msgid "Monthly refund"
 msgstr "Rétrocession mensuelle"
 
-#: lino_welfare/modlib/art60/models.py:121 lino_welfare/modlib/jobs/models.py:141
-#: lino_welfare/modlib/jobs/models.py:267
+#: lino_welfare/modlib/art60/models.py:121 lino_welfare/modlib/jobs/models.py:143
+#: lino_welfare/modlib/jobs/models.py:277
 msgid "hourly rate"
 msgstr "coût horaire"
 
-#: lino_welfare/modlib/art60/models.py:122 lino_welfare/modlib/jobs/models.py:142
+#: lino_welfare/modlib/art60/models.py:122 lino_welfare/modlib/jobs/models.py:144
 msgid "refund rate"
 msgstr "tarif de remboursement"
 
-#: lino_welfare/modlib/art60/models.py:175 lino_welfare/modlib/jobs/models.py:186
+#: lino_welfare/modlib/art60/models.py:175 lino_welfare/modlib/jobs/models.py:188
 #, python-format
 msgid "(%d candidatures have been marked inactive)"
 msgstr ""
 
 #: lino_welfare/modlib/art60/models.py:177 lino_welfare/modlib/isip/models.py:117
-#: lino_welfare/modlib/jobs/models.py:188 lino_welfare/modlib/pcsw/actions.py:85
+#: lino_welfare/modlib/jobs/models.py:190 lino_welfare/modlib/pcsw/actions.py:85
 #: lino_welfare/modlib/pcsw/actions.py:118
 msgid "Success"
 msgstr "Réussi"
 
-#: lino_welfare/modlib/art60/models.py:241 lino_welfare/modlib/jobs/ui.py:173
+#: lino_welfare/modlib/art60/models.py:241 lino_welfare/modlib/jobs/ui.py:185
 msgid "Only contracts of type"
 msgstr "Uniquement contrats de type"
 
 #: lino_welfare/modlib/art60/models.py:297
 #: lino_welfare/modlib/isip/choicelists.py:27
 msgid "Conventions"
 msgstr "Conventions"
@@ -683,61 +683,61 @@
 msgid "at"
 msgstr "à"
 
 #: lino_welfare/modlib/cal/models.py:186
 msgid "Managed by"
 msgstr "Traîté par"
 
-#: lino_welfare/modlib/cal/models.py:241
+#: lino_welfare/modlib/cal/models.py:240
 msgid "Notes"
 msgstr ""
 
-#: lino_welfare/modlib/cal/models.py:326
+#: lino_welfare/modlib/cal/models.py:325
 #: lino_welfare/modlib/client_vouchers/ui.py:38
 #: lino_welfare/modlib/contacts/models.py:139
 #: lino_welfare/modlib/contacts/models.py:227
-#: lino_welfare/modlib/contacts/models.py:313 lino_welfare/modlib/debts/ui.py:125
+#: lino_welfare/modlib/contacts/models.py:318 lino_welfare/modlib/debts/ui.py:125
 #: lino_welfare/modlib/finan/models.py:19 lino_welfare/modlib/isip/models.py:263
-#: lino_welfare/modlib/system/models.py:103 lino_welfare/modlib/users/ui.py:24
-#: lino_welfare/modlib/welfare/workflows.py:49
+#: lino_welfare/modlib/jobs/ui.py:74 lino_welfare/modlib/system/models.py:103
+#: lino_welfare/modlib/users/ui.py:24 lino_welfare/modlib/welfare/workflows.py:49
 msgid "General"
 msgstr "Général"
 
-#: lino_welfare/modlib/cal/models.py:331 lino_welfare/modlib/finan/models.py:25
+#: lino_welfare/modlib/cal/models.py:330 lino_welfare/modlib/finan/models.py:25
 msgid "More"
 msgstr "Plus"
 
-#: lino_welfare/modlib/cal/models.py:346
+#: lino_welfare/modlib/cal/models.py:345
 #: lino_welfare/modlib/integ/fixtures/std.py:30
 msgid "Appointment"
 msgstr "Rendez-vous"
 
-#: lino_welfare/modlib/cal/models.py:352
+#: lino_welfare/modlib/cal/models.py:351
 msgid "Summary"
-msgstr "Sommaire"
+msgstr "Résumé"
 
-#: lino_welfare/modlib/cal/models.py:367
+#: lino_welfare/modlib/cal/models.py:366
 #, python-format
 msgid "Created appointment for %(user)s with %(partner)s"
 msgstr ""
 
-#: lino_welfare/modlib/cal/models.py:408
+#: lino_welfare/modlib/cal/models.py:407
 #, fuzzy
 msgid "Task"
 msgstr "état"
 
-#: lino_welfare/modlib/cal/models.py:409
+#: lino_welfare/modlib/cal/models.py:408
 msgid "Tasks"
 msgstr ""
 
-#: lino_welfare/modlib/cal/models.py:412
+#: lino_welfare/modlib/cal/models.py:411
 msgid "Delegated to client"
 msgstr "à faire par bénéficiaire"
 
-#: lino_welfare/modlib/cbss/__init__.py:37 lino_welfare/modlib/pcsw/models.py:419
+#: lino_welfare/modlib/cbss/__init__.py:37 lino_welfare/modlib/pcsw/models.py:421
 msgid "CBSS"
 msgstr "BCSS"
 
 #: lino_welfare/modlib/cbss/choicelists.py:20
 #: lino_welfare/modlib/cbss/mixins.py:74
 msgid "Sent"
 msgstr "Exécuté"
@@ -927,15 +927,15 @@
 msgid "Tx25 Request"
 msgstr "Requête Tx25"
 
 #: lino_welfare/modlib/cbss/models.py:410
 msgid "Tx25 Requests"
 msgstr "Requêtes Tx25"
 
-#: lino_welfare/modlib/cbss/models.py:415 lino_welfare/modlib/pcsw/models.py:539
+#: lino_welfare/modlib/cbss/models.py:415 lino_welfare/modlib/pcsw/models.py:541
 msgid "History"
 msgstr "Historique"
 
 #: lino_welfare/modlib/cbss/models.py:562
 msgid "Requesting organisation"
 msgstr ""
 
@@ -1097,15 +1097,15 @@
 msgstr ""
 
 #: lino_welfare/modlib/cbss/tx25.py:710 lino_welfare/modlib/cbss/tx25.py:752
 msgid "SSIN "
 msgstr "NISS "
 
 #: lino_welfare/modlib/cbss/tx25.py:730 lino_welfare/modlib/immersion/models.py:86
-#: lino_welfare/modlib/isip/models.py:150 lino_welfare/modlib/jobs/models.py:125
+#: lino_welfare/modlib/isip/models.py:150 lino_welfare/modlib/jobs/models.py:127
 msgid "Organization"
 msgstr "Organisation"
 
 #: lino_welfare/modlib/cbss/tx25.py:811 lino_welfare/modlib/isip/models.py:54
 msgid "Reference"
 msgstr "Référence"
 
@@ -1348,15 +1348,15 @@
 msgstr "Permis de conduire"
 
 #: lino_welfare/modlib/cbss/tx25.py:1211
 msgid "Identity Cards"
 msgstr "Cartes d'identité"
 
 #: lino_welfare/modlib/cbss/tx25.py:1228 lino_welfare/modlib/pcsw/models.py:131
-#: lino_welfare/modlib/pcsw/models.py:951 lino_welfare/modlib/pcsw/models.py:1003
+#: lino_welfare/modlib/pcsw/models.py:953 lino_welfare/modlib/pcsw/models.py:1005
 #: lino_welfare/modlib/reception/models.py:106
 #: lino_welfare/modlib/reception/models.py:133
 msgid "Reason"
 msgstr "Raison"
 
 #: lino_welfare/modlib/cbss/tx25.py:1241
 msgid "Legal cohabitations"
@@ -1431,15 +1431,15 @@
 msgid "Birth location"
 msgstr "Lieu de naissance"
 
 #: lino_welfare/modlib/cbss/ui.py:208
 msgid "Civil state"
 msgstr "Etat civil"
 
-#: lino_welfare/modlib/cbss/ui.py:212 lino_welfare/modlib/xcourses/models.py:604
+#: lino_welfare/modlib/cbss/ui.py:212 lino_welfare/modlib/xcourses/models.py:605
 msgid "Address"
 msgstr "Adresse"
 
 #: lino_welfare/modlib/cbss/ui.py:223 lino_welfare/modlib/cbss/ui.py:245
 msgid "Requested action"
 msgstr "Action demandée"
 
@@ -1490,28 +1490,28 @@
 
 #: lino_welfare/modlib/contacts/models.py:118
 msgid "Cannot delete companies and persons imported from TIM"
 msgstr "On ne peut effacer les sociétés et les personnes importées de TIM"
 
 #: lino_welfare/modlib/contacts/models.py:159
 #: lino_welfare/modlib/contacts/models.py:247
-#: lino_welfare/modlib/contacts/models.py:332
+#: lino_welfare/modlib/contacts/models.py:337
 msgid "Contact"
 msgstr "Contact"
 
 #: lino_welfare/modlib/contacts/models.py:172
 #: lino_welfare/modlib/contacts/models.py:260
-#: lino_welfare/modlib/contacts/models.py:347
-#: lino_welfare/modlib/pcsw/models.py:561
+#: lino_welfare/modlib/contacts/models.py:352
+#: lino_welfare/modlib/pcsw/models.py:563
 msgid "Miscellaneous"
 msgstr "Divers"
 
 #: lino_welfare/modlib/contacts/models.py:181
 #: lino_welfare/modlib/households/models.py:80
-#: lino_welfare/modlib/pcsw/models.py:468
+#: lino_welfare/modlib/pcsw/models.py:470
 msgid "Person"
 msgstr "Personne"
 
 #: lino_welfare/modlib/contacts/models.py:182
 msgid "Persons"
 msgstr "Personnes"
 
@@ -2257,15 +2257,15 @@
 msgstr "Disponible"
 
 #: lino_welfare/modlib/integ/models.py:77
 msgid "Integration Clients"
 msgstr "Bénéficiares (SI)"
 
 #: lino_welfare/modlib/integ/models.py:106 lino_welfare/modlib/pcsw/models.py:88
-#: lino_welfare/modlib/pcsw/models.py:867
+#: lino_welfare/modlib/pcsw/models.py:869
 msgid "Integration phase"
 msgstr "Phase d'insertion"
 
 #: lino_welfare/modlib/integ/models.py:108
 msgid "Language knowledge"
 msgstr "Connaissance de langue"
 
@@ -2554,16 +2554,16 @@
 msgid "Reason of termination"
 msgstr "Motif d'arrêt"
 
 #: lino_welfare/modlib/isip/models.py:112
 msgid "Contract termination reasons"
 msgstr "Motifs d’arrêt de contrat"
 
-#: lino_welfare/modlib/isip/models.py:114 lino_welfare/modlib/jobs/models.py:407
-#: lino_welfare/modlib/pcsw/models.py:871 lino_welfare/modlib/pcsw/models.py:1048
+#: lino_welfare/modlib/isip/models.py:114 lino_welfare/modlib/jobs/models.py:421
+#: lino_welfare/modlib/pcsw/models.py:873 lino_welfare/modlib/pcsw/models.py:1050
 msgid "Designation"
 msgstr "Désignation"
 
 #: lino_welfare/modlib/isip/models.py:118
 #, fuzzy
 msgid "Require date ended"
 msgstr "Date de fin"
@@ -2580,15 +2580,15 @@
 msgid "duties company"
 msgstr "Obligations de l'entreprise"
 
 #: lino_welfare/modlib/isip/models.py:188
 msgid "ISIPs"
 msgstr "PIISs"
 
-#: lino_welfare/modlib/isip/models.py:192 lino_welfare/modlib/jobs/models.py:264
+#: lino_welfare/modlib/isip/models.py:192 lino_welfare/modlib/jobs/models.py:274
 msgid "Contract Type"
 msgstr "Type de contrat"
 
 #: lino_welfare/modlib/isip/models.py:197
 msgid "stages"
 msgstr "stages"
 
@@ -2639,23 +2639,23 @@
 msgstr "États de candidatures"
 
 #: lino_welfare/modlib/jobs/mixins.py:26
 msgctxt "jobs"
 msgid "Active"
 msgstr "Actifs"
 
-#: lino_welfare/modlib/jobs/mixins.py:27 lino_welfare/modlib/jobs/ui.py:443
+#: lino_welfare/modlib/jobs/mixins.py:27 lino_welfare/modlib/jobs/ui.py:457
 msgid "Probation"
 msgstr "période d'essai"
 
 #: lino_welfare/modlib/jobs/mixins.py:28
 msgid "Probation failed"
 msgstr "Abandon du stage"
 
-#: lino_welfare/modlib/jobs/mixins.py:29 lino_welfare/modlib/jobs/ui.py:435
+#: lino_welfare/modlib/jobs/mixins.py:29 lino_welfare/modlib/jobs/ui.py:449
 msgctxt "jobs"
 msgid "Working"
 msgstr "Travaille"
 
 #: lino_welfare/modlib/jobs/mixins.py:30
 msgctxt "jobs"
 msgid "Inactive"
@@ -2678,15 +2678,15 @@
 msgstr "Service utilisateur"
 
 #: lino_welfare/modlib/jobs/models.py:52
 msgid "Job providers"
 msgstr "Services utilisateurs"
 
 #: lino_welfare/modlib/jobs/models.py:54 lino_welfare/modlib/jobs/models.py:70
-#: lino_welfare/modlib/jobs/models.py:410
+#: lino_welfare/modlib/jobs/models.py:424
 msgid "Social economy"
 msgstr "Économie sociale"
 
 #: lino_welfare/modlib/jobs/models.py:67
 msgid "Employer"
 msgstr "Employeur"
 
@@ -2698,103 +2698,107 @@
 msgid "Art60§7 job supplyment type"
 msgstr "Type de mise à l'emploi art60§7"
 
 #: lino_welfare/modlib/jobs/models.py:92
 msgid "Art60§7 job supplyment types"
 msgstr "Types de mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/jobs/models.py:218
+#: lino_welfare/modlib/jobs/models.py:220
 msgid "Job Offer"
 msgstr "Offre d'emploi"
 
-#: lino_welfare/modlib/jobs/models.py:219
+#: lino_welfare/modlib/jobs/models.py:221
 msgid "Job Offers"
 msgstr "Offres d'emploi"
 
-#: lino_welfare/modlib/jobs/models.py:222 lino_welfare/modlib/jobs/models.py:257
+#: lino_welfare/modlib/jobs/models.py:224 lino_welfare/modlib/jobs/models.py:259
 #: lino_welfare/modlib/xcourses/models.py:71
 #: lino_welfare/modlib/xcourses/models.py:99
 #: lino_welfare/modlib/xcourses/models.py:170
 msgid "Name"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:226
+#: lino_welfare/modlib/jobs/models.py:228
 msgid "selection from"
 msgstr "Début de sélection"
 
-#: lino_welfare/modlib/jobs/models.py:229
+#: lino_welfare/modlib/jobs/models.py:231
 msgid "selection until"
 msgstr "Fin de sélection"
 
-#: lino_welfare/modlib/jobs/models.py:232
+#: lino_welfare/modlib/jobs/models.py:234
 #: lino_welfare/modlib/xcourses/models.py:172
 msgid "start date"
 msgstr "Date de début"
 
-#: lino_welfare/modlib/jobs/models.py:253 lino_welfare/modlib/jobs/ui.py:424
+#: lino_welfare/modlib/jobs/models.py:255 lino_welfare/modlib/jobs/ui.py:438
 msgid "Job"
 msgstr "Poste de travail"
 
-#: lino_welfare/modlib/jobs/models.py:254 lino_welfare/modlib/jobs/ui.py:82
-#: lino_welfare/modlib/jobs/ui.py:103
+#: lino_welfare/modlib/jobs/models.py:256 lino_welfare/modlib/jobs/ui.py:87
+#: lino_welfare/modlib/jobs/ui.py:115
 msgid "Jobs"
 msgstr "Postes de travail"
 
-#: lino_welfare/modlib/jobs/models.py:259 lino_welfare/modlib/jobs/models.py:402
+#: lino_welfare/modlib/jobs/models.py:261 lino_welfare/modlib/jobs/models.py:416
 msgid "Job Type"
 msgstr "Type de poste"
 
-#: lino_welfare/modlib/jobs/models.py:268
+#: lino_welfare/modlib/jobs/models.py:267
+msgid "Workplace"
+msgstr "Lieu de travail"
+
+#: lino_welfare/modlib/jobs/models.py:278
 msgid "capacity"
 msgstr "Capacité"
 
-#: lino_welfare/modlib/jobs/models.py:273
+#: lino_welfare/modlib/jobs/models.py:283
 #, python-format
 msgid "%(job)s at %(provider)s"
 msgstr "%(job)s chez %(provider)s"
 
-#: lino_welfare/modlib/jobs/models.py:324
+#: lino_welfare/modlib/jobs/models.py:338
 msgid "Job Candidature"
 msgstr "Candidature"
 
-#: lino_welfare/modlib/jobs/models.py:325
+#: lino_welfare/modlib/jobs/models.py:339
 msgid "Job Candidatures"
 msgstr "Candidatures"
 
-#: lino_welfare/modlib/jobs/models.py:333
+#: lino_welfare/modlib/jobs/models.py:347
 #: lino_welfare/modlib/xcourses/models.py:334
 msgid "date submitted"
 msgstr "Date déntrée"
 
-#: lino_welfare/modlib/jobs/models.py:334
+#: lino_welfare/modlib/jobs/models.py:348
 msgid "Date when the IA introduced this candidature."
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:341
+#: lino_welfare/modlib/jobs/models.py:355
 msgid "Art.60"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:343
+#: lino_welfare/modlib/jobs/models.py:357
 msgid "Whether an art.60 contract can satisfy this candidature."
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:347
+#: lino_welfare/modlib/jobs/models.py:361
 msgid "Art.61"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:349
+#: lino_welfare/modlib/jobs/models.py:363
 msgid "Whether an art.61 contract can satisfy this candidature."
 msgstr ""
 
-#: lino_welfare/modlib/jobs/models.py:374
+#: lino_welfare/modlib/jobs/models.py:388
 #, python-format
 msgid "Candidature by %(person)s"
 msgstr "Candidatures par %(person)s"
 
-#: lino_welfare/modlib/jobs/models.py:403
+#: lino_welfare/modlib/jobs/models.py:417
 msgid "Job Types"
 msgstr "Types de poste"
 
 #: lino_welfare/modlib/jobs/template_messages.py:6
 msgid "Renseignements généraux"
 msgstr ""
 
@@ -2802,36 +2806,40 @@
 msgid "Situation financière"
 msgstr ""
 
 #: lino_welfare/modlib/jobs/template_messages.py:9
 msgid "Nom du médiateur de dettes"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/ui.py:88
+#: lino_welfare/modlib/jobs/ui.py:93
 msgid "Documents"
 msgstr ""
 
-#: lino_welfare/modlib/jobs/ui.py:256
+#: lino_welfare/modlib/jobs/ui.py:105
+msgid "Workplaces"
+msgstr "Lieux de travail"
+
+#: lino_welfare/modlib/jobs/ui.py:268
 msgid "Job Contracts Search"
 msgstr "Recherche contrats de travail"
 
-#: lino_welfare/modlib/jobs/ui.py:359 lino_welfare/modlib/jobs/ui.py:439
-#: lino_welfare/modlib/xcourses/models.py:506
+#: lino_welfare/modlib/jobs/ui.py:371 lino_welfare/modlib/jobs/ui.py:453
+#: lino_welfare/modlib/xcourses/models.py:507
 msgid "Candidates"
 msgstr "Candidats"
 
-#: lino_welfare/modlib/jobs/ui.py:365
+#: lino_welfare/modlib/jobs/ui.py:377
 msgid "Experiences"
 msgstr "Expériences professionnelles"
 
-#: lino_welfare/modlib/jobs/ui.py:411 lino_welfare/modlib/jobs/ui.py:533
+#: lino_welfare/modlib/jobs/ui.py:425 lino_welfare/modlib/jobs/ui.py:547
 msgid "Contracts Situation"
 msgstr "Situation contrats Art 60-7"
 
-#: lino_welfare/modlib/jobs/ui.py:427
+#: lino_welfare/modlib/jobs/ui.py:441
 msgctxt "(place)"
 msgid " at "
 msgstr " chez "
 
 #: lino_welfare/modlib/ledger/models.py:15
 msgid "Disbursement orders to execute"
 msgstr "Mandats à exécuter"
@@ -3000,47 +3008,47 @@
 msgstr ""
 
 #: lino_welfare/modlib/newcomers/models.py:123
 msgid "Competence"
 msgstr "Compétence"
 
 #: lino_welfare/modlib/newcomers/models.py:124
-#: lino_welfare/modlib/pcsw/models.py:582
+#: lino_welfare/modlib/pcsw/models.py:584
 msgid "Competences"
 msgstr "Compétences"
 
 #: lino_welfare/modlib/newcomers/models.py:143
 #, fuzzy
 msgid "User"
 msgstr "Refuser"
 
 #: lino_welfare/modlib/newcomers/models.py:213
 #: lino_welfare/modlib/newcomers/models.py:365
 msgid "New Clients"
 msgstr "Nouveaux bénéficiaires"
 
 #: lino_welfare/modlib/newcomers/models.py:229
-#: lino_welfare/modlib/newcomers/models.py:278
+#: lino_welfare/modlib/newcomers/models.py:279
 msgid "New clients since"
 msgstr "Nouveaux bénéficiaires depuis"
 
-#: lino_welfare/modlib/newcomers/models.py:267
+#: lino_welfare/modlib/newcomers/models.py:268
 msgid "List of users available for new coachings"
 msgstr ""
 
-#: lino_welfare/modlib/newcomers/models.py:272
+#: lino_welfare/modlib/newcomers/models.py:273
 #: lino_welfare/modlib/newcomers/models.py:485
 msgid "Available Coaches"
 msgstr "Agents disponibles"
 
-#: lino_welfare/modlib/newcomers/models.py:276
+#: lino_welfare/modlib/newcomers/models.py:277
 msgid "Show suggested agents for"
 msgstr "Montrer agents proposés pour"
 
-#: lino_welfare/modlib/newcomers/models.py:281
+#: lino_welfare/modlib/newcomers/models.py:282
 msgid "New clients are those whose coaching started after this date"
 msgstr ""
 
 #: lino_welfare/modlib/newcomers/models.py:306
 msgid "Only for clients with given `faculty`."
 msgstr ""
 
@@ -3122,15 +3130,15 @@
 
 #: lino_welfare/modlib/pcsw/actions.py:145
 #, python-format
 msgid "This will end %(count)d coachings of %(client)s."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/choicelists.py:15
-#: lino_welfare/modlib/pcsw/models.py:946
+#: lino_welfare/modlib/pcsw/models.py:948
 #, fuzzy
 msgid "Dispense"
 msgstr "Réponse"
 
 #: lino_welfare/modlib/pcsw/choicelists.py:27
 msgid "Penalty"
 msgstr ""
@@ -3219,226 +3227,226 @@
 msgid "Contact person at local job office"
 msgstr "Personne de contacte ALE ?"
 
 #: lino_welfare/modlib/pcsw/models.py:236
 msgid "Circular reference"
 msgstr "référence circulaire ?"
 
-#: lino_welfare/modlib/pcsw/models.py:262
+#: lino_welfare/modlib/pcsw/models.py:264
 msgid "eID card expires in 2 months"
 msgstr "carte eID expire dans 2 mois"
 
-#: lino_welfare/modlib/pcsw/models.py:264
+#: lino_welfare/modlib/pcsw/models.py:266
 msgid "becomes available again in 1 month"
 msgstr "redevient disponible dans 1 mois"
 
-#: lino_welfare/modlib/pcsw/models.py:267
+#: lino_welfare/modlib/pcsw/models.py:269
 msgid "work permit suspension ends in 1 month"
 msgstr "fin de suspension du permis de travail dans 1 mois"
 
-#: lino_welfare/modlib/pcsw/models.py:350
+#: lino_welfare/modlib/pcsw/models.py:352
 msgid "Contract starts"
 msgstr "Contrat débute"
 
-#: lino_welfare/modlib/pcsw/models.py:356
+#: lino_welfare/modlib/pcsw/models.py:358
 msgid "Contract ends"
 msgstr "Contrat se termine"
 
-#: lino_welfare/modlib/pcsw/models.py:365
+#: lino_welfare/modlib/pcsw/models.py:367
 #, fuzzy
 msgid "Working at "
 msgstr "Travaille"
 
-#: lino_welfare/modlib/pcsw/models.py:372
+#: lino_welfare/modlib/pcsw/models.py:374
 msgid "Active contract"
 msgstr "Contrat actif"
 
-#: lino_welfare/modlib/pcsw/models.py:491
+#: lino_welfare/modlib/pcsw/models.py:493
 msgid "Human Links"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:497
+#: lino_welfare/modlib/pcsw/models.py:499
 msgid "Coaches"
 msgstr "Intervenants"
 
-#: lino_welfare/modlib/pcsw/models.py:523
+#: lino_welfare/modlib/pcsw/models.py:525
 msgid "Job search"
 msgstr "Recherche d'emploi"
 
-#: lino_welfare/modlib/pcsw/models.py:552
+#: lino_welfare/modlib/pcsw/models.py:554
 msgid "Calendar"
 msgstr "Calendrier"
 
-#: lino_welfare/modlib/pcsw/models.py:569
+#: lino_welfare/modlib/pcsw/models.py:571
 msgid "Career"
 msgstr "Parcours"
 
-#: lino_welfare/modlib/pcsw/models.py:576
+#: lino_welfare/modlib/pcsw/models.py:578
 msgid "Languages"
 msgstr "Langues"
 
-#: lino_welfare/modlib/pcsw/models.py:590
+#: lino_welfare/modlib/pcsw/models.py:592
 msgid "Contracts"
 msgstr "Contrats"
 
-#: lino_welfare/modlib/pcsw/models.py:635
+#: lino_welfare/modlib/pcsw/models.py:637
 msgid "Coached by"
 msgstr "Intervenant"
 
-#: lino_welfare/modlib/pcsw/models.py:641
+#: lino_welfare/modlib/pcsw/models.py:643
 msgid "and by"
 msgstr "et par"
 
-#: lino_welfare/modlib/pcsw/models.py:647
+#: lino_welfare/modlib/pcsw/models.py:649
 msgid "Nationality"
 msgstr "Nationalité"
 
-#: lino_welfare/modlib/pcsw/models.py:651
+#: lino_welfare/modlib/pcsw/models.py:653
 msgid "Extended filter criteria, e.g.:"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:652
+#: lino_welfare/modlib/pcsw/models.py:654
 msgid "Active: All those who have some active coaching."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:653
+#: lino_welfare/modlib/pcsw/models.py:655
 msgid "Only primary clients"
 msgstr "Dossiers titulaires seulement"
 
-#: lino_welfare/modlib/pcsw/models.py:782
+#: lino_welfare/modlib/pcsw/models.py:784
 msgid "and"
 msgstr "et"
 
-#: lino_welfare/modlib/pcsw/models.py:786
+#: lino_welfare/modlib/pcsw/models.py:788
 #, python-format
 msgid " on %(date)s"
 msgstr " le %(date)s"
 
-#: lino_welfare/modlib/pcsw/models.py:790
+#: lino_welfare/modlib/pcsw/models.py:792
 #, python-format
 msgid "Coached on %s"
 msgstr "Accompagné le %s"
 
-#: lino_welfare/modlib/pcsw/models.py:841
+#: lino_welfare/modlib/pcsw/models.py:843
 msgid "Check for valid identification"
 msgstr "Vérifier les données identifiantes"
 
-#: lino_welfare/modlib/pcsw/models.py:850
+#: lino_welfare/modlib/pcsw/models.py:852
 msgid "Neither valid eId data nor alternative identifying document."
 msgstr "Sans données eID ou document identifiant alternatif."
 
-#: lino_welfare/modlib/pcsw/models.py:868
+#: lino_welfare/modlib/pcsw/models.py:870
 msgid "Integration phases"
 msgstr "Phases d'insertion"
 
-#: lino_welfare/modlib/pcsw/models.py:872
+#: lino_welfare/modlib/pcsw/models.py:874
 msgid "Reference name"
 msgstr "Nom de référence"
 
-#: lino_welfare/modlib/pcsw/models.py:873
+#: lino_welfare/modlib/pcsw/models.py:875
 msgid "Considered active"
 msgstr "Considéré actif"
 
-#: lino_welfare/modlib/pcsw/models.py:898
+#: lino_welfare/modlib/pcsw/models.py:900
 msgid "activity"
 msgstr "Activité"
 
-#: lino_welfare/modlib/pcsw/models.py:899
+#: lino_welfare/modlib/pcsw/models.py:901
 msgid "activities"
 msgstr "Activités"
 
-#: lino_welfare/modlib/pcsw/models.py:902
+#: lino_welfare/modlib/pcsw/models.py:904
 msgid "Appears in Listing 104"
 msgstr "Apparaît dans la liste 104"
 
-#: lino_welfare/modlib/pcsw/models.py:909
+#: lino_welfare/modlib/pcsw/models.py:911
 msgid "Liste des \"activités\" ou \"codes profession\"."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:925
+#: lino_welfare/modlib/pcsw/models.py:927
 msgid "Dispense reason"
 msgstr "Motif de dispense"
 
-#: lino_welfare/modlib/pcsw/models.py:926
+#: lino_welfare/modlib/pcsw/models.py:928
 msgid "Dispense reasons"
 msgstr "Motifs de dispense"
 
-#: lino_welfare/modlib/pcsw/models.py:935
+#: lino_welfare/modlib/pcsw/models.py:937
 msgid "A list of reasons for being dispensed"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:947
+#: lino_welfare/modlib/pcsw/models.py:949
 msgid "Dispenses"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:955
+#: lino_welfare/modlib/pcsw/models.py:957
 #, fuzzy
 msgid "Dispensed from"
 msgstr "Devoirs personne"
 
-#: lino_welfare/modlib/pcsw/models.py:961
+#: lino_welfare/modlib/pcsw/models.py:963
 msgid "Liste de dispenses"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:978
+#: lino_welfare/modlib/pcsw/models.py:980
 msgid "Unemployment exclusion type"
 msgstr "Raison d'exclusion du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:979
+#: lino_welfare/modlib/pcsw/models.py:981
 msgid "Unemployment exclusion types"
 msgstr "Types d'exclusion du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:988
+#: lino_welfare/modlib/pcsw/models.py:990
 msgid ""
 "Liste des raisons possibles d'arrêter temporairement\n"
 "    le paiement d'une aide financière prévue."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:998
+#: lino_welfare/modlib/pcsw/models.py:1000
 msgid "Exclusion from unemployment"
 msgstr "Exclusion du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:999
+#: lino_welfare/modlib/pcsw/models.py:1001
 msgid "Exclusions from unemployment"
 msgstr "Exclusions du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:1008
+#: lino_welfare/modlib/pcsw/models.py:1010
 msgid "Excluded from"
 msgstr "Du"
 
-#: lino_welfare/modlib/pcsw/models.py:1025
+#: lino_welfare/modlib/pcsw/models.py:1027
 #, fuzzy
 msgid "Liste des exclusions."
 msgstr "exclusions"
 
-#: lino_welfare/modlib/pcsw/models.py:1031
+#: lino_welfare/modlib/pcsw/models.py:1033
 msgid "Unemployment situation"
 msgstr "Situation chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:1042
+#: lino_welfare/modlib/pcsw/models.py:1044
 msgid "Conviction"
 msgstr "Antécédent judiciaire"
 
-#: lino_welfare/modlib/pcsw/models.py:1043
+#: lino_welfare/modlib/pcsw/models.py:1045
 msgid "Convictions"
 msgstr "Antécédents judiciaires"
 
-#: lino_welfare/modlib/pcsw/models.py:1047
+#: lino_welfare/modlib/pcsw/models.py:1049
 msgid "Prejudicial"
 msgstr "Préjudiciable"
 
-#: lino_welfare/modlib/pcsw/models.py:1083
+#: lino_welfare/modlib/pcsw/models.py:1085
 msgid "aid type"
 msgstr "Type d'aide sociale"
 
-#: lino_welfare/modlib/pcsw/models.py:1084
+#: lino_welfare/modlib/pcsw/models.py:1086
 msgid "aid types"
 msgstr "Types d'aide sociale"
 
-#: lino_welfare/modlib/pcsw/models.py:1088
+#: lino_welfare/modlib/pcsw/models.py:1090
 msgid "Liste des types d'aide financière."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/fixtures/std.py:24
 #, fuzzy
 msgid "Formation"
 msgstr "période d'essai"
@@ -3639,888 +3647,894 @@
 msgid "Lino Welfare"
 msgstr "Lino pour CPAS"
 
 #: lino_welfare/modlib/welfare/help_texts.py:7
 msgid "The standard migrator for welfare."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:9
+#: lino_welfare/modlib/welfare/help_texts.py:8
 msgid "The plugin."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:11
+#: lino_welfare/modlib/welfare/help_texts.py:9
 msgid ""
 "Optionally specify the primary key (an integer) of the last granting for which "
 "you want to deactivate date range validation in confirmations. This is useful "
 "for keeping legacy confirmations that have been issued before the rule was "
 "activated."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:14
-#: lino_welfare/modlib/welfare/help_texts.py:19
-#: lino_welfare/modlib/welfare/help_texts.py:94
-#: lino_welfare/modlib/welfare/help_texts.py:96
-#: lino_welfare/modlib/welfare/help_texts.py:104
-#: lino_welfare/modlib/welfare/help_texts.py:106
-#: lino_welfare/modlib/welfare/help_texts.py:108
-#: lino_welfare/modlib/welfare/help_texts.py:117
-#: lino_welfare/modlib/welfare/help_texts.py:119
-#: lino_welfare/modlib/welfare/help_texts.py:121
-#: lino_welfare/modlib/welfare/help_texts.py:123
+#: lino_welfare/modlib/welfare/help_texts.py:10
+#: lino_welfare/modlib/welfare/help_texts.py:12
+#: lino_welfare/modlib/welfare/help_texts.py:43
+#: lino_welfare/modlib/welfare/help_texts.py:44
+#: lino_welfare/modlib/welfare/help_texts.py:47
+#: lino_welfare/modlib/welfare/help_texts.py:48
+#: lino_welfare/modlib/welfare/help_texts.py:49
+#: lino_welfare/modlib/welfare/help_texts.py:53
+#: lino_welfare/modlib/welfare/help_texts.py:54
+#: lino_welfare/modlib/welfare/help_texts.py:55
+#: lino_welfare/modlib/welfare/help_texts.py:56
 msgid "See lino.core.plugin.Plugin."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:16
+#: lino_welfare/modlib/welfare/help_texts.py:11
 msgid ""
 "A string referring to the model which represents the badge holder in your "
 "application. Default value is 'contacts.Person'."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:21
+#: lino_welfare/modlib/welfare/help_texts.py:13
 msgid "The descriptor for this plugin. See lino.core.plugin.Plugin."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:23
+#: lino_welfare/modlib/welfare/help_texts.py:14
 msgid ""
 "Whether executing requests should try to really connect to the CBSS. Real "
 "requests would fail with a timeout if run from behind an IP address that is not "
 "registered at the CBSS."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:26
+#: lino_welfare/modlib/welfare/help_texts.py:15
 msgid "Either None or one of ‘test’, ‘acpt’ or ‘prod’."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:28
+#: lino_welfare/modlib/welfare/help_texts.py:16
 #, fuzzy
 msgid "The status of a CBSSRequest."
 msgstr "Date de la demande"
 
-#: lino_welfare/modlib/welfare/help_texts.py:30
+#: lino_welfare/modlib/welfare/help_texts.py:17
 msgid ""
 "Possible values for the action field of a lino_welfare.modlib.cbss.models."
 "ManageAccessRequest."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:33
+#: lino_welfare/modlib/welfare/help_texts.py:18
 msgid ""
 "Ce service est sollicité au moment du démarrage de l’enquête sociale. Le CPAS "
 "déclare au réseau de la sécurité sociale qu’il possède un dossier pour lequel "
 "il a l’autorisation (dispositions légales et réglementaires) d’obtenir des "
 "informations des autres institutions en vue de compléter son enquête dans le "
 "cadre de l’octroi du revenu d’intégration. Cette déclaration concerne le "
 "répertoire sectoriel des CPAS à la SmalS-MvM et peut concerner plusieurs "
 "catégories de personnes : le demandeur, les cohabitants et les tiers concernés "
 "et ce, pour des finalités différentes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:36
+#: lino_welfare/modlib/welfare/help_texts.py:19
 msgid "L’opération contraire est aussi mise à disposition."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:38
+#: lino_welfare/modlib/welfare/help_texts.py:20
 msgid ""
 "Il est en plus possible d’obtenir une liste des enregistrements dans le "
 "répertoire sectoriel des CPAS à la SmalS-MvM ainsi qu’au sein du réseau BCSS."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:41
+#: lino_welfare/modlib/welfare/help_texts.py:21
 msgid ""
 "Possible values for the query_register field of a lino_welfare.modlib.cbss."
 "models.ManageAccessRequest."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:44
+#: lino_welfare/modlib/welfare/help_texts.py:22
 msgid "Query only the primary register."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:46
+#: lino_welfare/modlib/welfare/help_texts.py:23
 msgid "Query only the secondary register."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:48
+#: lino_welfare/modlib/welfare/help_texts.py:24
 msgid "Query both registers."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:50
+#: lino_welfare/modlib/welfare/help_texts.py:25
 msgid "Common Abstract Base Class for SSDNRequest and NewStyleRequest"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:52
+#: lino_welfare/modlib/welfare/help_texts.py:26
 msgid "alias of NotImplementedError"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:54
+#: lino_welfare/modlib/welfare/help_texts.py:27
 msgid ""
 "When duplicating a CBSS request, we want re-execute it. So please duplicate "
 "only the parameters, not the execution data like ticket, sent and status. Note "
 "that also the user will be set to the user who asked to duplicate (because this "
 "is a subclass of UserAuthored."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:57
+#: lino_welfare/modlib/welfare/help_texts.py:28
 msgid "CBSS requests that have a ticket may never be modified."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:59
-#: lino_welfare/modlib/welfare/help_texts.py:83
+#: lino_welfare/modlib/welfare/help_texts.py:29
+#: lino_welfare/modlib/welfare/help_texts.py:38
 msgid "Called when a successful reply has been received."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:61
+#: lino_welfare/modlib/welfare/help_texts.py:30
 msgid "This is the common part of a request for both classic and new-style."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:64
+#: lino_welfare/modlib/welfare/help_texts.py:31
 msgid ""
 "When we print a request, the resulting excerpt should go to the client’s "
 "history."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:67
+#: lino_welfare/modlib/welfare/help_texts.py:32
 msgid "Abstract Base Class for Models that represent SSDN (“classic”) requests."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:70
+#: lino_welfare/modlib/welfare/help_texts.py:33
 msgid ""
 "Validates the generated XML against the XSD files. Used by test suite. It is "
 "not necessary to validate each real request before actually sending it."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:73
+#: lino_welfare/modlib/welfare/help_texts.py:34
 msgid "SSDN specific part of a request."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:75
+#: lino_welfare/modlib/welfare/help_texts.py:35
 msgid ""
 "Wrap the given service request into the SSDN envelope by adding AuthorizedUser "
 "and other information common the all SSDN requests)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:78
+#: lino_welfare/modlib/welfare/help_texts.py:36
 msgid ""
 "Abstract Base Class for Models that represent “new style” requests to the CBSS "
 "(and responses)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:81
+#: lino_welfare/modlib/welfare/help_texts.py:37
 msgid "NewStyle specific part of a request."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:85
+#: lino_welfare/modlib/welfare/help_texts.py:39
 msgid ""
 "Abstract base for Requests that have a field national_id and a method "
 "get_ssin()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:88
+#: lino_welfare/modlib/welfare/help_texts.py:40
 msgid "Mixin for models that have certain fields"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:90
+#: lino_welfare/modlib/welfare/help_texts.py:41
 msgid "Space-separated list of all first names."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:92
+#: lino_welfare/modlib/welfare/help_texts.py:42
 msgid "Last name (family name)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:98
+#: lino_welfare/modlib/welfare/help_texts.py:45
 msgid ""
 "Model mixin to add to the base classes of your application’s pcsw.Client model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:101
+#: lino_welfare/modlib/welfare/help_texts.py:46
 msgid ""
 "Overrides lino.mixins.dupable.Dupable.find_similar_instances(), adding some "
 "additional rules."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:110
+#: lino_welfare/modlib/welfare/help_texts.py:50
 msgid ""
 "Whether to show only primary coachings in the columns (coachings per "
 "Integration phase table."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:113
+#: lino_welfare/modlib/welfare/help_texts.py:51
 msgid "Has access to data used by integration agents."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:115
+#: lino_welfare/modlib/welfare/help_texts.py:52
 msgid "Can configure social integration functionality."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:125
+#: lino_welfare/modlib/welfare/help_texts.py:57
 msgid "Refuse this newcomer request."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:127
+#: lino_welfare/modlib/welfare/help_texts.py:58
 msgid ""
 "Change client’s state to ‘former’. This will also end any active coachings."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:130
+#: lino_welfare/modlib/welfare/help_texts.py:59
 msgid "Has limited access to data of social workers. Can see contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:132
+#: lino_welfare/modlib/welfare/help_texts.py:60
 msgid "Can access data managed by general social workers."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:134
+#: lino_welfare/modlib/welfare/help_texts.py:61
 msgid "Can configure general social work functionality."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:136
+#: lino_welfare/modlib/welfare/help_texts.py:62
 msgid "Can manage external courses."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:138
+#: lino_welfare/modlib/welfare/help_texts.py:63
 msgid "Can manage and configure external courses."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:140
+#: lino_welfare/modlib/welfare/help_texts.py:64
 msgid "The Django model representing an aid type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:142
+#: lino_welfare/modlib/welfare/help_texts.py:65
 msgid ""
 "The short name for internal use, e.g. when a user must select an aid type from "
 "a combobox."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:145
+#: lino_welfare/modlib/welfare/help_texts.py:66
 msgid ""
 "The database model to use for issuing an aid confirmation of this type. This is "
 "a mandatory pointer to ConfirmationTypes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:148
+#: lino_welfare/modlib/welfare/help_texts.py:67
 msgid ""
 "The designation of this aid type as seen by the user e.g. when selecting an aid "
 "type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:151
+#: lino_welfare/modlib/welfare/help_texts.py:68
 msgid ""
 "The text to print as title in confirmations. See also lino_xl.lib.excerpts."
 "mixins.ExcerptTitle.excerpt_title."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:154
+#: lino_welfare/modlib/welfare/help_texts.py:69
 msgid ""
 "The body template to use when printing a confirmation of this type. If this "
 "field is empty, Lino uses the excerpt type’s body_template. See also lino.admin."
 "printing."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:157
+#: lino_welfare/modlib/welfare/help_texts.py:70
 msgid ""
 "Whether aid grantings of this type are considered as urgent. This is used by "
 "Confirmation.get_urgent_granting()"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:160
+#: lino_welfare/modlib/welfare/help_texts.py:71
 msgid ""
 "Pointer to the default lino_xl.lib.boards.models.Board for aid projects of this "
 "type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:163
+#: lino_welfare/modlib/welfare/help_texts.py:72
 msgid ""
 "Whether grantings for this aid type are to be signed by the client’s primary "
 "coach (see Client.get_primary_coach)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:166
+#: lino_welfare/modlib/welfare/help_texts.py:73
 msgid ""
 "A pointer to the ClientContactType to be used when selecting the pharmacy of a "
 "refund confirmation (RefundConfirmation.pharmacy)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:169
+#: lino_welfare/modlib/welfare/help_texts.py:74
 msgid "The Django model representing an aid granting."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:171
+#: lino_welfare/modlib/welfare/help_texts.py:75
 msgid "Pointer to the lino_welfare.modlib.pcsw.models.Client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:173
+#: lino_welfare/modlib/welfare/help_texts.py:76
 msgid "The type of aid being granted. Mandatory. Pointer to the AidType."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:175
+#: lino_welfare/modlib/welfare/help_texts.py:77
 msgid ""
 "Pointer to the user who is expected to “sign” this granting (i.e. to confirm "
 "that it is real)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:178
+#: lino_welfare/modlib/welfare/help_texts.py:78
 msgid "Pointer to the Board which decided to allocate this aid project."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:180
+#: lino_welfare/modlib/welfare/help_texts.py:79
 msgid "Currently only used for printing an isip.Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:182
+#: lino_welfare/modlib/welfare/help_texts.py:80
 msgid "Base class for all aid confirmations."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:184
+#: lino_welfare/modlib/welfare/help_texts.py:81
 #, fuzzy
 msgid ""
 "Return an error message if this confirmation lies outside of granted period."
 msgstr "Période %(p1)s hors de la période d'ocroi %(p2)s."
 
-#: lino_welfare/modlib/welfare/help_texts.py:187
+#: lino_welfare/modlib/welfare/help_texts.py:82
 msgid "Base class for both Granting and Confirmation."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:189
+#: lino_welfare/modlib/welfare/help_texts.py:83
 msgid "The confirmation state of this object. Pointer to ConfirmationStates."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:192
+#: lino_welfare/modlib/welfare/help_texts.py:84
 msgid "Sign this granting or confirmation, making most fields read-only."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:194
+#: lino_welfare/modlib/welfare/help_texts.py:85
 msgid "Revoke your signature of this granting or confirmation."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:196
+#: lino_welfare/modlib/welfare/help_texts.py:86
 msgid "Adds two fields."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:198
+#: lino_welfare/modlib/welfare/help_texts.py:87
 msgid "How to summarize entries of this type in the ESF summary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:200
+#: lino_welfare/modlib/welfare/help_texts.py:88
 msgid "Adds a virtual field client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:202
+#: lino_welfare/modlib/welfare/help_texts.py:89
 msgid "Virtual field which returns the partner if it is a client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:204
+#: lino_welfare/modlib/welfare/help_texts.py:90
+msgid ""
+"Shows calendar entries having either project or one guest pointing to this "
+"client."
+msgstr ""
+
+#: lino_welfare/modlib/welfare/help_texts.py:91
 msgid "Default values filled from lino_welfare.modlib.cbss.fixtures.sectors."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:207
+#: lino_welfare/modlib/welfare/help_texts.py:92
 msgid ""
 "Codes qualité (Hoedanigheidscodes). This table is usually filled with the "
 "official codes by lino_welfare.modlib.cbss.fixtures.purposes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:210
+#: lino_welfare/modlib/welfare/help_texts.py:93
 msgid "A request to the IdentifyPerson service."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:212
+#: lino_welfare/modlib/welfare/help_texts.py:94
 msgid "A request to the ManageAccess service."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:214
+#: lino_welfare/modlib/welfare/help_texts.py:95
 msgid "Pointer to Sector."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:216
+#: lino_welfare/modlib/welfare/help_texts.py:96
 msgid "Pointer to Purpose."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:218
+#: lino_welfare/modlib/welfare/help_texts.py:97
 msgid ""
 "The action to perform. This must be one of the values in lino_welfare.modlib."
 "cbss.choicelists.ManageActions"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:221
+#: lino_welfare/modlib/welfare/help_texts.py:98
 msgid ""
 "The register to be query. This must be one of the values in lino_welfare.modlib."
 "cbss.choicelists.QueryRegisters"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:224
+#: lino_welfare/modlib/welfare/help_texts.py:99
 msgid "A request to the RetrieveTIGroups service (aka Tx25)"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:226
+#: lino_welfare/modlib/welfare/help_texts.py:100
 #, fuzzy
 msgid "Whether to print empty rows."
 msgstr "Imprimer lignes vides"
 
-#: lino_welfare/modlib/welfare/help_texts.py:228
+#: lino_welfare/modlib/welfare/help_texts.py:101
 #, fuzzy
 msgid "Whether to ignore yearly incomes."
 msgstr "Inclure revenus annuels"
 
-#: lino_welfare/modlib/welfare/help_texts.py:230
+#: lino_welfare/modlib/welfare/help_texts.py:102
 msgid ""
 "Yield the entry groups for this budget, i.e. one item for each account group "
 "for which this budget has some data."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:233
+#: lino_welfare/modlib/welfare/help_texts.py:103
 msgid "The database model used to represent a budget actor."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:235
+#: lino_welfare/modlib/welfare/help_texts.py:104
 msgid "A detail row of a Budget."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:237
+#: lino_welfare/modlib/welfare/help_texts.py:105
 msgid ""
 "Optionally specify a budget actor who contributes this entry. Leave empty when "
 "the entry refers to the entire household."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:240
+#: lino_welfare/modlib/welfare/help_texts.py:106
 msgid ""
 "The amount of money. An empty amount is different from a zero amount in that "
 "the latter will be printed while the former not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:243
+#: lino_welfare/modlib/welfare/help_texts.py:107
 msgid "The related Account."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:245
+#: lino_welfare/modlib/welfare/help_texts.py:108
 msgid ""
 "An account is an item of an account chart used to collect ledger transactions "
 "or other accountable items."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:248
+#: lino_welfare/modlib/welfare/help_texts.py:109
 msgid "The multilingual designation of this account, as the users see it."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:251
+#: lino_welfare/modlib/welfare/help_texts.py:110
 msgid ""
 "The account group to which this account belongs. This must point to an instance "
 "of Group."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:254
+#: lino_welfare/modlib/welfare/help_texts.py:111
 msgid "The sequence number of this account within its group."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:256
+#: lino_welfare/modlib/welfare/help_texts.py:112
 msgid "An optional unique name which can be used to reference a given account."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:259
+#: lino_welfare/modlib/welfare/help_texts.py:113
 msgid ""
 "The account type of this account. This must point to an item of lino_welfare."
 "modlib.debts.AccountTypes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:262
+#: lino_welfare/modlib/welfare/help_texts.py:114
 msgid "Base class for both the volatile MainActor and the Actor model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:264
+#: lino_welfare/modlib/welfare/help_texts.py:115
 msgid "A volatile object that represents the budget partner as actor"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:266
+#: lino_welfare/modlib/welfare/help_texts.py:116
 msgid ""
 "Used for Entry.periods and Account.periods (the latter holds simply the default "
 "value for the former). It means: for how many months the entered amount counts. "
 "Default value is 1. For yearly amounts set it to 12."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:269
+#: lino_welfare/modlib/welfare/help_texts.py:117
 msgid "The Django model that represents a client summary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:271
+#: lino_welfare/modlib/welfare/help_texts.py:118
 msgid "Base class for all tables on ClientSummary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:273
+#: lino_welfare/modlib/welfare/help_texts.py:119
 msgid "Lists all ESF summaries for all clients."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:275
+#: lino_welfare/modlib/welfare/help_texts.py:120
 msgid "Lists the ESF summaries for a given client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:277
+#: lino_welfare/modlib/welfare/help_texts.py:121
 msgid "Base class for all statistical fields."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:279
+#: lino_welfare/modlib/welfare/help_texts.py:122
 msgid "Used as the verbose_name of field."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:281
+#: lino_welfare/modlib/welfare/help_texts.py:123
 #, fuzzy
 msgid "The internal field name."
 msgstr "Mise en situation interne"
 
-#: lino_welfare/modlib/welfare/help_texts.py:283
+#: lino_welfare/modlib/welfare/help_texts.py:124
 msgid "The field descriptor (an instance of a Django Field)"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:285
+#: lino_welfare/modlib/welfare/help_texts.py:125
 msgid "Count the number of presences."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:287
+#: lino_welfare/modlib/welfare/help_texts.py:126
 msgid "Count the real hours of presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:289
+#: lino_welfare/modlib/welfare/help_texts.py:127
 msgid "Count the event’s duration for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:291
+#: lino_welfare/modlib/welfare/help_texts.py:128
 msgid "Count a fixed time for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:293
+#: lino_welfare/modlib/welfare/help_texts.py:129
 msgid ""
 "Shows the members of the primary household of this person together with an "
 "amount which depends on whether that member is adult or not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:296
+#: lino_welfare/modlib/welfare/help_texts.py:130
 msgid ""
 "The amount to refund for children (household members less than lino_xl.lib."
 "households.Plugin.adult_age years old)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:299
+#: lino_welfare/modlib/welfare/help_texts.py:131
 msgid ""
 "The amount to refund for children (household members who are lino_xl.lib."
 "households.Plugin.adult_age years or older)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:302
+#: lino_welfare/modlib/welfare/help_texts.py:132
 msgid "The full name of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:304
+#: lino_welfare/modlib/welfare/help_texts.py:133
 msgid ""
 "The amount to pay. This is either child_tariff or adult_tarif depending on the "
 "age of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:307
+#: lino_welfare/modlib/welfare/help_texts.py:134
 msgid "Model mixin for all integration contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:309
+#: lino_welfare/modlib/welfare/help_texts.py:135
 msgid "The person who created this contract."
 msgstr "La personne qui a créé ce contrat."
 
-#: lino_welfare/modlib/welfare/help_texts.py:311
+#: lino_welfare/modlib/welfare/help_texts.py:136
 msgid "The responsible person at the general social service."
 msgstr "La personne responsable au service social général."
 
-#: lino_welfare/modlib/welfare/help_texts.py:313
+#: lino_welfare/modlib/welfare/help_texts.py:137
 msgid "The client for whom this contract is done."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:315
+#: lino_welfare/modlib/welfare/help_texts.py:138
 msgid "The start date of the contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:317
+#: lino_welfare/modlib/welfare/help_texts.py:139
 msgid "The planned end date of this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:319
+#: lino_welfare/modlib/welfare/help_texts.py:140
 msgid ""
 "The date when this contract was effectively ended. This field is set to the "
 "same value as applies_until."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:322
+#: lino_welfare/modlib/welfare/help_texts.py:141
 msgid "The reason of prematured ending. Pointer to ContractEnding"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:324
+#: lino_welfare/modlib/welfare/help_texts.py:142
 msgid "When the contract was issued to the client and signed by them."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:326
+#: lino_welfare/modlib/welfare/help_texts.py:143
 msgid "When the contract was ratified by the responsible board."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:328
+#: lino_welfare/modlib/welfare/help_texts.py:144
 msgid "The language of this contract. Default value is the client’s language."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:331
+#: lino_welfare/modlib/welfare/help_texts.py:145
 msgid "The type of this contract. Pointer to a subclass of ContractTypeBase."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:334
+#: lino_welfare/modlib/welfare/help_texts.py:146
 msgid ""
 "The printed title of a contract specifies just the contract type (not the "
 "number and name of client)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:337
+#: lino_welfare/modlib/welfare/help_texts.py:147
 msgid "Overrides lino_xl.lib.excerpts.Certifiable.get_excerpt_templates()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:340
+#: lino_welfare/modlib/welfare/help_texts.py:148
 msgid ""
 "If the contract’s author is the client’s primary coach, then set user_asd to "
 "None, otherwise set user_asd to the primary coach. We no longer suppose that "
 "only integration agents write contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:343
+#: lino_welfare/modlib/welfare/help_texts.py:149
 msgid "Checks for the following error conditions:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:345
+#: lino_welfare/modlib/welfare/help_texts.py:150
 msgid ""
 "Returns the last aid confirmation that has been issued for this contract. May "
 "be used in .odt template."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:348
+#: lino_welfare/modlib/welfare/help_texts.py:151
 msgid ""
 "Automatic evaluation events have the client as mandatory participant, plus "
 "possibly some other coach."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:351
+#: lino_welfare/modlib/welfare/help_texts.py:152
 msgid ""
 "All contracts of a demo project (not only one) are being printed. Overrides "
 "lino.modlib.printing.Printable.get_printable_demo_objects()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:354
+#: lino_welfare/modlib/welfare/help_texts.py:153
 msgid "Model mixin for integration contracts that have a single partner."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:356
+#: lino_welfare/modlib/welfare/help_texts.py:154
 msgid "Base for contract tables. Defines the following parameter fields:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:358
+#: lino_welfare/modlib/welfare/help_texts.py:155
 #, fuzzy
 msgid "See ContractEvents."
 msgstr "utilisable dans contrats"
 
-#: lino_welfare/modlib/welfare/help_texts.py:360
+#: lino_welfare/modlib/welfare/help_texts.py:156
 msgid "Show only contracts with the specified ContractEnding."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:362
+#: lino_welfare/modlib/welfare/help_texts.py:157
 msgid ""
 "Select “Yes” to show only contracts whose ending ContractEnding has is_success "
 "checked."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:365
+#: lino_welfare/modlib/welfare/help_texts.py:158
 msgid "The Django model representing an ISIP."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:367
+#: lino_welfare/modlib/welfare/help_texts.py:159
 msgid "The type of this contract. Pointer to ContractType."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:369
+#: lino_welfare/modlib/welfare/help_texts.py:160
 msgid "The type of study that is going to be followed during this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:372
+#: lino_welfare/modlib/welfare/help_texts.py:161
 msgid "The table of all ISIP contract types."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:374
+#: lino_welfare/modlib/welfare/help_texts.py:162
 msgid "The type of a Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:376
+#: lino_welfare/modlib/welfare/help_texts.py:163
 msgid "Whether contracts of this type need their study_type field filled in."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:379
+#: lino_welfare/modlib/welfare/help_texts.py:164
 msgid "Django model to represent an examination policy."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:381
+#: lino_welfare/modlib/welfare/help_texts.py:165
 msgid "A possible reason for premature termination of a contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:383
+#: lino_welfare/modlib/welfare/help_texts.py:166
 msgid ""
 "Represents a third-party external partner who participates in this contract. "
 "For every partner there is a rich text field describing their duties."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:386
+#: lino_welfare/modlib/welfare/help_texts.py:167
 msgid ""
 "A list of observable events for filtering contracts (ContractBaseTable."
 "observed_event)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:389
+#: lino_welfare/modlib/welfare/help_texts.py:168
 msgid ""
 "Whether the client has at least one ISIP contact during the observed date range."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:392
+#: lino_welfare/modlib/welfare/help_texts.py:169
 msgid "To see this table you need either IntegrationAgent or SocialCoordinator."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:395
+#: lino_welfare/modlib/welfare/help_texts.py:170
 msgid "Base class for all ContractType models."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:397
+#: lino_welfare/modlib/welfare/help_texts.py:171
 msgid "The full description of this contract type as used in printed documents."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:400
+#: lino_welfare/modlib/welfare/help_texts.py:172
 msgid "The default examination policy to be used for contracts of this type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:403
+#: lino_welfare/modlib/welfare/help_texts.py:173
 msgid ""
 "The overlap group to use when checking whether two contracts are overlapping or "
 "not. If this field is empty, Lino does not check at all for overlapping "
 "contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:406
+#: lino_welfare/modlib/welfare/help_texts.py:174
 msgid ""
 "The main template to use instead of the default template defined on the excerpt "
 "type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:409
+#: lino_welfare/modlib/welfare/help_texts.py:175
 msgid ""
 "The list of all known overlap groups to be selected for the overlap_group of a "
 "contract type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:412
+#: lino_welfare/modlib/welfare/help_texts.py:176
 msgid ""
 "Volatile object used to test for overlapping contracts. It is responsible for "
 "issuing the following error messages:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:415
+#: lino_welfare/modlib/welfare/help_texts.py:177
 msgid "A given client cannot have two active contracts at the same time."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:417
+#: lino_welfare/modlib/welfare/help_texts.py:178
 msgid ""
 "Organisation bénéficiant de l’agrément « Initiative d’économie sociale » "
 "octroyé par la Wallonie."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:420
+#: lino_welfare/modlib/welfare/help_texts.py:179
 #, fuzzy
 msgid "Shows all Art60 job supplyments."
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/welfare/help_texts.py:422
+#: lino_welfare/modlib/welfare/help_texts.py:180
 #, fuzzy
 msgid "Shows the Art60 job supplyments for this client."
 msgstr "Type de mise à l'emploi art.61"
 
-#: lino_welfare/modlib/welfare/help_texts.py:424
+#: lino_welfare/modlib/welfare/help_texts.py:181
 msgid ""
 "Model mixin for jobs.Contract and art61.Contract. And also for art60.Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:427
+#: lino_welfare/modlib/welfare/help_texts.py:182
 msgid "The duration of this job supplyment (number of working days)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:429
+#: lino_welfare/modlib/welfare/help_texts.py:183
 msgid "Django model used to represent a beneficiary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:431
+#: lino_welfare/modlib/welfare/help_texts.py:184
 msgid "Whether Lino should make ESF summaries for this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:433
+#: lino_welfare/modlib/welfare/help_texts.py:185
 msgid "A panel with general information about this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:435
+#: lino_welfare/modlib/welfare/help_texts.py:186
 msgid ""
 "A virtual field displaying a group of shortcut links for managing CVs "
 "(Curriculum Vitaes)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:438
+#: lino_welfare/modlib/welfare/help_texts.py:187
 msgid ""
 "A virtual field displaying a group of buttons for managing the “identifying "
 "document”, i.e. an uploaded document which has been used as alternative to the "
 "eID card."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:441
+#: lino_welfare/modlib/welfare/help_texts.py:188
 msgid "Pointer to PersonGroup. The intergration phase of this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:443
+#: lino_welfare/modlib/welfare/help_texts.py:189
 msgid "The civil state of this client. Allowed choices are defined in CivilState."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:446
+#: lino_welfare/modlib/welfare/help_texts.py:190
 #, fuzzy
 msgid "Pointer to ClientStates."
 msgstr "Bénéficiares (SI)"
 
-#: lino_welfare/modlib/welfare/help_texts.py:448
+#: lino_welfare/modlib/welfare/help_texts.py:191
 msgid ""
 "The date when this client got unemployed and stopped to have a regular work."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:451
+#: lino_welfare/modlib/welfare/help_texts.py:192
 msgid ""
 "The date when this client registered as unemployed and started to look for a "
 "new job."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:454
+#: lino_welfare/modlib/welfare/help_texts.py:193
 msgid ""
 "Return the last note of type “First meeting” for this client. Usage example see "
 "debts and notes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:457
+#: lino_welfare/modlib/welfare/help_texts.py:194
 msgid "The list that opens by Contacts ‣ Clients."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:459
+#: lino_welfare/modlib/welfare/help_texts.py:195
 msgid ""
 "If not empty, show only Clients whose client_state equals the specified value."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:462
+#: lino_welfare/modlib/welfare/help_texts.py:196
 msgid "Displays the response of an RetrieveTIGroupsRequest as a table."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:464
+#: lino_welfare/modlib/welfare/help_texts.py:197
 msgid "The Django database model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:466
+#: lino_welfare/modlib/welfare/help_texts.py:198
 msgid "Yield a list of all subsidizations activated for this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:468
+#: lino_welfare/modlib/welfare/help_texts.py:199
 #, fuzzy
 msgid "Shows the Art61 job supplyments for this client."
 msgstr "Type de mise à l'emploi art.61"
 
 #: lino_welfare/modlib/welfare/models.py:35
 msgid "Local job office"
 msgstr "Agence locale pour l'emploi"
@@ -4709,32 +4723,32 @@
 msgid "Dentist"
 msgstr "Dentiste"
 
 #: lino_welfare/modlib/welfare/fixtures/demo.py:781
 msgid "Pediatrician"
 msgstr "Pédiatre"
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:987
+#: lino_welfare/modlib/welfare/fixtures/demo.py:993
 msgid "A very hard job."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:988
+#: lino_welfare/modlib/welfare/fixtures/demo.py:994
 msgid "No supervisor. Only for independent people."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:1197
+#: lino_welfare/modlib/welfare/fixtures/demo.py:1215
 msgid "Urgent problem"
 msgstr "Problème urgent"
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:1197
+#: lino_welfare/modlib/welfare/fixtures/demo.py:1215
 #, fuzzy
 msgid "Complain"
 msgstr "Société"
 
-#: lino_welfare/modlib/welfare/fixtures/demo.py:1197
+#: lino_welfare/modlib/welfare/fixtures/demo.py:1215
 #, fuzzy
 msgid "Information"
 msgstr "période d'essai"
 
 #: lino_welfare/modlib/welfare/fixtures/std.py:83
 #, fuzzy
 msgid "Normal"
@@ -4908,27 +4922,27 @@
 msgid "The course which satisfies this request. Leave blank on open requests."
 msgstr ""
 
 #: lino_welfare/modlib/xcourses/models.py:352
 msgid "Course found"
 msgstr "Cours trouvé"
 
-#: lino_welfare/modlib/xcourses/models.py:496
+#: lino_welfare/modlib/xcourses/models.py:497
 msgid "Participants"
 msgstr ""
 
-#: lino_welfare/modlib/xcourses/models.py:534
+#: lino_welfare/modlib/xcourses/models.py:535
 msgid "Pending Course Requests"
 msgstr "Demandes de cours ouvertes"
 
-#: lino_welfare/modlib/xcourses/models.py:600
+#: lino_welfare/modlib/xcourses/models.py:601
 msgid "Age"
 msgstr ""
 
-#: lino_welfare/modlib/xcourses/models.py:614
+#: lino_welfare/modlib/xcourses/models.py:615
 msgid "unknown age"
 msgstr "age inconnu"
 
 #~ msgid "reason"
 #~ msgstr "raison"
 
 #~ msgid "eID card expires"
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/cpas2lino.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/garble.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/garble.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/gd2lino.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/initdb_tim.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/management/commands/watch_tim.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/settings.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,19 @@
         tb.add_action(self.modules.isip.MyContracts)
         # if self.is_installed("art60"):
         #     tb.add_action(self.modules.art60.MyContracts)
         # else:
         #     tb.add_action(self.modules.jobs.MyContracts)
         tb.add_action(self.modules.cal.EntriesByDay)
 
-    def get_installed_apps(self):
+    def get_installed_plugins(self):
         yield 'lino_welfare.modlib.system'
         # our custom system plugin must come before super() to avoid having
         # lino.modlib.system loaded
-        yield super().get_installed_apps()
+        yield super().get_installed_plugins()
         yield 'lino.modlib.help'
         yield 'lino_xl.lib.statbel.countries'
         yield 'lino_welfare.modlib.contacts'
 
         # yield 'lino.modlib.gfks'
         yield 'lino_xl.lib.appypod'
         yield 'django.contrib.humanize'  # translations for
@@ -97,15 +97,15 @@
         yield 'lino_welfare.modlib.pcsw'
         # yield 'lino_xl.lib.clients'
         # yield 'lino_xl.lib.coachings'
         yield 'lino_welfare.modlib.welfare'
 
         # NOTE: ordering influences (1) main menu (2) fixtures loading
         # e.g. pcsw.demo creates clients needed by cbss.demo
-        yield 'lino_welfare.modlib.sales'
+        yield 'lino_welfare.modlib.trading'
         # yield 'lino_welfare.modlib.pcsw'
         yield 'lino_welfare.modlib.ledger'
         yield 'lino_welfare.modlib.sepa'
         yield 'lino_xl.lib.b2c'
         yield 'lino_welfare.modlib.finan'
         # yield 'lino_xl.lib.bevats'
```

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/user_types.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/welfare/workflows.py` & `lino-welfare-24.5.0/lino_welfare/modlib/welfare/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/xcourses/__init__.py` & `lino-welfare-24.5.0/lino_welfare/modlib/xcourses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt` & `lino-welfare-24.5.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/xcourses/fixtures/demo.py` & `lino-welfare-24.5.0/lino_welfare/modlib/xcourses/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/modlib/xcourses/models.py` & `lino-welfare-24.5.0/lino_welfare/modlib/xcourses/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -405,26 +405,27 @@
                                                     blank=True))
         fields.update(CLIENTS_TABLE.parameters)
         super(CourseRequest, cls).setup_parameters(fields)
 
     @classmethod
     def get_request_queryset(self, ar):
         #~ raise Exception(20130424)
-        qs = super(CourseRequest, self).get_request_queryset(ar)
+        qs = super().get_request_queryset(ar)
         clients_qs = CLIENTS_TABLE.get_request_queryset(ar)
         #~ print 20130424, clients_qs
         qs = qs.filter(person__in=clients_qs)
-        if ar.param_values.request_state:
-            qs = qs.filter(state=ar.param_values.request_state)
-        if ar.param_values.course_content:
-            qs = qs.filter(content=ar.param_values.course_content)
-        if ar.param_values.course_provider:
-            qs = qs.filter(offer__provider=ar.param_values.course_provider)
-        if ar.param_values.course_offer:
-            qs = qs.filter(offer=ar.param_values.course_offer)
+        if (pv := ar.param_values) is None: return qs
+        if pv.request_state:
+            qs = qs.filter(state=pv.request_state)
+        if pv.course_content:
+            qs = qs.filter(content=pv.course_content)
+        if pv.course_provider:
+            qs = qs.filter(offer__provider=pv.course_provider)
+        if pv.course_offer:
+            qs = qs.filter(offer=pv.course_offer)
         return qs
 
     @classmethod
     def get_title_tags(self, ar):
         if ar.param_values.request_state:
             yield str(ar.param_values.request_state)
         if ar.param_values.course_content:
```

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/print_tx25.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/print_tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/demo.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt`

 * *Format-specific differences are supported for OpenOffice .odt files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: OpenDocument Text*

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-00000000: 504b 0304 1400 0000 0000 732e 6e58 5ec6  PK........s.nX^.
+00000000: 504b 0304 1400 0000 0000 3d10 a158 5ec6  PK........=..X^.
 00000010: 320c 2700 0000 2700 0000 0800 0000 6d69  2.'...'.......mi
 00000020: 6d65 7479 7065 6170 706c 6963 6174 696f  metypeapplicatio
 00000030: 6e2f 766e 642e 6f61 7369 732e 6f70 656e  n/vnd.oasis.open
 00000040: 646f 6375 6d65 6e74 2e74 6578 7450 4b03  document.textPK.
-00000050: 0414 0000 0008 0073 2e6e 5869 c544 95fe  .......s.nXi.D..
+00000050: 0414 0000 0008 003d 10a1 5869 c544 95fe  .......=..Xi.D..
 00000060: 0100 004d 0400 0008 0000 006d 6574 612e  ...M.......meta.
 00000070: 786d 6c8d 944f 8f9b 3010 c5ef fd14 88ee  xml..O..0.......
 00000080: d5d8 2624 2116 61a5 1eaa aada 6a2b 6d2a  ..&$!.a.....j+m*
 00000090: f516 3966 42bc 051b 19b3 6cbf 7dcd df25  ..9fB.....l.}..%
 000000a0: bb39 f482 c49b dfcc 7b1e 2c92 fbd7 b2f0  .9......{.,.....
 000000b0: 5ec0 d452 abbd 4f03 e27b a084 cea4 caf7  ^..R..O..{......
 000000c0: feaf c357 14fb f7e9 a744 9fcf 5200 cbb4  ...W.....D..R...
@@ -33,805 +33,805 @@
 00000200: f210 62be f9b5 7507 a9ad 145e af5b 7e2a  ..b...u....^.[~*
 00000210: 0009 dd28 ebbe a63f 88b2 e4f9 2c92 51d4  ...(...?....,.Q.
 00000220: a72e ce7b b55a 9074 d60c cf0d af2e 5321  ...{.Z.t......S!
 00000230: 1a0b ad36 d90c 4f13 c4c5 e1c2 8299 2a71  ...6..O.......*q
 00000240: 3c56 94fb baed 455a a82b 2e9c cb07 90fa  <V....EZ.+......
 00000250: b8df 8095 b680 f459 9fea e0bb 7b3c baeb  .......Y....{<..
 00000260: d9dd d77e 0d43 2dc1 5777 14df fa1f a4ff  ...~.C-.Ww......
-00000270: 0050 4b03 0414 0000 0008 0073 2e6e 5807  .PK........s.nX.
-00000280: 588d 1895 0d00 0028 6f00 000b 0000 0063  X......(o......c
-00000290: 6f6e 7465 6e74 2e78 6d6c ed5d db72 db38  ontent.xml.].r.8
-000002a0: 127d 9faf 6069 6a76 3353 cbbb aede c453  .}..`ijv3S.....S
-000002b0: 8aad 899d d84e caf2 642f 6f10 0949 1893  .....N..d/o..I..
-000002c0: 0407 842c db7f b03f b05f b02f f3be 8ffb  ...,...?._./....
-000002d0: e61f db06 6f22 294a a46c 3991 2b4a aa9c  ....o")J.l9.+J..
-000002e0: 10e8 6e1c 341a 7d01 c1e4 f5cf b7ae 23dd  ..n.4.}.......#.
-000002f0: 6016 10ea bd69 e88a d690 b067 519b 7893  `....i.....gQ.x.
-00000300: 378d 191f cbdd 86f4 f3e1 77af e978 4c2c  7.........w..xL,
-00000310: 7c60 536b e662 8fcb 16f5 38fc 2901 bb17  |`Sk.b....8.)...
-00000320: 1c44 bdc0 c0bc 038a 0212 1c78 c8c5 c101  .D.........x....
-00000330: b70e a88f bd84 eb20 4b7d 100e 16b5 04fc  ....... K}......
-00000340: cea9 cd1e 1267 b939 bee5 7599 056d 8e17  .....g.9..u..m..
-00000350: 8dea 8f1c 1267 b96d 86e6 7599 052d 6835  .....g.m..u..-h5
-00000360: cb3e a675 996f 0347 1e53 d0ba eb23 4e0a  .>.u.o.G.S...#N.
-00000370: 286e 1de2 5dbf 694c 39f7 0f54 753e 9f2b  (n..].iL9..Tu>.+
-00000380: 7353 a16c a2ea bd5e 4f0d 7b53 c056 4ae7  sS.l...^O.{S.VJ.
-00000390: cf98 1352 d996 8a1d 2c06 0b54 5dd1 d584  ...R....,..T]...
-000003a0: d6c5 1cd5 c527 68b3 90bc 993b c2ac b66a  .....'h....;...j
-000003b0: 1047 4bab 1adc 4c6a 5bc4 cd64 856a ac29  .GK...Lj[..d.j.)
-000003c0: 62b5 6d23 24ce 2faf 69d7 5f5e d3ce f2ba  b.m#$./.i._^....
-000003d0: 884f 57ac 4957 3d87 cef0 c7f9 d9c2 1698  .OW.IW=.........
-000003e0: 5b77 2c41 9b53 95c5 885f 7b9a 1175 969f  [w,A.S..._{..u..
-000003f0: 529a 4215 0cd1 060d e11a 9ad6 54a3 e70c  R.B.........T...
-00000400: f57c 2df9 9c11 8e59 86dc 5a4b 6e21 c74a  .|-....Y..ZKn!.J
-00000410: 354e dd32 a501 9dae 0285 8c6f 8499 a686  5N.2.......o....
-00000420: 2f14 11ac 6030 d4a8 3b25 0eec 95a2 ff7e  /...`0..;%.....~
-00000430: 7e36 b4a6 d845 0b62 524d 2c13 2fe0 c85b  ~6...E.bRM,./..[
-00000440: 6886 8945 5839 d396 cab0 4f19 4f15 33ae  h..EX9....O.O.3.
-00000450: ef30 61b5 8c14 db94 bbce eaed 2e7a 13d2  .0a..........z..
-00000460: 09b3 ed52 5280 63aa b0f5 61e3 c937 04cf  ...RR.c...a..7..
-00000470: bf6f e43c f97a 83e8 150c 2274 8b55 2c21  .o.<.z...."t.U,!
-00000480: 51d6 6fae 65d0 3555 d0a4 db18 4c64 e1e4  Q.o.e.5U....Ld..
-00000490: d924 8d43 633a f360 1210 bc62 05e2 5b1f  .$.Cc:.`...b..[.
-000004a0: 3322 ba90 13b2 1de4 2464 adde a18f 1019  3"......$d......
-000004b0: c7ae 8c84 9c43 27d8 493c 463a a552 3194  .....C'.I<F:.R1.
-000004c0: ca6e 0006 041b 85fa 0719 ee7c 7c60 ee6d  .n.........||`.m
-000004d0: 3d71 6273 507b 5c94 5870 1456 1098 bccc  =qbsP{\.Xp.V....
-000004e0: 1eae 2e55 d127 8bf0 0801 201e 2993 1718  ...U.'.... .)...
-000004f0: 8dc3 2407 88fc 4770 f85a 2d36 c4cf 63c8  ..$...Gp.Z-6..c.
-00000500: 0de4 31b2 b06c 63cb 81f6 c8b7 a7cd 52f4  ..1..lc.......R.
-00000510: 2ce6 f1a6 7185 a6d4 4566 4302 279e 90b8  ,...q...EfC.'...
-00000520: c4b9 4b7a 605c b5c0 5f47 e06a 7952 8e59  ..Kz`\.._G.jyR.Y
-00000530: 74c9 13ec 812e c14b 0573 1204 9b8f 08cb  t......K.s......
-00000540: 1048 1778 2e5d c200 5ec9 d07f 2e90 fc79  .H.x.]..^......y
-00000550: 2d0a 164b 5950 f884 5b10 4d6e 1023 e136  -..KYP..[.Mn.#.6
-00000560: da14 611f f89c 125c 497b 9546 b68e 45af  ..a....\I{.F..E.
-00000570: 0506 d994 7961 62f2 a671 01a6 fcc5 b146  ....yab..q.....F
-00000580: 2653 06b6 b631 6d15 4ede 8aca 706d 6669  &S...1m.N...pmfi
-00000590: db87 3824 ee70 56b6 05d2 8e35 68ee 028e  ..8$.pV....5h...
-000005a0: dd67 5840 e391 0bf8 383c ea2a 3718 b7a3  .gX@....8<.*7...
-000005b0: 1987 9139 b1e4 9035 f58f e1cf 1c7a 9fda  ...9...5.....z..
-000005c0: 5751 d88c 0789 b147 b1f4 f03b 29e6 0c9f  WQ.....G...;)...
-000005d0: 651f fc3e 669c c0f2 4785 0a72 c804 9cb7  e..>f...G..r....
-000005e0: 8bd8 0432 9586 0a65 9c9a 190a 1ed7 0c7c  ...2...e.......|
-000005f0: 841d a774 5cd9 123d c5c1 4563 16c1 981e  ...t\..=..Ec....
-00000600: f8c8 8eca 484d d12d 5023 348d 28b3 4559  ....HM.-P#4.(.EY
-00000610: a029 5acb e752 401d 624b df6b e1af 0df1  .)Z..R@.bK.k....
-00000620: 9d60 648b 24f3 4b22 0c09 9075 3d61 2247  .`d.$.K"...u=a"G
-00000630: 8092 c3a1 40fa 3d6e 8bdf 1be2 ffd5 1b31  ....@.=n.......1
-00000640: 8cae 05b4 4b3a 2f9f 0783 8ee2 34a0 ad30  ....K:/.....4..0
-00000650: 8b6b 8c7d 99d3 09e6 5381 1c39 7374 b7e9  .k.}....S..9st..
-00000660: 6a9f ba68 82cf f098 1781 4c18 f2a7 c44a  j..h......L....J
-00000670: 9a7d c444 f51f 3ec8 11f7 bb88 22c8 208d  .}.D..>.....". .
-00000680: 99b2 38a3 0e36 f364 3e05 ed4d 6013 4172  ..8..6.d>..M`.Ar
-00000690: 8223 4d26 d2e7 c007 7010 438e 8353 eb8b  .#M&....p.C..S..
-000006a0: 6a49 5974 fad8 9645 7738 0004 058f ca0e  jIYt...Ew8......
-000006b0: 7109 cf0a 088f 26e8 0c34 3146 4e90 ee9d  q.....&..41FN...
-000006c0: 1b01 04b2 40d9 a7c0 c8a9 bfd4 c1b0 130d  ....@...........
-000006d0: 1e4a 4fba a794 917b 2ab2 ac88 d3c9 2829  .JO....{*.....()
-000006e0: d357 ceec 12c6 8489 78d4 c3a1 f558 0e81  .W......x....X..
-000006f0: 1932 6cf1 579a e5fe 45ca fdf8 3124 89b6  .2l.W...E...1$..
-00000700: abcc c864 ca85 1d9a b165 c6ed 23ca b928  ...d.....e..#..(
-00000710: 9234 c580 8e47 acf2 a510 bc5f e68a 6566  .4...G....._..ef
-00000720: 592d 3de7 3a0b 7bda e632 7fd2 8b6b bb84  Y-=.:.{..2...k..
-00000730: b664 7563 6f9a 84a2 9425 b3b6 870b 3704  .duco....%....7.
-00000740: acd4 5f6a 48a4 d380 f0a8 6a30 7b4a b3e9  .._jH.....j0{J..
-00000750: a611 94df f930 9485 4589 b288 9c09 7ba5  .....0..E.....{.
-00000760: 38a3 d356 7add a2b8 68a1 4aa4 a94b 70d5  8..Vz...h.J..Kp.
-00000770: 7593 cba9 77b5 768d 67d2 ae58 7a51 7cc9  u...w.v.g..XzQ|.
-00000780: 71d0 c68b edf2 db2c e064 7c27 0710 aa40  q......,.d|'...@
-00000790: e41c 2254 62f4 fb35 116b 623e 664d 861c  .."Tb..5.kb>fM..
-000007a0: 4199 cfec 850e 85f6 330b 929e 8464 c041  A.......3....d.A
-000007b0: 390c bad7 34dd b68d ee28 33c3 3c6f 6de4  9...4....(3.<om.
-000007c0: cd2f 644d f1fa 7ef3 0655 bed2 a0ac 3057  ./dM..~..U....0W
-000007d0: 0fc8 3d8c a537 7dde 48db e638 8ac3 23ea  ..=..7}.H..8..#.
-000007e0: d88d b536 61e8 1db3 bd70 0f89 4019 0504  ...6a....p..@...
-000007f0: 7989 d84c 6724 39e9 8ee4 1779 c5a1 b683  y..Lg$9....y....
-00000800: 6f57 73a7 0421 ff93 edb1 b5da 1eab cc2d  oWs..!.........-
-00000810: 1fce 5cb7 2c97 c9b7 c27a 2db5 a561 2f6e  ..\.,....z-..a/n
-00000820: 7688 87e5 69bc 06ba a6fd d028 9a76 c011  v...i......(.v..
-00000830: e38b 56e2 d960 7ab1 808c 3244 d115 f848  ..V..`z...2D...H
-00000840: bca4 2236 a6d1 0c90 e34f d312 d09f 7916  .."6.....O....y.
-00000850: 9f85 077f 7294 a14c 9107 9826 0941 8825  ....r..L...&.A.%
-00000860: 4cda c5a8 5021 66f2 11b0 5e6f 22bb d406  L...P!f...^o"...
-00000870: f90e 93f9 a86c 276d cb58 a777 fe14 7b88  .....l'm.X.w..{.
-00000880: e3c5 ae7d daba 5f2d e50c 4250 0dcf 98da  ...}.._-..BP....
-00000890: 7ea7 65b7 cda7 e358 8aae 6b71 14f6 ad56  ~.e....X..kq...V
-000008a0: d822 b9dd 57da b9d8 5ea2 fbc9 e897 e2d0  ."..W...^.......
-000008b0: c6e8 8b5e c75b 3ef4 5a3b abbc 4f59 c59d  ...^.[>.Z;..OY..
-000008c0: 9ff6 3aaf 124b 78b2 6696 e2dc 269a 69af  ..:..Kx.f...&.i.
-000008d0: 5bd7 d2ce c504 dbdb 58d7 25af b816 7dd4  [.......X.%...}.
-000008e0: 3a0b 20b0 8233 826a 3dc4 159f 1570 36c3  :. ..3.j=....p6.
-000008f0: 39bf 4467 5cf8 9542 1513 7685 fe26 2ea3  9.Dg\..B..v..&..
-00000900: a204 2029 3056 1145 c172 8966 115d b51f  .. )0V.E.r.f.]..
-00000910: a4c8 8966 3496 3f35 5f61 950e e610 cf65  ...f4.?5_a.....e
-00000920: e141 c303 93c4 b444 1778 c919 d495 6f1a  .A.....D.x....o.
-00000930: 765c fb40 adc7 19a8 e978 9091 97e0 4ff9  v\.@.....x....O.
-00000940: 4268 c114 d9e2 6de2 1266 2817 310b 2797  Bh....m..f(.1.'.
-00000950: 9bf9 fa0d 52e0 8cdc b1a8 1389 37a3 b320  ....R.......7.. 
-00000960: aff8 9b3a 5439 f5ae a28c 9573 8d99 172a  ...:T9.....s...*
-00000970: 27bb c8a9 8a13 8b2d 3907 cd19 b4b1 30e8  '......-9.....0.
-00000980: 44b3 49df 7d9a 15c6 2a4e 3a8e 2ef2 f2c2  D.I.}...*N:.....
-00000990: 6471 b513 a8f4 1221 de74 132d ce50 576e  dq.....!.t.-.PWn
-000009a0: b332 d069 ef94 1461 a75d a765 c08b dea7  .2.i...a.].e....
-000009b0: 8683 ca2e 1976 21a8 47e6 bb64 5581 851c  .....v!.G..dU...
-000009c0: 9c24 1219 b150 d513 3c2e 6148 ad64 d5fe  .$...P..<.aH.d..
-000009d0: 4b09 e20d bed8 ec4f f73b e2bc cfd0 dba3  K......O.;......
-000009e0: 3632 bb66 57d7 9a4d 6474 ed76 d3d0 bba3  62.fW..Mdt.v....
-000009f0: 56ab a599 a839 2e3f 1a5e 5d3c a447 ca99  V....9.?.^]<.G..
-00000a00: fc24 7f76 1ca7 34c4 16f7 178c 4ec7 4a13  .$.v..4.....N.J.
-00000a10: 29d0 921c b783 0615 a1c3 e8a0 3992 1127  )...........9..'
-00000a20: 64d1 0159 ee04 3a6a 2a66 7e8a a959 a569  d..Y..:j*f~..Y.i
-00000a30: a2a2 69ab 0e43 8a2c c9e9 49c8 a1d6 d5ac  ..i..C.,..I.....
-00000a40: 8bb9 0e8a 5877 78bc f6e8 38ea 4b4f 9492  ....Xwx...8.KO..
-00000a50: 7376 62db 0eae 3824 ae75 c69c 3997 3637  svb...8$.u..9.67
-00000a60: 9e99 f1bc 337b 3eec b5ec 5d59 4e55 a389  ....3{>...]YNU..
-00000a70: 5067 e67a c5d9 858d 25e7 9360 c871 5f62  Pg.z....%..`.q_b
-00000a80: cf7a a7d7 fe69 db58 97d3 d9ad 60ed b47b  .z...i.X....`..{
-00000a90: cdad 635d 4e5e 7717 eb72 3af9 d5b0 6add  ..c]N^w..r:...j.
-00000aa0: 9636 d60d b3d3 eb69 cd4e a735 42cd 76cb  .6.....i.N.5B.v.
-00000ab0: 302c 645b 1da3 d7e9 ecfd f323 fc73 2dcd  0,d[.......#.s-.
-00000ac0: ee92 27a8 c4ba 439e a012 eb0e 7982 4aac  ..'...C.....y.J.
-00000ad0: 3be4 095a 48eb b5c6 a6a1 37c7 ad66 0f75  ;..ZH.....7..f.u
-00000ae0: bb1d dcb4 b41e b6c7 e2b7 516e ad7b 4fb0  ..........Qn.{O.
-00000af0: 05cd ee92 27a8 c4ba 439e a012 eb0e 7982  ....'...C.....y.
-00000b00: 4aac 3be4 09da 23b3 db1b 75f0 c8b4 b5a6  J.;...#...u.....
-00000b10: 618f baed b68e b576 778c ac96 868c dede  a......vw.......
-00000b20: 133c d613 5469 7697 3c41 25d6 1df2 0495  .<..Tiv.<A%.....
-00000b30: 5877 c813 5462 dd21 4f60 60ab a3b5 4708  Xw..Tb.!O``...G.
-00000b40: f295 5e73 d4ee f4b0 ae9b e3b6 6e8f 3464  ..^s........n.4d
-00000b50: 8eac f23a 7def 09b6 a0d9 5df2 0495 5877  ...:}.....]...Xw
-00000b60: c813 5462 dd21 4f50 89f5 cb7a 0275 e5fd  ..Tb.!OP...z.u..
-00000b70: deb8 6344 edbb f441 1c0a 1fbe 0e3f 470c  ..cD...A.....?G.
-00000b80: f0ef 33ec 2dee 092f 374a 6193 4d02 df41  ..3.-../7Ja.M..A
-00000b90: 77c9 3b23 d83e 37e2 369a d688 ba23 cd9c  w.;#.>7.6....#..
-00000ba0: 3ace 2ce0 2c7c 8f2d 8ea0 9785 3d71 80c4  :.,.,|.-....=q..
-00000bb0: 013d 83e4 e8b5 daf6 051f 479f 5eae 925d  .=........G.^..]
-00000bc0: d298 acc2 3412 53f0 c127 462c be30 aad1  ....4.S..'F,.0..
-00000bd0: 381c d27b 829c 3961 3cb0 a668 cca5 37d2  8..{..9a<..h..7.
-00000be0: 9f7e 9f51 fe57 17fd 46d9 c31f 41f4 148f  .~.Q.W..F...A...
-00000bf0: 3985 6116 3e38 76bb 1b9d fe47 2c59 7cf5  9.a.>8v....G,Y|.
-00000c00: 1873 03c7 06fe 5861 e06b d5ad ca33 b62c  .s....Xa.k...3.,
-00000c10: cfdc b2bc 6651 de34 bc92 25ee 6607 f90e  ....fQ.4..%.f...
-00000c20: 6829 8c8c 1da7 64dc e48d 446c 767e b9d9  h)....d...Dlv~..
-00000c30: 85a3 888b f947 d1d7 d760 6e1c 9e70 6c4d  .....G...`n..plM
-00000c40: e23e 5471 ac67 1dbd cf46 9870 ccbf d6f8  .>Tq.g...F.p....
-00000c50: 9f18 1de1 7b80 f0b5 007c 409e 4d6c 040f  ....{....|@.Ml..
-00000c60: 6b11 a84b 26a1 6edb 7a8c 4af8 39e0 1121  k..K&.n.z.J.9..!
-00000c70: 92c2 8fc3 e34b 7601 112f 551b 71db 9489  .....Kv../U.q...
-00000c80: 17a2 c798 23e2 c044 81d9 c32c 9e25 3a94  ....#..D...,.%:.
-00000c90: 60e1 a54d 855c ca47 7716 b8b9 2144 5836  `..M.\.Gw...!DX6
-00000ca0: 99f1 808a 40cb ee01 119b b90b d9af f41f  ....@...........
-00000cb0: 63d9 818f bce5 c9c0 74cd 70ba 433c 6592  c.......t.p.C<e.
-00000cc0: f868 1b64 6637 8260 3bdc 824d 3cb3 522f  .h.df7.`;..M<.R/
-00000cd0: fbc7 83cb f3fe d1c9 e052 3a9a 3212 7002  .........R:.2.p.
-00000ce0: d37d a5b7 5a3f a6ca 58e8 0174 4e02 49eb  .}..Z?..X..tN.I.
-00000cf0: 299a a1e8 ad97 35d3 5ffa ff38 ff78 f1f9  ).....5._..8.x..
-00000d00: f4ec 6c20 9dcd 2c98 a3a9 fd94 99e4 ce4f  ..l ..,........O
-00000d10: e0fd a07f f1f0 aff3 fee5 95f4 fee1 0ff6  ................
-00000d20: f05f 17c3 24ba 7acd 392c 3b80 1ddd e6d4  ._..$.z.9,;.....
-00000d30: 9a3e 6d8f 834b 96fa d79c dc48 9f15 aabc  .>m..K.....H....
-00000d40: 5372 bb7a f7d7 f973 ff42 fa3c 18c0 0fe2  Sr.z...s.B.<....
-00000d50: 893b cc80 badd 5ebd 1b0d 43d1 cce2 6e0c  .;....^...C...n.
-00000d60: ffba b82c 9a58 46b6 65cb dba7 804a ef28  ...,.XF.e....J.(
-00000d70: baae e8cd 97e5 2306 30c5 aba1 fcae 3fbc  ......#.0.....?.
-00000d80: 9206 cc43 c211 1a2f ca47 f48f 3ebe 1d4a  ...C.../.G..>..J
-00000d90: ef91 0585 8458 6db1 4e9d 477b 886c cb63  .....Xm.N.G{.l.c
-00000da0: ab91 5371 0b3f c94d aa8a 8dea 57d9 2bf2  ..Sq.?.M....W.+.
-00000db0: e54a c64d 92ef 1aaf 7d37 4ae6 6bbc 9add  .J.M....}7J.k...
-00000dc0: aebc 0d8b 8d1a af38 f7c5 c6be d8f8 a68a  .......8........
-00000dd0: 8d27 6721 6f4f 87fd 1796 7964 8b81 5f18  .'g!oO....yd.._.
-00000de0: e1f7 22fe 75d7 4479 917b bcbc 4aa0 ffeb  ..".u.Dy.{..J...
-00000df0: f078 70fe b7fe d9b1 d477 c6d4 0b60 9a7a  .xp......w...`.z
-00000e00: fb25 85f9 f3c1 6038 840c f11c 627c 1088  .%....`8....b|..
-00000e10: 34a5 f9f8 20bf a31b f0e1 7f96 f8c2 2808  4... .........(.
-00000e20: a026 0509 fbb2 7f9b da3d eb9f bf1d 5c5e  .&.......=....\^
-00000e30: fd53 7a37 2336 15f6 63ac d9e5 5d45 378a  .Sz7#6..c...]E7.
-00000e40: b9fc f62b 8cc8 fb0c 8e3e 80f7 b924 d700  ...+.....>...$..
-00000e50: aa63 ae39 8468 2b5a f3c5 b99e b797 83a3  .c.9.h+Z........
-00000e60: 932b e92d 64c4 b698 60dd 5dbb 13e0 df7f  .+.-d...`.].....
-00000e70: bce8 436d 4103 3c16 6545 efab 9615 835b  ..CmA.<.eE.....[
-00000e80: 5156 48af 1efe 3d1e c36c 1c45 fa4c 0792  QVH...=..l.E.L..
-00000e90: 4bb8 f481 0a87 c1c0 7f5c 6316 70c4 f9cc  K........\c.p...
-00000ea0: 9b24 58ab 0a90 ea1b 742b 72e8 4ac6 4d12  .$X.....t+r.J.M.
-00000eb0: f21a b7cd 364a f06b dc08 dbae bc0d 0b90  ....6J.k........
-00000ec0: 1a37 abf6 05c8 be00 f9a6 0a90 ade6 3f6b  .7............?k
-00000ed0: 8f44 eb65 3c17 540a 6690 3edd 1048 9e14  .D.e<.T.f.>..H..
-00000ee0: e9a3 e7dc 4963 ca24 f1b5 bbf8 e742 c549  ....Ic.$.....B.I
-00000ef0: a58f 2940 505e 564c 3e39 3d7b 37b8 1c4a  ..)@P^VL>9={7..J
-00000f00: 27c4 b1f1 0431 1198 cd35 9987 a9bd c4a3  '....1...5......
-00000f10: cd47 06ef 8db0 bfe0 72e3 4a78 7536 7ff8  .G......r.Jxu6..
-00000f20: 4f00 bbee 89ef 189f b1f2 df55 ebfa d03f  O..........U...?
-00000f30: fd2c f6d0 07c4 1c51 4dd4 7d29 b513 e0a3  .,.....QM.})....
-00000f40: 537f e918 7904 0bf4 4677 2732 db4f 8cdc  S...y...Fw'2.O..
-00000f50: a027 a6b3 d5d7 c057 6464 958c 9ba4 7735  .'.....Wdd....w5
-00000f60: ae4c 6f94 2ed6 b8d6 bc5d 791b a6b3 35ae  .Lo......]y...5.
-00000f70: 07ef d3d9 7d3a fb2d a5b3 db8c af1b 1ce6  ....}:.-........
-00000f80: ed7e f039 ef9f 9d0f 2e8e 4f07 97d2 3962  .~.9......O...9b
-00000f90: e2bd 7a73 cdcb 7edd 5034 fdf9 5ff6 1f0f  ..zs..~.P4.._...
-00000fa0: 2e3e 5e48 c7d8 23e2 6cbc bbee 45bf d654  .>^H..#.l...E..T
-00000fb0: b4d6 8b3b 871b 5cbc 1b9c 0da5 810d f9be  ...;..\.........
-00000fc0: 88f8 cf92 0e3f 17f8 ec6b 9ae4 fcb6 f575  .....?...k.....u
-00000fd0: 4fe3 86d4 0b38 99e0 9a69 49f5 3729 2b22  O....8...iI.7)+"
-00000fe0: 6b25 e326 61ba c6f7 1b9b ddd9 adfe c662  k%.&a..........b
-00000ff0: bbf2 36bd 535c fdad c23e 2dd9 a725 df52  ..6.S\...>-..%.R
-00001000: 5ab2 953b c5df 60bd 9f0d 4127 d826 e28e  Z..;..`...A'.&..
-00001010: e2cb aaf9 1f99 00d4 0a9f 2578 3f99 8dac  ..........%x?...
-00001020: e0dc 0758 6aee db2c 75c5 7f73 77f8 7f50  ...Xj..,u..sw..P
-00001030: 4b03 0414 0000 0008 0073 2e6e 5880 2079  K........s.nX. y
-00001040: 0360 0600 0016 2b00 000c 0000 0073 6574  .`....+......set
-00001050: 7469 6e67 732e 786d 6cb5 5a51 77da 3a0c  tings.xml.ZQw.:.
-00001060: 7ebf bfa2 87f7 8e96 756d e1b4 dd01 5ab6  ~.......um....Z.
-00001070: 6eb4 7008 5bcf dd9b 4904 f8e2 5839 b653  n.p.[...I...X9.S
-00001080: cabf 9fec 00eb 28b9 6349 fc44 9b38 9223  ......(.cI.D.8.#
-00001090: e9fb 2459 b9fa f812 8ba3 6750 9aa3 bcae  ..$Y......gP....
-000010a0: 9dbe 3ba9 1d81 0c31 e272 765d fb36 ee1d  ..;....1.rv].6..
-000010b0: 5fd6 3ede fc73 85d3 290f a115 6198 c620  _.>..s..)...a.. 
-000010c0: cdb1 0663 6889 3ea2 c7a5 6e65 b7af 6ba9  ...ch.>...ne..k.
-000010d0: 922d 649a eb96 6431 e896 095b 9880 dc3c  .-d...d1...[...<
-000010e0: d67a bdba e594 6557 5e04 978b ebda dc98  .z....eW^.......
-000010f0: a455 af2f 97cb 77cb f7ef 50cd eaa7 cd66  .U./..w...P....f
-00001100: b3ee ee6e 9686 28a7 7c76 a8aa 6cf5 6b55  ...n..(.|v..l.kU
-00001110: 88b8 5564 1fc8 36e3 9435 4e4e ceea d9ff  ..Ud..6..5NN....
-00001120: b5a3 f526 5f99 a651 bbd9 d861 f3fa 3757  ...&_..Q...a..7W
-00001130: 6b05 d9cf 3137 105b db1c ad2f dbad 5dd7  k...17.[.../..].
-00001140: 4865 eb99 c372 6bb5 dabe e77e 7fe6 3bad  He...rk....~..;.
-00001150: 6f2b 6063 4c6a 9b3b 6695 d01d 8172 56bb  o+`cLj.;f....rV.
-00001160: 39b9 aabf 1571 b8d8 3e4c 8d0f b94f 3c32  9....q..>L...O<2
-00001170: f3bd 82df 7f68 bc6f 9413 fe19 f86c be7f  .....h.o.....l..
-00001180: dba7 e797 27a7 c5a4 0773 5c8e 20a2 1883  ....'....s\. ...
-00001190: ee9c c919 e81d 0d13 4401 4cd6 6e8c 4aa1  ........D.L.n.J.
-000011a0: 988e 7bd9 51b8 d4f0 8011 e449 9f32 a10f  ..{.Q......I.2..
-000011b0: 167f 1cb3 e498 cb08 5e20 7a6b acfd 01e6  ........^ zk....
-000011c0: 9e21 68a8 d561 26bf 8f76 b6aa 8de2 d6d8  .!h..a&..v......
-000011d0: 3696 4bb8 3237 f64e cf1b e725 e22f 0f2a  6.K.27.N...%./.*
-000011e0: 8d93 cbc2 5235 9f08 a81e 2c4e 6ce5 d076  ....R5....,Nl..v
-000011f0: 5247 b918 b108 2c27 bb83 c660 9ce3 bb8b  RG....,'...`....
-00001200: 66b3 98f0 1f88 f198 44ed 46db 1c95 a15d  f.......D.F....]
-00001210: 9708 34b6 c2d4 7451 a4b1 dc05 f55a 7a89  ..4...tQ.....Zz.
-00001220: 70cb a477 1017 95a1 faad 5d7a 2c34 a8f6  p..w......]z,4..
-00001230: efbd 7959 908c 7400 0242 0351 4fd1 8502  ..yY..t..B.QO...
-00001240: 3bdf 73f1 35b9 e4dd 5ef3 d5fe 0594 1b0f  ;.s.5...^.......
-00001250: cfa6 d985 5431 43b9 f96f d2ea 9018 cc0c  ....T1C..o......
-00001260: 15ea 840c e0c1 674e bee5 8b21 f392 48b2  ......gN...!..H.
-00001270: fd93 ec0e 0b17 3385 a9dc 25e9 aa94 7491  ......3...%...t.
-00001280: 9c89 c2d7 3bb4 a544 e3dc b707 3de5 c0e9  ....;..D....=...
-00001290: e47f 522c 99f3 d0d7 f61d cbfa f471 8fbd  ..R,.........q..
-000012a0: 3cbe 05e7 3a03 d70f 0e94 0454 4f61 1c80  <...:......TOa..
-000012b0: 4977 934d 65e1 3e86 1733 142c 8439 8a08  Iw.Me.>..3.,.9..
-000012c0: 76c9 aa0a 35ed 2411 ab21 536c 66bd fac0  v...5.$..!Slf...
-000012d0: d4a2 872a 6666 8c8f 693c 0167 134f 2f37  ...*ff..i<.g.O/7
-000012e0: 02db 0140 2eca 4ac8 1fb3 c980 84d3 ebcc  ...@..J.........
-000012f0: b8f4 20ff 8e4c 13f5 08c6 b931 5a42 7890  .. ..L.....1ZBx.
-00001300: 2ac7 3ed6 f94f e495 2066 4278 d0f3 8be7  *.>..O.. fBx....
-00001310: acff adbd 6e15 5b3a b6af 5e59 57f0 2481  ....n.[:..^YW.$.
-00001320: 68c8 4393 aa7c 6897 d0d0 13c8 8c61 544b  h.C..|h......aTK
-00001330: 3d62 ec1c ef43 cb37 39a1 7669 e1d4 6c00  =b...C.79.vi..l.
-00001340: e243 8f8b b060 a5e9 86af 385b 8364 2a70  .C...`....8[.d*p
-00001350: e98d bfac 9d7c f178 40a6 17f0 0527 5e40  .....|.x@....'^@
-00001360: 6841 d765 891e 820a a9f8 a27c 747e 5efd  hA.e.......|t~^.
-00001370: 8b50 052d 4809 dcc5 8959 7541 080b c5ea  .P.-H....YuA....
-00001380: d53c 3033 ef30 0db6 136f 0b3e 93f6 1cc7  .<03.0...o.>....
-00001390: 4736 89b2 c277 309d 52e5 e8c3 2ff7 bacf  G6...w0.R.../...
-000013a0: 2620 6ed7 6751 be02 1754 a912 6190 1a6b  & n.gQ...T..a..k
-000013b0: ea3e 6538 f12f 0711 699f d9f4 7e26 5141  .>e8./..i...~&QA
-000013c0: 8f2b 6dfa a4f5 9e7a 0169 eea5 4f95 df92  .+m....z.i..O...
-000013d0: 8819 b0f5 cf18 e244 d0df 9e40 dea1 ea67  .......D...@...g
-000013e0: e191 01a9 abc7 e557 001f 259c e3f0 08a2  .......W..%.....
-000013f0: 5b46 6989 d057 2aa4 3227 d38e 755b 4664  [Fi..W*.2'..u[Fd
-00001400: 15b9 d054 a959 7f77 9908 53e1 0a7e 1f9e  ...T.Y.w..S..~..
-00001410: d630 10d1 1a14 0f40 fbcd affc cbc4 b0a4  .0.....@........
-00001420: 5444 2dbf a232 3748 58e8 276c 03f6 0c9f  TD-..27HX.'l....
-00001430: 044e d896 40c8 800b 4fa1 a547 60bd f20c  .N..@...O..G`...
-00001440: 63cc 2059 3d44 469a ef96 cfe4 a7da 4de3  c. Y=DF.......M.
-00001450: e2c3 e9c5 45c1 83c4 df1a f9d1 b8ef 8b63  ....E..........c
-00001460: 5dce f3d4 e8b9 b686 4257 59ec 79a2 a6cf  ].......BWY.y...
-00001470: 9cc0 2d6d 95ee 2793 da52 c031 d41a 0f6d  ..-m..'..R.1...m
-00001480: 1318 a67c 28eb d914 d54e 0d66 b45e bdbd  ...|(....N.f.^..
-00001490: 3212 f199 90f6 d8cb 43b5 3627 1521 f160  2.......C.6'.!.`
-000014a0: 17e3 84ba 183b beca 3f5e 2d78 c662 39ea  .....;..?^-x.b9.
-000014b0: 7b36 1a1b c8ae 40ed e300 d4be 89f1 e9f1  {6....@.........
-000014c0: 75c2 b0c4 6747 8796 69dd a16e cedc 63ce  u...gG..i..n..c.
-000014d0: 67f3 63b2 288a d4e6 b1a2 b5e1 5750 b2ad  g.c.(.......WP..
-000014e0: 3993 c354 52a3 e931 27da 5312 5083 c97f  9..TR..1'.S.P...
-000014f0: c491 43d4 dc6a aa2a b2f3 2750 a475 e258  ..C..j.*..'P.u.X
-00001500: 671b 89e5 e751 7d26 6729 b170 8e67 a2c2  g....Q}&g).p.g..
-00001510: 9d4d 6af5 e748 bdbd 2b38 1d60 8abc 9b13  .Mj..H..+8.`....
-00001520: 4507 5451 1d98 7169 8ba6 c212 ee64 f4bf  E.TQ..qi.....d..
-00001530: cf97 3dc0 3f80 e888 1d0c 0f99 f0dc 6a05  ..=.?.........j.
-00001540: e9c4 d820 eb89 15d5 9c21 911a 446d f79f  ... .....!..Dm..
-00001550: 877c 9dd1 f79a b9c7 e878 dcf6 c37e 74dd  .|.......x...~t.
-00001560: bd10 7424 137d 6091 9f4c 912a 451e df54  ..t$.}`..L.*E..T
-00001570: fef6 37c0 5485 c5e3 ae2d 042e 1dab 7ec1  ..7.T....-....~.
-00001580: 4997 c910 72cf 04cb b036 1a22 344b 6e3e  I...r....6."4Kn>
-00001590: 69d3 02c8 5f91 ef8c f4a7 a3cc 52b5 4cf6  i..._.......R.L.
-000015a0: 169b f3d9 c453 8b2d 5f48 4f08 3f40 21c5  .....S.-_HO.?@!.
-000015b0: eb1f 42b5 5cab d276 83b5 ac4b 21a5 db79  ..B.\..v...K!..y
-000015c0: 80be 27b2 d43e 4ace f567 21eb 80a3 e4f9  ..'..>J..g!.....
-000015d0: 1576 7385 05ce f959 874b 4669 e4a0 b90c  .vs....Y.KFi....
-000015e0: 26af 222b 982b dbdb 6d8f 457c 5451 28a9  &."+.+..m.E|TQ(.
-000015f0: 01fb 1509 0349 0501 5503 3eec 458a 4688  .....I..U.>.E.F.
-00001600: bbae 70dd de69 f3c3 d9d9 59c1 697e 6056  ..p..i....Y.i~`V
-00001610: 02f4 23de c294 a5c2 87ab 6d8b 9d95 99f9  ..#.......m.....
-00001620: f3c8 821f 18b9 b34c 8adf c060 b2a9 c2aa  .......L...`....
-00001630: 47fc 2d3e a2f9 926a c3a7 2b1b 49fa 899b  G.->...j..+.I...
-00001640: f903 9329 131d 3b0c f060 33a7 7204 94d9  ...)..;..`3.r...
-00001650: 2d16 dbc6 287b da43 0d94 3d0a f311 c9bf  -...({.C..=.....
-00001660: e72b ea6f 6226 a33d bd8d 0bb8 829d 4d1f  .+.ob&.=......M.
-00001670: 5934 221a 4329 de60 bd2a 9b75 5962 074c  Y4".C).`.*.uYb.L
-00001680: 96fe 098b 7a20 876f 4b5b 7f06 2b37 5306  ....z .oK[..+7S.
-00001690: b577 98fc 9734 6827 6d6d bd6d 1036 95db  .w...4h'mm.m.6..
-000016a0: 93a2 a58a aa37 5735 16a1 a8dc 4f4b ea6f  .....7W5....OK.o
-000016b0: 3edd ace7 7dd4 7af3 1350 4b03 0414 0000  >...}.z..PK.....
-000016c0: 0008 0073 2e6e 5882 07ab bed6 0f00 005f  ...s.nX........_
-000016d0: 7000 000a 0000 0073 7479 6c65 732e 786d  p......styles.xm
-000016e0: 6ced 5ddb 8ee3 b619 becf 5318 0a8a 0005  l.].......S.....
-000016f0: 244b f2d9 9871 b0bb 09b0 8bcd 4e16 9901  $K...q......N...
-00001700: 02f4 26d0 48b4 adae 240a 3a8c c7b9 ea53  ..&.H...$.:....S
-00001710: a437 bdea 450b f431 9a37 e993 9447 8992  .7..E..1.7...G..
-00001720: 4859 b23d 33ee a01b 2080 f9ff fcf9 1f3e  HY.=3... ......>
-00001730: 9e7e 929a ab6f 1fc3 60f0 0092 d487 d1b5  .~...o..`.......
-00001740: 6619 a636 0091 0b3d 3fda 5c6b 79b6 d6e7  f..6...=?.\ky...
-00001750: dae0 dbd5 5757 70bd f65d b0f4 a09b 8720  ....WWp..]..... 
-00001760: caf4 34db 0720 1da0 da51 baa4 44c4 9f44  ..4.. ...Q..D..D
-00001770: 4be8 a47e ba8c 9c10 a4cb cc5d c218 44bc  K..~.......]..D.
-00001780: d252 e45e 92b6 6809 11d6 b53a 6116 6b67  .R.^..h....:a.kg
-00001790: e031 eb5a 19f3 56ea 3af7 dd5b 26cc 626d  .1.Z..V.:..[&.bm
-000017a0: 2f71 765d 2b63 5ee4 54b1 fa1a 76ad fc98  /qv]+c^.T...v...
-000017b0: 06fa 1aea 2e0c 6327 f36b 5a3c 067e f4e5  ......c'.kZ<.~..
-000017c0: 5adb 6659 bc1c 0e77 bb9d b11b 1930 d90c  Z.fY...w.....0..
-000017d0: adc5 6231 24d4 4261 b7e0 8bf3 2420 5c9e  ..b1$.Ba....$ \.
-000017e0: 3b04 01c0 8da5 43cb b086 9c37 0499 d355  ;.....C....7...U
-000017f0: 3fcc 2baa 14e5 e13d 483a bbc6 c99c 4654  ?.+....=H:....FT
-00001800: d387 4d67 443c 6c14 ae71 b74e d219 1b84  ..MgD<l..q.N....
-00001810: b91a de91 d73d bc23 4fac 1b3a d956 1193  .....=.#O..:.V..
-00001820: f9f0 1322 92ff 7dfa a1c4 4212 766d 0bf3  ..."..}...B.vm..
-00001830: 565c e526 7edc d94c ca2d d687 1016 aae2  V\.&~..L.-......
-00001840: 0ab4 8312 756d d31c 0fe9 6f81 7bd7 cabe  ....um....o.{...
-00001850: 4bfc 0c24 02bb dbca ee3a 815b 781c 8632  K..$.....:.[x..2
-00001860: a721 3e6b 8838 74f0 8061 cab9 136c b452  .!>k.8t..a...l.R
-00001870: f264 9880 1826 59a1 c8ba fb00 85bc 6317  .d...&Y.......c.
-00001880: dd6b 9b85 81ba 7b61 2a67 dd24 9e27 6545  .k....{a*g.$.'eE
-00001890: ea8c 86a8 ab21 a0eb 0f3e d87d ad55 46ce  .....!...>.}.UF.
-000018a0: f600 2c6a 0120 c3d0 a12a 8449 1ca7 5a2b  ..,j. ...*.I..Z+
-000018b0: 58e6 10f3 14dd 0685 a41c 5493 4d31 ecaf  X.........T.M1..
-000018c0: 611e 2123 d05c c11c 081e 6390 f898 e404  a.!#.\....c.....
-000018d0: a4da b222 4144 5900 8f10 c9e6 0a41 4265  ..."ADY......ABe
-000018e0: 00f5 41c0 7b68 6192 540c 847a 98ea 7e84  ..A.{ha.T..z..~.
-000018f0: 8009 e3a5 50bb 325a a4e9 2893 85ef eea7  ....P.2Z..(.....
-00001900: 21a6 e978 f640 e323 6b47 9835 6d6d c567  !..x.@.#kG.5mm.g
-00001910: c835 44b3 e3da 7181 ee01 3748 5757 7464  .5D...q...7HWWtd
-00001920: 2b8a 07f4 3756 f25a bb73 b630 7446 da00  +...7V.Z.s.0tF..
-00001930: 0d61 9c25 f483 3da7 20b1 c35a fd2e 02d5  .a.%..=. ..Z....
-00001940: f206 95ca 98a4 6f40 841c 85fa 68ba f3d3  ......o@....h...
-00001950: b47f 8bc8 c7e9 e006 ec06 3fa1 0622 49d3  ..........?.."I.
-00001960: dfd4 58be 69d5 2261 524a 8ed8 cf5c 3496  ..X.i."aRJ...\4.
-00001970: 3e38 894f 40dd 57c3 37a8 5e20 d18b 971f  >8.O@.W.7.^ ....
-00001980: f2c8 d975 b13a 29e3 7830 89c8 b47c addd  ...u.:).x0...|..
-00001990: a011 ffd9 75a5 9091 29db 194c 6755 a78a  ....u...)..LgU..
-000019a0: 2299 5efd 9076 7e15 6ffd f036 9775 8182  ".^..v~.o..6.u..
-000019b0: d0a2 cd3e cd40 f804 01b4 8f0c e071 fa0c  ...>.@.......q..
-000019c0: 55c3 202b a7fb 06ae 37f9 7f45 e7cf 4ee2  U. +....7..E..N.
-000019d0: 7cfc f9a6 6897 291c a3e2 4de2 c45b 4e70  |...h.)...M..[Np
-000019e0: 0327 451d 038f c8bc 2844 8b48 90e8 b1b3  .'E.....(D.H....
-000019f0: 013a 15c6 29a8 76b1 6761 a4db cc41 d34e  .:..).v.ga...A.N
-00001a00: e269 abaf 0657 0517 6d43 8fd1 2401 92cc  .i...W..mC..$...
-00001a10: 4758 5ac3 e517 0062 7de7 675b 3d22 3398  GXZ....b}.g[="3.
-00001a20: 13ec 9c7d aa0d d1ae 6828 9881 7eaa 8c8a  ...}....h(..~...
-00001a30: a1f7 dee2 ca78 7e1a 07ce 9ee9 f11e 3878  .....x~.......8x
-00001a40: af35 b00e 5a2c 3182 55d6 be1a 88ff 58cb  .5..Z,1.U.....X.
-00001a50: 4857 b9c5 5c0f b076 f220 d361 9ea1 2d02  HW..\..v. .a..-.
-00001a60: d003 b4b8 428b 174b e6e1 c34e 0a9d 64e3  ....B..K...N..d.
-00001a70: 477a 06e3 6bcd 34c6 f6c8 45d8 29cb ef61  Gz..k.4...E.)..a
-00001a80: 96e1 b59d 69d8 96ed 16b0 7211 4a90 fcdc  ....i.....r.J...
-00001a90: 09f4 3476 5cb2 e95c 3b41 0ab0 7779 9398  ..4v\..\;A..wy..
-00001aa0: a3d6 1a41 57ea ff8a ccb2 46e6 1fb4 a26c  ...AW.....F....l
-00001ab0: 07fc cd16 c5e8 1e06 5e05 bb98 5947 2b3f  ........^...YG+?
-00001ac0: 27e2 5504 22ad c5c9 a46e d5a5 0def 9632  '.U."....n.....2
-00001ad0: f1c6 2300 8f6a a905 0391 db13 3576 3b6a  ..#..j......5v;j
-00001ae0: ec4b 418d ad40 4d3f d88c 26e7 804d 47dc  .KA..@M?..&..MG.
-00001af0: 5893 deb8 2155 fae0 460d 1685 a893 c032  X...!U..F......2
-00001b00: 6a07 cbe8 52c0 323a 0b58 ecf1 ec69 c1e2  j...R.2:.X...i..
-00001b10: c200 26d7 dad7 7313 ffa7 d5f1 338e b3be  ..&...s.....3...
-00001b20: f8c1 5594 03cb 0160 b560 8968 7266 2c8d  ..U....`.`.hrf,.
-00001b30: dbb1 34be 142c 8dcf 8325 0a98 97c2 d242  ..4..,...%.....B
-00001b40: 1c8a 888c 6bcd 47fb 56df ed89 302c a813  ....k.G.V...0,..
-00001b50: c0a8 a759 2dde d4b1 00ec d96a 514f ddee  ...Y-......jQO..
-00001b60: 49d0 9db4 4377 7229 d09d 3c35 742d 737a  I...Cwr)..<5t-sz
-00001b70: de39 73de 7bca 9cf7 9d31 3bcd 9e0a a927  .9s.{....1;....'
-00001b80: a166 da8e 9ae9 a5a0 667a 16d4 3068 3c3f  .f......fz..0h<?
-00001b90: 6a4e 19dd e62f 32ba f56c f589 47b7 cf68  jN.../2..l..G..h
-00001ba0: 77fb 3601 ce97 b760 0d13 a046 e5e1 2ddb  w.6....`...F..-.
-00001bb0: 3d16 a3df 1339 b8e6 0608 8040 4840 28e8  =....9.....@H@(.
-00001bc0: bc0b b3d1 12e4 2443 becb b14b d4e6 c8ba  ......$C...K....
-00001bd0: 90a4 c7a9 3dd4 cc0e 0829 8063 f47e b326  ....=....).c.~.&
-00001be0: a71c a7fa dfc1 629e dffd ef60 9087 1131  ......b....`...1
-00001bf0: e47c 1872 89d0 9e9a bccd 8300 641f c464  .|.r........d..d
-00001c00: 538f 21b6 3e6a 067e da40 046d 0178 3f20  S.!.>j.~.@.m.x? 
-00001c10: 1a51 ae45 9b1b 7272 f994 dad0 16ba 6953  .Q.E..rr......iS
-00001c20: fae6 2300 f1cf 7eb6 bd11 125e 4fea a767  ..#...~....^O..g
-00001c30: ca8b 95fe 7e0e 0b2b be7f 560b 6f71 a17c  ....~..+..V.oq.|
-00001c40: 89f1 f9c7 ef06 9409 2f34 6ef7 219a 16d2  ......../4n.!...
-00001c50: ba07 c834 df09 2d07 5aa2 4cad cda8 471d  ...4..-.Z.L...G.
-00001c60: 612e a312 7f8c 4144 45f5 1d7f 4010 bcc3  a.....ADE...@...
-00001c70: 8b8b 2893 eb7a 8753 cc03 17b1 9d03 0c6c  ..(..z.S.......l
-00001c80: b184 cc49 9cbe d94c c542 0917 93eb 24f4  ...I...L.B....$.
-00001c90: b283 8e17 6929 5f1d 510a 59b7 f1bb 1066  ....i)_.Q.Y....f
-00001ca0: df15 295a 3c82 a4a3 9fb6 6ca5 7984 abe4  ..)Z<.....l.y...
-00001cb0: c150 384c 350d 29d7 6f07 965a 6758 1111  .P8L5.).o..ZgX..
-00001cc0: 07e0 6383 3318 df75 be9d cb72 3f51 f390  ..c.3..u...r?Q..
-00001cd0: ae6a bd9a a1b0 9fb1 1ce9 81b7 a27b 5fc8  .j...........{_.
-00001ce0: 0b2f 8980 9fb0 a8b3 3a40 3540 10c7 a0f5  ./......:@5@....
-00001cf0: fd06 9904 a2c2 a23f e769 e6af f7c8 3fd1  .......?.i....?.
-00001d00: 0609 dfc1 c4eb 7da0 71c1 d87a bdfe 7d5a  ......}.q..z..}Z
-00001d10: d4f2 adbc e861 ee3e 623d da27 f223 51f6  .....a.>b=.'.#Q.
-00001d20: bb32 eb3e 6c90 c004 7ec1 bb4b 9a47 34c9  .2.>l...~..K.G4.
-00001d30: 3f6d 806f ed2c d77e 1014 94c5 c275 d76b  ?m.o.,.~.....u.k
-00001d40: 62e1 0e89 d261 9c91 4b2a 11d4 f16f 5625  b....a..K*...oV%
-00001d50: dd3a 1edc e970 bd4e 41a6 2303 4661 2825  .:...p.NA.#.Fa(%
-00001d60: ed2b a4cc 4932 32d1 f16c 80be 8589 ff2b  .+..I22..l.....+
-00001d70: c497 6cd0 2ec4 98b7 f23e 607b dc06 278a  ..l......>`{..'.
-00001d80: 6f47 990d cea6 44e6 dc00 5940 166e f472  oG....D...Y@.n.r
-00001d90: 2885 4871 5edd f4f1 aa0d 8f02 aa9c 3c83  (.Hq^.........<.
-00001da0: b871 9cc2 f000 a4ac 4e10 6f8b d987 e847  .q......N.o....G
-00001db0: b645 d71a 0a9a ef16 1d06 df8b c34a 87d0  .E...........J..
-00001dc0: 43d5 8344 cfee 2b98 f223 0fe0 cb68 b8f3  C..D..+..#...h..
-00001dd0: 8856 96ea 3345 9c7b 8424 18a7 853d cd12  .V..3E.{.$...=..
-00001de0: 991d abd6 455d 9ea2 fe84 5440 8e23 da30  ....E]....T@.#.0
-00001df0: 3c65 490e 2a5a 2a6e fdd4 0e47 6cd6 c902  <eI.*Z*n...Gl...
-00001e00: 27da e468 6b7b ad79 747b ebc2 3cca 1284  '..hk{.yt{..<...
-00001e10: aaef be2f 3c06 32bc 33ff 0292 8858 2b6d  .../<.2.3....X+m
-00001e20: 92f7 44c9 4d8a ca11 8b5d 9e85 f0b6 39ed  ..D.M....]....9.
-00001e30: d7f2 f200 5582 13de dd34 9b2b 7a76 7989  ....U....4.+zvy.
-00001e40: a2d6 6279 fe22 6bb3 a06e fd7a ab05 e9c3  ..by."k..n.z....
-00001e50: 4d09 c95a 508a f2ca d0b1 ea30 9e08 bbf7  M..ZP......0....
-00001e60: 0363 ec76 1f6f 4144 aede e981 e3a1 c5a6  .c.v.oAD........
-00001e70: 4e54 2463 45e0 877e 6155 47e8 c779 e466  NT$cE..~aUG..y.f
-00001e80: 3915 88c7 1a64 3c72 87b0 2c55 f70d 8e60  9....d<r..,U...`
-00001e90: 1d2d 6ed1 d2dd 2518 3226 56d9 a5ab bd87  .-n...%.2&V.....
-00001ea0: a44b fe8f f6ff 31b4 8ba8 03c5 56a9 06c5  .K....1.....V...
-00001eb0: 0484 0eda 67e1 dbd8 1c8f 7683 29ce d36d  ....g.....v.)..m
-00001ec0: 8de5 fc5d 2963 b79c 0a88 a225 8780 24fa  ...])c.....%..$.
-00001ed0: 1ce0 1ead 4150 3c31 2c03 9201 0b9c 182f  ....AP<1,....../
-00001ee0: 4f34 7174 ae54 3c51 213d 81bb 9a52 a844  O4qt.T<Q!=...R.D
-00001ef0: 96b9 c8e0 0664 5bbc f7c4 7db7 ae50 b552  .....d[...}..P.R
-00001f00: bb52 cda5 617d 837d e245 ad0e f32f 6567  .R..a}.}.E.../eg
-00001f10: 9be9 aa41 fdfb bfd0 b9f9 954c dea7 d537  ...A.......L...7
-00001f20: 32c5 15ed 596e 64d6 c711 1375 ad83 303e  2...Ynd....u..0>
-00001f30: 1098 f7c7 6702 ea31 6d1c 51dd a182 5f6c  ....g..1m.Q..._l
-00001f40: f397 7be8 eda5 c750 3dd2 2a63 c326 0bb6  ..{....P=.*c.&..
-00001f50: 6666 c536 2c1b 53e8 756f f509 544b 86ee  ff.6,.S.uo..TK..
-00001f60: 8cc8 e802 8cd3 235f bfc2 7160 1260 0d1e  ......#_..q`.`..
-00001f70: 6460 1a71 46d5 9d4e 4e2f d553 4d38 523d  d`.qF..NN/.SM8R=
-00001f80: 5b67 0fa6 498d a74d d982 55a9 6ec1 a156  [g..I..M..U.n..V
-00001f90: b87a 3be6 d44e 2503 7e2d 0d87 3806 22f9  .z;..N%.~-..8.".
-00001fa0: 0cd9 cade 7dca 3cad 431d e835 dd5c 4552  ....}.<.C..5.\ER
-00001fb0: eb47 f8a0 656c 0948 b6be 5baf ad03 6dd4  .G..el.H..[...m.
-00001fc0: 058c a7c2 e39d 4336 d9e7 4f54 f788 3d0f  ......C6..OT..=.
-00001fd0: f209 e369 bf6c f651 63ac 62e1 2cbb 1ad0  ...i.l.Qc.b.,...
-00001fe0: 61cd dbe9 b0ff 6854 745b 03b7 1cfd 9f0a  a.....hTt[......
-00001ff0: ab0f 91d7 7624 de1b 543e 91d7 0aaa 6780  ....v$..T>....g.
-00002000: c025 7458 7ab6 f2bc fdb5 af6b 8bb5 3a4f  .%tXz......k..:O
-00002010: ed54 0bb8 8a30 f569 826f 3e29 37cb d93e  .T...0.i.o>)7..>
-00002020: c6c7 f100 bf77 d31a 69a2 83a2 ac99 5997  .....w..i.....Y.
-00002030: 9590 d4af 4454 cf14 54c7 f916 4fea 7836  ....DT..T...O.x6
-00002040: 6019 e354 31e9 92b3 af3a cf65 86b3 8757  `..T1....:.e...W
-00002050: 8800 7eed abe9 9c1f 2945 ab31 92fb 618c  ..~.....)E.1..a.
-00002060: 9daa 507b d081 b4d1 f1d3 6127 1336 5ce4  ..P{......a'.6\.
-00002070: 949c 56ad 1b27 9218 3474 e42d 326d 009e  ..V..'..4t.-2m..
-00002080: c574 ee11 9924 ea43 92d9 6f8a adb1 30d9  .t...$.C..o...0.
-00002090: a470 8d76 cb70 073c fd7e 4f67 7984 224d  .p.v.p.<.~Ogy."M
-000020a0: 68bc c80a 95d0 9c19 533e cd91 beef 937c  h.......S>.....|
-000020b0: e9b5 a60b 0436 ff05 609d 1515 0a1f ab35  .....6..`......5
-000020c0: 93b1 5482 a472 77c7 40d8 af2a 1096 6958  ..T..rw.@..*..iX
-000020d0: 5369 2444 4a25 149c 7001 b118 bdae 58d8  Si$DJ%..p.....X.
-000020e0: c64c 1e8a 9250 8d04 2dbf 8040 8c5f 5720  .L...P..-..@._W 
-000020f0: 2686 3d96 4742 a054 43c1 0817 108b c9eb  &.=.GB.TC.......
-00002100: 8ac5 cc98 cde5 b110 28d5 5830 c205 c462  ........(.X0...b
-00002110: faaa 6261 9bc6 483e 6d8b 944a 2c38 e102  ..ba..H>m..J,8..
-00002120: 6231 7b5d b1b0 8db9 7ce2 1629 d558 30c2  b1{]....|..).X0.
-00002130: 05c4 62fe ba62 3131 e4d3 8540 a846 8296  ..b..b11...@.F..
-00002140: 5f40 2016 af2b 1033 63a1 8884 40a9 8682  _@ ..+.3c...@...
-00002150: 112e 2016 96f9 aa82 3132 8db1 7ce6 1629  .. .....12..|..)
-00002160: 9560 70c2 d306 a34a 1223 14c1 0ca4 ba0b  .`p....J.#......
-00002170: a3b5 bfc9 1372 463d 2808 3acb 2aac 21cc  .....rF=(.:.*.!.
-00002180: f06f 59b0 2ce6 137a 6dea c109 7280 f306  .oY.,..zm...r...
-00002190: b490 574c 0527 d107 2342 9d88 5f21 d7b1  ..WL.'..#B.._!..
-000021a0: 3cfe 7925 8d6b 2dd1 b08f ee20 f254 aafb  <.y%.k-.... .T..
-000021b0: 72d5 0f37 8cbd 586a 2d53 4099 5ea1 b7d3  r..7..Xj-S@.^...
-000021c0: f029 e262 51a6 aa64 0e65 324a c761 c030  .).bQ..d.e2J.a.0
-000021d0: 9a1f b909 f9f2 1d5e fb72 7d5b b452 27ac  .......^.r}[.R'.
-000021e0: 4290 8d62 d838 0daf 9ce0 2873 e198 5a24  B..b.8....(s..Z$
-000021f0: 8d87 d26c 50f9 98a1 7e41 b3fe a461 7055  ...lP...~A...apU
-00002200: efd8 2cdf 45f8 ea99 2116 b87d f391 c42d  ..,.E...!..}...-
-00002210: 2e14 1d9b e6eb b5ff 78ad 1972 6faf c80b  ........x..ro...
-00002220: adc3 230e 1d59 f88b 21d3 30e7 7ec4 f408  ..#..Y..!.0.~...
-00002230: 7177 269d 75e7 7bf8 f379 385f e047 eca9  qw&.u.{..y8_.G..
-00002240: e1b0 cdae 7e86 db97 60f8 f8f9 ed1e 5d82  ....~...`.....].
-00002250: dd33 fbf9 0d1f bfbc e196 619e 29e2 22bd  .3........a.).".
-00002260: db18 517f d8a5 f2dc 3d7d 1bd4 618c a83c  ..Q.....=}..a..<
-00002270: 3522 0cb4 2eb9 9375 adfd e72f 7f7f b101  5".....u.../....
-00002280: 812a d2cf 4ac5 8070 c8ca bffe e3a5 7aff  .*..J..p......z.
-00002290: 3146 2a7a ff21 237f fbd7 8b75 f563 ac54  1F*z.!#....u.c.T
-000022a0: 74f5 2703 ece9 fd9a 5b29 e9d7 c3da 57d3  t.'.....[)....W.
-000022b0: d84f 7cfb 0d0d 46be ab73 826a 5d42 4ec8  .O|...F..s.j]BN.
-000022c0: 1adf 163b 70b1 9116 330b ec19 c920 d3cb  ...;p...3.... ..
-000022d0: 8eec 4506 5d7a 0bd7 ac94 571c 991d edea  ..E.]z....W.....
-000022e0: 196f a40a eaec 3971 554f 5ad8 5497 9533  .o....9qUOZ.T..3
-000022f0: ad27 5363 342d 1786 0908 f42a 8335 42ff  .'Sc4-.....*.5B.
-00002300: fe58 b7a0 21bc a721 6fcf 6e88 355d b0a4  .X..!..!o.n.5]..
-00002310: 8cca 92b1 69cd 6767 b7e4 ddf9 4362 b2ac  ....i.gg....Cb..
-00002320: ab32 24b6 694d ce6e c81b 39fa 75f2 b2b4  .2$.iM.n..9.u...
-00002330: 6607 2a6a 5ac1 df98 f0e7 48a1 ef79 e2c7  f.*jZ.....H..y..
-00002340: 0fa5 75bb 2af9 e9f3 d11f fe23 27fb 0587  ..u.*......#'...
-00002350: fafa 45e7 0b04 d668 618c c767 bb44 60cf  ..E....ha..g.D`.
-00002360: a6c6 625e 17f7 bcf7 083e 7d3e fa0b 7907  ..b^.....>}>..y.
-00002370: dc5b 7fa4 c6dc c464 b6bc 537b e571 61dc  .[.....d..S{.qa.
-00002380: aaad eec1 4fa7 151f c416 e427 a98f dc67  ....O......'...g
-00002390: 9ab6 351b 4d25 6f13 5497 539f e02b 6aa7  ..5.M%o.T.S..+j.
-000023a0: 5e3c faf4 f9e8 aff0 f504 64b7 5793 af1c  ^<........d.W...
-000023b0: 8d1d 8372 d79c 233a 256e 289a a7f5 cb80  ...r..#:%n(.....
-000023c0: 2226 a5c4 1274 d333 5c4e fe74 d718 e4fa  "&...t.3\N.t....
-000023d0: a86f 767c 6f5c 31cb 6ced 6aaa daa5 dd8a  .ov|o\1.l.j.....
-000023e0: faf5 b7ca fd5c 435e 8804 ce1e e659 d541  .....\C^.....Y.A
-000023f0: 7168 6912 a69a 5308 85af 7a17 fcde 0429  qhi...S...z....)
-00002400: dd32 b7d8 16da 9f5a ca84 236b 21f1 9145  .2.....Z..#k!..E
-00002410: 30f1 f1b7 e759 ced1 89bc d475 62f1 133f  0....Y.....ub..?
-00002420: f4da aec5 3398 cd7b bb96 293d a3ae 9526  ....3..{..)=...&
-00002430: 5433 4bb8 b147 5ff0 6227 4645 5ea3 f5f1  T3K..G_.b'FE^...
-00002440: 29cd 2eeb a1f3 5858 6a92 647a 8d21 05bc  ).....XXj.dz.!..
-00002450: 0397 db1b a1ef f2b7 7b6c 6f84 d9c9 fec8  ........{lo.....
-00002460: 92b0 90cf 1ec9 38ca d4fa b596 c2c0 2f46  ......8......./F
-00002470: 31c7 c3e3 18cd d6d2 1c6e b990 e451 2bbf  1........n...Q+.
-00002480: 0b57 7b28 2d7c aaba b445 183c 6498 e0e6  .W{(-|...E.<d...
-00002490: 6fc9 e05b 7d10 c5ca b034 9c5c aede ca46  o..[}....4.\...F
-000024a0: 51e1 6e5c b0c1 ad1e 4579 1015 f7f7 ab49  Q.n\....Ey.....I
-000024b0: 6e6f 8f50 8db7 7e8a cbfb 2ad5 ea0c 157b  no.P..~...*....{
-000024c0: 1837 2b1b b614 0abe 5a5d d194 d432 f343  .7+.....Z]...2.C
-000024d0: d945 c59b 31ee 768c 670b f324 1db0 1f2c  .E..1.v.g..$...,
-000024e0: be01 a4ef e444 9652 28ea f2ab 6541 243f  .....D.R(...eA$?
-000024f0: 390d b938 cfc0 0171 8ca9 93c0 14b8 1075  9..8...q.......u
-00002500: d176 818c a92c 28ed 2e04 794e 2675 8565  .v...,(...yN&u.e
-00002510: ce34 8169 5f0a 213f 449d 860a 9bd1 38b9  .4.i_.!?D.....8.
-00002520: 15ac a33f 3b54 dc03 2729 eb55 7f95 ea96  ...?;T..').U....
-00002530: c986 6676 8111 d8bb 3d5e 4aed 131e f355  ..fv....=^J....U
-00002540: 2cae dfac 15fb 9864 58a6 a05c 5dd1 3c03  ,......dX..\].<.
-00002550: f93f cb39 5413 19b4 4c5c 1b31 4aa5 2adb  .?.9T...L\.1J.*.
-00002560: 352a b971 c681 49a7 c743 943f d513 1003  5*.q..I..C.?....
-00002570: e412 8fe4 79af 864d 91fd 9a79 fb3c cdbc  ....y..M...y.<..
-00002580: 3b4f 3309 dcd5 da45 9bda 161f 5ae5 9f42  ;O3....E....Z..B
-00002590: c187 7e3a 5dbb e187 dda4 db90 6c56 bcfa  ..~:].......lV..
-000025a0: fdb7 dbf7 7f1a 7cc4 cf9e 233f 2d4f fee8  ......|...#?-O..
-000025b0: 4370 f1d4 8d95 8c67 a655 f20f 9998 9afa  Cp.....g.U......
-000025c0: 48b3 f3eb dacc 1ce2 0d24 a3a2 f136 9230  H........$...6.0
-000025d0: a0b5 e3ea f7bf dde3 bf05 e36e b3c1 9b24  ...........n...$
-000025e0: 33a6 e6bf ff39 d33f c208 ffb5 2234 ff83  3....9.?...."4..
-000025f0: 8859 8145 ac3a 78a0 bd41 bb38 aaa4 f27a  .Y.E.:x..A.8...z
-00002600: 79e8 3827 8cb4 d52d f033 c0f2 b0c2 535c  y.8'...-.3....S\
-00002610: c60d 02e0 6664 1040 7b81 3c49 c8c9 b3c5  ....fd.@{.<I....
-00002620: 552b d957 8307 1889 52c8 f3ed 2a27 2dea  U+.W....R...*'-.
-00002630: ec26 3c84 f1a9 11ff 7d25 5173 32ec 0e0a  .&<.....}%Qs2...
-00002640: 367e 386d 9bd6 4c37 17ba 65de d9f6 d234  6~8m..L7..e....4
-00002650: 97d6 dc18 4f16 a3c9 c81e 4f91 dee6 7031  ....O.....O...p1
-00002660: b466 ac41 5c71 c554 c603 beb2 ad31 3f2b  .f.A\q.T.....1?+
-00002670: 21d3 427b 5393 893d b151 53e6 6c39 5a2c  !.B{S..=.QS.l9Z,
-00002680: cd39 6b0b d7ec 62f9 0f7e 0407 3f83 608d  .9k...b..~..?.`.
-00002690: b68a 83ef f318 4403 7b6c d886 d90a 8661  ......D.{l.....a
-000026a0: a3b3 8b25 b5f5 41f1 5318 e0cb 39a2 3615  ...%..A.S...9.6.
-000026b0: 0ce5 7f1e 70f5 5f50 4b03 0414 0000 0008  ....p._PK.......
-000026c0: 0073 2e6e 588a f1b2 ff03 0100 0083 0300  .s.nX...........
-000026d0: 000c 0000 006d 616e 6966 6573 742e 7264  .....manifest.rd
-000026e0: 66cd 93c1 6e83 300c 86ef 3c45 14ce 1060  f...n.0...<E...`
-000026f0: 9781 0a3d 0cf5 3c6d 4f90 85d0 4683 18c5  ...=..<mO...F...
-00002700: 6694 b75f 9656 53d5 c326 753d ec68 ebd7  f.._.VS..&u=.h..
-00002710: efcf f2ef cdf6 380e ec43 3b34 606b 9ea7  ......8..C;4`k..
-00002720: 1967 da2a e88c ddd7 7ca6 3e79 e4db 26da  .g.*....|.>y..&.
-00002730: b8ae af5e da1d f36a 8b95 af6a 7e20 9a2a  ...^...j...j~ .*
-00002740: 2196 6549 9787 14dc 5ee4 6559 8aac 1045  !.eI....^.eY...E
-00002750: 9178 4582 ab25 794c 2cc6 bc89 180b 1ead  .xE..%yL,.......
-00002760: 46e5 cc44 7e1a fbaa e51b cc54 73a4 75d0  F..D~......Ts.u.
-00002770: 987a f720 3d8b 699d 7450 398d 303b a5bf  .z. =.i.tP9.0;..
-00002780: 8776 a030 0589 0613 98b4 0dd3 2d0a e87b  .v.0........-..{
-00002790: a3b4 c8d3 428c 9aa4 80ae 8f5f 83f5 ce0c  ....B......_....
-000027a0: 9a8b 8021 ae38 7e63 bb2b d1f4 be8f 5b50  ...!.8~c.+....[P
-000027b0: f3a8 2dfd 91c7 6256 1d24 3e4b 47e7 b3f8  ..-...bV.$>KG...
-000027c0: ce2d 3cfc 6a23 0596 3c5e b8c6 3f45 bcc8  .-<.j#..<^..?E..
-000027d0: cb6d 8497 3bde 3b71 4f27 ef1f 2377 6af9  .m..;.;qO'..#wj.
-000027e0: 8f6a a24f 504b 0304 1400 0000 0000 732e  .j.OPK........s.
-000027f0: 6e58 0000 0000 0000 0000 0000 0000 1900  nX..............
-00002800: 0000 2f43 6f6e 6669 6775 7261 7469 6f6e  ../Configuration
-00002810: 7332 2f74 6f6f 6c62 6172 2f50 4b03 0414  s2/toolbar/PK...
-00002820: 0000 0000 0073 2e6e 5800 0000 0000 0000  .....s.nX.......
-00002830: 0000 0000 001b 0000 002f 436f 6e66 6967  ........./Config
-00002840: 7572 6174 696f 6e73 322f 746f 6f6c 7061  urations2/toolpa
-00002850: 6e65 6c2f 504b 0304 1400 0000 0000 732e  nel/PK........s.
-00002860: 6e58 0000 0000 0000 0000 0000 0000 1b00  nX..............
-00002870: 0000 2f43 6f6e 6669 6775 7261 7469 6f6e  ../Configuration
-00002880: 7332 2f70 6f70 7570 6d65 6e75 2f50 4b03  s2/popupmenu/PK.
-00002890: 0414 0000 0000 0073 2e6e 5800 0000 0000  .......s.nX.....
-000028a0: 0000 0000 0000 0019 0000 002f 436f 6e66  .........../Conf
-000028b0: 6967 7572 6174 696f 6e73 322f 6d65 6e75  igurations2/menu
-000028c0: 6261 722f 504b 0304 1400 0000 0000 732e  bar/PK........s.
-000028d0: 6e58 0000 0000 0000 0000 0000 0000 1b00  nX..............
-000028e0: 0000 2f43 6f6e 6669 6775 7261 7469 6f6e  ../Configuration
-000028f0: 7332 2f73 7461 7475 7362 6172 2f50 4b03  s2/statusbar/PK.
-00002900: 0414 0000 0000 0073 2e6e 5800 0000 0000  .......s.nX.....
-00002910: 0000 0000 0000 0020 0000 002f 436f 6e66  ....... .../Conf
-00002920: 6967 7572 6174 696f 6e73 322f 696d 6167  igurations2/imag
-00002930: 6573 2f42 6974 6d61 7073 2f50 4b03 0414  es/Bitmaps/PK...
-00002940: 0000 0008 0073 2e6e 5800 0000 0002 0000  .....s.nX.......
-00002950: 0000 0000 0027 0000 0043 6f6e 6669 6775  .....'...Configu
-00002960: 7261 7469 6f6e 7332 2f61 6363 656c 6572  rations2/acceler
-00002970: 6174 6f72 2f63 7572 7265 6e74 2e78 6d6c  ator/current.xml
-00002980: 0300 504b 0304 1400 0000 0000 732e 6e58  ..PK........s.nX
-00002990: 0000 0000 0000 0000 0000 0000 1900 0000  ................
-000029a0: 2f43 6f6e 6669 6775 7261 7469 6f6e 7332  /Configurations2
-000029b0: 2f66 6c6f 6174 6572 2f50 4b03 0414 0000  /floater/PK.....
-000029c0: 0000 0073 2e6e 5800 0000 0000 0000 0000  ...s.nX.........
-000029d0: 0000 001d 0000 002f 436f 6e66 6967 7572  ......./Configur
-000029e0: 6174 696f 6e73 322f 7072 6f67 7265 7373  ations2/progress
-000029f0: 6261 722f 504b 0304 1400 0000 0800 732e  bar/PK........s.
-00002a00: 6e58 f507 2387 1c01 0000 3e04 0000 1500  nX..#.....>.....
-00002a10: 0000 4d45 5441 2d49 4e46 2f6d 616e 6966  ..META-INF/manif
-00002a20: 6573 742e 786d 6cad 94c1 6ec3 200c 86ef  est.xml...n. ...
-00002a30: 7d8a 88eb 14d8 7a9a 5093 1e2a ed09 ba07  }.....z.P..*....
-00002a40: 60c4 4991 c044 60aa f6ed 47a2 b6e9 3475  `.I..D`...G...4u
-00002a50: 6ab4 dc6c 63fe ff93 b1d8 6c4f ce16 4708  j..lc.....lO..G.
-00002a60: d178 acd8 1b7f 6505 a0f6 8dc1 ae62 9ffb  .x....e......b..
-00002a70: 8ff2 9d6d ebd5 c629 342d 4492 d7a0 c8f7  ...m...)4-D.....
-00002a80: 30de d28a a580 d2ab 68a2 44e5 204a d2d2  0.......h.D. J..
-00002a90: f780 8dd7 c901 92fc d92f 47a7 5b76 07b0  ........./G.[v..
-00002aa0: 66f5 aa98 fc5a 63a1 ccf7 c379 ea6e 93b5  f....Zc....y.n..
-00002ab0: 65af e850 31f1 4864 2a3b 688c 2ae9 dc43  e..P1.Hd*;h.*..C
-00002ac0: c554 df5b a315 e536 71c4 868f c0fc 9e93  .T.[...6q.......
-00002ad0: 139c 8889 390c fb43 725f a88c 8d82 ae21  ....9..Cr_.....!
-00002ae0: efb1 7bc0 609c ea40 0ce7 b35c b447 1af8  ..{.`..@...\.G..
-00002af0: f21c 1f08 0fe4 6238 9ea5 1be9 6c21 2e2e  ......b8....l!..
-00002b00: eb80 d4f2 ac40 9417 7379 da9d c7d6 7429  .....@..sy....t)
-00002b10: 8c9b 11d7 4269 0d16 72ea 83d0 2984 bf07  ....Bi..r...)...
-00002b20: ff3f af27 5735 261c 1078 325c df2b cc7c  .?.'W5&..x2\.+.|
-00002b30: 964b 8d87 a67d c238 77bd 5c86 b911 bffe  .K...}.8w.\.....
-00002b40: 80fa 1b50 4b03 0414 0000 0008 0073 2e6e  ...PK........s.n
-00002b50: 5844 2fcb 1a3b 0400 00d4 0400 0018 0000  XD/..;..........
-00002b60: 0054 6875 6d62 6e61 696c 732f 7468 756d  .Thumbnails/thum
-00002b70: 626e 6169 6c2e 706e 67d5 91fb 331b 0600  bnail.png...3...
-00002b80: c733 ae3b e56c a3ba dada 4ef7 2873 b7ce  .3.;.l....N.(s..
-00002b90: ac3a adab f6da f3a8 b51e 75ae d5b1 ded4  .:........u.....
-00002ba0: e36e 4a38 136f 0ea9 7768 2292 2a22 24e2  .nJ8.o..wh".*"$.
-00002bb0: 9597 4844 4290 4598 0441 4422 91a4 92a0  ..HDB.E..AD"....
-00002bc0: 4d08 d290 782d 663f ee4f d8e7 87ef 7d3f  M...x-f?.O....}?
-00002bd0: df5f bf15 6121 81f6 b69f db02 0000 fba0  ._..a!..........
-00002be0: 7b7e e100 c007 2715 d067 637d 9265 f239  {~....'..gc}.e.9
-00002bf0: d793 8113 f620 c2ff 97e0 80e8 d0a0 f0b0  ..... ..........
-00002c00: a0b8 c70f 92e2 a252 320a f241 c074 5076  .......R2..A.tPv
-00002c10: 6e4e 5e02 a824 3fa7 24ab 1856 9697 5e5a  nN^..$?.$..V..^Z
-00002c20: 945b 5e94 0906 838b 5f54 414a 2a5f 9617  .[^....._TAJ*_..
-00002c30: 5557 5496 d420 2035 7595 b07a 6845 692d  UWT..  5u..zhEi-
-00002c40: a40a 5503 86d5 405f c14a 90b0 aaa6 ba6a  ..U...@_.J.....j
-00002c50: 381c 8944 d623 5e37 3735 229b 1a1b 5fa2  8..D.#^775"..._.
-00002c60: 690d cdad 5034 05dd 8a46 b460 502d 6d8d  i...P4...F.`P-m.
-00002c70: 183c 1a4f 86b5 f4a2 3b29 adaf 2bdb 1aeb  .<.O....;)..+...
-00002c80: 30cd 0da4 6628 ae05 de86 4591 5a10 542c  0...f(....E.Z.T,
-00002c90: 1283 c5b5 7562 db3b bbba 7098 ae8e 2e02  ....ub.;..p.....
-00002ca0: 1ed7 4d20 7690 98dd 640a b187 40ec a192  ..M v...d...@...
-00002cb0: a84c 1ab9 8342 c433 08b8 de1e 32a3 17cf  .L...B.3....2...
-00002cc0: 6290 a834 1a95 ceec 67d0 69cc 2126 bd8f  b..4....g.i.!&..
-00002cd0: c5a0 0e0c 0e92 fad9 a401 7e2f 93d3 c7e2  ..........~/....
-00002ce0: 3387 39e4 5109 8b3d 3638 2ee2 d209 1c16  3.9.Q..=68......
-00002cf0: 9d3f c218 670f f0b8 c362 0e4d c21b e172  .?..g....b.M...r
-00002d00: b9ec 713e 9737 2518 670b 78a3 53d3 5363  ..q>.7%.g.x.S.Sc
-00002d10: 9373 9c69 e9cc eccc 9450 32b3 209f 94ca  .s.i.....P2. ...
-00002d20: e6a7 27c4 c229 a948 209a 9f17 8ae5 1299  ..'..).H .......
-00002d30: 422a 162a a422 9954 3a23 5389 9796 1795  B*.*.".T:#S.....
-00002d40: 6a91 46af d0ac 2ab5 8665 e184 462e 5c56  j.F...*..e..F.\V
-00002d50: 2ead a8e4 efd4 4b46 9d42 add6 a856 dfad  ......KF.B...V..
-00002d60: 68d7 b56b 2b7a edda c6c6 c6da c6fb 8d4d  h..k+z.........M
-00002d70: c39a c1ac 3718 75bb fb5b 7b07 db9b faf7  ....7.u..[{.....
-00002d80: db9b 8726 ddd1 defa cece 8ec9 bc67 da3f  ...&.........g.?
-00002d90: dc37 1b8f f68c 168b e5e4 cae3 e363 31fc  .7...........c1.
-00002da0: 7b32 0060 351d e477 2722 4ba6 97e8 43e7  {2.`5..w'"K...C.
-00002db0: c39c d831 4e11 79fe d60c 5839 a3c2 d6f3  ...1N.y...X9....
-00002dc0: ae95 1886 88fc d10a b5d4 6d15 906e 7bff  ..........m..n{.
-00002dd0: c3d3 cf60 9f81 bf3e 1fe9 7dfe 8274 3b43  ...`...>..}..t;C
-00002de0: fb77 99de 11eb b91d 6c72 dc47 7969 9347  .w......lr.Gyi.G
-00002df0: 9ae4 6ebe 6fe5 74de 992f 9201 ffe5 3899  ..n.o.t../....8.
-00002e00: 30f2 09b0 7de5 de68 945d e084 e2e3 2bd6  0...}..h.]....+.
-00002e10: cb8f 70e9 bae6 d5dd 3a8f 5422 3e50 172e  ..p.....:.T">P..
-00002e20: 7113 7cb4 795c ffdc 01d0 8fdd 7aa6 9bbe  q.|.y\......z...
-00002e30: fac7 b020 bb36 479d 1f11 05e3 4be4 7c4c  ... .6G.....K.|L
-00002e40: 6d46 1a3c 1070 3db8 8b6d 3076 b828 6f83  mF.<.p=..m0v.(o.
-00002e50: 8083 3537 5e38 2957 eb86 1aaf 5c4c d1fb  ..57^8)W....\L..
-00002e60: 6072 9c97 2717 227d 1652 0b4d c34b 1735  `r..'."}.R.M.K.5
-00002e70: 9907 4be7 7448 15ae dd99 0f75 a095 c665  ..K.tH.....u...e
-00002e80: 7dc5 883f 289e 5998 5d14 c514 82ed 6050  }..?(.Y.].....`P
-00002e90: 716a a182 3514 bb75 d67b fd95 8a88 0971  qj..5..u.{.....q
-00002ea0: f520 07a4 e1d3 5c13 6dae cede ee78 8e95  . ....\.m....x..
-00002eb0: 395c 0e13 20ed aa65 fddf fe7c 2879 fbc4  9\.. ..e...|(y..
-00002ec0: eefe a7e6 ef9e e4c6 bbe4 76a3 929e 4610  ..........v...F.
-00002ed0: 12c7 49fc 94cb 0fdd a3b2 63ce 55e2 5cbd  ..I.......c.U.\.
-00002ee0: fffc 7d15 98c5 f059 7771 5ecc 04cb c22f  ..}....Ywq^..../
-00002ef0: c941 c687 977a 6ffe 507f b334 210c 9671  .A...zo.P..4!..q
-00002f00: 2b16 9178 165d d5ae f104 05cb 1e29 b1a0  +..x.].......)..
-00002f10: 0b51 3631 8868 0a65 2eae f0b1 8ca0 3b6e  .Q61.h.e......;n
-00002f20: 7baa adce cb0c 04da 57fb 9adc 55c0 6bca  {.......W...U.k.
-00002f30: 6b49 0516 334f 1d9a 6e82 c89d 59b7 746f  kI..3O..n...Y.to
-00002f40: 049d 5f1a 7fdd 5abb 63de 060b 4edd f09d  .._...Z.c...N...
-00002f50: cf76 3dda a94d f370 0aa6 719d a3cd 0d9b  .v=..M.p..q.....
-00002f60: 7fad beb1 97ee 86b8 ad79 42c4 7e3e 09df  .........yB.~>..
-00002f70: 4068 8e10 72fd 0005 8e8a 9c1c 8b3d ad40  @h..r........=.@
-00002f80: 569d ca57 36a1 17c2 b56e 7367 521d bdfa  V..W6....nsgR...
-00002f90: 2d05 74a4 c569 38de e001 f8df e3f5 5381  -.t..i8.......S.
-00002fa0: 558f 3b3a 4674 bd45 f0af 07f9 87f8 91ee  U.;:Ft.E........
-00002fb0: fe56 fc0f 504b 0102 1403 1400 0000 0000  .V..PK..........
-00002fc0: 732e 6e58 5ec6 320c 2700 0000 2700 0000  s.nX^.2.'...'...
-00002fd0: 0800 0000 0000 0000 0000 0000 b481 0000  ................
-00002fe0: 0000 6d69 6d65 7479 7065 504b 0102 1403  ..mimetypePK....
-00002ff0: 1400 0000 0800 732e 6e58 69c5 4495 fe01  ......s.nXi.D...
-00003000: 0000 4d04 0000 0800 0000 0000 0000 0000  ..M.............
-00003010: 0000 b481 4d00 0000 6d65 7461 2e78 6d6c  ....M...meta.xml
-00003020: 504b 0102 1403 1400 0000 0800 732e 6e58  PK..........s.nX
-00003030: 0758 8d18 950d 0000 286f 0000 0b00 0000  .X......(o......
-00003040: 0000 0000 0000 0000 b481 7102 0000 636f  ..........q...co
-00003050: 6e74 656e 742e 786d 6c50 4b01 0214 0314  ntent.xmlPK.....
-00003060: 0000 0008 0073 2e6e 5880 2079 0360 0600  .....s.nX. y.`..
-00003070: 0016 2b00 000c 0000 0000 0000 0000 0000  ..+.............
-00003080: 00b4 812f 1000 0073 6574 7469 6e67 732e  .../...settings.
-00003090: 786d 6c50 4b01 0214 0314 0000 0008 0073  xmlPK..........s
-000030a0: 2e6e 5882 07ab bed6 0f00 005f 7000 000a  .nX........_p...
-000030b0: 0000 0000 0000 0000 0000 00b4 81b9 1600  ................
-000030c0: 0073 7479 6c65 732e 786d 6c50 4b01 0214  .styles.xmlPK...
-000030d0: 0314 0000 0008 0073 2e6e 588a f1b2 ff03  .......s.nX.....
-000030e0: 0100 0083 0300 000c 0000 0000 0000 0000  ................
-000030f0: 0000 00b4 81b7 2600 006d 616e 6966 6573  ......&..manifes
-00003100: 742e 7264 6650 4b01 0214 0314 0000 0000  t.rdfPK.........
-00003110: 0073 2e6e 5800 0000 0000 0000 0000 0000  .s.nX...........
-00003120: 0019 0000 0000 0000 0000 0030 0000 00e4  ...........0....
-00003130: 2700 002f 436f 6e66 6967 7572 6174 696f  '../Configuratio
-00003140: 6e73 322f 746f 6f6c 6261 722f 504b 0102  ns2/toolbar/PK..
-00003150: 1403 1400 0000 0000 732e 6e58 0000 0000  ........s.nX....
-00003160: 0000 0000 0000 0000 1b00 0000 0000 0000  ................
-00003170: 0000 3000 0000 1b28 0000 2f43 6f6e 6669  ..0....(../Confi
-00003180: 6775 7261 7469 6f6e 7332 2f74 6f6f 6c70  gurations2/toolp
-00003190: 616e 656c 2f50 4b01 0214 0314 0000 0000  anel/PK.........
-000031a0: 0073 2e6e 5800 0000 0000 0000 0000 0000  .s.nX...........
-000031b0: 001b 0000 0000 0000 0000 0030 0000 0054  ...........0...T
-000031c0: 2800 002f 436f 6e66 6967 7572 6174 696f  (../Configuratio
-000031d0: 6e73 322f 706f 7075 706d 656e 752f 504b  ns2/popupmenu/PK
-000031e0: 0102 1403 1400 0000 0000 732e 6e58 0000  ..........s.nX..
-000031f0: 0000 0000 0000 0000 0000 1900 0000 0000  ................
-00003200: 0000 0000 3000 0000 8d28 0000 2f43 6f6e  ....0....(../Con
-00003210: 6669 6775 7261 7469 6f6e 7332 2f6d 656e  figurations2/men
-00003220: 7562 6172 2f50 4b01 0214 0314 0000 0000  ubar/PK.........
-00003230: 0073 2e6e 5800 0000 0000 0000 0000 0000  .s.nX...........
-00003240: 001b 0000 0000 0000 0000 0030 0000 00c4  ...........0....
-00003250: 2800 002f 436f 6e66 6967 7572 6174 696f  (../Configuratio
-00003260: 6e73 322f 7374 6174 7573 6261 722f 504b  ns2/statusbar/PK
-00003270: 0102 1403 1400 0000 0000 732e 6e58 0000  ..........s.nX..
-00003280: 0000 0000 0000 0000 0000 2000 0000 0000  .......... .....
-00003290: 0000 0000 3000 0000 fd28 0000 2f43 6f6e  ....0....(../Con
-000032a0: 6669 6775 7261 7469 6f6e 7332 2f69 6d61  figurations2/ima
-000032b0: 6765 732f 4269 746d 6170 732f 504b 0102  ges/Bitmaps/PK..
-000032c0: 1403 1400 0000 0800 732e 6e58 0000 0000  ........s.nX....
-000032d0: 0200 0000 0000 0000 2700 0000 0000 0000  ........'.......
-000032e0: 0000 0000 b481 3b29 0000 436f 6e66 6967  ......;)..Config
-000032f0: 7572 6174 696f 6e73 322f 6163 6365 6c65  urations2/accele
-00003300: 7261 746f 722f 6375 7272 656e 742e 786d  rator/current.xm
-00003310: 6c50 4b01 0214 0314 0000 0000 0073 2e6e  lPK..........s.n
-00003320: 5800 0000 0000 0000 0000 0000 0019 0000  X...............
-00003330: 0000 0000 0000 0030 0000 0082 2900 002f  .......0....)../
-00003340: 436f 6e66 6967 7572 6174 696f 6e73 322f  Configurations2/
-00003350: 666c 6f61 7465 722f 504b 0102 1403 1400  floater/PK......
-00003360: 0000 0000 732e 6e58 0000 0000 0000 0000  ....s.nX........
-00003370: 0000 0000 1d00 0000 0000 0000 0000 3000  ..............0.
-00003380: 0000 b929 0000 2f43 6f6e 6669 6775 7261  ...)../Configura
-00003390: 7469 6f6e 7332 2f70 726f 6772 6573 7362  tions2/progressb
-000033a0: 6172 2f50 4b01 0214 0314 0000 0008 0073  ar/PK..........s
-000033b0: 2e6e 58f5 0723 871c 0100 003e 0400 0015  .nX..#.....>....
-000033c0: 0000 0000 0000 0000 0000 00b4 81f4 2900  ..............).
-000033d0: 004d 4554 412d 494e 462f 6d61 6e69 6665  .META-INF/manife
-000033e0: 7374 2e78 6d6c 504b 0102 1403 1400 0000  st.xmlPK........
-000033f0: 0800 732e 6e58 442f cb1a 3b04 0000 d404  ..s.nXD/..;.....
-00003400: 0000 1800 0000 0000 0000 0000 0000 b481  ................
-00003410: 432b 0000 5468 756d 626e 6169 6c73 2f74  C+..Thumbnails/t
-00003420: 6875 6d62 6e61 696c 2e70 6e67 504b 0506  humbnail.pngPK..
-00003430: 0000 0000 1100 1100 7804 0000 b42f 0000  ........x..../..
-00003440: 0000                                     ..
+00000270: 0050 4b03 0414 0000 0008 003d 10a1 5814  .PK........=..X.
+00000280: 7065 d597 0d00 0028 6f00 000b 0000 0063  pe.....(o......c
+00000290: 6f6e 7465 6e74 2e78 6d6c ed5d cb72 db38  ontent.xml.].r.8
+000002a0: 16dd f757 b0d4 d533 e9ae a1f8 d2d3 93b8  ...W...3........
+000002b0: 4bb1 d5b1 13db 4959 eecc 6307 91a0 8436  K.....IY..c....6
+000002c0: 49b0 41c8 b2fd 07f3 03f3 05b3 e9fd 2c67  I.A...........,g
+000002d0: e71f 9b0b be44 5294 48d9 7222 5794 5439  .....DR.H.r"W.T9
+000002e0: 2180 7b71 7071 715f 0493 d73f dfba 8e74  !.{qpqq_...?...t
+000002f0: 8359 40a8 f7a6 a135 d586 843d 935a c49b  .Y@....5...=.Z..
+00000300: bc69 ccb8 2df7 1ad2 cf87 dfbd a6b6 4d4c  .i..-.........ML
+00000310: 7c60 5173 e662 8fcb 26f5 38fc 2901 b917  |`Qs.b..&.8.)...
+00000320: 1c44 bd40 c0bc 038a 0212 1c78 c8c5 c101  .D.@.......x....
+00000330: 370f a88f bd84 ea20 3bfa 209c 2c6a 09f8  7...... ;. .,j..
+00000340: 9d53 9b3c 1c9c a5e6 f896 d725 1663 73b4  .S.<.......%.cs.
+00000350: 685c 7fe6 7070 96da 6268 5e97 588c 05a9  h\..pp..bh^.X...
+00000360: 66c9 6d5a 97f8 3670 649b 82d4 5d1f 7152  f.mZ..6pd...].qR
+00000370: 4071 eb10 effa 4d63 cab9 7fa0 28f3 f9bc  @q....Mc....(...
+00000380: 3937 9a94 4d14 addf ef2b 616f 0ad8 4cc7  97..M....+ao..L.
+00000390: f933 e684 a32c 53c1 0e16 9305 8ad6 d494  .3...,S.........
+000003a0: 64ac 8b39 aa8b 4f8c cd42 f266 ee18 b3da  d..9..O..B.f....
+000003b0: a241 1c2d ed6a 7033 a9ad 1137 9315 a231  .A.-.jp3...7...1
+000003c0: a788 d5d6 8d70 707e 7b0d abfe f61a 5696  .....pp~{.....V.
+000003d0: d645 7cba 624f 7aca 3974 863f cecf 16ba  .E|.bOz.9t.?....
+000003e0: c0dc ba73 89b1 3951 998c f8b5 9719 8dce  ...s..9Q........
+000003f0: d253 4a53 a882 203a a021 5c5d 555b 4af4  .SJS.. :.!\]U[J.
+00000400: 9c19 3d5f 3b7c ce08 c72c 33dc 5c3b dc44  ..=_;|...,3.\;.D
+00000410: 8e99 4a9c ba65 4283 719a 0223 647c 23d4  ..J..eB.q..#d|#.
+00000420: 3455 7c21 8860 0581 ae44 dde9 e0c0 5ac9  4U|!.`...D....Z.
+00000430: faef e767 2373 8a5d b418 4caa 07cb c40b  ...g#s.]..L.....
+00000440: 38f2 1692 6162 1356 aeb4 ad30 ec53 c653  8...ab.V...0.S.S
+00000450: c1d8 f50d 26ec 969e 629b 72d7 597d dc45  ....&...b.r.Y}.E
+00000460: 6f32 74c2 2cab 7428 c031 1438 fa70 f0e4  o2t.,.t(.1.8.p..
+00000470: 1b82 e7df 3772 967c bd42 f40b 0a11 9ac5  ....7r.|.B......
+00000480: 2a92 7050 d66e ae25 d054 458c 498f 31a8  *.pP.n.%.TE.I.1.
+00000490: c8c2 c8b3 49ea 876c 3af3 6011 e0bc 6201  ....I..l:.`...b.
+000004a0: e25b 1f33 22ba 9013 921d e438 64b5 dea1  .[.3"......8d...
+000004b0: 8f60 19fb ae0c 879c 4127 d849 2c46 baa4  .`......A'.I,F..
+000004c0: 5236 94ca 6e00 0a04 0785 fa07 19ea bc7f  R6..n...........
+000004d0: 60ee 6d3d 76e2 7050 cb2e 722c 180a 3308  `.m=v.pP..r,..3.
+000004e0: 0c5e a60f 5797 8ae8 9385 7b04 0710 cf94  .^..W.....{.....
+000004f0: 890b f4c6 6112 0344 f623 387c ad14 1be2  ....a..D.#8|....
+00000500: 671b 6203 d946 2696 2d6c 3ad0 1ed9 f6b4  g.b..F&.-l:.....
+00000510: 598a 9ec5 3ade 34ae d094 bac8 6848 60c4  Y...:.4.....hH`.
+00000520: 9321 2e71 ee92 1e98 5729 d0d7 61b8 9a9f  .!.q....W)..a...
+00000530: 9423 165d f204 7b20 4bb0 52c1 9c04 c1e6  .#.]..{ K.R.....
+00000540: 33c2 3604 d205 9e4b 9730 8157 32f5 9f0b  3.6....K.0.W2...
+00000550: 43fe bc16 058b b92c 46f8 849b e04d 6e10  C......,F....Mn.
+00000560: 23e1 31da 14e1 00e8 9c12 5c49 7b95 44b6  #.1.......\I{.D.
+00000570: 8e45 ab05 0659 9479 6160 f2a6 7101 aafc  .E...Y.ya`..q...
+00000580: c5b1 462a 5306 b6b6 326d 154e 5e8b ca70  ..F*S...2m.N^..p
+00000590: 6da6 69db 8738 22ee 6856 7604 d28e 3568  m.i..8".hVv...5h
+000005a0: ee02 8edd 67d8 40fd 911b f838 3cca 2a33  ....g.@....8<.*3
+000005b0: 18b7 a319 8799 3931 e590 34b5 8fe1 cf1c  ......91..4.....
+000005c0: 7a9f 5a57 91db 8c27 89b1 47be f4f0 3b29  z.ZW...'..G...;)
+000005d0: a60c 9f65 1fec 3e66 9cc0 f647 890a 72c8  ...e..>f...G..r.
+000005e0: 048c b78b d804 2295 8602 699c 9299 0a1e  ......"...i.....
+000005f0: d74c 7c84 1da7 745e d914 3dc5 c945 6316  .L|...t^..=..Ec.
+00000600: 814d 0f7c 6445 69a4 dad4 4c10 2334 8d29  .M.|dEi...L.#4.)
+00000610: b344 5aa0 36d5 b6cf a580 3ac4 92be 57c3  .DZ.6.....:...W.
+00000620: 5f1b e23b c1c8 1241 e697 4418 0e40 e6f5  _..;...A..D..@..
+00000630: 8489 1801 520e 87c2 d0ef 7147 fcde 10ff  ....R.....qG....
+00000640: afde 9861 742d a05d d279 f93a 1874 1497  ...at-.].y.:.t..
+00000650: 016d 8555 5c63 eccb 9c4e 309f 0ae4 c899  .m.U\c...N0.....
+00000660: a3bb 4d77 fbd4 4513 7c86 6d5e 0432 61c8  ..Mw..E.|.m^.2a.
+00000670: 9f12 3369 f611 13d9 7ff8 2047 d4ef a211  ..3i...... G....
+00000680: 4106 694c 94c5 1975 b099 27f3 2948 6f02  A.iL...u..'.)Ho.
+00000690: 8708 8213 1c49 32e1 3e07 3a80 8318 721c  .....I2.>.:...r.
+000006a0: 9c6a 5f94 4bca a2d3 c796 2cba c309 c029  .j_.K.....,....)
+000006b0: 7854 7688 4b78 9641 589a a033 9084 8d9c  xTv.Kx.AX..3....
+000006c0: 203d 3b37 0208 4481 b24f 8190 537f a983   =;7..D..O..S...
+000006d0: 6127 9a3c e49e 744f 2923 f754 4459 11a5  a'.<..tO)#.TDY..
+000006e0: 9311 52a6 af9c d825 8c09 15f1 a887 43ed  ..R....%......C.
+000006f0: 311d 022b 64d8 e4af 54d3 fd8b 94fb f163  1..+d...T......c
+00000700: 3824 3aae 3223 9329 177a 68c4 9a19 b78f  8$:.2#.).zh.....
+00000710: 29e7 2249 529b 3a74 3c62 972f 05e3 fd36  )."IR.:t<b./...6
+00000720: 576c 33cb 4ae9 39f7 59e8 d336 b7f9 9356  Wl3.J.9.Y..6...V
+00000730: dcdb 25b4 25bb 1b5b d3c4 15a5 2499 bd3d  ..%.%..[....$..=
+00000740: 5c98 2120 a5fe 5243 c29d 0684 4759 83d1  \.! ..RC....GY..
+00000750: 6fb6 5a6e ea41 f99d 0f53 9958 a428 0bcf  o.Zn.A...S.X.(..
+00000760: 9990 57b2 d3bb 9d66 bf57 6417 6d54 0937  ..W....f.Wd.mT.7
+00000770: 6509 aeb2 6e71 39f1 ae96 aefe 4cd2 155b  e...nq9.....L..[
+00000780: 2f92 2f39 76da 7871 5c7e 9b05 9cd8 7772  /./9v.xq\~....wr
+00000790: 00ae 0a58 cec1 4325 4abf df13 b127 c663  ...X..C%J....'.c
+000007a0: f664 c411 a4f9 cc5a c850 483f b321 6925  .d.....Z.PH?.!i%
+000007b0: 2403 0ed2 6190 bdaa 6a96 a5f7 c699 15e6  $...a...j.......
+000007c0: 696b 236f 7d21 6d8a f7f7 9b57 a8f2 9d06  ik#o}!m....W....
+000007d0: 6185 b17a 40ee 612e ade5 f346 da36 c791  a..z@.a....F.6..
+000007e0: 1f1e 53c7 6aac d509 5deb 1a9d 8579 4818  ..S.j...]....yH.
+000007f0: ca28 20c8 4bd8 663a 23ce 4977 c4bf 482b  .( .K.f:#.Iw..H+
+00000800: 8ada 0ebe 5d4d 9d0e 08e9 9fac 8fed d5fa  ....]M..........
+00000810: 58a5 6e79 77e6 ba65 b14c be15 f66b a92d  X.nyw..e.L...k.-
+00000820: 757b 71b3 433c 2c4f e33d d054 f587 4651  u{q.C<,O.=.T..FQ
+00000830: b503 8e18 5fb4 12cf 02d5 8b19 6484 2192  ...._.......d.!.
+00000840: aec0 47e2 2515 b130 8d56 801c 7f9a a680  ..G.%..0.V......
+00000850: fecc 33f9 2c2c fcc9 5184 3245 1e60 9a24  ..3.,,..Q.2E.`.$
+00000860: 0342 2c61 d02e 6685 0c31 138f 80f6 7a13  .B,a..f..1....z.
+00000870: d9a5 16f0 7798 ccc7 6527 695b ca3a bdf3  ....w...e'i[.:..
+00000880: a7d8 431c 2f4e edd3 f6fd 6a29 6610 8c6a  ..C./N....j)f..j
+00000890: 58c6 54f7 bb6d ab63 3c1d c792 775d 8ba3  X.T..m.c<...w]..
+000008a0: 706e d5c2 11c9 9dbe d2ce c5f1 12dd 4f46  pn............OF
+000008b0: bfe4 8736 465f b43a de72 d16b edaa f236  ...6F_.:.r.k...6
+000008c0: 6515 757e d9eb ac4a cce1 c992 59f2 739b  e.u~...J....Y.s.
+000008d0: 48a6 b36e 5f4b 3b17 0bec 6c63 5f97 ace2  H..n_K;...lc_...
+000008e0: 5af4 51eb 2c00 c70a c608 b2f5 1057 5c2b  Z.Q.,........W\+
+000008f0: e06c 8673 7689 ceb8 b02b 852c 26ec 0aed  .l.sv....+.,&...
+00000900: 4d9c 4645 0140 9260 ac1a 1439 cba5 310b  M.FE.@.`...9..1.
+00000910: efaa fe20 4546 3423 b17c d57c 8556 3a98  ... EF4#.|.|.V:.
+00000920: 833f 9785 050d 0b26 896a 892e b092 33c8  .?.....&.j....3.
+00000930: 2bdf 34ac 38f7 815c 8f33 10d3 f130 c32f  +.4.8..\.3...0./
+00000940: c19f d285 d082 29b2 c4db c425 cc90 2e62  ......)....%...b
+00000950: 162e 2eb7 f2f5 07a4 4019 9963 9127 126f  ........@..c.'.o
+00000960: 4667 415e f037 7546 e5c4 bb6a 642c 9c6b  FgA^.7uF...jd,.k
+00000970: ccbc 5038 d94d 4e45 9c68 6c49 1d34 a7d0  ..P8.MNE.hlI.4..
+00000980: fa42 a113 c926 7df7 6954 188b 38e9 38ba  .B...&}.iT..8.8.
+00000990: c8f3 0b83 c5d5 46a0 d24a 8478 d343 b4a8  ......F..J.x.C..
+000009a0: a1ae 3c66 65a0 d3de 2929 c24e bb4e cb80  ..<fe...)).N.N..
+000009b0: 17ad 4f0d 0395 dd32 ec82 538f d477 49ab  ..O....2..S..wI.
+000009c0: 0213 3938 0924 326c 21ab 27d8 2e21 48b5  ..98.$2l!.'..!H.
+000009d0: 64d5 f94b 07c4 077c 71d8 9f6e 7744 bdaf  d..K...|q..nwD..
+000009e0: 3536 7a5d d368 75c6 9ad9 d2bb dd9e ad76  56z].hu........v
+000009f0: 91de eef6 7147 35bb 78d9 6166 ebc5 25c9  ....qG5.x.af..%.
+00000a00: 435a 52ce c427 f9da 711c d210 4bdc 5f80  CZR..'..q...K._.
+00000a10: 19cd 3490 0229 c971 3b48 b029 6418 159a  ..4..).q;H.)d...
+00000a20: 231e 7140 1615 c872 15e8 a8a9 18f9 350d  #.q@...r......5.
+00000a30: d52c 0d13 9baa baaa 1852 2449 aa27 2185  .,.......R$I.'!.
+00000a40: 5257 b21f c85c 0341 ac2b 1eaf 2d1d 477d  RW...\.A.+..-.G}
+00000a50: 6945 29a9 b313 cb72 7045 91b8 568d 3953  iE)....rpE..V.9S
+00000a60: 9736 365e 99fe bc2b 7b3e ecb5 f4bd b91c  .66^...+{>......
+00000a70: aa46 0ba1 cecc f58a ab0b 1b4b ea93 a0c8  .F.........K....
+00000a80: 715f a2cf 5ab7 dff9 69db 58cb 4fe7 93b1  q_..Z...i.X.O...
+00000a90: 763b fdd6 d6b1 2e07 afbb 8b75 399c fc6a  v;.........u9..j
+00000aa0: 5851 0775 b431 36f5 deb8 df6a f7ad be69  XQ.u.16....j...i
+00000ab0: e87d 0375 0dd3 1edb b68d f6f6 f911 f6b9  .}.u............
+00000ac0: 9664 77c9 1254 62dd 214b 5089 7587 2c41  .dw..Tb.!KP.u.,A
+00000ad0: 25d6 1db2 04bd b66a b5ba baa6 a95a af35  %......j.....Z.5
+00000ae0: ee18 6373 dceb a9ad 71cb 6e8b 4b00 bdbd  ..cs....q.n.K...
+00000af0: 2578 ac25 a892 ec2e 5982 4aac 3b64 092a  %x.%....Y.J.;d.*
+00000b00: b1ee 9025 a8c4 ba4b 96c0 1ce3 b6da ea58  ...%...K.......X
+00000b10: 4647 6fe9 9d0e c2dd 7eaf ddc1 fdbe ddc1  FGo.....~.......
+00000b20: 567f 1f13 3cde 1254 4876 a72c 4115 d65d  V...<..THv.,A..]
+00000b30: b204 5558 77c9 1254 61dd 214b d01f 1b63  ..UXw..Ta.!K...c
+00000b40: d536 bbe3 6e07 b78c 7177 8c7a 6db3 ade1  .6..n...qw.zm...
+00000b50: 4eaf 05cf fde5 c2f2 de12 6c49 b2bb 6409  N.........lI..d.
+00000b60: 2ab1 ee90 25a8 c4ba 4396 a012 eb97 b504  *...%...C.......
+00000b70: caca fbbd 71c7 985a 77e9 8328 0a1f be0e  ....q..Zw..(....
+00000b80: 3f47 0cf0 ef33 ec2d ee09 2f37 4a61 9345  ?G...3.-../7Ja.E
+00000b90: 02df 4177 c93b 2338 3e37 e236 9ada 88ba  ..Aw.;#8>7.6....
+00000ba0: 23c9 9c3a ce2c e02c 7c8f 2d4a d0cb cc9e  #..:.,.,|.-J....
+00000bb0: 3841 6280 9e81 73f4 5a6d fb8c 8fa3 4f2f  8Ab...s.Zm....O/
+00000bc0: 57f1 2e69 4c76 611a b129 d8e0 133d 665f  W..iLva..)...=f_
+00000bd0: 9855 6f1c 8ee8 3d41 ce9c 301e 9853 6473  .Uo...=A..0..Sds
+00000be0: e98d f4a7 df67 94ff d545 bf51 f6f0 4710  .....g...E.Q..G.
+00000bf0: 3dc5 734e 619a 850d 8ecd ee46 d5ff 8824  =.sNa......F...$
+00000c00: 8baf 1e61 6ee2 58c1 1fcb 0c6c adb2 557e  ...an.X....l..U~
+00000c10: fa96 f919 5be6 d72a f29b 8657 b2c4 ddec  ....[..*...W....
+00000c20: 20df 012d 8599 b1e3 94cc 9bbc 9188 d5ce   ..-............
+00000c30: 2f57 bb70 1671 31ff 28fa fa1a d48d c313  /W.p.q1.(.......
+00000c40: 8eb5 49dc 872a cef5 acb3 0fd8 1813 8ef9  ..I..*..........
+00000c50: d79a ff13 a363 7c0f 10be 1680 0fc8 b388  .....c|.........
+00000c60: 85e0 612d 0265 4925 946d 6b8f 5e09 3f07  ..a-.eI%.mk.^.?.
+00000c70: 3c1a 88a4 f0e3 f0f8 925d 40c4 4bd5 46dc  <........]@.K.F.
+00000c80: 3665 e285 e831 e688 38b0 5020 f630 8b57  6e...1..8.P .0.W
+00000c90: 890e 25d8 7869 5326 97f2 d19d 0966 6e04  ..%.xiS&.....fn.
+00000ca0: 1e96 4d66 3ca0 c2d1 b27b 40c4 66ee 82f7  ..Mf<....{@.f...
+00000cb0: 2bed c798 77e0 236f 7931 b05c 235c ee08  +...w.#oy1.\#\..
+00000cc0: 4f99 243e da06 9ed9 8320 c80e b7a0 13cf  O.$>..... ......
+00000cd0: 2cd4 cbc1 f1f0 f27c 7074 32bc 948e a68c  ,......|pt2.....
+00000ce0: 049c c072 5f69 edf6 8fa9 3016 7200 9993  ...r_i....0.r...
+00000cf0: 4052 fb4d 150c 6efb 65ad f497 c13f ce3f  @R.M..n.e....?.?
+00000d00: 5e7c 3e3d 3b1b 4a67 3313 d668 a83f 6516  ^|>=;.Jg3..h.?e.
+00000d10: b9f3 0b78 3f1c 5c3c fceb 7c70 7925 bd7f  ...x?.\<..|py%..
+00000d20: f883 3dfc d7c5 b088 9e56 730d cb06 6047  ..=......Vs...`G
+00000d30: 8f39 35a7 4f3b e360 92a5 c135 2737 d2e7  .95.O;.`...5'7..
+00000d40: 266d be6b e64e f5ee eff3 e7c1 85f4 7938  &m.k.N........y8
+00000d50: 841f c413 7798 0175 a7b3 fa34 ea7a 5335  ....w..u...4.zS5
+00000d60: 8aa7 31fc ebe2 b268 a219 d996 2d1f 9f02  ..1....h....-...
+00000d70: 2aad dbd4 b4a6 d67a 5936 6208 4bbc 1ac9  *......zY6b.K...
+00000d80: ef06 a32b 69c8 3c24 0ca1 fea2 6cc4 e0e8  ...+i.<$....l...
+00000d90: e3db 91f4 1e99 9048 88dd 16fb d47d b485  .......H.....}..
+00000da0: c8b6 3c36 1b39 15b7 f093 d8a4 2ad9 a87e  ..<6.9......*..~
+00000db0: 95bd 225e ae24 dc24 f8ae f1da 77a3 60be  .."^.$.$....w.`.
+00000dc0: c6ab d9ed f2db 30d9 a8f1 8a73 9f6c ec93  ......0....s.l..
+00000dd0: 8d6f 2ad9 7872 14f2 f674 3478 6191 4736  .o*.xr...t4xa.G6
+00000de0: 19f8 8511 7e2f fc5f 6f8d 9717 b1c7 cbcb  ....~/._o.......
+00000df0: 0406 bf8e 8e87 e77f 1b9c 1d4b 03c7 a65e  ...........K...^
+00000e00: 00cb d43a 2fc9 cd9f 0f87 a311 4488 e7e0  ...:/.......D...
+00000e10: e383 4084 29ad c73b f91d 3d80 0fff 33c5  ..@.)..;..=...3.
+00000e20: 1746 4100 3929 70d8 a7fd db94 eed9 e0fc  .FA.9)p.........
+00000e30: edf0 f2ea 9fd2 bb19 b1a8 d01f 7dcd 29ef  ............}.).
+00000e40: 3535 bd18 cb6f 3fc3 88ac cff0 e803 589f  55...o?.......X.
+00000e50: 4b72 0da0 bac6 9a22 44a7 a9b6 5e9c e979  Kr....."D...^..y
+00000e60: 7b39 3c3a b992 de42 446c 8905 d63d b53b  {9<:...BDl...=.;
+00000e70: 01fe fdc7 8b01 e416 34c0 b648 2bfa 5f35  ........4..H+._5
+00000e80: ad18 de8a b442 7af5 f06f db86 d538 4de9  .....Bz..o...8M.
+00000e90: 331d 4a2e e1d2 072a 0c06 03fb 718d 59c0  3.J....*....q.Y.
+00000ea0: 11e7 336f 9260 ad4a 40aa 6fd0 ad88 a12b  ..3o.`.J@.o....+
+00000eb0: 0937 09c8 6bdc 36db 28c0 af71 236c bbfc  .7..k.6.(..q#l..
+00000ec0: 364c 406a dcac da27 20fb 04e4 9b4a 40b6  6L@j...' ....J@.
+00000ed0: 1aff ac2d 89d6 8b78 2ea8 14cc 207c ba21  ...-...x.... |.!
+00000ee0: 103c 35a5 8f9e 7327 d994 49e2 6b77 f1cf  .<5...s'..I.kw..
+00000ef0: 858a 4aa5 8f29 4068 be2c 9f7c 727a f66e  ..J..)@h.,.|rz.n
+00000f00: 7839 924e 8863 e109 62c2 311b 6b22 0f43  x9.N.c..b.1.k".C
+00000f10: 7d89 a5cd 473a ef8d b0bf e074 e34a 5875  }...G:.....t.JXu
+00000f20: 367f f84f 00a7 ee89 ef18 9f31 f3df 55ed  6..O.......1..U.
+00000f30: fa30 38fd 2cce d007 c41c 914d d47d 29b5  .08.,......M.}).
+00000f40: 13e0 a3aa bf74 8c3c 8205 7abd b713 91ed  .....t.<..z.....
+00000f50: 2746 6ed0 53c3 d9ca 6be0 ab22 b22a c28d  'Fn.S...k..".*..
+00000f60: c2bb ea2b d39b 858b d5d7 9ab7 cb6f d370  ...+.........o.p
+00000f70: b6fa 7af0 3e9c dd87 b3df 5238 bb4d ffba  ..z.>.....R8.M..
+00000f80: 4131 6ff7 9dcf f9e0 ec7c 7871 7c3a bc94  A1o......|xq|:..
+00000f90: ce11 13ef d55b 6b5e f66b 7a53 d59e ff65  .....[k^.kzS...e
+00000fa0: fff1 f0e2 e385 748c 3d22 6ae3 bd75 2ffa  ......t.="j..u/.
+00000fb0: d556 536d bfb8 3adc f0e2 ddf0 6c24 0d2d  .VSm..:.....l$.-
+00000fc0: 88f7 85c7 7f96 70f8 b9c0 675f d324 f5db  ......p...g_.$..
+00000fd0: f6d7 adc6 8da8 1770 32c1 35c3 92ea 6f52  .......p2.5...oR
+00000fe0: 5678 d64a c24d dc74 8def 3736 72fb 35be  Vx.J.M.t..76r.5.
+00000ff0: b1d8 2ebf 0dc3 921a df2a ecc3 927d 58f2  .........*...}X.
+00001000: 2d85 255b b953 fc0d e6fb 5917 7482 2d22  -.%[.S....Y.t.-"
+00001010: ee28 beac 9cff 9101 402d f759 82f7 93d1  .(......@-.Y....
+00001020: c832 ce7d 80a5 e4be cd52 56fc 3777 87ff  .2.}.....RV.7w..
+00001030: 0750 4b03 0414 0000 0008 003d 10a1 5880  .PK........=..X.
+00001040: 2079 0360 0600 0016 2b00 000c 0000 0073   y.`....+......s
+00001050: 6574 7469 6e67 732e 786d 6cb5 5a51 77da  ettings.xml.ZQw.
+00001060: 3a0c 7ebf bfa2 87f7 8e96 756d e1b4 dd01  :.~.......um....
+00001070: 5ab6 6eb4 7008 5bcf dd9b 4904 f8e2 5839  Z.n.p.[...I...X9
+00001080: b653 cabf 9fec 00eb 28b9 6349 fc44 9b38  .S......(.cI.D.8
+00001090: 9223 e9fb 2459 b9fa f812 8ba3 6750 9aa3  .#..$Y......gP..
+000010a0: bcae 9dbe 3ba9 1d81 0c31 e272 765d fb36  ....;....1.rv].6
+000010b0: ee1d 5fd6 3ede fc73 85d3 290f a115 6198  .._.>..s..)...a.
+000010c0: c620 cdb1 0663 6889 3ea2 c7a5 6e65 b7af  . ...ch.>...ne..
+000010d0: 6ba9 922d 649a eb96 6431 e896 095b 9880  k..-d...d1...[..
+000010e0: dc3c d67a bdba e594 6557 5e04 978b ebda  .<.z....eW^.....
+000010f0: dc98 a455 af2f 97cb 77cb f7ef 50cd eaa7  ...U./..w...P...
+00001100: cd66 b3ee ee6e 9686 28a7 7c76 a8aa 6cf5  .f...n..(.|v..l.
+00001110: 6b55 88b8 5564 1fc8 36e3 9435 4e4e ceea  kU..Ud..6..5NN..
+00001120: d9ff b5a3 f526 5f99 a651 bbd9 d861 f3fa  .....&_..Q...a..
+00001130: 3757 6b05 d9cf 3137 105b db1c ad2f dbad  7Wk...17.[.../..
+00001140: 5dd7 4865 eb99 c372 6bb5 dabe e77e 7fe6  ].He...rk....~..
+00001150: 3bad 6f2b 6063 4c6a 9b3b 6695 d01d 8172  ;.o+`cLj.;f....r
+00001160: 56bb 39b9 aabf 1571 b8d8 3e4c 8d0f b94f  V.9....q..>L...O
+00001170: 3c32 f3bd 82df 7f68 bc6f 9413 fe19 f86c  <2.....h.o.....l
+00001180: be7f dba7 e797 27a7 c5a4 0773 5c8e 20a2  ......'....s\. .
+00001190: 1883 ee9c c919 e81d 0d13 4401 4cd6 6e8c  ..........D.L.n.
+000011a0: 4aa1 988e 7bd9 51b8 d4f0 8011 e449 9f32  J...{.Q......I.2
+000011b0: a10f 167f 1cb3 e498 cb08 5e20 7a6b acfd  ..........^ zk..
+000011c0: 01e6 9e21 68a8 d561 26bf 8f76 b6aa 8de2  ...!h..a&..v....
+000011d0: d6d8 3696 4bb8 3237 f64e cf1b e725 e22f  ..6.K.27.N...%./
+000011e0: 0f2a 8d93 cbc2 5235 9f08 a81e 2c4e 6ce5  .*....R5....,Nl.
+000011f0: d076 5247 b918 b108 2c27 bb83 c660 9ce3  .vRG....,'...`..
+00001200: bb8b 66b3 98f0 1f88 f198 44ed 46db 1c95  ..f.......D.F...
+00001210: a15d 9708 34b6 c2d4 7451 a4b1 dc05 f55a  .]..4...tQ.....Z
+00001220: 7a89 70cb a477 1017 95a1 faad 5d7a 2c34  z.p..w......]z,4
+00001230: a8f6 efbd 7959 908c 7400 0242 0351 4fd1  ....yY..t..B.QO.
+00001240: 8502 3bdf 73f1 35b9 e4dd 5ef3 d5fe 0594  ..;.s.5...^.....
+00001250: 1b0f cfa6 d985 5431 43b9 f96f d2ea 9018  ......T1C..o....
+00001260: cc0c 15ea 840c e0c1 674e bee5 8b21 f392  ........gN...!..
+00001270: 48b2 fd93 ec0e 0b17 3385 a9dc 25e9 aa94  H.......3...%...
+00001280: 7491 9c89 c2d7 3bb4 a544 e3dc b707 3de5  t.....;..D....=.
+00001290: c0e9 e47f 522c 99f3 d0d7 f61d cbfa f471  ....R,.........q
+000012a0: 8fbd 3cbe 05e7 3a03 d70f 0e94 0454 4f61  ..<...:......TOa
+000012b0: 1c80 4977 934d 65e1 3e86 1733 142c 8439  ..Iw.Me.>..3.,.9
+000012c0: 8a08 76c9 aa0a 35ed 2411 ab21 536c 66bd  ..v...5.$..!Slf.
+000012d0: fac0 d4a2 872a 6666 8c8f 693c 0167 134f  .....*ff..i<.g.O
+000012e0: 2f37 02db 0140 2eca 4ac8 1fb3 c980 84d3  /7...@..J.......
+000012f0: ebcc b8f4 20ff 8e4c 13f5 08c6 b931 5a42  .... ..L.....1ZB
+00001300: 7890 2ac7 3ed6 f94f e495 2066 4278 d0f3  x.*.>..O.. fBx..
+00001310: 8be7 acff adbd 6e15 5b3a b6af 5e59 57f0  ......n.[:..^YW.
+00001320: 2481 68c8 4393 aa7c 6897 d0d0 13c8 8c61  $.h.C..|h......a
+00001330: 544b 3d62 ec1c ef43 cb37 39a1 7669 e1d4  TK=b...C.79.vi..
+00001340: 6c00 e243 8f8b b060 a5e9 86af 385b 8364  l..C...`....8[.d
+00001350: 2a70 e98d bfac 9d7c f178 40a6 17f0 0527  *p.....|.x@....'
+00001360: 5e40 6841 d765 891e 820a a9f8 a27c 747e  ^@hA.e.......|t~
+00001370: 5efd 8b50 052d 4809 dcc5 8959 7541 080b  ^..P.-H....YuA..
+00001380: c5ea d53c 3033 ef30 0db6 136f 0b3e 93f6  ...<03.0...o.>..
+00001390: 1cc7 4736 89b2 c277 309d 52e5 e8c3 2ff7  ..G6...w0.R.../.
+000013a0: bacf 2620 6ed7 6751 be02 1754 a912 6190  ..& n.gQ...T..a.
+000013b0: 1a6b ea3e 6538 f12f 0711 699f d9f4 7e26  .k.>e8./..i...~&
+000013c0: 5141 8f2b 6dfa a4f5 9e7a 0169 eea5 4f95  QA.+m....z.i..O.
+000013d0: df92 8819 b0f5 cf18 e244 d0df 9e40 dea1  .........D...@..
+000013e0: ea67 e191 01a9 abc7 e557 001f 259c e3f0  .g.......W..%...
+000013f0: 08a2 5b46 6989 d057 2aa4 3227 d38e 755b  ..[Fi..W*.2'..u[
+00001400: 4664 15b9 d054 a959 7f77 9908 53e1 0a7e  Fd...T.Y.w..S..~
+00001410: 1f9e d630 10d1 1a14 0f40 fbcd affc cbc4  ...0.....@......
+00001420: b0a4 5444 2dbf a232 3748 58e8 276c 03f6  ..TD-..27HX.'l..
+00001430: 0c9f 044e d896 40c8 800b 4fa1 a547 60bd  ...N..@...O..G`.
+00001440: f20c 63cc 2059 3d44 469a ef96 cfe4 a7da  ..c. Y=DF.......
+00001450: 4de3 e2c3 e9c5 45c1 83c4 df1a f9d1 b8ef  M.....E.........
+00001460: 8b63 5dce f3d4 e8b9 b686 4257 59ec 79a2  .c].......BWY.y.
+00001470: a6cf 9cc0 2d6d 95ee 2793 da52 c031 d41a  ....-m..'..R.1..
+00001480: 0f6d 1318 a67c 28eb d914 d54e 0d66 b45e  .m...|(....N.f.^
+00001490: bdbd 3212 f199 90f6 d8cb 43b5 3627 1521  ..2.......C.6'.!
+000014a0: f160 17e3 84ba 183b beca 3f5e 2d78 c662  .`.....;..?^-x.b
+000014b0: 39ea 7b36 1a1b c8ae 40ed e300 d4be 89f1  9.{6....@.......
+000014c0: e9f1 75c2 b0c4 6747 8796 69dd a16e cedc  ..u...gG..i..n..
+000014d0: 63ce 67f3 63b2 288a d4e6 b1a2 b5e1 5750  c.g.c.(.......WP
+000014e0: b2ad 3993 c354 52a3 e931 27da 5312 5083  ..9..TR..1'.S.P.
+000014f0: c97f c491 43d4 dc6a aa2a b2f3 2750 a475  ....C..j.*..'P.u
+00001500: e258 671b 89e5 e751 7d26 6729 b170 8e67  .Xg....Q}&g).p.g
+00001510: a2c2 9d4d 6af5 e748 bdbd 2b38 1d60 8abc  ...Mj..H..+8.`..
+00001520: 9b13 4507 5451 1d98 7169 8ba6 c212 ee64  ..E.TQ..qi.....d
+00001530: f4bf cf97 3dc0 3f80 e888 1d0c 0f99 f0dc  ....=.?.........
+00001540: 6a05 e9c4 d820 eb89 15d5 9c21 911a 446d  j.... .....!..Dm
+00001550: f79f 877c 9dd1 f79a b9c7 e878 dcf6 c37e  ...|.......x...~
+00001560: 74dd bd10 7424 137d 6091 9f4c 912a 451e  t...t$.}`..L.*E.
+00001570: df54 fef6 37c0 5485 c5e3 ae2d 042e 1dab  .T..7.T....-....
+00001580: 7ec1 4997 c910 72cf 04cb b036 1a22 344b  ~.I...r....6."4K
+00001590: 6e3e 69d3 02c8 5f91 ef8c f4a7 a3cc 52b5  n>i..._.......R.
+000015a0: 4cf6 169b f3d9 c453 8b2d 5f48 4f08 3f40  L......S.-_HO.?@
+000015b0: 21c5 eb1f 42b5 5cab d276 83b5 ac4b 21a5  !...B.\..v...K!.
+000015c0: db79 80be 27b2 d43e 4ace f567 21eb 80a3  .y..'..>J..g!...
+000015d0: e4f9 1576 7385 05ce f959 874b 4669 e4a0  ...vs....Y.KFi..
+000015e0: b90c 26af 222b 982b dbdb 6d8f 457c 5451  ..&."+.+..m.E|TQ
+000015f0: 28a9 01fb 1509 0349 0501 5503 3eec 458a  (......I..U.>.E.
+00001600: 4688 bbae 70dd de69 f3c3 d9d9 59c1 697e  F...p..i....Y.i~
+00001610: 6056 02f4 23de c294 a5c2 87ab 6d8b 9d95  `V..#.......m...
+00001620: 99f9 f3c8 821f 18b9 b34c 8adf c060 b2a9  .........L...`..
+00001630: c2aa 47fc 2d3e a2f9 926a c3a7 2b1b 49fa  ..G.->...j..+.I.
+00001640: 899b f903 9329 131d 3b0c f060 33a7 7204  .....)..;..`3.r.
+00001650: 94d9 2d16 dbc6 287b da43 0d94 3d0a f311  ..-...({.C..=...
+00001660: c9bf e72b ea6f 6226 a33d bd8d 0bb8 829d  ...+.ob&.=......
+00001670: 4d1f 5934 221a 4329 de60 bd2a 9b75 5962  M.Y4".C).`.*.uYb
+00001680: 074c 96fe 098b 7a20 876f 4b5b 7f06 2b37  .L....z .oK[..+7
+00001690: 5306 b577 98fc 9734 6827 6d6d bd6d 1036  S..w...4h'mm.m.6
+000016a0: 95db 93a2 a58a aa37 5735 16a1 a8dc 4f4b  .......7W5....OK
+000016b0: ea6f 3edd ace7 7dd4 7af3 1350 4b03 0414  .o>...}.z..PK...
+000016c0: 0000 0008 003d 10a1 5896 d095 6ed7 0f00  .....=..X...n...
+000016d0: 005f 7000 000a 0000 0073 7479 6c65 732e  ._p......styles.
+000016e0: 786d 6ced 5ddb 8ee3 b619 becf 5318 0a8a  xml.].......S...
+000016f0: 0005 244b f2d9 9871 b0bb 09b0 8bcd 4e16  ..$K...q......N.
+00001700: 9901 02f4 26d0 48b4 adae 240a 3a8c c7b9  ....&.H...$.:...
+00001710: ea53 a437 bdea 450b f431 9a37 e993 9447  .S.7..E..1.7...G
+00001720: 8992 4859 b23d 33ee a01b 2080 f9ff fcf9  ..HY.=3... .....
+00001730: 1f3e 9e7e 929a ab6f 1fc3 60f0 0092 d487  .>.~...o..`.....
+00001740: d1b5 6619 a636 0091 0b3d 3fda 5c6b 79b6  ..f..6...=?.\ky.
+00001750: d6e7 dae0 dbd5 5757 70bd f65d b0f4 a09b  ......WWp..]....
+00001760: 8720 caf4 34db 0720 1da0 da51 baa4 44c4  . ..4.. ...Q..D.
+00001770: 9f44 4be8 a47e ba8c 9c10 a4cb cc5d c218  .DK..~.......]..
+00001780: 44bc d252 e45e 92b6 6809 11d6 b53a 6116  D..R.^..h....:a.
+00001790: 6b67 e031 eb5a 19f3 56ea 3af7 dd5b 26cc  kg.1.Z..V.:..[&.
+000017a0: 626d 2f71 765d 2b63 5ee4 54b1 fa1a 76ad  bm/qv]+c^.T...v.
+000017b0: fc98 06fa 1aea 2e0c 6327 f36b 5a3c 067e  ........c'.kZ<.~
+000017c0: f4e5 5adb 6659 bc1c 0e77 bb9d b11b 1930  ..Z.fY...w.....0
+000017d0: d90c adc5 6231 24d4 4261 b7e0 8bf3 2420  ....b1$.Ba....$ 
+000017e0: 5c9e 3b04 01c0 8da5 43cb b086 9c37 0499  \.;.....C....7..
+000017f0: d355 3fcc 2baa 14e5 e13d 483a bbc6 c99c  .U?.+....=H:....
+00001800: 4654 d387 4d67 443c 6c14 ae71 b74e d219  FT..MgD<l..q.N..
+00001810: 1b84 b91a de91 d73d bc23 4fac 1b3a d956  .......=.#O..:.V
+00001820: 1193 f9f0 1322 92ff 7dfa a1c4 4212 766d  ....."..}...B.vm
+00001830: 0bf3 565c e526 7edc d94c ca2d d687 1016  ..V\.&~..L.-....
+00001840: aae2 0ab4 8312 756d d31c 0fe9 6f81 7bd7  ......um....o.{.
+00001850: cabe 4bfc 0c24 02bb dbca ee3a 815b 781c  ..K..$.....:.[x.
+00001860: 8632 a721 3e6b 8838 74f0 8061 cab9 136c  .2.!>k.8t..a...l
+00001870: b452 f264 9880 1826 59a1 c8ba fb00 85bc  .R.d...&Y.......
+00001880: 6317 dd6b 9b85 81ba 7b61 2a67 dd24 9e27  c..k....{a*g.$.'
+00001890: 6545 ea8c 86a8 ab21 a0eb 0f3e d87d ad55  eE.....!...>.}.U
+000018a0: 46ce f600 2c6a 0120 c3d0 a12a 8449 1ca7  F...,j. ...*.I..
+000018b0: 5a2b 58e6 10f3 14dd 0685 a41c 5493 4d31  Z+X.........T.M1
+000018c0: ecaf 611e 2123 d05c c11c 081e 6390 f898  ..a.!#.\....c...
+000018d0: e404 a4da b222 4144 5900 8f10 c9e6 0a41  ....."ADY......A
+000018e0: 4265 00f5 41c0 7b68 6192 540c 847a 98ea  Be..A.{ha.T..z..
+000018f0: 7e84 8009 e3a5 50bb 325a a4e9 2893 85ef  ~.....P.2Z..(...
+00001900: eea7 21a6 e978 f640 e323 6b47 9835 6d6d  ..!..x.@.#kG.5mm
+00001910: c567 c835 44b3 e3da 7181 ee01 3748 5757  .g.5D...q...7HWW
+00001920: 7464 2b8a 07f4 3756 f25a bb73 b630 7446  td+...7V.Z.s.0tF
+00001930: da00 0d61 9c25 f483 3da7 20b1 c35a fd2e  ...a.%..=. ..Z..
+00001940: 02d5 f206 95ca 98a4 6f40 841c 85fa 68ba  ........o@....h.
+00001950: f3d3 b47f 8bc8 c7e9 e006 ec06 3fa1 0622  ............?.."
+00001960: 49d3 dfd4 58be 69d5 2261 524a 8ed8 cf5c  I...X.i."aRJ...\
+00001970: 3496 3e38 894f 40dd 57c3 37a8 5e20 d18b  4.>8.O@.W.7.^ ..
+00001980: 971f f2c8 d975 b13a 29e3 7830 89c8 b47c  .....u.:).x0...|
+00001990: addd a011 ffd9 75a5 9091 29db 194c 6755  ......u...)..LgU
+000019a0: a78a 2299 5efd 9076 7e15 6ffd f036 9775  ..".^..v~.o..6.u
+000019b0: 8182 d0a2 cd3e cd40 f804 01b4 8f0c e071  .....>.@.......q
+000019c0: fa0c 55c3 202b a7fb 06ae 37f9 7f45 e7cf  ..U. +....7..E..
+000019d0: 4ee2 7cfc f9a6 6897 291c a3e2 4de2 c45b  N.|...h.)...M..[
+000019e0: 4e70 0327 451d 038f c8bc 2844 8b48 90e8  Np.'E.....(D.H..
+000019f0: b1b3 013a 15c6 29a8 76b1 6761 a4db cc41  ...:..).v.ga...A
+00001a00: d34e e269 abaf 0657 0517 6d43 8fd1 2401  .N.i...W..mC..$.
+00001a10: 92cc 4758 5ac3 e517 0062 7de7 675b 3d22  ..GXZ....b}.g[="
+00001a20: 3398 13ec 9c7d aa0d d1ae 6828 9881 7eaa  3....}....h(..~.
+00001a30: 8c8a a1f7 dee2 ca78 7e1a 07ce 9ee9 f11e  .......x~.......
+00001a40: 3878 af35 b00e 5a2c 3182 55d6 be1a 88ff  8x.5..Z,1.U.....
+00001a50: 58cb 4857 b9c5 5c0f b076 f220 d361 9ea1  X.HW..\..v. .a..
+00001a60: 2d02 d003 b4b8 428b 174b e6e1 c34e 0a9d  -.....B..K...N..
+00001a70: 64e3 477a 06e3 6bcd 34c6 f6c8 45d8 29cb  d.Gz..k.4...E.).
+00001a80: ef61 96e1 b59d 69d8 96ed 16b0 7211 4a90  .a....i.....r.J.
+00001a90: fcdc 09f4 3476 5cb2 e95c 3b41 0ab0 7779  ....4v\..\;A..wy
+00001aa0: 9398 a3d6 1a41 57ea ff8a ccb2 46e6 1fb4  .....AW.....F...
+00001ab0: a26c 07fc cd16 c5e8 1e06 5e05 bb98 5947  .l........^...YG
+00001ac0: 2b3f 27e2 5504 22ad c5c9 a46e d5a5 0def  +?'.U."....n....
+00001ad0: 9632 f1c6 2300 8f6a a905 0391 db13 3576  .2..#..j......5v
+00001ae0: 3b6a ec4b 418d ad40 4d3f d88c 26e7 804d  ;j.KA..@M?..&..M
+00001af0: 47dc 5893 deb8 2155 fae0 460d 1685 a893  G.X...!U..F.....
+00001b00: c032 6a07 cbe8 52c0 323a 0b58 ecf1 ec69  .2j...R.2:.X...i
+00001b10: c1e2 c200 26d7 dad7 7313 ffa7 d5f1 338e  ....&...s.....3.
+00001b20: b3be f8c1 5594 03cb 0160 b560 8968 7266  ....U....`.`.hrf
+00001b30: 2c8d dbb1 34be 142c 8dcf 8325 0a98 97c2  ,...4..,...%....
+00001b40: d242 1c8a 888c 6bcd 47fb 56df ed89 302c  .B....k.G.V...0,
+00001b50: a813 c0a8 a759 2dde d4b1 00ec d96a 514f  .....Y-......jQO
+00001b60: ddee 49d0 9db4 4377 7229 d09d 3c35 742d  ..I...Cwr)..<5t-
+00001b70: 737a de39 73de 7bca 9cf7 9d31 3bcd 9e0a  sz.9s.{....1;...
+00001b80: a927 a166 da8e 9ae9 a5a0 667a 16d4 3068  .'.f......fz..0h
+00001b90: 3c3f 6a4e 19dd e62f 32ba f56c f589 47b7  <?jN.../2..l..G.
+00001ba0: cf68 77fb 3601 ce97 b760 0d13 a046 e5e1  .hw.6....`...F..
+00001bb0: 2ddb 3d16 a3df 1339 b8e6 0608 8040 4840  -.=....9.....@H@
+00001bc0: 28e8 bc0b b3d1 12e4 2443 becb b14b d4e6  (.......$C...K..
+00001bd0: c8ba 90a4 c7a9 3dd4 cc0e 0829 8063 f47e  ......=....).c.~
+00001be0: b326 a71c a7fa dfc1 629e dffd ef60 9087  .&......b....`..
+00001bf0: 1131 e47c 1872 89d0 9e9a bccd 8300 641f  .1.|.r........d.
+00001c00: c464 538f 21b6 3e6a 067e da40 046d 0178  .dS.!.>j.~.@.m.x
+00001c10: 3f20 1a51 ae45 9b1b 7272 f994 dad0 16ba  ? .Q.E..rr......
+00001c20: 6953 fae6 2300 f1cf 7eb6 bd11 125e 4fea  iS..#...~....^O.
+00001c30: a767 ca8b 95fe 7e0e 0b2b be7f 560b 6f71  .g....~..+..V.oq
+00001c40: a17c 89f1 f9c7 ef06 9409 2f34 6ef7 219a  .|......../4n.!.
+00001c50: 16d2 ba07 c834 df09 2d07 5aa2 4cad cda8  .....4..-.Z.L...
+00001c60: 471d 612e a312 7f8c 4144 45f5 1d7f 4010  G.a.....ADE...@.
+00001c70: bcc3 8b8b 2893 eb7a 8753 cc03 17b1 9d03  ....(..z.S......
+00001c80: 0c6c b184 cc49 9cbe d94c c542 0917 93eb  .l...I...L.B....
+00001c90: 24f4 b283 8e17 6929 5f1d 510a 59b7 f1bb  $.....i)_.Q.Y...
+00001ca0: 1066 df15 295a 3c82 a4a3 9fb6 6ca5 7984  .f..)Z<.....l.y.
+00001cb0: abe4 c150 384c 350d 29d7 6f07 965a 6758  ...P8L5.).o..ZgX
+00001cc0: 1111 07e0 6383 3318 df75 be9d cb72 3f51  ....c.3..u...r?Q
+00001cd0: f390 ae6a bd9a a1b0 9fb1 1ce9 81b7 a27b  ...j...........{
+00001ce0: 5fc8 0b2f 8980 9fb0 a8b3 3a40 3540 10c7  _../......:@5@..
+00001cf0: a0f5 fd06 9904 a2c2 a23f e769 e6af f7c8  .........?.i....
+00001d00: 3fd1 0609 dfc1 c4eb 7da0 71c1 d87a bdfe  ?.......}.q..z..
+00001d10: 7d5a d4f2 adbc e861 ee3e 623d da27 f223  }Z.....a.>b=.'.#
+00001d20: 51f6 bb32 eb3e 6c90 c004 7ec1 bb4b 9a47  Q..2.>l...~..K.G
+00001d30: 34c9 3f6d 806f ed2c d77e 1014 94c5 c275  4.?m.o.,.~.....u
+00001d40: d76b 62e1 0e89 d261 9c91 4b2a 11d4 f16f  .kb....a..K*...o
+00001d50: 5625 dd3a 1edc e970 bd4e 41a6 2303 4661  V%.:...p.NA.#.Fa
+00001d60: 2825 ed2b a4cc 4932 32d1 f16c 80be 8589  (%.+..I22..l....
+00001d70: ff2b c497 6cd0 2ec4 98b7 f23e 607b dc06  .+..l......>`{..
+00001d80: 278a 6f47 990d cea6 44e6 dc00 5940 166e  '.oG....D...Y@.n
+00001d90: f472 2885 4871 5edd f4f1 aa0d 8f02 aa9c  .r(.Hq^.........
+00001da0: 3c83 b871 9cc2 f000 a4ac 4e10 6f8b d987  <..q......N.o...
+00001db0: e847 b645 d71a 0a9a ef16 1d06 df8b c34a  .G.E...........J
+00001dc0: 87d0 43d5 8344 cfee 2b98 f223 0fe0 cb68  ..C..D..+..#...h
+00001dd0: b8f3 8856 96ea 3345 9c7b 8424 18a7 853d  ...V..3E.{.$...=
+00001de0: cd12 991d abd6 455d 9ea2 fe84 5440 8e23  ......E]....T@.#
+00001df0: da30 3c65 490e 2a5a 2a6e fdd4 0e47 6cd6  .0<eI.*Z*n...Gl.
+00001e00: c902 27da e468 6b7b ad79 747b ebc2 3cca  ..'..hk{.yt{..<.
+00001e10: 1284 aaef be2f 3c06 32bc 33ff 0292 8858  ...../<.2.3....X
+00001e20: 2b6d 92f7 44c9 4d8a ca11 8b5d 9e85 f0b6  +m..D.M....]....
+00001e30: 39ed d7f2 f200 5582 13de dd34 9b2b 7a76  9.....U....4.+zv
+00001e40: 7989 a2d6 6279 fe22 6bb3 a06e fd7a ab05  y...by."k..n.z..
+00001e50: e9c3 4d09 c95a 508a f2ca d0b1 ea30 9e08  ..M..ZP......0..
+00001e60: bbf7 0363 ec76 1f6f 4144 aede e981 e3a1  ...c.v.oAD......
+00001e70: c5a6 4e54 2463 45e0 877e 6155 47e8 c779  ..NT$cE..~aUG..y
+00001e80: e466 3915 88c7 1a64 3c72 87b0 2c55 f70d  .f9....d<r..,U..
+00001e90: 8e60 1d2d 6ed1 d2dd 2518 3226 56d9 a5ab  .`.-n...%.2&V...
+00001ea0: bd87 a44b fe8f f6ff 31b4 8ba8 03c5 56a9  ...K....1.....V.
+00001eb0: 06c5 0484 0eda 67e1 dbd8 1c8f 7683 29ce  ......g.....v.).
+00001ec0: d36d 8de5 fc5d 2963 b79c 0a88 a225 8780  .m...])c.....%..
+00001ed0: 24fa 1ce0 1ead 4150 3c31 2c03 9201 0b9c  $.....AP<1,.....
+00001ee0: 182f 4f34 7174 ae54 3c51 213d 81bb 9a52  ./O4qt.T<Q!=...R
+00001ef0: a844 96b9 c8e0 0664 5bbc f7c4 7db7 ae50  .D.....d[...}..P
+00001f00: b552 bb52 cda5 617d 837d e245 ad0e f32f  .R.R..a}.}.E.../
+00001f10: 6567 9be9 aa41 fdfb bfd0 b9f9 954c dea7  eg...A.......L..
+00001f20: d537 32c5 15ed 596e 64d6 c711 1375 ad83  .72...Ynd....u..
+00001f30: 303e 1098 f7c7 6702 ea31 6d1c 51dd a182  0>....g..1m.Q...
+00001f40: 5f6c f397 7be8 eda5 c750 3dd2 2a63 c326  _l..{....P=.*c.&
+00001f50: 0bb6 6666 c536 2c1b 53e8 756f f509 544b  ..ff.6,.S.uo..TK
+00001f60: 86ee 8cc8 e802 8cd3 235f bfc2 7160 1260  ........#_..q`.`
+00001f70: 0d1e 6460 1a71 46d5 9d4e 4e2f d553 4d38  ..d`.qF..NN/.SM8
+00001f80: 523d 5b67 0fa6 498d a74d d982 55a9 6ec1  R=[g..I..M..U.n.
+00001f90: a156 b87a 3be6 d44e 2503 7e2d 0d87 3806  .V.z;..N%.~-..8.
+00001fa0: 22f9 0cd9 cade 7dca 3cad 431d e835 dd5c  ".....}.<.C..5.\
+00001fb0: 4552 eb47 f8a0 656c 0948 b6be 5baf ad03  ER.G..el.H..[...
+00001fc0: 6dd4 058c a7c2 e39d 4336 d9e7 4f54 f788  m.......C6..OT..
+00001fd0: 3d0f f209 e369 bf6c f651 63ac 62e1 2cbb  =....i.l.Qc.b.,.
+00001fe0: 1ad0 61cd dbe9 b0ff 6854 745b 03b7 1cfd  ..a.....hTt[....
+00001ff0: 9f0a ab0f 91d7 7624 de1b 543e 91d7 0aaa  ......v$..T>....
+00002000: 6780 c025 7458 7ab6 f2bc fdb5 af6b 8bb5  g..%tXz......k..
+00002010: 3a4f ed54 0bb8 8a30 f569 826f 3e29 37cb  :O.T...0.i.o>)7.
+00002020: d93e c6c7 f100 bf77 d31a 69a2 83a2 ac99  .>.....w..i.....
+00002030: 5997 9590 d4af 4454 cf14 54c7 f916 4fea  Y.....DT..T...O.
+00002040: 7836 6019 e354 31e9 92b3 af3a cf65 86b3  x6`..T1....:.e..
+00002050: 8757 8800 7eed abe9 9c1f 2945 ab31 92fb  .W..~.....)E.1..
+00002060: 618c 9daa 507b d081 b4d1 f1d3 6127 1336  a...P{......a'.6
+00002070: 5ce4 949c 56ad 1b27 9218 3474 e42d 326d  \...V..'..4t.-2m
+00002080: 009e c574 ee11 9924 ea43 92d9 6f8a adb1  ...t...$.C..o...
+00002090: 30d9 a470 8d76 cb70 073c fd7e 4f67 7984  0..p.v.p.<.~Ogy.
+000020a0: 224d 68bc c80a 95d0 9c19 533e cd91 beef  "Mh.......S>....
+000020b0: 937c e9b5 a60b 0436 ff05 609d 1515 0a1f  .|.....6..`.....
+000020c0: ab35 93b1 5482 a472 77c7 40d8 af2a 1096  .5..T..rw.@..*..
+000020d0: 6958 5369 2444 4a25 149c 7001 b118 bdae  iXSi$DJ%..p.....
+000020e0: 58d8 c64c 1e8a 9250 8d04 2dbf 8040 8c5f  X..L...P..-..@._
+000020f0: 5720 2686 3d96 4742 a054 43c1 0817 108b  W &.=.GB.TC.....
+00002100: c9eb 8ac5 cc98 cde5 b110 28d5 5830 c205  ..........(.X0..
+00002110: c462 faaa 6261 9bc6 483e 6d8b 944a 2c38  .b..ba..H>m..J,8
+00002120: e102 6231 7b5d b1b0 8db9 7ce2 1629 d558  ..b1{]....|..).X
+00002130: 30c2 05c4 62fe ba62 3131 e4d3 8540 a846  0...b..b11...@.F
+00002140: 8296 5f40 2016 af2b 1033 63a1 8884 40a9  .._@ ..+.3c...@.
+00002150: 8682 112e 2016 96f9 aa82 3132 8db1 7ce6  .... .....12..|.
+00002160: 1629 9560 70c2 d306 a34a 1223 14c1 0ca4  .).`p....J.#....
+00002170: ba0b a3b5 bfc9 1372 463d 2808 3acb 2aac  .......rF=(.:.*.
+00002180: 21cc f06f 59b0 2ce6 137a 6dea c109 7280  !..oY.,..zm...r.
+00002190: f306 b490 574c 0527 d107 2342 9d88 5f21  ....WL.'..#B.._!
+000021a0: d7b1 3cfe 7925 8d6b 2dd1 b08f ee20 f254  ..<.y%.k-.... .T
+000021b0: aafb 72d5 0f37 8cbd 586a 2d53 4099 5ea1  ..r..7..Xj-S@.^.
+000021c0: b7d3 f029 e262 51a6 aa64 0e65 324a c761  ...).bQ..d.e2J.a
+000021d0: c030 9a1f b909 f9f2 1d5e fb72 7d5b b452  .0.......^.r}[.R
+000021e0: 27ac 3efa bb51 0c1b a7e1 9513 1c65 2e1c  '.>..Q.......e..
+000021f0: 538b a4f1 509a 0d2a 1f33 d42f 68d6 9f34  S...P..*.3./h..4
+00002200: 0cae ea1d 9be5 bb08 5f3d 33c4 02b7 6f3e  ........_=3...o>
+00002210: 92b8 c585 a263 d37c bdf6 1faf 3543 eeed  .....c.|....5C..
+00002220: 1579 a175 78c4 a123 0b7f 3164 1ae6 dc8f  .y.ux..#..1d....
+00002230: 981e 21ee cea4 b3ee 7c0f 7f3e 0fe7 0bfc  ..!.....|..>....
+00002240: 883d 351c b6d9 d5cf 70fb 120c 1f3f bfdd  .=5.....p....?..
+00002250: a34b b07b 663f bfe1 e397 37dc 32cc 3345  .K.{f?....7.2.3E
+00002260: 5ca4 771b 23ea 0fbb 549e bba7 6f83 3a8c  \.w.#...T...o.:.
+00002270: 1195 a746 8481 d625 77b2 aeb5 fffc e5ef  ...F...%w.......
+00002280: 2f36 2050 45fa 59a9 1810 0e59 f9d7 7fbc  /6 PE.Y....Y....
+00002290: 54ef 3fc6 4845 ef3f 64e4 6fff 7ab1 ae7e  T.?.HE.?d.o.z..~
+000022a0: 8c95 8aae fe64 803d bd5f 732b 25fd 7a58  .....d.=._s+%.zX
+000022b0: fb6a 1afb 896f bfa1 c1c8 7775 4e50 ad4b  .j...o....wuNP.K
+000022c0: c809 59e3 db62 072e 36d2 6266 813d 2319  ..Y..b..6.bf.=#.
+000022d0: 647a d991 bdc8 a04b 6fe1 9a95 f28a 23b3  dz.....Ko.....#.
+000022e0: a35d 3de3 8d54 419d 3d27 aeea 490b 9bea  .]=..TA.='..I...
+000022f0: b272 a6f5 646a 8ca6 e5c2 3001 815e 65b0  .r..dj....0..^e.
+00002300: 46e8 df1f eb16 3484 f734 e4ed d90d b1a6  F.....4..4......
+00002310: 0b96 9451 5932 36ad f9ec ec96 bc3b 7f48  ...QY26......;.H
+00002320: 4c96 7555 86c4 36ad c9d9 0d79 2347 bf4e  L.uU..6....y#G.N
+00002330: 5e96 d6ec 4045 4d2b f81b 13fe 1c29 f43d  ^...@EM+.....).=
+00002340: 4ffc f8a1 b46e 5725 3f7d 3efa c37f e464  O....nW%?}>....d
+00002350: bfe0 505f bfe8 7c81 c01a 2d8c f1f8 6c97  ..P_..|...-...l.
+00002360: 08ec d9d4 58cc ebe2 9ef7 1ec1 a7cf 477f  ....X.........G.
+00002370: 21ef 807b eb8f d498 9b98 cc96 776a af3c  !..{........wj.<
+00002380: 2e8c 5bb5 d53d f8e9 b4e2 83d8 82fc 24f5  ..[..=........$.
+00002390: 91fb 4cd3 b666 a3a9 e46d 82ea 72ea 137c  ..L..f...m..r..|
+000023a0: 45ed d48b 479f 3e1f fd15 be9e 80ec f66a  E...G.>........j
+000023b0: f295 a3b1 6350 ee9a 7344 a7c4 0d45 f3b4  ....cP..sD...E..
+000023c0: 7e19 50c4 a494 5882 6e7a 86cb c99f ee1a  ~.P...X.nz......
+000023d0: 835c 1ff5 cd8e ef8d 2b66 99ad 5d4d 55bb  .\......+f..]MU.
+000023e0: b45b 51bf fe56 b99f 6bc8 0b91 c0d9 c33c  .[Q..V..k......<
+000023f0: ab3a 280e 2d4d c254 730a a1f0 55ef 82df  .:(.-M.Ts...U...
+00002400: 9b20 a55b e616 db42 fb53 4b99 7064 2d24  . .[...B.SK.pd-$
+00002410: 3eb2 0826 3efe f63c cb39 3a91 97ba 4e2c  >..&>..<.9:...N,
+00002420: 7ee2 875e dbb5 7806 b379 6fd7 32a5 67d4  ~..^..x..yo.2.g.
+00002430: b5d2 846a 6609 37f6 e80b 5eec c4a8 c86b  ...jf.7...^....k
+00002440: b43e 3ea5 d965 3d74 1e0b 4b4d 924c af31  .>>..e=t..KM.L.1
+00002450: a480 77e0 727b 23f4 5dfe 768f ed8d 303b  ..w.r{#.].v...0;
+00002460: d91f 5912 16f2 d923 1947 995a bfd6 5218  ..Y....#.G.Z..R.
+00002470: f8c5 28e6 7878 1ca3 d95a 9ac3 2d17 923c  ..(.xx...Z..-..<
+00002480: 6ae5 77e1 6a0f a585 4f55 97b6 0883 870c  j.w.j...OU......
+00002490: 13dc fc2d 197c ab0f a258 1996 8693 cbd5  ...-.|...X......
+000024a0: 5bd9 282a dc8d 0b36 b8d5 a328 0fa2 e2fe  [.(*...6...(....
+000024b0: 7e35 c9ed ed11 aaf1 d64f 7179 5fa5 5a9d  ~5.......Oqy_.Z.
+000024c0: a162 0fe3 6665 c396 42c1 57ab 2b9a 925a  .b..fe..B.W.+..Z
+000024d0: 667e 28bb a878 33c6 dd8e f16c 619e a403  f~(..x3....la...
+000024e0: f683 c537 80f4 9d9c c852 0a45 5d7e b52c  ...7.....R.E]~.,
+000024f0: 88e4 27a7 2117 e719 3820 8e31 7512 9802  ..'.!...8 .1u...
+00002500: 17a2 2eda 2e90 3195 05a5 dd85 20cf c9a4  ......1..... ...
+00002510: aeb0 cc99 2630 ed4b 21e4 87a8 d350 6133  ....&0.K!....Pa3
+00002520: 1a27 b782 75f4 6787 8a7b e024 65bd eaaf  .'..u.g..{.$e...
+00002530: 52dd 32d9 d0cc 2e30 027b b7c7 4ba9 7dc2  R.2....0.{..K.}.
+00002540: 63be 8ac5 f59b b562 1f93 0ccb 1494 ab2b  c......b.......+
+00002550: 9a67 20ff 6739 876a 2283 9689 6b23 46a9  .g .g9.j"...k#F.
+00002560: 5465 bb46 2537 ce38 30e9 f478 88f2 a77a  Te.F%7.80..x...z
+00002570: 0262 805c e291 3cef d5b0 29b2 5f33 6f9f  .b.\..<...)._3o.
+00002580: a799 77e7 6926 81bb 5abb 6853 dbe2 43ab  ..w.i&..Z.hS..C.
+00002590: fc53 28f8 d04f a76b 37fc b09b 741b 92cd  .S(..O.k7...t...
+000025a0: 8a57 bfff 76fb fe4f 838f f8d9 73e4 a7e5  .W..v..O....s...
+000025b0: c91f 7d08 2e9e bab1 92f1 ccb4 4afe 2113  ..}.........J.!.
+000025c0: 5353 1f69 767e 5d9b 9943 bc81 6454 34de  SS.iv~]..C..dT4.
+000025d0: 4612 06b4 765c fdfe b77b fcb7 60dc 6d36  F...v\...{..`.m6
+000025e0: 7893 64c6 d4fc f73f 67fa 4718 e1bf 5684  x.d....?g.G...V.
+000025f0: e67f 1031 2bb0 8855 070f b437 6817 4795  ...1+..U...7h.G.
+00002600: 545e 2f0f 1de7 8491 b6ba 057e 0658 1e56  T^/........~.X.V
+00002610: 788a cbb8 4100 dc8c 0c02 682f 9027 0939  x...A.....h/.'.9
+00002620: 79b6 b86a 25fb 6af0 0023 510a 79be 5de5  y..j%.j..#Q.y.].
+00002630: a445 9ddd 8487 303e 35e2 bfaf 246a 4e86  .E....0>5...$jN.
+00002640: dd41 c1c6 0fa7 6dd3 9ae9 e642 b7cc 3bdb  .A....m....B..;.
+00002650: 5e9a e6d2 9a1b e3c9 6234 19d9 e329 d2db  ^.......b4...)..
+00002660: 1c2e 86d6 8c35 882b ae98 ca78 c057 b635  .....5.+...x.W.5
+00002670: e667 2564 5a68 6f6a 32b1 2736 6aca 9c2d  .g%dZhoj2.'6j..-
+00002680: 478b a539 676d e19a 5d2c ffc1 8fe0 e067  G..9gm..],.....g
+00002690: 10ac d156 71f0 7d1e 8368 608f 0ddb 305b  ...Vq.}..h`...0[
+000026a0: c130 6c74 76b1 a4b6 3e28 7e0a 037c 3947  .0ltv...>(~..|9G
+000026b0: d4a6 82a1 fccf 03ae fe0b 504b 0304 1400  ..........PK....
+000026c0: 0000 0800 3d10 a158 8af1 b2ff 0301 0000  ....=..X........
+000026d0: 8303 0000 0c00 0000 6d61 6e69 6665 7374  ........manifest
+000026e0: 2e72 6466 cd93 c16e 8330 0c86 ef3c 4514  .rdf...n.0...<E.
+000026f0: ce10 6097 810a 3d0c f53c 6d4f 9085 d046  ..`...=..<mO...F
+00002700: 8318 c566 94b7 5f96 5653 d5c3 2675 3dec  ...f.._.VS..&u=.
+00002710: 68eb d7ef cff2 efcd f638 0eec 433b 3460  h........8..C;4`
+00002720: 6b9e a719 67da 2ae8 8cdd d77c a63e 79e4  k...g.*....|.>y.
+00002730: db26 dab8 aeaf 5eda 1df3 6a8b 95af 6a7e  .&....^...j...j~
+00002740: 209a 2a21 9665 4997 8714 dc5e e465 598a   .*!.eI....^.eY.
+00002750: ac10 4591 7845 82ab 2579 4c2c c6bc 8918  ..E.xE..%yL,....
+00002760: 0b1e ad46 e5cc 447e 1afb aae5 1bcc 5473  ...F..D~......Ts
+00002770: a475 d098 7af7 203d 8b69 9d74 5039 8d30  .u..z. =.i.tP9.0
+00002780: 3ba5 bf87 76a0 3005 8906 1398 b40d d32d  ;...v.0........-
+00002790: 0ae8 7ba3 b4c8 d342 8c9a a480 ae8f 5f83  ..{....B......_.
+000027a0: f5ce 0c9a 8b80 21ae 387e 63bb 2bd1 f4be  ......!.8~c.+...
+000027b0: 8f5b 50f3 a82d fd91 c762 561d 243e 4b47  .[P..-...bV.$>KG
+000027c0: e7b3 f8ce 2d3c fc6a 2305 963c 5eb8 c63f  ....-<.j#..<^..?
+000027d0: 45bc c8cb 6d84 973b de3b 714f 27ef 1f23  E...m..;.;qO'..#
+000027e0: 776a f98f 6aa2 4f50 4b03 0414 0000 0000  wj..j.OPK.......
+000027f0: 003d 10a1 5800 0000 0000 0000 0000 0000  .=..X...........
+00002800: 0019 0000 002f 436f 6e66 6967 7572 6174  ...../Configurat
+00002810: 696f 6e73 322f 746f 6f6c 6261 722f 504b  ions2/toolbar/PK
+00002820: 0304 1400 0000 0000 3d10 a158 0000 0000  ........=..X....
+00002830: 0000 0000 0000 0000 1b00 0000 2f43 6f6e  ............/Con
+00002840: 6669 6775 7261 7469 6f6e 7332 2f74 6f6f  figurations2/too
+00002850: 6c70 616e 656c 2f50 4b03 0414 0000 0000  lpanel/PK.......
+00002860: 003d 10a1 5800 0000 0000 0000 0000 0000  .=..X...........
+00002870: 001b 0000 002f 436f 6e66 6967 7572 6174  ...../Configurat
+00002880: 696f 6e73 322f 706f 7075 706d 656e 752f  ions2/popupmenu/
+00002890: 504b 0304 1400 0000 0000 3d10 a158 0000  PK........=..X..
+000028a0: 0000 0000 0000 0000 0000 1900 0000 2f43  ............../C
+000028b0: 6f6e 6669 6775 7261 7469 6f6e 7332 2f6d  onfigurations2/m
+000028c0: 656e 7562 6172 2f50 4b03 0414 0000 0000  enubar/PK.......
+000028d0: 003d 10a1 5800 0000 0000 0000 0000 0000  .=..X...........
+000028e0: 001b 0000 002f 436f 6e66 6967 7572 6174  ...../Configurat
+000028f0: 696f 6e73 322f 7374 6174 7573 6261 722f  ions2/statusbar/
+00002900: 504b 0304 1400 0000 0000 3d10 a158 0000  PK........=..X..
+00002910: 0000 0000 0000 0000 0000 2000 0000 2f43  .......... .../C
+00002920: 6f6e 6669 6775 7261 7469 6f6e 7332 2f69  onfigurations2/i
+00002930: 6d61 6765 732f 4269 746d 6170 732f 504b  mages/Bitmaps/PK
+00002940: 0304 1400 0000 0800 3d10 a158 0000 0000  ........=..X....
+00002950: 0200 0000 0000 0000 2700 0000 436f 6e66  ........'...Conf
+00002960: 6967 7572 6174 696f 6e73 322f 6163 6365  igurations2/acce
+00002970: 6c65 7261 746f 722f 6375 7272 656e 742e  lerator/current.
+00002980: 786d 6c03 0050 4b03 0414 0000 0000 003d  xml..PK........=
+00002990: 10a1 5800 0000 0000 0000 0000 0000 0019  ..X.............
+000029a0: 0000 002f 436f 6e66 6967 7572 6174 696f  .../Configuratio
+000029b0: 6e73 322f 666c 6f61 7465 722f 504b 0304  ns2/floater/PK..
+000029c0: 1400 0000 0000 3d10 a158 0000 0000 0000  ......=..X......
+000029d0: 0000 0000 0000 1d00 0000 2f43 6f6e 6669  ........../Confi
+000029e0: 6775 7261 7469 6f6e 7332 2f70 726f 6772  gurations2/progr
+000029f0: 6573 7362 6172 2f50 4b03 0414 0000 0008  essbar/PK.......
+00002a00: 003d 10a1 58f5 0723 871c 0100 003e 0400  .=..X..#.....>..
+00002a10: 0015 0000 004d 4554 412d 494e 462f 6d61  .....META-INF/ma
+00002a20: 6e69 6665 7374 2e78 6d6c ad94 c16e c320  nifest.xml...n. 
+00002a30: 0c86 ef7d 8a88 eb14 d87a 9a50 931e 2aed  ...}.....z.P..*.
+00002a40: 09ba 0760 c449 91c0 4460 aaf6 ed47 a2b6  ...`.I..D`...G..
+00002a50: e934 756a b4dc 6c63 feff 93b1 d86c 4fce  .4uj..lc.....lO.
+00002a60: 1647 08d1 78ac d81b 7f65 05a0 f68d c1ae  .G..x....e......
+00002a70: 629f fb8f f29d 6deb d5c6 2934 2d44 92d7  b.....m...)4-D..
+00002a80: a0c8 f730 ded2 8aa5 80d2 ab68 a244 e520  ...0.......h.D. 
+00002a90: 4ad2 d2f7 808d d7c9 0192 fcd9 2f47 a75b  J.........../G.[
+00002aa0: 7607 b066 f5aa 98fc 5a63 a1cc f7c3 79ea  v..f....Zc....y.
+00002ab0: 6e93 b565 afe8 5031 f148 642a 3b68 8c2a  n..e..P1.Hd*;h.*
+00002ac0: e9dc 43c5 54df 5ba3 15e5 3671 c486 8fc0  ..C.T.[...6q....
+00002ad0: fc9e 9313 9c88 8939 0cfb 4372 5fa8 8c8d  .......9..Cr_...
+00002ae0: 82ae 21ef b17b c060 9cea 400c e7b3 5cb4  ..!..{.`..@...\.
+00002af0: 471a f8f2 1c1f 080f e462 389e a51b e96c  G........b8....l
+00002b00: 212e 2eeb 80d4 f2ac 4094 1773 79da 9dc7  !.......@..sy...
+00002b10: d674 298c 9b11 d742 690d 1672 ea83 d029  .t)....Bi..r...)
+00002b20: 84bf 07ff 3faf 2757 3526 1c10 7832 5cdf  ....?.'W5&..x2\.
+00002b30: 2bcc 7c96 4b8d 87a6 7dc2 3877 bd5c 86b9  +.|.K...}.8w.\..
+00002b40: 11bf fe80 fa1b 504b 0304 1400 0000 0800  ......PK........
+00002b50: 3d10 a158 442f cb1a 3b04 0000 d404 0000  =..XD/..;.......
+00002b60: 1800 0000 5468 756d 626e 6169 6c73 2f74  ....Thumbnails/t
+00002b70: 6875 6d62 6e61 696c 2e70 6e67 d591 fb33  humbnail.png...3
+00002b80: 1b06 00c7 33ae 3be5 6ca3 bada da4e f728  ....3.;.l....N.(
+00002b90: 73b7 ceac 3aad abf6 daf3 a8b5 1e75 aed5  s...:........u..
+00002ba0: b1de d4e3 6e4a 3813 6f0e a977 6822 922a  ....nJ8.o..wh".*
+00002bb0: 2224 e295 9748 4442 9045 9804 4144 2291  "$...HDB.E..AD".
+00002bc0: a492 a04d 08d2 9078 2d66 3fee 4fd8 e787  ...M...x-f?.O...
+00002bd0: ef7d 3fdf 5fbf 1561 2181 f6b6 9fdb 0200  .}?._..a!.......
+00002be0: 00fb a07b 7ee1 00c0 0727 15d0 6763 7d92  ...{~....'..gc}.
+00002bf0: 65f2 39d7 9381 13f6 20c2 ff97 e080 e8d0  e.9..... .......
+00002c00: a0f0 b0a0 b8c7 0f92 e2a2 5232 0af2 41c0  ..........R2..A.
+00002c10: 7450 766e 4e5e 02a8 243f a724 ab18 5696  tPvnN^..$?.$..V.
+00002c20: 975e 5a94 5b5e 9409 0683 8b5f 5441 4a2a  .^Z.[^....._TAJ*
+00002c30: 5f96 1755 5754 96d4 2020 3575 95b0 7a68  _..UWT..  5u..zh
+00002c40: 4569 2da4 0a55 0386 d540 5fc1 4a90 b0aa  Ei-..U...@_.J...
+00002c50: a6ba 6a38 1c89 44d6 235e 3737 3522 9b1a  ..j8..D.#^775"..
+00002c60: 1b5f a269 0dcd ad50 3405 dd8a 46b4 6050  ._.i...P4...F.`P
+00002c70: 2d6d 8d18 3c1a 4f86 b5f4 a23b 29ad af2b  -m..<.O....;)..+
+00002c80: db1a eb30 cd0d a466 28ae 05de 8645 915a  ...0...f(....E.Z
+00002c90: 1054 2c12 83c5 b575 62db 3bbb ba70 98ae  .T,....ub.;..p..
+00002ca0: 8e2e 021e d74d 2076 9098 dd64 0ab1 8740  .....M v...d...@
+00002cb0: eca1 92a8 4c1a b983 42c4 3308 b8de 1e32  ....L...B.3....2
+00002cc0: a317 cf62 90a8 341a 95ce ec67 d069 cc21  ...b..4....g.i.!
+00002cd0: 26bd 8fc5 a00e 0c0e 92fa d9a4 017e 2f93  &............~/.
+00002ce0: d3c7 e233 8739 e451 098b 3d36 382e e2d2  ...3.9.Q..=68...
+00002cf0: 091c 169d 3fc2 1867 0ff0 b8c3 620e 4dc2  ....?..g....b.M.
+00002d00: 1be1 72b9 ec71 3e97 3725 1867 0b78 a353  ..r..q>.7%.g.x.S
+00002d10: d353 6393 739c 69e9 ccec cc94 5032 b320  .Sc.s.i.....P2. 
+00002d20: 9f94 cae6 a727 c4c2 29a9 4820 9a9f 178a  .....'..).H ....
+00002d30: e512 9942 2a16 2aa4 2299 543a 2353 8997  ...B*.*.".T:#S..
+00002d40: 9617 956a 9146 afd0 ac2a b586 65e1 8446  ...j.F...*..e..F
+00002d50: 2e5c 562e ada8 e4ef d44b 469d 42ad d6a8  .\V......KF.B...
+00002d60: 56df ad68 d7b5 6b2b 7aed dac6 c6c6 dac6  V..h..k+z.......
+00002d70: fb8d 4dc3 9ac1 ac37 1875 bbfb 5b7b 07db  ..M....7.u..[{..
+00002d80: 9bfa f7db 9b87 26dd d1de face ce8e c9bc  ......&.........
+00002d90: 67da 3fdc 371b 8ff6 8c16 8be5 e4ca e3e3  g.?.7...........
+00002da0: 6331 fc7b 3200 6035 1de4 7727 224b a697  c1.{2.`5..w'"K..
+00002db0: e843 e7c3 9cd8 314e 1179 fed6 0c58 39a3  .C....1N.y...X9.
+00002dc0: c2d6 f3ae 9518 8688 fcd1 0ab5 d46d 1590  .............m..
+00002dd0: 6e7b ffc3 d3cf 609f 81bf 3e1f e97d fe82  n{....`...>..}..
+00002de0: 743b 43fb 7799 de11 ebb9 1d6c 72dc 4779  t;C.w......lr.Gy
+00002df0: 6993 479a e46e be6f e574 de99 2f92 01ff  i.G..n.o.t../...
+00002e00: e538 9930 f209 b07d e5de 6894 5de0 84e2  .8.0...}..h.]...
+00002e10: e32b d6cb 8f70 e9ba e6d5 dd3a 8f54 223e  .+...p.....:.T">
+00002e20: 5017 2e71 137c b479 5cff dc01 d08f dd7a  P..q.|.y\......z
+00002e30: a69b befa c7b0 20bb 3647 9d1f 1105 e34b  ...... .6G.....K
+00002e40: e47c 4c6d 461a 3c10 703d b88b 6d30 76b8  .|LmF.<.p=..m0v.
+00002e50: 286f 8380 8335 375e 3829 57eb 861a af5c  (o...57^8)W....\
+00002e60: 4cd1 fb60 729c 9727 1722 7d16 520b 4dc3  L..`r..'."}.R.M.
+00002e70: 4b17 3599 074b e774 4815 aedd 990f 75a0  K.5..K.tH.....u.
+00002e80: 95c6 657d c588 3f28 9e59 985d 14c5 1482  ..e}..?(.Y.]....
+00002e90: ed60 5071 6aa1 8235 14bb 75d6 7bfd 958a  .`Pqj..5..u.{...
+00002ea0: 8809 71f5 2007 a4e1 d35c 136d aece deee  ..q. ....\.m....
+00002eb0: 788e 9539 5c0e 1320 edaa 65fd dffe 7c28  x..9\.. ..e...|(
+00002ec0: 79fb c4ee fea7 e6ef 9ee4 c6bb e476 a392  y............v..
+00002ed0: 9e46 1012 c749 fc94 cb0f dda3 b263 ce55  .F...I.......c.U
+00002ee0: e25c bdff fc7d 1598 c5f0 5977 715e cc04  .\...}....Ywq^..
+00002ef0: cbc2 2fc9 41c6 8797 7a6f fe50 7fb3 3421  ../.A...zo.P..4!
+00002f00: 0c96 712b 1691 7816 5dd5 aef1 0405 cb1e  ..q+..x.].......
+00002f10: 29b1 a00b 5136 3188 680a 652e aef0 b18c  )...Q61.h.e.....
+00002f20: a03b 6e7b aaad cecb 0c04 da57 fb9a dc55  .;n{.......W...U
+00002f30: c06b ca6b 4905 1633 4f1d 9a6e 82c8 9d59  .k.kI..3O..n...Y
+00002f40: b774 6f04 9d5f 1a7f dd5a bb63 de06 0b4e  .to.._...Z.c...N
+00002f50: ddf0 9dcf 763d daa9 4df3 700a a671 9da3  ....v=..M.p..q..
+00002f60: cd0d 9b7f adbe b197 ee86 b8ad 7942 c47e  ............yB.~
+00002f70: 3e09 df40 688e 1072 fd00 058e 8a9c 1c8b  >..@h..r........
+00002f80: 3dad 4056 9dca 5736 a117 c2b5 6e73 6752  =.@V..W6....nsgR
+00002f90: 1dbd fa2d 0574 a4c5 6938 dee0 01f8 dfe3  ...-.t..i8......
+00002fa0: f553 8155 8f3b 3a46 74bd 45f0 af07 f987  .S.U.;:Ft.E.....
+00002fb0: f891 eefe 56fc 0f50 4b01 0214 0314 0000  ....V..PK.......
+00002fc0: 0000 003d 10a1 585e c632 0c27 0000 0027  ...=..X^.2.'...'
+00002fd0: 0000 0008 0000 0000 0000 0000 0000 00b4  ................
+00002fe0: 8100 0000 006d 696d 6574 7970 6550 4b01  .....mimetypePK.
+00002ff0: 0214 0314 0000 0008 003d 10a1 5869 c544  .........=..Xi.D
+00003000: 95fe 0100 004d 0400 0008 0000 0000 0000  .....M..........
+00003010: 0000 0000 00b4 814d 0000 006d 6574 612e  .......M...meta.
+00003020: 786d 6c50 4b01 0214 0314 0000 0008 003d  xmlPK..........=
+00003030: 10a1 5814 7065 d597 0d00 0028 6f00 000b  ..X.pe.....(o...
+00003040: 0000 0000 0000 0000 0000 00b4 8171 0200  .............q..
+00003050: 0063 6f6e 7465 6e74 2e78 6d6c 504b 0102  .content.xmlPK..
+00003060: 1403 1400 0000 0800 3d10 a158 8020 7903  ........=..X. y.
+00003070: 6006 0000 162b 0000 0c00 0000 0000 0000  `....+..........
+00003080: 0000 0000 b481 3110 0000 7365 7474 696e  ......1...settin
+00003090: 6773 2e78 6d6c 504b 0102 1403 1400 0000  gs.xmlPK........
+000030a0: 0800 3d10 a158 96d0 956e d70f 0000 5f70  ..=..X...n...._p
+000030b0: 0000 0a00 0000 0000 0000 0000 0000 b481  ................
+000030c0: bb16 0000 7374 796c 6573 2e78 6d6c 504b  ....styles.xmlPK
+000030d0: 0102 1403 1400 0000 0800 3d10 a158 8af1  ..........=..X..
+000030e0: b2ff 0301 0000 8303 0000 0c00 0000 0000  ................
+000030f0: 0000 0000 0000 b481 ba26 0000 6d61 6e69  .........&..mani
+00003100: 6665 7374 2e72 6466 504b 0102 1403 1400  fest.rdfPK......
+00003110: 0000 0000 3d10 a158 0000 0000 0000 0000  ....=..X........
+00003120: 0000 0000 1900 0000 0000 0000 0000 3000  ..............0.
+00003130: 0000 e727 0000 2f43 6f6e 6669 6775 7261  ...'../Configura
+00003140: 7469 6f6e 7332 2f74 6f6f 6c62 6172 2f50  tions2/toolbar/P
+00003150: 4b01 0214 0314 0000 0000 003d 10a1 5800  K..........=..X.
+00003160: 0000 0000 0000 0000 0000 001b 0000 0000  ................
+00003170: 0000 0000 0030 0000 001e 2800 002f 436f  .....0....(../Co
+00003180: 6e66 6967 7572 6174 696f 6e73 322f 746f  nfigurations2/to
+00003190: 6f6c 7061 6e65 6c2f 504b 0102 1403 1400  olpanel/PK......
+000031a0: 0000 0000 3d10 a158 0000 0000 0000 0000  ....=..X........
+000031b0: 0000 0000 1b00 0000 0000 0000 0000 3000  ..............0.
+000031c0: 0000 5728 0000 2f43 6f6e 6669 6775 7261  ..W(../Configura
+000031d0: 7469 6f6e 7332 2f70 6f70 7570 6d65 6e75  tions2/popupmenu
+000031e0: 2f50 4b01 0214 0314 0000 0000 003d 10a1  /PK..........=..
+000031f0: 5800 0000 0000 0000 0000 0000 0019 0000  X...............
+00003200: 0000 0000 0000 0030 0000 0090 2800 002f  .......0....(../
+00003210: 436f 6e66 6967 7572 6174 696f 6e73 322f  Configurations2/
+00003220: 6d65 6e75 6261 722f 504b 0102 1403 1400  menubar/PK......
+00003230: 0000 0000 3d10 a158 0000 0000 0000 0000  ....=..X........
+00003240: 0000 0000 1b00 0000 0000 0000 0000 3000  ..............0.
+00003250: 0000 c728 0000 2f43 6f6e 6669 6775 7261  ...(../Configura
+00003260: 7469 6f6e 7332 2f73 7461 7475 7362 6172  tions2/statusbar
+00003270: 2f50 4b01 0214 0314 0000 0000 003d 10a1  /PK..........=..
+00003280: 5800 0000 0000 0000 0000 0000 0020 0000  X............ ..
+00003290: 0000 0000 0000 0030 0000 0000 2900 002f  .......0....)../
+000032a0: 436f 6e66 6967 7572 6174 696f 6e73 322f  Configurations2/
+000032b0: 696d 6167 6573 2f42 6974 6d61 7073 2f50  images/Bitmaps/P
+000032c0: 4b01 0214 0314 0000 0008 003d 10a1 5800  K..........=..X.
+000032d0: 0000 0002 0000 0000 0000 0027 0000 0000  ...........'....
+000032e0: 0000 0000 0000 00b4 813e 2900 0043 6f6e  .........>)..Con
+000032f0: 6669 6775 7261 7469 6f6e 7332 2f61 6363  figurations2/acc
+00003300: 656c 6572 6174 6f72 2f63 7572 7265 6e74  elerator/current
+00003310: 2e78 6d6c 504b 0102 1403 1400 0000 0000  .xmlPK..........
+00003320: 3d10 a158 0000 0000 0000 0000 0000 0000  =..X............
+00003330: 1900 0000 0000 0000 0000 3000 0000 8529  ..........0....)
+00003340: 0000 2f43 6f6e 6669 6775 7261 7469 6f6e  ../Configuration
+00003350: 7332 2f66 6c6f 6174 6572 2f50 4b01 0214  s2/floater/PK...
+00003360: 0314 0000 0000 003d 10a1 5800 0000 0000  .......=..X.....
+00003370: 0000 0000 0000 001d 0000 0000 0000 0000  ................
+00003380: 0030 0000 00bc 2900 002f 436f 6e66 6967  .0....)../Config
+00003390: 7572 6174 696f 6e73 322f 7072 6f67 7265  urations2/progre
+000033a0: 7373 6261 722f 504b 0102 1403 1400 0000  ssbar/PK........
+000033b0: 0800 3d10 a158 f507 2387 1c01 0000 3e04  ..=..X..#.....>.
+000033c0: 0000 1500 0000 0000 0000 0000 0000 b481  ................
+000033d0: f729 0000 4d45 5441 2d49 4e46 2f6d 616e  .)..META-INF/man
+000033e0: 6966 6573 742e 786d 6c50 4b01 0214 0314  ifest.xmlPK.....
+000033f0: 0000 0008 003d 10a1 5844 2fcb 1a3b 0400  .....=..XD/..;..
+00003400: 00d4 0400 0018 0000 0000 0000 0000 0000  ................
+00003410: 00b4 8146 2b00 0054 6875 6d62 6e61 696c  ...F+..Thumbnail
+00003420: 732f 7468 756d 626e 6169 6c2e 706e 6750  s/thumbnail.pngP
+00003430: 4b05 0600 0000 0011 0011 0078 0400 00b7  K..........x....
+00003440: 2f00 0000 00                             /....
```

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/settings/mysql.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/settings/mysql.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_aids.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_aids.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_broken_gfks.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_cbss.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_cbss.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_clients.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_debts.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_debts.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/gerd/tests/test_watchtim.py` & `lino-welfare-24.5.0/lino_welfare/projects/gerd/tests/test_watchtim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/demo.py` & `lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg` & `lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg` & `lino-welfare-24.5.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/mathieu/tests/test_chatelet.py` & `lino-welfare-24.5.0/lino_welfare/projects/mathieu/tests/test_chatelet.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/projects/mathieu/tests/test_notify.py` & `lino-welfare-24.5.0/lino_welfare/projects/mathieu/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/scripts/load_plp.py` & `lino-welfare-24.5.0/lino_welfare/scripts/load_plp.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/lino_welfare/setup_info.py` & `lino-welfare-24.5.0/lino_welfare/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #   $ python setup.py test -s tests.PackagesTests
 
 requires = ['lino-cosi', 'pytidylib', 'django-iban', 'metafone', 'cairocffi']
 requires.append('suds-py3')
 
 SETUP_INFO = dict(name='lino-welfare',
-                  version='24.3.1',
+                  version='24.5.0',
                   install_requires=requires,
                   test_suite='tests',
                   tests_require=['pytest'],
                   include_package_data=True,
                   zip_safe=False,
                   description="A Lino plugin library for Belgian PCSWs",
                   long_description="""\
@@ -126,15 +126,15 @@
     'lino_welfare.modlib.newcomers.fixtures',
     'lino_welfare.modlib.pcsw',
     'lino_welfare.modlib.pcsw.fixtures',
     'lino_welfare.modlib.polls',
     'lino_welfare.modlib.polls.fixtures',
     'lino_welfare.modlib.projects',
     'lino_welfare.modlib.reception',
-    'lino_welfare.modlib.sales',
+    'lino_welfare.modlib.trading',
     'lino_welfare.modlib.sepa',
     'lino_welfare.modlib.sepa.fixtures',
     'lino_welfare.modlib.system',
     'lino_welfare.modlib.immersion',
     'lino_welfare.modlib.immersion.fixtures',
     'lino_welfare.modlib.users',
     'lino_welfare.modlib.users.fixtures',
```

### Comparing `lino-welfare-24.3.1/lino_welfare.egg-info/PKG-INFO` & `lino-welfare-24.5.0/lino_welfare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-welfare
-Version: 24.3.1
+Version: 24.5.0
 Summary: A Lino plugin library for Belgian PCSWs
 Home-page: https://gitlab.com/lino-framework/welfare
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lino-welfare-24.3.1/lino_welfare.egg-info/SOURCES.txt` & `lino-welfare-24.5.0/lino_welfare.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -262,22 +262,22 @@
 lino_welfare/modlib/polls/fixtures/demo.py
 lino_welfare/modlib/polls/fixtures/jobsearch.py
 lino_welfare/modlib/polls/fixtures/std.py
 lino_welfare/modlib/projects/__init__.py
 lino_welfare/modlib/projects/models.py
 lino_welfare/modlib/reception/__init__.py
 lino_welfare/modlib/reception/models.py
-lino_welfare/modlib/sales/__init__.py
-lino_welfare/modlib/sales/models.py
 lino_welfare/modlib/sepa/__init__.py
 lino_welfare/modlib/sepa/models.py
 lino_welfare/modlib/sepa/fixtures/__init__.py
 lino_welfare/modlib/sepa/fixtures/demo.py
 lino_welfare/modlib/system/__init__.py
 lino_welfare/modlib/system/models.py
+lino_welfare/modlib/trading/__init__.py
+lino_welfare/modlib/trading/models.py
 lino_welfare/modlib/users/__init__.py
 lino_welfare/modlib/users/models.py
 lino_welfare/modlib/users/ui.py
 lino_welfare/modlib/users/fixtures/__init__.py
 lino_welfare/modlib/users/fixtures/demo.py
 lino_welfare/modlib/users/fixtures/demo2.py
 lino_welfare/modlib/users/fixtures/demo_users.py
@@ -349,15 +349,14 @@
 lino_welfare/projects/mathieu/manage.py
 lino_welfare/projects/mathieu/settings/__init__.py
 lino_welfare/projects/mathieu/settings/demo.py
 lino_welfare/projects/mathieu/settings/doctests.py
 lino_welfare/projects/mathieu/settings/memory.py
 lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
 lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
-lino_welfare/projects/mathieu/t/restore.py
 lino_welfare/projects/mathieu/tests/__init__.py
 lino_welfare/projects/mathieu/tests/test_chatelet.py
 lino_welfare/projects/mathieu/tests/test_notify.py
 lino_welfare/projects/mathieu/tmp/restore.py
 lino_welfare/projects/weleup1r/__init__.py
 lino_welfare/projects/weleup1r/manage.py
 lino_welfare/projects/weleup1r/settings.py
```

### Comparing `lino-welfare-24.3.1/tasks.py` & `lino-welfare-24.5.0/tasks.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-24.3.1/tests/__init__.py` & `lino-welfare-24.5.0/tests/__init__.py`

 * *Files identical despite different names*

