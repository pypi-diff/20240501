# Comparing `tmp/horreum-0.12.1.tar.gz` & `tmp/horreum-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horreum-0.12.1.tar", max compression
+gzip compressed data, was "horreum-0.13.tar", max compression
```

## Comparing `horreum-0.12.1.tar` & `horreum-0.13.tar`

### file list

```diff
@@ -1,183 +1,187 @@
--rw-r--r--   0        0        0    11357 2024-04-25 07:44:26.007630 horreum-0.12.1/LICENSE
--rw-r--r--   0        0        0     4256 2024-04-25 07:44:26.007630 horreum-0.12.1/README.md
--rw-r--r--   0        0        0     1231 2024-04-25 07:44:26.011630 horreum-0.12.1/pyproject.toml
--rw-r--r--   0        0        0      209 2024-04-25 07:44:26.011630 horreum-0.12.1/src/horreum/__init__.py
--rw-r--r--   0        0        0      614 2024-04-25 07:44:26.011630 horreum-0.12.1/src/horreum/configs.py
--rw-r--r--   0        0        0     4487 2024-04-25 07:44:26.011630 horreum-0.12.1/src/horreum/horreum_client.py
--rw-r--r--   0        0        0     1108 2024-04-25 07:44:26.011630 horreum-0.12.1/src/horreum/keycloak_access_provider.py
--rw-r--r--   0        0        0     1557 2024-04-25 07:44:44.083606 horreum-0.12.1/src/horreum/raw_client/.kiota.log
--rw-r--r--   0        0        0     2970 2024-04-25 07:44:43.919606 horreum-0.12.1/src/horreum/raw_client/api/api_request_builder.py
--rw-r--r--   0        0        0     2036 2024-04-25 07:44:43.987606 horreum-0.12.1/src/horreum/raw_client/api/config/config_request_builder.py
--rw-r--r--   0        0        0     5746 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/config/datastore/datastore_request_builder.py
--rw-r--r--   0        0        0     4632 2024-04-25 07:44:43.987606 horreum-0.12.1/src/horreum/raw_client/api/config/datastore/item/id_item_request_builder.py
--rw-r--r--   0        0        0     3217 2024-04-25 07:44:43.987606 horreum-0.12.1/src/horreum/raw_client/api/config/datastore/item/test/test_request_builder.py
--rw-r--r--   0        0        0     3258 2024-04-25 07:44:43.987606 horreum-0.12.1/src/horreum/raw_client/api/config/keycloak/keycloak_request_builder.py
--rw-r--r--   0        0        0     3162 2024-04-25 07:44:43.987606 horreum-0.12.1/src/horreum/raw_client/api/config/version/version_request_builder.py
--rw-r--r--   0        0        0     3902 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/dataset/by_schema/by_schema_request_builder.py
--rw-r--r--   0        0        0     2392 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/dataset/dataset_request_builder.py
--rw-r--r--   0        0        0     4276 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/dataset/item/dataset_id_item_request_builder.py
--rw-r--r--   0        0        0     3132 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/dataset/item/label_values/label_values_request_builder.py
--rw-r--r--   0        0        0     3813 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/dataset/item/preview_label/preview_label_request_builder.py
--rw-r--r--   0        0        0     3805 2024-04-25 07:44:43.983606 horreum-0.12.1/src/horreum/raw_client/api/dataset/item/summary/summary_request_builder.py
--rw-r--r--   0        0        0     4964 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/dataset/list_/item/with_test_item_request_builder.py
--rw-r--r--   0        0        0     1688 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/dataset/list_/list_request_builder.py
--rw-r--r--   0        0        0     2357 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/experiment/experiment_request_builder.py
--rw-r--r--   0        0        0     3032 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/experiment/item/profiles/item/with_profile_item_request_builder.py
--rw-r--r--   0        0        0     5798 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/experiment/item/profiles/profiles_request_builder.py
--rw-r--r--   0        0        0     1358 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/experiment/item/with_test_item_request_builder.py
--rw-r--r--   0        0        0     3206 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/experiment/models_requests/models_request_builder.py
--rw-r--r--   0        0        0     4072 2024-04-25 07:44:43.979606 horreum-0.12.1/src/horreum/raw_client/api/experiment/run/run_request_builder.py
--rw-r--r--   0        0        0     3137 2024-04-25 07:44:43.943606 horreum-0.12.1/src/horreum/raw_client/api/run/autocomplete/autocomplete_request_builder.py
--rw-r--r--   0        0        0     3925 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/run/by_schema/by_schema_request_builder.py
--rw-r--r--   0        0        0     3885 2024-04-25 07:44:43.967606 horreum-0.12.1/src/horreum/raw_client/api/run/count/count_request_builder.py
--rw-r--r--   0        0        0     4231 2024-04-25 07:44:43.943606 horreum-0.12.1/src/horreum/raw_client/api/run/data/data_request_builder.py
--rw-r--r--   0        0        0     1713 2024-04-25 07:44:43.959606 horreum-0.12.1/src/horreum/raw_client/api/run/item/data/data_get_response.py
--rw-r--r--   0        0        0     4038 2024-04-25 07:44:43.947606 horreum-0.12.1/src/horreum/raw_client/api/run/item/data/data_request_builder.py
--rw-r--r--   0        0        0     3297 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/description/description_request_builder.py
--rw-r--r--   0        0        0     3006 2024-04-25 07:44:43.947606 horreum-0.12.1/src/horreum/raw_client/api/run/item/drop_token/drop_token_request_builder.py
--rw-r--r--   0        0        0     3913 2024-04-25 07:44:43.947606 horreum-0.12.1/src/horreum/raw_client/api/run/item/label_values/label_values_request_builder.py
--rw-r--r--   0        0        0     1729 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/metadata/metadata_get_response.py
--rw-r--r--   0        0        0     4116 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/metadata/metadata_request_builder.py
--rw-r--r--   0        0        0     3048 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/recalculate/recalculate_request_builder.py
--rw-r--r--   0        0        0     3021 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/reset_token/reset_token_request_builder.py
--rw-r--r--   0        0        0     7840 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/run_item_request_builder.py
--rw-r--r--   0        0        0     1725 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/schema/schema_post_response.py
--rw-r--r--   0        0        0     3827 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/schema/schema_request_builder.py
--rw-r--r--   0        0        0     3397 2024-04-25 07:44:43.947606 horreum-0.12.1/src/horreum/raw_client/api/run/item/summary/summary_request_builder.py
--rw-r--r--   0        0        0     3697 2024-04-25 07:44:43.947606 horreum-0.12.1/src/horreum/raw_client/api/run/item/trash/trash_request_builder.py
--rw-r--r--   0        0        0     3395 2024-04-25 07:44:43.959606 horreum-0.12.1/src/horreum/raw_client/api/run/item/update_access/update_access_request_builder.py
--rw-r--r--   0        0        0     3008 2024-04-25 07:44:43.963606 horreum-0.12.1/src/horreum/raw_client/api/run/item/waitfor_datasets/waitfor_datasets_request_builder.py
--rw-r--r--   0        0        0     3967 2024-04-25 07:44:43.943606 horreum-0.12.1/src/horreum/raw_client/api/run/list_/item/with_test_item_request_builder.py
--rw-r--r--   0        0        0     5823 2024-04-25 07:44:43.943606 horreum-0.12.1/src/horreum/raw_client/api/run/list_/list_request_builder.py
--rw-r--r--   0        0        0     3324 2024-04-25 07:44:43.943606 horreum-0.12.1/src/horreum/raw_client/api/run/recalculate_all/recalculate_all_request_builder.py
--rw-r--r--   0        0        0     4019 2024-04-25 07:44:43.967606 horreum-0.12.1/src/horreum/raw_client/api/run/run_request_builder.py
--rw-r--r--   0        0        0     3777 2024-04-25 07:44:43.967606 horreum-0.12.1/src/horreum/raw_client/api/run/test/test_request_builder.py
--rw-r--r--   0        0        0     3628 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/all_labels/all_labels_request_builder.py
--rw-r--r--   0        0        0     3227 2024-04-25 07:44:43.967606 horreum-0.12.1/src/horreum/raw_client/api/schema/all_transformers/all_transformers_request_builder.py
--rw-r--r--   0        0        0     3505 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/descriptors/descriptors_request_builder.py
--rw-r--r--   0        0        0     3490 2024-04-25 07:44:43.967606 horreum-0.12.1/src/horreum/raw_client/api/schema/find_usages/find_usages_request_builder.py
--rw-r--r--   0        0        0     1632 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/id_by_uri/id_by_uri_request_builder.py
--rw-r--r--   0        0        0     3012 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/id_by_uri/item/with_uri_item_request_builder.py
--rw-r--r--   0        0        0     3621 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/import_/import_request_builder.py
--rw-r--r--   0        0        0     2952 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/drop_token/drop_token_request_builder.py
--rw-r--r--   0        0        0     3120 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/export/export_request_builder.py
--rw-r--r--   0        0        0     6688 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/id_item_request_builder.py
--rw-r--r--   0        0        0     2996 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/labels/item/with_label_item_request_builder.py
--rw-r--r--   0        0        0     5741 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/labels/labels_request_builder.py
--rw-r--r--   0        0        0     3041 2024-04-25 07:44:43.971606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/reset_token/reset_token_request_builder.py
--rw-r--r--   0        0        0     3062 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/transformers/item/with_transformer_item_request_builder.py
--rw-r--r--   0        0        0     5825 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/transformers/transformers_request_builder.py
--rw-r--r--   0        0        0     3418 2024-04-25 07:44:43.975606 horreum-0.12.1/src/horreum/raw_client/api/schema/item/update_access/update_access_request_builder.py
--rw-r--r--   0        0        0     8425 2024-04-25 07:44:43.967606 horreum-0.12.1/src/horreum/raw_client/api/schema/schema_request_builder.py
--rw-r--r--   0        0        0     1649 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/test/by_name/by_name_request_builder.py
--rw-r--r--   0        0        0     3100 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/test/by_name/item/with_name_item_request_builder.py
--rw-r--r--   0        0        0     3297 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/test/folders/folders_request_builder.py
--rw-r--r--   0        0        0     3591 2024-04-25 07:44:43.927606 horreum-0.12.1/src/horreum/raw_client/api/test/import_/import_request_builder.py
--rw-r--r--   0        0        0     3628 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/add_token/add_token_request_builder.py
--rw-r--r--   0        0        0     3046 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/export/export_request_builder.py
--rw-r--r--   0        0        0     3198 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/fingerprint/fingerprint_request_builder.py
--rw-r--r--   0        0        0     4332 2024-04-25 07:44:43.931606 horreum-0.12.1/src/horreum/raw_client/api/test/item/label_values/label_values_request_builder.py
--rw-r--r--   0        0        0     3277 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/move/move_request_builder.py
--rw-r--r--   0        0        0     3555 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/test/item/notifications/notifications_request_builder.py
--rw-r--r--   0        0        0     4352 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/recalculate/recalculate_request_builder.py
--rw-r--r--   0        0        0     2990 2024-04-25 07:44:43.931606 horreum-0.12.1/src/horreum/raw_client/api/test/item/revoke_token/item/with_token_item_request_builder.py
--rw-r--r--   0        0        0     1720 2024-04-25 07:44:43.931606 horreum-0.12.1/src/horreum/raw_client/api/test/item/revoke_token/revoke_token_request_builder.py
--rw-r--r--   0        0        0     8520 2024-04-25 07:44:43.931606 horreum-0.12.1/src/horreum/raw_client/api/test/item/test_item_request_builder.py
--rw-r--r--   0        0        0     3168 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/tokens/tokens_request_builder.py
--rw-r--r--   0        0        0     3336 2024-04-25 07:44:43.935606 horreum-0.12.1/src/horreum/raw_client/api/test/item/transformers/transformers_request_builder.py
--rw-r--r--   0        0        0     3413 2024-04-25 07:44:43.927606 horreum-0.12.1/src/horreum/raw_client/api/test/item/update_access/update_access_request_builder.py
--rw-r--r--   0        0        0     3786 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/test/summary/summary_request_builder.py
--rw-r--r--   0        0        0     7644 2024-04-25 07:44:43.939606 horreum-0.12.1/src/horreum/raw_client/api/test/test_request_builder.py
--rw-r--r--   0        0        0     2612 2024-04-25 07:44:44.047606 horreum-0.12.1/src/horreum/raw_client/horreum_raw_client.py
--rw-r--r--   0        0        0     1256 2024-04-25 07:44:44.071606 horreum-0.12.1/src/horreum/raw_client/kiota-lock.json
--rw-r--r--   0        0        0      126 2024-04-25 07:44:43.991606 horreum-0.12.1/src/horreum/raw_client/models/access.py
--rw-r--r--   0        0        0     7031 2024-04-25 07:44:44.023606 horreum-0.12.1/src/horreum/raw_client/models/action.py
--rw-r--r--   0        0        0     1673 2024-04-25 07:44:44.007606 horreum-0.12.1/src/horreum/raw_client/models/action_secrets.py
--rw-r--r--   0        0        0     6321 2024-04-25 07:44:43.999606 horreum-0.12.1/src/horreum/raw_client/models/change_detection.py
--rw-r--r--   0        0        0     3346 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/condition_component.py
--rw-r--r--   0        0        0     1821 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/condition_component_properties.py
--rw-r--r--   0        0        0     1783 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/condition_component_type.py
--rw-r--r--   0        0        0     3427 2024-04-25 07:44:44.023606 horreum-0.12.1/src/horreum/raw_client/models/condition_config.py
--rw-r--r--   0        0        0     1859 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/condition_config_defaults.py
--rw-r--r--   0        0        0     3523 2024-04-25 07:44:44.031606 horreum-0.12.1/src/horreum/raw_client/models/dataset.py
--rw-r--r--   0        0        0     2482 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/dataset_info.py
--rw-r--r--   0        0        0     2523 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/dataset_list.py
--rw-r--r--   0        0        0     2778 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/dataset_log.py
--rw-r--r--   0        0        0     4352 2024-04-25 07:44:44.015606 horreum-0.12.1/src/horreum/raw_client/models/dataset_summary.py
--rw-r--r--   0        0        0     1939 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/dataset_summary_view.py
--rw-r--r--   0        0        0     6924 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/datastore.py
--rw-r--r--   0        0        0      136 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/datastore_access.py
--rw-r--r--   0        0        0     2108 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/datastore_test_response.py
--rw-r--r--   0        0        0      121 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/datastore_type.py
--rw-r--r--   0        0        0     2775 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/elasticsearch_datastore_config.py
--rw-r--r--   0        0        0     4477 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/error_details.py
--rw-r--r--   0        0        0     2592 2024-04-25 07:44:43.991606 horreum-0.12.1/src/horreum/raw_client/models/experiment_comparison.py
--rw-r--r--   0        0        0     4466 2024-04-25 07:44:44.031606 horreum-0.12.1/src/horreum/raw_client/models/experiment_profile.py
--rw-r--r--   0        0        0     4573 2024-04-25 07:44:44.023606 horreum-0.12.1/src/horreum/raw_client/models/experiment_result.py
--rw-r--r--   0        0        0     1845 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/experiment_result_dataset_info.py
--rw-r--r--   0        0        0     1879 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/experiment_result_profile.py
--rw-r--r--   0        0        0     1837 2024-04-25 07:44:44.019606 horreum-0.12.1/src/horreum/raw_client/models/experiment_result_results.py
--rw-r--r--   0        0        0     3058 2024-04-25 07:44:44.007606 horreum-0.12.1/src/horreum/raw_client/models/exported_label_values.py
--rw-r--r--   0        0        0     2581 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/extractor.py
--rw-r--r--   0        0        0     2001 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/fingerprint_value.py
--rw-r--r--   0        0        0     2215 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/fingerprints.py
--rw-r--r--   0        0        0     2340 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/fix_threshold_config.py
--rw-r--r--   0        0        0     3060 2024-04-25 07:44:44.019606 horreum-0.12.1/src/horreum/raw_client/models/fixed_threshold_detection_config.py
--rw-r--r--   0        0        0     1929 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/fixed_threshold_detection_config_max.py
--rw-r--r--   0        0        0     1929 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/fixed_threshold_detection_config_min.py
--rw-r--r--   0        0        0     2708 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/github_issue_comment_action.py
--rw-r--r--   0        0        0     2499 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/github_issue_create_action.py
--rw-r--r--   0        0        0     1865 2024-04-25 07:44:44.015606 horreum-0.12.1/src/horreum/raw_client/models/http_action.py
--rw-r--r--   0        0        0     1733 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/indexed_label_value_map.py
--rw-r--r--   0        0        0     2350 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/keycloak_config.py
--rw-r--r--   0        0        0     3820 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/label.py
--rw-r--r--   0        0        0     1756 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/label_in_fingerprint.py
--rw-r--r--   0        0        0     2487 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/label_in_report.py
--rw-r--r--   0        0        0     2126 2024-04-25 07:44:44.019606 horreum-0.12.1/src/horreum/raw_client/models/label_in_rule.py
--rw-r--r--   0        0        0     2190 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/label_in_variable.py
--rw-r--r--   0        0        0     2539 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/label_in_view.py
--rw-r--r--   0        0        0     2753 2024-04-25 07:44:44.007606 horreum-0.12.1/src/horreum/raw_client/models/label_info.py
--rw-r--r--   0        0        0     2324 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/label_location.py
--rw-r--r--   0        0        0     2380 2024-04-25 07:44:43.991606 horreum-0.12.1/src/horreum/raw_client/models/label_preview.py
--rw-r--r--   0        0        0     2791 2024-04-25 07:44:44.023606 horreum-0.12.1/src/horreum/raw_client/models/label_value.py
--rw-r--r--   0        0        0     1754 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/label_value_map.py
--rw-r--r--   0        0        0     1829 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/label_value_schema.py
--rw-r--r--   0        0        0     3221 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/missing_data_rule.py
--rw-r--r--   0        0        0     2534 2024-04-25 07:44:44.015606 horreum-0.12.1/src/horreum/raw_client/models/persistent_log.py
--rw-r--r--   0        0        0     1982 2024-04-25 07:44:44.031606 horreum-0.12.1/src/horreum/raw_client/models/postgres_datastore_config.py
--rw-r--r--   0        0        0     2887 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/protected_time_type.py
--rw-r--r--   0        0        0      144 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/protected_time_type_access.py
--rw-r--r--   0        0        0     2472 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/protected_type.py
--rw-r--r--   0        0        0      140 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/protected_type_access.py
--rw-r--r--   0        0        0     2602 2024-04-25 07:44:44.015606 horreum-0.12.1/src/horreum/raw_client/models/recalculation_status.py
--rw-r--r--   0        0        0     2970 2024-04-25 07:44:44.019606 horreum-0.12.1/src/horreum/raw_client/models/relative_difference_detection_config.py
--rw-r--r--   0        0        0     4792 2024-04-25 07:44:44.019606 horreum-0.12.1/src/horreum/raw_client/models/run.py
--rw-r--r--   0        0        0      130 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/run_access.py
--rw-r--r--   0        0        0     2286 2024-04-25 07:44:44.027606 horreum-0.12.1/src/horreum/raw_client/models/run_count.py
--rw-r--r--   0        0        0     5350 2024-04-25 07:44:44.007606 horreum-0.12.1/src/horreum/raw_client/models/run_extended.py
--rw-r--r--   0        0        0      138 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/run_extended_access.py
--rw-r--r--   0        0        0     4314 2024-04-25 07:44:44.031606 horreum-0.12.1/src/horreum/raw_client/models/run_summary.py
--rw-r--r--   0        0        0     2280 2024-04-25 07:44:44.047606 horreum-0.12.1/src/horreum/raw_client/models/runs_summary.py
--rw-r--r--   0        0        0     2966 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/schema.py
--rw-r--r--   0        0        0     2223 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/schema_descriptor.py
--rw-r--r--   0        0        0     2555 2024-04-25 07:44:43.991606 horreum-0.12.1/src/horreum/raw_client/models/schema_export.py
--rw-r--r--   0        0        0     2342 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/schema_query_result.py
--rw-r--r--   0        0        0     3124 2024-04-25 07:44:44.031606 horreum-0.12.1/src/horreum/raw_client/models/schema_usage.py
--rw-r--r--   0        0        0     2066 2024-04-25 07:44:44.047606 horreum-0.12.1/src/horreum/raw_client/models/secret.py
--rw-r--r--   0        0        0      116 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/sort_direction.py
--rw-r--r--   0        0        0     5589 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/test.py
--rw-r--r--   0        0        0     4436 2024-04-25 07:44:44.039606 horreum-0.12.1/src/horreum/raw_client/models/test_export.py
--rw-r--r--   0        0        0     1775 2024-04-25 07:44:43.991606 horreum-0.12.1/src/horreum/raw_client/models/test_export_datastore.py
--rw-r--r--   0        0        0     1760 2024-04-25 07:44:44.023606 horreum-0.12.1/src/horreum/raw_client/models/test_export_subscriptions.py
--rw-r--r--   0        0        0     2310 2024-04-25 07:44:44.003606 horreum-0.12.1/src/horreum/raw_client/models/test_listing.py
--rw-r--r--   0        0        0     2302 2024-04-25 07:44:44.035606 horreum-0.12.1/src/horreum/raw_client/models/test_query_result.py
--rw-r--r--   0        0        0     3455 2024-04-25 07:44:44.011606 horreum-0.12.1/src/horreum/raw_client/models/test_summary.py
--rw-r--r--   0        0        0     2660 2024-04-25 07:44:43.995606 horreum-0.12.1/src/horreum/raw_client/models/test_token.py
--rw-r--r--   0        0        0     4200 2024-04-25 07:44:44.015606 horreum-0.12.1/src/horreum/raw_client/models/transformer.py
--rw-r--r--   0        0        0     2768 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/transformer_info.py
--rw-r--r--   0        0        0     2389 2024-04-25 07:44:44.007606 horreum-0.12.1/src/horreum/raw_client/models/validation_error.py
--rw-r--r--   0        0        0     1804 2024-04-25 07:44:44.043606 horreum-0.12.1/src/horreum/raw_client/models/validation_error_error.py
--rw-r--r--   0        0        0     3546 2024-04-25 07:44:44.019606 horreum-0.12.1/src/horreum/raw_client/models/variable.py
--rw-r--r--   0        0        0     2373 2024-04-25 07:44:43.991606 horreum-0.12.1/src/horreum/raw_client/models/version_info.py
--rw-r--r--   0        0        0     2743 2024-04-25 07:44:44.015606 horreum-0.12.1/src/horreum/raw_client/models/watch.py
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 horreum-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 10:21:20.691823 horreum-0.13/LICENSE
+-rw-r--r--   0        0        0     4256 2024-05-01 10:21:20.691823 horreum-0.13/README.md
+-rw-r--r--   0        0        0     1229 2024-05-01 10:21:20.691823 horreum-0.13/pyproject.toml
+-rw-r--r--   0        0        0      209 2024-05-01 10:21:20.691823 horreum-0.13/src/horreum/__init__.py
+-rw-r--r--   0        0        0      614 2024-05-01 10:21:20.691823 horreum-0.13/src/horreum/configs.py
+-rw-r--r--   0        0        0     4487 2024-05-01 10:21:20.691823 horreum-0.13/src/horreum/horreum_client.py
+-rw-r--r--   0        0        0     1108 2024-05-01 10:21:20.691823 horreum-0.13/src/horreum/keycloak_access_provider.py
+-rw-r--r--   0        0        0     1557 2024-05-01 10:21:35.319909 horreum-0.13/src/horreum/raw_client/.kiota.log
+-rw-r--r--   0        0        0     2970 2024-05-01 10:21:35.155908 horreum-0.13/src/horreum/raw_client/api/api_request_builder.py
+-rw-r--r--   0        0        0     2036 2024-05-01 10:21:35.219909 horreum-0.13/src/horreum/raw_client/api/config/config_request_builder.py
+-rw-r--r--   0        0        0     5746 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/config/datastore/datastore_request_builder.py
+-rw-r--r--   0        0        0     4632 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/config/datastore/item/id_item_request_builder.py
+-rw-r--r--   0        0        0     3217 2024-05-01 10:21:35.219909 horreum-0.13/src/horreum/raw_client/api/config/datastore/item/test/test_request_builder.py
+-rw-r--r--   0        0        0     3258 2024-05-01 10:21:35.219909 horreum-0.13/src/horreum/raw_client/api/config/keycloak/keycloak_request_builder.py
+-rw-r--r--   0        0        0     3162 2024-05-01 10:21:35.219909 horreum-0.13/src/horreum/raw_client/api/config/version/version_request_builder.py
+-rw-r--r--   0        0        0     3902 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/dataset/by_schema/by_schema_request_builder.py
+-rw-r--r--   0        0        0     2392 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/dataset/dataset_request_builder.py
+-rw-r--r--   0        0        0     4276 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/dataset/item/dataset_id_item_request_builder.py
+-rw-r--r--   0        0        0     3132 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/dataset/item/label_values/label_values_request_builder.py
+-rw-r--r--   0        0        0     3813 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/dataset/item/preview_label/preview_label_request_builder.py
+-rw-r--r--   0        0        0     3805 2024-05-01 10:21:35.215909 horreum-0.13/src/horreum/raw_client/api/dataset/item/summary/summary_request_builder.py
+-rw-r--r--   0        0        0     4964 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/dataset/list_/item/with_test_item_request_builder.py
+-rw-r--r--   0        0        0     1688 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/dataset/list_/list_request_builder.py
+-rw-r--r--   0        0        0     2357 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/experiment/experiment_request_builder.py
+-rw-r--r--   0        0        0     3032 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/experiment/item/profiles/item/with_profile_item_request_builder.py
+-rw-r--r--   0        0        0     5798 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/experiment/item/profiles/profiles_request_builder.py
+-rw-r--r--   0        0        0     1358 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/experiment/item/with_test_item_request_builder.py
+-rw-r--r--   0        0        0     3206 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/experiment/models_requests/models_request_builder.py
+-rw-r--r--   0        0        0     4072 2024-05-01 10:21:35.211909 horreum-0.13/src/horreum/raw_client/api/experiment/run/run_request_builder.py
+-rw-r--r--   0        0        0     3176 2024-05-01 10:21:35.175908 horreum-0.13/src/horreum/raw_client/api/run/autocomplete/autocomplete_request_builder.py
+-rw-r--r--   0        0        0     3925 2024-05-01 10:21:35.175908 horreum-0.13/src/horreum/raw_client/api/run/by_schema/by_schema_request_builder.py
+-rw-r--r--   0        0        0     3885 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/count/count_request_builder.py
+-rw-r--r--   0        0        0     4231 2024-05-01 10:21:35.179909 horreum-0.13/src/horreum/raw_client/api/run/data/data_request_builder.py
+-rw-r--r--   0        0        0     1713 2024-05-01 10:21:35.191908 horreum-0.13/src/horreum/raw_client/api/run/item/data/data_get_response.py
+-rw-r--r--   0        0        0     4038 2024-05-01 10:21:35.179909 horreum-0.13/src/horreum/raw_client/api/run/item/data/data_request_builder.py
+-rw-r--r--   0        0        0     3297 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/description/description_request_builder.py
+-rw-r--r--   0        0        0     3006 2024-05-01 10:21:35.179909 horreum-0.13/src/horreum/raw_client/api/run/item/drop_token/drop_token_request_builder.py
+-rw-r--r--   0        0        0     4179 2024-05-01 10:21:35.179909 horreum-0.13/src/horreum/raw_client/api/run/item/label_values/label_values_request_builder.py
+-rw-r--r--   0        0        0     1729 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/metadata/metadata_get_response.py
+-rw-r--r--   0        0        0     4116 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/metadata/metadata_request_builder.py
+-rw-r--r--   0        0        0     3048 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/recalculate/recalculate_request_builder.py
+-rw-r--r--   0        0        0     3021 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/reset_token/reset_token_request_builder.py
+-rw-r--r--   0        0        0     7407 2024-05-01 10:21:35.191908 horreum-0.13/src/horreum/raw_client/api/run/item/run_item_request_builder.py
+-rw-r--r--   0        0        0     1725 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/schema/schema_post_response.py
+-rw-r--r--   0        0        0     3827 2024-05-01 10:21:35.195909 horreum-0.13/src/horreum/raw_client/api/run/item/schema/schema_request_builder.py
+-rw-r--r--   0        0        0     3397 2024-05-01 10:21:35.179909 horreum-0.13/src/horreum/raw_client/api/run/item/summary/summary_request_builder.py
+-rw-r--r--   0        0        0     3697 2024-05-01 10:21:35.179909 horreum-0.13/src/horreum/raw_client/api/run/item/trash/trash_request_builder.py
+-rw-r--r--   0        0        0     3395 2024-05-01 10:21:35.191908 horreum-0.13/src/horreum/raw_client/api/run/item/update_access/update_access_request_builder.py
+-rw-r--r--   0        0        0     3967 2024-05-01 10:21:35.175908 horreum-0.13/src/horreum/raw_client/api/run/list_/item/with_test_item_request_builder.py
+-rw-r--r--   0        0        0     5823 2024-05-01 10:21:35.175908 horreum-0.13/src/horreum/raw_client/api/run/list_/list_request_builder.py
+-rw-r--r--   0        0        0     3324 2024-05-01 10:21:35.175908 horreum-0.13/src/horreum/raw_client/api/run/recalculate_all/recalculate_all_request_builder.py
+-rw-r--r--   0        0        0     4019 2024-05-01 10:21:35.199909 horreum-0.13/src/horreum/raw_client/api/run/run_request_builder.py
+-rw-r--r--   0        0        0     3777 2024-05-01 10:21:35.199909 horreum-0.13/src/horreum/raw_client/api/run/test/test_request_builder.py
+-rw-r--r--   0        0        0     3628 2024-05-01 10:21:35.199909 horreum-0.13/src/horreum/raw_client/api/schema/all_labels/all_labels_request_builder.py
+-rw-r--r--   0        0        0     3227 2024-05-01 10:21:35.199909 horreum-0.13/src/horreum/raw_client/api/schema/all_transformers/all_transformers_request_builder.py
+-rw-r--r--   0        0        0     3505 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/schema/descriptors/descriptors_request_builder.py
+-rw-r--r--   0        0        0     3490 2024-05-01 10:21:35.199909 horreum-0.13/src/horreum/raw_client/api/schema/find_usages/find_usages_request_builder.py
+-rw-r--r--   0        0        0     1632 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/schema/id_by_uri/id_by_uri_request_builder.py
+-rw-r--r--   0        0        0     3012 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/schema/id_by_uri/item/with_uri_item_request_builder.py
+-rw-r--r--   0        0        0     3621 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/schema/import_/import_request_builder.py
+-rw-r--r--   0        0        0     2952 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/drop_token/drop_token_request_builder.py
+-rw-r--r--   0        0        0     3120 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/export/export_request_builder.py
+-rw-r--r--   0        0        0     6688 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/id_item_request_builder.py
+-rw-r--r--   0        0        0     2996 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/labels/item/with_label_item_request_builder.py
+-rw-r--r--   0        0        0     5741 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/labels/labels_request_builder.py
+-rw-r--r--   0        0        0     3041 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/reset_token/reset_token_request_builder.py
+-rw-r--r--   0        0        0     3062 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/schema/item/transformers/item/with_transformer_item_request_builder.py
+-rw-r--r--   0        0        0     5825 2024-05-01 10:21:35.207909 horreum-0.13/src/horreum/raw_client/api/schema/item/transformers/transformers_request_builder.py
+-rw-r--r--   0        0        0     3418 2024-05-01 10:21:35.203909 horreum-0.13/src/horreum/raw_client/api/schema/item/update_access/update_access_request_builder.py
+-rw-r--r--   0        0        0     8527 2024-05-01 10:21:35.199909 horreum-0.13/src/horreum/raw_client/api/schema/schema_request_builder.py
+-rw-r--r--   0        0        0     1649 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/by_name/by_name_request_builder.py
+-rw-r--r--   0        0        0     3100 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/by_name/item/with_name_item_request_builder.py
+-rw-r--r--   0        0        0     3297 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/folders/folders_request_builder.py
+-rw-r--r--   0        0        0     3591 2024-05-01 10:21:35.159908 horreum-0.13/src/horreum/raw_client/api/test/import_/import_request_builder.py
+-rw-r--r--   0        0        0     3628 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/add_token/add_token_request_builder.py
+-rw-r--r--   0        0        0     3046 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/export/export_request_builder.py
+-rw-r--r--   0        0        0     3198 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/fingerprint/fingerprint_request_builder.py
+-rw-r--r--   0        0        0     4598 2024-05-01 10:21:35.163908 horreum-0.13/src/horreum/raw_client/api/test/item/label_values/label_values_request_builder.py
+-rw-r--r--   0        0        0     3277 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/move/move_request_builder.py
+-rw-r--r--   0        0        0     3555 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/item/notifications/notifications_request_builder.py
+-rw-r--r--   0        0        0     4352 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/item/recalculate/recalculate_request_builder.py
+-rw-r--r--   0        0        0     2990 2024-05-01 10:21:35.163908 horreum-0.13/src/horreum/raw_client/api/test/item/revoke_token/item/with_token_item_request_builder.py
+-rw-r--r--   0        0        0     1720 2024-05-01 10:21:35.163908 horreum-0.13/src/horreum/raw_client/api/test/item/revoke_token/revoke_token_request_builder.py
+-rw-r--r--   0        0        0     8520 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/test_item_request_builder.py
+-rw-r--r--   0        0        0     3168 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/tokens/tokens_request_builder.py
+-rw-r--r--   0        0        0     3336 2024-05-01 10:21:35.167909 horreum-0.13/src/horreum/raw_client/api/test/item/transformers/transformers_request_builder.py
+-rw-r--r--   0        0        0     3413 2024-05-01 10:21:35.163908 horreum-0.13/src/horreum/raw_client/api/test/item/update_access/update_access_request_builder.py
+-rw-r--r--   0        0        0     3786 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/summary/summary_request_builder.py
+-rw-r--r--   0        0        0     7644 2024-05-01 10:21:35.171908 horreum-0.13/src/horreum/raw_client/api/test/test_request_builder.py
+-rw-r--r--   0        0        0     2612 2024-05-01 10:21:35.279909 horreum-0.13/src/horreum/raw_client/horreum_raw_client.py
+-rw-r--r--   0        0        0     1256 2024-05-01 10:21:35.303909 horreum-0.13/src/horreum/raw_client/kiota-lock.json
+-rw-r--r--   0        0        0      126 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/access.py
+-rw-r--r--   0        0        0     9115 2024-05-01 10:21:35.255909 horreum-0.13/src/horreum/raw_client/models/action.py
+-rw-r--r--   0        0        0     1673 2024-05-01 10:21:35.239909 horreum-0.13/src/horreum/raw_client/models/action_secrets.py
+-rw-r--r--   0        0        0     7235 2024-05-01 10:21:35.231909 horreum-0.13/src/horreum/raw_client/models/change_detection.py
+-rw-r--r--   0        0        0     3346 2024-05-01 10:21:35.227909 horreum-0.13/src/horreum/raw_client/models/condition_component.py
+-rw-r--r--   0        0        0     1821 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/condition_component_properties.py
+-rw-r--r--   0        0        0     1783 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/condition_component_type.py
+-rw-r--r--   0        0        0     3427 2024-05-01 10:21:35.255909 horreum-0.13/src/horreum/raw_client/models/condition_config.py
+-rw-r--r--   0        0        0     1859 2024-05-01 10:21:35.227909 horreum-0.13/src/horreum/raw_client/models/condition_config_defaults.py
+-rw-r--r--   0        0        0     3523 2024-05-01 10:21:35.263909 horreum-0.13/src/horreum/raw_client/models/dataset.py
+-rw-r--r--   0        0        0     2482 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/dataset_info.py
+-rw-r--r--   0        0        0     2523 2024-05-01 10:21:35.227909 horreum-0.13/src/horreum/raw_client/models/dataset_list.py
+-rw-r--r--   0        0        0     2778 2024-05-01 10:21:35.235909 horreum-0.13/src/horreum/raw_client/models/dataset_log.py
+-rw-r--r--   0        0        0     4352 2024-05-01 10:21:35.247909 horreum-0.13/src/horreum/raw_client/models/dataset_summary.py
+-rw-r--r--   0        0        0     1939 2024-05-01 10:21:35.227909 horreum-0.13/src/horreum/raw_client/models/dataset_summary_view.py
+-rw-r--r--   0        0        0     6924 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/datastore.py
+-rw-r--r--   0        0        0      136 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/datastore_access.py
+-rw-r--r--   0        0        0     2108 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/datastore_test_response.py
+-rw-r--r--   0        0        0      121 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/datastore_type.py
+-rw-r--r--   0        0        0     2457 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/e_divisive_detection_config.py
+-rw-r--r--   0        0        0      102 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/e_divisive_detection_config_model.py
+-rw-r--r--   0        0        0     2775 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/elasticsearch_datastore_config.py
+-rw-r--r--   0        0        0     4477 2024-05-01 10:21:35.239909 horreum-0.13/src/horreum/raw_client/models/error_details.py
+-rw-r--r--   0        0        0     2592 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/experiment_comparison.py
+-rw-r--r--   0        0        0     4466 2024-05-01 10:21:35.263909 horreum-0.13/src/horreum/raw_client/models/experiment_profile.py
+-rw-r--r--   0        0        0     4573 2024-05-01 10:21:35.255909 horreum-0.13/src/horreum/raw_client/models/experiment_result.py
+-rw-r--r--   0        0        0     1845 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/experiment_result_dataset_info.py
+-rw-r--r--   0        0        0     1879 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/experiment_result_profile.py
+-rw-r--r--   0        0        0     1837 2024-05-01 10:21:35.251909 horreum-0.13/src/horreum/raw_client/models/experiment_result_results.py
+-rw-r--r--   0        0        0     3058 2024-05-01 10:21:35.235909 horreum-0.13/src/horreum/raw_client/models/exported_label_values.py
+-rw-r--r--   0        0        0     2581 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/extractor.py
+-rw-r--r--   0        0        0     2001 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/fingerprint_value.py
+-rw-r--r--   0        0        0     2215 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/fingerprints.py
+-rw-r--r--   0        0        0     2340 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/fix_threshold_config.py
+-rw-r--r--   0        0        0     3597 2024-05-01 10:21:35.247909 horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config.py
+-rw-r--r--   0        0        0     1929 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config_max.py
+-rw-r--r--   0        0        0     1929 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config_min.py
+-rw-r--r--   0        0        0      117 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config_model.py
+-rw-r--r--   0        0        0     2901 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/github_issue_comment_action_config.py
+-rw-r--r--   0        0        0     2696 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/github_issue_create_action_config.py
+-rw-r--r--   0        0        0     2057 2024-05-01 10:21:35.279909 horreum-0.13/src/horreum/raw_client/models/http_action_config.py
+-rw-r--r--   0        0        0     1733 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/indexed_label_value_map.py
+-rw-r--r--   0        0        0     2350 2024-05-01 10:21:35.239909 horreum-0.13/src/horreum/raw_client/models/keycloak_config.py
+-rw-r--r--   0        0        0     3820 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/label.py
+-rw-r--r--   0        0        0     1756 2024-05-01 10:21:35.235909 horreum-0.13/src/horreum/raw_client/models/label_in_fingerprint.py
+-rw-r--r--   0        0        0     2487 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/label_in_report.py
+-rw-r--r--   0        0        0     2126 2024-05-01 10:21:35.251909 horreum-0.13/src/horreum/raw_client/models/label_in_rule.py
+-rw-r--r--   0        0        0     2190 2024-05-01 10:21:35.231909 horreum-0.13/src/horreum/raw_client/models/label_in_variable.py
+-rw-r--r--   0        0        0     2539 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/label_in_view.py
+-rw-r--r--   0        0        0     2753 2024-05-01 10:21:35.239909 horreum-0.13/src/horreum/raw_client/models/label_info.py
+-rw-r--r--   0        0        0     2324 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/label_location.py
+-rw-r--r--   0        0        0     2380 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/label_preview.py
+-rw-r--r--   0        0        0     2791 2024-05-01 10:21:35.255909 horreum-0.13/src/horreum/raw_client/models/label_value.py
+-rw-r--r--   0        0        0     1754 2024-05-01 10:21:35.231909 horreum-0.13/src/horreum/raw_client/models/label_value_map.py
+-rw-r--r--   0        0        0     1829 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/label_value_schema.py
+-rw-r--r--   0        0        0     3221 2024-05-01 10:21:35.263909 horreum-0.13/src/horreum/raw_client/models/missing_data_rule.py
+-rw-r--r--   0        0        0     2534 2024-05-01 10:21:35.247909 horreum-0.13/src/horreum/raw_client/models/persistent_log.py
+-rw-r--r--   0        0        0     1982 2024-05-01 10:21:35.263909 horreum-0.13/src/horreum/raw_client/models/postgres_datastore_config.py
+-rw-r--r--   0        0        0     2887 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/protected_time_type.py
+-rw-r--r--   0        0        0      144 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/protected_time_type_access.py
+-rw-r--r--   0        0        0     2472 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/protected_type.py
+-rw-r--r--   0        0        0      140 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/protected_type_access.py
+-rw-r--r--   0        0        0     2602 2024-05-01 10:21:35.247909 horreum-0.13/src/horreum/raw_client/models/recalculation_status.py
+-rw-r--r--   0        0        0     3560 2024-05-01 10:21:35.251909 horreum-0.13/src/horreum/raw_client/models/relative_difference_detection_config.py
+-rw-r--r--   0        0        0      129 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/relative_difference_detection_config_model.py
+-rw-r--r--   0        0        0     4792 2024-05-01 10:21:35.251909 horreum-0.13/src/horreum/raw_client/models/run.py
+-rw-r--r--   0        0        0      130 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/run_access.py
+-rw-r--r--   0        0        0     2286 2024-05-01 10:21:35.259909 horreum-0.13/src/horreum/raw_client/models/run_count.py
+-rw-r--r--   0        0        0     5350 2024-05-01 10:21:35.239909 horreum-0.13/src/horreum/raw_client/models/run_extended.py
+-rw-r--r--   0        0        0      138 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/run_extended_access.py
+-rw-r--r--   0        0        0     4314 2024-05-01 10:21:35.263909 horreum-0.13/src/horreum/raw_client/models/run_summary.py
+-rw-r--r--   0        0        0     2280 2024-05-01 10:21:35.279909 horreum-0.13/src/horreum/raw_client/models/runs_summary.py
+-rw-r--r--   0        0        0     2966 2024-05-01 10:21:35.235909 horreum-0.13/src/horreum/raw_client/models/schema.py
+-rw-r--r--   0        0        0     2223 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/schema_descriptor.py
+-rw-r--r--   0        0        0     2555 2024-05-01 10:21:35.219909 horreum-0.13/src/horreum/raw_client/models/schema_export.py
+-rw-r--r--   0        0        0     2342 2024-05-01 10:21:35.227909 horreum-0.13/src/horreum/raw_client/models/schema_query_result.py
+-rw-r--r--   0        0        0     3124 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/schema_usage.py
+-rw-r--r--   0        0        0     2066 2024-05-01 10:21:35.279909 horreum-0.13/src/horreum/raw_client/models/secret.py
+-rw-r--r--   0        0        0     2349 2024-05-01 10:21:35.251909 horreum-0.13/src/horreum/raw_client/models/slack_channel_message_action_config.py
+-rw-r--r--   0        0        0      116 2024-05-01 10:21:35.235909 horreum-0.13/src/horreum/raw_client/models/sort_direction.py
+-rw-r--r--   0        0        0     5589 2024-05-01 10:21:35.279909 horreum-0.13/src/horreum/raw_client/models/test.py
+-rw-r--r--   0        0        0     4436 2024-05-01 10:21:35.271909 horreum-0.13/src/horreum/raw_client/models/test_export.py
+-rw-r--r--   0        0        0     1775 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/test_export_datastore.py
+-rw-r--r--   0        0        0     1760 2024-05-01 10:21:35.255909 horreum-0.13/src/horreum/raw_client/models/test_export_subscriptions.py
+-rw-r--r--   0        0        0     2310 2024-05-01 10:21:35.235909 horreum-0.13/src/horreum/raw_client/models/test_listing.py
+-rw-r--r--   0        0        0     2302 2024-05-01 10:21:35.267909 horreum-0.13/src/horreum/raw_client/models/test_query_result.py
+-rw-r--r--   0        0        0     3455 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/test_summary.py
+-rw-r--r--   0        0        0     2660 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/test_token.py
+-rw-r--r--   0        0        0     4200 2024-05-01 10:21:35.247909 horreum-0.13/src/horreum/raw_client/models/transformer.py
+-rw-r--r--   0        0        0     2768 2024-05-01 10:21:35.275909 horreum-0.13/src/horreum/raw_client/models/transformer_info.py
+-rw-r--r--   0        0        0     2389 2024-05-01 10:21:35.239909 horreum-0.13/src/horreum/raw_client/models/validation_error.py
+-rw-r--r--   0        0        0     1804 2024-05-01 10:21:35.279909 horreum-0.13/src/horreum/raw_client/models/validation_error_error.py
+-rw-r--r--   0        0        0     3546 2024-05-01 10:21:35.251909 horreum-0.13/src/horreum/raw_client/models/variable.py
+-rw-r--r--   0        0        0     2373 2024-05-01 10:21:35.223909 horreum-0.13/src/horreum/raw_client/models/version_info.py
+-rw-r--r--   0        0        0     2743 2024-05-01 10:21:35.243909 horreum-0.13/src/horreum/raw_client/models/watch.py
+-rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 horreum-0.13/PKG-INFO
```

### Comparing `horreum-0.12.1/LICENSE` & `horreum-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/README.md` & `horreum-0.13/README.md`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/pyproject.toml` & `horreum-0.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horreum"
-version = "0.12.1"
+version = "0.13"
 description = "Horreum python library"
 keywords = ["horreum", "performance", "change-detection"]
 authors = ["Andrea Lamparelli <alampare@redhat.com>"]
 maintainers = [
     "Andrea Lamparelli <alampare@redhat.com>",
     "John O'Hara <johara@redhat.com>",
     "Stale Pedersen <spederse@redhat.com>"
```

### Comparing `horreum-0.12.1/src/horreum/configs.py` & `horreum-0.13/src/horreum/configs.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/horreum_client.py` & `horreum-0.13/src/horreum/horreum_client.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/keycloak_access_provider.py` & `horreum-0.13/src/horreum/keycloak_access_provider.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/.kiota.log` & `horreum-0.13/src/horreum/raw_client/.kiota.log`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/api_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/api_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/config/config_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/config/config_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/config/datastore/datastore_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/config/datastore/datastore_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/config/datastore/item/id_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/config/datastore/item/id_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/config/datastore/item/test/test_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/config/datastore/item/test/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/config/keycloak/keycloak_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/config/keycloak/keycloak_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/config/version/version_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/config/version/version_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/by_schema/by_schema_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/by_schema/by_schema_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/dataset_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/dataset_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/item/dataset_id_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/item/dataset_id_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/item/label_values/label_values_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/item/label_values/label_values_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/item/preview_label/preview_label_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/item/preview_label/preview_label_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/item/summary/summary_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/item/summary/summary_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/list_/item/with_test_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/list_/item/with_test_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/dataset/list_/list_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/dataset/list_/list_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/experiment/experiment_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/experiment/experiment_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/experiment/item/profiles/item/with_profile_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/experiment/item/profiles/item/with_profile_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/experiment/item/profiles/profiles_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/experiment/item/profiles/profiles_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/experiment/item/with_test_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/experiment/item/with_test_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/experiment/models_requests/models_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/experiment/models_requests/models_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/experiment/run/run_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/experiment/run/run_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/autocomplete/autocomplete_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/autocomplete/autocomplete_request_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,12 @@
         """
         if not raw_url:
             raise TypeError("raw_url cannot be null.")
         return AutocompleteRequestBuilder(self.request_adapter, raw_url)
     
     @dataclass
     class AutocompleteRequestBuilderGetQueryParameters():
+        # JSONPath to be autocompleted
         query: Optional[str] = None
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/by_schema/by_schema_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/by_schema/by_schema_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/count/count_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/count/count_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/data/data_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/data/data_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/data/data_get_response.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/data/data_get_response.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/data/data_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/data/data_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/description/description_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/description/description_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/drop_token/drop_token_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/drop_token/drop_token_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/label_values/label_values_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/label_values/label_values_request_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
         Instantiates a new LabelValuesRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/run/{id}/labelValues{?direction*,filter*,limit*,page*,sort*}", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/run/{id}/labelValues{?direction*,exclude*,filter*,include*,limit*,page*,sort*}", path_parameters)
     
     async def get(self,request_configuration: Optional[RequestConfiguration] = None) -> Optional[List[ExportedLabelValues]]:
         """
         Get all the label values for the run
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: Optional[List[ExportedLabelValues]]
         """
@@ -66,17 +66,23 @@
     class LabelValuesRequestBuilderGetQueryParameters():
         """
         Get all the label values for the run
         """
         # either Ascending or Descending
         direction: Optional[str] = None
 
+        # label name(s) to exclude from the result as scalar or comma separated
+        exclude: Optional[List[str]] = None
+
         # either a required json sub-document or path expression
         filter: Optional[str] = None
 
+        # label name(s) to include in the result as scalar or comma separated
+        include: Optional[List[str]] = None
+
         # the maximum number of results to include
         limit: Optional[int] = None
 
         # which page to skip to when using a limit
         page: Optional[int] = None
 
         # label name for sorting
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/metadata/metadata_get_response.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/metadata/metadata_get_response.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/metadata/metadata_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/metadata/metadata_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/recalculate/recalculate_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/recalculate/recalculate_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/reset_token/reset_token_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/reset_token/reset_token_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/run_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/run_item_request_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     from .metadata.metadata_request_builder import MetadataRequestBuilder
     from .recalculate.recalculate_request_builder import RecalculateRequestBuilder
     from .reset_token.reset_token_request_builder import ResetTokenRequestBuilder
     from .schema.schema_request_builder import SchemaRequestBuilder
     from .summary.summary_request_builder import SummaryRequestBuilder
     from .trash.trash_request_builder import TrashRequestBuilder
     from .update_access.update_access_request_builder import UpdateAccessRequestBuilder
-    from .waitfor_datasets.waitfor_datasets_request_builder import WaitforDatasetsRequestBuilder
 
 class RunItemRequestBuilder(BaseRequestBuilder):
     """
     Builds and executes requests for operations under /api/run/{id}
     """
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
@@ -169,23 +168,14 @@
         """
         The updateAccess property
         """
         from .update_access.update_access_request_builder import UpdateAccessRequestBuilder
 
         return UpdateAccessRequestBuilder(self.request_adapter, self.path_parameters)
     
-    @property
-    def waitfor_datasets(self) -> WaitforDatasetsRequestBuilder:
-        """
-        The waitforDatasets property
-        """
-        from .waitfor_datasets.waitfor_datasets_request_builder import WaitforDatasetsRequestBuilder
-
-        return WaitforDatasetsRequestBuilder(self.request_adapter, self.path_parameters)
-    
     @dataclass
     class RunItemRequestBuilderGetQueryParameters():
         """
         Get extended Run information by Run ID
         """
         # Run API token
         token: Optional[str] = None
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/schema/schema_post_response.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/schema/schema_post_response.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/schema/schema_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/schema/schema_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/summary/summary_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/summary/summary_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/trash/trash_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/trash/trash_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/update_access/update_access_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/item/update_access/update_access_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/item/waitfor_datasets/waitfor_datasets_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/export/export_request_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,54 +5,58 @@
 from kiota_abstractions.method import Method
 from kiota_abstractions.request_adapter import RequestAdapter
 from kiota_abstractions.request_information import RequestInformation
 from kiota_abstractions.request_option import RequestOption
 from kiota_abstractions.serialization import Parsable, ParsableFactory
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
-class WaitforDatasetsRequestBuilder(BaseRequestBuilder):
+if TYPE_CHECKING:
+    from .....models.test_export import TestExport
+
+class ExportRequestBuilder(BaseRequestBuilder):
     """
-    Builds and executes requests for operations under /api/run/{id}/waitforDatasets
+    Builds and executes requests for operations under /api/test/{id}/export
     """
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
-        Instantiates a new WaitforDatasetsRequestBuilder and sets the default values.
+        Instantiates a new ExportRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/run/{id}/waitforDatasets", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/export", path_parameters)
     
-    async def get(self,request_configuration: Optional[RequestConfiguration] = None) -> None:
+    async def get(self,request_configuration: Optional[RequestConfiguration] = None) -> Optional[TestExport]:
         """
-        Blocking call, waiting for datasets to be produced
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
-        Returns: None
+        Returns: Optional[TestExport]
         """
         request_info = self.to_get_request_information(
             request_configuration
         )
         if not self.request_adapter:
             raise Exception("Http core is null") 
-        return await self.request_adapter.send_no_response_content_async(request_info, None)
+        from .....models.test_export import TestExport
+
+        return await self.request_adapter.send_async(request_info, TestExport, None)
     
     def to_get_request_information(self,request_configuration: Optional[RequestConfiguration] = None) -> RequestInformation:
         """
-        Blocking call, waiting for datasets to be produced
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: RequestInformation
         """
         request_info = RequestInformation(Method.GET, self.url_template, self.path_parameters)
         request_info.configure(request_configuration)
+        request_info.headers.try_add("Accept", "application/json")
         return request_info
     
-    def with_url(self,raw_url: Optional[str] = None) -> WaitforDatasetsRequestBuilder:
+    def with_url(self,raw_url: Optional[str] = None) -> ExportRequestBuilder:
         """
         Returns a request builder with the provided arbitrary URL. Using this method means any other path or query parameters are ignored.
         param raw_url: The raw URL to use for the request builder.
-        Returns: WaitforDatasetsRequestBuilder
+        Returns: ExportRequestBuilder
         """
         if not raw_url:
             raise TypeError("raw_url cannot be null.")
-        return WaitforDatasetsRequestBuilder(self.request_adapter, raw_url)
+        return ExportRequestBuilder(self.request_adapter, raw_url)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/list_/item/with_test_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/list_/item/with_test_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/list_/list_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/list_/list_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/recalculate_all/recalculate_all_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/recalculate_all/recalculate_all_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/run_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/run_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/run/test/test_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/run/test/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/all_labels/all_labels_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/all_labels/all_labels_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/all_transformers/all_transformers_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/all_transformers/all_transformers_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/descriptors/descriptors_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/descriptors/descriptors_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/find_usages/find_usages_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/find_usages/find_usages_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/id_by_uri/id_by_uri_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/id_by_uri/id_by_uri_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/id_by_uri/item/with_uri_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/id_by_uri/item/with_uri_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/import_/import_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/import_/import_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/drop_token/drop_token_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/drop_token/drop_token_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/export/export_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/export/export_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/id_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/id_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/labels/item/with_label_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/labels/item/with_label_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/labels/labels_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/labels/labels_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/reset_token/reset_token_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/reset_token/reset_token_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/transformers/item/with_transformer_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/transformers/item/with_transformer_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/transformers/transformers_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/transformers/transformers_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/item/update_access/update_access_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/item/update_access/update_access_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/schema/schema_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/schema/schema_request_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
         Instantiates a new SchemaRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/schema{?direction*,limit*,page*,sort*}", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/schema{?direction*,limit*,page*,roles*,sort*}", path_parameters)
     
     def by_id_id(self,id_id: int) -> IdItemRequestBuilder:
         """
         Gets an item from the raw_client.api.schema.item collection
         param id_id: Schema ID to retrieve
         Returns: IdItemRequestBuilder
         """
@@ -180,12 +180,15 @@
 
         # limit the number of results
         limit: Optional[int] = None
 
         # filter by page number of a paginated list of Schemas
         page: Optional[int] = None
 
+        # __my, __all or a comma delimited  list of roles
+        roles: Optional[str] = None
+
         # Field name to sort results
         sort: Optional[str] = None
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/by_name/by_name_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/by_name/by_name_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/by_name/item/with_name_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/by_name/item/with_name_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/folders/folders_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/folders/folders_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/import_/import_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/import_/import_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/add_token/add_token_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/add_token/add_token_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/export/export_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/move/move_request_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 from __future__ import annotations
+from dataclasses import dataclass, field
 from kiota_abstractions.base_request_builder import BaseRequestBuilder
 from kiota_abstractions.base_request_configuration import RequestConfiguration
 from kiota_abstractions.get_path_parameters import get_path_parameters
 from kiota_abstractions.method import Method
 from kiota_abstractions.request_adapter import RequestAdapter
 from kiota_abstractions.request_information import RequestInformation
 from kiota_abstractions.request_option import RequestOption
 from kiota_abstractions.serialization import Parsable, ParsableFactory
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
-if TYPE_CHECKING:
-    from .....models.test_export import TestExport
-
-class ExportRequestBuilder(BaseRequestBuilder):
+class MoveRequestBuilder(BaseRequestBuilder):
     """
-    Builds and executes requests for operations under /api/test/{id}/export
+    Builds and executes requests for operations under /api/test/{id}/move
     """
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
-        Instantiates a new ExportRequestBuilder and sets the default values.
+        Instantiates a new MoveRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/export", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/move{?folder*}", path_parameters)
     
-    async def get(self,request_configuration: Optional[RequestConfiguration] = None) -> Optional[TestExport]:
+    async def post(self,request_configuration: Optional[RequestConfiguration] = None) -> None:
         """
+        Update the folder for a Test. Tests can be moved to different folders
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
-        Returns: Optional[TestExport]
+        Returns: None
         """
-        request_info = self.to_get_request_information(
+        request_info = self.to_post_request_information(
             request_configuration
         )
         if not self.request_adapter:
             raise Exception("Http core is null") 
-        from .....models.test_export import TestExport
-
-        return await self.request_adapter.send_async(request_info, TestExport, None)
+        return await self.request_adapter.send_no_response_content_async(request_info, None)
     
-    def to_get_request_information(self,request_configuration: Optional[RequestConfiguration] = None) -> RequestInformation:
+    def to_post_request_information(self,request_configuration: Optional[RequestConfiguration] = None) -> RequestInformation:
         """
+        Update the folder for a Test. Tests can be moved to different folders
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: RequestInformation
         """
-        request_info = RequestInformation(Method.GET, self.url_template, self.path_parameters)
+        request_info = RequestInformation(Method.POST, self.url_template, self.path_parameters)
         request_info.configure(request_configuration)
-        request_info.headers.try_add("Accept", "application/json")
         return request_info
     
-    def with_url(self,raw_url: Optional[str] = None) -> ExportRequestBuilder:
+    def with_url(self,raw_url: Optional[str] = None) -> MoveRequestBuilder:
         """
         Returns a request builder with the provided arbitrary URL. Using this method means any other path or query parameters are ignored.
         param raw_url: The raw URL to use for the request builder.
-        Returns: ExportRequestBuilder
+        Returns: MoveRequestBuilder
         """
         if not raw_url:
             raise TypeError("raw_url cannot be null.")
-        return ExportRequestBuilder(self.request_adapter, raw_url)
+        return MoveRequestBuilder(self.request_adapter, raw_url)
+    
+    @dataclass
+    class MoveRequestBuilderPostQueryParameters():
+        """
+        Update the folder for a Test. Tests can be moved to different folders
+        """
+        # New folder to store the tests
+        folder: Optional[str] = None
+
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/fingerprint/fingerprint_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/fingerprint/fingerprint_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/label_values/label_values_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/label_values/label_values_request_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
         Instantiates a new LabelValuesRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/labelValues{?after*,before*,direction*,filter*,filtering*,limit*,metrics*,page*,sort*}", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/labelValues{?after*,before*,direction*,exclude*,filter*,filtering*,include*,limit*,metrics*,page*,sort*}", path_parameters)
     
     async def get(self,request_configuration: Optional[RequestConfiguration] = None) -> Optional[List[ExportedLabelValues]]:
         """
         List all Label Values for a Test
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: Optional[List[ExportedLabelValues]]
         """
@@ -72,20 +72,26 @@
 
         # ISO-like date time string or epoch millis
         before: Optional[str] = None
 
         # either Ascending or Descending
         direction: Optional[str] = None
 
+        # label name(s) to exclude from the result as scalar or comma separated
+        exclude: Optional[List[str]] = None
+
         # either a required json sub-document or path expression
         filter: Optional[str] = None
 
         # Retrieve values for Filtering Labels
         filtering: Optional[bool] = None
 
+        # label name(s) to include in the result as scalar or comma separated
+        include: Optional[List[str]] = None
+
         # the maximum number of results to include
         limit: Optional[int] = None
 
         # Retrieve values for Metric Labels
         metrics: Optional[bool] = None
 
         # which page to skip to when using a limit
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/move/move_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/update_access/update_access_request_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,63 +6,69 @@
 from kiota_abstractions.method import Method
 from kiota_abstractions.request_adapter import RequestAdapter
 from kiota_abstractions.request_information import RequestInformation
 from kiota_abstractions.request_option import RequestOption
 from kiota_abstractions.serialization import Parsable, ParsableFactory
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
-class MoveRequestBuilder(BaseRequestBuilder):
+if TYPE_CHECKING:
+    from .....models.access import Access
+
+class UpdateAccessRequestBuilder(BaseRequestBuilder):
     """
-    Builds and executes requests for operations under /api/test/{id}/move
+    Builds and executes requests for operations under /api/test/{id}/updateAccess
     """
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
-        Instantiates a new MoveRequestBuilder and sets the default values.
+        Instantiates a new UpdateAccessRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/move{?folder*}", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/updateAccess?access={access}&owner={owner}", path_parameters)
     
     async def post(self,request_configuration: Optional[RequestConfiguration] = None) -> None:
         """
-        Update the folder for a Test. Tests can be moved to different folders
+        Update the Access configuration for a Test
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: None
         """
         request_info = self.to_post_request_information(
             request_configuration
         )
         if not self.request_adapter:
             raise Exception("Http core is null") 
         return await self.request_adapter.send_no_response_content_async(request_info, None)
     
     def to_post_request_information(self,request_configuration: Optional[RequestConfiguration] = None) -> RequestInformation:
         """
-        Update the folder for a Test. Tests can be moved to different folders
+        Update the Access configuration for a Test
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: RequestInformation
         """
         request_info = RequestInformation(Method.POST, self.url_template, self.path_parameters)
         request_info.configure(request_configuration)
         return request_info
     
-    def with_url(self,raw_url: Optional[str] = None) -> MoveRequestBuilder:
+    def with_url(self,raw_url: Optional[str] = None) -> UpdateAccessRequestBuilder:
         """
         Returns a request builder with the provided arbitrary URL. Using this method means any other path or query parameters are ignored.
         param raw_url: The raw URL to use for the request builder.
-        Returns: MoveRequestBuilder
+        Returns: UpdateAccessRequestBuilder
         """
         if not raw_url:
             raise TypeError("raw_url cannot be null.")
-        return MoveRequestBuilder(self.request_adapter, raw_url)
+        return UpdateAccessRequestBuilder(self.request_adapter, raw_url)
     
     @dataclass
-    class MoveRequestBuilderPostQueryParameters():
+    class UpdateAccessRequestBuilderPostQueryParameters():
         """
-        Update the folder for a Test. Tests can be moved to different folders
+        Update the Access configuration for a Test
         """
-        # New folder to store the tests
-        folder: Optional[str] = None
+        # New Access level for the Test
+        access: Optional[Access] = None
+
+        # Name of the new owner
+        owner: Optional[str] = None
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/notifications/notifications_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/notifications/notifications_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/recalculate/recalculate_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/recalculate/recalculate_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/revoke_token/item/with_token_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/revoke_token/item/with_token_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/revoke_token/revoke_token_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/revoke_token/revoke_token_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/test_item_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/test_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/tokens/tokens_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/tokens/tokens_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/transformers/transformers_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/item/transformers/transformers_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/item/update_access/update_access_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/summary/summary_request_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,68 +7,80 @@
 from kiota_abstractions.request_adapter import RequestAdapter
 from kiota_abstractions.request_information import RequestInformation
 from kiota_abstractions.request_option import RequestOption
 from kiota_abstractions.serialization import Parsable, ParsableFactory
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
-    from .....models.access import Access
+    from ....models.test_listing import TestListing
 
-class UpdateAccessRequestBuilder(BaseRequestBuilder):
+class SummaryRequestBuilder(BaseRequestBuilder):
     """
-    Builds and executes requests for operations under /api/test/{id}/updateAccess
+    Builds and executes requests for operations under /api/test/summary
     """
     def __init__(self,request_adapter: RequestAdapter, path_parameters: Union[str, Dict[str, Any]]) -> None:
         """
-        Instantiates a new UpdateAccessRequestBuilder and sets the default values.
+        Instantiates a new SummaryRequestBuilder and sets the default values.
         param path_parameters: The raw url or the url-template parameters for the request.
         param request_adapter: The request adapter to use to execute the requests.
         Returns: None
         """
-        super().__init__(request_adapter, "{+baseurl}/api/test/{id}/updateAccess?access={access}&owner={owner}", path_parameters)
+        super().__init__(request_adapter, "{+baseurl}/api/test/summary{?direction*,folder*,limit*,page*,roles*}", path_parameters)
     
-    async def post(self,request_configuration: Optional[RequestConfiguration] = None) -> None:
+    async def get(self,request_configuration: Optional[RequestConfiguration] = None) -> Optional[TestListing]:
         """
-        Update the Access configuration for a Test
+        Retrieve a summary of Tests in a folder
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
-        Returns: None
+        Returns: Optional[TestListing]
         """
-        request_info = self.to_post_request_information(
+        request_info = self.to_get_request_information(
             request_configuration
         )
         if not self.request_adapter:
             raise Exception("Http core is null") 
-        return await self.request_adapter.send_no_response_content_async(request_info, None)
+        from ....models.test_listing import TestListing
+
+        return await self.request_adapter.send_async(request_info, TestListing, None)
     
-    def to_post_request_information(self,request_configuration: Optional[RequestConfiguration] = None) -> RequestInformation:
+    def to_get_request_information(self,request_configuration: Optional[RequestConfiguration] = None) -> RequestInformation:
         """
-        Update the Access configuration for a Test
+        Retrieve a summary of Tests in a folder
         param request_configuration: Configuration for the request such as headers, query parameters, and middleware options.
         Returns: RequestInformation
         """
-        request_info = RequestInformation(Method.POST, self.url_template, self.path_parameters)
+        request_info = RequestInformation(Method.GET, self.url_template, self.path_parameters)
         request_info.configure(request_configuration)
+        request_info.headers.try_add("Accept", "application/json")
         return request_info
     
-    def with_url(self,raw_url: Optional[str] = None) -> UpdateAccessRequestBuilder:
+    def with_url(self,raw_url: Optional[str] = None) -> SummaryRequestBuilder:
         """
         Returns a request builder with the provided arbitrary URL. Using this method means any other path or query parameters are ignored.
         param raw_url: The raw URL to use for the request builder.
-        Returns: UpdateAccessRequestBuilder
+        Returns: SummaryRequestBuilder
         """
         if not raw_url:
             raise TypeError("raw_url cannot be null.")
-        return UpdateAccessRequestBuilder(self.request_adapter, raw_url)
+        return SummaryRequestBuilder(self.request_adapter, raw_url)
     
     @dataclass
-    class UpdateAccessRequestBuilderPostQueryParameters():
+    class SummaryRequestBuilderGetQueryParameters():
         """
-        Update the Access configuration for a Test
+        Retrieve a summary of Tests in a folder
         """
-        # New Access level for the Test
-        access: Optional[Access] = None
+        # Sort direction
+        direction: Optional[str] = None
+
+        # name of the Folder containing the Tests
+        folder: Optional[str] = None
+
+        # limit the result count
+        limit: Optional[int] = None
+
+        # filter by page number of a paginated list of 
+        page: Optional[int] = None
 
-        # Name of the new owner
-        owner: Optional[str] = None
+        # "__my", "__all" or a comma delimited  list of roles
+        roles: Optional[str] = None
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/api/test/test_request_builder.py` & `horreum-0.13/src/horreum/raw_client/api/test/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/horreum_raw_client.py` & `horreum-0.13/src/horreum/raw_client/horreum_raw_client.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/kiota-lock.json` & `horreum-0.13/src/horreum/raw_client/kiota-lock.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'descriptionHash'": "'E6B1D4A957DE5BD9E4B7EF3C189A3A049D4E5D86A3ED14E33067FA8DCEA37E0DCB472625852B412F62CF32B3E38DC69A01F3537143274C6D1706BDCBEC74FB44'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "clientClassName": "HorreumRawClient",
     "clientNamespaceName": "raw_client",
-    "descriptionHash": "E3279E397B98AEE69A674E70E9F128655714D4C4CAE34DB1E2D459A7B751CDA8BE3350DA110AF4901889F39E54F6922F806D3C58362553F7A3048C6EAE3B1E8C",
+    "descriptionHash": "E6B1D4A957DE5BD9E4B7EF3C189A3A049D4E5D86A3ED14E33067FA8DCEA37E0DCB472625852B412F62CF32B3E38DC69A01F3537143274C6D1706BDCBEC74FB44",
     "descriptionLocation": "../../../openapi/openapi.yaml",
     "deserializers": [
         "Microsoft.Kiota.Serialization.Json.JsonParseNodeFactory",
         "Microsoft.Kiota.Serialization.Text.TextParseNodeFactory",
         "Microsoft.Kiota.Serialization.Form.FormParseNodeFactory"
     ],
     "disabledValidationRules": [],
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/action.py` & `horreum-0.13/src/horreum/raw_client/models/datastore.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,146 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
-    from .action_config import Action_config
-    from .action_secrets import Action_secrets
-    from .github_issue_comment_action import GithubIssueCommentAction
-    from .github_issue_create_action import GithubIssueCreateAction
-    from .http_action import HttpAction
+    from .datastore_access import Datastore_access
+    from .datastore_config import Datastore_config
+    from .datastore_type import Datastore_type
+    from .elasticsearch_datastore_config import ElasticsearchDatastoreConfig
+    from .postgres_datastore_config import PostgresDatastoreConfig
 
 @dataclass
-class Action(AdditionalDataHolder, Parsable):
+class Datastore(AdditionalDataHolder, Parsable):
+    """
+    Type of backend datastore
+    """
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # The active property
-    active: Optional[bool] = None
+    # Access rights for the test. This defines the visibility of the Test in the UI
+    access: Optional[Datastore_access] = None
+    # Is this a built-in datastore? Built-in datastores cannot be deleted or modified
+    built_in: Optional[bool] = None
     # The config property
-    config: Optional[Action_config] = None
-    # The event property
-    event: Optional[str] = None
-    # The id property
+    config: Optional[Datastore_config] = None
+    # Unique Datastore id
     id: Optional[int] = None
-    # The runAlways property
-    run_always: Optional[bool] = None
-    # The secrets property
-    secrets: Optional[Action_secrets] = None
-    # The testId property
-    test_id: Optional[int] = None
-    # The type property
-    type: Optional[str] = None
+    # Name of the datastore, used to identify the datastore in the Test definition
+    name: Optional[str] = None
+    # Name of the team that owns the test. Users must belong to the team that owns a test to make modifications
+    owner: Optional[str] = None
+    # Type of backend datastore
+    type: Optional[Datastore_type] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> Action:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> Datastore:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: Action
+        Returns: Datastore
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return Action()
+        return Datastore()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
-        from .action_config import Action_config
-        from .action_secrets import Action_secrets
-        from .github_issue_comment_action import GithubIssueCommentAction
-        from .github_issue_create_action import GithubIssueCreateAction
-        from .http_action import HttpAction
-
-        from .action_config import Action_config
-        from .action_secrets import Action_secrets
-        from .github_issue_comment_action import GithubIssueCommentAction
-        from .github_issue_create_action import GithubIssueCreateAction
-        from .http_action import HttpAction
+        from .datastore_access import Datastore_access
+        from .datastore_config import Datastore_config
+        from .datastore_type import Datastore_type
+        from .elasticsearch_datastore_config import ElasticsearchDatastoreConfig
+        from .postgres_datastore_config import PostgresDatastoreConfig
+
+        from .datastore_access import Datastore_access
+        from .datastore_config import Datastore_config
+        from .datastore_type import Datastore_type
+        from .elasticsearch_datastore_config import ElasticsearchDatastoreConfig
+        from .postgres_datastore_config import PostgresDatastoreConfig
 
         fields: Dict[str, Callable[[Any], None]] = {
-            "active": lambda n : setattr(self, 'active', n.get_bool_value()),
-            "config": lambda n : setattr(self, 'config', n.get_object_value(Action_config)),
-            "event": lambda n : setattr(self, 'event', n.get_str_value()),
+            "access": lambda n : setattr(self, 'access', n.get_enum_value(Datastore_access)),
+            "builtIn": lambda n : setattr(self, 'built_in', n.get_bool_value()),
+            "config": lambda n : setattr(self, 'config', n.get_object_value(Datastore_config)),
             "id": lambda n : setattr(self, 'id', n.get_int_value()),
-            "runAlways": lambda n : setattr(self, 'run_always', n.get_bool_value()),
-            "secrets": lambda n : setattr(self, 'secrets', n.get_object_value(Action_secrets)),
-            "testId": lambda n : setattr(self, 'test_id', n.get_int_value()),
-            "type": lambda n : setattr(self, 'type', n.get_str_value()),
+            "name": lambda n : setattr(self, 'name', n.get_str_value()),
+            "owner": lambda n : setattr(self, 'owner', n.get_str_value()),
+            "type": lambda n : setattr(self, 'type', n.get_enum_value(Datastore_type)),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_bool_value("active", self.active)
+        writer.write_enum_value("access", self.access)
+        writer.write_bool_value("builtIn", self.built_in)
         writer.write_object_value("config", self.config)
-        writer.write_str_value("event", self.event)
         writer.write_int_value("id", self.id)
-        writer.write_bool_value("runAlways", self.run_always)
-        writer.write_object_value("secrets", self.secrets)
-        writer.write_int_value("testId", self.test_id)
-        writer.write_str_value("type", self.type)
+        writer.write_str_value("name", self.name)
+        writer.write_str_value("owner", self.owner)
+        writer.write_enum_value("type", self.type)
         writer.write_additional_data_value(self.additional_data)
     
     from kiota_abstractions.serialization import ComposedTypeWrapper
 
     @dataclass
-    class Action_config(ComposedTypeWrapper, Parsable):
+    class Datastore_config(ComposedTypeWrapper, Parsable):
         from kiota_abstractions.serialization import ComposedTypeWrapper
 
         """
-        Composed type wrapper for classes GithubIssueCommentAction, GithubIssueCreateAction, HttpAction
+        Composed type wrapper for classes ElasticsearchDatastoreConfig, PostgresDatastoreConfig
         """
         @staticmethod
-        def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> Action_config:
+        def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> Datastore_config:
             """
             Creates a new instance of the appropriate class based on discriminator value
             param parse_node: The parse node to use to read the discriminator value and create the object
-            Returns: Action_config
+            Returns: Datastore_config
             """
             if not parse_node:
                 raise TypeError("parse_node cannot be null.")
             try:
                 mapping_value = parse_node.get_child_node("").get_str_value()
             except AttributeError:
                 mapping_value = None
-            result = Action_config()
-            if mapping_value and mapping_value.casefold() == "GithubIssueCommentAction".casefold():
-                result.github_issue_comment_action = GithubIssueCommentAction()
-            elif mapping_value and mapping_value.casefold() == "GithubIssueCreateAction".casefold():
-                result.github_issue_create_action = GithubIssueCreateAction()
-            elif mapping_value and mapping_value.casefold() == "HttpAction".casefold():
-                result.http_action = HttpAction()
+            result = Datastore_config()
+            if mapping_value and mapping_value.casefold() == "ElasticsearchDatastoreConfig".casefold():
+                result.elasticsearch_datastore_config = ElasticsearchDatastoreConfig()
+            elif mapping_value and mapping_value.casefold() == "PostgresDatastoreConfig".casefold():
+                result.postgres_datastore_config = PostgresDatastoreConfig()
             return result
         
         def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
             """
             The deserialization information for the current model
             Returns: Dict[str, Callable[[ParseNode], None]]
             """
-            if self.github_issue_comment_action:
-                return self.github_issue_comment_action.get_field_deserializers()
-            if self.github_issue_create_action:
-                return self.github_issue_create_action.get_field_deserializers()
-            if self.http_action:
-                return self.http_action.get_field_deserializers()
+            if self.elasticsearch_datastore_config:
+                return self.elasticsearch_datastore_config.get_field_deserializers()
+            if self.postgres_datastore_config:
+                return self.postgres_datastore_config.get_field_deserializers()
             return {}
         
         def serialize(self,writer: SerializationWriter) -> None:
             """
             Serializes information the current object
             param writer: Serialization writer to use to serialize this model
             Returns: None
             """
             if not writer:
                 raise TypeError("writer cannot be null.")
-            if self.github_issue_comment_action:
-                writer.write_object_value(None, self.github_issue_comment_action)
-            elif self.github_issue_create_action:
-                writer.write_object_value(None, self.github_issue_create_action)
-            elif self.http_action:
-                writer.write_object_value(None, self.http_action)
+            if self.elasticsearch_datastore_config:
+                writer.write_object_value(None, self.elasticsearch_datastore_config)
+            elif self.postgres_datastore_config:
+                writer.write_object_value(None, self.postgres_datastore_config)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/action_secrets.py` & `horreum-0.13/src/horreum/raw_client/models/action_secrets.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/change_detection.py` & `horreum-0.13/src/horreum/raw_client/models/change_detection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from .change_detection_config import ChangeDetection_config
+    from .e_divisive_detection_config import EDivisiveDetectionConfig
     from .fixed_threshold_detection_config import FixedThresholdDetectionConfig
     from .relative_difference_detection_config import RelativeDifferenceDetectionConfig
 
 @dataclass
 class ChangeDetection(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
@@ -33,18 +34,20 @@
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         from .change_detection_config import ChangeDetection_config
+        from .e_divisive_detection_config import EDivisiveDetectionConfig
         from .fixed_threshold_detection_config import FixedThresholdDetectionConfig
         from .relative_difference_detection_config import RelativeDifferenceDetectionConfig
 
         from .change_detection_config import ChangeDetection_config
+        from .e_divisive_detection_config import EDivisiveDetectionConfig
         from .fixed_threshold_detection_config import FixedThresholdDetectionConfig
         from .relative_difference_detection_config import RelativeDifferenceDetectionConfig
 
         fields: Dict[str, Callable[[Any], None]] = {
             "config": lambda n : setattr(self, 'config', n.get_object_value(ChangeDetection_config)),
             "id": lambda n : setattr(self, 'id', n.get_int_value()),
             "model": lambda n : setattr(self, 'model', n.get_str_value()),
@@ -67,19 +70,20 @@
     from kiota_abstractions.serialization import ComposedTypeWrapper
 
     @dataclass
     class ChangeDetection_config(ComposedTypeWrapper, Parsable):
         from kiota_abstractions.serialization import ComposedTypeWrapper
 
         if TYPE_CHECKING:
+            from .e_divisive_detection_config import EDivisiveDetectionConfig
             from .fixed_threshold_detection_config import FixedThresholdDetectionConfig
             from .relative_difference_detection_config import RelativeDifferenceDetectionConfig
 
         """
-        Composed type wrapper for classes FixedThresholdDetectionConfig, RelativeDifferenceDetectionConfig
+        Composed type wrapper for classes EDivisiveDetectionConfig, FixedThresholdDetectionConfig, RelativeDifferenceDetectionConfig
         """
         @staticmethod
         def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> ChangeDetection_config:
             """
             Creates a new instance of the appropriate class based on discriminator value
             param parse_node: The parse node to use to read the discriminator value and create the object
             Returns: ChangeDetection_config
@@ -87,46 +91,55 @@
             if not parse_node:
                 raise TypeError("parse_node cannot be null.")
             try:
                 mapping_value = parse_node.get_child_node("model").get_str_value()
             except AttributeError:
                 mapping_value = None
             result = ChangeDetection_config()
-            if mapping_value and mapping_value.casefold() == "fixedThreshold".casefold():
+            if mapping_value and mapping_value.casefold() == "eDivisive".casefold():
+                from .e_divisive_detection_config import EDivisiveDetectionConfig
+
+                result.e_divisive_detection_config = EDivisiveDetectionConfig()
+            elif mapping_value and mapping_value.casefold() == "fixedThreshold".casefold():
                 from .fixed_threshold_detection_config import FixedThresholdDetectionConfig
 
                 result.fixed_threshold_detection_config = FixedThresholdDetectionConfig()
             elif mapping_value and mapping_value.casefold() == "relativeDifference".casefold():
                 from .relative_difference_detection_config import RelativeDifferenceDetectionConfig
 
                 result.relative_difference_detection_config = RelativeDifferenceDetectionConfig()
             return result
         
         def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
             """
             The deserialization information for the current model
             Returns: Dict[str, Callable[[ParseNode], None]]
             """
+            from .e_divisive_detection_config import EDivisiveDetectionConfig
             from .fixed_threshold_detection_config import FixedThresholdDetectionConfig
             from .relative_difference_detection_config import RelativeDifferenceDetectionConfig
 
+            if self.e_divisive_detection_config:
+                return self.e_divisive_detection_config.get_field_deserializers()
             if self.fixed_threshold_detection_config:
                 return self.fixed_threshold_detection_config.get_field_deserializers()
             if self.relative_difference_detection_config:
                 return self.relative_difference_detection_config.get_field_deserializers()
             return {}
         
         def serialize(self,writer: SerializationWriter) -> None:
             """
             Serializes information the current object
             param writer: Serialization writer to use to serialize this model
             Returns: None
             """
             if not writer:
                 raise TypeError("writer cannot be null.")
-            if self.fixed_threshold_detection_config:
+            if self.e_divisive_detection_config:
+                writer.write_object_value(None, self.e_divisive_detection_config)
+            elif self.fixed_threshold_detection_config:
                 writer.write_object_value(None, self.fixed_threshold_detection_config)
             elif self.relative_difference_detection_config:
                 writer.write_object_value(None, self.relative_difference_detection_config)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/condition_component.py` & `horreum-0.13/src/horreum/raw_client/models/condition_component.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/condition_component_properties.py` & `horreum-0.13/src/horreum/raw_client/models/condition_component_properties.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/condition_component_type.py` & `horreum-0.13/src/horreum/raw_client/models/condition_component_type.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/condition_config.py` & `horreum-0.13/src/horreum/raw_client/models/condition_config.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/condition_config_defaults.py` & `horreum-0.13/src/horreum/raw_client/models/condition_config_defaults.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/dataset.py` & `horreum-0.13/src/horreum/raw_client/models/dataset.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/dataset_info.py` & `horreum-0.13/src/horreum/raw_client/models/dataset_info.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/dataset_list.py` & `horreum-0.13/src/horreum/raw_client/models/dataset_list.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/dataset_log.py` & `horreum-0.13/src/horreum/raw_client/models/dataset_log.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/dataset_summary.py` & `horreum-0.13/src/horreum/raw_client/models/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/dataset_summary_view.py` & `horreum-0.13/src/horreum/raw_client/models/dataset_summary_view.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/datastore_test_response.py` & `horreum-0.13/src/horreum/raw_client/models/datastore_test_response.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/elasticsearch_datastore_config.py` & `horreum-0.13/src/horreum/raw_client/models/elasticsearch_datastore_config.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/error_details.py` & `horreum-0.13/src/horreum/raw_client/models/error_details.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/experiment_comparison.py` & `horreum-0.13/src/horreum/raw_client/models/experiment_comparison.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/experiment_profile.py` & `horreum-0.13/src/horreum/raw_client/models/experiment_profile.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/experiment_result.py` & `horreum-0.13/src/horreum/raw_client/models/experiment_result.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/experiment_result_dataset_info.py` & `horreum-0.13/src/horreum/raw_client/models/experiment_result_dataset_info.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/experiment_result_profile.py` & `horreum-0.13/src/horreum/raw_client/models/experiment_result_profile.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/experiment_result_results.py` & `horreum-0.13/src/horreum/raw_client/models/experiment_result_results.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/exported_label_values.py` & `horreum-0.13/src/horreum/raw_client/models/exported_label_values.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/extractor.py` & `horreum-0.13/src/horreum/raw_client/models/extractor.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/fingerprint_value.py` & `horreum-0.13/src/horreum/raw_client/models/fingerprint_value.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/fingerprints.py` & `horreum-0.13/src/horreum/raw_client/models/fingerprints.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/fix_threshold_config.py` & `horreum-0.13/src/horreum/raw_client/models/fix_threshold_config.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/fixed_threshold_detection_config.py` & `horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from .fixed_threshold_detection_config_max import FixedThresholdDetectionConfig_max
     from .fixed_threshold_detection_config_min import FixedThresholdDetectionConfig_min
+    from .fixed_threshold_detection_config_model import FixedThresholdDetectionConfig_model
 
 @dataclass
 class FixedThresholdDetectionConfig(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
     # Built In
     built_in: Optional[bool] = None
     # Upper bound for acceptable datapoint values
     max: Optional[FixedThresholdDetectionConfig_max] = None
     # Lower bound for acceptable datapoint values
     min: Optional[FixedThresholdDetectionConfig_min] = None
+    # The model property
+    model: Optional[FixedThresholdDetectionConfig_model] = None
     
     @staticmethod
     def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> FixedThresholdDetectionConfig:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
         Returns: FixedThresholdDetectionConfig
@@ -33,32 +36,36 @@
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         from .fixed_threshold_detection_config_max import FixedThresholdDetectionConfig_max
         from .fixed_threshold_detection_config_min import FixedThresholdDetectionConfig_min
+        from .fixed_threshold_detection_config_model import FixedThresholdDetectionConfig_model
 
         from .fixed_threshold_detection_config_max import FixedThresholdDetectionConfig_max
         from .fixed_threshold_detection_config_min import FixedThresholdDetectionConfig_min
+        from .fixed_threshold_detection_config_model import FixedThresholdDetectionConfig_model
 
         fields: Dict[str, Callable[[Any], None]] = {
             "builtIn": lambda n : setattr(self, 'built_in', n.get_bool_value()),
             "max": lambda n : setattr(self, 'max', n.get_object_value(FixedThresholdDetectionConfig_max)),
             "min": lambda n : setattr(self, 'min', n.get_object_value(FixedThresholdDetectionConfig_min)),
+            "model": lambda n : setattr(self, 'model', n.get_enum_value(FixedThresholdDetectionConfig_model)),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
         writer.write_bool_value("builtIn", self.built_in)
         writer.write_object_value("max", self.max)
         writer.write_object_value("min", self.min)
+        writer.write_enum_value("model", self.model)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/fixed_threshold_detection_config_max.py` & `horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config_max.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/fixed_threshold_detection_config_min.py` & `horreum-0.13/src/horreum/raw_client/models/fixed_threshold_detection_config_min.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/github_issue_comment_action.py` & `horreum-0.13/src/horreum/raw_client/models/persistent_log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from __future__ import annotations
+import datetime
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class GithubIssueCommentAction(AdditionalDataHolder, Parsable):
+class PersistentLog(AdditionalDataHolder, Parsable):
+    """
+    Persistent Log
+    """
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # The formatter property
-    formatter: Optional[str] = None
-    # The issue property
-    issue: Optional[str] = None
-    # The issueUrl property
-    issue_url: Optional[str] = None
-    # The owner property
-    owner: Optional[str] = None
-    # The repo property
-    repo: Optional[str] = None
+    # The id property
+    id: Optional[int] = None
+    # The level property
+    level: Optional[int] = None
+    # The message property
+    message: Optional[str] = None
+    # The timestamp property
+    timestamp: Optional[datetime.datetime] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> GithubIssueCommentAction:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> PersistentLog:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: GithubIssueCommentAction
+        Returns: PersistentLog
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return GithubIssueCommentAction()
+        return PersistentLog()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "formatter": lambda n : setattr(self, 'formatter', n.get_str_value()),
-            "issue": lambda n : setattr(self, 'issue', n.get_str_value()),
-            "issueUrl": lambda n : setattr(self, 'issue_url', n.get_str_value()),
-            "owner": lambda n : setattr(self, 'owner', n.get_str_value()),
-            "repo": lambda n : setattr(self, 'repo', n.get_str_value()),
+            "id": lambda n : setattr(self, 'id', n.get_int_value()),
+            "level": lambda n : setattr(self, 'level', n.get_int_value()),
+            "message": lambda n : setattr(self, 'message', n.get_str_value()),
+            "timestamp": lambda n : setattr(self, 'timestamp', n.get_datetime_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_str_value("formatter", self.formatter)
-        writer.write_str_value("issue", self.issue)
-        writer.write_str_value("issueUrl", self.issue_url)
-        writer.write_str_value("owner", self.owner)
-        writer.write_str_value("repo", self.repo)
+        writer.write_int_value("id", self.id)
+        writer.write_int_value("level", self.level)
+        writer.write_str_value("message", self.message)
+        writer.write_datetime_value("timestamp", self.timestamp)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/github_issue_create_action.py` & `horreum-0.13/src/horreum/raw_client/models/label_location.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class GithubIssueCreateAction(AdditionalDataHolder, Parsable):
+class LabelLocation(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # The formatter property
-    formatter: Optional[str] = None
-    # The owner property
-    owner: Optional[str] = None
-    # The repo property
-    repo: Optional[str] = None
-    # The title property
-    title: Optional[str] = None
+    # Unique ID for location that references Schema
+    test_id: Optional[int] = None
+    # Test name that references Schema
+    test_name: Optional[str] = None
+    # Location of Label usage
+    type: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> GithubIssueCreateAction:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> LabelLocation:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: GithubIssueCreateAction
+        Returns: LabelLocation
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return GithubIssueCreateAction()
+        return LabelLocation()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "formatter": lambda n : setattr(self, 'formatter', n.get_str_value()),
-            "owner": lambda n : setattr(self, 'owner', n.get_str_value()),
-            "repo": lambda n : setattr(self, 'repo', n.get_str_value()),
-            "title": lambda n : setattr(self, 'title', n.get_str_value()),
+            "testId": lambda n : setattr(self, 'test_id', n.get_int_value()),
+            "testName": lambda n : setattr(self, 'test_name', n.get_str_value()),
+            "type": lambda n : setattr(self, 'type', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_str_value("formatter", self.formatter)
-        writer.write_str_value("owner", self.owner)
-        writer.write_str_value("repo", self.repo)
-        writer.write_str_value("title", self.title)
+        writer.write_int_value("testId", self.test_id)
+        writer.write_str_value("testName", self.test_name)
+        writer.write_str_value("type", self.type)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/http_action.py` & `horreum-0.13/src/horreum/raw_client/models/http_action_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class HttpAction(AdditionalDataHolder, Parsable):
+class HttpActionConfig(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # The url property
+    # Action type
+    type: Optional[str] = None
+    # HTTP address
     url: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> HttpAction:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> HttpActionConfig:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: HttpAction
+        Returns: HttpActionConfig
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return HttpAction()
+        return HttpActionConfig()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
+            "type": lambda n : setattr(self, 'type', n.get_str_value()),
             "url": lambda n : setattr(self, 'url', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
+        writer.write_str_value("type", self.type)
         writer.write_str_value("url", self.url)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/indexed_label_value_map.py` & `horreum-0.13/src/horreum/raw_client/models/indexed_label_value_map.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/keycloak_config.py` & `horreum-0.13/src/horreum/raw_client/models/keycloak_config.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label.py` & `horreum-0.13/src/horreum/raw_client/models/label.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_in_fingerprint.py` & `horreum-0.13/src/horreum/raw_client/models/label_in_fingerprint.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_in_report.py` & `horreum-0.13/src/horreum/raw_client/models/label_in_report.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_in_rule.py` & `horreum-0.13/src/horreum/raw_client/models/label_in_rule.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_in_variable.py` & `horreum-0.13/src/horreum/raw_client/models/label_in_variable.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_in_view.py` & `horreum-0.13/src/horreum/raw_client/models/label_in_view.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_info.py` & `horreum-0.13/src/horreum/raw_client/models/label_info.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_location.py` & `horreum-0.13/src/horreum/raw_client/models/label_preview.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class LabelLocation(AdditionalDataHolder, Parsable):
+class LabelPreview(AdditionalDataHolder, Parsable):
+    """
+    Preview a Label Value derived from a Dataset Data. A preview allows users to apply a Label to a dataset and preview the Label Value result and processing errors in the UI
+    """
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Unique ID for location that references Schema
-    test_id: Optional[int] = None
-    # Test name that references Schema
-    test_name: Optional[str] = None
-    # Location of Label usage
-    type: Optional[str] = None
+    # Description of errors occurred attempting to generate Label Value Preview
+    output: Optional[str] = None
+    # Value value extracted from Dataset. This can be a scalar, array or JSON object
+    value: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> LabelLocation:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> LabelPreview:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: LabelLocation
+        Returns: LabelPreview
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return LabelLocation()
+        return LabelPreview()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "testId": lambda n : setattr(self, 'test_id', n.get_int_value()),
-            "testName": lambda n : setattr(self, 'test_name', n.get_str_value()),
-            "type": lambda n : setattr(self, 'type', n.get_str_value()),
+            "output": lambda n : setattr(self, 'output', n.get_str_value()),
+            "value": lambda n : setattr(self, 'value', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_int_value("testId", self.test_id)
-        writer.write_str_value("testName", self.test_name)
-        writer.write_str_value("type", self.type)
+        writer.write_str_value("output", self.output)
+        writer.write_str_value("value", self.value)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_preview.py` & `horreum-0.13/src/horreum/raw_client/models/postgres_datastore_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class LabelPreview(AdditionalDataHolder, Parsable):
+class PostgresDatastoreConfig(AdditionalDataHolder, Parsable):
     """
-    Preview a Label Value derived from a Dataset Data. A preview allows users to apply a Label to a dataset and preview the Label Value result and processing errors in the UI
+    Built in backend datastore
     """
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Description of errors occurred attempting to generate Label Value Preview
-    output: Optional[str] = None
-    # Value value extracted from Dataset. This can be a scalar, array or JSON object
-    value: Optional[str] = None
+    # Built In
+    built_in: Optional[bool] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> LabelPreview:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> PostgresDatastoreConfig:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: LabelPreview
+        Returns: PostgresDatastoreConfig
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return LabelPreview()
+        return PostgresDatastoreConfig()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "output": lambda n : setattr(self, 'output', n.get_str_value()),
-            "value": lambda n : setattr(self, 'value', n.get_str_value()),
+            "builtIn": lambda n : setattr(self, 'built_in', n.get_bool_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_str_value("output", self.output)
-        writer.write_str_value("value", self.value)
+        writer.write_bool_value("builtIn", self.built_in)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_value.py` & `horreum-0.13/src/horreum/raw_client/models/label_value.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_value_map.py` & `horreum-0.13/src/horreum/raw_client/models/label_value_map.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/label_value_schema.py` & `horreum-0.13/src/horreum/raw_client/models/label_value_schema.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/missing_data_rule.py` & `horreum-0.13/src/horreum/raw_client/models/missing_data_rule.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/persistent_log.py` & `horreum-0.13/src/horreum/raw_client/models/schema_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 from __future__ import annotations
-import datetime
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class PersistentLog(AdditionalDataHolder, Parsable):
-    """
-    Persistent Log
-    """
+class SchemaUsage(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # The id property
+    # Does schema have a JSON validation schema defined?
+    has_json_schema: Optional[bool] = None
+    # Schema unique ID
     id: Optional[int] = None
-    # The level property
-    level: Optional[int] = None
-    # The message property
-    message: Optional[str] = None
-    # The timestamp property
-    timestamp: Optional[datetime.datetime] = None
+    # Ordinal position of schema usage in Run/Dataset
+    key: Optional[str] = None
+    # Schema name
+    name: Optional[str] = None
+    # Source of schema usage, 0 is data, 1 is metadata. DataSets always use 0
+    source: Optional[int] = None
+    # Location of Schema Usage, 0 for Run, 1 for Dataset
+    type: Optional[int] = None
+    # Schema name
+    uri: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> PersistentLog:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> SchemaUsage:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: PersistentLog
+        Returns: SchemaUsage
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return PersistentLog()
+        return SchemaUsage()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
+            "hasJsonSchema": lambda n : setattr(self, 'has_json_schema', n.get_bool_value()),
             "id": lambda n : setattr(self, 'id', n.get_int_value()),
-            "level": lambda n : setattr(self, 'level', n.get_int_value()),
-            "message": lambda n : setattr(self, 'message', n.get_str_value()),
-            "timestamp": lambda n : setattr(self, 'timestamp', n.get_datetime_value()),
+            "key": lambda n : setattr(self, 'key', n.get_str_value()),
+            "name": lambda n : setattr(self, 'name', n.get_str_value()),
+            "source": lambda n : setattr(self, 'source', n.get_int_value()),
+            "type": lambda n : setattr(self, 'type', n.get_int_value()),
+            "uri": lambda n : setattr(self, 'uri', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
+        writer.write_bool_value("hasJsonSchema", self.has_json_schema)
         writer.write_int_value("id", self.id)
-        writer.write_int_value("level", self.level)
-        writer.write_str_value("message", self.message)
-        writer.write_datetime_value("timestamp", self.timestamp)
+        writer.write_str_value("key", self.key)
+        writer.write_str_value("name", self.name)
+        writer.write_int_value("source", self.source)
+        writer.write_int_value("type", self.type)
+        writer.write_str_value("uri", self.uri)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/postgres_datastore_config.py` & `horreum-0.13/src/horreum/raw_client/models/test_listing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
+if TYPE_CHECKING:
+    from .test_summary import TestSummary
+
 @dataclass
-class PostgresDatastoreConfig(AdditionalDataHolder, Parsable):
-    """
-    Built in backend datastore
-    """
+class TestListing(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Built In
-    built_in: Optional[bool] = None
+    # Number of tests when pagination is ignored
+    count: Optional[int] = None
+    # Array of Test Summaries
+    tests: Optional[List[TestSummary]] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> PostgresDatastoreConfig:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> TestListing:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: PostgresDatastoreConfig
+        Returns: TestListing
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return PostgresDatastoreConfig()
+        return TestListing()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
+        from .test_summary import TestSummary
+
+        from .test_summary import TestSummary
+
         fields: Dict[str, Callable[[Any], None]] = {
-            "builtIn": lambda n : setattr(self, 'built_in', n.get_bool_value()),
+            "count": lambda n : setattr(self, 'count', n.get_int_value()),
+            "tests": lambda n : setattr(self, 'tests', n.get_collection_of_object_values(TestSummary)),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_bool_value("builtIn", self.built_in)
+        writer.write_int_value("count", self.count)
+        writer.write_collection_of_object_values("tests", self.tests)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/protected_time_type.py` & `horreum-0.13/src/horreum/raw_client/models/protected_time_type.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/protected_type.py` & `horreum-0.13/src/horreum/raw_client/models/protected_type.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/recalculation_status.py` & `horreum-0.13/src/horreum/raw_client/models/recalculation_status.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/relative_difference_detection_config.py` & `horreum-0.13/src/horreum/raw_client/models/github_issue_comment_action_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class RelativeDifferenceDetectionConfig(AdditionalDataHolder, Parsable):
+class GithubIssueCommentActionConfig(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Built In
-    built_in: Optional[bool] = None
-    # Relative Difference Detection filter
-    filter: Optional[str] = None
-    # Minimal number of preceding datapoints
-    min_previous: Optional[int] = None
-    # Maximum difference between the aggregated value of last <window> datapoints and the mean of preceding values.
-    threshold: Optional[float] = None
-    # Number of most recent datapoints used for aggregating the value for comparison.
-    window: Optional[int] = None
+    # Object markdown formatter
+    formatter: Optional[str] = None
+    # GitHub issue number
+    issue: Optional[str] = None
+    # GitHub issue URL
+    issue_url: Optional[str] = None
+    # GitHub repo owner
+    owner: Optional[str] = None
+    # GitHub repo name
+    repo: Optional[str] = None
+    # Action type
+    type: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> RelativeDifferenceDetectionConfig:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> GithubIssueCommentActionConfig:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: RelativeDifferenceDetectionConfig
+        Returns: GithubIssueCommentActionConfig
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return RelativeDifferenceDetectionConfig()
+        return GithubIssueCommentActionConfig()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "builtIn": lambda n : setattr(self, 'built_in', n.get_bool_value()),
-            "filter": lambda n : setattr(self, 'filter', n.get_str_value()),
-            "minPrevious": lambda n : setattr(self, 'min_previous', n.get_int_value()),
-            "threshold": lambda n : setattr(self, 'threshold', n.get_float_value()),
-            "window": lambda n : setattr(self, 'window', n.get_int_value()),
+            "formatter": lambda n : setattr(self, 'formatter', n.get_str_value()),
+            "issue": lambda n : setattr(self, 'issue', n.get_str_value()),
+            "issueUrl": lambda n : setattr(self, 'issue_url', n.get_str_value()),
+            "owner": lambda n : setattr(self, 'owner', n.get_str_value()),
+            "repo": lambda n : setattr(self, 'repo', n.get_str_value()),
+            "type": lambda n : setattr(self, 'type', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_bool_value("builtIn", self.built_in)
-        writer.write_str_value("filter", self.filter)
-        writer.write_int_value("minPrevious", self.min_previous)
-        writer.write_float_value("threshold", self.threshold)
-        writer.write_int_value("window", self.window)
+        writer.write_str_value("formatter", self.formatter)
+        writer.write_str_value("issue", self.issue)
+        writer.write_str_value("issueUrl", self.issue_url)
+        writer.write_str_value("owner", self.owner)
+        writer.write_str_value("repo", self.repo)
+        writer.write_str_value("type", self.type)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/run.py` & `horreum-0.13/src/horreum/raw_client/models/run.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/run_count.py` & `horreum-0.13/src/horreum/raw_client/models/run_count.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/run_extended.py` & `horreum-0.13/src/horreum/raw_client/models/run_extended.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/run_summary.py` & `horreum-0.13/src/horreum/raw_client/models/run_summary.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/runs_summary.py` & `horreum-0.13/src/horreum/raw_client/models/runs_summary.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/schema.py` & `horreum-0.13/src/horreum/raw_client/models/schema.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/schema_descriptor.py` & `horreum-0.13/src/horreum/raw_client/models/schema_descriptor.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/schema_export.py` & `horreum-0.13/src/horreum/raw_client/models/schema_export.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/schema_query_result.py` & `horreum-0.13/src/horreum/raw_client/models/schema_query_result.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/secret.py` & `horreum-0.13/src/horreum/raw_client/models/secret.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test.py` & `horreum-0.13/src/horreum/raw_client/models/test.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_export.py` & `horreum-0.13/src/horreum/raw_client/models/test_export.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_export_datastore.py` & `horreum-0.13/src/horreum/raw_client/models/test_export_datastore.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_export_subscriptions.py` & `horreum-0.13/src/horreum/raw_client/models/test_export_subscriptions.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_listing.py` & `horreum-0.13/src/horreum/raw_client/models/test_token.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
-if TYPE_CHECKING:
-    from .test_summary import TestSummary
-
 @dataclass
-class TestListing(AdditionalDataHolder, Parsable):
+class TestToken(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Number of tests when pagination is ignored
-    count: Optional[int] = None
-    # Array of Test Summaries
-    tests: Optional[List[TestSummary]] = None
+    # Token description
+    description: Optional[str] = None
+    # Unique Token id
+    id: Optional[int] = None
+    # The permissions property
+    permissions: Optional[int] = None
+    # Test ID to apply Token
+    test_id: Optional[int] = None
+    # Test value
+    value: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> TestListing:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> TestToken:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: TestListing
+        Returns: TestToken
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return TestListing()
+        return TestToken()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
-        from .test_summary import TestSummary
-
-        from .test_summary import TestSummary
-
         fields: Dict[str, Callable[[Any], None]] = {
-            "count": lambda n : setattr(self, 'count', n.get_int_value()),
-            "tests": lambda n : setattr(self, 'tests', n.get_collection_of_object_values(TestSummary)),
+            "description": lambda n : setattr(self, 'description', n.get_str_value()),
+            "id": lambda n : setattr(self, 'id', n.get_int_value()),
+            "permissions": lambda n : setattr(self, 'permissions', n.get_int_value()),
+            "testId": lambda n : setattr(self, 'test_id', n.get_int_value()),
+            "value": lambda n : setattr(self, 'value', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_int_value("count", self.count)
-        writer.write_collection_of_object_values("tests", self.tests)
+        writer.write_str_value("description", self.description)
+        writer.write_int_value("id", self.id)
+        writer.write_int_value("permissions", self.permissions)
+        writer.write_int_value("testId", self.test_id)
+        writer.write_str_value("value", self.value)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_query_result.py` & `horreum-0.13/src/horreum/raw_client/models/test_query_result.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_summary.py` & `horreum-0.13/src/horreum/raw_client/models/test_summary.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/test_token.py` & `horreum-0.13/src/horreum/raw_client/models/transformer_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class TestToken(AdditionalDataHolder, Parsable):
+class TransformerInfo(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Token description
-    description: Optional[str] = None
-    # Unique Token id
-    id: Optional[int] = None
-    # The permissions property
-    permissions: Optional[int] = None
-    # Test ID to apply Token
-    test_id: Optional[int] = None
-    # Test value
-    value: Optional[str] = None
+    # Schema ID
+    schema_id: Optional[int] = None
+    # Schema name
+    schema_name: Optional[str] = None
+    # Schema uri
+    schema_uri: Optional[str] = None
+    # Transformer ID
+    transformer_id: Optional[int] = None
+    # Transformer name
+    transformer_name: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> TestToken:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> TransformerInfo:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: TestToken
+        Returns: TransformerInfo
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return TestToken()
+        return TransformerInfo()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "description": lambda n : setattr(self, 'description', n.get_str_value()),
-            "id": lambda n : setattr(self, 'id', n.get_int_value()),
-            "permissions": lambda n : setattr(self, 'permissions', n.get_int_value()),
-            "testId": lambda n : setattr(self, 'test_id', n.get_int_value()),
-            "value": lambda n : setattr(self, 'value', n.get_str_value()),
+            "schemaId": lambda n : setattr(self, 'schema_id', n.get_int_value()),
+            "schemaName": lambda n : setattr(self, 'schema_name', n.get_str_value()),
+            "schemaUri": lambda n : setattr(self, 'schema_uri', n.get_str_value()),
+            "transformerId": lambda n : setattr(self, 'transformer_id', n.get_int_value()),
+            "transformerName": lambda n : setattr(self, 'transformer_name', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_str_value("description", self.description)
-        writer.write_int_value("id", self.id)
-        writer.write_int_value("permissions", self.permissions)
-        writer.write_int_value("testId", self.test_id)
-        writer.write_str_value("value", self.value)
+        writer.write_int_value("schemaId", self.schema_id)
+        writer.write_str_value("schemaName", self.schema_name)
+        writer.write_str_value("schemaUri", self.schema_uri)
+        writer.write_int_value("transformerId", self.transformer_id)
+        writer.write_str_value("transformerName", self.transformer_name)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/transformer.py` & `horreum-0.13/src/horreum/raw_client/models/transformer.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/transformer_info.py` & `horreum-0.13/src/horreum/raw_client/models/slack_channel_message_action_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,54 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from kiota_abstractions.serialization import AdditionalDataHolder, Parsable, ParseNode, SerializationWriter
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 @dataclass
-class TransformerInfo(AdditionalDataHolder, Parsable):
+class SlackChannelMessageActionConfig(AdditionalDataHolder, Parsable):
     # Stores additional data not described in the OpenAPI description found when deserializing. Can be used for serialization as well.
     additional_data: Dict[str, Any] = field(default_factory=dict)
 
-    # Schema ID
-    schema_id: Optional[int] = None
-    # Schema name
-    schema_name: Optional[str] = None
-    # Schema uri
-    schema_uri: Optional[str] = None
-    # Transformer ID
-    transformer_id: Optional[int] = None
-    # Transformer name
-    transformer_name: Optional[str] = None
+    # Slack channel
+    channel: Optional[str] = None
+    # Object markdown formatter
+    formatter: Optional[str] = None
+    # Action type
+    type: Optional[str] = None
     
     @staticmethod
-    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> TransformerInfo:
+    def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> SlackChannelMessageActionConfig:
         """
         Creates a new instance of the appropriate class based on discriminator value
         param parse_node: The parse node to use to read the discriminator value and create the object
-        Returns: TransformerInfo
+        Returns: SlackChannelMessageActionConfig
         """
         if not parse_node:
             raise TypeError("parse_node cannot be null.")
-        return TransformerInfo()
+        return SlackChannelMessageActionConfig()
     
     def get_field_deserializers(self,) -> Dict[str, Callable[[ParseNode], None]]:
         """
         The deserialization information for the current model
         Returns: Dict[str, Callable[[ParseNode], None]]
         """
         fields: Dict[str, Callable[[Any], None]] = {
-            "schemaId": lambda n : setattr(self, 'schema_id', n.get_int_value()),
-            "schemaName": lambda n : setattr(self, 'schema_name', n.get_str_value()),
-            "schemaUri": lambda n : setattr(self, 'schema_uri', n.get_str_value()),
-            "transformerId": lambda n : setattr(self, 'transformer_id', n.get_int_value()),
-            "transformerName": lambda n : setattr(self, 'transformer_name', n.get_str_value()),
+            "channel": lambda n : setattr(self, 'channel', n.get_str_value()),
+            "formatter": lambda n : setattr(self, 'formatter', n.get_str_value()),
+            "type": lambda n : setattr(self, 'type', n.get_str_value()),
         }
         return fields
     
     def serialize(self,writer: SerializationWriter) -> None:
         """
         Serializes information the current object
         param writer: Serialization writer to use to serialize this model
         Returns: None
         """
         if not writer:
             raise TypeError("writer cannot be null.")
-        writer.write_int_value("schemaId", self.schema_id)
-        writer.write_str_value("schemaName", self.schema_name)
-        writer.write_str_value("schemaUri", self.schema_uri)
-        writer.write_int_value("transformerId", self.transformer_id)
-        writer.write_str_value("transformerName", self.transformer_name)
+        writer.write_str_value("channel", self.channel)
+        writer.write_str_value("formatter", self.formatter)
+        writer.write_str_value("type", self.type)
         writer.write_additional_data_value(self.additional_data)
```

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/validation_error.py` & `horreum-0.13/src/horreum/raw_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/validation_error_error.py` & `horreum-0.13/src/horreum/raw_client/models/validation_error_error.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/variable.py` & `horreum-0.13/src/horreum/raw_client/models/variable.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/version_info.py` & `horreum-0.13/src/horreum/raw_client/models/version_info.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/src/horreum/raw_client/models/watch.py` & `horreum-0.13/src/horreum/raw_client/models/watch.py`

 * *Files identical despite different names*

### Comparing `horreum-0.12.1/PKG-INFO` & `horreum-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horreum
-Version: 0.12.1
+Version: 0.13
 Summary: Horreum python library
 Home-page: https://github.com/Hyperfoil/horreum-client-python
 License: Apache 2.0
 Keywords: horreum,performance,change-detection
 Author: Andrea Lamparelli
 Author-email: alampare@redhat.com
 Maintainer: Andrea Lamparelli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: horreum Version: 0.12.1 Summary: Horreum python
+Metadata-Version: 2.1 Name: horreum Version: 0.13 Summary: Horreum python
 library Home-page: https://github.com/Hyperfoil/horreum-client-python License:
 Apache 2.0 Keywords: horreum,performance,change-detection Author: Andrea
 Lamparelli Author-email: alampare@redhat.com Maintainer: Andrea Lamparelli
 Maintainer-email: alampare@redhat.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

