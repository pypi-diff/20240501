# Comparing `tmp/aps-toolkit-0.5.1.tar.gz` & `tmp/aps-toolkit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.5.1.tar", last modified: Wed May  1 11:54:48 2024, max compression
+gzip compressed data, was "aps-toolkit-0.5.2.tar", last modified: Wed May  1 12:05:57 2024, max compression
```

## Comparing `aps-toolkit-0.5.1.tar` & `aps-toolkit-0.5.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 11:54:48.527213 aps-toolkit-0.5.1/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-01 11:54:48.526984 aps-toolkit-0.5.1/PKG-INFO
--rw-r--r--   0 chuongmep   (501) staff       (20)       38 2024-05-01 11:54:48.527258 aps-toolkit-0.5.1/setup.cfg
--rw-r--r--   0 chuongmep   (501) staff       (20)      874 2024-05-01 11:54:44.000000 aps-toolkit-0.5.1/setup.py
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 11:54:48.518204 aps-toolkit-0.5.1/src/
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 11:54:48.523456 aps-toolkit-0.5.1/src/aps_toolkit/
--rw-r--r--   0 chuongmep   (501) staff       (20)     4641 2024-05-01 11:49:58.000000 aps-toolkit-0.5.1/src/aps_toolkit/Auth.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    10134 2024-03-27 11:22:45.000000 aps-toolkit-0.5.1/src/aps_toolkit/BIM360.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     8892 2024-03-27 12:37:29.000000 aps-toolkit-0.5.1/src/aps_toolkit/Bucket.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2449 2024-03-24 09:10:01.000000 aps-toolkit-0.5.1/src/aps_toolkit/DbReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    12604 2024-03-24 09:10:01.000000 aps-toolkit-0.5.1/src/aps_toolkit/Derivative.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3845 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/Fragments.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2322 2024-03-27 12:03:33.000000 aps-toolkit-0.5.1/src/aps_toolkit/InputStream.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      880 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/aps_toolkit/ManifestItem.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1136 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/MaterialProperties.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1726 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/Materials.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3686 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/PackFileReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      925 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/aps_toolkit/PathInfo.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     4471 2024-03-21 13:54:46.000000 aps-toolkit-0.5.1/src/aps_toolkit/ProDbReaderCad.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3505 2024-03-24 09:10:01.000000 aps-toolkit-0.5.1/src/aps_toolkit/ProDbReaderNavis.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    13555 2024-03-19 13:36:16.000000 aps-toolkit-0.5.1/src/aps_toolkit/ProDbReaderRevit.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    13105 2024-03-27 11:22:45.000000 aps-toolkit-0.5.1/src/aps_toolkit/PropReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1376 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/Resource.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1067 2024-03-21 15:00:38.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFContent.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3333 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFGeometries.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1160 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFImage.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1037 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFLines.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      830 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFManifestType.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      886 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterialGroup.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      773 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterialMap.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      834 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterialMapScale.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     7567 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterials.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     9759 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFMesh.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      859 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFMetadata.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      936 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFPoints.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     6690 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFTransform.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      799 2024-03-17 07:21:07.000000 aps-toolkit-0.5.1/src/aps_toolkit/SVFUVMap.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      983 2024-03-27 11:30:06.000000 aps-toolkit-0.5.1/src/aps_toolkit/Token.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      701 2024-03-27 11:35:19.000000 aps-toolkit-0.5.1/src/aps_toolkit/__init__.py
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 11:54:48.524173 aps-toolkit-0.5.1/src/aps_toolkit.egg-info/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-01 11:54:48.000000 aps-toolkit-0.5.1/src/aps_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 chuongmep   (501) staff       (20)     1722 2024-05-01 11:54:48.000000 aps-toolkit-0.5.1/src/aps_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)        1 2024-05-01 11:54:48.000000 aps-toolkit-0.5.1/src/aps_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)       16 2024-05-01 11:54:48.000000 aps-toolkit-0.5.1/src/aps_toolkit.egg-info/requires.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)       17 2024-05-01 11:54:48.000000 aps-toolkit-0.5.1/src/aps_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 11:54:48.526708 aps-toolkit-0.5.1/src/test/
--rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-03-12 14:17:11.000000 aps-toolkit-0.5.1/src/test/__init__.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      946 2024-03-27 11:35:19.000000 aps-toolkit-0.5.1/src/test/context.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      826 2024-05-01 11:50:43.000000 aps-toolkit-0.5.1/src/test/test_auth.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2668 2024-03-27 11:22:45.000000 aps-toolkit-0.5.1/src/test/test_bim360.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1962 2024-03-27 12:24:47.000000 aps-toolkit-0.5.1/src/test/test_bucket.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      836 2024-03-24 09:10:01.000000 aps-toolkit-0.5.1/src/test/test_db_reader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1874 2024-03-24 09:10:01.000000 aps-toolkit-0.5.1/src/test/test_derivative.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      997 2024-03-13 15:06:23.000000 aps-toolkit-0.5.1/src/test/test_fragment.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      858 2024-03-13 15:27:50.000000 aps-toolkit-0.5.1/src/test/test_geometries.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      766 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/test/test_image.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1233 2024-03-13 15:27:50.000000 aps-toolkit-0.5.1/src/test/test_material.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      691 2024-03-13 15:27:50.000000 aps-toolkit-0.5.1/src/test/test_mesh.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      494 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/test/test_metadata.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1840 2024-03-27 11:22:45.000000 aps-toolkit-0.5.1/src/test/test_prop_reader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-03-21 13:54:46.000000 aps-toolkit-0.5.1/src/test/test_prop_reader_cad.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      777 2024-03-24 09:10:01.000000 aps-toolkit-0.5.1/src/test/test_prop_reader_navis.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3383 2024-03-12 14:17:11.000000 aps-toolkit-0.5.1/src/test/test_prop_reader_revit.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2915 2024-03-23 03:57:09.000000 aps-toolkit-0.5.1/src/test/test_svf_reader.py
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:05:57.219789 aps-toolkit-0.5.2/
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-01 12:05:57.219558 aps-toolkit-0.5.2/PKG-INFO
+-rw-r--r--   0 chuongmep   (501) staff       (20)       38 2024-05-01 12:05:57.219832 aps-toolkit-0.5.2/setup.cfg
+-rw-r--r--   0 chuongmep   (501) staff       (20)      874 2024-05-01 12:05:46.000000 aps-toolkit-0.5.2/setup.py
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:05:57.203537 aps-toolkit-0.5.2/src/
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:05:57.213311 aps-toolkit-0.5.2/src/aps_toolkit/
+-rw-r--r--   0 chuongmep   (501) staff       (20)     4895 2024-05-01 12:05:24.000000 aps-toolkit-0.5.2/src/aps_toolkit/Auth.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    10134 2024-03-27 11:22:45.000000 aps-toolkit-0.5.2/src/aps_toolkit/BIM360.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     8892 2024-03-27 12:37:29.000000 aps-toolkit-0.5.2/src/aps_toolkit/Bucket.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2449 2024-03-24 09:10:01.000000 aps-toolkit-0.5.2/src/aps_toolkit/DbReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    12604 2024-03-24 09:10:01.000000 aps-toolkit-0.5.2/src/aps_toolkit/Derivative.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3845 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/Fragments.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2322 2024-03-27 12:03:33.000000 aps-toolkit-0.5.2/src/aps_toolkit/InputStream.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      880 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/aps_toolkit/ManifestItem.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1136 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/MaterialProperties.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1726 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/Materials.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3686 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/PackFileReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      925 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/aps_toolkit/PathInfo.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     4471 2024-03-21 13:54:46.000000 aps-toolkit-0.5.2/src/aps_toolkit/ProDbReaderCad.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3505 2024-03-24 09:10:01.000000 aps-toolkit-0.5.2/src/aps_toolkit/ProDbReaderNavis.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    13555 2024-03-19 13:36:16.000000 aps-toolkit-0.5.2/src/aps_toolkit/ProDbReaderRevit.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    13105 2024-03-27 11:22:45.000000 aps-toolkit-0.5.2/src/aps_toolkit/PropReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1376 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/Resource.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1067 2024-03-21 15:00:38.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFContent.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3333 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFGeometries.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1160 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFImage.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1037 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFLines.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      830 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFManifestType.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      886 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterialGroup.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      773 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterialMap.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      834 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     7567 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterials.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     9759 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFMesh.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      859 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFMetadata.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      936 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFPoints.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     6690 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFTransform.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      799 2024-03-17 07:21:07.000000 aps-toolkit-0.5.2/src/aps_toolkit/SVFUVMap.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      983 2024-03-27 11:30:06.000000 aps-toolkit-0.5.2/src/aps_toolkit/Token.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      701 2024-03-27 11:35:19.000000 aps-toolkit-0.5.2/src/aps_toolkit/__init__.py
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:05:57.214066 aps-toolkit-0.5.2/src/aps_toolkit.egg-info/
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-01 12:05:57.000000 aps-toolkit-0.5.2/src/aps_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1722 2024-05-01 12:05:57.000000 aps-toolkit-0.5.2/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 chuongmep   (501) staff       (20)        1 2024-05-01 12:05:57.000000 aps-toolkit-0.5.2/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 chuongmep   (501) staff       (20)       16 2024-05-01 12:05:57.000000 aps-toolkit-0.5.2/src/aps_toolkit.egg-info/requires.txt
+-rw-r--r--   0 chuongmep   (501) staff       (20)       17 2024-05-01 12:05:57.000000 aps-toolkit-0.5.2/src/aps_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-01 12:05:57.219092 aps-toolkit-0.5.2/src/test/
+-rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-03-12 14:17:11.000000 aps-toolkit-0.5.2/src/test/__init__.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      946 2024-03-27 11:35:19.000000 aps-toolkit-0.5.2/src/test/context.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      757 2024-05-01 12:05:24.000000 aps-toolkit-0.5.2/src/test/test_auth.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2668 2024-03-27 11:22:45.000000 aps-toolkit-0.5.2/src/test/test_bim360.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1962 2024-03-27 12:24:47.000000 aps-toolkit-0.5.2/src/test/test_bucket.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      836 2024-03-24 09:10:01.000000 aps-toolkit-0.5.2/src/test/test_db_reader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1874 2024-03-24 09:10:01.000000 aps-toolkit-0.5.2/src/test/test_derivative.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      997 2024-03-13 15:06:23.000000 aps-toolkit-0.5.2/src/test/test_fragment.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      858 2024-03-13 15:27:50.000000 aps-toolkit-0.5.2/src/test/test_geometries.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      766 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/test/test_image.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1233 2024-03-13 15:27:50.000000 aps-toolkit-0.5.2/src/test/test_material.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      691 2024-03-13 15:27:50.000000 aps-toolkit-0.5.2/src/test/test_mesh.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      494 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/test/test_metadata.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1840 2024-03-27 11:22:45.000000 aps-toolkit-0.5.2/src/test/test_prop_reader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-03-21 13:54:46.000000 aps-toolkit-0.5.2/src/test/test_prop_reader_cad.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      777 2024-03-24 09:10:01.000000 aps-toolkit-0.5.2/src/test/test_prop_reader_navis.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3383 2024-03-12 14:17:11.000000 aps-toolkit-0.5.2/src/test/test_prop_reader_revit.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2915 2024-03-23 03:57:09.000000 aps-toolkit-0.5.2/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.5.1/PKG-INFO` & `aps-toolkit-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.1/setup.py` & `aps-toolkit-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.5.1",
+    version="0.5.2",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Auth.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,21 @@
         content = response.json()
         access_token = content['access_token']
         expires_in = content['expires_in']
         token_type = content['token_type']
         result = Token(access_token, token_type, expires_in)
         return result
 
-    def auth3leg(self, callback_url, scopes):
+    def auth3leg(self, callback_url=None, scopes=None) -> Token:
+        if not scopes:
+            scopes = 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'
+        if not callback_url:
+            # Default callback url
+            callback_url = "http://localhost:8080/api/auth/callback"
+
         class CallbackHandler(BaseHTTPRequestHandler):
             def do_GET(self):
                 nonlocal auth_instance
                 query = urllib.parse.urlparse(self.path).query
                 params = urllib.parse.parse_qs(query)
                 code = params.get('code', [''])[0]
                 if code:
@@ -73,39 +79,38 @@
                     self.end_headers()
                     self.wfile.write(b"Authentication successful. You can close this window now.")
                     result_token = handle_callback(callback_url, code)
                     auth_instance.access_token = result_token['access_token']
                     auth_instance.token_type = result_token['token_type']
                     auth_instance.expires_in = result_token['expires_in']
                     auth_instance.refresh_token = result_token.get('refresh_token')
-                    # self.server.shutdown()
 
                 else:
                     self.send_response(400)
                     self.end_headers()
                     self.wfile.write(b"Bad Request")
-                    # self.server.shutdown()
 
         def handle_callback(callback_url, code):
             tokenUrl = "https://developer.api.autodesk.com/authentication/v2/token"
             payload = {
                 "grant_type": "authorization_code",
                 "code": code,
                 "client_id": self.client_id,
                 "client_secret": self.client_secret,
                 "redirect_uri": callback_url
             }
             resp = requests.post(tokenUrl, data=payload)
+            if resp.status_code != 200:
+                raise Exception(resp.content)
             respJson = resp.json()
             return respJson
 
         def start_callback_server():
             server_address = ('', 8080)
             httpd = HTTPServer(server_address, CallbackHandler)
-            print('Starting callback server...')
             httpd.handle_request()
 
         auth_instance = self  # Reference to the Auth instance
 
         auth_url = f"https://developer.api.autodesk.com/authentication/v2/authorize?response_type=code&client_id={self.client_id}&redirect_uri={callback_url}&scope={scopes}"
         webbrowser.open(auth_url)
         start_callback_server()
```

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.5.2/src/aps_toolkit/BIM360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.5.2/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.5.2/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.5.2/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.5.2/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Materials.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.5.2/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.5.2/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.5.2/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.5.2/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.5.2/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.5.2/src/aps_toolkit/PropReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Resource.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.5.2/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/Token.py` & `aps-toolkit-0.5.2/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit/__init__.py` & `aps-toolkit-0.5.2/src/aps_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.5.2/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.1/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.5.2/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/context.py` & `aps-toolkit-0.5.2/src/test/context.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_auth.py` & `aps-toolkit-0.5.2/src/test/test_auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,10 +17,8 @@
         self.assertNotEquals(token.access_token, "")
 
     def test_auth3leg(self):
         auth = Auth()
         redirect_uri = "http://localhost:8080/api/auth/callback"
         scopes = 'data:read viewables:read'
         token = auth.auth3leg(redirect_uri, scopes)
-        print(token.access_token)
-        print(token.refresh_token)
         self.assertNotEquals(token.access_token, "")
```

### Comparing `aps-toolkit-0.5.1/src/test/test_bim360.py` & `aps-toolkit-0.5.2/src/test/test_bim360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_bucket.py` & `aps-toolkit-0.5.2/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_db_reader.py` & `aps-toolkit-0.5.2/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_derivative.py` & `aps-toolkit-0.5.2/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_fragment.py` & `aps-toolkit-0.5.2/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_geometries.py` & `aps-toolkit-0.5.2/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_image.py` & `aps-toolkit-0.5.2/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_material.py` & `aps-toolkit-0.5.2/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_mesh.py` & `aps-toolkit-0.5.2/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_prop_reader.py` & `aps-toolkit-0.5.2/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.5.2/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.5.2/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.5.2/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.1/src/test/test_svf_reader.py` & `aps-toolkit-0.5.2/src/test/test_svf_reader.py`

 * *Files identical despite different names*

