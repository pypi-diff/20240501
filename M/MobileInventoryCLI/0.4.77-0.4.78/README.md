# Comparing `tmp/MobileInventoryCLI-0.4.77.tar.gz` & `tmp/MobileInventoryCLI-0.4.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.77.tar", last modified: Tue Apr 30 17:49:37 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.78.tar", last modified: Tue Apr 30 18:21:12 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.77.tar` & `MobileInventoryCLI-0.4.78.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.334521 MobileInventoryCLI-0.4.77/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.334521 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.334521 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.334521 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.334521 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.334521 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   112310 2024-04-30 17:44:29.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    79243 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.337854 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-30 17:49:33.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2249 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-30 14:15:01.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-30 17:49:37.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-04-30 17:49:37.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-30 17:49:37.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-30 17:49:37.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-30 17:49:37.000000 MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-30 17:49:37.341188 MobileInventoryCLI-0.4.77/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-30 17:49:37.000000 MobileInventoryCLI-0.4.77/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.977936 MobileInventoryCLI-0.4.78/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.964603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.964603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.967936 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.967936 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.967936 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.967936 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   112964 2024-04-30 18:18:34.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.971269 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    79243 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-30 18:19:59.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2376 2024-04-30 18:21:09.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-30 17:49:46.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 18:21:12.974603 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-30 18:21:12.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-04-30 18:21:12.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-30 18:21:12.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-30 18:21:12.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-30 18:21:12.000000 MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-30 18:21:12.977936 MobileInventoryCLI-0.4.78/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-30 18:21:12.977936 MobileInventoryCLI-0.4.78/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-30 18:21:12.000000 MobileInventoryCLI-0.4.78/setup.py
```

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from qrcode import QRCode
 from barcode.writer import ImageWriter
 import csv,string,random
 import shutil,upcean
 import MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.possibleCode as pc
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.renderText2Png import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.DatePicker import *
 import geocoder
 
 filename="codesAndBarcodes.db"
 DEVMOD=False
 if DEVMOD:
     if Path(filename).exists():
         Path(filename).unlink()
@@ -2083,16 +2084,17 @@
             elif field.lower() in ['back','b']:
                 return
             elif field.lower() in ['?','help']:
                 self.helpTextPrint()
 
             if field not in self.valid_field_names:
                 raise Exception(f"InvalidField '{field}:{self.valid_field_names}'")
-            if field in ['Timestamp',]:
-                raise Exception(f"Field not supported for changes yet!")
+            
+            #if field in ['Timestamp',]:
+            #    raise Exception(f"Field not supported for changes yet!")
 
             with Session(self.engine) as session:
                 ext=code.lower().split('.')[0]
                 cd=code.lower().split('.')[-1]
                 if cd.lower() in ['q','quit']:
                     exit("user quit!")
                 elif cd.lower() in ['back','b']:
@@ -2172,15 +2174,24 @@
                             self.setValuePrompt(field,result[r],session)
                         except Exception as e:
                             print(e)
         else:
             self.helpTextPrint()
 
     def setValuePrompt(self,field,entry,session,value=None):
-        if field == 'Image':
+        if field == 'Timestamp':
+            while True:
+                try:
+                    timestamp_new=DateTimePkr()
+                    timestamp_new_f=timestamp_new.timestamp()
+                    value=timestamp_new_f
+                    break
+                except Exception as e:
+                    print(e)
+        elif field == 'Image':
                 while True:
                     try:
                         def mkPath(text,self):
                             try:
                                 p=Path(text)
                                 if p.exists() and p.is_file():
                                     return Path(p)
@@ -2208,29 +2219,35 @@
                                 ofile.write(d)
                         print(f"{Fore.light_green}{str(ifilePath.absolute())}{Fore.light_yellow} -> {Fore.light_red}{str(ofilePath.absolute())}{Style.reset}")
                         break
                     except Exception as e:
                         print(e)
         if not value:
             value=input(f"{Fore.green_yellow}Value {Fore.yellow}OLD{Style.reset}={Fore.tan}{getattr(entry,field)} {Style.reset}({Fore.green}{self.valid_fields[field]}{Style.reset}): ")
-        if value.lower() in ['q','quit']:
-            exit("user quit!")
-        elif value.lower() in ['b','back']:
-            return
-        elif value.lower() in ['?','help']:
-            self.helpTextPrint()
+            if value.lower() in ['q','quit']:
+                exit("user quit!")
+            elif value.lower() in ['b','back']:
+                return
+            elif value.lower() in ['?','help']:
+                self.helpTextPrint()
 
         if value not in ['']:
             t=self.valid_fields[field]
             if isinstance(t,String):
                 value=str(value)
             elif isinstance(t,Integer):
-                value=int(eval(value))
+                try:
+                    value=int(eval(value))
+                except Exception as e:
+                    value=int(value)
             elif isinstance(t,Float):
-                value=float(eval(value))
+                try:
+                    value=float(eval(value))
+                except Exception as e:
+                    value=float(value)
             elif isinstance(t,Boolean):
                 if value not in ['True','False','1','0']:
                     raise Exception(f"Not a Boolean: {['True','False','1','0']}")
                 value=bool(eval(value))
             setattr(entry,field,value)
             #as item was changed, log it in InList==True
             if field != 'InList':
```

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 								can be used to quick-show-list
 6:27 am 04-25-2024 -- added version value
 12:16 pm 04-25-2024 -- added EntryExtras class to add operator functionality to classes Entry and DayLog, so one can 						do:
 							a=Entry(Barcode='BARCODE',Code='CODE',Name='NAME',Price=1.99)
 							#any of [+|-|*|/|**]
 							b=a+10
 							b will be 11.99
+11:19 am 04-30-2024 -- added ability to add images from FS to db Images, added ability to edit timestamp using ie->ss-$barcode
```

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.77
+Version: 0.4.78
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.77/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.78/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.77/PKG-INFO` & `MobileInventoryCLI-0.4.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.77
+Version: 0.4.78
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.77/setup.py` & `MobileInventoryCLI-0.4.78/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.77'
+version='0.4.78'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

