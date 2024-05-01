# Comparing `tmp/segdb-0.0.1.tar.gz` & `tmp/segdb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segdb-0.0.1.tar", last modified: Thu Nov 16 12:37:34 2023, max compression
+gzip compressed data, was "segdb-0.0.3.tar", last modified: Wed May  1 13:31:42 2024, max compression
```

## Comparing `segdb-0.0.1.tar` & `segdb-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.206927 segdb-0.0.1/
--rw-r--r--   0 leonard   (1003) leonard   (1004)     6509 2023-11-16 12:37:34.202927 segdb-0.0.1/PKG-INFO
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     6043 2023-11-16 10:13:17.000000 segdb-0.0.1/README.md
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/segdb/
--rw-rw-r--   0 leonard   (1003) leonard   (1004)        0 2023-06-02 06:44:14.000000 segdb-0.0.1/segdb/__init__.py
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/segdb/classes/
--rw-rw-r--   0 leonard   (1003) leonard   (1004)      815 2023-06-02 09:49:05.000000 segdb-0.0.1/segdb/classes/Color.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     1042 2023-06-02 09:50:24.000000 segdb-0.0.1/segdb/classes/DB.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     6812 2023-11-16 10:11:10.000000 segdb-0.0.1/segdb/classes/Segment.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     1249 2023-06-02 09:50:56.000000 segdb-0.0.1/segdb/classes/Triplet.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)        0 2023-05-22 16:29:00.000000 segdb-0.0.1/segdb/classes/__init__.py
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/segdb/data/
--rw-rw-r--   0 leonard   (1003) leonard   (1004)      232 2023-06-01 16:30:20.000000 segdb-0.0.1/segdb/data/categories.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)       99 2023-06-01 12:45:57.000000 segdb-0.0.1/segdb/data/modifiers.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)    11464 2023-11-16 11:08:49.000000 segdb-0.0.1/segdb/data/segmentations.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     6670 2023-11-16 09:56:28.000000 segdb-0.0.1/segdb/data/types.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     2067 2023-06-02 09:48:00.000000 segdb-0.0.1/segdb/lookup.py
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/segdb/tools/
--rw-rw-r--   0 leonard   (1003) leonard   (1004)       60 2023-06-02 06:44:32.000000 segdb-0.0.1/segdb/tools/__init__.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     3552 2023-08-09 09:32:10.000000 segdb-0.0.1/segdb/tools/dcmqi_config_generator.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     3767 2023-05-22 17:03:40.000000 segdb-0.0.1/segdb/tools/generator.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)        0 2023-05-22 17:01:00.000000 segdb-0.0.1/segdb/tools/generator2.py
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     6102 2023-05-23 10:18:15.000000 segdb-0.0.1/segdb/tools/importer.py
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/segdb.egg-info/
--rw-r--r--   0 leonard   (1003) leonard   (1004)     6509 2023-11-16 12:37:34.000000 segdb-0.0.1/segdb.egg-info/PKG-INFO
--rw-rw-r--   0 leonard   (1003) leonard   (1004)      729 2023-11-16 12:37:34.000000 segdb-0.0.1/segdb.egg-info/SOURCES.txt
--rw-rw-r--   0 leonard   (1003) leonard   (1004)        1 2023-11-16 12:37:34.000000 segdb-0.0.1/segdb.egg-info/dependency_links.txt
--rw-rw-r--   0 leonard   (1003) leonard   (1004)        7 2023-11-16 12:37:34.000000 segdb-0.0.1/segdb.egg-info/requires.txt
--rw-rw-r--   0 leonard   (1003) leonard   (1004)       18 2023-11-16 12:37:34.000000 segdb-0.0.1/segdb.egg-info/top_level.txt
--rw-rw-r--   0 leonard   (1003) leonard   (1004)       38 2023-11-16 12:37:34.206927 segdb-0.0.1/setup.cfg
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     1253 2023-11-16 12:37:27.000000 segdb-0.0.1/setup.py
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/ymldicomseg/
--rw-rw-r--   0 leonard   (1003) leonard   (1004)       26 2023-05-22 15:44:48.000000 segdb-0.0.1/ymldicomseg/__init__.py
-drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2023-11-16 12:37:34.202927 segdb-0.0.1/ymldicomseg/data/
--rw-rw-r--   0 leonard   (1003) leonard   (1004)      100 2023-05-22 15:44:48.000000 segdb-0.0.1/ymldicomseg/data/categories.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)       81 2023-05-22 15:44:48.000000 segdb-0.0.1/ymldicomseg/data/modifyers.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     6561 2023-05-22 15:44:48.000000 segdb-0.0.1/ymldicomseg/data/segmentations.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)      856 2023-05-22 15:44:48.000000 segdb-0.0.1/ymldicomseg/data/types.csv
--rw-rw-r--   0 leonard   (1003) leonard   (1004)     3767 2023-05-22 15:44:48.000000 segdb-0.0.1/ymldicomseg/ymldicomseg.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/
+-rw-r--r--   0 leonard   (1003) leonard   (1004)     6509 2024-05-01 13:31:42.099676 segdb-0.0.3/PKG-INFO
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     6043 2023-11-16 10:13:17.000000 segdb-0.0.3/README.md
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.095676 segdb-0.0.3/segdb/
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)        0 2023-06-02 06:44:14.000000 segdb-0.0.3/segdb/__init__.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/segdb/classes/
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)      815 2023-06-02 09:49:05.000000 segdb-0.0.3/segdb/classes/Color.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     1042 2023-06-02 09:50:24.000000 segdb-0.0.3/segdb/classes/DB.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)    16610 2024-03-28 13:05:29.000000 segdb-0.0.3/segdb/classes/Segment.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     2437 2024-03-28 09:56:57.000000 segdb-0.0.3/segdb/classes/Triplet.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)        0 2023-05-22 16:29:00.000000 segdb-0.0.3/segdb/classes/__init__.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/segdb/data/
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)      232 2023-06-01 16:30:20.000000 segdb-0.0.3/segdb/data/categories.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)       99 2023-06-01 12:45:57.000000 segdb-0.0.3/segdb/data/modifiers.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)    14548 2023-12-11 13:32:08.000000 segdb-0.0.3/segdb/data/segmentations.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     9917 2023-12-11 13:27:34.000000 segdb-0.0.3/segdb/data/types.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     2067 2024-03-28 09:10:46.000000 segdb-0.0.3/segdb/lookup.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/segdb/tools/
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)       60 2023-06-02 06:44:32.000000 segdb-0.0.3/segdb/tools/__init__.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     3552 2023-08-09 09:32:10.000000 segdb-0.0.3/segdb/tools/dcmqi_config_generator.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     3767 2023-05-22 17:03:40.000000 segdb-0.0.3/segdb/tools/generator.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)        0 2023-05-22 17:01:00.000000 segdb-0.0.3/segdb/tools/generator2.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     6102 2023-05-23 10:18:15.000000 segdb-0.0.3/segdb/tools/importer.py
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)      586 2024-03-28 09:10:46.000000 segdb-0.0.3/segdb/tools/segdb_navigator.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/segdb.egg-info/
+-rw-r--r--   0 leonard   (1003) leonard   (1004)     6509 2024-05-01 13:31:42.000000 segdb-0.0.3/segdb.egg-info/PKG-INFO
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)      760 2024-05-01 13:31:42.000000 segdb-0.0.3/segdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)        1 2024-05-01 13:31:42.000000 segdb-0.0.3/segdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)        7 2024-05-01 13:31:42.000000 segdb-0.0.3/segdb.egg-info/requires.txt
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)       18 2024-05-01 13:31:42.000000 segdb-0.0.3/segdb.egg-info/top_level.txt
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)       38 2024-05-01 13:31:42.099676 segdb-0.0.3/setup.cfg
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     1253 2024-05-01 13:03:18.000000 segdb-0.0.3/setup.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/ymldicomseg/
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)       26 2023-05-22 15:44:48.000000 segdb-0.0.3/ymldicomseg/__init__.py
+drwxrwxr-x   0 leonard   (1003) leonard   (1004)        0 2024-05-01 13:31:42.099676 segdb-0.0.3/ymldicomseg/data/
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)      100 2023-05-22 15:44:48.000000 segdb-0.0.3/ymldicomseg/data/categories.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)       81 2023-05-22 15:44:48.000000 segdb-0.0.3/ymldicomseg/data/modifyers.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     6561 2023-05-22 15:44:48.000000 segdb-0.0.3/ymldicomseg/data/segmentations.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)      856 2023-05-22 15:44:48.000000 segdb-0.0.3/ymldicomseg/data/types.csv
+-rw-rw-r--   0 leonard   (1003) leonard   (1004)     3767 2023-05-22 15:44:48.000000 segdb-0.0.3/ymldicomseg/ymldicomseg.py
```

### Comparing `segdb-0.0.1/PKG-INFO` & `segdb-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segdb
-Version: 0.0.1
+Version: 0.0.3
 Summary: Database for uniform body segmentation.
 Home-page: https://github.com/MHubAI/SegDB
 Author: Leonard Nürnberg
 Author-email: lnuernberg@bwh.harvard.edu
 License: MIT
 Keywords: mhub
 Classifier: Development Status :: 4 - Beta
```

### Comparing `segdb-0.0.1/README.md` & `segdb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb/classes/Color.py` & `segdb-0.0.3/segdb/classes/Color.py`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb/classes/DB.py` & `segdb-0.0.3/segdb/classes/DB.py`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb/data/segmentations.csv` & `segdb-0.0.3/segdb/data/segmentations.csv`

 * *Files 17% similar despite different names*

```diff
@@ -103,24 +103,54 @@
 VERTEBRAE_T3,Vertebrae T3,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T3_STRUCTURE,,"241,214,145"
 VERTEBRAE_T4,Vertebrae T4,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T4_STRUCTURE,,"241,214,145"
 VERTEBRAE_T5,Vertebrae T5,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T5_STRUCTURE,,"241,214,145"
 VERTEBRAE_T6,Vertebrae T6,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T6_STRUCTURE,,"241,214,145"
 VERTEBRAE_T7,Vertebrae T7,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T7_STRUCTURE,,"241,214,145"
 VERTEBRAE_T8,Vertebrae T8,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T8_STRUCTURE,,"241,214,145"
 VERTEBRAE_T9,Vertebrae T9,C_TISSUE_STRUCTURE,T_BONE_VERTEBRAE_T9_STRUCTURE,,"241,214,145"
+VERTEBRAE_DISK_C2C3,Vertebrae Disk C2/C3,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_C2C3_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_C3C4,Vertebrae Disk C3/C4,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_C3C4_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_C4C5,Vertebrae Disk C4/C5,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_C4C5_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_C5C6,Vertebrae Disk C5/C6,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_C5C6_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_C6C7,Vertebrae Disk C6/C7,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_C6C7_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_C7T1,Vertebrae Disk C7/T1,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_C7T1_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T1T2,Vertebrae Disk T1/T2,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T1T2_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T2T3,Vertebrae Disk T2/T3,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T2T3_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T3T4,Vertebrae Disk T3/T4,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T3T4_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T4T5,Vertebrae Disk T4/T5,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T4T5_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T5T6,Vertebrae Disk T5/T6,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T5T6_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T6T7,Vertebrae Disk T6/T7,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T6T7_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T7T8,Vertebrae Disk T7/T8,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T7T8_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T8T9,Vertebrae Disk T8/T9,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T8T9_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T9T10,Vertebrae Disk T9/T10,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T9T10_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T10T11,Vertebrae Disk T10/T11,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T10T11_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T11T12,Vertebrae Disk T11/T12,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T11T12_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_T12L1,Vertebrae Disk T12/L1,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_T12L1_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_L1L2,Vertebrae Disk L1/L2,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_L1L2_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_L2L3,Vertebrae Disk L2/L3,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_L2L3_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_L3L4,Vertebrae Disk L3/L4,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_L3L4_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_L4L5,Vertebrae Disk L4/L5,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_L4L5_STRUCTURE,,"191, 169, 113"
+VERTEBRAE_DISK_L5S1,Vertebrae Disk L5/S1,C_BODY_STRUCTURE,T_DISK_VERTEBRAE_L5S1_STRUCTURE,,"191, 169, 113"
 CORONARY_ARTERY_RIGHT,Right Coronary Artery,C_BODY_STRUCTURE,T_ARTERY_CORONARY_RIGHT_STRUCTURE,,"172,74,74"
 CORONARY_ARTERY_LEFT,Left Coronary Artery,C_BODY_STRUCTURE,T_ARTERY_CORONARY_LEFT_STRUCTURE,,"172,74,74"
 CORONARY_ARTERY_CFLX,Circumflex Branch of the Coronary Artery,C_BODY_STRUCTURE,T_ARTERY_CORONARY_CFLX_LEFT_STRUCTURE,,"233,123,123"
 CORONARY_ARTERY_LAD,Left Anterior Descending Coronary Artery,C_BODY_STRUCTURE,T_ARTERY_CORONARY_AD_LEFT_STRUCTURE,,"180,49,49"
 CORONARY_ARTERY,Coronary Artery,C_BODY_STRUCTURE,T_ARTERY_CORONARY_STRUCTURE,,"172,74,74"
 HEART,Heart,C_BODY_STRUCTURE,T_HEART_STRUCTURE,,"206,110,84"
 NEOPLASM_MALIGNANT_PRIMARY,Primary malignant neoplasm,C_MORPHOLOGICALLY_ABNORMAL_STRUCTURE,T_NEOPLASM_MALIGNANT_PRIMARY_MABNORMALITY,,"255,0,0"
 AORTIC_VALVE,Aortic valve,C_BODY_STRUCTURE,T_VALVE_AORTIC_STRUCTURE,,"218,123,97"
 MITRAL_VALVE,Mitral valve,C_BODY_STRUCTURE,T_VALVE_MITRAL_STRUCTURE,,"159,63,27"
 PULMONARY_VALVE,Pulmonary valve,C_BODY_STRUCTURE,T_VALVE_PULMONARY_STRUCTURE,,"225,130,104"
 TRICUSPID_VALVE,Tricuspid valve,C_BODY_STRUCTURE,T_VALVE_TRICUSPID_STRUCTURE,,"166,70,38"
 SINOTRIAL_NODE,Sinoatrial conduction node,C_BODY_STRUCTURE,T_NODE_SINOATRIAL_STRUCTURE,,"255,255,255"
 ATRIOVENTRICULAR_NODE,Atrioventricular conduction node,C_BODY_STRUCTURE,T_NODE_ATRIOVENTRICULAR_STRUCTURE,,"255,255,255"
 PROSTATE,Prostate,C_BODY_STRUCTURE,T_PROSTATIC_STRUCTURE,,"230,158,140"
+PROSTATE_PERIPHERAL_ZONE,Peripheral zone of prostate,C_BODY_STRUCTURE,T_PROSTATIC_PZ_STRUCTURE,,"230,149,140"
+PROSTATE_TRANSITION_ZONE,Transition zone of prostate,C_BODY_STRUCTURE,T_PROSTATIC_TZ_STRUCTURE,,"230,194,140"
 CYST,Cyst,C_MORPHOLOGICALLY_ABNORMAL_STRUCTURE,T_CYST_MABNORMALITY,,"150,87,42"
 SPINAL_CANAL,Spinal canal,C_BODY_STRUCTURE,T_SPINAL_CANAL_STRUCTURE,,"204,99,61"
-PATHOLOGIC_CALCIFICATION,Pathologic calcification,C_MORPHOLOGICALLY_ABNORMAL_STRUCTURE,T_PATHOLOGIC_CALCIFICATION_MABNORMALITY,,"255,255,255"
+PATHOLOGIC_CALCIFICATION,Pathologic calcification,C_MORPHOLOGICALLY_ABNORMAL_STRUCTURE,T_PATHOLOGIC_CALCIFICATION_MABNORMALITY,,"255,255,255"
+PANCREATIC_DUCT,Pancreatic duct,C_BODY_STRUCTURE,T_PANCREATIC_DUCT_STRUCTURE,,"173,61,29"
+BILE_DUCT,Bile duct,C_BODY_STRUCTURE,T_BILE_DUCT_STRUCTURE,,"217,36,36"
+RENAL_VEIN,Renal vein,C_BODY_STRUCTURE,T_RENAL_VEIN_STRUCTURE,,"222,22,22"
+ARTERY,Artery (unspecific),C_BODY_STRUCTURE,T_ARTERIAL_STRUCTURE,,"171,27,30"
+VEIN,Vein (unspecific),C_BODY_STRUCTURE,T_VENOUS_STRUCTURE,,"27,9,99"
```

### Comparing `segdb-0.0.1/segdb/lookup.py` & `segdb-0.0.3/segdb/lookup.py`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb/tools/dcmqi_config_generator.py` & `segdb-0.0.3/segdb/tools/dcmqi_config_generator.py`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb/tools/generator.py` & `segdb-0.0.3/segdb/tools/generator.py`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb/tools/importer.py` & `segdb-0.0.3/segdb/tools/importer.py`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/segdb.egg-info/PKG-INFO` & `segdb-0.0.3/segdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segdb
-Version: 0.0.1
+Version: 0.0.3
 Summary: Database for uniform body segmentation.
 Home-page: https://github.com/MHubAI/SegDB
 Author: Leonard Nürnberg
 Author-email: lnuernberg@bwh.harvard.edu
 License: MIT
 Keywords: mhub
 Classifier: Development Status :: 4 - Beta
```

### Comparing `segdb-0.0.1/segdb.egg-info/SOURCES.txt` & `segdb-0.0.3/segdb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 segdb/data/segmentations.csv
 segdb/data/types.csv
 segdb/tools/__init__.py
 segdb/tools/dcmqi_config_generator.py
 segdb/tools/generator.py
 segdb/tools/generator2.py
 segdb/tools/importer.py
+segdb/tools/segdb_navigator.py
 ymldicomseg/__init__.py
 ymldicomseg/ymldicomseg.py
 ymldicomseg/data/categories.csv
 ymldicomseg/data/modifyers.csv
 ymldicomseg/data/segmentations.csv
 ymldicomseg/data/types.csv
```

### Comparing `segdb-0.0.1/setup.py` & `segdb-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 # install locally via `pip install -e .` (-> for development)
 # install from github via `pip install git+https://github.com/MHubAI/mhubio (-> in Dockerfiles)
 
 setuptools.setup(
     name = "segdb",
-    version = "0.0.1",
+    version = "0.0.3",
     author = "Leonard Nürnberg",
     author_email = "lnuernberg@bwh.harvard.edu",
     description = ("Database for uniform body segmentation."),
     license = "MIT",
     keywords = "mhub",
     url = "https://github.com/MHubAI/SegDB",
     packages=setuptools.find_packages(),
```

### Comparing `segdb-0.0.1/ymldicomseg/data/segmentations.csv` & `segdb-0.0.3/ymldicomseg/data/segmentations.csv`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/ymldicomseg/data/types.csv` & `segdb-0.0.3/ymldicomseg/data/types.csv`

 * *Files identical despite different names*

### Comparing `segdb-0.0.1/ymldicomseg/ymldicomseg.py` & `segdb-0.0.3/ymldicomseg/ymldicomseg.py`

 * *Files identical despite different names*

