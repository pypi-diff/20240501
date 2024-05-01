# Comparing `tmp/apicurioregistrysdk-2.5.7.tar.gz` & `tmp/apicurioregistrysdk-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurioregistrysdk-2.5.7.tar", max compression
+gzip compressed data, was "apicurioregistrysdk-2.5.9.tar", max compression
```

## Comparing `apicurioregistrysdk-2.5.7.tar` & `apicurioregistrysdk-2.5.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0      368 2023-12-18 12:35:45.493611 apicurioregistrysdk-2.5.7/README.md
--rw-r--r--   0        0        0        0 2023-12-18 12:35:45.493611 apicurioregistrysdk-2.5.7/apicurioregistrysdk/__init__.py
--rw-r--r--   0        0        0     1695 2023-12-18 12:50:49.939451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/.kiota.log
--rw-r--r--   0        0        0     3671 2023-12-18 12:50:49.867451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/admin_request_builder.py
--rw-r--r--   0        0        0     3864 2023-12-18 12:50:49.867451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py
--rw-r--r--   0        0        0     1358 2023-12-18 12:50:49.867451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/config/config_request_builder.py
--rw-r--r--   0        0        0     9641 2023-12-18 12:50:49.867451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
--rw-r--r--   0        0        0     4751 2023-12-18 12:50:49.867451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py
--rw-r--r--   0        0        0     4785 2023-12-18 12:50:49.875450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/export/export_request_builder.py
--rw-r--r--   0        0        0     3721 2023-12-18 12:50:49.871451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/import_/import_request_builder.py
--rw-r--r--   0        0        0     8873 2023-12-18 12:50:49.871451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py
--rw-r--r--   0        0        0     4392 2023-12-18 12:50:49.875450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py
--rw-r--r--   0        0        0     9263 2023-12-18 12:50:49.871451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
--rw-r--r--   0        0        0     7313 2023-12-18 12:50:49.871451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py
--rw-r--r--   0        0        0     9597 2023-12-18 12:50:49.871451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py
--rw-r--r--   0        0        0     9505 2023-12-18 12:50:49.867451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/rules/rules_request_builder.py
--rw-r--r--   0        0        0     8890 2023-12-18 12:50:49.875450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/groups_request_builder.py
--rw-r--r--   0        0        0    19829 2023-12-18 12:50:49.875450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py
--rw-r--r--   0        0        0    12882 2023-12-18 12:50:49.887451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
--rw-r--r--   0        0        0     6682 2023-12-18 12:50:49.875450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
--rw-r--r--   0        0        0    10903 2023-12-18 12:50:49.883451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
--rw-r--r--   0        0        0    10760 2023-12-18 12:50:49.887451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
--rw-r--r--   0        0        0     4649 2023-12-18 12:50:49.883451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py
--rw-r--r--   0        0        0     5797 2023-12-18 12:50:49.883451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py
--rw-r--r--   0        0        0     8149 2023-12-18 12:50:49.879450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/comments_request_builder.py
--rw-r--r--   0        0        0     7588 2023-12-18 12:50:49.879450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/item/with_comment_item_request_builder.py
--rw-r--r--   0        0        0    10314 2023-12-18 12:50:49.879450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
--rw-r--r--   0        0        0     6142 2023-12-18 12:50:49.883451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4476 2023-12-18 12:50:49.879450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
--rw-r--r--   0        0        0    10843 2023-12-18 12:50:49.879450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
--rw-r--r--   0        0        0    10720 2023-12-18 12:50:49.883451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
--rw-r--r--   0        0        0    15263 2023-12-18 12:50:49.887451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
--rw-r--r--   0        0        0     6645 2023-12-18 12:50:49.887451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py
--rw-r--r--   0        0        0     1797 2023-12-18 12:50:49.827450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py
--rw-r--r--   0        0        0     3816 2023-12-18 12:50:49.827450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4539 2023-12-18 12:50:49.827450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
--rw-r--r--   0        0        0     1756 2023-12-18 12:50:49.827450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py
--rw-r--r--   0        0        0     3802 2023-12-18 12:50:49.823450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4531 2023-12-18 12:50:49.823450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py
--rw-r--r--   0        0        0     1740 2023-12-18 12:50:49.823450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py
--rw-r--r--   0        0        0     5052 2023-12-18 12:50:49.823450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py
--rw-r--r--   0        0        0     5631 2023-12-18 12:50:49.819450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py
--rw-r--r--   0        0        0     2116 2023-12-18 12:50:49.811450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/ids_request_builder.py
--rw-r--r--   0        0        0     1140 2023-12-18 12:50:49.931451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/kiota-lock.json
--rw-r--r--   0        0        0     2481 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_content.py
--rw-r--r--   0        0        0     5796 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_meta_data.py
--rw-r--r--   0        0        0     1951 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_owner.py
--rw-r--r--   0        0        0     2647 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_reference.py
--rw-r--r--   0        0        0     2613 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_search_results.py
--rw-r--r--   0        0        0      139 2023-12-18 12:50:49.851451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_state.py
--rw-r--r--   0        0        0     1897 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_type_info.py
--rw-r--r--   0        0        0     2540 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/comment.py
--rw-r--r--   0        0        0     2683 2023-12-18 12:50:49.859450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/configuration_property.py
--rw-r--r--   0        0        0     2539 2023-12-18 12:50:49.851451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/create_group_meta_data.py
--rw-r--r--   0        0        0     2171 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/download_ref.py
--rw-r--r--   0        0        0     2780 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/editable_meta_data.py
--rw-r--r--   0        0        0     2727 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/error.py
--rw-r--r--   0        0        0     3453 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/group_meta_data.py
--rw-r--r--   0        0        0     2550 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/group_search_results.py
--rw-r--r--   0        0        0     5640 2023-12-18 12:50:49.859450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/limits.py
--rw-r--r--   0        0        0     2141 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/log_configuration.py
--rw-r--r--   0        0        0      286 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/log_level.py
--rw-r--r--   0        0        0     1917 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/named_log_configuration.py
--rw-r--r--   0        0        0     1879 2023-12-18 12:50:49.851451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/new_comment.py
--rw-r--r--   0        0        0     1778 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/properties.py
--rw-r--r--   0        0        0     2568 2023-12-18 12:50:49.851451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/role_mapping.py
--rw-r--r--   0        0        0      130 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/role_type.py
--rw-r--r--   0        0        0     2191 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/rule.py
--rw-r--r--   0        0        0      144 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/rule_type.py
--rw-r--r--   0        0        0     2170 2023-12-18 12:50:49.851451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/rule_violation_error.py
--rw-r--r--   0        0        0     4430 2023-12-18 12:50:49.859450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/searched_artifact.py
--rw-r--r--   0        0        0     3129 2023-12-18 12:50:49.859450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/searched_group.py
--rw-r--r--   0        0        0     5047 2023-12-18 12:50:49.859450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/searched_version.py
--rw-r--r--   0        0        0     2528 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/system_info.py
--rw-r--r--   0        0        0     1947 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/update_configuration_property.py
--rw-r--r--   0        0        0     2025 2023-12-18 12:50:49.843450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/update_role.py
--rw-r--r--   0        0        0     2178 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/update_state.py
--rw-r--r--   0        0        0     2756 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/user_info.py
--rw-r--r--   0        0        0     4877 2023-12-18 12:50:49.855450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/version_meta_data.py
--rw-r--r--   0        0        0     2595 2023-12-18 12:50:49.847451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/version_search_results.py
--rw-r--r--   0        0        0     3788 2023-12-18 12:50:49.827450 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/registry_client.py
--rw-r--r--   0        0        0    11994 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py
--rw-r--r--   0        0        0     1342 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/search/search_request_builder.py
--rw-r--r--   0        0        0     3677 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/system/info/info_request_builder.py
--rw-r--r--   0        0        0     3652 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/system/limits/limits_request_builder.py
--rw-r--r--   0        0        0     1642 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/system/system_request_builder.py
--rw-r--r--   0        0        0     3527 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/users/me/me_request_builder.py
--rw-r--r--   0        0        0     1282 2023-12-18 12:50:49.863451 apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/users/users_request_builder.py
--rw-r--r--   0        0        0     2604 2023-12-18 12:35:45.493611 apicurioregistrysdk-2.5.7/kiota-gen.py
--rw-r--r--   0        0        0   220578 2023-12-18 12:50:48.267448 apicurioregistrysdk-2.5.7/openapi.json
--rw-r--r--   0        0        0     1303 2023-12-18 12:35:58.697638 apicurioregistrysdk-2.5.7/pyproject.toml
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 apicurioregistrysdk-2.5.7/PKG-INFO
+-rw-r--r--   0        0        0      368 2024-03-11 11:15:51.991149 apicurioregistrysdk-2.5.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 11:15:51.991149 apicurioregistrysdk-2.5.9/apicurioregistrysdk/__init__.py
+-rw-r--r--   0        0        0     1695 2024-03-11 11:23:03.341999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/.kiota.log
+-rw-r--r--   0        0        0     3671 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/admin_request_builder.py
+-rw-r--r--   0        0        0     3864 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py
+-rw-r--r--   0        0        0     1358 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/config/config_request_builder.py
+-rw-r--r--   0        0        0     9641 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
+-rw-r--r--   0        0        0     4751 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py
+-rw-r--r--   0        0        0     4785 2024-03-11 11:23:03.289999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/export/export_request_builder.py
+-rw-r--r--   0        0        0     3721 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/import_/import_request_builder.py
+-rw-r--r--   0        0        0     8873 2024-03-11 11:23:03.281999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py
+-rw-r--r--   0        0        0     4392 2024-03-11 11:23:03.285999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py
+-rw-r--r--   0        0        0     9263 2024-03-11 11:23:03.289999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
+-rw-r--r--   0        0        0     7313 2024-03-11 11:23:03.289999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py
+-rw-r--r--   0        0        0     9597 2024-03-11 11:23:03.281999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0     9505 2024-03-11 11:23:03.281999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     8890 2024-03-11 11:23:03.265999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/groups_request_builder.py
+-rw-r--r--   0        0        0    19829 2024-03-11 11:23:03.277999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0    12882 2024-03-11 11:23:03.269999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6682 2024-03-11 11:23:03.269999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
+-rw-r--r--   0        0        0    10903 2024-03-11 11:23:03.265999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0    10760 2024-03-11 11:23:03.269999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     4649 2024-03-11 11:23:03.269999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py
+-rw-r--r--   0        0        0     5797 2024-03-11 11:23:03.269999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py
+-rw-r--r--   0        0        0     8149 2024-03-11 11:23:03.273999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/comments_request_builder.py
+-rw-r--r--   0        0        0     7588 2024-03-11 11:23:03.277999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/item/with_comment_item_request_builder.py
+-rw-r--r--   0        0        0    10314 2024-03-11 11:23:03.277999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6142 2024-03-11 11:23:03.277999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4476 2024-03-11 11:23:03.277999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
+-rw-r--r--   0        0        0    10843 2024-03-11 11:23:03.273999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
+-rw-r--r--   0        0        0    10720 2024-03-11 11:23:03.273999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
+-rw-r--r--   0        0        0    15263 2024-03-11 11:23:03.273999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
+-rw-r--r--   0        0        0     6645 2024-03-11 11:23:03.265999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py
+-rw-r--r--   0        0        0     1797 2024-03-11 11:23:03.261999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py
+-rw-r--r--   0        0        0     3816 2024-03-11 11:23:03.261999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4539 2024-03-11 11:23:03.261999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
+-rw-r--r--   0        0        0     1756 2024-03-11 11:23:03.261999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py
+-rw-r--r--   0        0        0     3802 2024-03-11 11:23:03.257999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4531 2024-03-11 11:23:03.257999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py
+-rw-r--r--   0        0        0     1740 2024-03-11 11:23:03.261999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py
+-rw-r--r--   0        0        0     5052 2024-03-11 11:23:03.265999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     5631 2024-03-11 11:23:03.261999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py
+-rw-r--r--   0        0        0     2116 2024-03-11 11:23:03.265999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/ids_request_builder.py
+-rw-r--r--   0        0        0     1140 2024-03-11 11:23:03.329999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/kiota-lock.json
+-rw-r--r--   0        0        0     2481 2024-03-11 11:23:03.241999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_content.py
+-rw-r--r--   0        0        0     5796 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_meta_data.py
+-rw-r--r--   0        0        0     1951 2024-03-11 11:23:03.241999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_owner.py
+-rw-r--r--   0        0        0     2647 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_reference.py
+-rw-r--r--   0        0        0     2613 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_search_results.py
+-rw-r--r--   0        0        0      139 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_state.py
+-rw-r--r--   0        0        0     1897 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_type_info.py
+-rw-r--r--   0        0        0     2540 2024-03-11 11:23:03.241999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/comment.py
+-rw-r--r--   0        0        0     2683 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/configuration_property.py
+-rw-r--r--   0        0        0     2539 2024-03-11 11:23:03.225998 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/create_group_meta_data.py
+-rw-r--r--   0        0        0     2171 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/download_ref.py
+-rw-r--r--   0        0        0     2780 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/editable_meta_data.py
+-rw-r--r--   0        0        0     2727 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/error.py
+-rw-r--r--   0        0        0     3453 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/group_meta_data.py
+-rw-r--r--   0        0        0     2550 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/group_search_results.py
+-rw-r--r--   0        0        0     5640 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/limits.py
+-rw-r--r--   0        0        0     2141 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/log_configuration.py
+-rw-r--r--   0        0        0      286 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/log_level.py
+-rw-r--r--   0        0        0     1917 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/named_log_configuration.py
+-rw-r--r--   0        0        0     1879 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/new_comment.py
+-rw-r--r--   0        0        0     1778 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/properties.py
+-rw-r--r--   0        0        0     2568 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/role_mapping.py
+-rw-r--r--   0        0        0      130 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/role_type.py
+-rw-r--r--   0        0        0     2191 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/rule.py
+-rw-r--r--   0        0        0      144 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/rule_type.py
+-rw-r--r--   0        0        0     2170 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/rule_violation_error.py
+-rw-r--r--   0        0        0     4430 2024-03-11 11:23:03.225998 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/searched_artifact.py
+-rw-r--r--   0        0        0     3129 2024-03-11 11:23:03.245999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/searched_group.py
+-rw-r--r--   0        0        0     5047 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/searched_version.py
+-rw-r--r--   0        0        0     2528 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/system_info.py
+-rw-r--r--   0        0        0     1947 2024-03-11 11:23:03.229999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/update_configuration_property.py
+-rw-r--r--   0        0        0     2025 2024-03-11 11:23:03.241999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/update_role.py
+-rw-r--r--   0        0        0     2178 2024-03-11 11:23:03.233999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/update_state.py
+-rw-r--r--   0        0        0     2756 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/user_info.py
+-rw-r--r--   0        0        0     4877 2024-03-11 11:23:03.241999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/version_meta_data.py
+-rw-r--r--   0        0        0     2595 2024-03-11 11:23:03.237999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/version_search_results.py
+-rw-r--r--   0        0        0     3788 2024-03-11 11:23:03.257999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/registry_client.py
+-rw-r--r--   0        0        0    11994 2024-03-11 11:23:03.257999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0     1342 2024-03-11 11:23:03.249999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/search/search_request_builder.py
+-rw-r--r--   0        0        0     3677 2024-03-11 11:23:03.281999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/system/info/info_request_builder.py
+-rw-r--r--   0        0        0     3652 2024-03-11 11:23:03.281999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/system/limits/limits_request_builder.py
+-rw-r--r--   0        0        0     1642 2024-03-11 11:23:03.277999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/system/system_request_builder.py
+-rw-r--r--   0        0        0     3527 2024-03-11 11:23:03.289999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/users/me/me_request_builder.py
+-rw-r--r--   0        0        0     1282 2024-03-11 11:23:03.289999 apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/users/users_request_builder.py
+-rw-r--r--   0        0        0     2604 2024-03-11 11:15:51.991149 apicurioregistrysdk-2.5.9/kiota-gen.py
+-rw-r--r--   0        0        0   220578 2024-03-11 11:23:01.769989 apicurioregistrysdk-2.5.9/openapi.json
+-rw-r--r--   0        0        0     1303 2024-03-11 11:16:09.151265 apicurioregistrysdk-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 apicurioregistrysdk-2.5.9/PKG-INFO
```

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/.kiota.log` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/.kiota.log`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/admin_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/admin_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/config/config_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/config/config_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/export/export_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/export/export_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/import_/import_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/import_/import_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/admin/rules/rules_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/admin/rules/rules_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/groups_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/groups_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/comments_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/comments_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/item/with_comment_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/comments/item/with_comment_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/ids/ids_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/ids/ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/kiota-lock.json` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/kiota-lock.json`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_content.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_content.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_meta_data.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_owner.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_owner.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_reference.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_reference.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_search_results.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/artifact_type_info.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/artifact_type_info.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/comment.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/comment.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/configuration_property.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/configuration_property.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/create_group_meta_data.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/create_group_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/download_ref.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/download_ref.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/editable_meta_data.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/editable_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/error.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/error.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/group_meta_data.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/group_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/group_search_results.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/group_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/limits.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/limits.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/log_configuration.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/log_configuration.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/named_log_configuration.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/named_log_configuration.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/new_comment.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/new_comment.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/properties.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/properties.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/role_mapping.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/role_mapping.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/rule.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/rule.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/rule_violation_error.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/rule_violation_error.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/searched_artifact.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/searched_artifact.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/searched_group.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/searched_group.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/searched_version.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/searched_version.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/system_info.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/update_configuration_property.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/update_configuration_property.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/update_role.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/update_role.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/update_state.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/update_state.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/user_info.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/user_info.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/version_meta_data.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/version_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/models/version_search_results.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/models/version_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/registry_client.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/registry_client.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/search/search_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/search/search_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/system/info/info_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/system/info/info_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/system/limits/limits_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/system/limits/limits_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/system/system_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/system/system_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/users/me/me_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/users/me/me_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/apicurioregistrysdk/client/users/users_request_builder.py` & `apicurioregistrysdk-2.5.9/apicurioregistrysdk/client/users/users_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/kiota-gen.py` & `apicurioregistrysdk-2.5.9/kiota-gen.py`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/openapi.json` & `apicurioregistrysdk-2.5.9/openapi.json`

 * *Files identical despite different names*

### Comparing `apicurioregistrysdk-2.5.7/pyproject.toml` & `apicurioregistrysdk-2.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apicurioregistrysdk"
-version = "2.5.7"
+version = "2.5.9"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "apicurioregistrysdk"}]
 include = [
     { path = "openapi.json", format=["sdist", "wheel"] },
     { path = "apicurioregistrysdk/client/**/*", format=["sdist", "wheel"] },
```

### Comparing `apicurioregistrysdk-2.5.7/PKG-INFO` & `apicurioregistrysdk-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicurioregistrysdk
-Version: 2.5.7
+Version: 2.5.9
 Summary: 
 Home-page: https://github.com/apicurio/apicurio-registry
 License: Apache 2.0
 Keywords: apicurio,registry
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.9,<4.0
```

