# Comparing `tmp/caluma_alexandria-4.0.2.tar.gz` & `tmp/caluma_alexandria-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-4.0.2.tar", max compression
+gzip compressed data, was "caluma_alexandria-4.1.0.tar", max compression
```

## Comparing `caluma_alexandria-4.0.2.tar` & `caluma_alexandria-4.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    24432 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/LICENSE
--rw-r--r--   0        0        0     8517 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/__init__.py
--rw-r--r--   0        0        0     2199 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/api.py
--rw-r--r--   0        0        0      127 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/apps.py
--rw-r--r--   0        0        0    13523 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/factories.py
--rw-r--r--   0        0        0     6937 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/filters.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/__init__.py
--rw-r--r--   0        0        0     2394 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/encrypt_files.py
--rw-r--r--   0        0        0      586 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/generate_missing_thumbnails.py
--rw-r--r--   0        0        0     1084 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/set_mime_type_and_size.py
--rw-r--r--   0        0        0    12553 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2840 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0      652 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0007_category_parent.py
--rw-r--r--   0        0        0      397 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0008_document_date.py
--rw-r--r--   0        0        0      466 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0009_file_checksum.py
--rw-r--r--   0        0        0     2973 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0010_mark.py
--rw-r--r--   0        0        0     1205 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0011_tag_uuid.py
--rw-r--r--   0        0        0     1655 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0012_tag_uuid_schema.py
--rw-r--r--   0        0        0     2086 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0013_file_content.py
--rw-r--r--   0        0        0      975 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0014_file_mime_type_size.py
--rw-r--r--   0        0        0     3304 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0015_fix_modified_by_description.py
--rw-r--r--   0        0        0      672 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0016_category_allowed_mime_types.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0    10789 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/models.py
--rw-r--r--   0        0        0     1823 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/presign_urls.py
--rw-r--r--   0        0        0    11412 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/serializers.py
--rw-r--r--   0        0        0      409 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/urls.py
--rw-r--r--   0        0        0     1655 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/validations.py
--rw-r--r--   0        0        0     9113 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/views.py
--rw-r--r--   0        0        0     1363 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/visibilities.py
--rw-r--r--   0        0        0     1703 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/dav.py
--rw-r--r--   0        0        0     4530 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/dav_provider.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     7449 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     5154 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/settings/django.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/backends/__init__.py
--rw-r--r--   0        0        0     1493 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/backends/s3.py
--rw-r--r--   0        0        0     2595 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/fields.py
--rw-r--r--   0        0        0      162 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/urls.py
--rw-r--r--   0        0        0     1048 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/wsgi.py
--rw-r--r--   0        0        0     3290 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/pyproject.toml
--rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 caluma_alexandria-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0    24786 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/LICENSE
+-rw-r--r--   0        0        0     8661 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/__init__.py
+-rw-r--r--   0        0        0     2199 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/api.py
+-rw-r--r--   0        0        0      127 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/apps.py
+-rw-r--r--   0        0        0    13523 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/factories.py
+-rw-r--r--   0        0        0     6937 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/filters.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2394 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/management/commands/encrypt_files.py
+-rw-r--r--   0        0        0      586 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/management/commands/generate_missing_thumbnails.py
+-rw-r--r--   0        0        0     1084 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/management/commands/set_mime_type_and_size.py
+-rw-r--r--   0        0        0    12553 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2840 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0      652 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0007_category_parent.py
+-rw-r--r--   0        0        0      397 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0008_document_date.py
+-rw-r--r--   0        0        0      466 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0009_file_checksum.py
+-rw-r--r--   0        0        0     2973 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0010_mark.py
+-rw-r--r--   0        0        0     1205 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0011_tag_uuid.py
+-rw-r--r--   0        0        0     1655 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0012_tag_uuid_schema.py
+-rw-r--r--   0        0        0     2086 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0013_file_content.py
+-rw-r--r--   0        0        0      975 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0014_file_mime_type_size.py
+-rw-r--r--   0        0        0     3304 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0015_fix_modified_by_description.py
+-rw-r--r--   0        0        0      672 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/0016_category_allowed_mime_types.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0    10789 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/models.py
+-rw-r--r--   0        0        0     1823 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/presign_urls.py
+-rw-r--r--   0        0        0    11075 2024-05-01 10:57:08.293382 caluma_alexandria-4.1.0/alexandria/core/serializers.py
+-rw-r--r--   0        0        0      409 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1655 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/core/validations.py
+-rw-r--r--   0        0        0     9051 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/core/views.py
+-rw-r--r--   0        0        0     1363 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0     1703 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/dav.py
+-rw-r--r--   0        0        0     4530 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/dav_provider.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4505 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     7617 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     5154 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/settings/django.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/storages/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/storages/backends/__init__.py
+-rw-r--r--   0        0        0     1493 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/storages/backends/s3.py
+-rw-r--r--   0        0        0     2595 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/storages/fields.py
+-rw-r--r--   0        0        0      162 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/urls.py
+-rw-r--r--   0        0        0     1048 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/alexandria/wsgi.py
+-rw-r--r--   0        0        0     3290 2024-05-01 10:57:08.297382 caluma_alexandria-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10411 1970-01-01 00:00:00.000000 caluma_alexandria-4.1.0/PKG-INFO
```

### Comparing `caluma_alexandria-4.0.2/CHANGELOG.md` & `caluma_alexandria-4.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# 4.1.0
+### Feature
+* Allow custom implementation of username and group getters ([`72bf2e4`](https://github.com/projectcaluma/alexandria/commit/72bf2e42862bb72fbd34cda059b8df0aa107ef7a))
+
+### Fix
+* **core:** Add get_user_and_group for serializer ([`b5bc3b6`](https://github.com/projectcaluma/alexandria/commit/b5bc3b67645bb2fe46dc547f94f8399ee5c2ecb7))
+
 # 4.0.2
 ### Fix
 * **mime:** Allow file extension checking if all fails ([`ddaa134`](https://github.com/projectcaluma/alexandria/commit/ddaa1344b2cde98a0c52f3311772d36da6e28c28))
 * Use atomic for document and file creation ([`1a630ad`](https://github.com/projectcaluma/alexandria/commit/1a630adb83a8351d1ed01b3070790e65b00cc43d))
 
 # 4.0.1
 ### Fix
```

### Comparing `caluma_alexandria-4.0.2/LICENSE` & `caluma_alexandria-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/README.md` & `caluma_alexandria-4.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 - Authentication configuration
   - `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
   - `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
   - `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
   - `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
   - `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
   - `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
+  - `ALEXANDRIA_GET_USER_AND_GROUP_FUNCTION`: Overwrite the import string if further configuration how user and group are determined is needed.
 - Authorization configurations
   - `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#visibilities) classes that define visibility for all models
   - `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#permissions) classes that define permissions for all models
 - Data validation configuration
   - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#data-validation) classes that define custom validations. A default base class is used for file validation. Extend `AlexandriaValidator` for own validations.
 - Thumbnail configuration (optional)
```

### Comparing `caluma_alexandria-4.0.2/alexandria/core/api.py` & `caluma_alexandria-4.1.0/alexandria/core/api.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/factories.py` & `caluma_alexandria-4.1.0/alexandria/core/factories.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/filters.py` & `caluma_alexandria-4.1.0/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/management/commands/encrypt_files.py` & `caluma_alexandria-4.1.0/alexandria/core/management/commands/encrypt_files.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/management/commands/generate_missing_thumbnails.py` & `caluma_alexandria-4.1.0/alexandria/core/management/commands/generate_missing_thumbnails.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/management/commands/set_mime_type_and_size.py` & `caluma_alexandria-4.1.0/alexandria/core/management/commands/set_mime_type_and_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0007_category_parent.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0007_category_parent.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0010_mark.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0010_mark.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0011_tag_uuid.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0011_tag_uuid.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0012_tag_uuid_schema.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0012_tag_uuid_schema.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0013_file_content.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0013_file_content.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0014_file_mime_type_size.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0014_file_mime_type_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0015_fix_modified_by_description.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0015_fix_modified_by_description.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/migrations/0016_category_allowed_mime_types.py` & `caluma_alexandria-4.1.0/alexandria/core/migrations/0016_category_allowed_mime_types.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/models.py` & `caluma_alexandria-4.1.0/alexandria/core/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/presign_urls.py` & `caluma_alexandria-4.1.0/alexandria/core/presign_urls.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/serializers.py` & `caluma_alexandria-4.1.0/alexandria/core/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 
 from django.conf import settings
 from django.db.transaction import atomic
 from django.template.defaultfilters import slugify
 from django.utils import translation
+from django.utils.module_loading import import_string
 from generic_permissions.validation import ValidatorMixin
 from generic_permissions.visibilities import (
     VisibilityResourceRelatedField,
     VisibilitySerializerMixin,
 )
 from rest_framework_json_api import serializers
 
@@ -20,39 +21,35 @@
 class BaseSerializer(
     ValidatorMixin, VisibilitySerializerMixin, serializers.ModelSerializer
 ):
     serializer_related_field = VisibilityResourceRelatedField
 
     created_at = serializers.DateTimeField(read_only=True)
 
+    def get_user_and_group(self):
+        return import_string(settings.ALEXANDRIA_GET_USER_AND_GROUP_FUNCTION)(
+            self.context.get("request")
+        )
+
     def is_valid(self, *args, **kwargs):
         # Prime data so the validators are called (and default values filled
         # if client didn't pass them.)
-        group = getattr(
-            self.context["request"].user,
-            settings.ALEXANDRIA_CREATED_BY_GROUP_PROPERTY,
-            None,
-        )
-        user = getattr(
-            self.context["request"].user,
-            settings.ALEXANDRIA_CREATED_BY_USER_PROPERTY,
-            None,
-        )
+        user, group = self.get_user_and_group()
         self.initial_data.setdefault("created_by_group", group)
         self.initial_data.setdefault("modified_by_group", group)
         self.initial_data.setdefault("created_by_user", user)
         self.initial_data.setdefault("modified_by_user", user)
         return super().is_valid(*args, **kwargs)
 
     def validate(self, *args, **kwargs):
         validated_data = super().validate(*args, **kwargs)
 
-        user = self.context["request"].user
-        username = getattr(user, settings.ALEXANDRIA_CREATED_BY_USER_PROPERTY)
-        validated_data["modified_by_user"] = username
+        user, group = self.get_user_and_group()
+        validated_data["modified_by_user"] = user
+        validated_data["modified_by_group"] = group
 
         return validated_data
 
     def validate_created_by_user(self, value):
         # Created by user can be set on creation, then must remain constant
         if self.instance:
             # can't change created_by_user on existing instances
@@ -186,25 +183,16 @@
         if (
             instance.variant != models.File.Variant.ORIGINAL
             or not settings.ALEXANDRIA_USE_MANABI
         ):
             return None
         request = self.context.get("request")
         host = request.get_host() if request else "localhost"
-        username = getattr(
-            getattr(request, "user", None),
-            settings.ALEXANDRIA_CREATED_BY_USER_PROPERTY,
-            None,
-        )
-        group = getattr(
-            getattr(request, "user", None),
-            settings.ALEXANDRIA_CREATED_BY_GROUP_PROPERTY,
-            None,
-        )
-        return instance.get_webdav_url(username, group, host)
+        user, group = self.get_user_and_group()
+        return instance.get_webdav_url(user, group, host)
 
     def validate(self, *args, **kwargs):
         """Validate the data.
 
         Validation can be extended by adding ValidatorClass to the
         `validator_classes` attribute of the FileViewSet.
         """
```

### Comparing `caluma_alexandria-4.0.2/alexandria/core/validations.py` & `caluma_alexandria-4.1.0/alexandria/core/validations.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/core/views.py` & `caluma_alexandria-4.1.0/alexandria/core/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from tempfile import NamedTemporaryFile
 
 import requests
 from django.conf import settings
 from django.core.exceptions import ValidationError as DjangoCoreValidationError
 from django.core.files.base import ContentFile
 from django.http import FileResponse
+from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
 from generic_permissions.permissions import AllowAny, PermissionViewMixin
 from generic_permissions.visibilities import VisibilityViewMixin
 from rest_framework.authentication import get_authorization_header
 from rest_framework.decorators import action, permission_classes
 from rest_framework.exceptions import (
     AuthenticationFailed,
@@ -126,24 +127,21 @@
         )
 
         if response.status_code == HTTP_401_UNAUTHORIZED:
             raise AuthenticationFailed(response.json().get("detail"))
 
         response.raise_for_status()
 
-        username = getattr(
-            request.user, settings.ALEXANDRIA_CREATED_BY_USER_PROPERTY, None
-        )
-        group = getattr(
-            request.user, settings.ALEXANDRIA_CREATED_BY_GROUP_PROPERTY, None
+        user, group = import_string(settings.ALEXANDRIA_GET_USER_AND_GROUP_FUNCTION)(
+            request
         )
 
         file_name = f"{splitext(file.name)[0]}.pdf"
         converted_document, __ = create_document_file(
-            user=username,
+            user=user,
             group=group,
             category=document.category,
             document_title={
                 k: f"{ splitext(v)[0]}.pdf" for k, v in document.title.items()
             },
             file_name=file_name,
             file_content=ContentFile(response.content, file_name),
```

### Comparing `caluma_alexandria-4.0.2/alexandria/core/visibilities.py` & `caluma_alexandria-4.1.0/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/dav.py` & `caluma_alexandria-4.1.0/alexandria/dav.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/dav_provider.py` & `caluma_alexandria-4.1.0/alexandria/dav_provider.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-4.1.0/alexandria/oidc_auth/authentication.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 from django.core.cache import cache
 from django.core.exceptions import ImproperlyConfigured, SuspiciousOperation
 from django.utils.encoding import force_bytes
 from django.utils.module_loading import import_string
 from mozilla_django_oidc.auth import OIDCAuthenticationBackend
 
 
+def get_user_and_group(request):
+    if request is None:
+        return None, None
+
+    user = getattr(request.user, settings.ALEXANDRIA_CREATED_BY_USER_PROPERTY, None)
+    group = getattr(request.user, settings.ALEXANDRIA_CREATED_BY_GROUP_PROPERTY, None)
+    return user, group
+
+
 class AlexandriaAuthenticationBackend(OIDCAuthenticationBackend):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.OIDC_USERNAME_CLAIM = self.get_settings("OIDC_USERNAME_CLAIM")
         self.OIDC_OP_INTROSPECT_ENDPOINT = self.get_settings(
             "OIDC_OP_INTROSPECT_ENDPOINT"
```

### Comparing `caluma_alexandria-4.0.2/alexandria/oidc_auth/models.py` & `caluma_alexandria-4.1.0/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/settings/alexandria.py` & `caluma_alexandria-4.1.0/alexandria/settings/alexandria.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 )
 ALEXANDRIA_CREATED_BY_USER_PROPERTY = env.str(
     "ALEXANDRIA_CREATED_BY_USER_PROPERTY", default="username"
 )
 ALEXANDRIA_CREATED_BY_GROUP_PROPERTY = env.str(
     "ALEXANDRIA_CREATED_BY_GROUP_PROPERTY", default="group"
 )
+ALEXANDRIA_GET_USER_AND_GROUP_FUNCTION = env.str(
+    "ALEXANDRIA_GET_USER_AND_GROUP_FUNCTION",
+    default="alexandria.oidc_auth.authentication.get_user_and_group",
+)
 
 
 # Extensions
 ALEXANDRIA_VISIBILITY_CLASSES = env.list(
     "ALEXANDRIA_VISIBILITY_CLASSES",
     default=default(["generic_permissions.visibilities.Any"], []),
 )
```

### Comparing `caluma_alexandria-4.0.2/alexandria/settings/django.py` & `caluma_alexandria-4.1.0/alexandria/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/storages/backends/s3.py` & `caluma_alexandria-4.1.0/alexandria/storages/backends/s3.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/storages/fields.py` & `caluma_alexandria-4.1.0/alexandria/storages/fields.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/alexandria/wsgi.py` & `caluma_alexandria-4.1.0/alexandria/wsgi.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.2/pyproject.toml` & `caluma_alexandria-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "4.0.2"
+version = "4.1.0"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `caluma_alexandria-4.0.2/PKG-INFO` & `caluma_alexandria-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma-alexandria
-Version: 4.0.2
+Version: 4.1.0
 Summary: Document management service
 Home-page: https://github.com/projectcaluma/alexandria
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -110,14 +110,15 @@
 - Authentication configuration
   - `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
   - `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
   - `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
   - `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
   - `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
   - `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
+  - `ALEXANDRIA_GET_USER_AND_GROUP_FUNCTION`: Overwrite the import string if further configuration how user and group are determined is needed.
 - Authorization configurations
   - `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#visibilities) classes that define visibility for all models
   - `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#permissions) classes that define permissions for all models
 - Data validation configuration
   - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#data-validation) classes that define custom validations. A default base class is used for file validation. Extend `AlexandriaValidator` for own validations.
 - Thumbnail configuration (optional)
```

