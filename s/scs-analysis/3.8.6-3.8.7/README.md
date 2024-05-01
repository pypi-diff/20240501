# Comparing `tmp/scs_analysis-3.8.6.tar.gz` & `tmp/scs_analysis-3.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs_analysis-3.8.6.tar", last modified: Tue Apr 30 09:03:10 2024, max compression
+gzip compressed data, was "scs_analysis-3.8.7.tar", last modified: Wed May  1 09:51:06 2024, max compression
```

## Comparing `scs_analysis-3.8.6.tar` & `scs_analysis-3.8.7.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.421790 scs_analysis-3.8.6/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.6/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-30 09:03:10.421579 scs_analysis-3.8.6/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-30 09:03:10.421827 scs_analysis-3.8.6/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.393802 scs_analysis-3.8.6/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.408030 scs_analysis-3.8.6/src/scs_analysis/
--rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/__init__.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.6/src/scs_analysis/alert.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.6/src/scs_analysis/alert_status.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/aws_byline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.6/src/scs_analysis/aws_client_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/aws_mqtt_client.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/aws_topic_history.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4140 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/aws_topic_origin.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/aws_topic_publisher.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/aws_upload_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/baseline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.6/src/scs_analysis/baseline_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.409463 scs_analysis-3.8.6/src/scs_analysis/chart/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6609 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/client_traffic.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.419559 scs_analysis-3.8.6/src/scs_analysis/cmd/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert.py
--rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_origin.py
--rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     4821 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_client_traffic.py
--rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_email.py
--rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-r--r--   0 bruno      (502) admin       (80)     4805 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     4539 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     2373 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_join.py
--rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_controller.py
--rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3454 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_node.py
--rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisations.py
--rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_error.py
--rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
--rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_density.py
--rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_localize.py
--rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_median.py
--rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_record.py
--rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_single_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_uds.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5844 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6685 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_email.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_user_credentials.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8095 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_user_identity.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7640 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_csv.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3591 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4000 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_monitor_check.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4110 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_report.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_collation_summary.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_join.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_reader.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_segmentor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.6/src/scs_analysis/csv_writer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs_analysis-3.8.6/src/scs_analysis/device_controller.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs_analysis-3.8.6/src/scs_analysis/device_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.6/src/scs_analysis/device_monitor_status.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.421068 scs_analysis-3.8.6/src/scs_analysis/handler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/handler/batch_download_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/configuration_csv_generator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5567 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/handler/csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5903 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/handler/csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/mqtt_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/sample_midpoint.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/histo_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2175 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/localised_datetime.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/monitor_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/multi_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.6/src/scs_analysis/node.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_path_roots.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_user_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs_analysis-3.8.6/src/scs_analysis/organisations.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.6/src/scs_analysis/sample_aggregate.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_average.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_distance.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_duplicates.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_error.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_gas_concentration.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/sample_gas_density.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/sample_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.6/src/scs_analysis/sample_iso_8601.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_localize.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_low_pass.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_max.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_median.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_midpoint.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_min.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/sample_noise.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_nullify.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/sample_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.6/src/scs_analysis/sample_slope.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_sort.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_stats.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/sample_subset.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_time_shift.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/socket_receiver.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.6/src/scs_analysis/timer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/uds_receiver.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.421270 scs_analysis-3.8.6/src/scs_analysis.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.724794 scs_analysis-3.8.7/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.7/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-05-01 09:51:06.724563 scs_analysis-3.8.7/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-05-01 09:51:06.724838 scs_analysis-3.8.7/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.696774 scs_analysis-3.8.7/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.711302 scs_analysis-3.8.7/src/scs_analysis/
+-rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/__init__.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.7/src/scs_analysis/alert.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.7/src/scs_analysis/alert_status.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/aws_byline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.7/src/scs_analysis/aws_client_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/aws_mqtt_client.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/aws_topic_history.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4140 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/aws_topic_origin.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/aws_topic_publisher.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/aws_upload_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/baseline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.7/src/scs_analysis/baseline_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.712662 scs_analysis-3.8.7/src/scs_analysis/chart/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6609 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/client_traffic.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.722627 scs_analysis-3.8.7/src/scs_analysis/cmd/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_origin.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4821 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_client_traffic.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4805 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4539 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2373 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3984 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3454 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5416 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4679 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4657 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6495 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6209 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisations.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_density.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_localize.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_uds.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5912 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6958 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_email.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_user_credentials.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8128 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_user_identity.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     9402 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7640 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_csv.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3591 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4000 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_monitor_check.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4110 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_report.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_collation_summary.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_join.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_reader.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_segmentor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.7/src/scs_analysis/csv_writer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7377 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/device_controller.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5405 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/device_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.7/src/scs_analysis/device_monitor_status.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.723993 scs_analysis-3.8.7/src/scs_analysis/handler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/handler/batch_download_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5567 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/handler/csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5903 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/handler/csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/mqtt_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/sample_midpoint.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/histo_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2175 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/localised_datetime.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/monitor_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/multi_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.7/src/scs_analysis/node.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6552 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5855 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_path_roots.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5563 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_user_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6565 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8124 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisations.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.7/src/scs_analysis/sample_aggregate.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_average.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_distance.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_duplicates.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_error.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_gas_concentration.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/sample_gas_density.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/sample_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.7/src/scs_analysis/sample_iso_8601.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_localize.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_low_pass.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_max.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_median.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_midpoint.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_min.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/sample_noise.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_nullify.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/sample_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.7/src/scs_analysis/sample_slope.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_sort.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_stats.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.7/src/scs_analysis/sample_subset.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_time_shift.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/socket_receiver.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.7/src/scs_analysis/timer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/uds_receiver.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.724214 scs_analysis-3.8.7/src/scs_analysis.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      252 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       13 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs_analysis-3.8.6/LICENSE` & `scs_analysis-3.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/PKG-INFO` & `scs_analysis-3.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.6
+Version: 3.8.7
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs_analysis-3.8.6/README.md` & `scs_analysis-3.8.7/README.md`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/setup.py` & `scs_analysis-3.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/alert.py` & `scs_analysis-3.8.7/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/alert_status.py` & `scs_analysis-3.8.7/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_byline.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_client_auth.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_mqtt_client.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_topic_history.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_topic_origin.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_topic_origin.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_topic_publisher.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/aws_upload_interval.py` & `scs_analysis-3.8.7/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/baseline.py` & `scs_analysis-3.8.7/src/scs_analysis/baseline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/baseline_conf.py` & `scs_analysis-3.8.7/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/chart/chart.py` & `scs_analysis-3.8.7/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/chart/histo_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/chart/multi_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/chart/single_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/client_traffic.py` & `scs_analysis-3.8.7/src/scs_analysis/client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert_status.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_origin.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_origin.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_client_traffic.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_email.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_report.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_join.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_controller.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,35 +17,35 @@
     """unix message line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -t DEVICE_TAG "
-                                                    "[{ [-w] [-i INDENT] | [-s] -m CMD_TOKENS }]] [-v] ",
+                                                    "{ [-s] -m CMD_TOKENS | [-w] [-i INDENT] } [-v] ",
                                               version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
                                  help="the device tag")
 
         # mode...
         self.__parser.add_option("--message", "-m", type="string", action="store", dest="message",
                                  help="send the given command(s)")
 
         # output...
-        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="wrapper", default=False,
-                                 help="report message wrapper")
-
         self.__parser.add_option("--std", "-s", action="store_true", dest="std", default=False,
                                  help="write to stderr and stdout")
 
+        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="wrapper", default=False,
+                                 help="report message wrapper")
+
         self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor_status.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_node.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find devices for the given organisation or device tag")
+                                 help="find devices for the organisation or device tag")
 
         self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
                                  help="create a device")
 
         self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
                                  help="delete the device")
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 class CmdOrganisationPathRoots(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [-l ORG_LABEL] | "
+        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [-l ORG_LABEL [-m]] | "
                                                     "-C -l ORG_LABEL -r PATH_ROOT | "
                                                     "-D -l ORG_LABEL -r PATH_ROOT } "
-                                                    "[-m] [-i INDENT] [-v]", version=version())
+                                                    "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -73,14 +73,17 @@
 
         if count != 1:
             return False
 
         if not self.find and self.org_label is None:
             return False
 
+        if self.memberships and self.org_label is None:
+            return False
+
         if (self.create or self.delete) and self.path_root is None:
             return False
 
         if self.__args:
             return False
 
         return True
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 class CmdOrganisationUserPaths(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F { -e EMAIL | -r PATH_ROOT } | "
+        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F -e EMAIL [-r PATH_ROOT] | "
                                                     "-C -e EMAIL -r PATH_ROOT -x PATH_EXTENSION | "
                                                     "-D -e EMAIL -r PATH_ROOT -x PATH_EXTENSION } "
                                                     "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find users for the given username or organisation")
+                                 help="find for email (and path root)")
 
         self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
-                                 help="create a user")
+                                 help="create an OUP")
 
         self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
-                                 help="delete the user for the given username and organisation")
+                                 help="delete for email, path root and extension")
 
         # fields...
         self.__parser.add_option("--email", "-e", type="string", action="store", dest="email",
-                                 help="the user's email address'")
+                                 help="the user's email address")
 
         self.__parser.add_option("--path-root", "-r", type="string", action="store", dest="path_root",
                                  help="the organisation path root")
 
         self.__parser.add_option("--path-extension", "-x", type="string", action="store", dest="path_extension",
-                                 help="the organisation path root")
+                                 help="the path extension")
 
         # output...
         self.__parser.add_option("--indent", "-i", type="int", action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find users for the given username or organisation")
+                                 help="Find users for the given username or organisation")
 
         self.__parser.add_option("--Retrieve", "-R", action="store_true", dest="retrieve", default=False,
-                                 help="retrieve the user for the given username and organisation")
+                                 help="Retrieve the user for the given username and organisation")
 
         self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
-                                 help="create a user")
+                                 help="Create a user")
 
         self.__parser.add_option("--Update", "-U", action="store_true", dest="update", default=False,
                                  help="Update the user")
 
         self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
-                                 help="delete the user for the given username and organisation")
+                                 help="Delete the user for the given username and organisation")
 
         # fields...
         self.__parser.add_option("--email", "-e", type="string", action="store", dest="email",
                                  help="the user's email address (exact match)")
 
         self.__parser.add_option("--org-label", "-l", type="string", action="store", dest="org_label",
                                  help="the organisation label")
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisations.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find the organisations I belong to")
+                                 help="Find the organisations visible to me")
 
         self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
-                                 help="create an organisation")
+                                 help="Create an organisation")
 
         self.__parser.add_option("--Update", "-U", type="string", action="store", dest="update",
-                                 help="update the organisation with the given LABEL")
+                                 help="Update the organisation with the given LABEL")
 
         self.__parser.add_option("--Delete", "-D", type="string", action="store", dest="delete",
-                                 help="delete the organisation")
+                                 help="Delete the organisation")
 
         # fields...
         self.__parser.add_option("--label", "-l", type="string", action="store", dest="label",
                                  help="the organisation label")
 
         self.__parser.add_option("--id", "-d", type="int", action="store", dest="id",
                                  help="the organisation ID")
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_error.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_concentration.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_density.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_localize.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_median.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_record.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_single_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_uds.py` & `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cognito_devices.py` & `scs_analysis-3.8.7/src/scs_analysis/cognito_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_devices utility is used to
+The cognito_devices utility is used to find, update or delete the Cognito identity records of SCS devices.
 
 SYNOPSIS
 cognito_devices.py  [-c CREDENTIALS] { -F [{ -t DEVICE_TAG | -n INVOICE }] [-m] | -U DEVICE_TAG INVOICE |
 -D DEVICE_TAG } [-i INDENT] [-v]
 
 EXAMPLES
 cognito_devices.py -vi4 -c super -F -m
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cognito_email.py` & `scs_analysis-3.8.7/src/scs_analysis/cognito_email.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,25 @@
 * UNCONFIRMED - the account creation email is re-sent
 * CONFIRMED - a password reset code is sent and the user account enters the PASSWORD_RESET_REQUIRED state
 * PASSWORD_RESET_REQUIRED - a password reset code is re-sent
 * FORCE_CHANGE_PASSWORD - the temporary password is re-sent
 
 Emails cannot be sent to users in the DISABLED state.
 
+When an email is received, the cognito_email utility should be used to process the response, which is one of:
+
+* Confirm account - using the emailed confirmation code
+* Set password - using the emailed temporary password
+* Reset password - using the emailed reset code
+
 SYNOPSIS
-cognito_email.py { -e | -s | -r } EMAIL [-v]
+cognito_email.py { -e | -c | -s | -r } [-v] EMAIL
 
 EXAMPLES
-./cognito_email.py -r someone@me.com
+cognito_email.py -r someone@me.com
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
 scs_analysis/cognito_user_identity
 scs_analysis/cognito_users
 """
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cognito_user_credentials.py` & `scs_analysis-3.8.7/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cognito_user_identity.py` & `scs_analysis-3.8.7/src/scs_analysis/cognito_user_identity.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,41 @@
 Created on 24 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_user_identity utility is used to create, update and retrieve the AWS Cognito identity for the user.
+The cognito_user_identity utility is used to create, update and retrieve a AWS Cognito identity for the user.
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
-excercised in order for the account to gain a CONFIRMED status.
+exercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
 cognito_user_identity.py [-c CREDENTIALS] | -C | -R | -U } [-i INDENT] [-v]
 
 EXAMPLES
-./cognito_user_identity.py -R
+cognito_user_identity.py -R -c super
 
 DOCUMENT EXAMPLE
-{"username": "506cd055-1978-4984-9f17-2fad77797fa1", "email": "bruno.beloff@southcoastscience.com",
-"given-name": "Bruno", "family-name": "Beloff", "confirmation-status": "CONFIRMED", "enabled": true,
-"email-verified": true, "is-super": true, "is-tester": true, "is-financial": true,
-"created": "2023-04-20T11:45:21Z", "last-updated": "2023-06-26T14:39:17Z"}
+{
+    "username": "dc4cc7c2-e591-4619-b6eb-c4700daf6dff",
+    "email": "production@southcoastscience.com",
+    "given-name": "Production",
+    "family-name": "User",
+    "confirmation-status": "CONFIRMED",
+    "enabled": true,
+    "email-verified": true,
+    "is-super": true,
+    "created": "2023-03-31T10:18:54Z",
+    "last-updated": "2023-03-31T10:34:58Z"
+}
 
 SEE ALSO
+scs_analysis/cognito_email
 scs_analysis/cognito_user_credentials
 
 RESOURCES
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 """
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/cognito_users.py` & `scs_analysis-3.8.7/src/scs_analysis/cognito_users.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,35 +4,69 @@
 Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_users utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
-by organisation administrators and superusers.
+The cognito_users utility is used to create, update and retrieve AWS Cognito identities on behalf of other users.
+The utility can only be used by organisation administrators and superusers.
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
-excercised in order for the account to gain a CONFIRMED status.
+exercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
-cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -c CONFIRMATION | -s { 0 | 1 } } }] | \
--C | -U -e EMAIL_ADDR | -D -e EMAIL_ADDR } [-i INDENT] [-v]
+cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -o CONFIRMATION | -s { 0 | 1 } } }] [-m] |
+-C -g GIVEN_NAME -f FAMILY_NAME -e EMAIL_ADDR | -U EMAIL_ADDR [-g GIVEN_NAME] [-f FAMILY_NAME] [-e EMAIL_ADDR]
+[-s { 0 | 1 }] | -D EMAIL_ADDR } [-i INDENT] [-v]
 
 EXAMPLES
 cognito_users.py -Fe bruno.beloff@southcoastscience.com
 
 DOCUMENT EXAMPLE
-{"username": "506cd055-1978-4984-9f17-2fad77797fa1", "email": "bruno.beloff@southcoastscience.com",
-"given-name": "Bruno", "family-name": "Beloff", "confirmation-status": "CONFIRMED", "enabled": true,
-"email-verified": true, "is-super": true, "is-tester": true, "is-financial": true,
-"created": "2023-04-20T11:45:21Z", "last-updated": "2023-06-26T14:39:17Z"}
+[
+Created on 24 Jan 2022
+
+@author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+source repo: scs_analysis
+
+DESCRIPTION
+The cognito_users utility is used to create, update and retrieve AWS Cognito identities on behalf of other users.
+The utility can only be used by organisation administrators and superusers.
+
+If the --Create function is used, an email is sent to the new user. The verification link in the email must be
+exercised in order for the account to gain a CONFIRMED status.
+
+SYNOPSIS
+cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -o CONFIRMATION | -s { 0 | 1 } } }] [-m] |
+-C -g GIVEN_NAME -f FAMILY_NAME -e EMAIL_ADDR | -U EMAIL_ADDR [-g GIVEN_NAME] [-f FAMILY_NAME] [-e EMAIL_ADDR]
+[-s { 0 | 1 }] | -D EMAIL_ADDR } [-i INDENT] [-v]
+
+EXAMPLES
+cognito_users.py -Fe bruno.beloff@southcoastscience.com
+
+DOCUMENT EXAMPLE
+[
+    {
+        "username": "506cd055-1978-4984-9f17-2fad77797fa1",
+        "email": "bruno.beloff@southcoastscience.com",
+        "given-name": "Bruno",
+        "family-name": "Beloff",
+        "confirmation-status": "CONFIRMED",
+        "enabled": true,
+        "email-verified": true,
+        "created": "2023-04-20T11:45:21Z",
+        "last-updated": "2024-04-18T13:15:23Z"
+    }
+]
 
 SEE ALSO
 scs_analysis/cognito_devices
+scs_analysis/cognito_email
 scs_analysis/cognito_user_credentials
 scs_analysis/organisation_users
 
 RESOURCES
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 """
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/configuration_csv.py` & `scs_analysis-3.8.7/src/scs_analysis/configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/configuration_monitor.py` & `scs_analysis-3.8.7/src/scs_analysis/configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/configuration_monitor_check.py` & `scs_analysis-3.8.7/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/configuration_report.py` & `scs_analysis-3.8.7/src/scs_analysis/configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/csv_collation_summary.py` & `scs_analysis-3.8.7/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/csv_collator.py` & `scs_analysis-3.8.7/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/csv_join.py` & `scs_analysis-3.8.7/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/csv_reader.py` & `scs_analysis-3.8.7/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/csv_segmentor.py` & `scs_analysis-3.8.7/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/csv_writer.py` & `scs_analysis-3.8.7/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/device_controller.py` & `scs_analysis-3.8.7/src/scs_analysis/device_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 In the batch message mode, each command should be separated by a semicolon (;). Each command is sent as a separate
 message. Typically, message tokens are presented on the command line wrapped in double quote (") characters.
 
 A maximum of 30 seconds is available for the device to respond to the published message. After this time, the
 device_controller utility will terminate.
 
 SYNOPSIS
-device_controller.py [-c CREDENTIALS] -t DEVICE_TAG [{ [-w] [-i INDENT] | [-s] -m CMD_TOKENS }]] [-v]
+device_controller.py [-c CREDENTIALS] -t DEVICE_TAG { [-s] -m CMD_TOKENS | [-w] [-i INDENT] } [-v]
 
 EXAMPLES
 device_controller.py -c super -t scs-be2-3 -s -m "vcal_baseline -i4; gas_baseline"
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/device_monitor.py` & `scs_analysis-3.8.7/src/scs_analysis/device_monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 
 """
 Created on 28 Jun 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 DESCRIPTION
-The device monitor periodically checks on the availability and health of every air quality monitoring device. The
-device_monitor utility is used to manage the email addresses associated with individual devices.
+The device monitor periodically checks on the availability and health of every air quality monitoring device.
+The device_monitor utility is used to manage the email addresses for alerts associated with individual devices.
 
 SYNOPSIS
 device_monitor.py [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -t DEVICE_TAG } [-x]] | -A EMAIL_ADDR DEVICE_TAG [-j] |
 -S DEVICE_TAG { 0 | 1 } | -D EMAIL_ADDR [{ -t DEVICE_TAG | -f }] } [-i INDENT] [-v]
 
 EXAMPLES
-device_monitor.py -c super -Ft scs-opc-109
+device_monitor.py -c super -Ft scs-bgx-570
 
 DOCUMENT EXAMPLE
-{"scs-be2-3": {"device-tag": "scs-be2-3", "recipients": [{"email": "bbeloff@me.com", "json-message": true},
-{"email": "bruno.beloff@southcoastscience.com", "json-message": false}], "suspended": false}}
+{
+    "scs-bgx-570": {
+        "device-tag": "scs-bgx-570",
+        "recipients": [
+            {
+                "email": "bruno.beloff@southcoastscience.com",
+                "json-message": false
+            }
+        ],
+        "suspended": false
+    }
+}
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
 scs_analysis/device_monitor_status
 """
 
 import sys
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/device_monitor_status.py` & `scs_analysis-3.8.7/src/scs_analysis/device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/batch_download_reporter.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/configuration_csv_generator.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/csv_collator.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/csv_segmentor.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/mqtt_reporter.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/sample_midpoint.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/handler/sample_regression.py` & `scs_analysis-3.8.7/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/histo_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/localised_datetime.py` & `scs_analysis-3.8.7/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/monitor_auth.py` & `scs_analysis-3.8.7/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/multi_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/node.py` & `scs_analysis-3.8.7/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/organisation_devices.py` & `scs_analysis-3.8.7/src/scs_analysis/organisation_devices.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,42 @@
 Created on 19 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_devices utility is used to
+The organisation_devices utility is used to manage the relationship between organisations and Cognito devices. The
+utility can find, create and delete these relationships.
+
+Over a period of time, a device may pass from ownership by one organisation to ownership by another. Each
+ownership period is represented by a separate record. Where the start of an ownership is not known, the start
+datetime is recorded as 1970-01-01T00:00:00Z.
 
 SYNOPSIS
-organisation_devices.py [-c CREDENTIALS] { -F { -l ORG_LABEL | -t DEVICE_TAG } | \
--C -l ORG_LABEL -t DEVICE_TAG -p PATH_ROOT GROUP LOCATION -d DEPLOYMENT_LABEL | \
--E -l ORG_LABEL -t DEVICE_TAG -p PATH_ROOT GROUP LOCATION | \
--D -t DEVICE_TAG } \
-[-i INDENT] [-v]
+organisation_devices.py [-c CREDENTIALS] { -F { -l ORG_LABEL | -t DEVICE_TAG } |
+-C -l ORG_LABEL -t DEVICE_TAG -p PATH_ROOT GROUP LOCATION -d DEPLOYMENT_LABEL | -D -t DEVICE_TAG } [-i INDENT] [-v]
 
 EXAMPLES
-organisation_devices.py -F -l NARA
+organisation_devices.py -F -l "South Coast Science (Demo)"
+
+organisation_devices.py -c super -vi4 -F -t scs-bgx-570
 
 DOCUMENT EXAMPLE
-{"DeviceTag": "scs-bgx-401", "OrgID": 1, "DevicePath": "south-coast-science-demo/brighton/loc/1/",
-"EnvironmentPath": "south-coast-science-demo/brighton/device/praxis-000401/",
-"StartDatetime": "2022-01-17T10:40:04Z", "EndDatetime": null,
-"DeploymentLabel": "Preston Circus"}
+[
+    {
+        "DeviceTag": "scs-bgx-570",
+        "OrgID": 68,
+        "DeploymentLabel": "Praxis / Urban @ Preston Circus, Brighton",
+        "DevicePath": "south-coast-science-demo/brighton-urban/device/praxis-000570/",
+        "LocationPath": "south-coast-science-demo/brighton-urban/loc/1/",
+        "StartDatetime": "2021-07-30T10:42:38Z",
+        "EndDatetime": null
+    }
+]
 
 SEE ALSO
 scs_analysis/cognito_devices
 scs_analysis/cognito_user_credentials
 """
 
 import sys
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/organisation_path_roots.py` & `scs_analysis-3.8.7/src/scs_analysis/organisation_user_paths.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,79 +4,97 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_path_roots utility is used to
+The organisation_user_paths utility is used to find, create or delete organisation user paths (OUPs). OUPs
+are used to restrict user access:
+
+* If no OUPs are associated with a user, then the user may view all of topics associated with the organisation(s)
+that the user is a member of
+
+* If one or more OUP is associated with a user, then the the user may only view the projects identified by the OUPs
+within an organisation path root
+
+See the organisation_path_roots utility for more information.
 
 SYNOPSIS
-organisation_path_roots.py  [-c CREDENTIALS] \
-{ -F -l ORG_LABEL | -C -l ORG_LABEL -r PATH_ROOT | -D -l ORG_LABEL -r PATH_ROOT } [-m] [-i INDENT] [-v]
+organisation_user_paths.py  [-c CREDENTIALS] { -F { -e EMAIL | -r PATH_ROOT } |
+-C -e EMAIL -r PATH_ROOT -x PATH_EXTENSION | -D -e EMAIL -r PATH_ROOT -x PATH_EXTENSION } [-i INDENT] [-v]
 
 EXAMPLES
-organisation_path_roots.py -vi4 -c super -Fl 4sfera -m
+organisation_user_paths.py -i4 -c super -F -e bruno.beloff@southcoastscience.com -r south-coast-science-demo/
 
 DOCUMENT EXAMPLE
-{"OPRID": 11, "OrgID": 1, "PathRoot": "ricardo/"}
+{
+    "Username": "506cd055-1978-4984-9f17-2fad77797fa1",
+    "OPRID": 75,
+    "PathExtension": "brighton-urban/"
+}
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
+scs_analysis/organisation_path_roots
 """
 
 import sys
 
-from scs_analysis.cmd.cmd_organisation_path_roots import CmdOrganisationPathRoots
+from scs_analysis.cmd.cmd_organisation_user_paths import CmdOrganisationUserPaths
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
-from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot
+from scs_core.aws.security.organisation import OrganisationPathRoot, OrganisationUserPath
 from scs_core.aws.security.organisation_manager import OrganisationManager
-from scs_core.aws.security.opr_membership import OPRMembership
-
-from scs_core.client.http_exception import HTTPException
+from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 
+from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    org = None
-    report = None
+    report = []
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdOrganisationPathRoots()
+        cmd = CmdOrganisationUserPaths()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisation_path_roots', verbose=cmd.verbose)
+        Logging.config('organisation_user_paths', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
-        if cmd.org_label is not None and not Organisation.is_valid_label(cmd.org_label):
-            logger.error("the organisation label '%s' is not valid." % cmd.org_label)
+        if not Datum.is_email_address(cmd.email):
+            logger.error("email address '%s' is not valid." % cmd.email)
             exit(2)
 
-        if cmd.path_root is not None and not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
-            logger.error("the path root '%s' is not valid." % cmd.path_root)
+        if cmd.path_root and not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
+            logger.error("path root '%s' is not valid." % cmd.path_root)
+            exit(2)
+
+        if cmd.path_extension is not None and not OrganisationUserPath.is_valid_path_extension(cmd.path_extension):
+            logger.error("path extension '%s' is not valid." % cmd.path_extension)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # authentication...
 
         credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
@@ -91,62 +109,59 @@
             logger.error("login: %s." % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
+        finder = CognitoUserFinder()
         manager = OrganisationManager()
 
 
         # ------------------------------------------------------------------------------------------------------------
         # validation...
 
-        if cmd.org_label is not None:
-            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
+        cognito = finder.get_by_email(auth.id_token, cmd.email)
+
+        if cognito is None:
+            logger.error("no Cognito user found for email: '%s'." % cmd.email)
+            exit(1)
+
+        if cmd.path_root:
+            opr = manager.get_opr_by_path_root(auth.id_token, cmd.path_root)
 
-            if org is None:
-                logger.error("no organisation found for label: '%s'." % cmd.org_label)
+            if opr is None:
+                logger.error("no organisation path root found for path: '%s'." % cmd.path_root)
                 exit(1)
 
-            org_id = org.org_id
+            opr_id = opr.opr_id
 
         else:
-            org_id = None
+            opr_id = None
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            report = manager.find_oprs(auth.id_token, org_id=org_id)
-
-            if cmd.memberships:
-                oups = manager.find_oups(auth.id_token)
-                report = OPRMembership.merge(report, oups)
+            report = manager.find_oups(auth.id_token, username=cognito.username, opr_id=opr_id)
 
         if cmd.create:
-            org = OrganisationPathRoot(0, org.org_id, cmd.path_root)
-            report = manager.insert_opr(auth.id_token, org)
+            report = OrganisationUserPath(cognito.username, opr_id, cmd.path_extension)
+            manager.assert_oup(auth.id_token, report)
 
         if cmd.delete:
-            opr = manager.get_opr_by_path_root(auth.id_token, cmd.path_root)
-
-            if opr is None:
-                logger.error("no path root found for path: '%s'." % cmd.path_root)
-                exit(1)
-
-            # delete...
-            manager.delete_opr(auth.id_token, opr.opr_id)
+            oup = OrganisationUserPath(cognito.username, opr_id, cmd.path_extension)
+            manager.delete_oup(auth.id_token, oup)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
-        if report is not None:
+        if not cmd.delete:
             print(JSONify.dumps(report, indent=cmd.indent))
 
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/organisation_users.py` & `scs_analysis-3.8.7/src/scs_analysis/organisation_users.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,49 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_users utility is used to
+The organisation_users utility is used to manage the relationship between organisations and Cognito users. The
+utility can find, create, update and delete organisation user records.
+
+Users may belong to more than one organisation. (Additionally, superusers typically belong to no organisation.)
+Organisation administrators and superusers can use this utility to add or remove membership of an organisation for
+individual users.
 
 SYNOPSIS
-organisation_users.py  [-c CREDENTIALS] { -F { -e EMAIL | -l ORG_LABEL } | \
--R -e EMAIL -l ORG_LABEL | \
--C -e EMAIL -l ORG_LABEL -o { 0 | 1 } -d { 0 | 1 } | \
--U -e EMAIL -l ORG_LABEL [-o { 0 | 1 }] [-d { 0 | 1 }] [-s { 0 | 1 }] | \
--D -e EMAIL -l ORG_LABEL } \
-[-i INDENT] [-v]
+organisation_users.py  [-c CREDENTIALS] {
+-F [{ -e EMAIL | -l ORG_LABEL }] |
+-R -e EMAIL -l ORG_LABEL |
+-C -e EMAIL -l ORG_LABEL -o { 0 | 1 } -d { 0 | 1 } |
+-U -e EMAIL -l ORG_LABEL [-o { 0 | 1 }] [-d { 0 | 1 }] [-s { 0 | 1 }] |
+-D -e EMAIL -l ORG_LABEL } [-i INDENT] [-v]
 
 EXAMPLES
-organisation_users.py -F -l NARA
+organisation_users.py -vi4 -c super -Fe bruno.beloff@southcoastscience.com
 
 DOCUMENT EXAMPLE
-{"Username": 111, "OrgID": 1, "IsOrgAdmin": true, "IsDeviceAdmin": true, "IsSuspended": false}
+[
+    {
+        "Username": "506cd055-1978-4984-9f17-2fad77797fa1",
+        "OrgID": 68,
+        "IsOrgAdmin": true,
+        "IsDeviceAdmin": false,
+        "IsSuspended": false
+    },
+    {
+        "Username": "506cd055-1978-4984-9f17-2fad77797fa1",
+        "OrgID": 69,
+        "IsOrgAdmin": true,
+        "IsDeviceAdmin": false,
+        "IsSuspended": false
+    }
+]
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
 scs_analysis/cognito_users
 """
 
 import sys
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/organisations.py` & `scs_analysis-3.8.7/src/scs_analysis/organisations.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,36 +7,62 @@
 
 source repo: scs_analysis
 
 DESCRIPTION
 The organisations utility is used to find, create, update or delete organisation records.
 
 The utility supports a parent / child relationship between organisations - a child organisation can be
-thought of as a subdivision of its parent. Users belonging to an organisation have the same rights over
-child organisation data and devices as then have
+thought of as a subdivision of its parent: users belonging to an organisation have the same rights over
+child organisation data and devices as they have for data and devices within their own organisation.
 
 SYNOPSIS
 organisations.py [-c CREDENTIALS] {
 -F [{ -l LABEL | -d ID }] [-m] |
 -C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL [-p PARENT_LABEL] |
 -U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] [-p PARENT_LABEL] |
 -D LABEL } [-i INDENT] [-v]
 
 EXAMPLES
-organisations.py -F
+organisations.py -vi4 -c super -U "South Coast Science (Test)" -p "South Coast Science (Dev)"
+
+organisations.py -vi4 -c super -Fl "South Coast Science (Dev)" -m
 
 DOCUMENT EXAMPLE
-{"OrgID": 1, "Label": "SCS", "LongName": "South Coast Science", "URL": "https://www.southcoastscience.com",
-"Owner": "bruno.beloff@southcoastscience.com", "ParentID": null}
+{
+    "OrgID": 68,
+    "Label": "South Coast Science (Demo)",
+    "LongName": "a demonstration of South Coast Science air quality monitoring instruments",
+    "URL": "https://www.southcoastscience.com",
+    "Owner": "bruno.beloff@southcoastscience.com",
+    "ParentID": null
+}
 
 DOCUMENT EXAMPLE - MEMBERSHIPS
-{"organisation": {"OrgID": 11, "Label": "CEPEMAR", "LongName": "CEPEMAR", "URL": "http://cepemar.com",
-"Owner": "felipe.tatagiba@cepemar.com", "ParentID": null}, "children": [
-{"OrgID": 82, "Label": "Vale", "LongName": "Vale S.A.", "URL": "http://www.vale.com/",
-"Owner": "felipe.tatagiba@cepemar.com", "ParentID": 11}]}
+[
+    {
+        "organisation": {
+            "OrgID": 69,
+            "Label": "South Coast Science (Dev)",
+            "LongName": "development operations for South Coast Science air quality monitoring instruments",
+            "URL": "https://www.southcoastscience.com",
+            "Owner": "bruno.beloff@southcoastscience.com",
+            "ParentID": null
+        },
+        "children": [
+            {
+                "OrgID": 71,
+                "Label": "South Coast Science (Test)",
+                "LongName": "a test account for South Coast Science customers",
+                "URL": "https://www.southcoastscience.com",
+                "Owner": "bruno.beloff@southcoastscience.com",
+                "ParentID": 69
+            }
+        ]
+    }
+]
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
 """
 
 import sys
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_aggregate.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_average.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_collator.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_distance.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_duplicates.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_error.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_gas_concentration.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_gas_density.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_interval.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_iso_8601.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_localize.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_low_pass.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_max.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_median.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_midpoint.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_min.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_noise.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_nullify.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_paths.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_regression.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_slope.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_sort.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_stats.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_subset.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/sample_time_shift.py` & `scs_analysis-3.8.7/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/single_chart.py` & `scs_analysis-3.8.7/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/socket_receiver.py` & `scs_analysis-3.8.7/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/timer.py` & `scs_analysis-3.8.7/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis/uds_receiver.py` & `scs_analysis-3.8.7/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.6/src/scs_analysis.egg-info/PKG-INFO` & `scs_analysis-3.8.7/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.6
+Version: 3.8.7
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs_analysis-3.8.6/src/scs_analysis.egg-info/SOURCES.txt` & `scs_analysis-3.8.7/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

