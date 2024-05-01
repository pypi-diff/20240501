# Comparing `tmp/azuresphere_imagemetadata-0.0.4.tar.gz` & `tmp/azuresphere_imagemetadata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuresphere_imagemetadata-0.0.4.tar", last modified: Fri Nov 17 16:13:03 2023, max compression
+gzip compressed data, was "azuresphere_imagemetadata-0.0.5.tar", last modified: Wed May  1 14:20:41 2024, max compression
```

## Comparing `azuresphere_imagemetadata-0.0.4.tar` & `azuresphere_imagemetadata-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,60 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1784 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1016 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.415441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      341 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/certificates/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1078 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/certificates/app_test_sign.pfx
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      814 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/certificates/tp_app_test_sign.cer
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1075 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/guid_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1769 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/image.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9200 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/image_metadata.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_headers/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      341 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_headers/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1811 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_headers/image_metadata.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1587 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_headers/image_metadata_section.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      341 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4241 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/abi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3115 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/compression.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2361 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/debug.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8160 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/identity.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3175 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/image_policy.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/internal/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      341 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/internal/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5984 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/internal/capabilities.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2645 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/internal/onebl.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1214 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/metadata.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2183 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/metadata_id.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      948 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/not_implemented.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1654 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/required_offset.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1900 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/revocation.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2927 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/signature.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2843 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/temporary_image.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3828 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/utils.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      341 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3042 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/app_development.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4018 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/der_encoded.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2626 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/signing_info.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-17 16:13:03.415441 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1784 2023-11-17 16:13:03.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1940 2023-11-17 16:13:03.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-11-17 16:13:03.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       21 2023-11-17 16:13:03.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-11-17 16:13:03.000000 azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       67 2023-11-17 16:13:03.419441 azuresphere_imagemetadata-0.0.4/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1467 2023-11-17 16:12:37.000000 azuresphere_imagemetadata-0.0.4/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.768238 azuresphere_imagemetadata-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     2766 2024-05-01 14:20:41.768238 azuresphere_imagemetadata-0.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2024-05-01 14:20:41.768238 azuresphere_imagemetadata-0.0.5/setup.cfg
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.752238 azuresphere_imagemetadata-0.0.5/src/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.756238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/
+-rw-rw-r--   0 root         (0) root         (0)     1073 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1016 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/README.md
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.756238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/certificates/
+-rw-rw-r--   0 root         (0) root         (0)     1078 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/certificates/app_test_sign.pfx
+-rw-rw-r--   0 root         (0) root         (0)      814 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/certificates/tp_app_test_sign.cer
+-rw-rw-r--   0 root         (0) root         (0)     1075 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/guid_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1769 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/image.py
+-rw-rw-r--   0 root         (0) root         (0)     8739 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/image_manifest.py
+-rw-rw-r--   0 root         (0) root         (0)     9200 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/image_metadata.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.756238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_headers/
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_headers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1811 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_headers/image_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     1587 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_headers/image_metadata_section.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.764238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4241 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/abi.py
+-rw-rw-r--   0 root         (0) root         (0)     3115 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/compression.py
+-rw-rw-r--   0 root         (0) root         (0)     2361 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/debug.py
+-rw-rw-r--   0 root         (0) root         (0)     8160 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/identity.py
+-rw-rw-r--   0 root         (0) root         (0)     3175 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/image_policy.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.764238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/internal/
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/internal/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5984 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/internal/capabilities.py
+-rw-rw-r--   0 root         (0) root         (0)     2644 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/internal/onebl.py
+-rw-rw-r--   0 root         (0) root         (0)     1214 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     2183 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/metadata_id.py
+-rw-rw-r--   0 root         (0) root         (0)      948 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/not_implemented.py
+-rw-rw-r--   0 root         (0) root         (0)     1654 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/required_offset.py
+-rw-rw-r--   0 root         (0) root         (0)     1900 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/revocation.py
+-rw-rw-r--   0 root         (0) root         (0)     2926 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/signature.py
+-rw-rw-r--   0 root         (0) root         (0)     2843 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/temporary_image.py
+-rw-rw-r--   0 root         (0) root         (0)     3828 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/utils.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.764238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3042 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/app_development.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/der_encoded.py
+-rw-rw-r--   0 root         (0) root         (0)     2626 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/signing_info.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.768238 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2766 2024-05-01 14:20:41.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2464 2024-05-01 14:20:41.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-01 14:20:41.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       21 2024-05-01 14:20:41.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       26 2024-05-01 14:20:41.000000 azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-01 14:20:41.768238 azuresphere_imagemetadata-0.0.5/tests/
+-rw-rw-r--   0 root         (0) root         (0)     1116 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_certificate_files_match.py
+-rw-rw-r--   0 root         (0) root         (0)      651 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_dotnet_app.py
+-rw-rw-r--   0 root         (0) root         (0)     4421 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_knownset_recovery_files.py
+-rw-rw-r--   0 root         (0) root         (0)     2934 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_latest_recovery_files.py
+-rw-rw-r--   0 root         (0) root         (0)      588 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_package_version.py
+-rw-rw-r--   0 root         (0) root         (0)      752 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_parse_application.py
+-rw-rw-r--   0 root         (0) root         (0)     1579 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_parse_capability.py
+-rw-rw-r--   0 root         (0) root         (0)     3175 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_serialization.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2024-05-01 14:18:13.000000 azuresphere_imagemetadata-0.0.5/tests/test_signing.py
```

### Comparing `azuresphere_imagemetadata-0.0.4/LICENSE` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/LICENSE`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/README.md` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/README.md`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/certificates/app_test_sign.pfx` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/certificates/app_test_sign.pfx`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/certificates/tp_app_test_sign.cer` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/certificates/tp_app_test_sign.cer`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/guid_utils.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/guid_utils.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/image.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/image.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/image_metadata.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/image_metadata.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_headers/image_metadata.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_headers/image_metadata.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_headers/image_metadata_section.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_headers/image_metadata_section.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/abi.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/abi.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/compression.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/compression.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/debug.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/debug.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/identity.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/identity.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/image_policy.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/image_policy.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/internal/capabilities.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/internal/capabilities.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/internal/onebl.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/internal/onebl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from ..metadata import MetadataSection
 import struct
 
 
 class OneBlInformationSection(MetadataSection):
-
     """
     Documents the binary format of OneBlInformation:
         uint32_t Information1
         uint32_t Information2
         uint32_t Information3
         uint32_t ChipId
         uint32_t Major
```

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/metadata.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/metadata.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/metadata_id.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/metadata_id.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/not_implemented.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/not_implemented.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/required_offset.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/required_offset.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/revocation.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/revocation.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/signature.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         elif self.signing_type == SigningType.ECDsa384:
             return "ECDsa384"
         else:
             raise Exception("Unknown signing type")
 
 
 class SignatureSection(MetadataSection):
-
     """
     The signature section contains the certificate hash and signing type used to sign the image.
     # byte[20] SigningCertThumbprint
     # uint32 signing type
     """
 
     def __init__(self, data=None):
```

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/temporary_image.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/temporary_image.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/metadata_sections/utils.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/metadata_sections/utils.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/app_development.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/app_development.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/der_encoded.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/der_encoded.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata/signing/signing_info.py` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata/signing/signing_info.py`

 * *Files identical despite different names*

### Comparing `azuresphere_imagemetadata-0.0.4/azuresphere_imagemetadata.egg-info/SOURCES.txt` & `azuresphere_imagemetadata-0.0.5/src/azuresphere_imagemetadata.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-LICENSE
-README.md
-setup.cfg
-setup.py
-azuresphere_imagemetadata/__init__.py
-azuresphere_imagemetadata/guid_utils.py
-azuresphere_imagemetadata/image.py
-azuresphere_imagemetadata/image_metadata.py
-azuresphere_imagemetadata.egg-info/PKG-INFO
-azuresphere_imagemetadata.egg-info/SOURCES.txt
-azuresphere_imagemetadata.egg-info/dependency_links.txt
-azuresphere_imagemetadata.egg-info/requires.txt
-azuresphere_imagemetadata.egg-info/top_level.txt
-azuresphere_imagemetadata/certificates/app_test_sign.pfx
-azuresphere_imagemetadata/certificates/tp_app_test_sign.cer
-azuresphere_imagemetadata/metadata_headers/__init__.py
-azuresphere_imagemetadata/metadata_headers/image_metadata.py
-azuresphere_imagemetadata/metadata_headers/image_metadata_section.py
-azuresphere_imagemetadata/metadata_sections/__init__.py
-azuresphere_imagemetadata/metadata_sections/abi.py
-azuresphere_imagemetadata/metadata_sections/compression.py
-azuresphere_imagemetadata/metadata_sections/debug.py
-azuresphere_imagemetadata/metadata_sections/identity.py
-azuresphere_imagemetadata/metadata_sections/image_policy.py
-azuresphere_imagemetadata/metadata_sections/metadata.py
-azuresphere_imagemetadata/metadata_sections/metadata_id.py
-azuresphere_imagemetadata/metadata_sections/not_implemented.py
-azuresphere_imagemetadata/metadata_sections/required_offset.py
-azuresphere_imagemetadata/metadata_sections/revocation.py
-azuresphere_imagemetadata/metadata_sections/signature.py
-azuresphere_imagemetadata/metadata_sections/temporary_image.py
-azuresphere_imagemetadata/metadata_sections/utils.py
-azuresphere_imagemetadata/metadata_sections/internal/__init__.py
-azuresphere_imagemetadata/metadata_sections/internal/capabilities.py
-azuresphere_imagemetadata/metadata_sections/internal/onebl.py
-azuresphere_imagemetadata/signing/__init__.py
-azuresphere_imagemetadata/signing/app_development.py
-azuresphere_imagemetadata/signing/der_encoded.py
-azuresphere_imagemetadata/signing/signing_info.py
+pyproject.toml
+src/azuresphere_imagemetadata/LICENSE
+src/azuresphere_imagemetadata/README.md
+src/azuresphere_imagemetadata/__init__.py
+src/azuresphere_imagemetadata/guid_utils.py
+src/azuresphere_imagemetadata/image.py
+src/azuresphere_imagemetadata/image_manifest.py
+src/azuresphere_imagemetadata/image_metadata.py
+src/azuresphere_imagemetadata.egg-info/PKG-INFO
+src/azuresphere_imagemetadata.egg-info/SOURCES.txt
+src/azuresphere_imagemetadata.egg-info/dependency_links.txt
+src/azuresphere_imagemetadata.egg-info/requires.txt
+src/azuresphere_imagemetadata.egg-info/top_level.txt
+src/azuresphere_imagemetadata/certificates/app_test_sign.pfx
+src/azuresphere_imagemetadata/certificates/tp_app_test_sign.cer
+src/azuresphere_imagemetadata/metadata_headers/__init__.py
+src/azuresphere_imagemetadata/metadata_headers/image_metadata.py
+src/azuresphere_imagemetadata/metadata_headers/image_metadata_section.py
+src/azuresphere_imagemetadata/metadata_sections/__init__.py
+src/azuresphere_imagemetadata/metadata_sections/abi.py
+src/azuresphere_imagemetadata/metadata_sections/compression.py
+src/azuresphere_imagemetadata/metadata_sections/debug.py
+src/azuresphere_imagemetadata/metadata_sections/identity.py
+src/azuresphere_imagemetadata/metadata_sections/image_policy.py
+src/azuresphere_imagemetadata/metadata_sections/metadata.py
+src/azuresphere_imagemetadata/metadata_sections/metadata_id.py
+src/azuresphere_imagemetadata/metadata_sections/not_implemented.py
+src/azuresphere_imagemetadata/metadata_sections/required_offset.py
+src/azuresphere_imagemetadata/metadata_sections/revocation.py
+src/azuresphere_imagemetadata/metadata_sections/signature.py
+src/azuresphere_imagemetadata/metadata_sections/temporary_image.py
+src/azuresphere_imagemetadata/metadata_sections/utils.py
+src/azuresphere_imagemetadata/metadata_sections/internal/__init__.py
+src/azuresphere_imagemetadata/metadata_sections/internal/capabilities.py
+src/azuresphere_imagemetadata/metadata_sections/internal/onebl.py
+src/azuresphere_imagemetadata/signing/__init__.py
+src/azuresphere_imagemetadata/signing/app_development.py
+src/azuresphere_imagemetadata/signing/der_encoded.py
+src/azuresphere_imagemetadata/signing/signing_info.py
+tests/test_certificate_files_match.py
+tests/test_dotnet_app.py
+tests/test_knownset_recovery_files.py
+tests/test_latest_recovery_files.py
+tests/test_package_version.py
+tests/test_parse_application.py
+tests/test_parse_capability.py
+tests/test_serialization.py
+tests/test_signing.py
```

