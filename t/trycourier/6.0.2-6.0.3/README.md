# Comparing `tmp/trycourier-6.0.2.tar.gz` & `tmp/trycourier-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-6.0.2.tar", max compression
+gzip compressed data, was "trycourier-6.0.3.tar", max compression
```

## Comparing `trycourier-6.0.2.tar` & `trycourier-6.0.3.tar`

### file list

```diff
@@ -1,366 +1,366 @@
--rw-r--r--   0        0        0     1063 2024-04-22 21:37:23.896554 trycourier-6.0.2/LICENSE
--rw-r--r--   0        0        0     5507 2024-04-22 21:37:23.896554 trycourier-6.0.2/README.md
--rw-r--r--   0        0        0      596 2024-04-22 21:37:23.896554 trycourier-6.0.2/pyproject.toml
--rw-r--r--   0        0        0    14108 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/__init__.py
--rw-r--r--   0        0        0      751 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/__init__.py
--rw-r--r--   0        0        0    26958 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/client.py
--rw-r--r--   0        0        0     1100 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/__init__.py
--rw-r--r--   0        0        0     1199 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/audience.py
--rw-r--r--   0        0        0      971 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/audience_list_response.py
--rw-r--r--   0        0        0      939 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/audience_member.py
--rw-r--r--   0        0        0     1052 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/audience_member_get_response.py
--rw-r--r--   0        0        0      996 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/audience_member_list_response.py
--rw-r--r--   0        0        0      901 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/audience_update_response.py
--rw-r--r--   0        0        0      971 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/base_filter_config.py
--rw-r--r--   0        0        0      386 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/comparison_operator.py
--rw-r--r--   0        0        0      249 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/filter.py
--rw-r--r--   0        0        0      255 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/filter_config.py
--rw-r--r--   0        0        0      152 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/logical_operator.py
--rw-r--r--   0        0        0     1191 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/nested_filter_config.py
--rw-r--r--   0        0        0      240 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/operator.py
--rw-r--r--   0        0        0     1252 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audiences/types/single_filter_config.py
--rw-r--r--   0        0        0      299 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/__init__.py
--rw-r--r--   0        0        0     9927 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/client.py
--rw-r--r--   0        0        0      453 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/__init__.py
--rw-r--r--   0        0        0      905 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/actor.py
--rw-r--r--   0        0        0     1164 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/audit_event.py
--rw-r--r--   0        0        0      988 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/get_audit_event_params.py
--rw-r--r--   0        0        0      886 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/list_audit_events_params.py
--rw-r--r--   0        0        0      983 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/list_audit_events_response.py
--rw-r--r--   0        0        0      906 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/audit_events/types/target.py
--rw-r--r--   0        0        0      137 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/auth_tokens/__init__.py
--rw-r--r--   0        0        0     7017 2024-04-22 21:37:23.896554 trycourier-6.0.2/src/courier/auth_tokens/client.py
--rw-r--r--   0        0        0      152 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/auth_tokens/types/__init__.py
--rw-r--r--   0        0        0      882 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/auth_tokens/types/issue_token_response.py
--rw-r--r--   0        0        0     1847 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/__init__.py
--rw-r--r--   0        0        0    16401 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/client.py
--rw-r--r--   0        0        0     2836 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/__init__.py
--rw-r--r--   0        0        0      962 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/accessor_type.py
--rw-r--r--   0        0        0      988 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation.py
--rw-r--r--   0        0        0     1054 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_ad_hoc_invoke_params.py
--rw-r--r--   0        0        0      138 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_max_items_type.py
--rw-r--r--   0        0        0     1935 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_retain.py
--rw-r--r--   0        0        0      192 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_retain_type.py
--rw-r--r--   0        0        0      178 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_scope.py
--rw-r--r--   0        0        0     3102 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_step.py
--rw-r--r--   0        0        0     1329 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_add_to_digest_step.py
--rw-r--r--   0        0        0     1048 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_cancel_step.py
--rw-r--r--   0        0        0     1331 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_delay_step.py
--rw-r--r--   0        0        0     1758 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_fetch_data_step.py
--rw-r--r--   0        0        0     1186 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_fetch_data_webhook.py
--rw-r--r--   0        0        0      171 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_fetch_data_webhook_method.py
--rw-r--r--   0        0        0     1108 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_invoke_params.py
--rw-r--r--   0        0        0      978 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_invoke_response.py
--rw-r--r--   0        0        0     1015 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_invoke_step.py
--rw-r--r--   0        0        0     1056 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_invoke_template_params.py
--rw-r--r--   0        0        0     1088 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_run_context.py
--rw-r--r--   0        0        0     1262 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_send_list_step.py
--rw-r--r--   0        0        0     1295 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_send_step.py
--rw-r--r--   0        0        0     1030 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_step.py
--rw-r--r--   0        0        0     1102 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_step_option.py
--rw-r--r--   0        0        0     1052 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_throttle_on_throttle.py
--rw-r--r--   0        0        0      176 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_throttle_scope.py
--rw-r--r--   0        0        0     2275 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_throttle_step.py
--rw-r--r--   0        0        0     1039 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_update_profile_step.py
--rw-r--r--   0        0        0     1058 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/automation_v_2_send_step.py
--rw-r--r--   0        0        0      184 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/merge_algorithm.py
--rw-r--r--   0        0        0      101 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/automations/types/profile.py
--rw-r--r--   0        0        0      419 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/__init__.py
--rw-r--r--   0        0        0    28905 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/client.py
--rw-r--r--   0        0        0      579 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/__init__.py
--rw-r--r--   0        0        0     1716 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand.py
--rw-r--r--   0        0        0      962 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand_colors.py
--rw-r--r--   0        0        0      963 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand_get_all_response.py
--rw-r--r--   0        0        0     1120 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand_parameters.py
--rw-r--r--   0        0        0     1052 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand_settings.py
--rw-r--r--   0        0        0      907 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand_snippet.py
--rw-r--r--   0        0        0      915 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brand_snippets.py
--rw-r--r--   0        0        0      958 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/brands/types/brands_response.py
--rw-r--r--   0        0        0     1059 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/__init__.py
--rw-r--r--   0        0        0    29688 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/client.py
--rw-r--r--   0        0        0     1603 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/__init__.py
--rw-r--r--   0        0        0      975 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_create_job_response.py
--rw-r--r--   0        0        0      970 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_params.py
--rw-r--r--   0        0        0      899 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_response.py
--rw-r--r--   0        0        0     1015 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_users_params.py
--rw-r--r--   0        0        0     1022 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_users_response.py
--rw-r--r--   0        0        0      883 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_ingest_error.py
--rw-r--r--   0        0        0      955 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_ingest_users_params.py
--rw-r--r--   0        0        0      975 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_ingest_users_response.py
--rw-r--r--   0        0        0      184 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_job_status.py
--rw-r--r--   0        0        0      173 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_job_user_status.py
--rw-r--r--   0        0        0     1161 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/bulk_message_user_response.py
--rw-r--r--   0        0        0     1512 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_content_message.py
--rw-r--r--   0        0        0     1096 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message.py
--rw-r--r--   0        0        0     1218 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message_user.py
--rw-r--r--   0        0        0     1672 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message_v_1.py
--rw-r--r--   0        0        0      310 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message_v_2.py
--rw-r--r--   0        0        0     1165 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_template_message.py
--rw-r--r--   0        0        0     1046 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/bulk/types/job_details.py
--rw-r--r--   0        0        0    17231 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/client.py
--rw-r--r--   0        0        0     1127 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/__init__.py
--rw-r--r--   0        0        0      527 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/__init__.py
--rw-r--r--   0        0        0      289 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/already_exists_error.py
--rw-r--r--   0        0        0      277 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      268 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/conflict_error.py
--rw-r--r--   0        0        0      298 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/message_not_found_error.py
--rw-r--r--   0        0        0      269 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      297 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/errors/payment_required_error.py
--rw-r--r--   0        0        0     1207 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/__init__.py
--rw-r--r--   0        0        0      988 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/already_exists.py
--rw-r--r--   0        0        0      985 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/bad_request.py
--rw-r--r--   0        0        0      939 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/base_error.py
--rw-r--r--   0        0        0      213 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/channel_classification.py
--rw-r--r--   0        0        0      935 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/channel_preference.py
--rw-r--r--   0        0        0      983 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/conflict.py
--rw-r--r--   0        0        0      876 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/email.py
--rw-r--r--   0        0        0      990 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/message_not_found.py
--rw-r--r--   0        0        0      983 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/not_found.py
--rw-r--r--   0        0        0     1137 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/notification_preference_details.py
--rw-r--r--   0        0        0      230 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/notification_preferences.py
--rw-r--r--   0        0        0      886 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/paging.py
--rw-r--r--   0        0        0      988 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/payment_required.py
--rw-r--r--   0        0        0      177 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/preference_status.py
--rw-r--r--   0        0        0     1038 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/recipient_preferences.py
--rw-r--r--   0        0        0      883 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/rule.py
--rw-r--r--   0        0        0     1147 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/commons/types/user_tenant_association.py
--rw-r--r--   0        0        0      853 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/api_error.py
--rw-r--r--   0        0        0     2088 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/core/request_options.py
--rw-r--r--   0        0        0      159 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/environment.py
--rw-r--r--   0        0        0      413 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/__init__.py
--rw-r--r--   0        0        0    67584 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/client.py
--rw-r--r--   0        0        0      569 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/__init__.py
--rw-r--r--   0        0        0      937 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/list.py
--rw-r--r--   0        0        0      957 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/list_get_all_response.py
--rw-r--r--   0        0        0     1032 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/list_get_subscriptions_response.py
--rw-r--r--   0        0        0      986 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/list_put_params.py
--rw-r--r--   0        0        0     1166 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/list_subscription_recipient.py
--rw-r--r--   0        0        0     1125 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/lists/types/put_subscriptions_recipient.py
--rw-r--r--   0        0        0      527 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/__init__.py
--rw-r--r--   0        0        0    39524 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/client.py
--rw-r--r--   0        0        0      747 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/__init__.py
--rw-r--r--   0        0        0     1157 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/list_messages_response.py
--rw-r--r--   0        0        0     2811 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/message_details.py
--rw-r--r--   0        0        0      932 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/message_history_response.py
--rw-r--r--   0        0        0      357 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/message_status.py
--rw-r--r--   0        0        0      233 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/reason.py
--rw-r--r--   0        0        0     1234 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/render_output.py
--rw-r--r--   0        0        0     1022 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/render_output_response.py
--rw-r--r--   0        0        0     1050 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/rendered_message_block.py
--rw-r--r--   0        0        0     1499 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/messages/types/rendered_message_content.py
--rw-r--r--   0        0        0      985 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/__init__.py
--rw-r--r--   0        0        0    43287 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/client.py
--rw-r--r--   0        0        0     1463 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/__init__.py
--rw-r--r--   0        0        0      943 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/base_check.py
--rw-r--r--   0        0        0      229 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/block_type.py
--rw-r--r--   0        0        0      947 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/check.py
--rw-r--r--   0        0        0      168 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/check_status.py
--rw-r--r--   0        0        0     1127 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/message_routing.py
--rw-r--r--   0        0        0      183 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/message_routing_channel.py
--rw-r--r--   0        0        0      161 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/message_routing_method.py
--rw-r--r--   0        0        0      941 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification.py
--rw-r--r--   0        0        0     1216 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_block.py
--rw-r--r--   0        0        0     1151 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_channel.py
--rw-r--r--   0        0        0      931 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_channel_content.py
--rw-r--r--   0        0        0      224 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_content.py
--rw-r--r--   0        0        0      935 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_content_hierarchy.py
--rw-r--r--   0        0        0     1139 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_get_content_response.py
--rw-r--r--   0        0        0      989 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/notification_list_response.py
--rw-r--r--   0        0        0      908 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/submission_checks_get_response.py
--rw-r--r--   0        0        0      912 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/notifications/types/submission_checks_replace_response.py
--rw-r--r--   0        0        0     1877 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/__init__.py
--rw-r--r--   0        0        0    41051 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/client.py
--rw-r--r--   0        0        0     2897 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/__init__.py
--rw-r--r--   0        0        0      947 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/address.py
--rw-r--r--   0        0        0     1015 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/airship_profile.py
--rw-r--r--   0        0        0      867 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/airship_profile_audience.py
--rw-r--r--   0        0        0      893 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/delete_list_subscription_response.py
--rw-r--r--   0        0        0      104 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/device_type.py
--rw-r--r--   0        0        0      232 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/discord.py
--rw-r--r--   0        0        0      193 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/expo.py
--rw-r--r--   0        0        0     1348 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/get_list_subscriptions_list.py
--rw-r--r--   0        0        0     1092 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/get_list_subscriptions_response.py
--rw-r--r--   0        0        0     1036 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/intercom.py
--rw-r--r--   0        0        0      854 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/intercom_recipient.py
--rw-r--r--   0        0        0      883 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/merge_profile_response.py
--rw-r--r--   0        0        0      566 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/ms_teams.py
--rw-r--r--   0        0        0      886 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/ms_teams_base_properties.py
--rw-r--r--   0        0        0      895 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/multiple_tokens.py
--rw-r--r--   0        0        0      986 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/profile_get_parameters.py
--rw-r--r--   0        0        0     1019 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/profile_get_response.py
--rw-r--r--   0        0        0      885 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/replace_profile_response.py
--rw-r--r--   0        0        0      859 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_direct_message.py
--rw-r--r--   0        0        0      858 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_channel.py
--rw-r--r--   0        0        0     1005 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_channel_id.py
--rw-r--r--   0        0        0     1026 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_channel_name.py
--rw-r--r--   0        0        0     1015 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
--rw-r--r--   0        0        0      996 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_email.py
--rw-r--r--   0        0        0      999 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_user_id.py
--rw-r--r--   0        0        0      991 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_slack_channel.py
--rw-r--r--   0        0        0      987 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_slack_email.py
--rw-r--r--   0        0        0      990 2024-04-22 21:37:23.900554 trycourier-6.0.2/src/courier/profiles/types/send_to_slack_user_id.py
--rw-r--r--   0        0        0      316 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/slack.py
--rw-r--r--   0        0        0      866 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/slack_base_properties.py
--rw-r--r--   0        0        0      935 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/snooze_rule.py
--rw-r--r--   0        0        0      148 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/snooze_rule_type.py
--rw-r--r--   0        0        0      992 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/subscribe_to_lists_request.py
--rw-r--r--   0        0        0     1123 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
--rw-r--r--   0        0        0      887 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/subscribe_to_lists_response.py
--rw-r--r--   0        0        0      845 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/token.py
--rw-r--r--   0        0        0     2026 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/profiles/types/user_profile.py
--rw-r--r--   0        0        0        0 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/py.typed
--rw-r--r--   0        0        0     4101 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/__init__.py
--rw-r--r--   0        0        0     6149 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/__init__.py
--rw-r--r--   0        0        0      122 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/attachment.py
--rw-r--r--   0        0        0     1031 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/audience_filter.py
--rw-r--r--   0        0        0     1201 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/audience_recipient.py
--rw-r--r--   0        0        0     2961 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/base_message.py
--rw-r--r--   0        0        0     1039 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/base_message_send_to.py
--rw-r--r--   0        0        0      856 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/base_social_presence.py
--rw-r--r--   0        0        0     1366 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/brand_settings_email.py
--rw-r--r--   0        0        0     1637 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/brand_settings_in_app.py
--rw-r--r--   0        0        0     1367 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/brand_settings_social_presence.py
--rw-r--r--   0        0        0     1308 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/brand_template.py
--rw-r--r--   0        0        0     1201 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/brand_template_override.py
--rw-r--r--   0        0        0     2359 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/channel.py
--rw-r--r--   0        0        0      898 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/channel_metadata.py
--rw-r--r--   0        0        0      174 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/channel_source.py
--rw-r--r--   0        0        0      252 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/content.py
--rw-r--r--   0        0        0     1546 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/content_message.py
--rw-r--r--   0        0        0      183 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/criteria.py
--rw-r--r--   0        0        0      933 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/delay.py
--rw-r--r--   0        0        0     2131 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_action_node.py
--rw-r--r--   0        0        0     1126 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_base_node.py
--rw-r--r--   0        0        0     2524 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_channel_node.py
--rw-r--r--   0        0        0     1056 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_content.py
--rw-r--r--   0        0        0     1180 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_content_sugar.py
--rw-r--r--   0        0        0     1178 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_divider_node.py
--rw-r--r--   0        0        0     1449 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_group_node.py
--rw-r--r--   0        0        0     1689 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_image_node.py
--rw-r--r--   0        0        0     1384 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_meta_node.py
--rw-r--r--   0        0        0     8164 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_node.py
--rw-r--r--   0        0        0     1697 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_quote_node.py
--rw-r--r--   0        0        0     2459 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/elemental_text_node.py
--rw-r--r--   0        0        0     1063 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/email_footer.py
--rw-r--r--   0        0        0     1023 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/email_head.py
--rw-r--r--   0        0        0     1141 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/email_header.py
--rw-r--r--   0        0        0      119 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/expires_in_type.py
--rw-r--r--   0        0        0     1257 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/expiry.py
--rw-r--r--   0        0        0      160 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/i_action_button_style.py
--rw-r--r--   0        0        0      169 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/i_alignment.py
--rw-r--r--   0        0        0      160 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/i_preferences.py
--rw-r--r--   0        0        0     1139 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/i_profile_preferences.py
--rw-r--r--   0        0        0      909 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/icons.py
--rw-r--r--   0        0        0      172 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/in_app_placement.py
--rw-r--r--   0        0        0      886 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/invalid_list_pattern_recipient.py
--rw-r--r--   0        0        0      884 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/invalid_list_recipient.py
--rw-r--r--   0        0        0      884 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/invalid_user_recipient.py
--rw-r--r--   0        0        0     1027 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/list_filter.py
--rw-r--r--   0        0        0     1122 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/list_pattern_recipient.py
--rw-r--r--   0        0        0      848 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/list_pattern_recipient_type.py
--rw-r--r--   0        0        0     1185 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/list_recipient.py
--rw-r--r--   0        0        0      841 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/list_recipient_type.py
--rw-r--r--   0        0        0      848 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/locale.py
--rw-r--r--   0        0        0      160 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/locales.py
--rw-r--r--   0        0        0      906 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/logo.py
--rw-r--r--   0        0        0      227 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message.py
--rw-r--r--   0        0        0     1502 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_channel_email_override.py
--rw-r--r--   0        0        0      154 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_channels.py
--rw-r--r--   0        0        0     1123 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_context.py
--rw-r--r--   0        0        0      123 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_data.py
--rw-r--r--   0        0        0     1723 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_metadata.py
--rw-r--r--   0        0        0      196 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_providers.py
--rw-r--r--   0        0        0     1477 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_providers_type.py
--rw-r--r--   0        0        0      181 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/message_recipient.py
--rw-r--r--   0        0        0      891 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/metadata.py
--rw-r--r--   0        0        0      910 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/ms_teams_recipient.py
--rw-r--r--   0        0        0      193 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/override.py
--rw-r--r--   0        0        0     1258 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/preference.py
--rw-r--r--   0        0        0      990 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/preferences.py
--rw-r--r--   0        0        0      583 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/recipient.py
--rw-r--r--   0        0        0      125 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/recipient_data.py
--rw-r--r--   0        0        0     1462 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/routing.py
--rw-r--r--   0        0        0      289 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/routing_channel.py
--rw-r--r--   0        0        0      154 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/routing_method.py
--rw-r--r--   0        0        0     1279 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/routing_strategy_channel.py
--rw-r--r--   0        0        0     1135 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/routing_strategy_provider.py
--rw-r--r--   0        0        0      175 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/rule_type.py
--rw-r--r--   0        0        0      898 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/slack_recipient.py
--rw-r--r--   0        0        0     1212 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/template_message.py
--rw-r--r--   0        0        0      160 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/text_align.py
--rw-r--r--   0        0        0      164 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/text_style.py
--rw-r--r--   0        0        0     1114 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/timeout.py
--rw-r--r--   0        0        0      916 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/timeouts.py
--rw-r--r--   0        0        0      856 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/tracking_override.py
--rw-r--r--   0        0        0     2035 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/user_recipient.py
--rw-r--r--   0        0        0      841 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/user_recipient_type.py
--rw-r--r--   0        0        0     1029 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/utm.py
--rw-r--r--   0        0        0     1101 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/send/types/widget_background.py
--rw-r--r--   0        0        0      411 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/__init__.py
--rw-r--r--   0        0        0     5598 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/client.py
--rw-r--r--   0        0        0      564 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/__init__.py
--rw-r--r--   0        0        0       89 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/channel_identifier.py
--rw-r--r--   0        0        0     1091 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/list_templates_response.py
--rw-r--r--   0        0        0     1781 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/notification_templates.py
--rw-r--r--   0        0        0     1351 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/routing_strategy.py
--rw-r--r--   0        0        0      162 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/routing_strategy_method.py
--rw-r--r--   0        0        0      889 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/tag.py
--rw-r--r--   0        0        0      992 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/templates/types/tag_data.py
--rw-r--r--   0        0        0      449 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/__init__.py
--rw-r--r--   0        0        0    29517 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/client.py
--rw-r--r--   0        0        0      624 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/__init__.py
--rw-r--r--   0        0        0      935 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/default_preferences.py
--rw-r--r--   0        0        0     1737 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/list_users_for_tenant_response.py
--rw-r--r--   0        0        0     1005 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/subscription_topic.py
--rw-r--r--   0        0        0      184 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/subscription_topic_status.py
--rw-r--r--   0        0        0      110 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/template_property.py
--rw-r--r--   0        0        0     1904 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/tenant.py
--rw-r--r--   0        0        0     1698 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/tenants/types/tenant_list_response.py
--rw-r--r--   0        0        0       65 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/translations/__init__.py
--rw-r--r--   0        0        0    10736 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/translations/client.py
--rw-r--r--   0        0        0      155 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/types/__init__.py
--rw-r--r--   0        0        0     1592 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/types/send_message_response.py
--rw-r--r--   0        0        0     1354 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/client.py
--rw-r--r--   0        0        0      409 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/__init__.py
--rw-r--r--   0        0        0    17633 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/client.py
--rw-r--r--   0        0        0      561 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/types/__init__.py
--rw-r--r--   0        0        0     1345 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/types/topic_preference.py
--rw-r--r--   0        0        0     1276 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/types/topic_preference_update.py
--rw-r--r--   0        0        0      926 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/types/user_preferences_get_response.py
--rw-r--r--   0        0        0     1090 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/types/user_preferences_list_response.py
--rw-r--r--   0        0        0      873 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/preferences/types/user_preferences_update_response.py
--rw-r--r--   0        0        0      229 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tenants/__init__.py
--rw-r--r--   0        0        0    28095 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tenants/client.py
--rw-r--r--   0        0        0      308 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tenants/types/__init__.py
--rw-r--r--   0        0        0     1288 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
--rw-r--r--   0        0        0     1740 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tenants/types/list_tenants_for_user_response.py
--rw-r--r--   0        0        0      765 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/__init__.py
--rw-r--r--   0        0        0    28284 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/client.py
--rw-r--r--   0        0        0     1135 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/__init__.py
--rw-r--r--   0        0        0      878 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/delete_user_token_opts.py
--rw-r--r--   0        0        0     1576 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/device.py
--rw-r--r--   0        0        0      117 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/expiry_date.py
--rw-r--r--   0        0        0      161 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/get_all_tokens_response.py
--rw-r--r--   0        0        0      875 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/get_user_token_opts.py
--rw-r--r--   0        0        0     1160 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/get_user_token_response.py
--rw-r--r--   0        0        0      861 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/get_user_tokens_opts.py
--rw-r--r--   0        0        0      183 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/patch_op.py
--rw-r--r--   0        0        0     1158 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/patch_operation.py
--rw-r--r--   0        0        0      928 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/patch_user_token_opts.py
--rw-r--r--   0        0        0      179 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/provider_key.py
--rw-r--r--   0        0        0      915 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/put_user_token_opts.py
--rw-r--r--   0        0        0      930 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/put_user_tokens_opts.py
--rw-r--r--   0        0        0      177 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/token_status.py
--rw-r--r--   0        0        0     1387 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/tracking.py
--rw-r--r--   0        0        0     1790 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/users/tokens/types/user_token.py
--rw-r--r--   0        0        0       78 2024-04-22 21:37:23.904554 trycourier-6.0.2/src/courier/version.py
--rw-r--r--   0        0        0     6000 1970-01-01 00:00:00.000000 trycourier-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-01 02:48:53.976418 trycourier-6.0.3/LICENSE
+-rw-r--r--   0        0        0     5507 2024-05-01 02:48:53.976418 trycourier-6.0.3/README.md
+-rw-r--r--   0        0        0      595 2024-05-01 02:48:53.976418 trycourier-6.0.3/pyproject.toml
+-rw-r--r--   0        0        0    14108 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/__init__.py
+-rw-r--r--   0        0        0    28202 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/client.py
+-rw-r--r--   0        0        0     1100 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience.py
+-rw-r--r--   0        0        0      971 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_list_response.py
+-rw-r--r--   0        0        0      939 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_member.py
+-rw-r--r--   0        0        0     1052 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_member_get_response.py
+-rw-r--r--   0        0        0      996 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_member_list_response.py
+-rw-r--r--   0        0        0      901 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/audience_update_response.py
+-rw-r--r--   0        0        0      971 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/base_filter_config.py
+-rw-r--r--   0        0        0      386 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/comparison_operator.py
+-rw-r--r--   0        0        0      249 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/filter.py
+-rw-r--r--   0        0        0      255 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/filter_config.py
+-rw-r--r--   0        0        0      152 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/logical_operator.py
+-rw-r--r--   0        0        0     1191 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/nested_filter_config.py
+-rw-r--r--   0        0        0      240 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/operator.py
+-rw-r--r--   0        0        0     1252 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audiences/types/single_filter_config.py
+-rw-r--r--   0        0        0      299 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/__init__.py
+-rw-r--r--   0        0        0    10417 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/client.py
+-rw-r--r--   0        0        0      453 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/__init__.py
+-rw-r--r--   0        0        0      905 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/actor.py
+-rw-r--r--   0        0        0     1164 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/audit_event.py
+-rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/get_audit_event_params.py
+-rw-r--r--   0        0        0      886 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_params.py
+-rw-r--r--   0        0        0      983 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_response.py
+-rw-r--r--   0        0        0      906 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/audit_events/types/target.py
+-rw-r--r--   0        0        0      137 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/__init__.py
+-rw-r--r--   0        0        0     7229 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/client.py
+-rw-r--r--   0        0        0      152 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/types/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/auth_tokens/types/issue_token_response.py
+-rw-r--r--   0        0        0     1847 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/__init__.py
+-rw-r--r--   0        0        0    16885 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/client.py
+-rw-r--r--   0        0        0     2836 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/accessor_type.py
+-rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation.py
+-rw-r--r--   0        0        0     1054 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_ad_hoc_invoke_params.py
+-rw-r--r--   0        0        0      138 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_max_items_type.py
+-rw-r--r--   0        0        0     1954 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_retain.py
+-rw-r--r--   0        0        0      192 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_retain_type.py
+-rw-r--r--   0        0        0      178 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_scope.py
+-rw-r--r--   0        0        0     3128 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_step.py
+-rw-r--r--   0        0        0     1355 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_add_to_digest_step.py
+-rw-r--r--   0        0        0     1048 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_cancel_step.py
+-rw-r--r--   0        0        0     1331 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_delay_step.py
+-rw-r--r--   0        0        0     1784 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_step.py
+-rw-r--r--   0        0        0     1186 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_webhook.py
+-rw-r--r--   0        0        0      171 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_webhook_method.py
+-rw-r--r--   0        0        0     1108 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_params.py
+-rw-r--r--   0        0        0      978 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_response.py
+-rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_step.py
+-rw-r--r--   0        0        0     1056 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_invoke_template_params.py
+-rw-r--r--   0        0        0     1088 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_run_context.py
+-rw-r--r--   0        0        0     1262 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_send_list_step.py
+-rw-r--r--   0        0        0     1295 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_send_step.py
+-rw-r--r--   0        0        0     1030 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_step.py
+-rw-r--r--   0        0        0     1102 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_step_option.py
+-rw-r--r--   0        0        0     1052 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_throttle_on_throttle.py
+-rw-r--r--   0        0        0      176 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_throttle_scope.py
+-rw-r--r--   0        0        0     2301 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_throttle_step.py
+-rw-r--r--   0        0        0     1039 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_update_profile_step.py
+-rw-r--r--   0        0        0     1058 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/automation_v_2_send_step.py
+-rw-r--r--   0        0        0      184 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/merge_algorithm.py
+-rw-r--r--   0        0        0      101 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/automations/types/profile.py
+-rw-r--r--   0        0        0      419 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/__init__.py
+-rw-r--r--   0        0        0    29995 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/client.py
+-rw-r--r--   0        0        0      579 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/__init__.py
+-rw-r--r--   0        0        0     1716 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand.py
+-rw-r--r--   0        0        0      962 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_colors.py
+-rw-r--r--   0        0        0      963 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_get_all_response.py
+-rw-r--r--   0        0        0     1120 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_parameters.py
+-rw-r--r--   0        0        0     1052 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_settings.py
+-rw-r--r--   0        0        0      907 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_snippet.py
+-rw-r--r--   0        0        0      915 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brand_snippets.py
+-rw-r--r--   0        0        0      958 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/brands/types/brands_response.py
+-rw-r--r--   0        0        0     1059 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/__init__.py
+-rw-r--r--   0        0        0    30912 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/client.py
+-rw-r--r--   0        0        0     1603 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_create_job_response.py
+-rw-r--r--   0        0        0      970 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_params.py
+-rw-r--r--   0        0        0      899 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_response.py
+-rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_params.py
+-rw-r--r--   0        0        0     1022 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_response.py
+-rw-r--r--   0        0        0      883 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_error.py
+-rw-r--r--   0        0        0      955 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_params.py
+-rw-r--r--   0        0        0      975 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_response.py
+-rw-r--r--   0        0        0      184 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_job_status.py
+-rw-r--r--   0        0        0      173 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_job_user_status.py
+-rw-r--r--   0        0        0     1161 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/bulk_message_user_response.py
+-rw-r--r--   0        0        0     1512 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_content_message.py
+-rw-r--r--   0        0        0     1096 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message.py
+-rw-r--r--   0        0        0     1218 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_user.py
+-rw-r--r--   0        0        0     1672 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_v_1.py
+-rw-r--r--   0        0        0      310 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_v_2.py
+-rw-r--r--   0        0        0     1165 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_template_message.py
+-rw-r--r--   0        0        0     1046 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/bulk/types/job_details.py
+-rw-r--r--   0        0        0    17491 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/client.py
+-rw-r--r--   0        0        0     1127 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/__init__.py
+-rw-r--r--   0        0        0      527 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/__init__.py
+-rw-r--r--   0        0        0      289 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/already_exists_error.py
+-rw-r--r--   0        0        0      277 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      268 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/conflict_error.py
+-rw-r--r--   0        0        0      298 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/message_not_found_error.py
+-rw-r--r--   0        0        0      269 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      297 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/errors/payment_required_error.py
+-rw-r--r--   0        0        0     1207 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/__init__.py
+-rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/already_exists.py
+-rw-r--r--   0        0        0      985 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/bad_request.py
+-rw-r--r--   0        0        0      939 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/base_error.py
+-rw-r--r--   0        0        0      213 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/channel_classification.py
+-rw-r--r--   0        0        0      935 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/channel_preference.py
+-rw-r--r--   0        0        0      983 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/conflict.py
+-rw-r--r--   0        0        0      876 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/email.py
+-rw-r--r--   0        0        0      990 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/message_not_found.py
+-rw-r--r--   0        0        0      983 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/not_found.py
+-rw-r--r--   0        0        0     1137 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/notification_preference_details.py
+-rw-r--r--   0        0        0      230 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/notification_preferences.py
+-rw-r--r--   0        0        0      886 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/paging.py
+-rw-r--r--   0        0        0      988 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/payment_required.py
+-rw-r--r--   0        0        0      177 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/preference_status.py
+-rw-r--r--   0        0        0     1038 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/recipient_preferences.py
+-rw-r--r--   0        0        0      883 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/rule.py
+-rw-r--r--   0        0        0     1353 2024-05-01 02:48:53.976418 trycourier-6.0.3/src/courier/commons/types/user_tenant_association.py
+-rw-r--r--   0        0        0      853 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/api_error.py
+-rw-r--r--   0        0        0     2088 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/core/request_options.py
+-rw-r--r--   0        0        0      159 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/environment.py
+-rw-r--r--   0        0        0      413 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/__init__.py
+-rw-r--r--   0        0        0    69860 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/client.py
+-rw-r--r--   0        0        0      569 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list.py
+-rw-r--r--   0        0        0      957 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_get_all_response.py
+-rw-r--r--   0        0        0     1032 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_get_subscriptions_response.py
+-rw-r--r--   0        0        0      986 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_put_params.py
+-rw-r--r--   0        0        0     1166 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/list_subscription_recipient.py
+-rw-r--r--   0        0        0     1125 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/lists/types/put_subscriptions_recipient.py
+-rw-r--r--   0        0        0      527 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/__init__.py
+-rw-r--r--   0        0        0    41212 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/client.py
+-rw-r--r--   0        0        0      747 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/__init__.py
+-rw-r--r--   0        0        0     1157 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/list_messages_response.py
+-rw-r--r--   0        0        0     2811 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/message_details.py
+-rw-r--r--   0        0        0      932 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/message_history_response.py
+-rw-r--r--   0        0        0      357 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/message_status.py
+-rw-r--r--   0        0        0      233 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/reason.py
+-rw-r--r--   0        0        0     1234 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/render_output.py
+-rw-r--r--   0        0        0     1022 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/render_output_response.py
+-rw-r--r--   0        0        0     1050 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/rendered_message_block.py
+-rw-r--r--   0        0        0     1499 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/messages/types/rendered_message_content.py
+-rw-r--r--   0        0        0      985 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/__init__.py
+-rw-r--r--   0        0        0    45003 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/client.py
+-rw-r--r--   0        0        0     1463 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/base_check.py
+-rw-r--r--   0        0        0      229 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/block_type.py
+-rw-r--r--   0        0        0      947 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/check.py
+-rw-r--r--   0        0        0      168 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/check_status.py
+-rw-r--r--   0        0        0     1127 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/message_routing.py
+-rw-r--r--   0        0        0      183 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/message_routing_channel.py
+-rw-r--r--   0        0        0      161 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/message_routing_method.py
+-rw-r--r--   0        0        0      941 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification.py
+-rw-r--r--   0        0        0     1216 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_block.py
+-rw-r--r--   0        0        0     1151 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_channel.py
+-rw-r--r--   0        0        0      931 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_channel_content.py
+-rw-r--r--   0        0        0      224 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_content.py
+-rw-r--r--   0        0        0      935 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_content_hierarchy.py
+-rw-r--r--   0        0        0     1139 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_get_content_response.py
+-rw-r--r--   0        0        0      989 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/notification_list_response.py
+-rw-r--r--   0        0        0      908 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/submission_checks_get_response.py
+-rw-r--r--   0        0        0      912 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/notifications/types/submission_checks_replace_response.py
+-rw-r--r--   0        0        0     1877 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/__init__.py
+-rw-r--r--   0        0        0    43043 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/client.py
+-rw-r--r--   0        0        0     2897 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/__init__.py
+-rw-r--r--   0        0        0      947 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/address.py
+-rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/airship_profile.py
+-rw-r--r--   0        0        0      867 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/airship_profile_audience.py
+-rw-r--r--   0        0        0      893 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/delete_list_subscription_response.py
+-rw-r--r--   0        0        0      104 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/device_type.py
+-rw-r--r--   0        0        0      232 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/discord.py
+-rw-r--r--   0        0        0      193 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/expo.py
+-rw-r--r--   0        0        0     1348 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_list.py
+-rw-r--r--   0        0        0     1092 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1036 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/intercom.py
+-rw-r--r--   0        0        0      854 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/intercom_recipient.py
+-rw-r--r--   0        0        0      883 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/merge_profile_response.py
+-rw-r--r--   0        0        0      566 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/ms_teams.py
+-rw-r--r--   0        0        0      886 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/ms_teams_base_properties.py
+-rw-r--r--   0        0        0      895 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/multiple_tokens.py
+-rw-r--r--   0        0        0      986 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/profile_get_parameters.py
+-rw-r--r--   0        0        0     1019 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/profile_get_response.py
+-rw-r--r--   0        0        0      885 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/replace_profile_response.py
+-rw-r--r--   0        0        0      859 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_direct_message.py
+-rw-r--r--   0        0        0      858 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_channel.py
+-rw-r--r--   0        0        0     1005 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_id.py
+-rw-r--r--   0        0        0     1026 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_name.py
+-rw-r--r--   0        0        0     1015 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
+-rw-r--r--   0        0        0      996 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_email.py
+-rw-r--r--   0        0        0      999 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_user_id.py
+-rw-r--r--   0        0        0      991 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_slack_channel.py
+-rw-r--r--   0        0        0      987 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_slack_email.py
+-rw-r--r--   0        0        0      990 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/send_to_slack_user_id.py
+-rw-r--r--   0        0        0      316 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/slack.py
+-rw-r--r--   0        0        0      866 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/slack_base_properties.py
+-rw-r--r--   0        0        0      935 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/snooze_rule.py
+-rw-r--r--   0        0        0      148 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/snooze_rule_type.py
+-rw-r--r--   0        0        0      992 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request.py
+-rw-r--r--   0        0        0     1123 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
+-rw-r--r--   0        0        0      887 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_response.py
+-rw-r--r--   0        0        0      845 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/token.py
+-rw-r--r--   0        0        0     2026 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/profiles/types/user_profile.py
+-rw-r--r--   0        0        0        0 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/py.typed
+-rw-r--r--   0        0        0     4101 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/__init__.py
+-rw-r--r--   0        0        0     6149 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/__init__.py
+-rw-r--r--   0        0        0      122 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/attachment.py
+-rw-r--r--   0        0        0     1031 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/audience_filter.py
+-rw-r--r--   0        0        0     1201 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/audience_recipient.py
+-rw-r--r--   0        0        0     2961 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/base_message.py
+-rw-r--r--   0        0        0     1039 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/base_message_send_to.py
+-rw-r--r--   0        0        0      856 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/base_social_presence.py
+-rw-r--r--   0        0        0     1366 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_settings_email.py
+-rw-r--r--   0        0        0     1637 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_settings_in_app.py
+-rw-r--r--   0        0        0     1367 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_settings_social_presence.py
+-rw-r--r--   0        0        0     1308 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_template.py
+-rw-r--r--   0        0        0     1201 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/brand_template_override.py
+-rw-r--r--   0        0        0     2359 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/channel.py
+-rw-r--r--   0        0        0      898 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/channel_metadata.py
+-rw-r--r--   0        0        0      174 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/channel_source.py
+-rw-r--r--   0        0        0      252 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/content.py
+-rw-r--r--   0        0        0     1546 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/content_message.py
+-rw-r--r--   0        0        0      183 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/criteria.py
+-rw-r--r--   0        0        0      933 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/delay.py
+-rw-r--r--   0        0        0     2131 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_action_node.py
+-rw-r--r--   0        0        0     1126 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_base_node.py
+-rw-r--r--   0        0        0     2524 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_channel_node.py
+-rw-r--r--   0        0        0     1056 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_content.py
+-rw-r--r--   0        0        0     1180 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_content_sugar.py
+-rw-r--r--   0        0        0     1178 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_divider_node.py
+-rw-r--r--   0        0        0     1449 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_group_node.py
+-rw-r--r--   0        0        0     1689 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_image_node.py
+-rw-r--r--   0        0        0     1384 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_meta_node.py
+-rw-r--r--   0        0        0     8164 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_node.py
+-rw-r--r--   0        0        0     1697 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_quote_node.py
+-rw-r--r--   0        0        0     2459 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/elemental_text_node.py
+-rw-r--r--   0        0        0     1063 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/email_footer.py
+-rw-r--r--   0        0        0     1023 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/email_head.py
+-rw-r--r--   0        0        0     1141 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/email_header.py
+-rw-r--r--   0        0        0      119 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/expires_in_type.py
+-rw-r--r--   0        0        0     1257 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/expiry.py
+-rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_action_button_style.py
+-rw-r--r--   0        0        0      169 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_alignment.py
+-rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_preferences.py
+-rw-r--r--   0        0        0     1139 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/i_profile_preferences.py
+-rw-r--r--   0        0        0      909 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/icons.py
+-rw-r--r--   0        0        0      172 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/in_app_placement.py
+-rw-r--r--   0        0        0      886 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/invalid_list_pattern_recipient.py
+-rw-r--r--   0        0        0      884 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/invalid_list_recipient.py
+-rw-r--r--   0        0        0      884 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/invalid_user_recipient.py
+-rw-r--r--   0        0        0     1027 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_filter.py
+-rw-r--r--   0        0        0     1122 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_pattern_recipient.py
+-rw-r--r--   0        0        0      848 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_pattern_recipient_type.py
+-rw-r--r--   0        0        0     1185 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_recipient.py
+-rw-r--r--   0        0        0      841 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/list_recipient_type.py
+-rw-r--r--   0        0        0      848 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/locale.py
+-rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/locales.py
+-rw-r--r--   0        0        0      906 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/logo.py
+-rw-r--r--   0        0        0      227 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message.py
+-rw-r--r--   0        0        0     1502 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_channel_email_override.py
+-rw-r--r--   0        0        0      154 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_channels.py
+-rw-r--r--   0        0        0     1123 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_context.py
+-rw-r--r--   0        0        0      123 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_data.py
+-rw-r--r--   0        0        0     1723 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_metadata.py
+-rw-r--r--   0        0        0      196 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_providers.py
+-rw-r--r--   0        0        0     1477 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_providers_type.py
+-rw-r--r--   0        0        0      181 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/message_recipient.py
+-rw-r--r--   0        0        0      891 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/metadata.py
+-rw-r--r--   0        0        0      910 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/ms_teams_recipient.py
+-rw-r--r--   0        0        0      193 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/override.py
+-rw-r--r--   0        0        0     1258 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/preference.py
+-rw-r--r--   0        0        0      990 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/preferences.py
+-rw-r--r--   0        0        0      583 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/recipient.py
+-rw-r--r--   0        0        0      125 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/recipient_data.py
+-rw-r--r--   0        0        0     1462 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing.py
+-rw-r--r--   0        0        0      289 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_channel.py
+-rw-r--r--   0        0        0      154 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_method.py
+-rw-r--r--   0        0        0     1279 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_strategy_channel.py
+-rw-r--r--   0        0        0     1135 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/routing_strategy_provider.py
+-rw-r--r--   0        0        0      175 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/rule_type.py
+-rw-r--r--   0        0        0      898 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/slack_recipient.py
+-rw-r--r--   0        0        0     1212 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/template_message.py
+-rw-r--r--   0        0        0      160 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/text_align.py
+-rw-r--r--   0        0        0      164 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/text_style.py
+-rw-r--r--   0        0        0     1114 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/timeout.py
+-rw-r--r--   0        0        0      916 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/timeouts.py
+-rw-r--r--   0        0        0      856 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/tracking_override.py
+-rw-r--r--   0        0        0     2035 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/user_recipient.py
+-rw-r--r--   0        0        0      841 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/user_recipient_type.py
+-rw-r--r--   0        0        0     1029 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/utm.py
+-rw-r--r--   0        0        0     1101 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/send/types/widget_background.py
+-rw-r--r--   0        0        0      411 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/__init__.py
+-rw-r--r--   0        0        0     5852 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/client.py
+-rw-r--r--   0        0        0      564 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/channel_identifier.py
+-rw-r--r--   0        0        0     1091 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/list_templates_response.py
+-rw-r--r--   0        0        0     1781 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/notification_templates.py
+-rw-r--r--   0        0        0     1351 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/routing_strategy.py
+-rw-r--r--   0        0        0      162 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/routing_strategy_method.py
+-rw-r--r--   0        0        0      889 2024-05-01 02:48:53.980418 trycourier-6.0.3/src/courier/templates/types/tag.py
+-rw-r--r--   0        0        0      992 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/templates/types/tag_data.py
+-rw-r--r--   0        0        0      449 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/__init__.py
+-rw-r--r--   0        0        0    30865 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/client.py
+-rw-r--r--   0        0        0      624 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/default_preferences.py
+-rw-r--r--   0        0        0     1737 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/list_users_for_tenant_response.py
+-rw-r--r--   0        0        0     1005 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/subscription_topic.py
+-rw-r--r--   0        0        0      184 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/subscription_topic_status.py
+-rw-r--r--   0        0        0      110 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/template_property.py
+-rw-r--r--   0        0        0     1904 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/tenant.py
+-rw-r--r--   0        0        0     1698 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/tenants/types/tenant_list_response.py
+-rw-r--r--   0        0        0       65 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/translations/__init__.py
+-rw-r--r--   0        0        0    11268 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/translations/client.py
+-rw-r--r--   0        0        0      155 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/types/__init__.py
+-rw-r--r--   0        0        0     1592 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/types/send_message_response.py
+-rw-r--r--   0        0        0     1354 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/__init__.py
+-rw-r--r--   0        0        0     1067 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/client.py
+-rw-r--r--   0        0        0      409 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/__init__.py
+-rw-r--r--   0        0        0    18445 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/client.py
+-rw-r--r--   0        0        0      561 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/__init__.py
+-rw-r--r--   0        0        0     1345 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/topic_preference.py
+-rw-r--r--   0        0        0     1276 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/topic_preference_update.py
+-rw-r--r--   0        0        0      926 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_get_response.py
+-rw-r--r--   0        0        0     1090 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_list_response.py
+-rw-r--r--   0        0        0      873 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_update_response.py
+-rw-r--r--   0        0        0      229 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/__init__.py
+-rw-r--r--   0        0        0    28780 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/client.py
+-rw-r--r--   0        0        0      308 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/types/__init__.py
+-rw-r--r--   0        0        0     1397 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
+-rw-r--r--   0        0        0     1740 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tenants/types/list_tenants_for_user_response.py
+-rw-r--r--   0        0        0      765 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/__init__.py
+-rw-r--r--   0        0        0    29460 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/client.py
+-rw-r--r--   0        0        0     1135 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/__init__.py
+-rw-r--r--   0        0        0      878 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/delete_user_token_opts.py
+-rw-r--r--   0        0        0     1576 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/device.py
+-rw-r--r--   0        0        0      117 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/expiry_date.py
+-rw-r--r--   0        0        0      161 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_all_tokens_response.py
+-rw-r--r--   0        0        0      875 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_opts.py
+-rw-r--r--   0        0        0     1160 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_response.py
+-rw-r--r--   0        0        0      861 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/get_user_tokens_opts.py
+-rw-r--r--   0        0        0      183 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/patch_op.py
+-rw-r--r--   0        0        0     1158 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/patch_operation.py
+-rw-r--r--   0        0        0      928 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/patch_user_token_opts.py
+-rw-r--r--   0        0        0      179 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/provider_key.py
+-rw-r--r--   0        0        0      915 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/put_user_token_opts.py
+-rw-r--r--   0        0        0      930 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/put_user_tokens_opts.py
+-rw-r--r--   0        0        0      177 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/token_status.py
+-rw-r--r--   0        0        0     1387 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/tracking.py
+-rw-r--r--   0        0        0     1790 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/users/tokens/types/user_token.py
+-rw-r--r--   0        0        0       78 2024-05-01 02:48:53.984418 trycourier-6.0.3/src/courier/version.py
+-rw-r--r--   0        0        0     6000 1970-01-01 00:00:00.000000 trycourier-6.0.3/PKG-INFO
```

### Comparing `trycourier-6.0.2/LICENSE` & `trycourier-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/README.md` & `trycourier-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/pyproject.toml` & `trycourier-6.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "trycourier"
-version = "v6.0.2"
+version = "v6.0.3"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "courier", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.21.2"
 pydantic = ">= 1.9.2"
 typing_extensions = ">= 4.0.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.8.0"
+mypy = "1.9.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
 python-dateutil = "^2.9.0"
 
 [tool.pytest.ini_options]
 testpaths = [ "tests" ]
 asyncio_mode = "auto"
```

### Comparing `trycourier-6.0.2/src/courier/__init__.py` & `trycourier-6.0.3/src/courier/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/__init__.py` & `trycourier-6.0.3/src/courier/audiences/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/client.py` & `trycourier-6.0.3/src/courier/audiences/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,31 +26,40 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Audience:
         """
         Returns the specified audience by id.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience_id
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience_id
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Audience
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audiences.get(
             audience_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -82,25 +91,36 @@
         description: typing.Optional[str] = OMIT,
         filter: typing.Optional[Filter] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AudienceUpdateResponse:
         """
         Creates or updates audience.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience id
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience id
 
-            - name: typing.Optional[str]. The name of the audience
+        name : typing.Optional[str]
+            The name of the audience
 
-            - description: typing.Optional[str]. A description of the audience
+        description : typing.Optional[str]
+            A description of the audience
 
-            - filter: typing.Optional[Filter].
+        filter : typing.Optional[Filter]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudienceUpdateResponse
+
+        Examples
+        --------
         from courier import SingleFilterConfig
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audiences.update(
@@ -118,16 +138,16 @@
         if name is not OMIT:
             _request["name"] = name
         if description is not OMIT:
             _request["description"] = description
         if filter is not OMIT:
             _request["filter"] = filter
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -157,31 +177,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Deletes the specified audience.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience id
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience id
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audiences.delete(
             audience_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -211,34 +240,44 @@
         *,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AudienceMemberListResponse:
         """
         Get list of members of an audience.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience id
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of members
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience id
+
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of members
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudienceMemberListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audiences.list_members(
             audience_id="string",
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}/members"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
@@ -275,31 +314,40 @@
 
     def list_audiences(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> AudienceListResponse:
         """
         Get the audiences associated with the authorization token.
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audiences
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of audiences
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudienceListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audiences.list_audiences(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -337,31 +385,40 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Audience:
         """
         Returns the specified audience by id.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience_id
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience_id
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Audience
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audiences.get(
             audience_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -393,25 +450,36 @@
         description: typing.Optional[str] = OMIT,
         filter: typing.Optional[Filter] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AudienceUpdateResponse:
         """
         Creates or updates audience.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience id
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience id
 
-            - name: typing.Optional[str]. The name of the audience
+        name : typing.Optional[str]
+            The name of the audience
 
-            - description: typing.Optional[str]. A description of the audience
+        description : typing.Optional[str]
+            A description of the audience
 
-            - filter: typing.Optional[Filter].
+        filter : typing.Optional[Filter]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudienceUpdateResponse
+
+        Examples
+        --------
         from courier import SingleFilterConfig
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audiences.update(
@@ -429,16 +497,16 @@
         if name is not OMIT:
             _request["name"] = name
         if description is not OMIT:
             _request["description"] = description
         if filter is not OMIT:
             _request["filter"] = filter
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -468,31 +536,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Deletes the specified audience.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience id
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience id
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audiences.delete(
             audience_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -522,34 +599,44 @@
         *,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AudienceMemberListResponse:
         """
         Get list of members of an audience.
 
-        Parameters:
-            - audience_id: str. A unique identifier representing the audience id
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of members
+        Parameters
+        ----------
+        audience_id : str
+            A unique identifier representing the audience id
+
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of members
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudienceMemberListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audiences.list_members(
             audience_id="string",
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}/members"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
@@ -586,31 +673,40 @@
 
     async def list_audiences(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> AudienceListResponse:
         """
         Get the audiences associated with the authorization token.
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audiences
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of audiences
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudienceListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audiences.list_audiences(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
```

### Comparing `trycourier-6.0.2/src/courier/audiences/types/__init__.py` & `trycourier-6.0.3/src/courier/audiences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/audience.py` & `trycourier-6.0.3/src/courier/audiences/types/audience.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/audience_list_response.py` & `trycourier-6.0.3/src/courier/audiences/types/audience_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/audience_member.py` & `trycourier-6.0.3/src/courier/audiences/types/audience_member.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/audience_member_get_response.py` & `trycourier-6.0.3/src/courier/audiences/types/audience_member_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/audience_member_list_response.py` & `trycourier-6.0.3/src/courier/audiences/types/audience_member_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/audience_update_response.py` & `trycourier-6.0.3/src/courier/audiences/types/audience_update_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/base_filter_config.py` & `trycourier-6.0.3/src/courier/audiences/types/base_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/nested_filter_config.py` & `trycourier-6.0.3/src/courier/audiences/types/nested_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audiences/types/single_filter_config.py` & `trycourier-6.0.3/src/courier/audiences/types/single_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audit_events/client.py` & `trycourier-6.0.3/src/courier/audit_events/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,31 +20,40 @@
 
     def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListAuditEventsResponse:
         """
         Fetch the list of audit events
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audit events.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of audit events.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListAuditEventsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audit_events.list(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -75,31 +84,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, audit_event_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AuditEvent:
         """
         Fetch a specific audit event by ID.
 
-        Parameters:
-            - audit_event_id: str. A unique identifier associated with the audit event you wish to retrieve
+        Parameters
+        ----------
+        audit_event_id : str
+            A unique identifier associated with the audit event you wish to retrieve
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AuditEvent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.audit_events.get(
             audit_event_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audit-events/{jsonable_encoder(audit_event_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -130,31 +148,40 @@
 
     async def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListAuditEventsResponse:
         """
         Fetch the list of audit events
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audit events.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of audit events.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListAuditEventsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audit_events.list(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -185,31 +212,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, audit_event_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AuditEvent:
         """
         Fetch a specific audit event by ID.
 
-        Parameters:
-            - audit_event_id: str. A unique identifier associated with the audit event you wish to retrieve
+        Parameters
+        ----------
+        audit_event_id : str
+            A unique identifier associated with the audit event you wish to retrieve
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AuditEvent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.audit_events.get(
             audit_event_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audit-events/{jsonable_encoder(audit_event_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
```

### Comparing `trycourier-6.0.2/src/courier/audit_events/types/actor.py` & `trycourier-6.0.3/src/courier/audit_events/types/actor.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audit_events/types/audit_event.py` & `trycourier-6.0.3/src/courier/audit_events/types/audit_event.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audit_events/types/get_audit_event_params.py` & `trycourier-6.0.3/src/courier/audit_events/types/get_audit_event_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audit_events/types/list_audit_events_params.py` & `trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audit_events/types/list_audit_events_response.py` & `trycourier-6.0.3/src/courier/audit_events/types/list_audit_events_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/audit_events/types/target.py` & `trycourier-6.0.3/src/courier/audit_events/types/target.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/auth_tokens/client.py` & `trycourier-6.0.3/src/courier/auth_tokens/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,38 +28,47 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> IssueTokenResponse:
         """
         Returns a new access token.
 
-        Parameters:
-            - scope: str.
+        Parameters
+        ----------
+        scope : str
 
-            - expires_in: str.
+        expires_in : str
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        IssueTokenResponse
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.auth_tokens.issue_token(
             scope="string",
             expires_in="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "auth/issue-token"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "auth/issue-token"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"scope": scope, "expires_in": expires_in})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"scope": scope, "expires_in": expires_in}),
@@ -102,38 +111,47 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> IssueTokenResponse:
         """
         Returns a new access token.
 
-        Parameters:
-            - scope: str.
+        Parameters
+        ----------
+        scope : str
+
+        expires_in : str
+
+        idempotency_key : typing.Optional[str]
 
-            - expires_in: str.
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        IssueTokenResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.auth_tokens.issue_token(
             scope="string",
             expires_in="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "auth/issue-token"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "auth/issue-token"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"scope": scope, "expires_in": expires_in})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"scope": scope, "expires_in": expires_in}),
```

### Comparing `trycourier-6.0.2/src/courier/auth_tokens/types/issue_token_response.py` & `trycourier-6.0.3/src/courier/auth_tokens/types/issue_token_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/__init__.py` & `trycourier-6.0.3/src/courier/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/client.py` & `trycourier-6.0.3/src/courier/automations/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,25 +30,35 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AutomationInvokeResponse:
         """
         Invoke an automation run from an automation template.
 
-        Parameters:
-            - template_id: str. A unique identifier representing the automation template to be invoked. This could be the Automation Template ID or the Automation Template Alias.
+        Parameters
+        ----------
+        template_id : str
+            A unique identifier representing the automation template to be invoked. This could be the Automation Template ID or the Automation Template Alias.
 
-            - request: AutomationInvokeParams.
+        request : AutomationInvokeParams
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AutomationInvokeResponse
+
+        Examples
+        --------
         from courier import AutomationInvokeParams
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.automations.invoke_automation_template(
@@ -59,16 +69,16 @@
                 profile={"key": "value"},
                 recipient="string",
                 template="string",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"automations/{jsonable_encoder(template_id)}/invoke"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -107,23 +117,32 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AutomationInvokeResponse:
         """
         Invoke an ad hoc automation run. This endpoint accepts a JSON payload with a series of automation steps. For information about what steps are available, checkout the ad hoc automation guide [here](https://www.courier.com/docs/automations/steps/).
 
-        Parameters:
-            - request: AutomationAdHocInvokeParams.
+        Parameters
+        ----------
+        request : AutomationAdHocInvokeParams
+
+        idempotency_key : typing.Optional[str]
+
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        AutomationInvokeResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             Automation,
             AutomationAdHocInvokeParams,
             AutomationDelayStep,
             AutomationSendStep,
         )
         from courier.client import Courier
@@ -149,16 +168,16 @@
                         ),
                     ],
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "automations/invoke"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "automations/invoke"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -201,25 +220,35 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AutomationInvokeResponse:
         """
         Invoke an automation run from an automation template.
 
-        Parameters:
-            - template_id: str. A unique identifier representing the automation template to be invoked. This could be the Automation Template ID or the Automation Template Alias.
+        Parameters
+        ----------
+        template_id : str
+            A unique identifier representing the automation template to be invoked. This could be the Automation Template ID or the Automation Template Alias.
 
-            - request: AutomationInvokeParams.
+        request : AutomationInvokeParams
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AutomationInvokeResponse
+
+        Examples
+        --------
         from courier import AutomationInvokeParams
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.automations.invoke_automation_template(
@@ -230,16 +259,16 @@
                 profile={"key": "value"},
                 recipient="string",
                 template="string",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"automations/{jsonable_encoder(template_id)}/invoke"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -278,23 +307,32 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AutomationInvokeResponse:
         """
         Invoke an ad hoc automation run. This endpoint accepts a JSON payload with a series of automation steps. For information about what steps are available, checkout the ad hoc automation guide [here](https://www.courier.com/docs/automations/steps/).
 
-        Parameters:
-            - request: AutomationAdHocInvokeParams.
+        Parameters
+        ----------
+        request : AutomationAdHocInvokeParams
+
+        idempotency_key : typing.Optional[str]
+
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        AutomationInvokeResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             Automation,
             AutomationAdHocInvokeParams,
             AutomationDelayStep,
             AutomationSendStep,
         )
         from courier.client import AsyncCourier
@@ -320,16 +358,16 @@
                         ),
                     ],
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "automations/invoke"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "automations/invoke"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
```

### Comparing `trycourier-6.0.2/src/courier/automations/types/__init__.py` & `trycourier-6.0.3/src/courier/automations/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/accessor_type.py` & `trycourier-6.0.3/src/courier/automations/types/accessor_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation.py` & `trycourier-6.0.3/src/courier/automations/types/automation.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_ad_hoc_invoke_params.py` & `trycourier-6.0.3/src/courier/automations/types/automation_ad_hoc_invoke_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_retain.py` & `trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_retain.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from ...core.pydantic_utilities import pydantic_v1
 from .automation_add_to_batch_retain_type import AutomationAddToBatchRetainType
 
 
 class AutomationAddToBatchRetain(pydantic_v1.BaseModel):
     """
     Defines what items should be retained and passed along to the next steps when the batch is released
-    ---
+
+    Examples
+    --------
     from courier import AutomationAddToBatchRetain
 
     AutomationAddToBatchRetain(
         type="highest",
         count=10,
         sort_key="refs.data.my_custom_scoring",
     )
```

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_add_to_batch_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_add_to_batch_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from .automation_add_to_batch_retain import AutomationAddToBatchRetain
 from .automation_add_to_batch_scope import AutomationAddToBatchScope
 from .automation_step import AutomationStep
 
 
 class AutomationAddToBatchStep(AutomationStep):
     """
+    Examples
+    --------
     from courier import AutomationAddToBatchRetain, AutomationAddToBatchStep
 
     AutomationAddToBatchStep(
         action="add-to-batch",
         wait_period="PT5M",
         max_wait_period="PT1H",
         retain=AutomationAddToBatchRetain(
```

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_add_to_digest_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_add_to_digest_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 from .automation_step import AutomationStep
 
 
 class AutomationAddToDigestStep(AutomationStep):
     """
+    Examples
+    --------
     from courier import AutomationAddToDigestStep
 
     AutomationAddToDigestStep(
         action="add-to-digest",
         subscription_topic_id="RAJE97CMT04KDJJ88ZDS2TP1690S",
     )
     """
```

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_cancel_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_cancel_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_delay_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_delay_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_fetch_data_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .automation_fetch_data_webhook import AutomationFetchDataWebhook
 from .automation_step import AutomationStep
 from .merge_algorithm import MergeAlgorithm
 
 
 class AutomationFetchDataStep(AutomationStep):
     """
+    Examples
+    --------
     from courier import AutomationFetchDataStep, AutomationFetchDataWebhook
 
     AutomationFetchDataStep(
         action="fetch-data",
         merge_strategy="none",
         webhook=AutomationFetchDataWebhook(
             body={"foo": "bar"},
```

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_fetch_data_webhook.py` & `trycourier-6.0.3/src/courier/automations/types/automation_fetch_data_webhook.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_invoke_params.py` & `trycourier-6.0.3/src/courier/automations/types/automation_invoke_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_invoke_response.py` & `trycourier-6.0.3/src/courier/automations/types/automation_invoke_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_invoke_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_invoke_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_invoke_template_params.py` & `trycourier-6.0.3/src/courier/automations/types/automation_invoke_template_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_run_context.py` & `trycourier-6.0.3/src/courier/automations/types/automation_run_context.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_send_list_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_send_list_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_send_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_send_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_step_option.py` & `trycourier-6.0.3/src/courier/automations/types/automation_step_option.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_throttle_on_throttle.py` & `trycourier-6.0.3/src/courier/automations/types/automation_throttle_on_throttle.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_throttle_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_throttle_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .automation_step import AutomationStep
 from .automation_throttle_on_throttle import AutomationThrottleOnThrottle
 from .automation_throttle_scope import AutomationThrottleScope
 
 
 class AutomationThrottleStep(AutomationStep):
     """
+    Examples
+    --------
     from courier import AutomationThrottleOnThrottle, AutomationThrottleStep
 
     AutomationThrottleStep(
         action="throttle",
         max_allowed=1,
         period="PT5M",
         scope="dynamic",
```

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_update_profile_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_update_profile_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/automations/types/automation_v_2_send_step.py` & `trycourier-6.0.3/src/courier/automations/types/automation_v_2_send_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/client.py` & `trycourier-6.0.3/src/courier/brands/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,32 @@
         *,
         request: BrandParameters,
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Brand:
         """
-        Parameters:
-            - request: BrandParameters.
+        Parameters
+        ----------
+        request : BrandParameters
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Brand
+
+        Examples
+        --------
         from courier import BrandParameters, BrandSettings, BrandSnippets
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.brands.create(
@@ -62,16 +71,16 @@
                 name="string",
                 settings=BrandSettings(),
                 snippets=BrandSnippets(),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -107,31 +116,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Brand:
         """
         Fetch a specific brand by brand ID.
 
-        Parameters:
-            - brand_id: str. A unique identifier associated with the brand you wish to retrieve.
+        Parameters
+        ----------
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Brand
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.brands.get(
             brand_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -155,31 +173,40 @@
 
     def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> BrandsResponse:
         """
         Get the list of brands.
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of brands.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of brands.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        BrandsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.brands.list(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -210,31 +237,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Delete a brand by brand ID.
 
-        Parameters:
-            - brand_id: str. A unique identifier associated with the brand you wish to retrieve.
+        Parameters
+        ----------
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.brands.delete(
             brand_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -266,25 +302,35 @@
         settings: typing.Optional[BrandSettings] = OMIT,
         snippets: typing.Optional[BrandSnippets] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Brand:
         """
         Replace an existing brand with the supplied values.
 
-        Parameters:
-            - brand_id: str. A unique identifier associated with the brand you wish to update.
+        Parameters
+        ----------
+        brand_id : str
+            A unique identifier associated with the brand you wish to update.
+
+        name : str
+            The name of the brand.
+
+        settings : typing.Optional[BrandSettings]
 
-            - name: str. The name of the brand.
+        snippets : typing.Optional[BrandSnippets]
 
-            - settings: typing.Optional[BrandSettings].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - snippets: typing.Optional[BrandSnippets].
+        Returns
+        -------
+        Brand
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             BrandColors,
             BrandSettings,
             BrandSnippet,
             BrandSnippets,
             Email,
         )
@@ -314,16 +360,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if settings is not OMIT:
             _request["settings"] = settings
         if snippets is not OMIT:
             _request["snippets"] = snippets
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -361,23 +407,32 @@
         *,
         request: BrandParameters,
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Brand:
         """
-        Parameters:
-            - request: BrandParameters.
+        Parameters
+        ----------
+        request : BrandParameters
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Brand
+
+        Examples
+        --------
         from courier import BrandParameters, BrandSettings, BrandSnippets
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.brands.create(
@@ -386,16 +441,16 @@
                 name="string",
                 settings=BrandSettings(),
                 snippets=BrandSnippets(),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -431,31 +486,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Brand:
         """
         Fetch a specific brand by brand ID.
 
-        Parameters:
-            - brand_id: str. A unique identifier associated with the brand you wish to retrieve.
+        Parameters
+        ----------
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Brand
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.brands.get(
             brand_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -479,31 +543,40 @@
 
     async def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> BrandsResponse:
         """
         Get the list of brands.
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of brands.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of brands.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        BrandsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.brands.list(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -534,31 +607,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Delete a brand by brand ID.
 
-        Parameters:
-            - brand_id: str. A unique identifier associated with the brand you wish to retrieve.
+        Parameters
+        ----------
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.brands.delete(
             brand_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -590,25 +672,35 @@
         settings: typing.Optional[BrandSettings] = OMIT,
         snippets: typing.Optional[BrandSnippets] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Brand:
         """
         Replace an existing brand with the supplied values.
 
-        Parameters:
-            - brand_id: str. A unique identifier associated with the brand you wish to update.
+        Parameters
+        ----------
+        brand_id : str
+            A unique identifier associated with the brand you wish to update.
+
+        name : str
+            The name of the brand.
+
+        settings : typing.Optional[BrandSettings]
 
-            - name: str. The name of the brand.
+        snippets : typing.Optional[BrandSnippets]
 
-            - settings: typing.Optional[BrandSettings].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - snippets: typing.Optional[BrandSnippets].
+        Returns
+        -------
+        Brand
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             BrandColors,
             BrandSettings,
             BrandSnippet,
             BrandSnippets,
             Email,
         )
@@ -638,16 +730,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if settings is not OMIT:
             _request["settings"] = settings
         if snippets is not OMIT:
             _request["snippets"] = snippets
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
```

### Comparing `trycourier-6.0.2/src/courier/brands/types/__init__.py` & `trycourier-6.0.3/src/courier/brands/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand.py` & `trycourier-6.0.3/src/courier/brands/types/brand.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand_colors.py` & `trycourier-6.0.3/src/courier/brands/types/brand_colors.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand_get_all_response.py` & `trycourier-6.0.3/src/courier/brands/types/brand_get_all_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand_parameters.py` & `trycourier-6.0.3/src/courier/brands/types/brand_parameters.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand_settings.py` & `trycourier-6.0.3/src/courier/brands/types/brand_settings.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand_snippet.py` & `trycourier-6.0.3/src/courier/brands/types/brand_snippet.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brand_snippets.py` & `trycourier-6.0.3/src/courier/brands/types/brand_snippets.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/brands/types/brands_response.py` & `trycourier-6.0.3/src/courier/brands/types/brands_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/__init__.py` & `trycourier-6.0.3/src/courier/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/client.py` & `trycourier-6.0.3/src/courier/tenants/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,271 +8,301 @@
 from ..commons.types.bad_request import BadRequest
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
-from .types.bulk_create_job_response import BulkCreateJobResponse
-from .types.bulk_get_job_response import BulkGetJobResponse
-from .types.bulk_get_job_users_response import BulkGetJobUsersResponse
-from .types.bulk_ingest_users_params import BulkIngestUsersParams
-from .types.inbound_bulk_message import InboundBulkMessage
+from .types.default_preferences import DefaultPreferences
+from .types.list_users_for_tenant_response import ListUsersForTenantResponse
+from .types.template_property import TemplateProperty
+from .types.tenant import Tenant
+from .types.tenant_list_response import TenantListResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class BulkClient:
+class TenantsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def create_job(
+    def create_or_replace(
         self,
+        tenant_id: str,
         *,
-        message: InboundBulkMessage,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
+        name: str,
+        parent_tenant_id: typing.Optional[str] = OMIT,
+        default_preferences: typing.Optional[DefaultPreferences] = OMIT,
+        properties: typing.Optional[typing.Sequence[TemplateProperty]] = OMIT,
+        user_profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        brand_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkCreateJobResponse:
+    ) -> Tenant:
         """
-        Parameters:
-            - message: InboundBulkMessage.
+        Parameters
+        ----------
+        tenant_id : str
+            A unique identifier representing the tenant to be returned.
 
-            - idempotency_key: typing.Optional[str].
+        name : str
+            Name of the tenant.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        parent_tenant_id : typing.Optional[str]
+            Tenant's parent id (if any).
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from courier import InboundBulkMessage, InboundBulkTemplateMessage
+        default_preferences : typing.Optional[DefaultPreferences]
+            Defines the preferences used for the tenant when the user hasn't specified their own.
+
+        properties : typing.Optional[typing.Sequence[TemplateProperty]]
+            Arbitrary properties accessible to a template.
+
+        user_profile : typing.Optional[typing.Dict[str, typing.Any]]
+            A user profile object merged with user profile on send.
+
+        brand_id : typing.Optional[str]
+            Brand to be used for the account when one is not specified by the send call.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tenant
+
+        Examples
+        --------
+        from courier import DefaultPreferences, SubscriptionTopic
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.bulk.create_job(
-            message=InboundBulkMessage(
-                message=InboundBulkTemplateMessage(),
-                brand="string",
-                data={"string": {"key": "value"}},
-                event="string",
-                locale={"string": {"key": "value"}},
-                override={"key": "value"},
-            ),
-        )
-        """
+        client.tenants.create_or_replace(
+            tenant_id="string",
+            name="string",
+            parent_tenant_id="string",
+            default_preferences=DefaultPreferences(
+                items=[SubscriptionTopic()],
+            ),
+            properties=[{"key": "value"}],
+            user_profile={"string": {"key": "value"}},
+            brand_id="string",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if parent_tenant_id is not OMIT:
+            _request["parent_tenant_id"] = parent_tenant_id
+        if default_preferences is not OMIT:
+            _request["default_preferences"] = default_preferences
+        if properties is not OMIT:
+            _request["properties"] = properties
+        if user_profile is not OMIT:
+            _request["user_profile"] = user_profile
+        if brand_id is not OMIT:
+            _request["brand_id"] = brand_id
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "bulk"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"message": message})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"message": message}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkCreateJobResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def ingest_users(
-        self,
-        job_id: str,
-        *,
-        request: BulkIngestUsersParams,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    def get(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tenant:
         """
-        Ingest user data into a Bulk Job
-
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Parameters
+        ----------
+        tenant_id : str
+            A unique identifier representing the tenant to be returned.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tenant
 
-            - request: BulkIngestUsersParams.
-
-            - idempotency_key: typing.Optional[str].
-
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from courier import (
-            BulkIngestUsersParams,
-            InboundBulkMessageUser,
-            RecipientPreferences,
-            UserRecipient,
-        )
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.bulk.ingest_users(
-            job_id="string",
-            request=BulkIngestUsersParams(
-                users=[
-                    InboundBulkMessageUser(
-                        preferences=RecipientPreferences(),
-                        profile={"key": "value"},
-                        recipient="string",
-                        data={"key": "value"},
-                        to=UserRecipient(),
-                    )
-                ],
-            ),
+        client.tenants.get(
+            tenant_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def run_job(
+    def list(
         self,
-        job_id: str,
         *,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
+        limit: typing.Optional[int] = None,
+        cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    ) -> TenantListResponse:
         """
-        Run a bulk job
-
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Parameters
+        ----------
+        limit : typing.Optional[int]
+            The number of accousnts to return
+            (defaults to 20, maximum value of 100)
+
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        TenantListResponse
 
-            - idempotency_key: typing.Optional[str].
-
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.bulk.run_job(
-            job_id="string",
+        client.tenants.list(
+            limit=1,
+            cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/run"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tenants"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
-            if request_options is not None
-            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(TenantListResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_job(self, job_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> BulkGetJobResponse:
+    def delete(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Get a bulk job
-
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant to be deleted.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.bulk.get_job(
-            job_id="string",
+        client.tenants.delete(
+            tenant_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -283,48 +313,79 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_users(
-        self, job_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkGetJobUsersResponse:
+    def get_users_by_tenant(
+        self,
+        tenant_id: str,
+        *,
+        limit: typing.Optional[int] = None,
+        cursor: typing.Optional[str] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListUsersForTenantResponse:
         """
-        Get Bulk Job Users
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant for user membership.
+
+        limit : typing.Optional[int]
+            The number of accounts to return
+            (defaults to 20, maximum value of 100)
+
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Returns
+        -------
+        ListUsersForTenantResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.bulk.get_users(
-            job_id="string",
+        client.tenants.get_users_by_tenant(
+            tenant_id="string",
+            limit=1,
+            cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/users"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}/users"
+            ),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -333,273 +394,301 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobUsersResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncBulkClient:
+class AsyncTenantsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def create_job(
+    async def create_or_replace(
         self,
+        tenant_id: str,
         *,
-        message: InboundBulkMessage,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
+        name: str,
+        parent_tenant_id: typing.Optional[str] = OMIT,
+        default_preferences: typing.Optional[DefaultPreferences] = OMIT,
+        properties: typing.Optional[typing.Sequence[TemplateProperty]] = OMIT,
+        user_profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        brand_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkCreateJobResponse:
+    ) -> Tenant:
         """
-        Parameters:
-            - message: InboundBulkMessage.
+        Parameters
+        ----------
+        tenant_id : str
+            A unique identifier representing the tenant to be returned.
 
-            - idempotency_key: typing.Optional[str].
+        name : str
+            Name of the tenant.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        parent_tenant_id : typing.Optional[str]
+            Tenant's parent id (if any).
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from courier import InboundBulkMessage, InboundBulkTemplateMessage
+        default_preferences : typing.Optional[DefaultPreferences]
+            Defines the preferences used for the tenant when the user hasn't specified their own.
+
+        properties : typing.Optional[typing.Sequence[TemplateProperty]]
+            Arbitrary properties accessible to a template.
+
+        user_profile : typing.Optional[typing.Dict[str, typing.Any]]
+            A user profile object merged with user profile on send.
+
+        brand_id : typing.Optional[str]
+            Brand to be used for the account when one is not specified by the send call.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tenant
+
+        Examples
+        --------
+        from courier import DefaultPreferences, SubscriptionTopic
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.bulk.create_job(
-            message=InboundBulkMessage(
-                message=InboundBulkTemplateMessage(),
-                brand="string",
-                data={"string": {"key": "value"}},
-                event="string",
-                locale={"string": {"key": "value"}},
-                override={"key": "value"},
-            ),
-        )
-        """
+        await client.tenants.create_or_replace(
+            tenant_id="string",
+            name="string",
+            parent_tenant_id="string",
+            default_preferences=DefaultPreferences(
+                items=[SubscriptionTopic()],
+            ),
+            properties=[{"key": "value"}],
+            user_profile={"string": {"key": "value"}},
+            brand_id="string",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if parent_tenant_id is not OMIT:
+            _request["parent_tenant_id"] = parent_tenant_id
+        if default_preferences is not OMIT:
+            _request["default_preferences"] = default_preferences
+        if properties is not OMIT:
+            _request["properties"] = properties
+        if user_profile is not OMIT:
+            _request["user_profile"] = user_profile
+        if brand_id is not OMIT:
+            _request["brand_id"] = brand_id
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "bulk"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"message": message})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"message": message}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkCreateJobResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def ingest_users(
-        self,
-        job_id: str,
-        *,
-        request: BulkIngestUsersParams,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    async def get(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tenant:
         """
-        Ingest user data into a Bulk Job
-
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Parameters
+        ----------
+        tenant_id : str
+            A unique identifier representing the tenant to be returned.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tenant
 
-            - request: BulkIngestUsersParams.
-
-            - idempotency_key: typing.Optional[str].
-
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from courier import (
-            BulkIngestUsersParams,
-            InboundBulkMessageUser,
-            RecipientPreferences,
-            UserRecipient,
-        )
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.bulk.ingest_users(
-            job_id="string",
-            request=BulkIngestUsersParams(
-                users=[
-                    InboundBulkMessageUser(
-                        preferences=RecipientPreferences(),
-                        profile={"key": "value"},
-                        recipient="string",
-                        data={"key": "value"},
-                        to=UserRecipient(),
-                    )
-                ],
-            ),
+        await client.tenants.get(
+            tenant_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def run_job(
+    async def list(
         self,
-        job_id: str,
         *,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
+        limit: typing.Optional[int] = None,
+        cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    ) -> TenantListResponse:
         """
-        Run a bulk job
-
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Parameters
+        ----------
+        limit : typing.Optional[int]
+            The number of accousnts to return
+            (defaults to 20, maximum value of 100)
+
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        TenantListResponse
 
-            - idempotency_key: typing.Optional[str].
-
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.bulk.run_job(
-            job_id="string",
+        await client.tenants.list(
+            limit=1,
+            cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/run"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tenants"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
-            if request_options is not None
-            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(TenantListResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_job(
-        self, job_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkGetJobResponse:
+    async def delete(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Get a bulk job
-
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant to be deleted.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.bulk.get_job(
-            job_id="string",
+        await client.tenants.delete(
+            tenant_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -610,48 +699,79 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_users(
-        self, job_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkGetJobUsersResponse:
+    async def get_users_by_tenant(
+        self,
+        tenant_id: str,
+        *,
+        limit: typing.Optional[int] = None,
+        cursor: typing.Optional[str] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListUsersForTenantResponse:
         """
-        Get Bulk Job Users
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant for user membership.
+
+        limit : typing.Optional[int]
+            The number of accounts to return
+            (defaults to 20, maximum value of 100)
+
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - job_id: str. A unique identifier representing the bulk job
+        Returns
+        -------
+        ListUsersForTenantResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.bulk.get_users(
-            job_id="string",
+        await client.tenants.get_users_by_tenant(
+            tenant_id="string",
+            limit=1,
+            cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/users"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}/users"
+            ),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "limit": limit,
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -660,15 +780,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobUsersResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.2/src/courier/bulk/types/__init__.py` & `trycourier-6.0.3/src/courier/bulk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_create_job_response.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_create_job_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_params.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_response.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_users_params.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_get_job_users_response.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_get_job_users_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_ingest_error.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_error.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_ingest_users_params.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_ingest_users_response.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_ingest_users_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/bulk_message_user_response.py` & `trycourier-6.0.3/src/courier/bulk/types/bulk_message_user_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_content_message.py` & `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_content_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message.py` & `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message_user.py` & `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_user.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_message_v_1.py` & `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_message_v_1.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/inbound_bulk_template_message.py` & `trycourier-6.0.3/src/courier/bulk/types/inbound_bulk_template_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/bulk/types/job_details.py` & `trycourier-6.0.3/src/courier/bulk/types/job_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/client.py` & `trycourier-6.0.3/src/courier/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,29 +35,40 @@
 OMIT = typing.cast(typing.Any, ...)
 
 
 class Courier:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
 
-        - environment: CourierEnvironment. The environment to use for requests from the client. from .environment import CourierEnvironment
+    environment : CourierEnvironment
+        The environment to use for requests from the client. from .environment import CourierEnvironment
 
-                                           Defaults to CourierEnvironment.PRODUCTION
 
-        - authorization_token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+        Defaults to CourierEnvironment.PRODUCTION
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+
+    authorization_token : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.Client]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from courier.client import Courier
 
     client = Courier(
         authorization_token="YOUR_AUTHORIZATION_TOKEN",
     )
     """
 
@@ -66,15 +77,15 @@
         *,
         base_url: typing.Optional[str] = None,
         environment: CourierEnvironment = CourierEnvironment.PRODUCTION,
         authorization_token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = os.getenv(
             "COURIER_AUTH_TOKEN"
         ),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None,
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         if authorization_token is None:
             raise ApiError(
                 body="The client must be instantiated be either passing in authorization_token or setting COURIER_AUTH_TOKEN"
             )
@@ -110,23 +121,33 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SendMessageResponse:
         """
         Use the send API to send a message to one or more recipients.
 
-        Parameters:
-            - message: Message. Defines the message to be delivered
+        Parameters
+        ----------
+        message : Message
+            Defines the message to be delivered
+
+        idempotency_key : typing.Optional[str]
+
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        SendMessageResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             AudienceRecipient,
             Channel,
             ContentMessage,
             Delay,
             ElementalContent,
             Expiry,
@@ -155,16 +176,16 @@
                 delay=Delay(),
                 expiry=Expiry(),
                 to=AudienceRecipient(),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "send"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "send"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"message": message})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"message": message}),
@@ -195,29 +216,40 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCourier:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
 
-        - environment: CourierEnvironment. The environment to use for requests from the client. from .environment import CourierEnvironment
+    environment : CourierEnvironment
+        The environment to use for requests from the client. from .environment import CourierEnvironment
 
-                                           Defaults to CourierEnvironment.PRODUCTION
 
-        - authorization_token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+        Defaults to CourierEnvironment.PRODUCTION
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+
+    authorization_token : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.AsyncClient]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from courier.client import AsyncCourier
 
     client = AsyncCourier(
         authorization_token="YOUR_AUTHORIZATION_TOKEN",
     )
     """
 
@@ -226,15 +258,15 @@
         *,
         base_url: typing.Optional[str] = None,
         environment: CourierEnvironment = CourierEnvironment.PRODUCTION,
         authorization_token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = os.getenv(
             "COURIER_AUTH_TOKEN"
         ),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         if authorization_token is None:
             raise ApiError(
                 body="The client must be instantiated be either passing in authorization_token or setting COURIER_AUTH_TOKEN"
             )
@@ -270,23 +302,33 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SendMessageResponse:
         """
         Use the send API to send a message to one or more recipients.
 
-        Parameters:
-            - message: Message. Defines the message to be delivered
+        Parameters
+        ----------
+        message : Message
+            Defines the message to be delivered
+
+        idempotency_key : typing.Optional[str]
+
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        SendMessageResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             AudienceRecipient,
             Channel,
             ContentMessage,
             Delay,
             ElementalContent,
             Expiry,
@@ -315,16 +357,16 @@
                 delay=Delay(),
                 expiry=Expiry(),
                 to=AudienceRecipient(),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "send"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "send"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"message": message})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"message": message}),
```

### Comparing `trycourier-6.0.2/src/courier/commons/__init__.py` & `trycourier-6.0.3/src/courier/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/errors/__init__.py` & `trycourier-6.0.3/src/courier/commons/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/__init__.py` & `trycourier-6.0.3/src/courier/commons/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/already_exists.py` & `trycourier-6.0.3/src/courier/commons/types/already_exists.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/bad_request.py` & `trycourier-6.0.3/src/courier/commons/types/bad_request.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/base_error.py` & `trycourier-6.0.3/src/courier/commons/types/base_error.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/channel_preference.py` & `trycourier-6.0.3/src/courier/commons/types/channel_preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/conflict.py` & `trycourier-6.0.3/src/courier/commons/types/conflict.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/email.py` & `trycourier-6.0.3/src/courier/commons/types/email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/message_not_found.py` & `trycourier-6.0.3/src/courier/commons/types/message_not_found.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/not_found.py` & `trycourier-6.0.3/src/courier/commons/types/not_found.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/notification_preference_details.py` & `trycourier-6.0.3/src/courier/commons/types/notification_preference_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/paging.py` & `trycourier-6.0.3/src/courier/commons/types/paging.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/payment_required.py` & `trycourier-6.0.3/src/courier/commons/types/payment_required.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/recipient_preferences.py` & `trycourier-6.0.3/src/courier/commons/types/recipient_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/rule.py` & `trycourier-6.0.3/src/courier/commons/types/rule.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/commons/types/user_tenant_association.py` & `trycourier-6.0.3/src/courier/send/types/message_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,21 @@
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 
 
-class UserTenantAssociation(pydantic_v1.BaseModel):
-    user_id: str = pydantic_v1.Field()
+class MessageContext(pydantic_v1.BaseModel):
+    tenant_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    User ID for the assocation between tenant and user
+    An id of a tenant, see [tenants api docs](https://www.courier.com/docs/reference/tenants/).
+    Will load brand, default preferences and any other base context data associated with this tenant.
     """
 
-    type: typing.Literal["user"]
-    tenant_id: str = pydantic_v1.Field()
-    """
-    Tenant ID for the assocation between tenant and user
-    """
-
-    profile: typing.Dict[str, typing.Any]
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `trycourier-6.0.2/src/courier/core/__init__.py` & `trycourier-6.0.3/src/courier/core/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/core/client_wrapper.py` & `trycourier-6.0.3/src/courier/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "trycourier",
-            "X-Fern-SDK-Version": "v6.0.2",
+            "X-Fern-SDK-Version": "v6.0.3",
         }
         headers["Authorization"] = f"Bearer {self._get_authorization_token()}"
         return headers
 
     def _get_authorization_token(self) -> str:
         if isinstance(self._authorization_token, str):
             return self._authorization_token
```

### Comparing `trycourier-6.0.2/src/courier/core/datetime_utils.py` & `trycourier-6.0.3/src/courier/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/core/file.py` & `trycourier-6.0.3/src/courier/core/file.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/core/http_client.py` & `trycourier-6.0.3/src/courier/core/http_client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/core/jsonable_encoder.py` & `trycourier-6.0.3/src/courier/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/core/request_options.py` & `trycourier-6.0.3/src/courier/core/request_options.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/client.py` & `trycourier-6.0.3/src/courier/lists/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,34 +35,44 @@
         cursor: typing.Optional[str] = None,
         pattern: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListGetAllResponse:
         """
         Returns all of the lists, with the ability to filter based on a pattern.
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next page of lists.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next page of lists.
+
+        pattern : typing.Optional[str]
+            "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListGetAllResponse
 
-            - pattern: typing.Optional[str]. "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.list(
             cursor="string",
             pattern="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         "pattern": pattern,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -96,31 +106,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> List:
         """
         Returns a list based on the list ID provided.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        List
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.get(
             list_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -146,21 +165,30 @@
 
     def update(
         self, list_id: str, *, request: ListPutParams, request_options: typing.Optional[RequestOptions] = None
     ) -> List:
         """
         Create or replace an existing list with the supplied values.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - request: ListPutParams.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request : ListPutParams
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        List
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             ListPutParams,
             NotificationPreferenceDetails,
             RecipientPreferences,
             Rule,
         )
@@ -207,16 +235,16 @@
                         )
                     },
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -244,31 +272,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Delete a list by list ID.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.delete(
             list_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -290,31 +327,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def restore(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Restore a previously deleted list.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.restore(
             list_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/restore"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -347,34 +393,44 @@
         *,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListGetSubscriptionsResponse:
         """
         Get the list's subscriptions.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of list subscriptions
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of list subscriptions
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListGetSubscriptionsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.get_subscribers(
             list_id="string",
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
@@ -415,21 +471,30 @@
         *,
         request: typing.Sequence[PutSubscriptionsRecipient],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes the users to the list, overwriting existing subscriptions. If the list does not exist, it will be automatically created.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request : typing.Sequence[PutSubscriptionsRecipient]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request: typing.Sequence[PutSubscriptionsRecipient].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             NotificationPreferenceDetails,
             PutSubscriptionsRecipient,
             RecipientPreferences,
             Rule,
         )
@@ -478,16 +543,16 @@
                         },
                     ),
                 )
             ],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -527,25 +592,35 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes additional users to the list, without modifying existing subscriptions. If the list does not exist, it will be automatically created.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request : typing.Sequence[PutSubscriptionsRecipient]
 
-            - request: typing.Sequence[PutSubscriptionsRecipient].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             NotificationPreferenceDetails,
             PutSubscriptionsRecipient,
             RecipientPreferences,
             Rule,
         )
@@ -594,16 +669,16 @@
                         },
                     ),
                 )
             ],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -644,23 +719,33 @@
         *,
         preferences: typing.Optional[RecipientPreferences] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribe a user to an existing list (note: if the List does not exist, it will be automatically created).
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        user_id : str
+            A unique identifier representing the recipient associated with the list
 
-            - user_id: str. A unique identifier representing the recipient associated with the list
+        preferences : typing.Optional[RecipientPreferences]
 
-            - preferences: typing.Optional[RecipientPreferences].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             NotificationPreferenceDetails,
             RecipientPreferences,
             Rule,
         )
         from courier.client import Courier
@@ -707,16 +792,16 @@
             ),
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if preferences is not OMIT:
             _request["preferences"] = preferences
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -749,34 +834,44 @@
 
     def unsubscribe(
         self, list_id: str, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Delete a subscription to a list by list ID and user ID.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - user_id: str. A unique identifier representing the recipient associated with the list
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        user_id : str
+            A unique identifier representing the recipient associated with the list
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.unsubscribe(
             list_id="string",
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -814,34 +909,44 @@
         cursor: typing.Optional[str] = None,
         pattern: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListGetAllResponse:
         """
         Returns all of the lists, with the ability to filter based on a pattern.
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next page of lists.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next page of lists.
+
+        pattern : typing.Optional[str]
+            "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListGetAllResponse
 
-            - pattern: typing.Optional[str]. "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.list(
             cursor="string",
             pattern="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         "pattern": pattern,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -875,31 +980,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> List:
         """
         Returns a list based on the list ID provided.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        List
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.get(
             list_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -925,21 +1039,30 @@
 
     async def update(
         self, list_id: str, *, request: ListPutParams, request_options: typing.Optional[RequestOptions] = None
     ) -> List:
         """
         Create or replace an existing list with the supplied values.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - request: ListPutParams.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request : ListPutParams
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        List
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             ListPutParams,
             NotificationPreferenceDetails,
             RecipientPreferences,
             Rule,
         )
@@ -986,16 +1109,16 @@
                         )
                     },
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -1023,31 +1146,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Delete a list by list ID.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.delete(
             list_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -1069,31 +1201,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def restore(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Restore a previously deleted list.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.restore(
             list_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/restore"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -1126,34 +1267,44 @@
         *,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListGetSubscriptionsResponse:
         """
         Get the list's subscriptions.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of list subscriptions
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of list subscriptions
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListGetSubscriptionsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.get_subscribers(
             list_id="string",
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
@@ -1194,21 +1345,30 @@
         *,
         request: typing.Sequence[PutSubscriptionsRecipient],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes the users to the list, overwriting existing subscriptions. If the list does not exist, it will be automatically created.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request : typing.Sequence[PutSubscriptionsRecipient]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request: typing.Sequence[PutSubscriptionsRecipient].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             NotificationPreferenceDetails,
             PutSubscriptionsRecipient,
             RecipientPreferences,
             Rule,
         )
@@ -1257,16 +1417,16 @@
                         },
                     ),
                 )
             ],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -1306,25 +1466,35 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes additional users to the list, without modifying existing subscriptions. If the list does not exist, it will be automatically created.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        request : typing.Sequence[PutSubscriptionsRecipient]
 
-            - request: typing.Sequence[PutSubscriptionsRecipient].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             NotificationPreferenceDetails,
             PutSubscriptionsRecipient,
             RecipientPreferences,
             Rule,
         )
@@ -1373,16 +1543,16 @@
                         },
                     ),
                 )
             ],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -1423,23 +1593,33 @@
         *,
         preferences: typing.Optional[RecipientPreferences] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribe a user to an existing list (note: if the List does not exist, it will be automatically created).
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        user_id : str
+            A unique identifier representing the recipient associated with the list
 
-            - user_id: str. A unique identifier representing the recipient associated with the list
+        preferences : typing.Optional[RecipientPreferences]
 
-            - preferences: typing.Optional[RecipientPreferences].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             ChannelPreference,
             NotificationPreferenceDetails,
             RecipientPreferences,
             Rule,
         )
         from courier.client import AsyncCourier
@@ -1486,16 +1666,16 @@
             ),
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if preferences is not OMIT:
             _request["preferences"] = preferences
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -1528,34 +1708,44 @@
 
     async def unsubscribe(
         self, list_id: str, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Delete a subscription to a list by list ID and user ID.
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - user_id: str. A unique identifier representing the recipient associated with the list
+        Parameters
+        ----------
+        list_id : str
+            A unique identifier representing the list you wish to retrieve.
+
+        user_id : str
+            A unique identifier representing the recipient associated with the list
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.unsubscribe(
             list_id="string",
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
```

### Comparing `trycourier-6.0.2/src/courier/lists/types/__init__.py` & `trycourier-6.0.3/src/courier/lists/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/types/list.py` & `trycourier-6.0.3/src/courier/lists/types/list.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/types/list_get_all_response.py` & `trycourier-6.0.3/src/courier/lists/types/list_get_all_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/types/list_get_subscriptions_response.py` & `trycourier-6.0.3/src/courier/lists/types/list_get_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/types/list_put_params.py` & `trycourier-6.0.3/src/courier/lists/types/list_put_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/types/list_subscription_recipient.py` & `trycourier-6.0.3/src/courier/lists/types/list_subscription_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/lists/types/put_subscriptions_recipient.py` & `trycourier-6.0.3/src/courier/lists/types/put_subscriptions_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/__init__.py` & `trycourier-6.0.3/src/courier/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/client.py` & `trycourier-6.0.3/src/courier/messages/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,45 +42,67 @@
         enqueued_after: typing.Optional[str] = None,
         trace_id: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListMessagesResponse:
         """
         Fetch the statuses of messages you've previously sent.
 
-        Parameters:
-            - archived: typing.Optional[bool]. A boolean value that indicates whether archived messages should be included in the response.
+        Parameters
+        ----------
+        archived : typing.Optional[bool]
+            A boolean value that indicates whether archived messages should be included in the response.
 
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of messages.
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of messages.
 
-            - event: typing.Optional[str]. A unique identifier representing the event that was used to send the event.
+        event : typing.Optional[str]
+            A unique identifier representing the event that was used to send the event.
 
-            - list_: typing.Optional[str]. A unique identifier representing the list the message was sent to.
+        list_ : typing.Optional[str]
+            A unique identifier representing the list the message was sent to.
 
-            - message_id: typing.Optional[str]. A unique identifier representing the message_id returned from either /send or /send/list.
+        message_id : typing.Optional[str]
+            A unique identifier representing the message_id returned from either /send or /send/list.
 
-            - notification: typing.Optional[str]. A unique identifier representing the notification that was used to send the event.
+        notification : typing.Optional[str]
+            A unique identifier representing the notification that was used to send the event.
 
-            - provider: typing.Optional[typing.Union[str, typing.Sequence[str]]]. The key assocated to the provider you want to filter on. E.g., sendgrid, inbox, twilio, slack, msteams, etc. Allows multiple values to be set in query parameters.
+        provider : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            The key assocated to the provider you want to filter on. E.g., sendgrid, inbox, twilio, slack, msteams, etc. Allows multiple values to be set in query parameters.
 
-            - recipient: typing.Optional[str]. A unique identifier representing the recipient associated with the requested profile.
+        recipient : typing.Optional[str]
+            A unique identifier representing the recipient associated with the requested profile.
 
-            - status: typing.Optional[typing.Union[str, typing.Sequence[str]]]. An indicator of the current status of the message. Allows multiple values to be set in query parameters.
+        status : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            An indicator of the current status of the message. Allows multiple values to be set in query parameters.
 
-            - tag: typing.Optional[typing.Union[str, typing.Sequence[str]]]. A tag placed in the metadata.tags during a notification send. Allows multiple values to be set in query parameters.
+        tag : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            A tag placed in the metadata.tags during a notification send. Allows multiple values to be set in query parameters.
 
-            - tags: typing.Optional[str]. A comma delimited list of 'tags'. Messages will be returned if they match any of the tags passed in.
+        tags : typing.Optional[str]
+            A comma delimited list of 'tags'. Messages will be returned if they match any of the tags passed in.
 
-            - tenant_id: typing.Optional[str]. Messages sent with the context of a Tenant
+        tenant_id : typing.Optional[str]
+            Messages sent with the context of a Tenant
 
-            - enqueued_after: typing.Optional[str]. The enqueued datetime of a message to filter out messages received before.
+        enqueued_after : typing.Optional[str]
+            The enqueued datetime of a message to filter out messages received before.
 
-            - trace_id: typing.Optional[str]. The unique identifier used to trace the requests
+        trace_id : typing.Optional[str]
+            The unique identifier used to trace the requests
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListMessagesResponse
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.messages.list(
             archived=True,
@@ -96,16 +118,16 @@
             tags="string",
             tenant_id="string",
             enqueued_after="string",
             trace_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "archived": archived,
                         "cursor": cursor,
                         "event": event,
                         "list": list_,
@@ -149,31 +171,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, message_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> MessageDetails:
         """
         Fetch the status of a message you've previously sent.
 
-        Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier associated with the message you wish to retrieve (results from a send).
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        MessageDetails
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.messages.get(
             message_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -206,35 +239,45 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MessageDetails:
         """
         Cancel a message that is currently in the process of being delivered. A well-formatted API call to the cancel message API will return either `200` status code for a successful cancellation or `409` status code for an unsuccessful cancellation. Both cases will include the actual message record in the response body (see details below).
 
-        Parameters:
-            - message_id: str. A unique identifier representing the message ID
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier representing the message ID
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        MessageDetails
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.messages.cancel(
             message_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/cancel"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -269,34 +312,44 @@
         *,
         type: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MessageHistoryResponse:
         """
         Fetch the array of events of a message you've previously sent.
 
-        Parameters:
-            - message_id: str. A unique identifier representing the message ID
-
-            - type: typing.Optional[str]. A supported Message History type that will filter the events returned.
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier representing the message ID
+
+        type : typing.Optional[str]
+            A supported Message History type that will filter the events returned.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        MessageHistoryResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.messages.get_history(
             message_id="string",
             type="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/history"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "type": type,
                         **(
@@ -333,31 +386,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_content(
         self, message_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> RenderOutputResponse:
         """
-        Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier associated with the message you wish to retrieve (results from a send).
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RenderOutputResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.messages.get_content(
             message_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/output"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -383,31 +445,40 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def archive(self, request_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Parameters:
-            - request_id: str. A unique identifier representing the request ID
+        Parameters
+        ----------
+        request_id : str
+            A unique identifier representing the request ID
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.messages.archive(
             request_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"requests/{jsonable_encoder(request_id)}/archive"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -457,45 +528,67 @@
         enqueued_after: typing.Optional[str] = None,
         trace_id: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListMessagesResponse:
         """
         Fetch the statuses of messages you've previously sent.
 
-        Parameters:
-            - archived: typing.Optional[bool]. A boolean value that indicates whether archived messages should be included in the response.
+        Parameters
+        ----------
+        archived : typing.Optional[bool]
+            A boolean value that indicates whether archived messages should be included in the response.
 
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of messages.
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of messages.
 
-            - event: typing.Optional[str]. A unique identifier representing the event that was used to send the event.
+        event : typing.Optional[str]
+            A unique identifier representing the event that was used to send the event.
 
-            - list_: typing.Optional[str]. A unique identifier representing the list the message was sent to.
+        list_ : typing.Optional[str]
+            A unique identifier representing the list the message was sent to.
 
-            - message_id: typing.Optional[str]. A unique identifier representing the message_id returned from either /send or /send/list.
+        message_id : typing.Optional[str]
+            A unique identifier representing the message_id returned from either /send or /send/list.
 
-            - notification: typing.Optional[str]. A unique identifier representing the notification that was used to send the event.
+        notification : typing.Optional[str]
+            A unique identifier representing the notification that was used to send the event.
 
-            - provider: typing.Optional[typing.Union[str, typing.Sequence[str]]]. The key assocated to the provider you want to filter on. E.g., sendgrid, inbox, twilio, slack, msteams, etc. Allows multiple values to be set in query parameters.
+        provider : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            The key assocated to the provider you want to filter on. E.g., sendgrid, inbox, twilio, slack, msteams, etc. Allows multiple values to be set in query parameters.
 
-            - recipient: typing.Optional[str]. A unique identifier representing the recipient associated with the requested profile.
+        recipient : typing.Optional[str]
+            A unique identifier representing the recipient associated with the requested profile.
 
-            - status: typing.Optional[typing.Union[str, typing.Sequence[str]]]. An indicator of the current status of the message. Allows multiple values to be set in query parameters.
+        status : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            An indicator of the current status of the message. Allows multiple values to be set in query parameters.
 
-            - tag: typing.Optional[typing.Union[str, typing.Sequence[str]]]. A tag placed in the metadata.tags during a notification send. Allows multiple values to be set in query parameters.
+        tag : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            A tag placed in the metadata.tags during a notification send. Allows multiple values to be set in query parameters.
 
-            - tags: typing.Optional[str]. A comma delimited list of 'tags'. Messages will be returned if they match any of the tags passed in.
+        tags : typing.Optional[str]
+            A comma delimited list of 'tags'. Messages will be returned if they match any of the tags passed in.
 
-            - tenant_id: typing.Optional[str]. Messages sent with the context of a Tenant
+        tenant_id : typing.Optional[str]
+            Messages sent with the context of a Tenant
 
-            - enqueued_after: typing.Optional[str]. The enqueued datetime of a message to filter out messages received before.
+        enqueued_after : typing.Optional[str]
+            The enqueued datetime of a message to filter out messages received before.
 
-            - trace_id: typing.Optional[str]. The unique identifier used to trace the requests
+        trace_id : typing.Optional[str]
+            The unique identifier used to trace the requests
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListMessagesResponse
+
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.messages.list(
             archived=True,
@@ -511,16 +604,16 @@
             tags="string",
             tenant_id="string",
             enqueued_after="string",
             trace_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "archived": archived,
                         "cursor": cursor,
                         "event": event,
                         "list": list_,
@@ -564,31 +657,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, message_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> MessageDetails:
         """
         Fetch the status of a message you've previously sent.
 
-        Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier associated with the message you wish to retrieve (results from a send).
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        MessageDetails
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.messages.get(
             message_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -621,35 +725,45 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MessageDetails:
         """
         Cancel a message that is currently in the process of being delivered. A well-formatted API call to the cancel message API will return either `200` status code for a successful cancellation or `409` status code for an unsuccessful cancellation. Both cases will include the actual message record in the response body (see details below).
 
-        Parameters:
-            - message_id: str. A unique identifier representing the message ID
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier representing the message ID
 
-            - idempotency_key: typing.Optional[str].
+        idempotency_key : typing.Optional[str]
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        MessageDetails
+
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.messages.cancel(
             message_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/cancel"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -684,34 +798,44 @@
         *,
         type: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MessageHistoryResponse:
         """
         Fetch the array of events of a message you've previously sent.
 
-        Parameters:
-            - message_id: str. A unique identifier representing the message ID
-
-            - type: typing.Optional[str]. A supported Message History type that will filter the events returned.
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier representing the message ID
+
+        type : typing.Optional[str]
+            A supported Message History type that will filter the events returned.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        MessageHistoryResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.messages.get_history(
             message_id="string",
             type="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/history"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "type": type,
                         **(
@@ -748,31 +872,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_content(
         self, message_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> RenderOutputResponse:
         """
-        Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
+        Parameters
+        ----------
+        message_id : str
+            A unique identifier associated with the message you wish to retrieve (results from a send).
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RenderOutputResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.messages.get_content(
             message_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/output"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -798,31 +931,40 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def archive(self, request_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Parameters:
-            - request_id: str. A unique identifier representing the request ID
+        Parameters
+        ----------
+        request_id : str
+            A unique identifier representing the request ID
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.messages.archive(
             request_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"requests/{jsonable_encoder(request_id)}/archive"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
```

### Comparing `trycourier-6.0.2/src/courier/messages/types/__init__.py` & `trycourier-6.0.3/src/courier/messages/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/list_messages_response.py` & `trycourier-6.0.3/src/courier/messages/types/list_messages_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/message_details.py` & `trycourier-6.0.3/src/courier/messages/types/message_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/message_history_response.py` & `trycourier-6.0.3/src/courier/messages/types/message_history_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/render_output.py` & `trycourier-6.0.3/src/courier/messages/types/render_output.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/render_output_response.py` & `trycourier-6.0.3/src/courier/messages/types/render_output_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/rendered_message_block.py` & `trycourier-6.0.3/src/courier/messages/types/rendered_message_block.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/messages/types/rendered_message_content.py` & `trycourier-6.0.3/src/courier/messages/types/rendered_message_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/__init__.py` & `trycourier-6.0.3/src/courier/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/client.py` & `trycourier-6.0.3/src/courier/notifications/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,31 +26,39 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationListResponse:
         """
-        Parameters:
-            - cursor: typing.Optional[str].
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NotificationListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.notifications.list(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -81,31 +89,39 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_content(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationGetContentResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NotificationGetContentResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.notifications.get_content(
             id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/content"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -129,31 +145,39 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_draft_content(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationGetContentResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NotificationGetContentResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.notifications.get_draft_content(
             id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/content"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -182,23 +206,31 @@
         id: str,
         *,
         blocks: typing.Optional[typing.Sequence[NotificationBlock]] = OMIT,
         channels: typing.Optional[typing.Sequence[NotificationChannel]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
 
-            - blocks: typing.Optional[typing.Sequence[NotificationBlock]].
+        blocks : typing.Optional[typing.Sequence[NotificationBlock]]
 
-            - channels: typing.Optional[typing.Sequence[NotificationChannel]].
+        channels : typing.Optional[typing.Sequence[NotificationChannel]]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             NotificationBlock,
             NotificationChannel,
             NotificationChannelContent,
         )
         from courier.client import Courier
 
@@ -231,16 +263,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {}
         if blocks is not OMIT:
             _request["blocks"] = blocks
         if channels is not OMIT:
             _request["channels"] = channels
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/variations"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -275,23 +307,31 @@
         id: str,
         *,
         blocks: typing.Optional[typing.Sequence[NotificationBlock]] = OMIT,
         channels: typing.Optional[typing.Sequence[NotificationChannel]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        blocks : typing.Optional[typing.Sequence[NotificationBlock]]
 
-            - blocks: typing.Optional[typing.Sequence[NotificationBlock]].
+        channels : typing.Optional[typing.Sequence[NotificationChannel]]
 
-            - channels: typing.Optional[typing.Sequence[NotificationChannel]].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             NotificationBlock,
             NotificationChannel,
             NotificationChannelContent,
         )
         from courier.client import Courier
 
@@ -324,16 +364,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {}
         if blocks is not OMIT:
             _request["blocks"] = blocks
         if channels is not OMIT:
             _request["channels"] = channels
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/variations"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -363,34 +403,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_submission_checks(
         self, id: str, submission_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SubmissionChecksGetResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        submission_id : str
 
-            - submission_id: str.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        SubmissionChecksGetResponse
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.notifications.get_submission_checks(
             id="string",
             submission_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -420,23 +468,31 @@
         id: str,
         submission_id: str,
         *,
         checks: typing.Sequence[BaseCheck],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SubmissionChecksReplaceResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        submission_id : str
+
+        checks : typing.Sequence[BaseCheck]
 
-            - submission_id: str.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - checks: typing.Sequence[BaseCheck].
+        Returns
+        -------
+        SubmissionChecksReplaceResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import BaseCheck
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.notifications.replace_submission_checks(
@@ -448,16 +504,16 @@
                     status="RESOLVED",
                     type="custom",
                 )
             ],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"checks": checks})
@@ -488,34 +544,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel_submission(
         self, id: str, submission_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        submission_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - submission_id: str.
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.notifications.cancel_submission(
             id="string",
             submission_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -545,31 +609,39 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationListResponse:
         """
-        Parameters:
-            - cursor: typing.Optional[str].
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NotificationListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.notifications.list(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -600,31 +672,39 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_content(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationGetContentResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NotificationGetContentResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.notifications.get_content(
             id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/content"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -648,31 +728,39 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_draft_content(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationGetContentResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NotificationGetContentResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.notifications.get_draft_content(
             id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/content"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -701,23 +789,31 @@
         id: str,
         *,
         blocks: typing.Optional[typing.Sequence[NotificationBlock]] = OMIT,
         channels: typing.Optional[typing.Sequence[NotificationChannel]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
 
-            - blocks: typing.Optional[typing.Sequence[NotificationBlock]].
+        blocks : typing.Optional[typing.Sequence[NotificationBlock]]
 
-            - channels: typing.Optional[typing.Sequence[NotificationChannel]].
+        channels : typing.Optional[typing.Sequence[NotificationChannel]]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             NotificationBlock,
             NotificationChannel,
             NotificationChannelContent,
         )
         from courier.client import AsyncCourier
 
@@ -750,16 +846,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {}
         if blocks is not OMIT:
             _request["blocks"] = blocks
         if channels is not OMIT:
             _request["channels"] = channels
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/variations"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -794,23 +890,31 @@
         id: str,
         *,
         blocks: typing.Optional[typing.Sequence[NotificationBlock]] = OMIT,
         channels: typing.Optional[typing.Sequence[NotificationChannel]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        blocks : typing.Optional[typing.Sequence[NotificationBlock]]
 
-            - blocks: typing.Optional[typing.Sequence[NotificationBlock]].
+        channels : typing.Optional[typing.Sequence[NotificationChannel]]
 
-            - channels: typing.Optional[typing.Sequence[NotificationChannel]].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier import (
             NotificationBlock,
             NotificationChannel,
             NotificationChannelContent,
         )
         from courier.client import AsyncCourier
 
@@ -843,16 +947,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {}
         if blocks is not OMIT:
             _request["blocks"] = blocks
         if channels is not OMIT:
             _request["channels"] = channels
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/variations"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -882,34 +986,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_submission_checks(
         self, id: str, submission_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SubmissionChecksGetResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        submission_id : str
 
-            - submission_id: str.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        SubmissionChecksGetResponse
+
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.notifications.get_submission_checks(
             id="string",
             submission_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -939,23 +1051,31 @@
         id: str,
         submission_id: str,
         *,
         checks: typing.Sequence[BaseCheck],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SubmissionChecksReplaceResponse:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        submission_id : str
+
+        checks : typing.Sequence[BaseCheck]
 
-            - submission_id: str.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - checks: typing.Sequence[BaseCheck].
+        Returns
+        -------
+        SubmissionChecksReplaceResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import BaseCheck
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.notifications.replace_submission_checks(
@@ -967,16 +1087,16 @@
                     status="RESOLVED",
                     type="custom",
                 )
             ],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"checks": checks})
@@ -1007,34 +1127,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel_submission(
         self, id: str, submission_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        submission_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - submission_id: str.
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.notifications.cancel_submission(
             id="string",
             submission_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
```

### Comparing `trycourier-6.0.2/src/courier/notifications/types/__init__.py` & `trycourier-6.0.3/src/courier/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/base_check.py` & `trycourier-6.0.3/src/courier/notifications/types/base_check.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/check.py` & `trycourier-6.0.3/src/courier/notifications/types/check.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/message_routing.py` & `trycourier-6.0.3/src/courier/notifications/types/message_routing.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification.py` & `trycourier-6.0.3/src/courier/notifications/types/notification.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification_block.py` & `trycourier-6.0.3/src/courier/notifications/types/notification_block.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification_channel.py` & `trycourier-6.0.3/src/courier/notifications/types/notification_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification_channel_content.py` & `trycourier-6.0.3/src/courier/notifications/types/notification_channel_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification_content_hierarchy.py` & `trycourier-6.0.3/src/courier/notifications/types/notification_content_hierarchy.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification_get_content_response.py` & `trycourier-6.0.3/src/courier/notifications/types/notification_get_content_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/notification_list_response.py` & `trycourier-6.0.3/src/courier/notifications/types/notification_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/submission_checks_get_response.py` & `trycourier-6.0.3/src/courier/notifications/types/submission_checks_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/notifications/types/submission_checks_replace_response.py` & `trycourier-6.0.3/src/courier/notifications/types/submission_checks_replace_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/__init__.py` & `trycourier-6.0.3/src/courier/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/client.py` & `trycourier-6.0.3/src/courier/profiles/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,31 +28,42 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ProfileGetResponse:
         """
         Returns the specified user profile.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ProfileGetResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.get(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -84,38 +95,50 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MergeProfileResponse:
         """
         Merge the supplied values with an existing profile or create a new profile if one doesn't already exist.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        profile : typing.Dict[str, typing.Any]
+
+        idempotency_key : typing.Optional[str]
 
-            - profile: typing.Dict[str, typing.Any].
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        MergeProfileResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.create(
             user_id="string",
             profile={"string": {"key": "value"}},
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
@@ -156,34 +179,45 @@
     ) -> ReplaceProfileResponse:
         """
         When using `PUT`, be sure to include all the key-value pairs required by the recipient's profile.
         Any key-value pairs that exist in the profile but fail to be included in the `PUT` request will be
         removed from the profile. Remember, a `PUT` update is a full replacement of the data. For partial updates,
         use the [Patch](https://www.courier.com/docs/reference/profiles/patch/) request.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
-
-            - profile: typing.Dict[str, typing.Any].
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        profile : typing.Dict[str, typing.Any]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ReplaceProfileResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.replace(
             user_id="string",
             profile={"string": {"key": "value"}},
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
@@ -213,31 +247,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Deletes the specified user profile.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.delete(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -267,34 +312,44 @@
         *,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetListSubscriptionsResponse:
         """
         Returns the subscribed lists for a specified user.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of message statuses.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of message statuses.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetListSubscriptionsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.get_list_subscriptions(
             user_id="string",
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
@@ -337,41 +392,51 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SubscribeToListsResponse:
         """
         Subscribes the given user to one or more lists. If the list does not exist, it will be created.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request : SubscribeToListsRequest
+
+        idempotency_key : typing.Optional[str]
 
-            - request: SubscribeToListsRequest.
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        SubscribeToListsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import SubscribeToListsRequest, SubscribeToListsRequestListObject
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.subscribe_to_lists(
             user_id="string",
             request=SubscribeToListsRequest(
                 lists=[SubscribeToListsRequestListObject()],
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -407,31 +472,40 @@
 
     def delete_list_subscription(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DeleteListSubscriptionResponse:
         """
         Removes all list subscriptions for given user.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteListSubscriptionResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.profiles.delete_list_subscription(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -462,31 +536,42 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ProfileGetResponse:
         """
         Returns the specified user profile.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ProfileGetResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.get(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -518,38 +603,50 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MergeProfileResponse:
         """
         Merge the supplied values with an existing profile or create a new profile if one doesn't already exist.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        profile : typing.Dict[str, typing.Any]
+
+        idempotency_key : typing.Optional[str]
 
-            - profile: typing.Dict[str, typing.Any].
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        MergeProfileResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.create(
             user_id="string",
             profile={"string": {"key": "value"}},
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
@@ -590,34 +687,45 @@
     ) -> ReplaceProfileResponse:
         """
         When using `PUT`, be sure to include all the key-value pairs required by the recipient's profile.
         Any key-value pairs that exist in the profile but fail to be included in the `PUT` request will be
         removed from the profile. Remember, a `PUT` update is a full replacement of the data. For partial updates,
         use the [Patch](https://www.courier.com/docs/reference/profiles/patch/) request.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
-
-            - profile: typing.Dict[str, typing.Any].
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        profile : typing.Dict[str, typing.Any]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ReplaceProfileResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.replace(
             user_id="string",
             profile={"string": {"key": "value"}},
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
@@ -647,31 +755,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Deletes the specified user profile.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.delete(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -701,34 +820,44 @@
         *,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetListSubscriptionsResponse:
         """
         Returns the subscribed lists for a specified user.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of message statuses.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of message statuses.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetListSubscriptionsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.get_list_subscriptions(
             user_id="string",
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
@@ -771,41 +900,51 @@
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SubscribeToListsResponse:
         """
         Subscribes the given user to one or more lists. If the list does not exist, it will be created.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request : SubscribeToListsRequest
+
+        idempotency_key : typing.Optional[str]
 
-            - request: SubscribeToListsRequest.
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
-            - idempotency_key: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - idempotency_expiry: typing.Optional[str]. The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        Returns
+        -------
+        SubscribeToListsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier import SubscribeToListsRequest, SubscribeToListsRequestListObject
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.subscribe_to_lists(
             user_id="string",
             request=SubscribeToListsRequest(
                 lists=[SubscribeToListsRequestListObject()],
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
@@ -841,31 +980,40 @@
 
     async def delete_list_subscription(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DeleteListSubscriptionResponse:
         """
         Removes all list subscriptions for given user.
 
-        Parameters:
-            - user_id: str. A unique identifier representing the user associated with the requested profile.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier representing the user associated with the requested profile.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteListSubscriptionResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.profiles.delete_list_subscription(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
```

### Comparing `trycourier-6.0.2/src/courier/profiles/types/__init__.py` & `trycourier-6.0.3/src/courier/profiles/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/address.py` & `trycourier-6.0.3/src/courier/profiles/types/address.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/airship_profile.py` & `trycourier-6.0.3/src/courier/profiles/types/airship_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/airship_profile_audience.py` & `trycourier-6.0.3/src/courier/profiles/types/airship_profile_audience.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/delete_list_subscription_response.py` & `trycourier-6.0.3/src/courier/profiles/types/delete_list_subscription_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/get_list_subscriptions_list.py` & `trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_list.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/get_list_subscriptions_response.py` & `trycourier-6.0.3/src/courier/profiles/types/get_list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/intercom.py` & `trycourier-6.0.3/src/courier/profiles/types/intercom.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/intercom_recipient.py` & `trycourier-6.0.3/src/courier/profiles/types/intercom_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/merge_profile_response.py` & `trycourier-6.0.3/src/courier/profiles/types/merge_profile_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/ms_teams.py` & `trycourier-6.0.3/src/courier/profiles/types/ms_teams.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/ms_teams_base_properties.py` & `trycourier-6.0.3/src/courier/profiles/types/ms_teams_base_properties.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/multiple_tokens.py` & `trycourier-6.0.3/src/courier/profiles/types/multiple_tokens.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/profile_get_parameters.py` & `trycourier-6.0.3/src/courier/profiles/types/profile_get_parameters.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/profile_get_response.py` & `trycourier-6.0.3/src/courier/profiles/types/profile_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/replace_profile_response.py` & `trycourier-6.0.3/src/courier/profiles/types/replace_profile_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_direct_message.py` & `trycourier-6.0.3/src/courier/profiles/types/send_direct_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_channel.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_channel_id.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_channel_name.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_channel_name.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_conversation_id.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_conversation_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_email.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_ms_teams_user_id.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_ms_teams_user_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_slack_channel.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_slack_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_slack_email.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_slack_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/send_to_slack_user_id.py` & `trycourier-6.0.3/src/courier/profiles/types/send_to_slack_user_id.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/slack_base_properties.py` & `trycourier-6.0.3/src/courier/profiles/types/slack_base_properties.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/snooze_rule.py` & `trycourier-6.0.3/src/courier/profiles/types/snooze_rule.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/subscribe_to_lists_request.py` & `trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/subscribe_to_lists_request_list_object.py` & `trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_request_list_object.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/subscribe_to_lists_response.py` & `trycourier-6.0.3/src/courier/profiles/types/subscribe_to_lists_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/token.py` & `trycourier-6.0.3/src/courier/profiles/types/token.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/profiles/types/user_profile.py` & `trycourier-6.0.3/src/courier/profiles/types/user_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/__init__.py` & `trycourier-6.0.3/src/courier/send/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/__init__.py` & `trycourier-6.0.3/src/courier/send/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/audience_filter.py` & `trycourier-6.0.3/src/courier/send/types/audience_filter.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/audience_recipient.py` & `trycourier-6.0.3/src/courier/send/types/audience_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/base_message.py` & `trycourier-6.0.3/src/courier/send/types/base_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/base_message_send_to.py` & `trycourier-6.0.3/src/courier/send/types/base_message_send_to.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/base_social_presence.py` & `trycourier-6.0.3/src/courier/send/types/base_social_presence.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/brand_settings_email.py` & `trycourier-6.0.3/src/courier/send/types/brand_settings_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/brand_settings_in_app.py` & `trycourier-6.0.3/src/courier/send/types/brand_settings_in_app.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/brand_settings_social_presence.py` & `trycourier-6.0.3/src/courier/send/types/brand_settings_social_presence.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/brand_template.py` & `trycourier-6.0.3/src/courier/send/types/brand_template.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/brand_template_override.py` & `trycourier-6.0.3/src/courier/send/types/brand_template_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/channel.py` & `trycourier-6.0.3/src/courier/send/types/channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/channel_metadata.py` & `trycourier-6.0.3/src/courier/send/types/channel_metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/content_message.py` & `trycourier-6.0.3/src/courier/send/types/content_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/delay.py` & `trycourier-6.0.3/src/courier/send/types/delay.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_action_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_action_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_base_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_base_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_channel_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_channel_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_content.py` & `trycourier-6.0.3/src/courier/send/types/elemental_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_content_sugar.py` & `trycourier-6.0.3/src/courier/send/types/elemental_content_sugar.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_divider_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_divider_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_group_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_group_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_image_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_image_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_meta_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_meta_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_quote_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_quote_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/elemental_text_node.py` & `trycourier-6.0.3/src/courier/send/types/elemental_text_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/email_footer.py` & `trycourier-6.0.3/src/courier/send/types/email_footer.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/email_head.py` & `trycourier-6.0.3/src/courier/send/types/email_head.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/email_header.py` & `trycourier-6.0.3/src/courier/send/types/email_header.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/expiry.py` & `trycourier-6.0.3/src/courier/send/types/expiry.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/i_profile_preferences.py` & `trycourier-6.0.3/src/courier/send/types/i_profile_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/icons.py` & `trycourier-6.0.3/src/courier/send/types/icons.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/invalid_list_pattern_recipient.py` & `trycourier-6.0.3/src/courier/send/types/invalid_list_pattern_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/invalid_list_recipient.py` & `trycourier-6.0.3/src/courier/send/types/invalid_list_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/invalid_user_recipient.py` & `trycourier-6.0.3/src/courier/send/types/invalid_user_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/list_filter.py` & `trycourier-6.0.3/src/courier/send/types/list_filter.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/list_pattern_recipient.py` & `trycourier-6.0.3/src/courier/send/types/list_pattern_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/list_pattern_recipient_type.py` & `trycourier-6.0.3/src/courier/send/types/list_pattern_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/list_recipient.py` & `trycourier-6.0.3/src/courier/send/types/list_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/list_recipient_type.py` & `trycourier-6.0.3/src/courier/send/types/list_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/locale.py` & `trycourier-6.0.3/src/courier/send/types/locale.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/logo.py` & `trycourier-6.0.3/src/courier/send/types/logo.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/message_channel_email_override.py` & `trycourier-6.0.3/src/courier/send/types/message_channel_email_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/message_context.py` & `trycourier-6.0.3/src/courier/templates/types/routing_strategy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from .channel_identifier import ChannelIdentifier
+from .routing_strategy_method import RoutingStrategyMethod
 
 
-class MessageContext(pydantic_v1.BaseModel):
-    tenant_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+class RoutingStrategy(pydantic_v1.BaseModel):
+    method: RoutingStrategyMethod = pydantic_v1.Field()
     """
-    An id of a tenant, see [tenants api docs](https://www.courier.com/docs/reference/tenants/).
-    Will load brand, default preferences and any other base context data associated with this tenant.
+    The method for selecting channels to send the message with. Value can be either 'single' or 'all'. If not provided will default to 'single'
+    """
+
+    channels: typing.List[ChannelIdentifier] = pydantic_v1.Field()
+    """
+    An array of valid channel identifiers (like email, push, sms, etc.) and additional routing nodes.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.2/src/courier/send/types/message_metadata.py` & `trycourier-6.0.3/src/courier/send/types/message_metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/message_providers_type.py` & `trycourier-6.0.3/src/courier/send/types/message_providers_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/metadata.py` & `trycourier-6.0.3/src/courier/send/types/metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/ms_teams_recipient.py` & `trycourier-6.0.3/src/courier/send/types/ms_teams_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/preference.py` & `trycourier-6.0.3/src/courier/send/types/preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/preferences.py` & `trycourier-6.0.3/src/courier/send/types/preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/recipient.py` & `trycourier-6.0.3/src/courier/send/types/recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/routing.py` & `trycourier-6.0.3/src/courier/send/types/routing.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/routing_strategy_channel.py` & `trycourier-6.0.3/src/courier/send/types/routing_strategy_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/routing_strategy_provider.py` & `trycourier-6.0.3/src/courier/send/types/routing_strategy_provider.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/slack_recipient.py` & `trycourier-6.0.3/src/courier/send/types/slack_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/template_message.py` & `trycourier-6.0.3/src/courier/send/types/template_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/timeout.py` & `trycourier-6.0.3/src/courier/send/types/timeout.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/timeouts.py` & `trycourier-6.0.3/src/courier/send/types/timeouts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/tracking_override.py` & `trycourier-6.0.3/src/courier/send/types/tracking_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/user_recipient.py` & `trycourier-6.0.3/src/courier/send/types/user_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/user_recipient_type.py` & `trycourier-6.0.3/src/courier/send/types/user_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/utm.py` & `trycourier-6.0.3/src/courier/send/types/utm.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/send/types/widget_background.py` & `trycourier-6.0.3/src/courier/send/types/widget_background.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/templates/client.py` & `trycourier-6.0.3/src/courier/templates/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,31 +19,40 @@
 
     def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListTemplatesResponse:
         """
         Returns a list of notification templates
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of templates
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of templates
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListTemplatesResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.templates.list(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
@@ -81,31 +90,40 @@
 
     async def list(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListTemplatesResponse:
         """
         Returns a list of notification templates
 
-        Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of templates
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of templates
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListTemplatesResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.templates.list(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "cursor": cursor,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
```

### Comparing `trycourier-6.0.2/src/courier/templates/types/__init__.py` & `trycourier-6.0.3/src/courier/templates/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/templates/types/list_templates_response.py` & `trycourier-6.0.3/src/courier/templates/types/list_templates_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/templates/types/notification_templates.py` & `trycourier-6.0.3/src/courier/templates/types/notification_templates.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/templates/types/routing_strategy.py` & `trycourier-6.0.3/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .channel_identifier import ChannelIdentifier
-from .routing_strategy_method import RoutingStrategyMethod
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
 
 
-class RoutingStrategy(pydantic_v1.BaseModel):
-    method: RoutingStrategyMethod = pydantic_v1.Field()
+class AddUserToSingleTenantsParamsProfile(pydantic_v1.BaseModel):
     """
-    The method for selecting channels to send the message with. Value can be either 'single' or 'all'. If not provided will default to 'single'
+    AddUserToSingleTenantsParamsProfile is no longer used for Add a User to a Single Tenant
     """
 
-    channels: typing.List[ChannelIdentifier] = pydantic_v1.Field()
+    title: str
+    email: str = pydantic_v1.Field()
     """
-    An array of valid channel identifiers (like email, push, sms, etc.) and additional routing nodes.
+    Email Address
+    """
+
+    phone_number: str = pydantic_v1.Field()
+    """
+    A valid phone number
+    """
+
+    locale: str = pydantic_v1.Field()
+    """
+    The user's preferred ISO 639-1 language code.
+    """
+
+    additional_fields: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    Additional provider specific fields may be specified.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.2/src/courier/templates/types/tag.py` & `trycourier-6.0.3/src/courier/templates/types/tag.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/templates/types/tag_data.py` & `trycourier-6.0.3/src/courier/templates/types/tag_data.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/tenants/client.py` & `trycourier-6.0.3/src/courier/users/tenants/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,90 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ..commons.errors.bad_request_error import BadRequestError
-from ..commons.types.bad_request import BadRequest
-from ..core.api_error import ApiError
-from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.remove_none_from_dict import remove_none_from_dict
-from ..core.request_options import RequestOptions
-from .types.default_preferences import DefaultPreferences
-from .types.list_users_for_tenant_response import ListUsersForTenantResponse
-from .types.template_property import TemplateProperty
-from .types.tenant import Tenant
-from .types.tenant_list_response import TenantListResponse
+from ...commons.types.user_tenant_association import UserTenantAssociation
+from ...core.api_error import ApiError
+from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
+from .types.list_tenants_for_user_response import ListTenantsForUserResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class TenantsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def create_or_replace(
+    def add_multple(
         self,
-        tenant_id: str,
+        user_id: str,
         *,
-        name: str,
-        parent_tenant_id: typing.Optional[str] = OMIT,
-        default_preferences: typing.Optional[DefaultPreferences] = OMIT,
-        properties: typing.Optional[typing.Sequence[TemplateProperty]] = OMIT,
-        user_profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        brand_id: typing.Optional[str] = OMIT,
+        tenants: typing.Sequence[UserTenantAssociation],
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Tenant:
+    ) -> None:
         """
-        Parameters:
-            - tenant_id: str. A unique identifier representing the tenant to be returned.
-
-            - name: str. Name of the tenant.
-
-            - parent_tenant_id: typing.Optional[str]. Tenant's parent id (if any).
-
-            - default_preferences: typing.Optional[DefaultPreferences]. Defines the preferences used for the tenant when the user hasn't specified their own.
-
-            - properties: typing.Optional[typing.Sequence[TemplateProperty]]. Arbitrary properties accessible to a template.
-
-            - user_profile: typing.Optional[typing.Dict[str, typing.Any]]. A user profile object merged with user profile on send.
-
-            - brand_id: typing.Optional[str]. Brand to be used for the account when one is not specified by the send call.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from courier import DefaultPreferences, SubscriptionTopic
+        This endpoint is used to add a user to
+        multiple tenants in one call.
+        A custom profile can also be supplied for each tenant.
+        This profile will be merged with the user's main
+        profile when sending to the user with that tenant.
+
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        tenants : typing.Sequence[UserTenantAssociation]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        from courier import UserTenantAssociation
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.tenants.create_or_replace(
-            tenant_id="string",
-            name="string",
-            parent_tenant_id="string",
-            default_preferences=DefaultPreferences(
-                items=[SubscriptionTopic()],
-            ),
-            properties=[{"key": "value"}],
-            user_profile={"string": {"key": "value"}},
-            brand_id="string",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if parent_tenant_id is not OMIT:
-            _request["parent_tenant_id"] = parent_tenant_id
-        if default_preferences is not OMIT:
-            _request["default_preferences"] = default_preferences
-        if properties is not OMIT:
-            _request["properties"] = properties
-        if user_profile is not OMIT:
-            _request["user_profile"] = user_profile
-        if brand_id is not OMIT:
-            _request["brand_id"] = brand_id
+        client.users.tenants.add_multple(
+            user_id="string",
+            tenants=[
+                UserTenantAssociation(
+                    user_id="string",
+                    type="user",
+                    tenant_id="string",
+                    profile={"string": {"key": "value"}},
+                )
+            ],
+        )
+        """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"tenants": tenants})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"tenants": tenants}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -108,45 +94,84 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tenant:
+    def add(
+        self,
+        user_id: str,
+        tenant_id: str,
+        *,
+        profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
         """
-        Parameters:
-            - tenant_id: str. A unique identifier representing the tenant to be returned.
+        This endpoint is used to add a single tenant.
+
+        A custom profile can also be supplied with the tenant.
+        This profile will be merged with the user's main profile
+        when sending to the user with that tenant.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to be added to the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be added to.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        profile : typing.Optional[typing.Dict[str, typing.Any]]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.tenants.get(
+        client.users.tenants.add(
+            user_id="string",
             tenant_id="string",
+            profile={"string": {"key": "value"}},
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if profile is not OMIT:
+            _request["profile"] = profile
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -154,63 +179,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(
-        self,
-        *,
-        limit: typing.Optional[int] = None,
-        cursor: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> TenantListResponse:
+    def remove_all(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Parameters:
-            - limit: typing.Optional[int]. The number of accousnts to return
-                                           (defaults to 20, maximum value of 100)
-            - cursor: typing.Optional[str]. Continue the pagination with the next cursor
+        Removes a user from any tenants they may have been associated with.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.tenants.list(
-            limit=1,
-            cursor="string",
+        client.users.tenants.remove_all(
+            user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tenants"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -219,40 +236,58 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(TenantListResponse, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def remove(self, user_id: str, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Parameters:
-            - tenant_id: str. Id of the tenant to be deleted.
+        Removes a user from the supplied tenant.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be removed from.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.tenants.delete(
+        client.users.tenants.remove(
+            user_id="string",
             tenant_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -270,47 +305,61 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_users_by_tenant(
+    def list(
         self,
-        tenant_id: str,
+        user_id: str,
         *,
         limit: typing.Optional[int] = None,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListUsersForTenantResponse:
+    ) -> ListTenantsForUserResponse:
         """
-        Parameters:
-            - tenant_id: str. Id of the tenant for user membership.
+        Returns a paginated list of user tenant associations.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to retrieve all associated tenants for.
 
-            - limit: typing.Optional[int]. The number of accounts to return
-                                           (defaults to 20, maximum value of 100)
-            - cursor: typing.Optional[str]. Continue the pagination with the next cursor
+        limit : typing.Optional[int]
+            The number of accounts to return
+            (defaults to 20, maximum value of 100)
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListTenantsForUserResponse
+
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.tenants.get_users_by_tenant(
-            tenant_id="string",
+        client.users.tenants.list(
+            user_id="string",
             limit=1,
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}/users"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "limit": limit,
                         "cursor": cursor,
                         **(
@@ -332,97 +381,86 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(ListTenantsForUserResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTenantsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def create_or_replace(
+    async def add_multple(
         self,
-        tenant_id: str,
+        user_id: str,
         *,
-        name: str,
-        parent_tenant_id: typing.Optional[str] = OMIT,
-        default_preferences: typing.Optional[DefaultPreferences] = OMIT,
-        properties: typing.Optional[typing.Sequence[TemplateProperty]] = OMIT,
-        user_profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        brand_id: typing.Optional[str] = OMIT,
+        tenants: typing.Sequence[UserTenantAssociation],
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Tenant:
+    ) -> None:
         """
-        Parameters:
-            - tenant_id: str. A unique identifier representing the tenant to be returned.
-
-            - name: str. Name of the tenant.
-
-            - parent_tenant_id: typing.Optional[str]. Tenant's parent id (if any).
-
-            - default_preferences: typing.Optional[DefaultPreferences]. Defines the preferences used for the tenant when the user hasn't specified their own.
-
-            - properties: typing.Optional[typing.Sequence[TemplateProperty]]. Arbitrary properties accessible to a template.
-
-            - user_profile: typing.Optional[typing.Dict[str, typing.Any]]. A user profile object merged with user profile on send.
-
-            - brand_id: typing.Optional[str]. Brand to be used for the account when one is not specified by the send call.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from courier import DefaultPreferences, SubscriptionTopic
+        This endpoint is used to add a user to
+        multiple tenants in one call.
+        A custom profile can also be supplied for each tenant.
+        This profile will be merged with the user's main
+        profile when sending to the user with that tenant.
+
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        tenants : typing.Sequence[UserTenantAssociation]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        from courier import UserTenantAssociation
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.tenants.create_or_replace(
-            tenant_id="string",
-            name="string",
-            parent_tenant_id="string",
-            default_preferences=DefaultPreferences(
-                items=[SubscriptionTopic()],
-            ),
-            properties=[{"key": "value"}],
-            user_profile={"string": {"key": "value"}},
-            brand_id="string",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if parent_tenant_id is not OMIT:
-            _request["parent_tenant_id"] = parent_tenant_id
-        if default_preferences is not OMIT:
-            _request["default_preferences"] = default_preferences
-        if properties is not OMIT:
-            _request["properties"] = properties
-        if user_profile is not OMIT:
-            _request["user_profile"] = user_profile
-        if brand_id is not OMIT:
-            _request["brand_id"] = brand_id
+        await client.users.tenants.add_multple(
+            user_id="string",
+            tenants=[
+                UserTenantAssociation(
+                    user_id="string",
+                    type="user",
+                    tenant_id="string",
+                    profile={"string": {"key": "value"}},
+                )
+            ],
+        )
+        """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"tenants": tenants})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"tenants": tenants}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -432,45 +470,84 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tenant:
+    async def add(
+        self,
+        user_id: str,
+        tenant_id: str,
+        *,
+        profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
         """
-        Parameters:
-            - tenant_id: str. A unique identifier representing the tenant to be returned.
+        This endpoint is used to add a single tenant.
+
+        A custom profile can also be supplied with the tenant.
+        This profile will be merged with the user's main profile
+        when sending to the user with that tenant.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to be added to the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be added to.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        profile : typing.Optional[typing.Dict[str, typing.Any]]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.tenants.get(
+        await client.users.tenants.add(
+            user_id="string",
             tenant_id="string",
+            profile={"string": {"key": "value"}},
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if profile is not OMIT:
+            _request["profile"] = profile
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"),
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -478,63 +555,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(
-        self,
-        *,
-        limit: typing.Optional[int] = None,
-        cursor: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> TenantListResponse:
+    async def remove_all(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Parameters:
-            - limit: typing.Optional[int]. The number of accousnts to return
-                                           (defaults to 20, maximum value of 100)
-            - cursor: typing.Optional[str]. Continue the pagination with the next cursor
+        Removes a user from any tenants they may have been associated with.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.tenants.list(
-            limit=1,
-            cursor="string",
+        await client.users.tenants.remove_all(
+            user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tenants"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -543,40 +612,60 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(TenantListResponse, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    async def remove(
+        self, user_id: str, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> None:
         """
-        Parameters:
-            - tenant_id: str. Id of the tenant to be deleted.
+        Removes a user from the supplied tenant.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be removed from.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.tenants.delete(
+        await client.users.tenants.remove(
+            user_id="string",
             tenant_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -594,47 +683,61 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_users_by_tenant(
+    async def list(
         self,
-        tenant_id: str,
+        user_id: str,
         *,
         limit: typing.Optional[int] = None,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListUsersForTenantResponse:
+    ) -> ListTenantsForUserResponse:
         """
-        Parameters:
-            - tenant_id: str. Id of the tenant for user membership.
+        Returns a paginated list of user tenant associations.
+
+        Parameters
+        ----------
+        user_id : str
+            Id of the user to retrieve all associated tenants for.
 
-            - limit: typing.Optional[int]. The number of accounts to return
-                                           (defaults to 20, maximum value of 100)
-            - cursor: typing.Optional[str]. Continue the pagination with the next cursor
+        limit : typing.Optional[int]
+            The number of accounts to return
+            (defaults to 20, maximum value of 100)
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListTenantsForUserResponse
+
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.tenants.get_users_by_tenant(
-            tenant_id="string",
+        await client.users.tenants.list(
+            user_id="string",
             limit=1,
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}/users"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "limit": limit,
                         "cursor": cursor,
                         **(
@@ -656,15 +759,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(ListTenantsForUserResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.2/src/courier/tenants/types/__init__.py` & `trycourier-6.0.3/src/courier/tenants/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/tenants/types/default_preferences.py` & `trycourier-6.0.3/src/courier/users/tokens/types/get_user_tokens_opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .subscription_topic import SubscriptionTopic
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
 
 
-class DefaultPreferences(pydantic_v1.BaseModel):
-    items: typing.List[SubscriptionTopic]
+class GetUserTokensOpts(pydantic_v1.BaseModel):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.2/src/courier/tenants/types/list_users_for_tenant_response.py` & `trycourier-6.0.3/src/courier/tenants/types/list_users_for_tenant_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/tenants/types/subscription_topic.py` & `trycourier-6.0.3/src/courier/tenants/types/subscription_topic.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/tenants/types/tenant.py` & `trycourier-6.0.3/src/courier/tenants/types/tenant.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/tenants/types/tenant_list_response.py` & `trycourier-6.0.3/src/courier/tenants/types/tenant_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/translations/client.py` & `trycourier-6.0.3/src/courier/translations/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,34 +21,45 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(self, domain: str, locale: str, *, request_options: typing.Optional[RequestOptions] = None) -> str:
         """
         Get translations by locale
 
-        Parameters:
-            - domain: str. The domain you want to retrieve translations for. Only `default` is supported at the moment
+        Parameters
+        ----------
+        domain : str
+            The domain you want to retrieve translations for. Only `default` is supported at the moment
+
+        locale : str
+            The locale you want to retrieve the translations for
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        str
+            .po file translation content
 
-            - locale: str. The locale you want to retrieve the translations for
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.translations.get(
             domain="string",
             locale="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -77,37 +88,47 @@
 
     def update(
         self, domain: str, locale: str, *, request: str, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Update a translation
 
-        Parameters:
-            - domain: str. The domain you want to retrieve translations for. Only `default` is supported at the moment
+        Parameters
+        ----------
+        domain : str
+            The domain you want to retrieve translations for. Only `default` is supported at the moment
+
+        locale : str
+            The locale you want to retrieve the translations for
+
+        request : str
 
-            - locale: str. The locale you want to retrieve the translations for
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request: str.
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.translations.update(
             domain="string",
             locale="string",
             request="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request),
@@ -140,34 +161,45 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get(self, domain: str, locale: str, *, request_options: typing.Optional[RequestOptions] = None) -> str:
         """
         Get translations by locale
 
-        Parameters:
-            - domain: str. The domain you want to retrieve translations for. Only `default` is supported at the moment
+        Parameters
+        ----------
+        domain : str
+            The domain you want to retrieve translations for. Only `default` is supported at the moment
+
+        locale : str
+            The locale you want to retrieve the translations for
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        str
+            .po file translation content
 
-            - locale: str. The locale you want to retrieve the translations for
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.translations.get(
             domain="string",
             locale="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -196,37 +228,47 @@
 
     async def update(
         self, domain: str, locale: str, *, request: str, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Update a translation
 
-        Parameters:
-            - domain: str. The domain you want to retrieve translations for. Only `default` is supported at the moment
+        Parameters
+        ----------
+        domain : str
+            The domain you want to retrieve translations for. Only `default` is supported at the moment
+
+        locale : str
+            The locale you want to retrieve the translations for
+
+        request : str
 
-            - locale: str. The locale you want to retrieve the translations for
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request: str.
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.translations.update(
             domain="string",
             locale="string",
             request="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request),
```

### Comparing `trycourier-6.0.2/src/courier/types/send_message_response.py` & `trycourier-6.0.3/src/courier/types/send_message_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/__init__.py` & `trycourier-6.0.3/src/courier/users/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/client.py` & `trycourier-6.0.3/src/courier/users/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/preferences/client.py` & `trycourier-6.0.3/src/courier/users/preferences/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,31 +29,40 @@
 
     def list(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserPreferencesListResponse:
         """
         Fetch all user preferences.
 
-        Parameters:
-            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier associated with the user whose preferences you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        UserPreferencesListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.preferences.list(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/preferences"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -81,34 +90,44 @@
 
     def get(
         self, user_id: str, topic_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserPreferencesGetResponse:
         """
         Fetch user preferences for a specific subscription topic.
 
-        Parameters:
-            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier associated with the user whose preferences you wish to retrieve.
+
+        topic_id : str
+            A unique identifier associated with a subscription topic.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        UserPreferencesGetResponse
 
-            - topic_id: str. A unique identifier associated with a subscription topic.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.preferences.get(
             user_id="string",
             topic_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -142,23 +161,33 @@
         *,
         topic: TopicPreferenceUpdate,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UserPreferencesUpdateResponse:
         """
         Update or Create user preferences for a specific subscription topic.
 
-        Parameters:
-            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier associated with the user whose preferences you wish to retrieve.
+
+        topic_id : str
+            A unique identifier associated with a subscription topic.
+
+        topic : TopicPreferenceUpdate
 
-            - topic_id: str. A unique identifier associated with a subscription topic.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - topic: TopicPreferenceUpdate.
+        Returns
+        -------
+        UserPreferencesUpdateResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
         from courier.users import TopicPreferenceUpdate
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.preferences.update(
@@ -168,16 +197,16 @@
                 status="OPTED_IN",
                 has_custom_routing=True,
                 custom_routing=["inbox", "email"],
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"topic": topic})
@@ -217,31 +246,40 @@
 
     async def list(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserPreferencesListResponse:
         """
         Fetch all user preferences.
 
-        Parameters:
-            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier associated with the user whose preferences you wish to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        UserPreferencesListResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.preferences.list(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/preferences"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -269,34 +307,44 @@
 
     async def get(
         self, user_id: str, topic_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserPreferencesGetResponse:
         """
         Fetch user preferences for a specific subscription topic.
 
-        Parameters:
-            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier associated with the user whose preferences you wish to retrieve.
+
+        topic_id : str
+            A unique identifier associated with a subscription topic.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        UserPreferencesGetResponse
 
-            - topic_id: str. A unique identifier associated with a subscription topic.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.preferences.get(
             user_id="string",
             topic_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -330,23 +378,33 @@
         *,
         topic: TopicPreferenceUpdate,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UserPreferencesUpdateResponse:
         """
         Update or Create user preferences for a specific subscription topic.
 
-        Parameters:
-            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+        Parameters
+        ----------
+        user_id : str
+            A unique identifier associated with the user whose preferences you wish to retrieve.
+
+        topic_id : str
+            A unique identifier associated with a subscription topic.
+
+        topic : TopicPreferenceUpdate
 
-            - topic_id: str. A unique identifier associated with a subscription topic.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - topic: TopicPreferenceUpdate.
+        Returns
+        -------
+        UserPreferencesUpdateResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
         from courier.users import TopicPreferenceUpdate
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.preferences.update(
@@ -356,16 +414,16 @@
                 status="OPTED_IN",
                 has_custom_routing=True,
                 custom_routing=["inbox", "email"],
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"topic": topic})
```

### Comparing `trycourier-6.0.2/src/courier/users/preferences/types/__init__.py` & `trycourier-6.0.3/src/courier/users/preferences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/preferences/types/topic_preference.py` & `trycourier-6.0.3/src/courier/users/preferences/types/topic_preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/preferences/types/topic_preference_update.py` & `trycourier-6.0.3/src/courier/users/preferences/types/topic_preference_update.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/preferences/types/user_preferences_get_response.py` & `trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/preferences/types/user_preferences_list_response.py` & `trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/preferences/types/user_preferences_update_response.py` & `trycourier-6.0.3/src/courier/users/preferences/types/user_preferences_update_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py` & `trycourier-6.0.3/src/courier/users/tokens/types/patch_operation.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,34 +3,28 @@
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
 
 
-class AddUserToSingleTenantsParamsProfile(pydantic_v1.BaseModel):
-    title: str
-    email: str = pydantic_v1.Field()
+class PatchOperation(pydantic_v1.BaseModel):
+    op: str = pydantic_v1.Field()
     """
-    Email Address
+    The operation to perform.
     """
 
-    phone_number: str = pydantic_v1.Field()
+    path: str = pydantic_v1.Field()
     """
-    A valid phone number
+    The JSON path specifying the part of the profile to operate on.
     """
 
-    locale: str = pydantic_v1.Field()
+    value: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The user's preferred ISO 639-1 language code.
-    """
-
-    additional_fields: typing.Dict[str, typing.Any] = pydantic_v1.Field()
-    """
-    Additional provider specific fields may be specified.
+    The value for the operation.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.2/src/courier/users/tenants/types/list_tenants_for_user_response.py` & `trycourier-6.0.3/src/courier/users/tenants/types/list_tenants_for_user_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/__init__.py` & `trycourier-6.0.3/src/courier/users/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/client.py` & `trycourier-6.0.3/src/courier/users/tokens/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,31 +25,40 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def add_multiple(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Adds multiple tokens to a user and overwrites matching existing tokens.
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.tokens.add_multiple(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -80,23 +89,33 @@
 
     def add(
         self, user_id: str, token: str, *, request: UserToken, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Adds a single token to a user and overwrites a matching existing token.
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
 
-            - token: str. The full token string.
+        token : str
+            The full token string.
 
-            - request: UserToken.
+        request : UserToken
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import Courier
         from courier.users import Device, Tracking, UserToken
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.tokens.add(
@@ -121,16 +140,16 @@
                     lat="string",
                     long_="string",
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
@@ -170,23 +189,33 @@
         *,
         request: PatchUserTokenOpts,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Apply a JSON Patch (RFC 6902) to the specified token.
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        token : str
+            The full token string.
 
-            - token: str. The full token string.
+        request : PatchUserTokenOpts
 
-            - request: PatchUserTokenOpts.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import Courier
         from courier.users import PatchOperation, PatchUserTokenOpts
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.tokens.update(
@@ -194,16 +223,16 @@
             token="string",
             request=PatchUserTokenOpts(
                 patch=[PatchOperation()],
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
@@ -238,34 +267,44 @@
 
     def get(
         self, user_id: str, token: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetUserTokenResponse:
         """
         Get single token available for a `:token`
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
-
-            - token: str. The full token string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        token : str
+            The full token string.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetUserTokenResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.tokens.get(
             user_id="string",
             token="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -292,31 +331,40 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetAllTokensResponse:
         """
         Gets all tokens available for a :user_id
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetAllTokensResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.users.tokens.list(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -347,31 +395,40 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def add_multiple(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Adds multiple tokens to a user and overwrites matching existing tokens.
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.tokens.add_multiple(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -402,23 +459,33 @@
 
     async def add(
         self, user_id: str, token: str, *, request: UserToken, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Adds a single token to a user and overwrites a matching existing token.
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
 
-            - token: str. The full token string.
+        token : str
+            The full token string.
 
-            - request: UserToken.
+        request : UserToken
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import AsyncCourier
         from courier.users import Device, Tracking, UserToken
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.tokens.add(
@@ -443,16 +510,16 @@
                     lat="string",
                     long_="string",
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(
+            method="PUT",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
@@ -492,23 +559,33 @@
         *,
         request: PatchUserTokenOpts,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Apply a JSON Patch (RFC 6902) to the specified token.
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        token : str
+            The full token string.
 
-            - token: str. The full token string.
+        request : PatchUserTokenOpts
 
-            - request: PatchUserTokenOpts.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        None
+
+        Examples
+        --------
         from courier.client import AsyncCourier
         from courier.users import PatchOperation, PatchUserTokenOpts
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.tokens.update(
@@ -516,16 +593,16 @@
             token="string",
             request=PatchUserTokenOpts(
                 patch=[PatchOperation()],
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
@@ -560,34 +637,44 @@
 
     async def get(
         self, user_id: str, token: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetUserTokenResponse:
         """
         Get single token available for a `:token`
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
-
-            - token: str. The full token string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        token : str
+            The full token string.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetUserTokenResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.tokens.get(
             user_id="string",
             token="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
@@ -616,31 +703,40 @@
 
     async def list(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetAllTokensResponse:
         """
         Gets all tokens available for a :user_id
 
-        Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+        Parameters
+        ----------
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetAllTokensResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.users.tokens.list(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
```

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/__init__.py` & `trycourier-6.0.3/src/courier/users/tokens/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/delete_user_token_opts.py` & `trycourier-6.0.3/src/courier/users/tokens/types/delete_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/device.py` & `trycourier-6.0.3/src/courier/users/tokens/types/device.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/get_user_token_opts.py` & `trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/get_user_token_response.py` & `trycourier-6.0.3/src/courier/users/tokens/types/get_user_token_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/get_user_tokens_opts.py` & `trycourier-6.0.3/src/courier/users/tokens/types/put_user_tokens_opts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from .user_token import UserToken
 
 
-class GetUserTokensOpts(pydantic_v1.BaseModel):
+class PutUserTokensOpts(pydantic_v1.BaseModel):
     user_id: str
+    tokens: typing.List[UserToken]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/patch_operation.py` & `trycourier-6.0.3/src/courier/commons/types/user_tenant_association.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class PatchOperation(pydantic_v1.BaseModel):
-    op: str = pydantic_v1.Field()
+class UserTenantAssociation(pydantic_v1.BaseModel):
+    user_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The operation to perform.
+    User ID for the assocation between tenant and user
     """
 
-    path: str = pydantic_v1.Field()
+    type: typing.Optional[typing.Literal["user"]] = None
+    tenant_id: str = pydantic_v1.Field()
     """
-    The JSON path specifying the part of the profile to operate on.
+    Tenant ID for the assocation between tenant and user
     """
 
-    value: typing.Optional[str] = pydantic_v1.Field(default=None)
+    profile: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
-    The value for the operation.
+    Additional metadata to be applied to a user profile when used in a tenant context
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/patch_user_token_opts.py` & `trycourier-6.0.3/src/courier/users/tokens/types/patch_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/put_user_token_opts.py` & `trycourier-6.0.3/src/courier/users/tokens/types/put_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/put_user_tokens_opts.py` & `trycourier-6.0.3/src/courier/tenants/types/default_preferences.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .user_token import UserToken
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .subscription_topic import SubscriptionTopic
 
 
-class PutUserTokensOpts(pydantic_v1.BaseModel):
-    user_id: str
-    tokens: typing.List[UserToken]
+class DefaultPreferences(pydantic_v1.BaseModel):
+    items: typing.Optional[typing.List[SubscriptionTopic]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/tracking.py` & `trycourier-6.0.3/src/courier/users/tokens/types/tracking.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/src/courier/users/tokens/types/user_token.py` & `trycourier-6.0.3/src/courier/users/tokens/types/user_token.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.2/PKG-INFO` & `trycourier-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 6.0.2
+Version: 6.0.3
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

