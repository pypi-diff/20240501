# Comparing `tmp/one_interfaces-6.8.0.tar.gz` & `tmp/one_interfaces-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\one_interfaces-6.8.0.tar", last modified: Thu Apr 11 15:54:23 2024, max compression
+gzip compressed data, was "dist\one_interfaces-6.9.0.tar", last modified: Wed May  1 18:11:20 2024, max compression
```

## Comparing `one_interfaces-6.8.0.tar` & `one_interfaces-6.9.0.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 15:54:23.220019 one_interfaces-6.8.0/
--rw-rw-rw-   0        0        0      580 2022-07-05 14:29:22.000000 one_interfaces-6.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0       62 2022-07-05 14:29:22.000000 one_interfaces-6.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1217 2024-04-11 15:54:23.221019 one_interfaces-6.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      394 2022-11-11 17:33:49.000000 one_interfaces-6.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 15:54:23.212019 one_interfaces-6.8.0/one_interfaces/
--rw-rw-rw-   0        0        0       23 2024-04-11 15:51:44.000000 one_interfaces-6.8.0/one_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/account_status_pb2.py
--rw-rw-rw-   0        0        0     2440 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/activity_pb2.py
--rw-rw-rw-   0        0        0     1899 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/activity_type_pb2.py
--rw-rw-rw-   0        0        0     2231 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/address_pb2.py
--rw-rw-rw-   0        0        0     1681 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/agency_pb2.py
--rw-rw-rw-   0        0        0     1874 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_pb2.py
--rw-rw-rw-   0        0        0     2811 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_result_pb2.py
--rw-rw-rw-   0        0        0     1769 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_results_import_profile_pb2.py
--rw-rw-rw-   0        0        0     1758 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/analyte_results_import_telemetry_pb2.py
--rw-rw-rw-   0        0        0     1223 2024-04-11 15:53:20.000000 one_interfaces-6.8.0/one_interfaces/apierror_pb2.py
--rw-rw-rw-   0        0        0     1393 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/apiresponse_pb2.py
--rw-rw-rw-   0        0        0     1941 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/auditevent_pb2.py
--rw-rw-rw-   0        0        0     1474 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cell_monitor_backup_pb2.py
--rw-rw-rw-   0        0        0     1519 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cell_pb2.py
--rw-rw-rw-   0        0        0     1541 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/celldata_binding_pb2.py
--rw-rw-rw-   0        0        0     1988 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/celldata_pb2.py
--rw-rw-rw-   0        0        0     1534 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cells_pb2.py
--rw-rw-rw-   0        0        0     1871 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/cellvalue_backup_pb2.py
--rw-rw-rw-   0        0        0     4778 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/client_pb2.py
--rw-rw-rw-   0        0        0     2054 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/coagmeasurement_pb2.py
--rw-rw-rw-   0        0        0     2429 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/column_pb2.py
--rw-rw-rw-   0        0        0     2097 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/computation_binding_pb2.py
--rw-rw-rw-   0        0        0     2564 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/computation_pb2.py
--rw-rw-rw-   0        0        0     1893 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/computation_variable_binding_pb2.py
--rw-rw-rw-   0        0        0     2027 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/configuration_note_pb2.py
--rw-rw-rw-   0        0        0     2970 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/configuration_pb2.py
--rw-rw-rw-   0        0        0     1499 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/configuration_tag_pb2.py
--rw-rw-rw-   0        0        0    13410 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/content_pb2.py
--rw-rw-rw-   0        0        0     1951 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/csv_configuration_file_pb2.py
--rw-rw-rw-   0        0        0     1743 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/data_source_binding_pb2.py
--rw-rw-rw-   0        0        0     2052 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/data_source_configuration_pb2.py
--rw-rw-rw-   0        0        0     1536 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py
--rw-rw-rw-   0        0        0     2041 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py
--rw-rw-rw-   0        0        0     1523 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py
--rw-rw-rw-   0        0        0     3269 2024-04-11 15:53:21.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_pb2.py
--rw-rw-rw-   0        0        0     2247 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_pb2.py
--rw-rw-rw-   0        0        0     3800 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py
--rw-rw-rw-   0        0        0     2063 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_type_pb2.py
--rw-rw-rw-   0        0        0     2020 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/digital_twin_user_right_pb2.py
--rw-rw-rw-   0        0        0     1342 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/display_options_pb2.py
--rw-rw-rw-   0        0        0     1820 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_source_definition_pb2.py
--rw-rw-rw-   0        0        0     1669 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_definition_pb2.py
--rw-rw-rw-   0        0        0     1376 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_field_pb2.py
--rw-rw-rw-   0        0        0     1605 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py
--rw-rw-rw-   0        0        0     1508 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_pb2.py
--rw-rw-rw-   0        0        0     2309 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enterprise_dataset_definition_pb2.py
--rw-rw-rw-   0        0        0     1303 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_aggregate_pb2.py
--rw-rw-rw-   0        0        0     1408 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_auditevent_pb2.py
--rw-rw-rw-   0        0        0     1385 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_azure_notification_hubtype_pb2.py
--rw-rw-rw-   0        0        0     1642 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_cell_range_action_pb2.py
--rw-rw-rw-   0        0        0     1782 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_datasource_pb2.py
--rw-rw-rw-   0        0        0     1392 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_day_pb2.py
--rw-rw-rw-   0        0        0     1515 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py
--rw-rw-rw-   0        0        0     1381 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_digital_twin_restriction_pb2.py
--rw-rw-rw-   0        0        0     1422 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_digital_twin_user_right_pb2.py
--rw-rw-rw-   0        0        0     1339 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_domain_source_pb2.py
--rw-rw-rw-   0        0        0     1373 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_entity_pb2.py
--rw-rw-rw-   0        0        0     1433 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_identity_provider_pb2.py
--rw-rw-rw-   0        0        0     1552 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_import_status_pb2.py
--rw-rw-rw-   0        0        0     1416 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_limit_operation_pb2.py
--rw-rw-rw-   0        0        0     1437 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_limit_pb2.py
--rw-rw-rw-   0        0        0     1545 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_month_pb2.py
--rw-rw-rw-   0        0        0     1606 2024-04-11 15:53:22.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_category_pb2.py
--rw-rw-rw-   0        0        0     1557 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_delivery_method_pb2.py
--rw-rw-rw-   0        0        0     1427 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_message_type_pb2.py
--rw-rw-rw-   0        0        0     1346 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_notification_platform_pb2.py
--rw-rw-rw-   0        0        0     1452 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_one_log_level_pb2.py
--rw-rw-rw-   0        0        0     1374 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_output_placement_pb2.py
--rw-rw-rw-   0        0        0     1269 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_rendering_engine_pb2.py
--rw-rw-rw-   0        0        0     1681 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py
--rw-rw-rw-   0        0        0     1663 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_pb2.py
--rw-rw-rw-   0        0        0     3080 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_sampling_statistic_pb2.py
--rw-rw-rw-   0        0        0     1483 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_time_context_pb2.py
--rw-rw-rw-   0        0        0     1388 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_time_unit_pb2.py
--rw-rw-rw-   0        0        0    27482 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_timezone_pb2.py
--rw-rw-rw-   0        0        0     1415 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_valid_value_restriction_pb2.py
--rw-rw-rw-   0        0        0     1376 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_variable_type_pb2.py
--rw-rw-rw-   0        0        0     2357 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_wims_week_definition_pb2.py
--rw-rw-rw-   0        0        0     1341 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/enum_worksheet_pb2.py
--rw-rw-rw-   0        0        0     1768 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/execution_details_pb2.py
--rw-rw-rw-   0        0        0     2010 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/execution_parameter_pb2.py
--rw-rw-rw-   0        0        0     1211 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/expression_line_pb2.py
--rw-rw-rw-   0        0        0     2205 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/feature_pb2.py
--rw-rw-rw-   0        0        0     1589 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/feature_state_type_pb2.py
--rw-rw-rw-   0        0        0     1793 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/file_configuration_pb2.py
--rw-rw-rw-   0        0        0     1563 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/gauge_data_point_pb2.py
--rw-rw-rw-   0        0        0     1560 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/gis_pb2.py
--rw-rw-rw-   0        0        0     1231 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/historian_binding_pb2.py
--rw-rw-rw-   0        0        0     1981 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/historian_data_pb2.py
--rw-rw-rw-   0        0        0     1536 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/i18nkey_text_reference_pb2.py
--rw-rw-rw-   0        0        0     1855 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/ingest_client_pb2.py
--rw-rw-rw-   0        0        0     1698 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/jsonTicksDateTime_pb2.py
--rw-rw-rw-   0        0        0     1325 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/key_value_pb2.py
--rw-rw-rw-   0        0        0     1668 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/limit_configuration_pb2.py
--rw-rw-rw-   0        0        0     2385 2024-04-11 15:53:23.000000 one_interfaces-6.8.0/one_interfaces/limit_pb2.py
--rw-rw-rw-   0        0        0     1948 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/measurement_pb2.py
--rw-rw-rw-   0        0        0     1768 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/model_execution_pb2.py
--rw-rw-rw-   0        0        0     1424 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/model_location_pb2.py
--rw-rw-rw-   0        0        0     2433 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/model_template_pb2.py
--rw-rw-rw-   0        0        0     1233 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/multi_point2d_pb2.py
--rw-rw-rw-   0        0        0     1233 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/multi_point3d_pb2.py
--rw-rw-rw-   0        0        0     1472 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/note_pb2.py
--rw-rw-rw-   0        0        0     1695 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_broadcast_pb2.py
--rw-rw-rw-   0        0        0     1448 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_contact_pb2.py
--rw-rw-rw-   0        0        0     1859 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_device_pb2.py
--rw-rw-rw-   0        0        0     2430 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_direct_preference_pb2.py
--rw-rw-rw-   0        0        0     2254 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_event_pb2.py
--rw-rw-rw-   0        0        0     2267 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_in_app_notification_message_pb2.py
--rw-rw-rw-   0        0        0     1743 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_preference_pb2.py
--rw-rw-rw-   0        0        0     2174 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_template_pb2.py
--rw-rw-rw-   0        0        0     2201 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_topic_pb2.py
--rw-rw-rw-   0        0        0     1828 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_topic_variable_pb2.py
--rw-rw-rw-   0        0        0     2450 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/notification_user_preference_pb2.py
--rw-rw-rw-   0        0        0     2455 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/operation_export_pb2.py
--rw-rw-rw-   0        0        0     2111 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/outputcell_backup_pb2.py
--rw-rw-rw-   0        0        0     1552 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/pagination_pb2.py
--rw-rw-rw-   0        0        0     2177 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_agency_code_pb2.py
--rw-rw-rw-   0        0        0     1674 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_agency_code_type_pb2.py
--rw-rw-rw-   0        0        0     1819 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_definition_pb2.py
--rw-rw-rw-   0        0        0     2356 2024-04-11 15:53:24.000000 one_interfaces-6.8.0/one_interfaces/parameter_pb2.py
--rw-rw-rw-   0        0        0     2569 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/plant_status_pb2.py
--rw-rw-rw-   0        0        0     1158 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/point2d_pb2.py
--rw-rw-rw-   0        0        0     1186 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/point3d_pb2.py
--rw-rw-rw-   0        0        0     1637 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/post_filtering_column_definition_pb2.py
--rw-rw-rw-   0        0        0     1878 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/post_filtering_pb2.py
--rw-rw-rw-   0        0        0     1585 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/privileges_pb2.py
--rw-rw-rw-   0        0        0     2503 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/product_offering_pb2.py
--rw-rw-rw-   0        0        0     2064 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/quantity_type_pb2.py
--rw-rw-rw-   0        0        0     1448 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/record_auditinfo_pb2.py
--rw-rw-rw-   0        0        0     2076 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_json_v2_pb2.py
--rw-rw-rw-   0        0        0     2780 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_pb2.py
--rw-rw-rw-   0        0        0     2178 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_runs_pb2.py
--rw-rw-rw-   0        0        0     1842 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_definition_tags_pb2.py
--rw-rw-rw-   0        0        0     1677 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_parameter_pb2.py
--rw-rw-rw-   0        0        0     2382 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/report_run_pb2.py
--rw-rw-rw-   0        0        0     1971 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/reportable_qualifier_definition_pb2.py
--rw-rw-rw-   0        0        0     1417 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/reportable_qualifier_pb2.py
--rw-rw-rw-   0        0        0     1252 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/rights_pb2.py
--rw-rw-rw-   0        0        0     2008 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/role_pb2.py
--rw-rw-rw-   0        0        0     1972 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/row_index_pb2.py
--rw-rw-rw-   0        0        0     1346 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/row_merge_result_pb2.py
--rw-rw-rw-   0        0        0     1692 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/row_pb2.py
--rw-rw-rw-   0        0        0     1403 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_occurrence_pb2.py
--rw-rw-rw-   0        0        0     2186 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_pb2.py
--rw-rw-rw-   0        0        0     1472 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_recurrence_pattern_pb2.py
--rw-rw-rw-   0        0        0     1887 2024-04-11 15:53:25.000000 one_interfaces-6.8.0/one_interfaces/schedule_type_pb2.py
--rw-rw-rw-   0        0        0     2533 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/scope_pb2.py
--rw-rw-rw-   0        0        0     1931 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/search_option_pb2.py
--rw-rw-rw-   0        0        0     2186 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/series_pb2.py
--rw-rw-rw-   0        0        0     2279 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/service_tech_tenant_request_pb2.py
--rw-rw-rw-   0        0        0     1649 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_connection_info_pb2.py
--rw-rw-rw-   0        0        0     1261 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py
--rw-rw-rw-   0        0        0     1567 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_payload_pb2.py
--rw-rw-rw-   0        0        0     1598 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_pb2.py
--rw-rw-rw-   0        0        0     1624 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/signalr_one_hub_message_pb2.py
--rw-rw-rw-   0        0        0     1197 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_binding_pb2.py
--rw-rw-rw-   0        0        0     1699 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_computation_pb2.py
--rw-rw-rw-   0        0        0     1753 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_definition_pb2.py
--rw-rw-rw-   0        0        0     1500 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/spreadsheet_pb2.py
--rw-rw-rw-   0        0        0     1820 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/template_parameter_pb2.py
--rw-rw-rw-   0        0        0     2465 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/tenant_pb2.py
--rw-rw-rw-   0        0        0     1680 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/tenant_product_offering_pb2.py
--rw-rw-rw-   0        0        0     2113 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/test_analyte_group_pb2.py
--rw-rw-rw-   0        0        0     1415 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/time_context_pb2.py
--rw-rw-rw-   0        0        0     2106 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/timeseriesdata_pb2.py
--rw-rw-rw-   0        0        0     1372 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/timewindow_pb2.py
--rw-rw-rw-   0        0        0     1499 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/timezones_pb2.py
--rw-rw-rw-   0        0        0     1835 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/unit_agency_code_pb2.py
--rw-rw-rw-   0        0        0     1627 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/unit_agency_code_type_pb2.py
--rw-rw-rw-   0        0        0     1701 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/unit_pb2.py
--rw-rw-rw-   0        0        0     1308 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/user_password_management_pb2.py
--rw-rw-rw-   0        0        0     4289 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/user_pb2.py
--rw-rw-rw-   0        0        0     1812 2024-04-11 15:53:26.000000 one_interfaces-6.8.0/one_interfaces/user_preference_pb2.py
--rw-rw-rw-   0        0        0     1969 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/user_profile_pb2.py
--rw-rw-rw-   0        0        0     1784 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/valid_value_pb2.py
--rw-rw-rw-   0        0        0     1966 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/variable_pb2.py
--rw-rw-rw-   0        0        0     1799 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/worksheet_definition_pb2.py
--rw-rw-rw-   0        0        0     1511 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/worksheet_pb2.py
--rw-rw-rw-   0        0        0     1789 2024-04-11 15:53:27.000000 one_interfaces-6.8.0/one_interfaces/worksheet_view_pb2.py
-drwxrwxrwx   0        0        0        0 2024-04-11 15:54:23.219348 one_interfaces-6.8.0/one_interfaces.egg-info/
--rw-rw-rw-   0        0        0     1217 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7545 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 15:54:22.000000 one_interfaces-6.8.0/one_interfaces.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        4 2022-07-05 14:29:22.000000 one_interfaces-6.8.0/requirements.txt
--rw-rw-rw-   0        0        0      159 2024-04-11 15:54:23.222019 one_interfaces-6.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1714 2022-11-11 17:30:03.000000 one_interfaces-6.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:11:20.440651 one_interfaces-6.9.0/
+-rw-rw-rw-   0        0        0      580 2022-07-05 14:29:22.000000 one_interfaces-6.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       62 2022-07-05 14:29:22.000000 one_interfaces-6.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1217 2024-05-01 18:11:20.441653 one_interfaces-6.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2022-11-11 17:33:49.000000 one_interfaces-6.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 18:11:20.430651 one_interfaces-6.9.0/one_interfaces/
+-rw-rw-rw-   0        0        0       23 2024-05-01 18:06:59.000000 one_interfaces-6.9.0/one_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/account_status_pb2.py
+-rw-rw-rw-   0        0        0     2440 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/activity_pb2.py
+-rw-rw-rw-   0        0        0     1899 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/activity_type_pb2.py
+-rw-rw-rw-   0        0        0     2231 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/address_pb2.py
+-rw-rw-rw-   0        0        0     1681 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/agency_pb2.py
+-rw-rw-rw-   0        0        0     1874 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/analyte_pb2.py
+-rw-rw-rw-   0        0        0     2811 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/analyte_result_pb2.py
+-rw-rw-rw-   0        0        0     1769 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/analyte_results_import_profile_pb2.py
+-rw-rw-rw-   0        0        0     1758 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/analyte_results_import_telemetry_pb2.py
+-rw-rw-rw-   0        0        0     1223 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/apierror_pb2.py
+-rw-rw-rw-   0        0        0     1393 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/apiresponse_pb2.py
+-rw-rw-rw-   0        0        0     1941 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/auditevent_pb2.py
+-rw-rw-rw-   0        0        0     1474 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/cell_monitor_backup_pb2.py
+-rw-rw-rw-   0        0        0     1519 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/cell_pb2.py
+-rw-rw-rw-   0        0        0     1541 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/celldata_binding_pb2.py
+-rw-rw-rw-   0        0        0     1988 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/celldata_pb2.py
+-rw-rw-rw-   0        0        0     1534 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/cells_pb2.py
+-rw-rw-rw-   0        0        0     1871 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/cellvalue_backup_pb2.py
+-rw-rw-rw-   0        0        0     4778 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/client_pb2.py
+-rw-rw-rw-   0        0        0     2054 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/coagmeasurement_pb2.py
+-rw-rw-rw-   0        0        0     2429 2024-05-01 18:09:28.000000 one_interfaces-6.9.0/one_interfaces/column_pb2.py
+-rw-rw-rw-   0        0        0     2097 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/computation_binding_pb2.py
+-rw-rw-rw-   0        0        0     2564 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/computation_pb2.py
+-rw-rw-rw-   0        0        0     1893 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/computation_variable_binding_pb2.py
+-rw-rw-rw-   0        0        0     2027 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/configuration_note_pb2.py
+-rw-rw-rw-   0        0        0     2970 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/configuration_pb2.py
+-rw-rw-rw-   0        0        0     1499 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/configuration_tag_pb2.py
+-rw-rw-rw-   0        0        0    13410 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/content_pb2.py
+-rw-rw-rw-   0        0        0     1951 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/csv_configuration_file_pb2.py
+-rw-rw-rw-   0        0        0     1743 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/data_source_binding_pb2.py
+-rw-rw-rw-   0        0        0     2052 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/data_source_configuration_pb2.py
+-rw-rw-rw-   0        0        0     1536 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     2041 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py
+-rw-rw-rw-   0        0        0     1523 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     3269 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_pb2.py
+-rw-rw-rw-   0        0        0     2247 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_subtype_pb2.py
+-rw-rw-rw-   0        0        0     3800 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     2063 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_type_pb2.py
+-rw-rw-rw-   0        0        0     2020 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/digital_twin_user_right_pb2.py
+-rw-rw-rw-   0        0        0     1342 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/display_options_pb2.py
+-rw-rw-rw-   0        0        0     1820 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/enterprise_data_source_definition_pb2.py
+-rw-rw-rw-   0        0        0     1669 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enterprise_data_table_definition_pb2.py
+-rw-rw-rw-   0        0        0     1376 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enterprise_data_table_field_pb2.py
+-rw-rw-rw-   0        0        0     1605 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py
+-rw-rw-rw-   0        0        0     1508 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enterprise_data_table_query_pb2.py
+-rw-rw-rw-   0        0        0     2309 2024-05-01 18:09:29.000000 one_interfaces-6.9.0/one_interfaces/enterprise_dataset_definition_pb2.py
+-rw-rw-rw-   0        0        0     1303 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_aggregate_pb2.py
+-rw-rw-rw-   0        0        0     1408 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_auditevent_pb2.py
+-rw-rw-rw-   0        0        0     1385 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_azure_notification_hubtype_pb2.py
+-rw-rw-rw-   0        0        0     1642 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_cell_range_action_pb2.py
+-rw-rw-rw-   0        0        0     1782 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_datasource_pb2.py
+-rw-rw-rw-   0        0        0     1392 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_day_pb2.py
+-rw-rw-rw-   0        0        0     1515 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py
+-rw-rw-rw-   0        0        0     1381 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_digital_twin_restriction_pb2.py
+-rw-rw-rw-   0        0        0     1422 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_digital_twin_user_right_pb2.py
+-rw-rw-rw-   0        0        0     1339 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_domain_source_pb2.py
+-rw-rw-rw-   0        0        0     1373 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_entity_pb2.py
+-rw-rw-rw-   0        0        0     1433 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_identity_provider_pb2.py
+-rw-rw-rw-   0        0        0     1552 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_import_status_pb2.py
+-rw-rw-rw-   0        0        0     1416 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_limit_operation_pb2.py
+-rw-rw-rw-   0        0        0     1437 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_limit_pb2.py
+-rw-rw-rw-   0        0        0     1545 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_month_pb2.py
+-rw-rw-rw-   0        0        0     1606 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_notification_category_pb2.py
+-rw-rw-rw-   0        0        0     1557 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_notification_delivery_method_pb2.py
+-rw-rw-rw-   0        0        0     1427 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_notification_message_type_pb2.py
+-rw-rw-rw-   0        0        0     1346 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_notification_platform_pb2.py
+-rw-rw-rw-   0        0        0     1452 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_one_log_level_pb2.py
+-rw-rw-rw-   0        0        0     1374 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_output_placement_pb2.py
+-rw-rw-rw-   0        0        0     1269 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_rendering_engine_pb2.py
+-rw-rw-rw-   0        0        0     1681 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py
+-rw-rw-rw-   0        0        0     1663 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_reportable_qualifier_pb2.py
+-rw-rw-rw-   0        0        0     3080 2024-05-01 18:09:30.000000 one_interfaces-6.9.0/one_interfaces/enum_sampling_statistic_pb2.py
+-rw-rw-rw-   0        0        0     1483 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_time_context_pb2.py
+-rw-rw-rw-   0        0        0     1388 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_time_unit_pb2.py
+-rw-rw-rw-   0        0        0    27482 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_timezone_pb2.py
+-rw-rw-rw-   0        0        0     1415 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_valid_value_restriction_pb2.py
+-rw-rw-rw-   0        0        0     1376 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_variable_type_pb2.py
+-rw-rw-rw-   0        0        0     2357 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_wims_week_definition_pb2.py
+-rw-rw-rw-   0        0        0     1341 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/enum_worksheet_pb2.py
+-rw-rw-rw-   0        0        0     1768 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/execution_details_pb2.py
+-rw-rw-rw-   0        0        0     1756 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/execution_parameter_pb2.py
+-rw-rw-rw-   0        0        0     1211 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/expression_line_pb2.py
+-rw-rw-rw-   0        0        0     2205 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/feature_pb2.py
+-rw-rw-rw-   0        0        0     1589 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/feature_state_type_pb2.py
+-rw-rw-rw-   0        0        0     1793 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/file_configuration_pb2.py
+-rw-rw-rw-   0        0        0     1563 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/gauge_data_point_pb2.py
+-rw-rw-rw-   0        0        0     1560 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/gis_pb2.py
+-rw-rw-rw-   0        0        0     1231 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/historian_binding_pb2.py
+-rw-rw-rw-   0        0        0     1981 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/historian_data_pb2.py
+-rw-rw-rw-   0        0        0     1536 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/i18nkey_text_reference_pb2.py
+-rw-rw-rw-   0        0        0     1855 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/ingest_client_pb2.py
+-rw-rw-rw-   0        0        0     1698 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/jsonTicksDateTime_pb2.py
+-rw-rw-rw-   0        0        0     1325 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/key_value_pb2.py
+-rw-rw-rw-   0        0        0     1668 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/limit_configuration_pb2.py
+-rw-rw-rw-   0        0        0     2385 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/limit_pb2.py
+-rw-rw-rw-   0        0        0     1948 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/measurement_pb2.py
+-rw-rw-rw-   0        0        0     1842 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/model_execution_pb2.py
+-rw-rw-rw-   0        0        0     1424 2024-05-01 18:09:31.000000 one_interfaces-6.9.0/one_interfaces/model_location_pb2.py
+-rw-rw-rw-   0        0        0     2433 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/model_template_pb2.py
+-rw-rw-rw-   0        0        0     1233 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/multi_point2d_pb2.py
+-rw-rw-rw-   0        0        0     1233 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/multi_point3d_pb2.py
+-rw-rw-rw-   0        0        0     1472 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/note_pb2.py
+-rw-rw-rw-   0        0        0     1695 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_broadcast_pb2.py
+-rw-rw-rw-   0        0        0     1448 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_contact_pb2.py
+-rw-rw-rw-   0        0        0     1859 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_device_pb2.py
+-rw-rw-rw-   0        0        0     2430 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_direct_preference_pb2.py
+-rw-rw-rw-   0        0        0     2254 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_event_pb2.py
+-rw-rw-rw-   0        0        0     2267 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_in_app_notification_message_pb2.py
+-rw-rw-rw-   0        0        0     1743 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_preference_pb2.py
+-rw-rw-rw-   0        0        0     2174 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_template_pb2.py
+-rw-rw-rw-   0        0        0     2201 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_topic_pb2.py
+-rw-rw-rw-   0        0        0     1828 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_topic_variable_pb2.py
+-rw-rw-rw-   0        0        0     2450 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/notification_user_preference_pb2.py
+-rw-rw-rw-   0        0        0     2455 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/operation_export_pb2.py
+-rw-rw-rw-   0        0        0     2111 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/outputcell_backup_pb2.py
+-rw-rw-rw-   0        0        0     1552 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/pagination_pb2.py
+-rw-rw-rw-   0        0        0     2177 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/parameter_agency_code_pb2.py
+-rw-rw-rw-   0        0        0     1674 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/parameter_agency_code_type_pb2.py
+-rw-rw-rw-   0        0        0     1819 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/parameter_definition_pb2.py
+-rw-rw-rw-   0        0        0     2356 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/parameter_pb2.py
+-rw-rw-rw-   0        0        0     1451 2024-05-01 18:09:32.000000 one_interfaces-6.9.0/one_interfaces/parameter_value_pb2.py
+-rw-rw-rw-   0        0        0     2569 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/plant_status_pb2.py
+-rw-rw-rw-   0        0        0     1158 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/point2d_pb2.py
+-rw-rw-rw-   0        0        0     1186 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/point3d_pb2.py
+-rw-rw-rw-   0        0        0     1637 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/post_filtering_column_definition_pb2.py
+-rw-rw-rw-   0        0        0     1878 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/post_filtering_pb2.py
+-rw-rw-rw-   0        0        0     1585 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/privileges_pb2.py
+-rw-rw-rw-   0        0        0     2503 2024-05-01 18:09:33.000000 one_interfaces-6.9.0/one_interfaces/product_offering_pb2.py
+-rw-rw-rw-   0        0        0     2064 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/quantity_type_pb2.py
+-rw-rw-rw-   0        0        0     1448 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/record_auditinfo_pb2.py
+-rw-rw-rw-   0        0        0     2076 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/report_definition_json_v2_pb2.py
+-rw-rw-rw-   0        0        0     2780 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/report_definition_pb2.py
+-rw-rw-rw-   0        0        0     2178 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/report_definition_runs_pb2.py
+-rw-rw-rw-   0        0        0     1842 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/report_definition_tags_pb2.py
+-rw-rw-rw-   0        0        0     1677 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/report_parameter_pb2.py
+-rw-rw-rw-   0        0        0     2382 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/report_run_pb2.py
+-rw-rw-rw-   0        0        0     1971 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/reportable_qualifier_definition_pb2.py
+-rw-rw-rw-   0        0        0     1417 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/reportable_qualifier_pb2.py
+-rw-rw-rw-   0        0        0     1252 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/rights_pb2.py
+-rw-rw-rw-   0        0        0     2008 2024-05-01 18:10:13.000000 one_interfaces-6.9.0/one_interfaces/role_pb2.py
+-rw-rw-rw-   0        0        0     1972 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/row_index_pb2.py
+-rw-rw-rw-   0        0        0     1346 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/row_merge_result_pb2.py
+-rw-rw-rw-   0        0        0     1692 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/row_pb2.py
+-rw-rw-rw-   0        0        0     1403 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/schedule_occurrence_pb2.py
+-rw-rw-rw-   0        0        0     2186 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/schedule_pb2.py
+-rw-rw-rw-   0        0        0     1472 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/schedule_recurrence_pattern_pb2.py
+-rw-rw-rw-   0        0        0     1887 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/schedule_type_pb2.py
+-rw-rw-rw-   0        0        0     2533 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/scope_pb2.py
+-rw-rw-rw-   0        0        0     1931 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/search_option_pb2.py
+-rw-rw-rw-   0        0        0     2186 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/series_pb2.py
+-rw-rw-rw-   0        0        0     2279 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/service_tech_tenant_request_pb2.py
+-rw-rw-rw-   0        0        0     1649 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/signalr_one_hub_connection_info_pb2.py
+-rw-rw-rw-   0        0        0     1261 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py
+-rw-rw-rw-   0        0        0     1567 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/signalr_one_hub_event_payload_pb2.py
+-rw-rw-rw-   0        0        0     1598 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/signalr_one_hub_event_pb2.py
+-rw-rw-rw-   0        0        0     1624 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/signalr_one_hub_message_pb2.py
+-rw-rw-rw-   0        0        0     1197 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/spreadsheet_binding_pb2.py
+-rw-rw-rw-   0        0        0     1699 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/spreadsheet_computation_pb2.py
+-rw-rw-rw-   0        0        0     1753 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/spreadsheet_definition_pb2.py
+-rw-rw-rw-   0        0        0     1500 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/spreadsheet_pb2.py
+-rw-rw-rw-   0        0        0     1912 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/template_parameter_pb2.py
+-rw-rw-rw-   0        0        0     2465 2024-05-01 18:10:14.000000 one_interfaces-6.9.0/one_interfaces/tenant_pb2.py
+-rw-rw-rw-   0        0        0     1680 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/tenant_product_offering_pb2.py
+-rw-rw-rw-   0        0        0     2113 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/test_analyte_group_pb2.py
+-rw-rw-rw-   0        0        0     1415 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/time_context_pb2.py
+-rw-rw-rw-   0        0        0     2106 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/timeseriesdata_pb2.py
+-rw-rw-rw-   0        0        0     1372 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/timewindow_pb2.py
+-rw-rw-rw-   0        0        0     1499 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/timezones_pb2.py
+-rw-rw-rw-   0        0        0     1835 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/unit_agency_code_pb2.py
+-rw-rw-rw-   0        0        0     1627 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/unit_agency_code_type_pb2.py
+-rw-rw-rw-   0        0        0     1701 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/unit_pb2.py
+-rw-rw-rw-   0        0        0     1308 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/user_password_management_pb2.py
+-rw-rw-rw-   0        0        0     4289 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/user_pb2.py
+-rw-rw-rw-   0        0        0     1812 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/user_preference_pb2.py
+-rw-rw-rw-   0        0        0     1969 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/user_profile_pb2.py
+-rw-rw-rw-   0        0        0     1784 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/valid_value_pb2.py
+-rw-rw-rw-   0        0        0     1966 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/variable_pb2.py
+-rw-rw-rw-   0        0        0     1799 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/worksheet_definition_pb2.py
+-rw-rw-rw-   0        0        0     1511 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/worksheet_pb2.py
+-rw-rw-rw-   0        0        0     1789 2024-05-01 18:10:15.000000 one_interfaces-6.9.0/one_interfaces/worksheet_view_pb2.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:11:20.439651 one_interfaces-6.9.0/one_interfaces.egg-info/
+-rw-rw-rw-   0        0        0     1217 2024-05-01 18:11:19.000000 one_interfaces-6.9.0/one_interfaces.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7583 2024-05-01 18:11:19.000000 one_interfaces-6.9.0/one_interfaces.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 18:11:19.000000 one_interfaces-6.9.0/one_interfaces.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 18:11:19.000000 one_interfaces-6.9.0/one_interfaces.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        4 2022-07-05 14:29:22.000000 one_interfaces-6.9.0/requirements.txt
+-rw-rw-rw-   0        0        0      159 2024-05-01 18:11:20.442652 one_interfaces-6.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2022-11-11 17:30:03.000000 one_interfaces-6.9.0/setup.py
```

### Comparing `one_interfaces-6.8.0/LICENSE.txt` & `one_interfaces-6.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/PKG-INFO` & `one_interfaces-6.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: one_interfaces
-Version: 6.8.0
+Version: 6.9.0
 Summary: Python bindings for ONE.
 Home-page: https://github.com/aquaticinformatics/one_interfaces
 Author: Aquatic Informatics
 Author-email: info@aquaticinformatics.com
 Maintainer: Aquatic Informatics
 License: BSD
 Description: One_Interfaces
```

### Comparing `one_interfaces-6.8.0/one_interfaces/account_status_pb2.py` & `one_interfaces-6.9.0/one_interfaces/account_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/activity_pb2.py` & `one_interfaces-6.9.0/one_interfaces/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/activity_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/activity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/address_pb2.py` & `one_interfaces-6.9.0/one_interfaces/address_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/agency_pb2.py` & `one_interfaces-6.9.0/one_interfaces/agency_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/analyte_pb2.py` & `one_interfaces-6.9.0/one_interfaces/analyte_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/analyte_result_pb2.py` & `one_interfaces-6.9.0/one_interfaces/analyte_result_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/analyte_results_import_profile_pb2.py` & `one_interfaces-6.9.0/one_interfaces/analyte_results_import_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/analyte_results_import_telemetry_pb2.py` & `one_interfaces-6.9.0/one_interfaces/analyte_results_import_telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/apierror_pb2.py` & `one_interfaces-6.9.0/one_interfaces/apierror_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/apiresponse_pb2.py` & `one_interfaces-6.9.0/one_interfaces/apiresponse_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/auditevent_pb2.py` & `one_interfaces-6.9.0/one_interfaces/auditevent_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/cell_monitor_backup_pb2.py` & `one_interfaces-6.9.0/one_interfaces/cell_monitor_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/cell_pb2.py` & `one_interfaces-6.9.0/one_interfaces/cell_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/celldata_binding_pb2.py` & `one_interfaces-6.9.0/one_interfaces/celldata_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/celldata_pb2.py` & `one_interfaces-6.9.0/one_interfaces/celldata_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/cells_pb2.py` & `one_interfaces-6.9.0/one_interfaces/cells_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/cellvalue_backup_pb2.py` & `one_interfaces-6.9.0/one_interfaces/cellvalue_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/client_pb2.py` & `one_interfaces-6.9.0/one_interfaces/client_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/coagmeasurement_pb2.py` & `one_interfaces-6.9.0/one_interfaces/coagmeasurement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/column_pb2.py` & `one_interfaces-6.9.0/one_interfaces/column_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/computation_binding_pb2.py` & `one_interfaces-6.9.0/one_interfaces/computation_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/computation_pb2.py` & `one_interfaces-6.9.0/one_interfaces/computation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/computation_variable_binding_pb2.py` & `one_interfaces-6.9.0/one_interfaces/computation_variable_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/configuration_note_pb2.py` & `one_interfaces-6.9.0/one_interfaces/configuration_note_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/configuration_pb2.py` & `one_interfaces-6.9.0/one_interfaces/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/configuration_tag_pb2.py` & `one_interfaces-6.9.0/one_interfaces/configuration_tag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/content_pb2.py` & `one_interfaces-6.9.0/one_interfaces/content_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/csv_configuration_file_pb2.py` & `one_interfaces-6.9.0/one_interfaces/csv_configuration_file_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/data_source_binding_pb2.py` & `one_interfaces-6.9.0/one_interfaces/data_source_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/data_source_configuration_pb2.py` & `one_interfaces-6.9.0/one_interfaces/data_source_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_subtype_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/digital_twin_user_right_pb2.py` & `one_interfaces-6.9.0/one_interfaces/digital_twin_user_right_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/display_options_pb2.py` & `one_interfaces-6.9.0/one_interfaces/display_options_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enterprise_data_source_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enterprise_data_source_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enterprise_data_table_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_field_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enterprise_data_table_field_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enterprise_data_table_query_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enterprise_data_table_query_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enterprise_dataset_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enterprise_dataset_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_aggregate_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_aggregate_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_auditevent_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_auditevent_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_azure_notification_hubtype_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_azure_notification_hubtype_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_cell_range_action_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_cell_range_action_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_datasource_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_day_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_day_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_digital_twin_restriction_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_digital_twin_restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_digital_twin_user_right_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_digital_twin_user_right_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_domain_source_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_domain_source_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_entity_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_identity_provider_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_identity_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_import_status_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_import_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_limit_operation_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_limit_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_limit_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_limit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_month_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_month_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_notification_category_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_notification_category_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_notification_delivery_method_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_notification_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_notification_message_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_notification_message_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_notification_platform_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_notification_platform_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_one_log_level_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_one_log_level_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_output_placement_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_output_placement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_rendering_engine_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_rendering_engine_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_reportable_qualifier_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_reportable_qualifier_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_sampling_statistic_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_sampling_statistic_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_time_context_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_time_context_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_time_unit_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_time_unit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_timezone_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_valid_value_restriction_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_valid_value_restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_variable_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_variable_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_wims_week_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_wims_week_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/enum_worksheet_pb2.py` & `one_interfaces-6.9.0/one_interfaces/enum_worksheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/execution_details_pb2.py` & `one_interfaces-6.9.0/one_interfaces/execution_details_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/execution_parameter_pb2.py` & `one_interfaces-6.9.0/one_interfaces/series_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: execution_parameter.proto
+# source: series.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import limit_pb2 as limit__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x65xecution_parameter.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x9b\x02\n\x12\x45xecutionParameter\x12\x10\n\x08modelTag\x18\x01 \x01(\t\x12\x11\n\tmodelUnit\x18\x02 \x01(\t\x12\x30\n\nupperLimit\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nlowerLimit\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\x06values\x18\x05 \x03(\x0b\x32\x1f.ExecutionParameter.ValuesEntry\x1aK\n\x0bValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue:\x02\x38\x01\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cseries.proto\x1a\x0blimit.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x02\n\tTelemetry\x12\x13\n\x0bparameterId\x18\x01 \x01(\x05\x12\x15\n\rparameterGuid\x18\x02 \x01(\t\x12\x0e\n\x06unitId\x18\x03 \x01(\r\x12\x10\n\x08unitGuid\x18\x04 \x01(\t\x12\x11\n\tprecision\x18\x05 \x01(\r\x12.\n\ndatapoints\x18\x06 \x03(\x0b\x32\x1a.Telemetry.DatapointsEntry\x12\x16\n\x06limits\x18\x07 \x03(\x0b\x32\x06.Limit\x12/\n\ttwinRefId\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x1a\x31\n\x0f\x44\x61tapointsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"#\n\x06Series\x12\x19\n\x05items\x18\x01 \x03(\x0b\x32\n.TelemetryB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'execution_parameter_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'series_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._options = None
-  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._serialized_options = b'8\001'
-  _globals['_EXECUTIONPARAMETER']._serialized_start=62
-  _globals['_EXECUTIONPARAMETER']._serialized_end=345
-  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._serialized_start=270
-  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._serialized_end=345
+  _globals['_TELEMETRY_DATAPOINTSENTRY']._options = None
+  _globals['_TELEMETRY_DATAPOINTSENTRY']._serialized_options = b'8\001'
+  _globals['_TELEMETRY']._serialized_start=62
+  _globals['_TELEMETRY']._serialized_end=342
+  _globals['_TELEMETRY_DATAPOINTSENTRY']._serialized_start=293
+  _globals['_TELEMETRY_DATAPOINTSENTRY']._serialized_end=342
+  _globals['_SERIES']._serialized_start=344
+  _globals['_SERIES']._serialized_end=379
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/expression_line_pb2.py` & `one_interfaces-6.9.0/one_interfaces/expression_line_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/feature_pb2.py` & `one_interfaces-6.9.0/one_interfaces/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/feature_state_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/feature_state_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/file_configuration_pb2.py` & `one_interfaces-6.9.0/one_interfaces/file_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/gauge_data_point_pb2.py` & `one_interfaces-6.9.0/one_interfaces/gauge_data_point_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/gis_pb2.py` & `one_interfaces-6.9.0/one_interfaces/gis_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/historian_binding_pb2.py` & `one_interfaces-6.9.0/one_interfaces/historian_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/historian_data_pb2.py` & `one_interfaces-6.9.0/one_interfaces/historian_data_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/i18nkey_text_reference_pb2.py` & `one_interfaces-6.9.0/one_interfaces/i18nkey_text_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/ingest_client_pb2.py` & `one_interfaces-6.9.0/one_interfaces/ingest_client_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/jsonTicksDateTime_pb2.py` & `one_interfaces-6.9.0/one_interfaces/jsonTicksDateTime_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/key_value_pb2.py` & `one_interfaces-6.9.0/one_interfaces/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/limit_configuration_pb2.py` & `one_interfaces-6.9.0/one_interfaces/limit_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/limit_pb2.py` & `one_interfaces-6.9.0/one_interfaces/limit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/measurement_pb2.py` & `one_interfaces-6.9.0/one_interfaces/measurement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/model_execution_pb2.py` & `one_interfaces-6.9.0/one_interfaces/model_execution_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import execution_parameter_pb2 as execution__parameter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15model_execution.proto\x1a\x19\x65xecution_parameter.proto\"\xc7\x01\n\x0eModelExecution\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\ttwinRefId\x18\x03 \x01(\t\x12\x17\n\x0f\x65xternalModelId\x18\x04 \x01(\t\x12\x1d\n\x15\x66orecastDurationHours\x18\x05 \x01(\x01\x12#\n\x06inputs\x18\x06 \x03(\x0b\x32\x13.ExecutionParameter\x12$\n\x07outputs\x18\x07 \x03(\x0b\x32\x13.ExecutionParameter\"1\n\x0fModelExecutions\x12\x1e\n\x05items\x18\x01 \x03(\x0b\x32\x0f.ModelExecutionB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15model_execution.proto\x1a\x19\x65xecution_parameter.proto\"\xed\x01\n\x0eModelExecution\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\ttwinRefId\x18\x03 \x01(\t\x12\x17\n\x0f\x65xternalModelId\x18\x04 \x01(\t\x12\x10\n\x08tenantId\x18\x05 \x01(\t\x12\x1d\n\x15\x66orecastDurationHours\x18\x06 \x01(\x01\x12\x12\n\ntimestamps\x18\x07 \x03(\t\x12#\n\x06inputs\x18\x08 \x03(\x0b\x32\x13.ExecutionParameter\x12$\n\x07outputs\x18\t \x03(\x0b\x32\x13.ExecutionParameter\"1\n\x0fModelExecutions\x12\x1e\n\x05items\x18\x01 \x03(\x0b\x32\x0f.ModelExecutionB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'model_execution_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
   _globals['_MODELEXECUTION']._serialized_start=53
-  _globals['_MODELEXECUTION']._serialized_end=252
-  _globals['_MODELEXECUTIONS']._serialized_start=254
-  _globals['_MODELEXECUTIONS']._serialized_end=303
+  _globals['_MODELEXECUTION']._serialized_end=290
+  _globals['_MODELEXECUTIONS']._serialized_start=292
+  _globals['_MODELEXECUTIONS']._serialized_end=341
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/model_location_pb2.py` & `one_interfaces-6.9.0/one_interfaces/model_location_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/model_template_pb2.py` & `one_interfaces-6.9.0/one_interfaces/model_template_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/multi_point2d_pb2.py` & `one_interfaces-6.9.0/one_interfaces/multi_point2d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/multi_point3d_pb2.py` & `one_interfaces-6.9.0/one_interfaces/multi_point3d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/note_pb2.py` & `one_interfaces-6.9.0/one_interfaces/note_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_broadcast_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_contact_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_contact_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_device_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_device_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_direct_preference_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_direct_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_event_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_in_app_notification_message_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_in_app_notification_message_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_preference_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_template_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_template_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_topic_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_topic_variable_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_topic_variable_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/notification_user_preference_pb2.py` & `one_interfaces-6.9.0/one_interfaces/notification_user_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/operation_export_pb2.py` & `one_interfaces-6.9.0/one_interfaces/operation_export_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/outputcell_backup_pb2.py` & `one_interfaces-6.9.0/one_interfaces/outputcell_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/pagination_pb2.py` & `one_interfaces-6.9.0/one_interfaces/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/parameter_agency_code_pb2.py` & `one_interfaces-6.9.0/one_interfaces/parameter_agency_code_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/parameter_agency_code_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/parameter_agency_code_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/parameter_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/parameter_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/parameter_pb2.py` & `one_interfaces-6.9.0/one_interfaces/parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/plant_status_pb2.py` & `one_interfaces-6.9.0/one_interfaces/plant_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/point2d_pb2.py` & `one_interfaces-6.9.0/one_interfaces/point2d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/point3d_pb2.py` & `one_interfaces-6.9.0/one_interfaces/point3d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/post_filtering_column_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/post_filtering_column_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/post_filtering_pb2.py` & `one_interfaces-6.9.0/one_interfaces/post_filtering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/privileges_pb2.py` & `one_interfaces-6.9.0/one_interfaces/privileges_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/product_offering_pb2.py` & `one_interfaces-6.9.0/one_interfaces/product_offering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/quantity_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/quantity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/record_auditinfo_pb2.py` & `one_interfaces-6.9.0/one_interfaces/record_auditinfo_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/report_definition_json_v2_pb2.py` & `one_interfaces-6.9.0/one_interfaces/report_definition_json_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/report_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/report_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/report_definition_runs_pb2.py` & `one_interfaces-6.9.0/one_interfaces/report_definition_runs_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/report_definition_tags_pb2.py` & `one_interfaces-6.9.0/one_interfaces/report_definition_tags_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/report_parameter_pb2.py` & `one_interfaces-6.9.0/one_interfaces/report_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/report_run_pb2.py` & `one_interfaces-6.9.0/one_interfaces/report_run_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/reportable_qualifier_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/reportable_qualifier_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/reportable_qualifier_pb2.py` & `one_interfaces-6.9.0/one_interfaces/reportable_qualifier_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/rights_pb2.py` & `one_interfaces-6.9.0/one_interfaces/rights_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/role_pb2.py` & `one_interfaces-6.9.0/one_interfaces/role_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/row_index_pb2.py` & `one_interfaces-6.9.0/one_interfaces/row_index_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/row_merge_result_pb2.py` & `one_interfaces-6.9.0/one_interfaces/row_merge_result_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/row_pb2.py` & `one_interfaces-6.9.0/one_interfaces/row_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/schedule_occurrence_pb2.py` & `one_interfaces-6.9.0/one_interfaces/schedule_occurrence_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/schedule_pb2.py` & `one_interfaces-6.9.0/one_interfaces/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/schedule_recurrence_pattern_pb2.py` & `one_interfaces-6.9.0/one_interfaces/schedule_recurrence_pattern_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/schedule_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/schedule_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/scope_pb2.py` & `one_interfaces-6.9.0/one_interfaces/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/search_option_pb2.py` & `one_interfaces-6.9.0/one_interfaces/search_option_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/series_pb2.py` & `one_interfaces-6.9.0/one_interfaces/test_analyte_group_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: series.proto
+# source: test_analyte_group.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import limit_pb2 as limit__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+import record_auditinfo_pb2 as record__auditinfo__pb2
+import analyte_pb2 as analyte__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cseries.proto\x1a\x0blimit.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x02\n\tTelemetry\x12\x13\n\x0bparameterId\x18\x01 \x01(\x05\x12\x15\n\rparameterGuid\x18\x02 \x01(\t\x12\x0e\n\x06unitId\x18\x03 \x01(\r\x12\x10\n\x08unitGuid\x18\x04 \x01(\t\x12\x11\n\tprecision\x18\x05 \x01(\r\x12.\n\ndatapoints\x18\x06 \x03(\x0b\x32\x1a.Telemetry.DatapointsEntry\x12\x16\n\x06limits\x18\x07 \x03(\x0b\x32\x06.Limit\x12/\n\ttwinRefId\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x1a\x31\n\x0f\x44\x61tapointsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"#\n\x06Series\x12\x19\n\x05items\x18\x01 \x03(\x0b\x32\n.TelemetryB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18test_analyte_group.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x16record_auditinfo.proto\x1a\ranalyte.proto\"\xb0\x02\n\x10TestAnalyteGroup\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rauthTwinRefId\x18\x03 \x01(\t\x12\x31\n\x0bpropertyBag\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cuiDefinition\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05notes\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x10\n\x08isActive\x18\x07 \x01(\x08\x12\x1a\n\x08\x61nalytes\x18\x08 \x03(\x0b\x32\x08.Analyte\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"5\n\x11TestAnalyteGroups\x12 \n\x05items\x18\x01 \x03(\x0b\x32\x11.TestAnalyteGroupB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'series_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'test_analyte_group_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_TELEMETRY_DATAPOINTSENTRY']._options = None
-  _globals['_TELEMETRY_DATAPOINTSENTRY']._serialized_options = b'8\001'
-  _globals['_TELEMETRY']._serialized_start=62
-  _globals['_TELEMETRY']._serialized_end=342
-  _globals['_TELEMETRY_DATAPOINTSENTRY']._serialized_start=293
-  _globals['_TELEMETRY_DATAPOINTSENTRY']._serialized_end=342
-  _globals['_SERIES']._serialized_start=344
-  _globals['_SERIES']._serialized_end=379
+  _globals['_TESTANALYTEGROUP']._serialized_start=100
+  _globals['_TESTANALYTEGROUP']._serialized_end=404
+  _globals['_TESTANALYTEGROUPS']._serialized_start=406
+  _globals['_TESTANALYTEGROUPS']._serialized_end=459
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/service_tech_tenant_request_pb2.py` & `one_interfaces-6.9.0/one_interfaces/service_tech_tenant_request_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_connection_info_pb2.py` & `one_interfaces-6.9.0/one_interfaces/signalr_one_hub_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py` & `one_interfaces-6.9.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_payload_pb2.py` & `one_interfaces-6.9.0/one_interfaces/signalr_one_hub_event_payload_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_event_pb2.py` & `one_interfaces-6.9.0/one_interfaces/signalr_one_hub_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/signalr_one_hub_message_pb2.py` & `one_interfaces-6.9.0/one_interfaces/signalr_one_hub_message_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/spreadsheet_binding_pb2.py` & `one_interfaces-6.9.0/one_interfaces/spreadsheet_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/spreadsheet_computation_pb2.py` & `one_interfaces-6.9.0/one_interfaces/spreadsheet_computation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/spreadsheet_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/spreadsheet_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/spreadsheet_pb2.py` & `one_interfaces-6.9.0/one_interfaces/spreadsheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/template_parameter_pb2.py` & `one_interfaces-6.9.0/one_interfaces/template_parameter_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18template_parameter.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xca\x02\n\x11TemplateParameter\x12\x13\n\x0bparameterId\x18\x01 \x01(\r\x12\x11\n\toneUnitId\x18\x02 \x01(\r\x12\x31\n\x0btelemetryId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x10\n\x08modelTag\x18\x05 \x01(\t\x12\x11\n\tmodelUnit\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nupperLimit\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nlowerLimit\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValueB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18template_parameter.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xfe\x02\n\x11TemplateParameter\x12\x13\n\x0bparameterId\x18\x01 \x01(\r\x12\x11\n\toneUnitId\x18\x02 \x01(\r\x12\x31\n\x0btelemetryId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x10\n\x08modelTag\x18\x05 \x01(\t\x12\x11\n\tmodelUnit\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nupperLimit\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nlowerLimit\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x64\x65\x66\x61ultValue\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValueB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'template_parameter_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
   _globals['_TEMPLATEPARAMETER']._serialized_start=61
-  _globals['_TEMPLATEPARAMETER']._serialized_end=391
+  _globals['_TEMPLATEPARAMETER']._serialized_end=443
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/tenant_pb2.py` & `one_interfaces-6.9.0/one_interfaces/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/tenant_product_offering_pb2.py` & `one_interfaces-6.9.0/one_interfaces/tenant_product_offering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/test_analyte_group_pb2.py` & `one_interfaces-6.9.0/one_interfaces/user_profile_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: test_analyte_group.proto
+# source: user_profile.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 import record_auditinfo_pb2 as record__auditinfo__pb2
-import analyte_pb2 as analyte__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18test_analyte_group.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x16record_auditinfo.proto\x1a\ranalyte.proto\"\xb0\x02\n\x10TestAnalyteGroup\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rauthTwinRefId\x18\x03 \x01(\t\x12\x31\n\x0bpropertyBag\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cuiDefinition\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05notes\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x10\n\x08isActive\x18\x07 \x01(\x08\x12\x1a\n\x08\x61nalytes\x18\x08 \x03(\x0b\x32\x08.Analyte\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"5\n\x11TestAnalyteGroups\x12 \n\x05items\x18\x01 \x03(\x0b\x32\x11.TestAnalyteGroupB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12user_profile.proto\x1a\x16record_auditinfo.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a google/protobuf/field_mask.proto\"\xe1\x01\n\x0bUserProfile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x0clanguageCode\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11\x63urrentLocationId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\nupdateMask\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"+\n\x0cUserProfiles\x12\x1b\n\x05items\x18\x01 \x03(\x0b\x32\x0c.UserProfileB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'test_analyte_group_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_profile_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_TESTANALYTEGROUP']._serialized_start=100
-  _globals['_TESTANALYTEGROUP']._serialized_end=404
-  _globals['_TESTANALYTEGROUPS']._serialized_start=406
-  _globals['_TESTANALYTEGROUPS']._serialized_end=459
+  _globals['_USERPROFILE']._serialized_start=113
+  _globals['_USERPROFILE']._serialized_end=338
+  _globals['_USERPROFILES']._serialized_start=340
+  _globals['_USERPROFILES']._serialized_end=383
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/time_context_pb2.py` & `one_interfaces-6.9.0/one_interfaces/time_context_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/timeseriesdata_pb2.py` & `one_interfaces-6.9.0/one_interfaces/timeseriesdata_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/timewindow_pb2.py` & `one_interfaces-6.9.0/one_interfaces/timewindow_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/timezones_pb2.py` & `one_interfaces-6.9.0/one_interfaces/timezones_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/unit_agency_code_pb2.py` & `one_interfaces-6.9.0/one_interfaces/unit_agency_code_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/unit_agency_code_type_pb2.py` & `one_interfaces-6.9.0/one_interfaces/unit_agency_code_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/unit_pb2.py` & `one_interfaces-6.9.0/one_interfaces/unit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/user_password_management_pb2.py` & `one_interfaces-6.9.0/one_interfaces/user_password_management_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/user_pb2.py` & `one_interfaces-6.9.0/one_interfaces/user_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/user_preference_pb2.py` & `one_interfaces-6.9.0/one_interfaces/user_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/user_profile_pb2.py` & `one_interfaces-6.9.0/one_interfaces/variable_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: user_profile.proto
+# source: variable.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import record_auditinfo_pb2 as record__auditinfo__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
-from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
+import enum_variable_type_pb2 as enum__variable__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12user_profile.proto\x1a\x16record_auditinfo.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a google/protobuf/field_mask.proto\"\xe1\x01\n\x0bUserProfile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x0clanguageCode\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11\x63urrentLocationId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\nupdateMask\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"+\n\x0cUserProfiles\x12\x1b\n\x05items\x18\x01 \x03(\x0b\x32\x0c.UserProfileB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0evariable.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x18\x65num_variable_type.proto\"\xa4\x02\n\x08Variable\x12\x0f\n\x07i18nKey\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12:\n\x14suggestedParameterId\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x0e\n\x06values\x18\x05 \x03(\x01\x12\'\n\x0cvariableType\x18\x06 \x01(\x0e\x32\x11.EnumVariableType\x12\x32\n\x0c\x65rrorMessage\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\x08rowCount\x18\t \x01(\x0b\x32\x1b.google.protobuf.Int32ValueH\x00\x42\n\n\x08metadata\"%\n\tVariables\x12\x18\n\x05items\x18\x01 \x03(\x0b\x32\t.VariableB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_profile_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'variable_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_USERPROFILE']._serialized_start=113
-  _globals['_USERPROFILE']._serialized_end=338
-  _globals['_USERPROFILES']._serialized_start=340
-  _globals['_USERPROFILES']._serialized_end=383
+  _globals['_VARIABLE']._serialized_start=77
+  _globals['_VARIABLE']._serialized_end=369
+  _globals['_VARIABLES']._serialized_start=371
+  _globals['_VARIABLES']._serialized_end=408
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/valid_value_pb2.py` & `one_interfaces-6.9.0/one_interfaces/valid_value_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/variable_pb2.py` & `one_interfaces-6.9.0/one_interfaces/parameter_value_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: variable.proto
+# source: parameter_value.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
-import enum_variable_type_pb2 as enum__variable__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0evariable.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x18\x65num_variable_type.proto\"\xa4\x02\n\x08Variable\x12\x0f\n\x07i18nKey\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12:\n\x14suggestedParameterId\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x0e\n\x06values\x18\x05 \x03(\x01\x12\'\n\x0cvariableType\x18\x06 \x01(\x0e\x32\x11.EnumVariableType\x12\x32\n\x0c\x65rrorMessage\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\x08rowCount\x18\t \x01(\x0b\x32\x1b.google.protobuf.Int32ValueH\x00\x42\n\n\x08metadata\"%\n\tVariables\x12\x18\n\x05items\x18\x01 \x03(\x0b\x32\t.VariableB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15parameter_value.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x83\x01\n\x0eParameterValue\x12\x11\n\ttimestamp\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bstringValue\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'variable_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'parameter_value_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_VARIABLE']._serialized_start=77
-  _globals['_VARIABLE']._serialized_end=369
-  _globals['_VARIABLES']._serialized_start=371
-  _globals['_VARIABLES']._serialized_end=408
+  _globals['_PARAMETERVALUE']._serialized_start=58
+  _globals['_PARAMETERVALUE']._serialized_end=189
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.8.0/one_interfaces/worksheet_definition_pb2.py` & `one_interfaces-6.9.0/one_interfaces/worksheet_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/worksheet_pb2.py` & `one_interfaces-6.9.0/one_interfaces/worksheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces/worksheet_view_pb2.py` & `one_interfaces-6.9.0/one_interfaces/worksheet_view_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.8.0/one_interfaces.egg-info/PKG-INFO` & `one_interfaces-6.9.0/one_interfaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: one-interfaces
-Version: 6.8.0
+Version: 6.9.0
 Summary: Python bindings for ONE.
 Home-page: https://github.com/aquaticinformatics/one_interfaces
 Author: Aquatic Informatics
 Author-email: info@aquaticinformatics.com
 Maintainer: Aquatic Informatics
 License: BSD
 Description: One_Interfaces
```

### Comparing `one_interfaces-6.8.0/one_interfaces.egg-info/SOURCES.txt` & `one_interfaces-6.9.0/one_interfaces.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 one_interfaces/operation_export_pb2.py
 one_interfaces/outputcell_backup_pb2.py
 one_interfaces/pagination_pb2.py
 one_interfaces/parameter_agency_code_pb2.py
 one_interfaces/parameter_agency_code_type_pb2.py
 one_interfaces/parameter_definition_pb2.py
 one_interfaces/parameter_pb2.py
+one_interfaces/parameter_value_pb2.py
 one_interfaces/plant_status_pb2.py
 one_interfaces/point2d_pb2.py
 one_interfaces/point3d_pb2.py
 one_interfaces/post_filtering_column_definition_pb2.py
 one_interfaces/post_filtering_pb2.py
 one_interfaces/privileges_pb2.py
 one_interfaces/product_offering_pb2.py
```

### Comparing `one_interfaces-6.8.0/setup.py` & `one_interfaces-6.9.0/setup.py`

 * *Files identical despite different names*

