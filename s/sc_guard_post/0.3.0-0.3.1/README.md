# Comparing `tmp/sc_guard_post-0.3.0.tar.gz` & `tmp/sc_guard_post-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_guard_post-0.3.0.tar", max compression
+gzip compressed data, was "sc_guard_post-0.3.1.tar", max compression
```

## Comparing `sc_guard_post-0.3.0.tar` & `sc_guard_post-0.3.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     4954 2023-11-26 03:08:58.254746 sc_guard_post-0.3.0/README.md
--rw-r--r--   0        0        0     6148 2023-11-26 02:47:09.591059 sc_guard_post-0.3.0/guard_post/.DS_Store
--rw-r--r--   0        0        0       27 2024-01-11 23:32:46.094897 sc_guard_post-0.3.0/guard_post/__init__.py
--rw-r--r--   0        0        0       47 2023-11-26 02:40:49.296967 sc_guard_post-0.3.0/guard_post/api/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.413098 sc_guard_post-0.3.0/guard_post/api/assigns/__init__.py
--rw-r--r--   0        0        0     4478 2023-11-26 03:03:10.653612 sc_guard_post-0.3.0/guard_post/api/assigns/assign_edge_api_assigns_add_post.py
--rw-r--r--   0        0        0     4356 2023-11-26 03:03:08.946288 sc_guard_post-0.3.0/guard_post/api/assigns/check_relationship_api_assigns_check_post.py
--rw-r--r--   0        0        0     4435 2023-11-26 03:03:07.304123 sc_guard_post-0.3.0/guard_post/api/assigns/expand_relationship_api_assigns_expand_post.py
--rw-r--r--   0        0        0     4455 2023-11-26 03:03:05.559557 sc_guard_post-0.3.0/guard_post/api/assigns/list_edges_api_assigns_list_post.py
--rw-r--r--   0        0        0     4361 2023-11-26 03:03:03.647340 sc_guard_post-0.3.0/guard_post/api/assigns/revoke_user_to_org_api_assigns_revoke_post.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.429233 sc_guard_post-0.3.0/guard_post/api/azure_ad/__init__.py
--rw-r--r--   0        0        0     3535 2024-01-26 00:57:16.444246 sc_guard_post-0.3.0/guard_post/api/azure_ad/get_user_api_active_dir_get_user_get.py
--rw-r--r--   0        0        0     2160 2023-11-26 03:02:55.954122 sc_guard_post-0.3.0/guard_post/api/azure_ad/signon_api_active_dir_signon_post.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.453209 sc_guard_post-0.3.0/guard_post/api/orgs/__init__.py
--rw-r--r--   0        0        0     4474 2023-11-26 03:02:52.462787 sc_guard_post-0.3.0/guard_post/api/orgs/delete_api_orgs_delete_post.py
--rw-r--r--   0        0        0     4693 2023-11-26 03:02:47.713971 sc_guard_post-0.3.0/guard_post/api/orgs/list_items_api_orgs_list_get.py
--rw-r--r--   0        0        0     4353 2023-11-26 03:02:50.185066 sc_guard_post-0.3.0/guard_post/api/orgs/sync_api_orgs_sync_post.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.333381 sc_guard_post-0.3.0/guard_post/api/ready/__init__.py
--rw-r--r--   0        0        0     4846 2023-11-26 03:05:55.218205 sc_guard_post-0.3.0/guard_post/api/ready/readiness_check_api_ready_get.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.409228 sc_guard_post-0.3.0/guard_post/api/relations/__init__.py
--rw-r--r--   0        0        0     2172 2023-11-26 03:02:39.133082 sc_guard_post-0.3.0/guard_post/api/relations/list_objs_api_relations_list_objs_post.py
--rw-r--r--   0        0        0     2242 2023-11-26 02:40:49.592831 sc_guard_post-0.3.0/guard_post/api/relations/traverse_api_relations_traverse_post.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.476708 sc_guard_post-0.3.0/guard_post/api/sites/__init__.py
--rw-r--r--   0        0        0     4486 2023-11-26 03:03:19.091570 sc_guard_post-0.3.0/guard_post/api/sites/delete_api_sites_delete_post.py
--rw-r--r--   0        0        0     4711 2023-11-26 03:03:17.410941 sc_guard_post-0.3.0/guard_post/api/sites/list_sites_api_sites_list_get.py
--rw-r--r--   0        0        0     4365 2023-11-26 03:03:15.598852 sc_guard_post-0.3.0/guard_post/api/sites/sync_api_sites_sync_post.py
--rw-r--r--   0        0        0        0 2023-11-26 02:40:49.434455 sc_guard_post-0.3.0/guard_post/api/users/__init__.py
--rw-r--r--   0        0        0     4486 2023-11-26 03:03:25.062995 sc_guard_post-0.3.0/guard_post/api/users/delete_api_users_delete_post.py
--rw-r--r--   0        0        0     4707 2023-11-26 03:03:23.652085 sc_guard_post-0.3.0/guard_post/api/users/list_items_api_users_list_get.py
--rw-r--r--   0        0        0     4637 2023-11-26 03:03:22.148339 sc_guard_post-0.3.0/guard_post/api/users/sync_api_users_sync_post.py
--rw-r--r--   0        0        0    12209 2023-11-26 03:05:33.255683 sc_guard_post-0.3.0/guard_post/client.py
--rw-r--r--   0        0        0    16865 2024-04-30 21:55:21.449643 sc_guard_post-0.3.0/guard_post/core.py
--rw-r--r--   0        0        0      470 2023-11-26 03:05:30.702423 sc_guard_post-0.3.0/guard_post/errors.py
--rw-r--r--   0        0        0       90 2023-11-30 19:08:01.874605 sc_guard_post-0.3.0/guard_post/imports.py
--rw-r--r--   0        0        0        0 2024-04-01 19:08:14.074472 sc_guard_post-0.3.0/guard_post/migrate/enums.py
--rw-r--r--   0        0        0      483 2024-04-01 19:14:05.042732 sc_guard_post-0.3.0/guard_post/migrate/models.py
--rw-r--r--   0        0        0     3188 2023-11-26 02:40:49.280097 sc_guard_post-0.3.0/guard_post/models/__init__.py
--rw-r--r--   0        0        0    35365 2024-01-26 00:46:46.770822 sc_guard_post-0.3.0/guard_post/models/azure_user.py
--rw-r--r--   0        0        0      158 2023-11-26 03:03:28.990086 sc_guard_post-0.3.0/guard_post/models/azure_user_acr_type_0.py
--rw-r--r--   0        0        0      181 2023-11-26 02:40:49.573939 sc_guard_post-0.3.0/guard_post/models/azure_user_appidacr_type_0.py
--rw-r--r--   0        0        0      179 2023-11-26 02:40:49.581752 sc_guard_post-0.3.0/guard_post/models/azure_user_azpacr_type_0.py
--rw-r--r--   0        0        0     1256 2023-11-26 03:03:32.307887 sc_guard_post-0.3.0/guard_post/models/azure_user_claims.py
--rw-r--r--   0        0        0      157 2023-11-26 03:03:35.071810 sc_guard_post-0.3.0/guard_post/models/azure_user_ver.py
--rw-r--r--   0        0        0     3900 2023-11-26 03:03:47.031527 sc_guard_post-0.3.0/guard_post/models/create_org.py
--rw-r--r--   0        0        0     1253 2023-11-26 03:03:42.747569 sc_guard_post-0.3.0/guard_post/models/create_org_attributes.py
--rw-r--r--   0        0        0     1249 2023-11-26 03:03:45.030569 sc_guard_post-0.3.0/guard_post/models/create_org_key_type_0.py
--rw-r--r--   0        0        0     4097 2023-11-26 03:03:53.904982 sc_guard_post-0.3.0/guard_post/models/create_site.py
--rw-r--r--   0        0        0     1258 2023-11-26 03:03:50.094291 sc_guard_post-0.3.0/guard_post/models/create_site_attributes.py
--rw-r--r--   0        0        0     1254 2023-11-26 03:03:52.293091 sc_guard_post-0.3.0/guard_post/models/create_site_key_type_0.py
--rw-r--r--   0        0        0     3576 2023-11-26 03:03:57.851458 sc_guard_post-0.3.0/guard_post/models/create_user.py
--rw-r--r--   0        0        0     1258 2023-11-26 03:03:55.366133 sc_guard_post-0.3.0/guard_post/models/create_user_attributes.py
--rw-r--r--   0        0        0     1254 2023-11-26 03:03:56.568227 sc_guard_post-0.3.0/guard_post/models/create_user_key_type_0.py
--rw-r--r--   0        0        0     2260 2023-11-26 03:04:00.187815 sc_guard_post-0.3.0/guard_post/models/delete_org.py
--rw-r--r--   0        0        0     1249 2023-11-26 03:03:59.197872 sc_guard_post-0.3.0/guard_post/models/delete_org_key_type_0.py
--rw-r--r--   0        0        0     2277 2023-11-26 03:04:05.289214 sc_guard_post-0.3.0/guard_post/models/delete_site.py
--rw-r--r--   0        0        0     1254 2023-11-26 03:04:01.320262 sc_guard_post-0.3.0/guard_post/models/delete_site_key_type_0.py
--rw-r--r--   0        0        0     2277 2023-11-26 03:04:09.015013 sc_guard_post-0.3.0/guard_post/models/delete_user.py
--rw-r--r--   0        0        0     1254 2023-11-26 03:04:07.143750 sc_guard_post-0.3.0/guard_post/models/delete_user_key_type_0.py
--rw-r--r--   0        0        0     1703 2023-11-26 03:04:21.932423 sc_guard_post-0.3.0/guard_post/models/edge.py
--rw-r--r--   0        0        0     2494 2023-11-26 03:04:10.865403 sc_guard_post-0.3.0/guard_post/models/edge_input.py
--rw-r--r--   0        0        0     3236 2023-11-26 03:04:16.017815 sc_guard_post-0.3.0/guard_post/models/edge_keys.py
--rw-r--r--   0        0        0     1244 2023-11-26 03:04:12.887056 sc_guard_post-0.3.0/guard_post/models/edge_keys_end_type_0.py
--rw-r--r--   0        0        0     1254 2023-11-26 03:04:14.542981 sc_guard_post-0.3.0/guard_post/models/edge_keys_start_type_0.py
--rw-r--r--   0        0        0     2401 2023-11-26 03:04:19.134830 sc_guard_post-0.3.0/guard_post/models/edge_userset.py
--rw-r--r--   0        0        0     3608 2023-11-26 03:04:25.626690 sc_guard_post-0.3.0/guard_post/models/error_model.py
--rw-r--r--   0        0        0     1297 2023-11-26 03:04:23.383087 sc_guard_post-0.3.0/guard_post/models/error_model_details_type_0_item.py
--rw-r--r--   0        0        0     2382 2023-11-26 03:04:27.513273 sc_guard_post-0.3.0/guard_post/models/error_response.py
--rw-r--r--   0        0        0     2508 2023-11-26 03:04:30.526424 sc_guard_post-0.3.0/guard_post/models/expand_input.py
--rw-r--r--   0        0        0     1259 2023-11-26 03:04:28.889585 sc_guard_post-0.3.0/guard_post/models/expand_input_key_type_0.py
--rw-r--r--   0        0        0     2194 2023-11-26 03:04:31.912649 sc_guard_post-0.3.0/guard_post/models/http_validation_error.py
--rw-r--r--   0        0        0     2154 2023-12-01 19:24:29.880001 sc_guard_post-0.3.0/guard_post/models/list_objects_input_key.py
--rw-r--r--   0        0        0     1274 2023-11-26 03:04:33.184989 sc_guard_post-0.3.0/guard_post/models/list_objects_input_key_key.py
--rw-r--r--   0        0        0     4968 2023-11-26 03:04:37.451132 sc_guard_post-0.3.0/guard_post/models/org.py
--rw-r--r--   0        0        0     1220 2023-11-26 03:04:35.217225 sc_guard_post-0.3.0/guard_post/models/org_attributes.py
--rw-r--r--   0        0        0     1216 2023-11-26 03:04:36.431451 sc_guard_post-0.3.0/guard_post/models/org_key_type_0.py
--rw-r--r--   0        0        0     2106 2024-04-30 21:43:44.048401 sc_guard_post-0.3.0/guard_post/models/pydantic_models/__init__.py
--rw-r--r--   0        0        0     1911 2023-11-26 03:04:39.778322 sc_guard_post-0.3.0/guard_post/models/ready_response.py
--rw-r--r--   0        0        0     5165 2023-11-26 03:04:43.462767 sc_guard_post-0.3.0/guard_post/models/site.py
--rw-r--r--   0        0        0     1225 2023-11-26 03:04:40.952670 sc_guard_post-0.3.0/guard_post/models/site_attributes.py
--rw-r--r--   0        0        0     1221 2023-11-26 03:04:42.168124 sc_guard_post-0.3.0/guard_post/models/site_key_type_0.py
--rw-r--r--   0        0        0     2806 2023-11-26 02:40:49.578194 sc_guard_post-0.3.0/guard_post/models/status.py
--rw-r--r--   0        0        0     5058 2023-11-26 03:04:49.057320 sc_guard_post-0.3.0/guard_post/models/user.py
--rw-r--r--   0        0        0     1225 2023-11-26 03:04:44.619590 sc_guard_post-0.3.0/guard_post/models/user_attributes.py
--rw-r--r--   0        0        0     1221 2023-11-26 03:04:45.599589 sc_guard_post-0.3.0/guard_post/models/user_key_type_0.py
--rw-r--r--   0        0        0     2154 2023-11-26 03:04:50.281630 sc_guard_post-0.3.0/guard_post/models/validation_error.py
--rw-r--r--   0        0        0       25 2023-11-26 02:40:38.111601 sc_guard_post-0.3.0/guard_post/py.typed
--rw-r--r--   0        0        0      163 2024-04-30 21:12:45.877322 sc_guard_post-0.3.0/guard_post/references.py
--rw-r--r--   0        0        0      968 2023-11-26 03:05:28.161323 sc_guard_post-0.3.0/guard_post/types.py
--rw-r--r--   0        0        0      639 2024-04-30 21:56:12.871114 sc_guard_post-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5770 1970-01-01 00:00:00.000000 sc_guard_post-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4954 2023-11-26 03:08:58.254746 sc_guard_post-0.3.1/README.md
+-rw-r--r--   0        0        0     6148 2023-11-26 02:47:09.591059 sc_guard_post-0.3.1/guard_post/.DS_Store
+-rw-r--r--   0        0        0       27 2024-01-11 23:32:46.094897 sc_guard_post-0.3.1/guard_post/__init__.py
+-rw-r--r--   0        0        0       47 2023-11-26 02:40:49.296967 sc_guard_post-0.3.1/guard_post/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.413098 sc_guard_post-0.3.1/guard_post/api/assigns/__init__.py
+-rw-r--r--   0        0        0     4478 2023-11-26 03:03:10.653612 sc_guard_post-0.3.1/guard_post/api/assigns/assign_edge_api_assigns_add_post.py
+-rw-r--r--   0        0        0     4356 2023-11-26 03:03:08.946288 sc_guard_post-0.3.1/guard_post/api/assigns/check_relationship_api_assigns_check_post.py
+-rw-r--r--   0        0        0     4435 2023-11-26 03:03:07.304123 sc_guard_post-0.3.1/guard_post/api/assigns/expand_relationship_api_assigns_expand_post.py
+-rw-r--r--   0        0        0     4455 2023-11-26 03:03:05.559557 sc_guard_post-0.3.1/guard_post/api/assigns/list_edges_api_assigns_list_post.py
+-rw-r--r--   0        0        0     4361 2023-11-26 03:03:03.647340 sc_guard_post-0.3.1/guard_post/api/assigns/revoke_user_to_org_api_assigns_revoke_post.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.429233 sc_guard_post-0.3.1/guard_post/api/azure_ad/__init__.py
+-rw-r--r--   0        0        0     3535 2024-01-26 00:57:16.444246 sc_guard_post-0.3.1/guard_post/api/azure_ad/get_user_api_active_dir_get_user_get.py
+-rw-r--r--   0        0        0     2160 2023-11-26 03:02:55.954122 sc_guard_post-0.3.1/guard_post/api/azure_ad/signon_api_active_dir_signon_post.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.453209 sc_guard_post-0.3.1/guard_post/api/orgs/__init__.py
+-rw-r--r--   0        0        0     4474 2023-11-26 03:02:52.462787 sc_guard_post-0.3.1/guard_post/api/orgs/delete_api_orgs_delete_post.py
+-rw-r--r--   0        0        0     4693 2023-11-26 03:02:47.713971 sc_guard_post-0.3.1/guard_post/api/orgs/list_items_api_orgs_list_get.py
+-rw-r--r--   0        0        0     4353 2023-11-26 03:02:50.185066 sc_guard_post-0.3.1/guard_post/api/orgs/sync_api_orgs_sync_post.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.333381 sc_guard_post-0.3.1/guard_post/api/ready/__init__.py
+-rw-r--r--   0        0        0     4846 2023-11-26 03:05:55.218205 sc_guard_post-0.3.1/guard_post/api/ready/readiness_check_api_ready_get.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.409228 sc_guard_post-0.3.1/guard_post/api/relations/__init__.py
+-rw-r--r--   0        0        0     2172 2023-11-26 03:02:39.133082 sc_guard_post-0.3.1/guard_post/api/relations/list_objs_api_relations_list_objs_post.py
+-rw-r--r--   0        0        0     2242 2023-11-26 02:40:49.592831 sc_guard_post-0.3.1/guard_post/api/relations/traverse_api_relations_traverse_post.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.476708 sc_guard_post-0.3.1/guard_post/api/sites/__init__.py
+-rw-r--r--   0        0        0     4486 2023-11-26 03:03:19.091570 sc_guard_post-0.3.1/guard_post/api/sites/delete_api_sites_delete_post.py
+-rw-r--r--   0        0        0     4711 2023-11-26 03:03:17.410941 sc_guard_post-0.3.1/guard_post/api/sites/list_sites_api_sites_list_get.py
+-rw-r--r--   0        0        0     4365 2023-11-26 03:03:15.598852 sc_guard_post-0.3.1/guard_post/api/sites/sync_api_sites_sync_post.py
+-rw-r--r--   0        0        0        0 2023-11-26 02:40:49.434455 sc_guard_post-0.3.1/guard_post/api/users/__init__.py
+-rw-r--r--   0        0        0     4486 2023-11-26 03:03:25.062995 sc_guard_post-0.3.1/guard_post/api/users/delete_api_users_delete_post.py
+-rw-r--r--   0        0        0     4707 2023-11-26 03:03:23.652085 sc_guard_post-0.3.1/guard_post/api/users/list_items_api_users_list_get.py
+-rw-r--r--   0        0        0     4637 2023-11-26 03:03:22.148339 sc_guard_post-0.3.1/guard_post/api/users/sync_api_users_sync_post.py
+-rw-r--r--   0        0        0    12209 2023-11-26 03:05:33.255683 sc_guard_post-0.3.1/guard_post/client.py
+-rw-r--r--   0        0        0    16865 2024-04-30 21:55:21.449643 sc_guard_post-0.3.1/guard_post/core.py
+-rw-r--r--   0        0        0      470 2023-11-26 03:05:30.702423 sc_guard_post-0.3.1/guard_post/errors.py
+-rw-r--r--   0        0        0       90 2023-11-30 19:08:01.874605 sc_guard_post-0.3.1/guard_post/imports.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:08:14.074472 sc_guard_post-0.3.1/guard_post/migrate/enums.py
+-rw-r--r--   0        0        0      483 2024-04-01 19:14:05.042732 sc_guard_post-0.3.1/guard_post/migrate/models.py
+-rw-r--r--   0        0        0     3188 2023-11-26 02:40:49.280097 sc_guard_post-0.3.1/guard_post/models/__init__.py
+-rw-r--r--   0        0        0    35365 2024-01-26 00:46:46.770822 sc_guard_post-0.3.1/guard_post/models/azure_user.py
+-rw-r--r--   0        0        0      158 2023-11-26 03:03:28.990086 sc_guard_post-0.3.1/guard_post/models/azure_user_acr_type_0.py
+-rw-r--r--   0        0        0      181 2023-11-26 02:40:49.573939 sc_guard_post-0.3.1/guard_post/models/azure_user_appidacr_type_0.py
+-rw-r--r--   0        0        0      179 2023-11-26 02:40:49.581752 sc_guard_post-0.3.1/guard_post/models/azure_user_azpacr_type_0.py
+-rw-r--r--   0        0        0     1256 2023-11-26 03:03:32.307887 sc_guard_post-0.3.1/guard_post/models/azure_user_claims.py
+-rw-r--r--   0        0        0      157 2023-11-26 03:03:35.071810 sc_guard_post-0.3.1/guard_post/models/azure_user_ver.py
+-rw-r--r--   0        0        0     3900 2023-11-26 03:03:47.031527 sc_guard_post-0.3.1/guard_post/models/create_org.py
+-rw-r--r--   0        0        0     1253 2023-11-26 03:03:42.747569 sc_guard_post-0.3.1/guard_post/models/create_org_attributes.py
+-rw-r--r--   0        0        0     1249 2023-11-26 03:03:45.030569 sc_guard_post-0.3.1/guard_post/models/create_org_key_type_0.py
+-rw-r--r--   0        0        0     4097 2023-11-26 03:03:53.904982 sc_guard_post-0.3.1/guard_post/models/create_site.py
+-rw-r--r--   0        0        0     1258 2023-11-26 03:03:50.094291 sc_guard_post-0.3.1/guard_post/models/create_site_attributes.py
+-rw-r--r--   0        0        0     1254 2023-11-26 03:03:52.293091 sc_guard_post-0.3.1/guard_post/models/create_site_key_type_0.py
+-rw-r--r--   0        0        0     3576 2023-11-26 03:03:57.851458 sc_guard_post-0.3.1/guard_post/models/create_user.py
+-rw-r--r--   0        0        0     1258 2023-11-26 03:03:55.366133 sc_guard_post-0.3.1/guard_post/models/create_user_attributes.py
+-rw-r--r--   0        0        0     1254 2023-11-26 03:03:56.568227 sc_guard_post-0.3.1/guard_post/models/create_user_key_type_0.py
+-rw-r--r--   0        0        0     2260 2023-11-26 03:04:00.187815 sc_guard_post-0.3.1/guard_post/models/delete_org.py
+-rw-r--r--   0        0        0     1249 2023-11-26 03:03:59.197872 sc_guard_post-0.3.1/guard_post/models/delete_org_key_type_0.py
+-rw-r--r--   0        0        0     2277 2023-11-26 03:04:05.289214 sc_guard_post-0.3.1/guard_post/models/delete_site.py
+-rw-r--r--   0        0        0     1254 2023-11-26 03:04:01.320262 sc_guard_post-0.3.1/guard_post/models/delete_site_key_type_0.py
+-rw-r--r--   0        0        0     2277 2023-11-26 03:04:09.015013 sc_guard_post-0.3.1/guard_post/models/delete_user.py
+-rw-r--r--   0        0        0     1254 2023-11-26 03:04:07.143750 sc_guard_post-0.3.1/guard_post/models/delete_user_key_type_0.py
+-rw-r--r--   0        0        0     1703 2023-11-26 03:04:21.932423 sc_guard_post-0.3.1/guard_post/models/edge.py
+-rw-r--r--   0        0        0     2494 2023-11-26 03:04:10.865403 sc_guard_post-0.3.1/guard_post/models/edge_input.py
+-rw-r--r--   0        0        0     3236 2023-11-26 03:04:16.017815 sc_guard_post-0.3.1/guard_post/models/edge_keys.py
+-rw-r--r--   0        0        0     1244 2023-11-26 03:04:12.887056 sc_guard_post-0.3.1/guard_post/models/edge_keys_end_type_0.py
+-rw-r--r--   0        0        0     1254 2023-11-26 03:04:14.542981 sc_guard_post-0.3.1/guard_post/models/edge_keys_start_type_0.py
+-rw-r--r--   0        0        0     2401 2023-11-26 03:04:19.134830 sc_guard_post-0.3.1/guard_post/models/edge_userset.py
+-rw-r--r--   0        0        0     3608 2023-11-26 03:04:25.626690 sc_guard_post-0.3.1/guard_post/models/error_model.py
+-rw-r--r--   0        0        0     1297 2023-11-26 03:04:23.383087 sc_guard_post-0.3.1/guard_post/models/error_model_details_type_0_item.py
+-rw-r--r--   0        0        0     2382 2023-11-26 03:04:27.513273 sc_guard_post-0.3.1/guard_post/models/error_response.py
+-rw-r--r--   0        0        0     2508 2023-11-26 03:04:30.526424 sc_guard_post-0.3.1/guard_post/models/expand_input.py
+-rw-r--r--   0        0        0     1259 2023-11-26 03:04:28.889585 sc_guard_post-0.3.1/guard_post/models/expand_input_key_type_0.py
+-rw-r--r--   0        0        0     2194 2023-11-26 03:04:31.912649 sc_guard_post-0.3.1/guard_post/models/http_validation_error.py
+-rw-r--r--   0        0        0     2154 2023-12-01 19:24:29.880001 sc_guard_post-0.3.1/guard_post/models/list_objects_input_key.py
+-rw-r--r--   0        0        0     1274 2023-11-26 03:04:33.184989 sc_guard_post-0.3.1/guard_post/models/list_objects_input_key_key.py
+-rw-r--r--   0        0        0     4968 2023-11-26 03:04:37.451132 sc_guard_post-0.3.1/guard_post/models/org.py
+-rw-r--r--   0        0        0     1220 2023-11-26 03:04:35.217225 sc_guard_post-0.3.1/guard_post/models/org_attributes.py
+-rw-r--r--   0        0        0     1216 2023-11-26 03:04:36.431451 sc_guard_post-0.3.1/guard_post/models/org_key_type_0.py
+-rw-r--r--   0        0        0     2106 2024-04-30 21:43:44.048401 sc_guard_post-0.3.1/guard_post/models/pydantic_models/__init__.py
+-rw-r--r--   0        0        0     1911 2023-11-26 03:04:39.778322 sc_guard_post-0.3.1/guard_post/models/ready_response.py
+-rw-r--r--   0        0        0     5165 2023-11-26 03:04:43.462767 sc_guard_post-0.3.1/guard_post/models/site.py
+-rw-r--r--   0        0        0     1225 2023-11-26 03:04:40.952670 sc_guard_post-0.3.1/guard_post/models/site_attributes.py
+-rw-r--r--   0        0        0     1221 2023-11-26 03:04:42.168124 sc_guard_post-0.3.1/guard_post/models/site_key_type_0.py
+-rw-r--r--   0        0        0     2806 2023-11-26 02:40:49.578194 sc_guard_post-0.3.1/guard_post/models/status.py
+-rw-r--r--   0        0        0     5058 2023-11-26 03:04:49.057320 sc_guard_post-0.3.1/guard_post/models/user.py
+-rw-r--r--   0        0        0     1225 2023-11-26 03:04:44.619590 sc_guard_post-0.3.1/guard_post/models/user_attributes.py
+-rw-r--r--   0        0        0     1221 2023-11-26 03:04:45.599589 sc_guard_post-0.3.1/guard_post/models/user_key_type_0.py
+-rw-r--r--   0        0        0     2154 2023-11-26 03:04:50.281630 sc_guard_post-0.3.1/guard_post/models/validation_error.py
+-rw-r--r--   0        0        0       25 2023-11-26 02:40:38.111601 sc_guard_post-0.3.1/guard_post/py.typed
+-rw-r--r--   0        0        0      163 2024-04-30 21:12:45.877322 sc_guard_post-0.3.1/guard_post/references.py
+-rw-r--r--   0        0        0      968 2023-11-26 03:05:28.161323 sc_guard_post-0.3.1/guard_post/types.py
+-rw-r--r--   0        0        0      616 2024-04-30 22:32:01.527896 sc_guard_post-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 sc_guard_post-0.3.1/PKG-INFO
```

### Comparing `sc_guard_post-0.3.0/README.md` & `sc_guard_post-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/.DS_Store` & `sc_guard_post-0.3.1/guard_post/.DS_Store`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/assigns/assign_edge_api_assigns_add_post.py` & `sc_guard_post-0.3.1/guard_post/api/assigns/assign_edge_api_assigns_add_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/assigns/check_relationship_api_assigns_check_post.py` & `sc_guard_post-0.3.1/guard_post/api/assigns/check_relationship_api_assigns_check_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/assigns/expand_relationship_api_assigns_expand_post.py` & `sc_guard_post-0.3.1/guard_post/api/assigns/expand_relationship_api_assigns_expand_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/assigns/list_edges_api_assigns_list_post.py` & `sc_guard_post-0.3.1/guard_post/api/assigns/list_edges_api_assigns_list_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/assigns/revoke_user_to_org_api_assigns_revoke_post.py` & `sc_guard_post-0.3.1/guard_post/api/assigns/revoke_user_to_org_api_assigns_revoke_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/azure_ad/get_user_api_active_dir_get_user_get.py` & `sc_guard_post-0.3.1/guard_post/api/azure_ad/get_user_api_active_dir_get_user_get.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/azure_ad/signon_api_active_dir_signon_post.py` & `sc_guard_post-0.3.1/guard_post/api/azure_ad/signon_api_active_dir_signon_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/orgs/delete_api_orgs_delete_post.py` & `sc_guard_post-0.3.1/guard_post/api/orgs/delete_api_orgs_delete_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/orgs/list_items_api_orgs_list_get.py` & `sc_guard_post-0.3.1/guard_post/api/orgs/list_items_api_orgs_list_get.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/orgs/sync_api_orgs_sync_post.py` & `sc_guard_post-0.3.1/guard_post/api/orgs/sync_api_orgs_sync_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/ready/readiness_check_api_ready_get.py` & `sc_guard_post-0.3.1/guard_post/api/ready/readiness_check_api_ready_get.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/relations/list_objs_api_relations_list_objs_post.py` & `sc_guard_post-0.3.1/guard_post/api/relations/list_objs_api_relations_list_objs_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/relations/traverse_api_relations_traverse_post.py` & `sc_guard_post-0.3.1/guard_post/api/relations/traverse_api_relations_traverse_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/sites/delete_api_sites_delete_post.py` & `sc_guard_post-0.3.1/guard_post/api/sites/delete_api_sites_delete_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/sites/list_sites_api_sites_list_get.py` & `sc_guard_post-0.3.1/guard_post/api/sites/list_sites_api_sites_list_get.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/sites/sync_api_sites_sync_post.py` & `sc_guard_post-0.3.1/guard_post/api/sites/sync_api_sites_sync_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/users/delete_api_users_delete_post.py` & `sc_guard_post-0.3.1/guard_post/api/users/delete_api_users_delete_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/users/list_items_api_users_list_get.py` & `sc_guard_post-0.3.1/guard_post/api/users/list_items_api_users_list_get.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/api/users/sync_api_users_sync_post.py` & `sc_guard_post-0.3.1/guard_post/api/users/sync_api_users_sync_post.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/client.py` & `sc_guard_post-0.3.1/guard_post/client.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/core.py` & `sc_guard_post-0.3.1/guard_post/core.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/__init__.py` & `sc_guard_post-0.3.1/guard_post/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/azure_user.py` & `sc_guard_post-0.3.1/guard_post/models/azure_user.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/azure_user_claims.py` & `sc_guard_post-0.3.1/guard_post/models/azure_user_claims.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_org.py` & `sc_guard_post-0.3.1/guard_post/models/create_org.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_org_attributes.py` & `sc_guard_post-0.3.1/guard_post/models/create_org_attributes.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_org_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/create_org_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_site.py` & `sc_guard_post-0.3.1/guard_post/models/create_site.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_site_attributes.py` & `sc_guard_post-0.3.1/guard_post/models/create_site_attributes.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_site_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/create_site_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_user.py` & `sc_guard_post-0.3.1/guard_post/models/create_user.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_user_attributes.py` & `sc_guard_post-0.3.1/guard_post/models/create_user_attributes.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/create_user_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/create_user_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/delete_org.py` & `sc_guard_post-0.3.1/guard_post/models/delete_org.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/delete_org_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/delete_org_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/delete_site.py` & `sc_guard_post-0.3.1/guard_post/models/delete_site.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/delete_site_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/delete_site_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/delete_user.py` & `sc_guard_post-0.3.1/guard_post/models/delete_user.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/delete_user_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/delete_user_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/edge.py` & `sc_guard_post-0.3.1/guard_post/models/edge.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/edge_input.py` & `sc_guard_post-0.3.1/guard_post/models/edge_input.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/edge_keys.py` & `sc_guard_post-0.3.1/guard_post/models/edge_keys.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/edge_keys_end_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/edge_keys_end_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/edge_keys_start_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/edge_keys_start_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/edge_userset.py` & `sc_guard_post-0.3.1/guard_post/models/edge_userset.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/error_model.py` & `sc_guard_post-0.3.1/guard_post/models/error_model.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/error_model_details_type_0_item.py` & `sc_guard_post-0.3.1/guard_post/models/error_model_details_type_0_item.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/error_response.py` & `sc_guard_post-0.3.1/guard_post/models/error_response.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/expand_input.py` & `sc_guard_post-0.3.1/guard_post/models/expand_input.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/expand_input_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/expand_input_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/http_validation_error.py` & `sc_guard_post-0.3.1/guard_post/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/list_objects_input_key.py` & `sc_guard_post-0.3.1/guard_post/models/list_objects_input_key.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/list_objects_input_key_key.py` & `sc_guard_post-0.3.1/guard_post/models/list_objects_input_key_key.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/org.py` & `sc_guard_post-0.3.1/guard_post/models/org.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/org_attributes.py` & `sc_guard_post-0.3.1/guard_post/models/org_attributes.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/org_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/org_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/pydantic_models/__init__.py` & `sc_guard_post-0.3.1/guard_post/models/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/ready_response.py` & `sc_guard_post-0.3.1/guard_post/models/ready_response.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/site.py` & `sc_guard_post-0.3.1/guard_post/models/site.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/site_attributes.py` & `sc_guard_post-0.3.1/guard_post/models/site_attributes.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/site_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/site_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/status.py` & `sc_guard_post-0.3.1/guard_post/models/status.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/user.py` & `sc_guard_post-0.3.1/guard_post/models/user.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/user_attributes.py` & `sc_guard_post-0.3.1/guard_post/models/user_attributes.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/user_key_type_0.py` & `sc_guard_post-0.3.1/guard_post/models/user_key_type_0.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/models/validation_error.py` & `sc_guard_post-0.3.1/guard_post/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/guard_post/types.py` & `sc_guard_post-0.3.1/guard_post/types.py`

 * *Files identical despite different names*

### Comparing `sc_guard_post-0.3.0/pyproject.toml` & `sc_guard_post-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc_guard_post"
-version = "0.3.0"
+version = "0.3.1"
 description = "The store connect authorization client."
 
 authors = []
 
 readme = "README.md"
 packages = [{ include = "guard_post" }]
 include = ["CHANGELOG.md", "guard_post/py.typed"]
@@ -14,15 +14,14 @@
 httpx = ">=0.20.0,<=0.26.0"
 attrs = ">=21.3.0"
 python-dateutil = "^2.8.0"
 loguru = "^0.7.2"
 devtools = "^0.12.2"
 pydantic = { extras = ["email"], version = "^2.5.3" }
 sqlalchemy = "^2.0.29"
-mysqlclient = "^2.2.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["I"]
```

### Comparing `sc_guard_post-0.3.0/PKG-INFO` & `sc_guard_post-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: sc_guard_post
-Version: 0.3.0
+Version: 0.3.1
 Summary: The store connect authorization client.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=21.3.0)
 Requires-Dist: devtools (>=0.12.2,<0.13.0)
 Requires-Dist: httpx (>=0.20.0,<=0.26.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: mysqlclient (>=2.2.4,<3.0.0)
 Requires-Dist: pydantic[email] (>=2.5.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Description-Content-Type: text/markdown
 
 # store-connect-auth-z-client
 A client library for accessing sc_auth
```

