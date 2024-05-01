# Comparing `tmp/minknow_api-5.9.1.tar.gz` & `tmp/minknow_api-5.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minknow_api-5.9.1.tar", last modified: Wed Mar 27 10:46:27 2024, max compression
+gzip compressed data, was "minknow_api-5.9.5.tar", last modified: Wed May  1 13:05:03 2024, max compression
```

## Comparing `minknow_api-5.9.1.tar` & `minknow_api-5.9.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:27.907057 minknow_api-5.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-27 10:46:27.907057 minknow_api-5.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-27 10:46:17.000000 minknow_api-5.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:27.903057 minknow_api-5.9.1/minknow_api/
--rw-r--r--   0 runner    (1001) docker     (127)    28403 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/_support.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    44495 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/acquisition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25816 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/acquisition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/acquisition_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    83930 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/analysis_configuration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    37700 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/analysis_configuration_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    54764 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/analysis_configuration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    34708 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/basecaller_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28374 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/basecaller_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    42812 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/basecaller_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/ca.crt
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    52535 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28044 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39259 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/data_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    59790 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    60431 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/device_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/device_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:27.907057 minknow_api-5.9.1/minknow_api/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/create_client_certificates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7894 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/export_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/extract_run_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/list_sequencing_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/load_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/manage_simulated_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/run_after_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    24323 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/examples/start_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    18759 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18886 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/instance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20779 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/instance_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/keystore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/keystore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/keystore_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    68440 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/manager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    63963 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/manager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    78970 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/manager_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/minion_device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/minion_device_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/minion_device_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/post_processing_protocol_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26060 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/promethion_device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/promethion_device_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/promethion_device_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    54401 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/protocol_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    49056 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/protocol_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    60499 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/protocol_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/protocol_settings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/protocol_settings_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/protocol_settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/report_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/report_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/report_data_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/rpc_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/run_until_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/run_until_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18918 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/run_until_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    56661 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/statistics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26580 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/statistics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    48397 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/statistics_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:27.907057 minknow_api-5.9.1/minknow_api/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/tools/any_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19105 2024-03-27 10:46:17.000000 minknow_api-5.9.1/minknow_api/tools/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:46:27.907057 minknow_api-5.9.1/minknow_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-27 10:46:27.000000 minknow_api-5.9.1/minknow_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-27 10:46:27.000000 minknow_api-5.9.1/minknow_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 10:46:27.000000 minknow_api-5.9.1/minknow_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 10:46:27.000000 minknow_api-5.9.1/minknow_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 10:46:27.000000 minknow_api-5.9.1/minknow_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 10:46:27.907057 minknow_api-5.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-27 10:46:17.000000 minknow_api-5.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:05:03.959699 minknow_api-5.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-01 13:05:03.959699 minknow_api-5.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-01 13:04:55.000000 minknow_api-5.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:05:03.955699 minknow_api-5.9.5/minknow_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    28403 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44495 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/acquisition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25816 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/acquisition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/acquisition_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83930 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/analysis_configuration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37700 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/analysis_configuration_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54764 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/analysis_configuration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34708 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/basecaller_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28374 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/basecaller_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42812 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/basecaller_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52535 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28044 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39259 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/data_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59790 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60431 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/device_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/device_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:05:03.955699 minknow_api-5.9.5/minknow_api/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/create_client_certificates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7894 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/export_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/extract_run_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/list_sequencing_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/load_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/manage_simulated_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/run_after_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24952 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/examples/start_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18759 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18886 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/instance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20779 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/instance_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/keystore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/keystore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/keystore_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68440 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/manager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63963 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/manager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78970 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/manager_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/minion_device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/minion_device_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/minion_device_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/post_processing_protocol_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26060 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/promethion_device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/promethion_device_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/promethion_device_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54401 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/protocol_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49056 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/protocol_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60499 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/protocol_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/protocol_settings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/protocol_settings_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/protocol_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/report_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/report_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/report_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/rpc_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/run_until_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/run_until_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18918 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/run_until_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56661 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/statistics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26580 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/statistics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48397 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/statistics_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:05:03.959699 minknow_api-5.9.5/minknow_api/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/tools/any_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-01 13:04:55.000000 minknow_api-5.9.5/minknow_api/tools/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:05:03.959699 minknow_api-5.9.5/minknow_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-01 13:05:03.000000 minknow_api-5.9.5/minknow_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-01 13:05:03.000000 minknow_api-5.9.5/minknow_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:05:03.000000 minknow_api-5.9.5/minknow_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 13:05:03.000000 minknow_api-5.9.5/minknow_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 13:05:03.000000 minknow_api-5.9.5/minknow_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:05:03.959699 minknow_api-5.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-01 13:04:55.000000 minknow_api-5.9.5/setup.py
```

### Comparing `minknow_api-5.9.1/PKG-INFO` & `minknow_api-5.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minknow_api
-Version: 5.9.1
+Version: 5.9.5
 Summary: MinKNOW RPC API bindings
 Home-page: https://github.com/nanoporetech/minknow_api
 Author: Oxford Nanopore Technologies PLC
 Author-email: info@nanoporetech.com
 Description-Content-Type: text/markdown
 Requires-Dist: importlib-resources<3.3; python_version < "3.7.0"
 Requires-Dist: grpcio~=1.51
```

### Comparing `minknow_api-5.9.1/README.md` & `minknow_api-5.9.5/README.md`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/__init__.py` & `minknow_api-5.9.5/minknow_api/__init__.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/_support.py` & `minknow_api-5.9.5/minknow_api/_support.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/acquisition_pb2.py` & `minknow_api-5.9.5/minknow_api/acquisition_pb2.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,26 @@
   _globals['_SETBREAMINFOREQUEST']._serialized_end=6564
   _globals['_SETBREAMINFORESPONSE']._serialized_start=6566
   _globals['_SETBREAMINFORESPONSE']._serialized_end=6588
   _globals['_APPENDMUXSCANRESULTRESPONSE']._serialized_start=6590
   _globals['_APPENDMUXSCANRESULTRESPONSE']._serialized_end=6619
   _globals['_ACQUISITIONSERVICE']._serialized_start=7677
   _globals['_ACQUISITIONSERVICE']._serialized_end=9169
+MuxScanMetadata.__doc__ = """Provides information about how mux scans are configured.  This
+primarily information to help present mux scan results to the user
+(see `MuxScanResult`).
+
+Attributes:
+    auto_mux_scan_period_hours:
+        How frequently automatic scans are scheduled to occur.
+    category_groups:
+        Presentation information for categories.  Describes the
+        preferred way to present mux scan categories to users. Groups
+        should be presented in the order of this list.
+"""
 StopRequest.__doc__ = """Attributes:
     wait_until_ready:
         Defaults to false If false will return as soon as minknow
         enters the FINISHING state. If true then returns as soon as
         minknow enters the READY state.
     keep_power_on:
         Force the MinION/GridION ASIC power to be kept on after the
@@ -170,59 +182,56 @@
         this option is set to `false` (or is left unset), then the
         application configuration determines whether the power will be
         left on when the acquisition finishes -- see the
         `powered_when_idle` and `flongle_powered_when_idle`
         configuration options for further details.  This option has no
         effect on PromethIONs.  Since 1.15.2
 """
-ChannelStateInfo.__doc__ = """Attributes:
-    groups:
-        The groups of channel states.  The groups are ordered
-        according to the "order" attribute of the group style in the
-        channel states configuration.
-"""
-MuxScanResult.__doc__ = """A report of the states of channel muxes (wells) across the flow cell.
-Every channel mux (well) is assigned to a specific category describing
-its state (for example, is it expected to produce good results, and if
-not why not?). This is a report of how many channel muxes are in each
-category.
+BreamInfo.__doc__ = """Information provided by Bream.  Note that this is provided by the
+protocol, and some protocols may choose not to provide this.
 
 Attributes:
-    counts:
-        How many channel muxes are in each category.  The sum of all
-        the values in this map should be the number of channels
-        multiplied by the number of muxes on each channel (eg:
-        512x4=2048 on a MinION Mk1B without a flongle adapter).  eg.
-        'sequencing': 1500
-    mux_scan_timestamp:
-        When this mux scan result was added (Seconds since the start
-        of the acquisition).
+    mux_scan_metadata:
+        Presentation information for mux scan results.
+    mux_scan_results:
+        Mux scan results.
+    target_translocation_speed:
+        The ideal translocation speed range.  This can be used to
+        provide context for speed graphs (see the statistics RPCs),
+        showing what range is considered "good".
+    target_q_score:
+        The ideal quality (Q) score range.  This can be used to
+        provide context for q-score graphs (see the statistics RPCs),
+        showing what range is considered "good".
+    target_temperature:
+        The ideal temperature range.  This can be used to provide
+        context for temperature (see the statistics RPCs), showing
+        what range is considered "good".  Note that a protocol may
+        request a different temperature range than this (eg: it might
+        request a tighter range, or it may adjust the temperature it
+        is requesting throughout the run). This intended only to
+        provide context when presenting data to users.
 """
-AcquisitionYieldSummary.TotalsPerDuplexCategory.__doc__ = """Note: If duplex isn't enabled, all reads and basecalls will be classed
-as 'simplex' and the 'duplex' fields will be 0."""
-MuxScanMetadata.CategoryGroup.__doc__ = """Attributes:
+GetProgressResponse.__doc__ = """Attributes:
+    raw_per_channel:
+        The amount of raw data (per channel) that has been acquired
+        and processed.
+"""
+MuxScanMetadata.Category.__doc__ = """A category that a channel mux can be assigned.
+
+Attributes:
     name:
-        The name of the group.
+        Name of the category.  This is the value that will be in the
+        `MuxScanResult.counts` field.  The user should not be shown
+        this. Instead, `style.label` should be displayed.
     style:
-        How to render the group in a graphical user interface.
-    category:
-        The categories contained in the group.  Within this group,
-        categories should be presented in the order of this list.
-"""
-GetAcquisitionRunInfoRequest.__doc__ = """Attributes:
-    run_id:
-        The acquisition period to get information about.
-"""
-GetProgressResponse.RawPerChannel.__doc__ = """Attributes:
-    acquired:
-        Number of samples (per channel) acquired from the device.
-    processed:
-        Number of samples (per channel) passed to the analysis
-        pipeline for processing.  This can be compared to acquired to
-        see how far behind the analysis is lagging.
+        How to render the category in a graphical user interface.
+    global_order:
+        An order ranking for the category when displaying them without
+        using groups.
 """
 AcquisitionConfigSummary.__doc__ = """This field has been removed Since 5.8
 
 Attributes:
     purpose:
         The purpose, as supplied to `acquisition.start()`
     basecalling_enabled:
@@ -269,14 +278,117 @@
     events_to_base_ratio:
         Number of bases per event
     sample_rate:
         Sample rate for the acquisition.  Since 3.3
     channel_count:
         Channel count used in the acquisition.  Since 3.3
 """
+ChannelStateInfo.ChannelState.__doc__ = """Attributes:
+    id:
+        The numeric identifier of the state.  This is what is reported
+        in any other APIs that return a channel state ID.
+    name:
+        The internal name of the state.  This is what is reported in
+        any other APIs that return a channel state name.
+    style:
+        How to render the channel state in a graphical user interface.
+        Note that the style may be missing from some channel states
+        (such as the ones that are built in to MinKNOW).
+    global_order:
+        An order ranking for the channel states when they are
+        ungrouped.  This can be used to order the channel states after
+        merging the groups.
+"""
+ChannelStateInfo.Group.__doc__ = """Attributes:
+    name:
+        The name of the group.
+    style:
+        How to render the group in a graphical user interface.  Note
+        that the style may be missing from some groups (such as the
+        ones that are built in to MinKNOW).
+    states:
+        The channel states contained in the group.  The groups are
+        ordered according to the "order" attribute of the channel
+        state style in the channel states configuration.
+"""
+ChannelStateInfo.__doc__ = """Attributes:
+    groups:
+        The groups of channel states.  The groups are ordered
+        according to the "order" attribute of the group style in the
+        channel states configuration.
+"""
+ChannelStateInfo.Style.__doc__ = """Attributes:
+    label:
+        The human-readable name to display when rendering this channel
+        state or group.
+    description:
+        A sentence describing the meaning of the channel state or
+        group.  This can be used as a tooltip, for example.
+    colour:
+        The colour to use when rendering this channel state or group.
+        This is a six-digit hex string describing an RGB colour (eg:
+        "ff00ff" for purple).
+"""
+MuxScanResult.__doc__ = """A report of the states of channel muxes (wells) across the flow cell.
+Every channel mux (well) is assigned to a specific category describing
+its state (for example, is it expected to produce good results, and if
+not why not?). This is a report of how many channel muxes are in each
+category.
+
+Attributes:
+    counts:
+        How many channel muxes are in each category.  The sum of all
+        the values in this map should be the number of channels
+        multiplied by the number of muxes on each channel (eg:
+        512x4=2048 on a MinION Mk1B without a flongle adapter).  eg.
+        'sequencing': 1500
+    mux_scan_timestamp:
+        When this mux scan result was added (Seconds since the start
+        of the acquisition).
+"""
+MuxScanMetadata.Style.__doc__ = """Presentation information for a category or group.
+
+Attributes:
+    label:
+        The human-readable name to display when rendering this
+        category or group.
+    description:
+        A sentence describing the meaning of the category or group.
+        This can be used as a tooltip, for example.
+    colour:
+        The colour to use when rendering this category or group.  This
+        is a six-digit hex string describing an RGB colour (eg:
+        "ff0000" for red).
+"""
+BreamInfo.Range.__doc__ = """Represents a range of values."""
+SetBreamInfoRequest.__doc__ = """Attributes:
+    info:
+        The information to set.  Note that, other than treating the
+        top-level fields independently (see the other flags on this
+        request), MinKNOW Core will not do anything special to the
+        data. In particular, the caller must fill in the
+        `mux_scan_timestamp` field in `MuxScanResult` messages.
+    overwrite_unset_fields:
+        If any `BreamInfo` fields were set in a previous call, but are
+        unset in the `info` field of this call, then use the old value
+        for them.  For example, to just update the mux_scan_metadata
+        field, use a BreamInfo object with only the
+        `mux_scan_metadata` field set, and leave this as False. To
+        clear the entire BreamInfo structure, leave `info` empty and
+        set this to True.
+"""
+MuxScanMetadata.CategoryGroup.__doc__ = """Attributes:
+    name:
+        The name of the group.
+    style:
+        How to render the group in a graphical user interface.
+    category:
+        The categories contained in the group.  Within this group,
+        categories should be presented in the order of this list.
+"""
 StartRequest.__doc__ = """ Protobuf messages for input/output of RPC calls
 
 Attributes:
     dont_wait_for_device_ready:
         Prevent waiting until the device is ready before starting
         acquisition.  Defaults to false.  By default, MinKNOW will
         block in the start() call for the device and flow cell to be
@@ -342,34 +454,98 @@
         writing a final_summary.txt file if the purpose is set to
         SEQUENCING.  Since 3.5 (NB: in 3.3 and 3.4, final_summary.txt
         was always written out if file_output was enabled).
     start_request:
         Start request that will be used to trigger analysis, used to
         union over all the different types of analysis possible.
 """
+AcquisitionYieldSummary.TotalsPerDuplexCategory.__doc__ = """Note: If duplex isn't enabled, all reads and basecalls will be classed
+as 'simplex' and the 'duplex' fields will be 0."""
 AcquisitionWriterSummary.__doc__ = """Attributes:
     bytes_to_write_produced:
         Number of bytes which minknow needs to write in order to
         finish the experiment.
     bytes_to_write_failed:
         Number of bytes which minknow has failed to write to final
         location. These reads are instead contained in the
         fallback/tmp locations.
     bytes_to_write_completed:
         Number of bytes which minknow has written to final location.
 """
+StartResponse.__doc__ = """Attributes:
+    run_id:
+        Globally-unique identifier generated when the acquisition is
+        started.  This is guaranteed to unique, including aross
+        sequencing devices.
+"""
+AcquisitionRunInfo.__doc__ = """Attributes:
+    run_id:
+        The unique identifier assigned to this acquisition run.  This
+        is guaranteed to be made of ASCII characters, and at most 40
+        characters. It is globally unique across all acquisitions on
+        all MinKNOW instances.
+    startup_state:
+        Current startup task (or STARTUP_UNKNOWN if not starting up).
+    startup_state_estimated_end:
+        Estimated time for current startup state to end.  In some
+        cases this field is left unset, to indicate no estimation.
+    startup_state_estimated_percent_complete:
+        Estimate startup state completion percent (0 - 1).  In some
+        cases this field is left at 0, indicating no estimation.
+    state:
+        Indicates the current state of the acquisition.
+    finishing_state:
+        If the experiment is finishing, an extra piece of state
+        describing the current finishing state.
+    stop_reason:
+        The reason the acquisition period was ended.
+    start_time:
+        When the acquisition period was started (UTC).
+    data_read_start_time:
+        When MinKNOW began acquiring data (UTC).  Unset if the
+        acquisition is still starting up.
+    data_read_end_time:
+        When the MinKNOW stopped acquiring data (UTC).  Unset if the
+        acquisition is still acquiring.
+    end_time:
+        When the acquisition terminated (UTC).  Unset if the
+        acquisition period is still running.
+    yield_summary:
+        Summary of acquisition yields.  Since 1.12
+    config_summary:
+        Summary of the configuration settings for a run.  Since 1.14
+    writer_summary:
+        Summary of writer yields.  Since 4.0
+    bream_info:
+        Set information provided by the Bream toolkit.
+    target_run_until_criteria:
+        Target Run-Until Critiera, used to determine when the
+        acquisition should be paused or stopped.  Since 5.3
+"""
+GetProgressResponse.RawPerChannel.__doc__ = """Attributes:
+    acquired:
+        Number of samples (per channel) acquired from the device.
+    processed:
+        Number of samples (per channel) passed to the analysis
+        pipeline for processing.  This can be compared to acquired to
+        see how far behind the analysis is lagging.
+"""
 SetSignalReaderRequest.__doc__ = """Attributes:
     reader:
         The type of signal reader to use
     hdf_source:
         The following settings are optional, and only used when
         setting the reader to hdf5
     hdf_mode:
          Defaults to UNSPECIFIED, since this setting is optional
 """
+GetAcquisitionRunInfoRequest.__doc__ = """Attributes:
+    run_id:
+        The acquisition period to get information about.
+"""
 AcquisitionYieldSummary.__doc__ = """Attributes:
     read_count:
         Number of reads selected by analysis as good reads.  The reads
         in this counter are completed, but not necessarily on disk
         yet.
     fraction_basecalled:
         This is the fraction of whole reads that the base-caller has
@@ -429,184 +605,8 @@
     alignment_coverage:
         Number of bases that match the target reference(s) expressed
         as a fraction of the total size of the target reference(s).
         eg: For a specified alignment-targets with 2000 and 3000
         bases, if "alignment_matches" is 2500, then
         "alignment_coverage" will be 0.5  Since 4.3
 """
-ChannelStateInfo.Style.__doc__ = """Attributes:
-    label:
-        The human-readable name to display when rendering this channel
-        state or group.
-    description:
-        A sentence describing the meaning of the channel state or
-        group.  This can be used as a tooltip, for example.
-    colour:
-        The colour to use when rendering this channel state or group.
-        This is a six-digit hex string describing an RGB colour (eg:
-        "ff00ff" for purple).
-"""
-AcquisitionRunInfo.__doc__ = """Attributes:
-    run_id:
-        The unique identifier assigned to this acquisition run.  This
-        is guaranteed to be made of ASCII characters, and at most 40
-        characters. It is globally unique across all acquisitions on
-        all MinKNOW instances.
-    startup_state:
-        Current startup task (or STARTUP_UNKNOWN if not starting up).
-    startup_state_estimated_end:
-        Estimated time for current startup state to end.  In some
-        cases this field is left unset, to indicate no estimation.
-    startup_state_estimated_percent_complete:
-        Estimate startup state completion percent (0 - 1).  In some
-        cases this field is left at 0, indicating no estimation.
-    state:
-        Indicates the current state of the acquisition.
-    finishing_state:
-        If the experiment is finishing, an extra piece of state
-        describing the current finishing state.
-    stop_reason:
-        The reason the acquisition period was ended.
-    start_time:
-        When the acquisition period was started (UTC).
-    data_read_start_time:
-        When MinKNOW began acquiring data (UTC).  Unset if the
-        acquisition is still starting up.
-    data_read_end_time:
-        When the MinKNOW stopped acquiring data (UTC).  Unset if the
-        acquisition is still acquiring.
-    end_time:
-        When the acquisition terminated (UTC).  Unset if the
-        acquisition period is still running.
-    yield_summary:
-        Summary of acquisition yields.  Since 1.12
-    config_summary:
-        Summary of the configuration settings for a run.  Since 1.14
-    writer_summary:
-        Summary of writer yields.  Since 4.0
-    bream_info:
-        Set information provided by the Bream toolkit.
-    target_run_until_criteria:
-        Target Run-Until Critiera, used to determine when the
-        acquisition should be paused or stopped.  Since 5.3
-"""
-SetBreamInfoRequest.__doc__ = """Attributes:
-    info:
-        The information to set.  Note that, other than treating the
-        top-level fields independently (see the other flags on this
-        request), MinKNOW Core will not do anything special to the
-        data. In particular, the caller must fill in the
-        `mux_scan_timestamp` field in `MuxScanResult` messages.
-    overwrite_unset_fields:
-        If any `BreamInfo` fields were set in a previous call, but are
-        unset in the `info` field of this call, then use the old value
-        for them.  For example, to just update the mux_scan_metadata
-        field, use a BreamInfo object with only the
-        `mux_scan_metadata` field set, and leave this as False. To
-        clear the entire BreamInfo structure, leave `info` empty and
-        set this to True.
-"""
-MuxScanMetadata.Style.__doc__ = """Presentation information for a category or group.
-
-Attributes:
-    label:
-        The human-readable name to display when rendering this
-        category or group.
-    description:
-        A sentence describing the meaning of the category or group.
-        This can be used as a tooltip, for example.
-    colour:
-        The colour to use when rendering this category or group.  This
-        is a six-digit hex string describing an RGB colour (eg:
-        "ff0000" for red).
-"""
-GetProgressResponse.__doc__ = """Attributes:
-    raw_per_channel:
-        The amount of raw data (per channel) that has been acquired
-        and processed.
-"""
-StartResponse.__doc__ = """Attributes:
-    run_id:
-        Globally-unique identifier generated when the acquisition is
-        started.  This is guaranteed to unique, including aross
-        sequencing devices.
-"""
-ChannelStateInfo.Group.__doc__ = """Attributes:
-    name:
-        The name of the group.
-    style:
-        How to render the group in a graphical user interface.  Note
-        that the style may be missing from some groups (such as the
-        ones that are built in to MinKNOW).
-    states:
-        The channel states contained in the group.  The groups are
-        ordered according to the "order" attribute of the channel
-        state style in the channel states configuration.
-"""
-MuxScanMetadata.Category.__doc__ = """A category that a channel mux can be assigned.
-
-Attributes:
-    name:
-        Name of the category.  This is the value that will be in the
-        `MuxScanResult.counts` field.  The user should not be shown
-        this. Instead, `style.label` should be displayed.
-    style:
-        How to render the category in a graphical user interface.
-    global_order:
-        An order ranking for the category when displaying them without
-        using groups.
-"""
-ChannelStateInfo.ChannelState.__doc__ = """Attributes:
-    id:
-        The numeric identifier of the state.  This is what is reported
-        in any other APIs that return a channel state ID.
-    name:
-        The internal name of the state.  This is what is reported in
-        any other APIs that return a channel state name.
-    style:
-        How to render the channel state in a graphical user interface.
-        Note that the style may be missing from some channel states
-        (such as the ones that are built in to MinKNOW).
-    global_order:
-        An order ranking for the channel states when they are
-        ungrouped.  This can be used to order the channel states after
-        merging the groups.
-"""
-MuxScanMetadata.__doc__ = """Provides information about how mux scans are configured.  This
-primarily information to help present mux scan results to the user
-(see `MuxScanResult`).
-
-Attributes:
-    auto_mux_scan_period_hours:
-        How frequently automatic scans are scheduled to occur.
-    category_groups:
-        Presentation information for categories.  Describes the
-        preferred way to present mux scan categories to users. Groups
-        should be presented in the order of this list.
-"""
-BreamInfo.__doc__ = """Information provided by Bream.  Note that this is provided by the
-protocol, and some protocols may choose not to provide this.
-
-Attributes:
-    mux_scan_metadata:
-        Presentation information for mux scan results.
-    mux_scan_results:
-        Mux scan results.
-    target_translocation_speed:
-        The ideal translocation speed range.  This can be used to
-        provide context for speed graphs (see the statistics RPCs),
-        showing what range is considered "good".
-    target_q_score:
-        The ideal quality (Q) score range.  This can be used to
-        provide context for q-score graphs (see the statistics RPCs),
-        showing what range is considered "good".
-    target_temperature:
-        The ideal temperature range.  This can be used to provide
-        context for temperature (see the statistics RPCs), showing
-        what range is considered "good".  Note that a protocol may
-        request a different temperature range than this (eg: it might
-        request a tighter range, or it may adjust the temperature it
-        is requesting throughout the run). This intended only to
-        provide context when presenting data to users.
-"""
-BreamInfo.Range.__doc__ = """Represents a range of values."""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/acquisition_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/acquisition_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/acquisition_service.py` & `minknow_api-5.9.5/minknow_api/acquisition_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/analysis_configuration_pb2.py` & `minknow_api-5.9.5/minknow_api/analysis_configuration_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -208,148 +208,332 @@
   _globals['_SETDYNAMICANALYSISCONFIGURATIONRESPONSE']._serialized_end=13694
   _globals['_ANALYSISCONFIGURATIONSERVICE']._serialized_start=13697
   _globals['_ANALYSISCONFIGURATIONSERVICE']._serialized_end=16429
 DynamicAnalysisConfiguration.__doc__ = """Attributes:
     read_scale_tracking:
         Parameters for read scale tracking:
 """
-WriterConfiguration.ChannelConfiguration.ChannelRanges.__doc__ = """Attributes:
-    ranges:
-        List of start/end paired channel numbers which should be
-        enabled for writing.  All channels in inclusive ranges should
-        be enabled.
+BasecallerConfiguration.TargetFiltering.__doc__ = """Since 3.7"""
+BarcodingConfiguration.__doc__ = """Since 3.5
+
+Attributes:
+    barcoding_kits:
+        The barcoding kits in use One entry per kit If no barcoding
+        kits are supplied, barcoding is disabled.
+    trim_barcodes:
+        Whether Guppy should trim barcodes If not specified, this
+        value defaults to false (not triming barcodes) If barcoding is
+        not enabled (e.g., because no barcoding kits are specified),
+        this parameter has no effect.
+    require_barcodes_both_ends:
+        Barcode is only classified if a barcode above `min_score` is
+        present at both ends of the basecalled read.
+    detect_mid_strand_barcodes:
+        Search for barcodes through the entire length of the read.  If
+        a barcode is found in the middle of a read the read is marked
+        as unclassified.
+    min_score:
+        Minimum alignment score to consider a valid barcode.  Maximum
+        value is 100, defaults to 60.
+    min_score_rear:
+        Minimum score to consider a valid barcode (overrides min_score
+        for rear barcodes).  Maximum value is 100, defaults to
+        min_score if not specified.
+    min_score_mid:
+        Minimum score to consider a valid mid barcode (only valid if
+        detect_mid_strand_barcodes is specified).  Maximum value is
+        100, defaults to 60.
+    min_score_mask:
+        The minimum score required for the barcode mask to be
+        detected.  Maximum value is 100, defaults to 40.
+    ignore_unspecified_barcodes:
+        If set, barcodes that aren't in barcode user data list will be
+        ignored  Since 5.6
 """
 WriterConfiguration.ChannelConfiguration.__doc__ = """Used to control which channels for a specific data type emit data
 
 Attributes:
     channels:
         Control the way channels are enabled for this data type.
 """
-WriterConfiguration.BulkConfiguration.__doc__ = """Control settings for the bulk writer
-
-Attributes:
+ChannelStates.Logic.Behaviour.__doc__ = """Attributes:
+    reset_on_mux_change:
+        TODO: MinKNOW 5: replace int32 with bool for these options
+        these are ints but act like bools
+    latch:
+        If the latch value is set to true, then when the criteria for
+        this channel state is active, then the latch will keep it
+        active until the channel state is reset.
+    reset_on_effective_mux_change:
+        An 'effective mux change' is any mux change apart from the one
+        triggered with the purpose of disconnecting a channel (turning
+        a channel off). For example, if a channel is in pore, and the
+        user changes the channel configuration to 'disconnected', that
+        mux change will not be an effective mux change. Any other mux
+        change is considered an 'effective mux change'. So if a
+        channel saturates, the mux change to disconnected is an
+        effective mux change. Similarly, a change from disconnected to
+        a pore is an effective mux change.  Use this reset mode to
+        make the channel state persist on non-effective mux changes.
+        For example, if a channel state is in 'multiple' and the user
+        triggers a channel configuration change to 'disconnected', the
+        state will remain in multiple if it has this option on. The
+        multiple state will be reset at all other mux changes (i.e.
+        effective mux changes).
+    reset_on_effective_well_change:
+        An 'effective well change' is any well change apart from the
+        one triggered with the purpose of disconnecting a channel
+        (turning a channel off). For example, if a channel is in
+        well_1, and the user changes the channel configuration to
+        'unblock_1', that change will not be an effective well change.
+        A change to disconnected is also not considered an effective
+        well change.  Use this reset mode to make the channel state
+        persist on non-effective well changes. For example, if a
+        channel state is in 'multiple' and the user triggers a channel
+        configuration change to 'disconnected', the state will remain
+        in multiple if it has this option on. The multiple state will
+        be reset then when the mux is set to a different setting.
+"""
+WriterConfiguration.ReadBamConfiguration.__doc__ = """Attributes:
+    enable:
+        Control if a BAM file should be generated per channel.
+    file_pattern:
+        The pattern used to find a BAM files name.  default: bam{basec
+        all_status}/{flow_cell_id}_{run_id}_{batch_number}.bam Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+    batch_count:
+        How many reads are placed in each batch (after batch_count
+        reads {batch_number} is increased in the pattern).
+    bases_per_batch:
+        Number of estimated bases within a batch before it rotates to
+        a new batch
+    no_output_based_batching:
+        Do not perform batching based on output (time-based batching
+        is still performed, if specified)
+    disable_writing_multiple_alignments:
+        If true minknow will only write the primary alignment for each
+        read.
+    disable_writing_passed_reads:
+        Since 5.8 Prevent reads which have successfully basecalled
+        being written to bam.
+    disable_writing_failed_reads:
+        Prevent reads which have failed basecalling being written to
+        bam.
+    disable_writing_force_skipped_reads:
+        disable writing reads which have been force skipped by the
+        basecaller.
+    batch_duration:
+        The batch duration, for time-based batching  If time-based
+        batching is enabled then, in addition to completing batches
+        when the `batch_count` or `bases_per_batch` target (above) is
+        reached, batches will also be completed when: - At least one
+        read has been written to the batch, AND - `batch_duration` has
+        elapsed since the last batch was completed (or since the start
+        of the acquisition, for the first batch)  If this field is not
+        set, then the default time-based batching configuration will
+        be used.  If this field is set to zero or a negative value,
+        then time-based batching will be disabled.  Since 5.6
+"""
+DynamicAnalysisConfiguration.ReadScaleTracking.__doc__ = """Attributes:
+    conductance_scan_voltage:
+        Set the voltage the most recent conductance scan occured at.
+    channel_conductance:
+        Per channel/well conductance values
+"""
+PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.__doc__ = """Attributes:
+    pore_types:
+        Map with pore type as key, mapped to the list of wells to set
+        for.  It is undefined what will happen if one call sets the
+        pore type of a channel and well to two pore types.
+"""
+ReadClassificationParams.__doc__ = """Attributes:
+    max_sample_size:
+        This tells minknow the maximum number of means to store in
+        memory before using a different strategy to calculate medians.
+        If the number of means goes over this size then the strategy
+        used may be less accurate, but will not use as much memory in
+        minknow
+    selected_classifications:
+        A list of classifications that are deemed interesting, and
+        will be marked to be written out to file
+    open_pore_classifications:
+        A set of classifications whose level should be tracked as the
+        level of open pore (fed back into read detection analysis).
+        Read chunks selected by this filter will be aggregated for use
+        in read detection.
+    open_pore_ewma_weight:
+        A weighting figure for the exponentially weighted moving
+        average given to the newest data. eg. 0.7 would weight new
+        data with 0.3 and all previous data with 0.7.  By default 0.5
+        is used.
+    open_pore_ignore_after_reset_seconds:
+        A number of seconds to ignore new chunks for after a reset
+        occurs on a channel this allows analysis to ignore spikes or
+        bad data on the channel for a small section of time.  By
+        default 0.0 is used - and chunks are accepted immediately.
+    classification_strategy:
+        Determine how to classify a whole read based on the strategy
+        'ultimate':      Chooses the last (ultimate) read chunk's
+        classification 'penultimate':   Chooses the second-to-last
+        read chunk's clasification 'modal':         Chooses the most
+        common classification out of all read chunks 'threshold':
+        Chooses a classification based on the combination of threshold
+        parameters.                  If selected, values for the
+        "selected_classifications_fraction_required"
+        and "selected_chunks_required" fields will be used to
+        determine the                  read classification (see
+        below).
+    selected_classifications_fraction_required:
+        For the "threshold" classification strategy, specify the
+        minimum fraction (in duration) of a completed read that needs
+        to be in any of the "selected_classifications". For example,
+        using 0 means that all reads will written out unless further
+        constrained by the "selected_classifications_chunk_required"
+        field.  Note that this option only applies to the 'threshold'
+        classification strategy and will be ignored for other
+        classification strategies.
+    selected_classifications_chunks_required:
+        For the "threshold" classification strategy, specify the
+        minimum number of chunks of a completed read that needs to be
+        in any of the "selected_classifications". For example, using 1
+        means that the entire read will be written if ANY chunk has a
+        classification in "selected_classifications" unless further
+        constrained by the
+        "selected_classifications_fraction_required" field.  Note that
+        this option only applies to the 'threshold' classification
+        strategy and will be ignored for other classification
+        strategies.
+"""
+ChannelStates.Logic.Ranges.__doc__ = """Dont really like this way of doing it, but it has to match the old
+way..."""
+GetChannelStatesDescResponse.ChannelState.__doc__ = """Attributes:
+    id:
+        The numeric identifier of the state.  This is what is reported
+        in any other APIs that return a channel state ID.
+    name:
+        The internal name of the state.  This is what is reported in
+        any other APIs that return a channel state name.
+    style:
+        How to render the channel state in a graphical user interface.
+        Note that the style may be missing from some channel states
+        (such as the ones that are built in to MinKNOW).
+    global_order:
+        An order ranking for the channel states when they are
+        ungrouped.  This can be used to order the channel states after
+        merging the groups.
+"""
+DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance.__doc__ = """Attributes:
+    well_conductance:
+        Per well conductance values.
+"""
+WriterConfiguration.ReadFast5Configuration.__doc__ = """Attributes:
     compression_level:
         Control the level of compression applied to read data.  0:
         No compression will be applied to data. 1-9: Passed to zlib
         compression, 1 is the fastest      compression, 9 is the
         smallest possible output.
     compression_type:
         Control the type of compression applied to the read data.  By
         default the vbz compressor is used (except in the single read
         case).
-    file_pattern:
-        The pattern used to find a bulk files name. If left empty but
-        output is enabled a default pattern is used.  default:
-        {data_set}.fast5 Where each {xxx} section is replaced with an
-        attribute from the minknow state when the file is written.
-        See file pattern attributes above.
     raw:
-        Raw data, stored with channel calibration data  Stored under
-        /Raw/Channel_*/Signal
-    events:
-        Minknow event data  Stored under
-        /IntermediateData/Channel_*/Events
-    reads:
-        Minknow read data  Stored under
-        /IntermediateData/Channel_*/Reads
-    multiplex:
-        Device multiplex data  Stored under
-        /MultiplexData/Channel_*/Multiplex
-    channel_states:
-        Channel state data  Stored under /StateData/Channel_*/States
-    device_metadata:
-        Device metadata (bias and temperature information)  Stored in
-        a per frame sequence in /Device/MetaData
-    device_commands:
-        Device commands  Stored with the frame commands take effect
-        sequence in /Device/AsicCommands
-    dynamic_analysis_config:
-        Dynamic analysis configuration  Stored with the frame config
-        took effect in /Meta/User/DynamicAnalysisConfiguration
-"""
-DynamicAnalysisConfiguration.ReadScaleTracking.__doc__ = """Attributes:
-    conductance_scan_voltage:
-        Set the voltage the most recent conductance scan occured at.
-    channel_conductance:
-        Per channel/well conductance values
-"""
-PoreTypeConfiguration.ChannelWell.__doc__ = """Attributes:
-    channel:
-        Channel number to control pore type for.  Must be less than
-        channel count for the current platform
-    well:
-        Well to control pore type for.  Wells outside the available
-        wells on the flowcell are ignored.
-"""
-WriterConfiguration.ReadPod5Configuration.__doc__ = """Attributes:
-    enable:
-        Control if a POD5 file should be generated per channel.
+        Raw data, stored with calibration data, and read attributes.
+        Stored under /Raw/Reads_*/Signal
+    fastq:
+        Fastq data, stored as a string.  Stored under
+        /Analyses/Basecall_1D_*/BaseCalled_(template|complement)/Fastq
+    trace_table:
+        Trace table received from Guppy  Stored under
+        /Analyses/Basecall_1D_*/BaseCalled_template/Trace
+    move_table:
+        Move table received from Guppy  Stored under
+        /Analyses/Basecall_1D_*/BaseCalled_template/Move
+    modifications_table:
+        Base modification probability table  Store under
+        /Analyses/Basecall_1D_*/BaseCalled_template/ModBaseProbs
+    disable_writing_passed_reads:
+        Prevent reads which have successfully basecalled being written
+        to fast5.
+    disable_writing_failed_reads:
+        Prevent reads which have failed basecalling being written to
+        fast5.
+    disable_writing_force_skipped_reads:
+        disable writing reads which have been force skipped by the
+        basecaller.
     file_pattern:
-        The pattern used to find a POD5 files name.  default: pod5{bas
-        ecall_status}/{flow_cell_id}_{run_id}_{batch_number}.pod5
+        The pattern used to find a fast5 files name.  default: fast5{b
+        asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fast5
         Where each {xxx} section is replaced with an attribute from
         the minknow state when the file is written.  See file pattern
         attributes above.
+    fastq_header_pattern:
+        The pattern used to find a fastq header.  default: {read_id}
+        runid={run_id} read={read_number} ch={channel_name}
+        start_time={read_start_time} Where each {xxx} section is
+        replaced with an attribute from the minknow state when the
+        fastq is generated.
     batch_count:
         How many reads are placed in each batch (after batch_count
         reads {batch_number} is increased in the pattern).
     bases_per_batch:
         Number of estimated bases within a batch before it rotates to
         a new batch
     no_output_based_batching:
         Do not perform batching based on output (time-based batching
         is still performed, if specified)
-    disable_writing_passed_reads:
-        Prevent reads which have successfully basecalled being written
-        to pod5.
-    disable_writing_failed_reads:
-        Prevent reads which have failed basecalling being written to
-        pod5.
-    disable_writing_force_skipped_reads:
-        disable writing reads which have been force skipped by the
-        basecaller.
     batch_duration:
         The batch duration, for time-based batching  If time-based
         batching is enabled then, in addition to completing batches
         when the `batch_count` or `bases_per_batch` target (above) is
         reached, batches will also be completed when: - At least one
         read has been written to the batch, AND - `batch_duration` has
         elapsed since the last batch was completed (or since the start
         of the acquisition, for the first batch)  If this field is not
         set, then the default time-based batching configuration will
         be used.  If this field is set to zero or a negative value,
         then time-based batching will be disabled.  Since 5.6
 """
-WriterConfiguration.ReadBamConfiguration.__doc__ = """Attributes:
+GetChannelStatesDescResponse.Style.__doc__ = """Attributes:
+    label:
+        The human-readable name to display when rendering this channel
+        state or group.
+    description:
+        A sentence describing the meaning of the channel state or
+        group.  This can be used as a tooltip, for example.
+    colour:
+        The colour to use when rendering this channel state or group.
+        This is a six-digit hex string describing an RGB colour (eg:
+        "ff00ff" for purple).
+"""
+WriterConfiguration.ReadPod5Configuration.__doc__ = """Attributes:
     enable:
-        Control if a BAM file should be generated per channel.
+        Control if a POD5 file should be generated per channel.
     file_pattern:
-        The pattern used to find a BAM files name.  default: bam{basec
-        all_status}/{flow_cell_id}_{run_id}_{batch_number}.bam Where
-        each {xxx} section is replaced with an attribute from the
-        minknow state when the file is written.  See file pattern
+        The pattern used to find a POD5 files name.  default: pod5{bas
+        ecall_status}/{flow_cell_id}_{run_id}_{batch_number}.pod5
+        Where each {xxx} section is replaced with an attribute from
+        the minknow state when the file is written.  See file pattern
         attributes above.
     batch_count:
         How many reads are placed in each batch (after batch_count
         reads {batch_number} is increased in the pattern).
     bases_per_batch:
         Number of estimated bases within a batch before it rotates to
         a new batch
     no_output_based_batching:
         Do not perform batching based on output (time-based batching
         is still performed, if specified)
-    disable_writing_multiple_alignments:
-        If true minknow will only write the primary alignment for each
-        read.
     disable_writing_passed_reads:
-        Since 5.8 Prevent reads which have successfully basecalled
-        being written to bam.
+        Prevent reads which have successfully basecalled being written
+        to pod5.
     disable_writing_failed_reads:
         Prevent reads which have failed basecalling being written to
-        bam.
+        pod5.
     disable_writing_force_skipped_reads:
         disable writing reads which have been force skipped by the
         basecaller.
     batch_duration:
         The batch duration, for time-based batching  If time-based
         batching is enabled then, in addition to completing batches
         when the `batch_count` or `bases_per_batch` target (above) is
@@ -357,166 +541,64 @@
         read has been written to the batch, AND - `batch_duration` has
         elapsed since the last batch was completed (or since the start
         of the acquisition, for the first batch)  If this field is not
         set, then the default time-based batching configuration will
         be used.  If this field is set to zero or a negative value,
         then time-based batching will be disabled.  Since 5.6
 """
-GetChannelStatesDescResponse.ChannelState.__doc__ = """Attributes:
-    id:
-        The numeric identifier of the state.  This is what is reported
-        in any other APIs that return a channel state ID.
+ReadDetectionParams.__doc__ = """Attributes:
+    open_pore_min:
+        The minimum level which is considered open pore (this value is
+        relative to open_pore_default or the tracked open_pore
+        section, if tracking is being used.)  This value must be <=
+        0.0 if tracking is being used.
+    open_pore_max:
+        The maximum level which is considered open pore (this value is
+        relative to open_pore_default or the tracked open_pore
+        section, if tracking is being used.)  This value must be >=
+        0.0 if tracking is being used.
+    open_pore_default:
+        The default value to use for open pore, either when tracking
+        isn't being used, or when open pore tracking has no value
+        currently.
+    open_pore_seconds_required:
+        Minimum number of seconds events must lie within the range of
+        open pore in order to allow a read to break.
+"""
+GetChannelStatesDescResponse.Group.__doc__ = """Attributes:
     name:
-        The internal name of the state.  This is what is reported in
-        any other APIs that return a channel state name.
+        The name of the group.
     style:
-        How to render the channel state in a graphical user interface.
-        Note that the style may be missing from some channel states
-        (such as the ones that are built in to MinKNOW).
-    global_order:
-        An order ranking for the channel states when they are
-        ungrouped.  This can be used to order the channel states after
-        merging the groups.
-"""
-BasecallerConfiguration.ReadFiltering.__doc__ = """Attributes:
-    min_duplex_qscore:
-        Since 5.8
-"""
-ChannelStates.Logic.Ranges.__doc__ = """Dont really like this way of doing it, but it has to match the old
-way..."""
-GetChannelStatesDescResponse.__doc__ = """Attributes:
-    groups:
-        The groups of channel states.  The groups are ordered
-        according to the "order" attribute of the group style in the
-        channel states configuration.
-"""
-WriterConfiguration.__doc__ = """Configuration for the output writers for MinKNOWs analysis pipeline.
-Each writer has its own section in this message, where individual data
-elements can be enabled or disabled.  File pattern attributes
------------------------ Writers have a 'file_pattern' field which
-controls where individual files will be written to. The pattern is
-expanded for each individual read, and then the read placed in the
-required file. The tokens used to expand depend on the file type:
-Read centric files (fastq, (multi-)fast5, protobuf):  -
-read_classification:  The classification applied to the completed read
-(eg. strand).  - batch_number:         The batch number of this read,
-evaluated based on the destination file.  - read_id:
-Unique read id for each read, formatted as a hash.  - read_number:
-The read number (unique per channel, incrementing number assigned to
-each read by MinKNOW).  - channel_name:         The name of the
-channel which produced the read.  - read_start_time:      Read start
-time formatted in rfc3339 format.  - basecall_status:      Basecalling
-output status (derived from WriterDefaults section in analysis
-config).  - pore_type:            Type of pore (as specified by
-#set_pore_type_configuration).  General attributes:  - daq_start_time:
-Data acquisition start time formatted as YYYYMMDD_hhmm.  -
-protocol_start_time:  Time the current protocol was started.  -
-run_id:               Acquisition run id formatted as hash.  -
-short_run_id:         Shortened version of acquisition run id
-formatted as hash.  - protocol_run_id:      Protocol run id formatted
-as hash.  - short_protocol_run_id: Shortened protocol run id formatted
-as hash.  - asic_id:              Integer id assigned to the asic in
-the connected flow cell.  - flow_cell_id:         Flow cell integer as
-read from eeprom.  - machine_id:           Name of the machine
-(hostname or machine identifier depending on the sequencer type).  -
-device_id:            Name of the connected sequencing device (eg.
-MN12345).  - sample_id:            Sample id entered by the user when
-starting a protocol.  - version_string:       Version string of the
-running MinKNOW instance  - protocol_group_id:    Protocol group
-entered by user when starting a protocol.  - protocol_purpose:
-Prupose of protocol (see protocol.set_protocol_purpose())
-
-Attributes:
-    read_fast5:
-        Configuration for the fast5 writer.  If not specified, no
-        multi fast5 outputs are generated.
-    read_fastq:
-        Configuration for the fastq writer.  If not specified, no
-        fastq outputs are generated.
-    read_bam:
-        Configuration for the BAM writer.  If not specified, no BAM
-        outputs are generated.
-    read_pod5:
-        Configuration for the POD5 writer.  If not specified no POD5
-        outputs are generated.
-    sequencing_summary:
-        Configuration for Sequencing Summary file  If not specified,
-        no summary file is generated.
-    bulk:
-        Configuration for the bulk writer.  If not specified, a basic
-        bulk output is generated.
-    report:
-        Configuration for the report writer  If
-        acquisition.StartRequest.generate_report is set for the
-        acquisition period, and empty paths (or no report config) are
-        supplied for reports default paths are used.
-    read_filters:
-        Parameters for filtering reads for writing.  If not present,
-        then no filtering will be applied, so no reads will be
-        excluded.
-"""
-DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance.__doc__ = """Attributes:
-    well_conductance:
-        Per well conductance values.
-"""
-ChannelStates.Group.__doc__ = """ TODO: group styling and description should not be defined here, as
-this allows channel states to declare themselves as being part of the
-same group but specify different styling and descriptions."""
-AnalysisConfiguration.__doc__ = """Attributes:
-    read_scaling:
-        Add read scale tracking to the pipeline. If this message is
-        unspecified, read scaling is not enabled.
+        How to render the group in a graphical user interface.  Note
+        that the style may be missing from some groups (such as the
+        ones that are built in to MinKNOW).
+    states:
+        The channel states contained in the group.  The groups are
+        ordered according to the "order" attribute of the channel
+        state style in the channel states configuration.
 """
-BarcodingConfiguration.__doc__ = """Since 3.5
+LampConfiguration.__doc__ = """Since 4.1
 
 Attributes:
-    barcoding_kits:
-        The barcoding kits in use One entry per kit If no barcoding
-        kits are supplied, barcoding is disabled.
-    trim_barcodes:
-        Whether Guppy should trim barcodes If not specified, this
-        value defaults to false (not triming barcodes) If barcoding is
-        not enabled (e.g., because no barcoding kits are specified),
-        this parameter has no effect.
-    require_barcodes_both_ends:
-        Barcode is only classified if a barcode above `min_score` is
-        present at both ends of the basecalled read.
-    detect_mid_strand_barcodes:
-        Search for barcodes through the entire length of the read.  If
-        a barcode is found in the middle of a read the read is marked
-        as unclassified.
-    min_score:
-        Minimum alignment score to consider a valid barcode.  Maximum
-        value is 100, defaults to 60.
-    min_score_rear:
-        Minimum score to consider a valid barcode (overrides min_score
-        for rear barcodes).  Maximum value is 100, defaults to
-        min_score if not specified.
-    min_score_mid:
-        Minimum score to consider a valid mid barcode (only valid if
-        detect_mid_strand_barcodes is specified).  Maximum value is
-        100, defaults to 60.
-    min_score_mask:
-        The minimum score required for the barcode mask to be
-        detected.  Maximum value is 100, defaults to 40.
-    ignore_unspecified_barcodes:
-        If set, barcodes that aren't in barcode user data list will be
-        ignored  Since 5.6
-"""
-WriterConfiguration.ChannelConfiguration.ChannelList.__doc__ = """Attributes:
-    channels:
-        List of channel names (one based) which should be enabled for
-        writing.
+    lamp_kit:
+        Set the lamp kit being used.
+    min_score_barcodes:
+        Optionally specify a min score to detect a valid lamp barcode.
+    min_score_masks:
+        Optionally set the minimimum valid score for a lamp mask.
+    min_score_targets:
+        Optionally specify a minimum score for lamp targets.
 """
-GetSummaryResponse.__doc__ = """Attributes:
-    analysis_enabled:
-        Whether any analysis is enabled.  If this is false, everything
-        else will be false as well.
-    basecalling_enabled:
-        Whether basecalling is enabled.
+PoreTypeConfiguration.ChannelWell.__doc__ = """Attributes:
+    channel:
+        Channel number to control pore type for.  Must be less than
+        channel count for the current platform
+    well:
+        Well to control pore type for.  Wells outside the available
+        wells on the flowcell are ignored.
 """
 EventDetection.__doc__ = """Attributes:
     window_size:
         The window size that the tstats are calculated from
     threshold:
         The peak detection must be above this threshold at a minimum
         for it to be detected as an event.
@@ -547,14 +629,36 @@
         indicating the command is fully applied). Setting this value
         to > 0 will allow minknow to record the mux change as active
         up to this number of samples _before_ the device recorded the
         change as active. Mux changes are never shifted forwards.  A
         value of 0 will disable shifting of mux changes.  Note: no
         longer used.
 """
+ChannelStates.Logic.__doc__ = """Attributes:
+    rank:
+        Specifies the order in which channel state criteria will be
+        evaluated; the smaller the number, the earlier it will be
+        evaluated. The first criteria to match will be selected
+    pattern:
+        Note that this is a regex based pattern for describing a read
+        classification sequence. For example you can specify:
+        "unavailableunavailable" or:      "(unavailable)(unavailable)"
+        to recognise two consecutive read chunks classified as
+        unavailable.  You can also use "?" at the end of one of the
+        classifications in the sequence to indicate that it may or may
+        not be present at that point. For example:
+        "(pore)(transition)?(event)"  This will match both of the
+        sequences:      pore, transition, event      pore, event  The
+        technical documentation has more information on the range of
+        regex patterns you can apply.
+        https://minknow.git.oxfordnanolabs.local/minknow-
+        core/analysis/channel-states.html
+    ranges:
+        Range is [lower_pa, upper_pa)
+"""
 AlignmentConfiguration.__doc__ = """Since 4.0
 
 Attributes:
     reference_files:
         Provide an index to align reads against once basecalled.  Any
         acceptable reference format to guppy can be passed here:   -
         fasta reference file   - minimap index file
@@ -585,94 +689,14 @@
 Attributes:
     global_pore_type:
         Set all channel/wells to one pore type.
     channel_well_pore_types:
         Set channel/wells to different pore types.  Pore types can be
         created without being used by adding an empty entry.
 """
-ChannelStates.Logic.__doc__ = """Attributes:
-    rank:
-        Specifies the order in which channel state criteria will be
-        evaluated; the smaller the number, the earlier it will be
-        evaluated. The first criteria to match will be selected
-    pattern:
-        Note that this is a regex based pattern for describing a read
-        classification sequence. For example you can specify:
-        "unavailableunavailable" or:      "(unavailable)(unavailable)"
-        to recognise two consecutive read chunks classified as
-        unavailable.  You can also use "?" at the end of one of the
-        classifications in the sequence to indicate that it may or may
-        not be present at that point. For example:
-        "(pore)(transition)?(event)"  This will match both of the
-        sequences:      pore, transition, event      pore, event  The
-        technical documentation has more information on the range of
-        regex patterns you can apply.
-        https://minknow.git.oxfordnanolabs.local/minknow-
-        core/analysis/channel-states.html
-    ranges:
-        Range is [lower_pa, upper_pa)
-"""
-ReadClassificationParams.__doc__ = """Attributes:
-    max_sample_size:
-        This tells minknow the maximum number of means to store in
-        memory before using a different strategy to calculate medians.
-        If the number of means goes over this size then the strategy
-        used may be less accurate, but will not use as much memory in
-        minknow
-    selected_classifications:
-        A list of classifications that are deemed interesting, and
-        will be marked to be written out to file
-    open_pore_classifications:
-        A set of classifications whose level should be tracked as the
-        level of open pore (fed back into read detection analysis).
-        Read chunks selected by this filter will be aggregated for use
-        in read detection.
-    open_pore_ewma_weight:
-        A weighting figure for the exponentially weighted moving
-        average given to the newest data. eg. 0.7 would weight new
-        data with 0.3 and all previous data with 0.7.  By default 0.5
-        is used.
-    open_pore_ignore_after_reset_seconds:
-        A number of seconds to ignore new chunks for after a reset
-        occurs on a channel this allows analysis to ignore spikes or
-        bad data on the channel for a small section of time.  By
-        default 0.0 is used - and chunks are accepted immediately.
-    classification_strategy:
-        Determine how to classify a whole read based on the strategy
-        'ultimate':      Chooses the last (ultimate) read chunk's
-        classification 'penultimate':   Chooses the second-to-last
-        read chunk's clasification 'modal':         Chooses the most
-        common classification out of all read chunks 'threshold':
-        Chooses a classification based on the combination of threshold
-        parameters.                  If selected, values for the
-        "selected_classifications_fraction_required"
-        and "selected_chunks_required" fields will be used to
-        determine the                  read classification (see
-        below).
-    selected_classifications_fraction_required:
-        For the "threshold" classification strategy, specify the
-        minimum fraction (in duration) of a completed read that needs
-        to be in any of the "selected_classifications". For example,
-        using 0 means that all reads will written out unless further
-        constrained by the "selected_classifications_chunk_required"
-        field.  Note that this option only applies to the 'threshold'
-        classification strategy and will be ignored for other
-        classification strategies.
-    selected_classifications_chunks_required:
-        For the "threshold" classification strategy, specify the
-        minimum number of chunks of a completed read that needs to be
-        in any of the "selected_classifications". For example, using 1
-        means that the entire read will be written if ANY chunk has a
-        classification in "selected_classifications" unless further
-        constrained by the
-        "selected_classifications_fraction_required" field.  Note that
-        this option only applies to the 'threshold' classification
-        strategy and will be ignored for other classification
-        strategies.
-"""
 WriterConfiguration.ReadFastqConfiguration.__doc__ = """Attributes:
     enable:
         Control if a fastq file should be generated per channel.
     file_pattern:
         The pattern used to find a fastq files name.  default: fastq{b
         asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fastq
         Where each {xxx} section is replaced with an attribute from
@@ -712,14 +736,144 @@
         read has been written to the batch, AND - `batch_duration` has
         elapsed since the last batch was completed (or since the start
         of the acquisition, for the first batch)  If this field is not
         set, then the default time-based batching configuration will
         be used.  If this field is set to zero or a negative value,
         then time-based batching will be disabled.  Since 5.6
 """
+WriterConfiguration.ChannelConfiguration.ChannelList.__doc__ = """Attributes:
+    channels:
+        List of channel names (one based) which should be enabled for
+        writing.
+"""
+ReadClassificationParams.Parameters.__doc__ = """Attributes:
+    rules_in_execution_order:
+        An execution rule has the following format:  "pore =
+        (median,gt,185)&(median,lt,260)&(median_sd,lt,40)"  "median"
+        and "median_sd" are apart of a small subset of variable values
+        describing a read or read chunk, that are exposed to execution
+        rules. The full list of variable values and their descriptions
+        are documented here:
+        https://minknow.git.oxfordnanolabs.local/minknow-
+        core/analysis/reads.html  "gt" and "lt" describe how data can
+        be compared: gt: greater than lt: less than eq: equal ne: not
+        equal  Constant values like "185" or "260" can also be
+        specified. These can be real numbers also.  Note that
+        variables dont always have to be on the left and const values
+        on the right. The following sub rules are also valid:
+        (200,lt,median_sd) (median_before,gt,median) (5,lt,10)
+"""
+ReadFilters.__doc__ = """Parameters for filtering out reads from being written.  The tests are
+combined using a logical AND: if any given test fails, the read will
+not be written. Only reads that pass all (non-zero) tests will be
+written out.  Currently, it is only possible to filter on read length.
+This can be given in samples or MinKNOW events.
+
+Attributes:
+    read_length_min:
+        Only write reads that contain at least this many samples.  The
+        default zero value will not exclude any reads.
+    read_length_max:
+        Only write reads that contain at most this many samples.  If
+        set to zero (the default), this test is not applied (as though
+        it had been set to a value longer than any possible read).
+    event_count_min:
+        Only write reads that contain at least this many MinKNOW
+        events.  The default zero value will not exclude any reads.
+    event_count_max:
+        Only write reads that contain at most this many MinKNOW
+        events.  If set to zero (the default), this test is not
+        applied (as though it had been set to a value longer than any
+        possible read).
+"""
+WriterConfiguration.__doc__ = """Configuration for the output writers for MinKNOWs analysis pipeline.
+Each writer has its own section in this message, where individual data
+elements can be enabled or disabled.  File pattern attributes
+----------------------- Writers have a 'file_pattern' field which
+controls where individual files will be written to. The pattern is
+expanded for each individual read, and then the read placed in the
+required file. The tokens used to expand depend on the file type:
+Read centric files (fastq, (multi-)fast5, protobuf):  -
+read_classification:  The classification applied to the completed read
+(eg. strand).  - batch_number:         The batch number of this read,
+evaluated based on the destination file.  - read_id:
+Unique read id for each read, formatted as a hash.  - read_number:
+The read number (unique per channel, incrementing number assigned to
+each read by MinKNOW).  - channel_name:         The name of the
+channel which produced the read.  - read_start_time:      Read start
+time formatted in rfc3339 format.  - basecall_status:      Basecalling
+output status (derived from WriterDefaults section in analysis
+config).  - pore_type:            Type of pore (as specified by
+#set_pore_type_configuration).  General attributes:  - daq_start_time:
+Data acquisition start time formatted as YYYYMMDD_hhmm.  -
+protocol_start_time:  Time the current protocol was started.  -
+run_id:               Acquisition run id formatted as hash.  -
+short_run_id:         Shortened version of acquisition run id
+formatted as hash.  - protocol_run_id:      Protocol run id formatted
+as hash.  - short_protocol_run_id: Shortened protocol run id formatted
+as hash.  - asic_id:              Integer id assigned to the asic in
+the connected flow cell.  - flow_cell_id:         Flow cell integer as
+read from eeprom.  - machine_id:           Name of the machine
+(hostname or machine identifier depending on the sequencer type).  -
+device_id:            Name of the connected sequencing device (eg.
+MN12345).  - sample_id:            Sample id entered by the user when
+starting a protocol.  - version_string:       Version string of the
+running MinKNOW instance  - protocol_group_id:    Protocol group
+entered by user when starting a protocol.  - protocol_purpose:
+Prupose of protocol (see protocol.set_protocol_purpose())
+
+Attributes:
+    read_fast5:
+        Configuration for the fast5 writer.  If not specified, no
+        multi fast5 outputs are generated.
+    read_fastq:
+        Configuration for the fastq writer.  If not specified, no
+        fastq outputs are generated.
+    read_bam:
+        Configuration for the BAM writer.  If not specified, no BAM
+        outputs are generated.
+    read_pod5:
+        Configuration for the POD5 writer.  If not specified no POD5
+        outputs are generated.
+    sequencing_summary:
+        Configuration for Sequencing Summary file  If not specified,
+        no summary file is generated.
+    bulk:
+        Configuration for the bulk writer.  If not specified, a basic
+        bulk output is generated.
+    report:
+        Configuration for the report writer  If
+        acquisition.StartRequest.generate_report is set for the
+        acquisition period, and empty paths (or no report config) are
+        supplied for reports default paths are used.
+    read_filters:
+        Parameters for filtering reads for writing.  If not present,
+        then no filtering will be applied, so no reads will be
+        excluded.
+"""
+GetSummaryResponse.__doc__ = """Attributes:
+    analysis_enabled:
+        Whether any analysis is enabled.  If this is false, everything
+        else will be false as well.
+    basecalling_enabled:
+        Whether basecalling is enabled.
+"""
+BasecallerConfiguration.ReadFiltering.__doc__ = """Attributes:
+    min_duplex_qscore:
+        Since 5.8
+"""
+ChannelStates.Group.__doc__ = """ TODO: group styling and description should not be defined here, as
+this allows channel states to declare themselves as being part of the
+same group but specify different styling and descriptions."""
+GetChannelStatesDescResponse.__doc__ = """Attributes:
+    groups:
+        The groups of channel states.  The groups are ordered
+        according to the "order" attribute of the group style in the
+        channel states configuration.
+"""
 BasecallerConfiguration.__doc__ = """Since 3.0
 
 Attributes:
     enable:
         Choose if guppy is enabled or disabled.  If set to false then
         no basecalling will take place, and the rest of the config is
         ignored.
@@ -768,75 +922,71 @@
         deciding when read splitting should be enabled.
     min_score_read_splitting:
         Override score to use for guppy read splitting. If not
         specified a default value is used from guppy.  Since 4.5
         Note: Since 5.9 this option has no effect, the basecaller is
         responsible for deciding read splitting score.
 """
-GetChannelStatesDescResponse.Group.__doc__ = """Attributes:
-    name:
-        The name of the group.
-    style:
-        How to render the group in a graphical user interface.  Note
-        that the style may be missing from some groups (such as the
-        ones that are built in to MinKNOW).
-    states:
-        The channel states contained in the group.  The groups are
-        ordered according to the "order" attribute of the channel
-        state style in the channel states configuration.
+WriterConfiguration.ChannelConfiguration.ChannelRanges.__doc__ = """Attributes:
+    ranges:
+        List of start/end paired channel numbers which should be
+        enabled for writing.  All channels in inclusive ranges should
+        be enabled.
 """
-BasecallerConfiguration.TargetFiltering.__doc__ = """Since 3.7"""
-ReadScalingParams.__doc__ = """Since 5.3  Quantile Information:
+WriterConfiguration.SequencingSummaryConfiguration.__doc__ = """Attributes:
+    enable:
+        Should a sequencing summary file be generated
+    file_pattern:
+        The pattern used to find a summary files name.  default:
+        sequencing_summary_{flow_cell_id}_{short_run_id}.txt Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+"""
+WriterConfiguration.BulkConfiguration.__doc__ = """Control settings for the bulk writer
 
 Attributes:
-    quantile_locations:
-        Position of quantiles in scaling data to use when computing
-        scale parameters.
-    quantile_weights_shift:
-        If present, must be the same length as quantile_locations.
-        Represents the coefficients that shall be multiplied with
-        measured quantiles to give a predicted_shift
-    quantile_weights_scale:
-        If present, must be the same length as quantile_locations.
-        Represents the coefficients that shall be multiplied with
-        measured quantiles to give a predicted_scale
-    tracking_alpha:
-        Alpha value to use in ewma calculation for scale and shift
-        tracking. 1 updates instantly. 0 does not update.
-    alpha_number_estimates_decay:
-        Alpha decay value to use. Higher values cause a more rapid
-        decay in greater trust of earlier numbers.
-    quantile_maxdiff:
-        Maximum difference in event quantiles which will be added into
-        trackers.  This is used to filter away cases where pore signal
-        is included in the read and thus cannot be trusted.
-    trust_limit_fraction:
-        Maximum fraction change between one tracked value and the next
-        which will be trusted. Higher values are not trusted.
-    diff_threshold:
-        The minimum difference between an event and the next to
-        include it in the subsampling
-    emission_threshold:
-        After how many cumulative pA is a new event emitted in the
-        subsampling
-    dacs_breakpoint:
-        Cumulative pA sum required to compute scaling. Any events
-        after this sum are not considered in scaling.
-    conductance_factor_scale:
-        Scale factor applied to conductance to produce a basic scale
-        estimate, also combined with q90_q10_to_normal.
-    conductance_factor_shift:
-        Scale factor applied to conductance to produce a basic shift
-        estimate.
-"""
-PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.__doc__ = """Attributes:
-    pore_types:
-        Map with pore type as key, mapped to the list of wells to set
-        for.  It is undefined what will happen if one call sets the
-        pore type of a channel and well to two pore types.
+    compression_level:
+        Control the level of compression applied to read data.  0:
+        No compression will be applied to data. 1-9: Passed to zlib
+        compression, 1 is the fastest      compression, 9 is the
+        smallest possible output.
+    compression_type:
+        Control the type of compression applied to the read data.  By
+        default the vbz compressor is used (except in the single read
+        case).
+    file_pattern:
+        The pattern used to find a bulk files name. If left empty but
+        output is enabled a default pattern is used.  default:
+        {data_set}.fast5 Where each {xxx} section is replaced with an
+        attribute from the minknow state when the file is written.
+        See file pattern attributes above.
+    raw:
+        Raw data, stored with channel calibration data  Stored under
+        /Raw/Channel_*/Signal
+    events:
+        Minknow event data  Stored under
+        /IntermediateData/Channel_*/Events
+    reads:
+        Minknow read data  Stored under
+        /IntermediateData/Channel_*/Reads
+    multiplex:
+        Device multiplex data  Stored under
+        /MultiplexData/Channel_*/Multiplex
+    channel_states:
+        Channel state data  Stored under /StateData/Channel_*/States
+    device_metadata:
+        Device metadata (bias and temperature information)  Stored in
+        a per frame sequence in /Device/MetaData
+    device_commands:
+        Device commands  Stored with the frame commands take effect
+        sequence in /Device/AsicCommands
+    dynamic_analysis_config:
+        Dynamic analysis configuration  Stored with the frame config
+        took effect in /Meta/User/DynamicAnalysisConfiguration
 """
 WriterConfiguration.ReportConfiguration.__doc__ = """Control settings for the report writer
 
 Attributes:
     pdf_report_file_pattern:
         DEPRECATED 6.0: As of 5.1 a pdf report is not generated at
         all. This field will be removed in 6.0  The pattern used to
@@ -906,206 +1056,56 @@
         The pattern used to suffix custom reports.  default:
         "_{flow_cell_id}_{short_run_id}" Where each {xxx} section is
         replaced with an attribute from the minknow state when the
         file is written.  Custom reports use this to build filenames:
         - "custom_report{suffix}.txt"  See file pattern attributes
         above.
 """
-ReadFilters.__doc__ = """Parameters for filtering out reads from being written.  The tests are
-combined using a logical AND: if any given test fails, the read will
-not be written. Only reads that pass all (non-zero) tests will be
-written out.  Currently, it is only possible to filter on read length.
-This can be given in samples or MinKNOW events.
-
-Attributes:
-    read_length_min:
-        Only write reads that contain at least this many samples.  The
-        default zero value will not exclude any reads.
-    read_length_max:
-        Only write reads that contain at most this many samples.  If
-        set to zero (the default), this test is not applied (as though
-        it had been set to a value longer than any possible read).
-    event_count_min:
-        Only write reads that contain at least this many MinKNOW
-        events.  The default zero value will not exclude any reads.
-    event_count_max:
-        Only write reads that contain at most this many MinKNOW
-        events.  If set to zero (the default), this test is not
-        applied (as though it had been set to a value longer than any
-        possible read).
-"""
-WriterConfiguration.SequencingSummaryConfiguration.__doc__ = """Attributes:
-    enable:
-        Should a sequencing summary file be generated
-    file_pattern:
-        The pattern used to find a summary files name.  default:
-        sequencing_summary_{flow_cell_id}_{short_run_id}.txt Where
-        each {xxx} section is replaced with an attribute from the
-        minknow state when the file is written.  See file pattern
-        attributes above.
-"""
-ReadClassificationParams.Parameters.__doc__ = """Attributes:
-    rules_in_execution_order:
-        An execution rule has the following format:  "pore =
-        (median,gt,185)&(median,lt,260)&(median_sd,lt,40)"  "median"
-        and "median_sd" are apart of a small subset of variable values
-        describing a read or read chunk, that are exposed to execution
-        rules. The full list of variable values and their descriptions
-        are documented here:
-        https://minknow.git.oxfordnanolabs.local/minknow-
-        core/analysis/reads.html  "gt" and "lt" describe how data can
-        be compared: gt: greater than lt: less than eq: equal ne: not
-        equal  Constant values like "185" or "260" can also be
-        specified. These can be real numbers also.  Note that
-        variables dont always have to be on the left and const values
-        on the right. The following sub rules are also valid:
-        (200,lt,median_sd) (median_before,gt,median) (5,lt,10)
+AnalysisConfiguration.__doc__ = """Attributes:
+    read_scaling:
+        Add read scale tracking to the pipeline. If this message is
+        unspecified, read scaling is not enabled.
 """
-LampConfiguration.__doc__ = """Since 4.1
+ReadScalingParams.__doc__ = """Since 5.3  Quantile Information:
 
 Attributes:
-    lamp_kit:
-        Set the lamp kit being used.
-    min_score_barcodes:
-        Optionally specify a min score to detect a valid lamp barcode.
-    min_score_masks:
-        Optionally set the minimimum valid score for a lamp mask.
-    min_score_targets:
-        Optionally specify a minimum score for lamp targets.
-"""
-ReadDetectionParams.__doc__ = """Attributes:
-    open_pore_min:
-        The minimum level which is considered open pore (this value is
-        relative to open_pore_default or the tracked open_pore
-        section, if tracking is being used.)  This value must be <=
-        0.0 if tracking is being used.
-    open_pore_max:
-        The maximum level which is considered open pore (this value is
-        relative to open_pore_default or the tracked open_pore
-        section, if tracking is being used.)  This value must be >=
-        0.0 if tracking is being used.
-    open_pore_default:
-        The default value to use for open pore, either when tracking
-        isn't being used, or when open pore tracking has no value
-        currently.
-    open_pore_seconds_required:
-        Minimum number of seconds events must lie within the range of
-        open pore in order to allow a read to break.
-"""
-GetChannelStatesDescResponse.Style.__doc__ = """Attributes:
-    label:
-        The human-readable name to display when rendering this channel
-        state or group.
-    description:
-        A sentence describing the meaning of the channel state or
-        group.  This can be used as a tooltip, for example.
-    colour:
-        The colour to use when rendering this channel state or group.
-        This is a six-digit hex string describing an RGB colour (eg:
-        "ff00ff" for purple).
-"""
-WriterConfiguration.ReadFast5Configuration.__doc__ = """Attributes:
-    compression_level:
-        Control the level of compression applied to read data.  0:
-        No compression will be applied to data. 1-9: Passed to zlib
-        compression, 1 is the fastest      compression, 9 is the
-        smallest possible output.
-    compression_type:
-        Control the type of compression applied to the read data.  By
-        default the vbz compressor is used (except in the single read
-        case).
-    raw:
-        Raw data, stored with calibration data, and read attributes.
-        Stored under /Raw/Reads_*/Signal
-    fastq:
-        Fastq data, stored as a string.  Stored under
-        /Analyses/Basecall_1D_*/BaseCalled_(template|complement)/Fastq
-    trace_table:
-        Trace table received from Guppy  Stored under
-        /Analyses/Basecall_1D_*/BaseCalled_template/Trace
-    move_table:
-        Move table received from Guppy  Stored under
-        /Analyses/Basecall_1D_*/BaseCalled_template/Move
-    modifications_table:
-        Base modification probability table  Store under
-        /Analyses/Basecall_1D_*/BaseCalled_template/ModBaseProbs
-    disable_writing_passed_reads:
-        Prevent reads which have successfully basecalled being written
-        to fast5.
-    disable_writing_failed_reads:
-        Prevent reads which have failed basecalling being written to
-        fast5.
-    disable_writing_force_skipped_reads:
-        disable writing reads which have been force skipped by the
-        basecaller.
-    file_pattern:
-        The pattern used to find a fast5 files name.  default: fast5{b
-        asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fast5
-        Where each {xxx} section is replaced with an attribute from
-        the minknow state when the file is written.  See file pattern
-        attributes above.
-    fastq_header_pattern:
-        The pattern used to find a fastq header.  default: {read_id}
-        runid={run_id} read={read_number} ch={channel_name}
-        start_time={read_start_time} Where each {xxx} section is
-        replaced with an attribute from the minknow state when the
-        fastq is generated.
-    batch_count:
-        How many reads are placed in each batch (after batch_count
-        reads {batch_number} is increased in the pattern).
-    bases_per_batch:
-        Number of estimated bases within a batch before it rotates to
-        a new batch
-    no_output_based_batching:
-        Do not perform batching based on output (time-based batching
-        is still performed, if specified)
-    batch_duration:
-        The batch duration, for time-based batching  If time-based
-        batching is enabled then, in addition to completing batches
-        when the `batch_count` or `bases_per_batch` target (above) is
-        reached, batches will also be completed when: - At least one
-        read has been written to the batch, AND - `batch_duration` has
-        elapsed since the last batch was completed (or since the start
-        of the acquisition, for the first batch)  If this field is not
-        set, then the default time-based batching configuration will
-        be used.  If this field is set to zero or a negative value,
-        then time-based batching will be disabled.  Since 5.6
-"""
-ChannelStates.Logic.Behaviour.__doc__ = """Attributes:
-    reset_on_mux_change:
-        TODO: MinKNOW 5: replace int32 with bool for these options
-        these are ints but act like bools
-    latch:
-        If the latch value is set to true, then when the criteria for
-        this channel state is active, then the latch will keep it
-        active until the channel state is reset.
-    reset_on_effective_mux_change:
-        An 'effective mux change' is any mux change apart from the one
-        triggered with the purpose of disconnecting a channel (turning
-        a channel off). For example, if a channel is in pore, and the
-        user changes the channel configuration to 'disconnected', that
-        mux change will not be an effective mux change. Any other mux
-        change is considered an 'effective mux change'. So if a
-        channel saturates, the mux change to disconnected is an
-        effective mux change. Similarly, a change from disconnected to
-        a pore is an effective mux change.  Use this reset mode to
-        make the channel state persist on non-effective mux changes.
-        For example, if a channel state is in 'multiple' and the user
-        triggers a channel configuration change to 'disconnected', the
-        state will remain in multiple if it has this option on. The
-        multiple state will be reset at all other mux changes (i.e.
-        effective mux changes).
-    reset_on_effective_well_change:
-        An 'effective well change' is any well change apart from the
-        one triggered with the purpose of disconnecting a channel
-        (turning a channel off). For example, if a channel is in
-        well_1, and the user changes the channel configuration to
-        'unblock_1', that change will not be an effective well change.
-        A change to disconnected is also not considered an effective
-        well change.  Use this reset mode to make the channel state
-        persist on non-effective well changes. For example, if a
-        channel state is in 'multiple' and the user triggers a channel
-        configuration change to 'disconnected', the state will remain
-        in multiple if it has this option on. The multiple state will
-        be reset then when the mux is set to a different setting.
+    quantile_locations:
+        Position of quantiles in scaling data to use when computing
+        scale parameters.
+    quantile_weights_shift:
+        If present, must be the same length as quantile_locations.
+        Represents the coefficients that shall be multiplied with
+        measured quantiles to give a predicted_shift
+    quantile_weights_scale:
+        If present, must be the same length as quantile_locations.
+        Represents the coefficients that shall be multiplied with
+        measured quantiles to give a predicted_scale
+    tracking_alpha:
+        Alpha value to use in ewma calculation for scale and shift
+        tracking. 1 updates instantly. 0 does not update.
+    alpha_number_estimates_decay:
+        Alpha decay value to use. Higher values cause a more rapid
+        decay in greater trust of earlier numbers.
+    quantile_maxdiff:
+        Maximum difference in event quantiles which will be added into
+        trackers.  This is used to filter away cases where pore signal
+        is included in the read and thus cannot be trusted.
+    trust_limit_fraction:
+        Maximum fraction change between one tracked value and the next
+        which will be trusted. Higher values are not trusted.
+    diff_threshold:
+        The minimum difference between an event and the next to
+        include it in the subsampling
+    emission_threshold:
+        After how many cumulative pA is a new event emitted in the
+        subsampling
+    dacs_breakpoint:
+        Cumulative pA sum required to compute scaling. Any events
+        after this sum are not considered in scaling.
+    conductance_factor_scale:
+        Scale factor applied to conductance to produce a basic scale
+        estimate, also combined with q90_q10_to_normal.
+    conductance_factor_shift:
+        Scale factor applied to conductance to produce a basic shift
+        estimate.
 """
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/analysis_configuration_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/analysis_configuration_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/analysis_configuration_service.py` & `minknow_api-5.9.5/minknow_api/analysis_configuration_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/basecaller_pb2.py` & `minknow_api-5.9.5/minknow_api/basecaller_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -127,90 +127,32 @@
   _globals['_UPDATEPROGRESSRESPONSE']._serialized_end=4705
   _globals['_SENDPINGREQUEST']._serialized_start=4707
   _globals['_SENDPINGREQUEST']._serialized_end=4749
   _globals['_SENDPINGRESPONSE']._serialized_start=4751
   _globals['_SENDPINGRESPONSE']._serialized_end=4769
   _globals['_BASECALLER']._serialized_start=5000
   _globals['_BASECALLER']._serialized_end=6765
-RunInfo.__doc__ = """Attributes:
+CancelRequest.__doc__ = """Attributes:
     id:
-        The ID of the run, as returned by start().
-    start_request_oneof:
-        The original message used to start the run.
-    start_basecalling_request:
-        Set if basecalling reads
-    start_barcoding_request:
-        Set if barcoding reads
-    start_alignment_request:
-        Set if aligning reads
-    start_post_processing_protocol_request:
-        Set if aligning reads
-    state:
-        What state the run is in.  While the basecalling is running
-        the state field will be ``STATE_RUNNING``.
-    errors:
-        If state is STATE_ERROR, this will contain (some of) the
-        errors encountered.  Note that if there are a lot of errors,
-        only some may be returned.
-    files_discovered:
-        The number of files selected for input.
-    progress_current:
-        The current basecalling progress (with respect to
-        progress_total).  This is intended to be an estimate of how
-        close to completion the basecalling run is. The numbers have
-        no particular meaning other than as a proportion of
-        progress_total.  Note that this only really has useful meaning
-        while state is STATE_RUNNING. On STATE_SUCCESS, it will always
-        be the same as progress_total. On STATE_ERROR or
-        STATE_CANCELLED, it may give some indication of how far
-        through basecalling was when it failed or was cancelled.
-    progress_total:
-        The maximum value of progress_current.  (progress_current /
-        progress_total) * 100 will give a percentage completion.  If
-        this is 0, it should be interpreted as "unknown progress".
-    start_time:
-        When basecalling was started (UTC).
-    end_time:
-        When basecalling ended (UTC).  Unset if basecalling is still
-        running.
-    estimated_end_time:
-        An estimate for when basecalling will end (UTC).  Unset if
-        basecalling has finished, or if an estimate cannot be
-        calculated (eg: because the baescalling software does not
-        support it).  Since 3.6.
+        An identifier as returned from a call to start() or list().
 """
-StartAlignmentRequest.__doc__ = """Attributes:
-    name:
-        User specified name to identify the alignment run.
-    input_reads_directories:
-        Input directories to search for reads to be aligned.
-        Currently, only one directory can be specified, but this
-        definition allows for multiple in the future without breaking
-        compatibility.
-    output_reads_directory:
-        Output directory where aligned reads will be placed.
-    recursive:
-        Recursively find fast5 files to align in the
-        `input_reads_directories`.  If False, only the fast5 files
-        directly in one of the `input_reads_directories` will be
-        aligned. If True, subdirectories of those directories will
-        also be searched recursively.
-    alignment_configuration:
-        Options to control alignment performed once basecalling reads
-        is complete.
+SendPingResponse.__doc__ = """Since 5.0"""
+ListConfigsByKitResponse.PerFlowCell.__doc__ = """Attributes:
+    kit_configs:
+        Key: kit name (eg: "SQK-LSK109") Value: list of configuration
+        names
 """
-ListSettingsForPostProcessingProtocolRequest.__doc__ = """Attributes:
-    identifier:
-        specify the protocol with a string containing all the
-        protocol's identifying components, eg:
-        "SYSTEM:post_processing/artic"
+StartBarcodingResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the basecalling run that was started. This
+        can be used to monitor or cancel the run.
 """
-StartPostProcessingProtocolResponse.__doc__ = """Attributes:
+StartAlignmentResponse.__doc__ = """Attributes:
     id:
-        An identifier for the protocol run that was started. This can
+        An identifier for the alignment run that was started. This can
         be used to monitor or cancel the run.
 """
 StartPostProcessingProtocolRequest.__doc__ = """Attributes:
     identifier:
         identifier value from a protocol returned from
         list_post_processing_protocols.
     sequencing_protocol_run_id:
@@ -224,29 +166,77 @@
     output_directory:
         Output directory where the analysed output should be written.
     setting_values:
         Configured values for display settings for the protocol (see
         basecaller.list_settings_for_protocol) keys missing from the
         original protocol will cause errors.
 """
-ListSettingsForPostProcessingProtocolResponse.__doc__ = """Attributes:
-    requires_fast5_input:
-        Does the protocol require fast5 files as input
-    requires_fastq_input:
-        Does the protocol require fastq files as input
-    requires_bam_input:
-        Does the protocol require bam files as input
-    protocol_settings:
-        List of protocol settings used by the post processing protocol
+GetInfoResponse.__doc__ = """Attributes:
+    runs:
+        Information about the requested runs.
+"""
+StartAlignmentRequest.__doc__ = """Attributes:
+    name:
+        User specified name to identify the alignment run.
+    input_reads_directories:
+        Input directories to search for reads to be aligned.
+        Currently, only one directory can be specified, but this
+        definition allows for multiple in the future without breaking
+        compatibility.
+    output_reads_directory:
+        Output directory where aligned reads will be placed.
+    recursive:
+        Recursively find fast5 files to align in the
+        `input_reads_directories`.  If False, only the fast5 files
+        directly in one of the `input_reads_directories` will be
+        aligned. If True, subdirectories of those directories will
+        also be searched recursively.
+    alignment_configuration:
+        Options to control alignment performed once basecalling reads
+        is complete.
+"""
+ListConfigsByKitResponse.__doc__ = """Attributes:
+    flow_cell_configs:
+        Key: flow cell type (eg: "FLO-MIN107") Value: FlowCellConfigs
+        describing configurations available for that flow cell.
 """
 ListConfigsByKitResponse.ConfigList.__doc__ = """Attributes:
     configs:
         List of configuration names, to be used in
         ``StartBasecallingRequest.configuration``
 """
+WatchRequest.__doc__ = """Attributes:
+    send_finished_runs:
+        By default, no information will be sent about runs that were
+        already finished when this call was made. Setting this to true
+        will cause the state of already-finished runs to be returned.
+    names:
+        The names of the values you wish to watch.
+    allow_missing:
+        Whether to allow missing values.  If set, names that are not
+        present in the store will be omitted from the first response,
+        but will still be watched. If and when they are added, a
+        message will be sent with the set values. Otherwise, missing
+        values will cause an immediate error.  Defaults to 'false'
+"""
+WatchResponse.__doc__ = """Attributes:
+    runs:
+        The current state of some of the runs.
+    values:
+        The values that have changed.  The first received message will
+        contain the current state of all the watched values.
+        Subsequent messages will only contain the values that changed.
+    removed_values:
+        The values that have been removed.
+"""
+StartPostProcessingProtocolResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the protocol run that was started. This can
+        be used to monitor or cancel the run.
+"""
 StartRequest.__doc__ = """ Protobuf messages for input/output of RPC calls
 
 Attributes:
     dont_wait_for_device_ready:
         Prevent waiting until the device is ready before starting
         acquisition.  Defaults to false.  By default, MinKNOW will
         block in the start() call for the device and flow cell to be
@@ -312,20 +302,35 @@
         writing a final_summary.txt file if the purpose is set to
         SEQUENCING.  Since 3.5 (NB: in 3.3 and 3.4, final_summary.txt
         was always written out if file_output was enabled).
     start_request:
         Start request that will be used to trigger analysis, used to
         union over all the different types of analysis possible.
 """
-MakeAlignmentIndexRequest.__doc__ = """Attributes:
-    input_alignment_reference:
-        Input fasta reference to use for building the index.
-    output_alignment_index:
-        Output file path to write index (mmi file) to.  Must have a
-        ".mmi" extension, and the paths parent directory must exist.
+ListSettingsForPostProcessingProtocolResponse.__doc__ = """Attributes:
+    requires_fast5_input:
+        Does the protocol require fast5 files as input
+    requires_fastq_input:
+        Does the protocol require fastq files as input
+    requires_bam_input:
+        Does the protocol require bam files as input
+    protocol_settings:
+        List of protocol settings used by the post processing protocol
+"""
+StartBasecallingResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the basecalling run that was started. This
+        can be used to monitor or cancel the run.
+"""
+UpdateProgressRequest.__doc__ = """Attributes:
+    id:
+        id of the protocol to update (stored in environment variable
+        for python process)
+    progress:
+        Progress indicator, 0-1.
 """
 StartBarcodingRequest.__doc__ = """Attributes:
     name:
         User specified name to identify the barcoding run.
     input_reads_directories:
         Input directories to search for reads to be basecalled.
         Currently, only one directory can be specified, but this
@@ -343,33 +348,20 @@
         directly in one of the `input_reads_directories` will be
         basecalled. If True, subdirectories of those directories will
         also be searched recursively.
     barcoding_configuration:
         Options to control barcoding performed once basecalling reads
         is complete.
 """
-WatchResponse.__doc__ = """Attributes:
-    runs:
-        The current state of some of the runs.
-    values:
-        The values that have changed.  The first received message will
-        contain the current state of all the watched values.
-        Subsequent messages will only contain the values that changed.
-    removed_values:
-        The values that have been removed.
-"""
-StartBasecallingResponse.__doc__ = """Attributes:
-    id:
-        An identifier for the basecalling run that was started. This
-        can be used to monitor or cancel the run.
-"""
-ListConfigsByKitResponse.__doc__ = """Attributes:
-    flow_cell_configs:
-        Key: flow cell type (eg: "FLO-MIN107") Value: FlowCellConfigs
-        describing configurations available for that flow cell.
+MakeAlignmentIndexRequest.__doc__ = """Attributes:
+    input_alignment_reference:
+        Input fasta reference to use for building the index.
+    output_alignment_index:
+        Output file path to write index (mmi file) to.  Must have a
+        ".mmi" extension, and the paths parent directory must exist.
 """
 PostProcessingProtocolInfo.__doc__ = """Attributes:
     identifier:
         System identifier for the protocol
     name:
         Readable name for the protocol (appropriate for use as a key
         in translation database).  Note that this may not be unique:
@@ -379,54 +371,83 @@
         Protocol version.  This might not be set for all protocols or
         all providers.
     description:
         A description of the protocol.
     provider:
         The source of the post-processing protocol.
 """
-GetInfoResponse.__doc__ = """Attributes:
-    runs:
-        Information about the requested runs.
-"""
-SendPingResponse.__doc__ = """Since 5.0"""
-WatchRequest.__doc__ = """Attributes:
-    send_finished_runs:
-        By default, no information will be sent about runs that were
-        already finished when this call was made. Setting this to true
-        will cause the state of already-finished runs to be returned.
-    names:
-        The names of the values you wish to watch.
-    allow_missing:
-        Whether to allow missing values.  If set, names that are not
-        present in the store will be omitted from the first response,
-        but will still be watched. If and when they are added, a
-        message will be sent with the set values. Otherwise, missing
-        values will cause an immediate error.  Defaults to 'false'
+RunInfo.__doc__ = """Attributes:
+    id:
+        The ID of the run, as returned by start().
+    start_request_oneof:
+        The original message used to start the run.
+    start_basecalling_request:
+        Set if basecalling reads
+    start_barcoding_request:
+        Set if barcoding reads
+    start_alignment_request:
+        Set if aligning reads
+    start_post_processing_protocol_request:
+        Set if aligning reads
+    state:
+        What state the run is in.  While the basecalling is running
+        the state field will be ``STATE_RUNNING``.
+    errors:
+        If state is STATE_ERROR, this will contain (some of) the
+        errors encountered.  Note that if there are a lot of errors,
+        only some may be returned.
+    files_discovered:
+        The number of files selected for input.
+    progress_current:
+        The current basecalling progress (with respect to
+        progress_total).  This is intended to be an estimate of how
+        close to completion the basecalling run is. The numbers have
+        no particular meaning other than as a proportion of
+        progress_total.  Note that this only really has useful meaning
+        while state is STATE_RUNNING. On STATE_SUCCESS, it will always
+        be the same as progress_total. On STATE_ERROR or
+        STATE_CANCELLED, it may give some indication of how far
+        through basecalling was when it failed or was cancelled.
+    progress_total:
+        The maximum value of progress_current.  (progress_current /
+        progress_total) * 100 will give a percentage completion.  If
+        this is 0, it should be interpreted as "unknown progress".
+    start_time:
+        When basecalling was started (UTC).
+    end_time:
+        When basecalling ended (UTC).  Unset if basecalling is still
+        running.
+    estimated_end_time:
+        An estimate for when basecalling will end (UTC).  Unset if
+        basecalling has finished, or if an estimate cannot be
+        calculated (eg: because the baescalling software does not
+        support it).  Since 3.6.
 """
 SendPingRequest.__doc__ = """Since 5.0
 
 Attributes:
     ping_data:
         The json data to send as a ping.  note: if this string is not
         a valid json object, an error will be raised.
     days_until_expiry:
         Should the ping fail to send, the number of days the ping will
         be stored before being cleaned up.
 """
-ListConfigsByKitResponse.PerFlowCell.__doc__ = """Attributes:
-    kit_configs:
-        Key: kit name (eg: "SQK-LSK109") Value: list of configuration
-        names
-"""
-UpdateProgressRequest.__doc__ = """Attributes:
+GetInfoRequest.__doc__ = """Attributes:
+    selection:
+        The selection of runs to return information about.  If no
+        selection is provided, the call will return all currently-
+        running basecall runs (as though PRESET_ALL_RUNNING were
+        selected).
+    preset:
+        A pre-determined selection of runs.
     id:
-        id of the protocol to update (stored in environment variable
-        for python process)
-    progress:
-        Progress indicator, 0-1.
+        An identifier, as returned by start().
+    list:
+        A list of identifiers, as returned by start().
 """
 StartBasecallingRequest.__doc__ = """Attributes:
     name:
         User specified name to identify the basecall run.
     input_reads_directories:
         Input directories to search for reads to be basecalled.
         Currently, only one directory can be specified, but this
@@ -471,35 +492,14 @@
         read splitting should be enabled.
     min_score_read_splitting:
         Override score to use for guppy read splitting. If not
         specified a default value is used from guppy.  Note: Since 5.9
         this option has no effect, the basecaller is responsible for
         deciding when read splitting should be enabled.
 """
-StartBarcodingResponse.__doc__ = """Attributes:
-    id:
-        An identifier for the basecalling run that was started. This
-        can be used to monitor or cancel the run.
-"""
-StartAlignmentResponse.__doc__ = """Attributes:
-    id:
-        An identifier for the alignment run that was started. This can
-        be used to monitor or cancel the run.
-"""
-CancelRequest.__doc__ = """Attributes:
-    id:
-        An identifier as returned from a call to start() or list().
-"""
-GetInfoRequest.__doc__ = """Attributes:
-    selection:
-        The selection of runs to return information about.  If no
-        selection is provided, the call will return all currently-
-        running basecall runs (as though PRESET_ALL_RUNNING were
-        selected).
-    preset:
-        A pre-determined selection of runs.
-    id:
-        An identifier, as returned by start().
-    list:
-        A list of identifiers, as returned by start().
+ListSettingsForPostProcessingProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        specify the protocol with a string containing all the
+        protocol's identifying components, eg:
+        "SYSTEM:post_processing/artic"
 """
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/basecaller_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/basecaller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/basecaller_service.py` & `minknow_api-5.9.5/minknow_api/basecaller_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/ca.crt` & `minknow_api-5.9.5/minknow_api/ca.crt`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/data.py` & `minknow_api-5.9.5/minknow_api/data.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/data_pb2.py` & `minknow_api-5.9.5/minknow_api/data_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -173,33 +173,142 @@
   _globals['_GETEXPERIMENTYIELDINFORESPONSE_PROTOBUFREADWRITINGSTATISTICS']._serialized_end=9147
   _globals['_GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS']._serialized_start=9150
   _globals['_GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS']._serialized_end=9698
   _globals['_GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS_FILETYPEINFO']._serialized_start=9587
   _globals['_GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS_FILETYPEINFO']._serialized_end=9698
   _globals['_DATASERVICE']._serialized_start=9701
   _globals['_DATASERVICE']._serialized_end=10864
-GetReadStatisticsResponse.PerChannelData.__doc__ = """Attributes:
-    configurations:
-        Data for each channel configuration seen on this channel.
-        Note that each channel configuration will only appear once in
-        this list, and this list is *not* in any way ordered by time.
-        The only reason it is not a map is because of restrictions on
-        map key types.
-    samples_since_start:
-        The number of samples collected before this channel's first
-        sample.
-    seconds_since_start:
-        The number of seconds elapsed since data acquisition started.
-        This is the same as ``samples_since_start``, but expressed in
-        seconds.
-    samples_duration:
-        The number of samples collected for this channel.
-    seconds_duration:
-        The number of seconds of data captured for this session.  This
-        is the same as ``samples_duration``, but expressed in seconds.
+GetSignalBytesResponse.ChannelData.__doc__ = """Attributes:
+    data:
+        The signal data.  This is the byte representation of a C-style
+        array of values. Values are stored in order and adjacent to
+        each other.  The type of the elements will depend on whether
+        calibrated data was chosen. The get_data_types() RPC call
+        should be used to determine the precise format of the data,
+        but in general terms, uncalibrated data will be signed
+        integers and calibrated data will be floating-point numbers.
+        Returning the data in this format allows it to be efficiently
+        processed in dynamic languages that can pass the data straight
+        down to a native runtime. For example, in Python, this data
+        can be intepreted directly into a numpy array using
+        numpy.fromstring().  Calibrated data is in picoamps.
+        Uncalibrated data is the raw values output by the device's ADC
+        (analogue-digital converter).
+    config_changes:
+        The configuration changes on the channel during data
+        collection.  If channel configuration changes were requested,
+        this will contain all the channel configuration changes that
+        affect the returned data. This will include at least one
+        element, with offset 0, that describes the configuration at
+        the time the first sample was taken.  Note that the offset is
+        the zero-based index into the adc or picoamps list.  The
+        changes will be ordered by offset.
+"""
+GetChannelStatesResponse.ChannelStateData.__doc__ = """Attributes:
+    channel:
+        Represents the channel number, indexed from one. (i.e. what
+        channel did the channel state change happened on)
+    state:
+        depending on the channel state request, MinKNOW can fill in
+        either the name or the criteria id of the channel state. The
+        criteria id (or state_id) is the number passed in the channel
+        states configuration. Note that MinKNOW also has some default
+        channel states (like unclassified, pending mux change) which
+        receive unique ids - these are numbers bigger than 200.
+    acquisition_raw_index:
+        Indices of when the channel state was first seen. For example,
+        if a request is done half way through the experiment, the
+        first message will contain the current state on the requested
+        channels. The acquisition/analysis index of these would be
+        from when the channel states were set. These are exactly the
+        same numbers we see in the bulk file, in the 'states' table
+    config:
+        Channel config (mux state) the channel state was determined
+        on.
+"""
+GetSignalBytesRequest.__doc__ = """Attributes:
+    length:
+        The amount of data to return.  If this is omitted, data will
+        be streamed until the call is cancelled.
+    seconds:
+        The amount of data to return in seconds.  The number of
+        samples returned will be just enough to cover this period of
+        time. Cannot be specified at the same time as ``samples``.
+    samples:
+        The amount of data to return in samples.  The result will
+        contain exactly this many samples. If this is not possible,
+        the call will fail. Cannot be specified at the same time as
+        ``seconds``.
+    first_channel:
+        The first channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    last_channel:
+        The last channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    include_channel_configs:
+        Whether to include channel configuration settings.
+    include_bias_voltages:
+        Whether to include bias voltage information.
+    calibrated_data:
+        Whether the data should be calibrated.
+    return_when_listening:
+        When this value is set to true, then an empty message will be
+        sent back to the client to indicate that the backend has
+        acknowleged the request, and that any calls made that will
+        affect the signal after that initial  response will be
+        reflected in the next messages
+"""
+GetSignalMinMaxResponse.ChannelData.__doc__ = """Attributes:
+    calibrated_minima:
+        The minimum value for each window.  The type of the elements
+        will depend on whether calibrated data was chosen.
+        Uncalibrated data will be signed integers and calibrated data
+        will be floating-point numbers.  It would be nice to use the
+        "oneof" enum-like type to capture this, but you can't have
+        repeated members in a oneof, and nor can you have a repeated
+        oneof field.  We can simply include message fields for both
+        types of data, as all fields are optional in proto3.  We will
+        rely on the code that constructs this message to guarantee
+        that we don't try and put both types of data into the same
+        message.  Calibrated data is in picoamps. Uncalibrated data is
+        the raw values output by the device's ADC (analogue-digital
+        converter).  This is guaranteed to be the same size as the
+        respective foo_maxima field.
+    calibrated_maxima:
+        The maximum value for each window.  See comments for the
+        "minima" fields above for details of calibrated and
+        uncalibrated data.  This is guaranteed to be the same size as
+        the respective foo_minima field.
+"""
+GetDataTypesResponse.DataType.__doc__ = """Attributes:
+    type:
+        The basic type of the data item.
+    big_endian:
+        Whether the type is big-endian (high-byte first).  For numeric
+        data types, if this is not set, they are little-endian (low-
+        byte first).
+    size:
+        The size of the data type in bytes.
+"""
+GetLiveReadsRequest.UnblockAction.__doc__ = """Attributes:
+    duration:
+        Duration of unblock in seconds.
+"""
+GetSignalMinMaxRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    last_channel:
+        The last channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    window_size:
+        The size of window to summarise.  A value of zero will be
+        rejected; there is no default.
+    calibrated_data:
+        Whether the data should be calibrated.
 """
 GetReadStatisticsRequest.__doc__ = """Attributes:
     channels:
         List of channels required, indexed from 1.
     duration:
         How long to collect the statistics for
     no_current_statistics:
@@ -213,145 +322,142 @@
     required_classifications:
         Specify classifications which the user wants information
         about.  The default behaviour (when empty) is to return
         information on all classifications.  Specifying which
         classifications the user needs information about may allow the
         implementation to be more efficient.
 """
-GetReadStatisticsResponse.ChunkStatistics.__doc__ = """Attributes:
-    median_sd:
-        Aggregated median_sd value from all classified reads. Computed
-        as median(median_sd[...])
-    median:
-        Aggregated median_sd value from all classified reads.
-        Computed as median(median[...])
-    range:
-        Aggregated range value from all classified reads.  Computed as
-        median(q90[...] - q10[...])
+GetReadStatisticsResponse.Statistics.__doc__ = """Attributes:
+    q_5:
+         Quantiles (percentiles)
 """
-GetReadStatisticsResponse.PerConfigurationData.__doc__ = """Attributes:
-    channel_configuration:
-        The channel configuration active during the reads these
-        statistics were gathered for.
-    classifications:
-        Map from classification names to statistics about read
-        (chunks) with that classification.
-    incomplete:
-        If statistics about complete reads were requested, this field
-        may contain data for a final, incomplete read (whose
-        classification is therefore unknown).  This field will not be
-        set if read chunks were requested, or if the data capture
-        happened to end at a complete read boundary.
+GetReadStatisticsResponse.__doc__ = """Attributes:
+    channels:
+        Data for each requested channel, in the same order as
+        requested.
+    samples_since_start:
+        The number of samples collected before the first sample
+        included in this response.  This gives the position of the
+        first data point which all channels share in the calculated
+        statistics. Each individual channel may have samples from read
+        chunks previous to this sample due to read boundaries not
+        being consistent across channels.
+    seconds_since_start:
+        The number of seconds elapsed before the first sample included
+        in this response.  This is the same as
+        ``samples_since_start``, but expressed in seconds.
 """
-GetSignalMinMaxRequest.__doc__ = """Attributes:
-    first_channel:
-        The first channel (inclusive) to return data for.  Note that
-        channel numbering starts at 1.
-    last_channel:
-        The last channel (inclusive) to return data for.  Note that
-        channel numbering starts at 1.
-    window_size:
-        The size of window to summarise.  A value of zero will be
-        rejected; there is no default.
-    calibrated_data:
-        Whether the data should be calibrated.
+GetChannelStatesResponse.__doc__ = """Attributes:
+    channel_states:
+        The streamed data for all channels will be appended to this
+        vector. After the request is made, all the channel state
+        changes are streamed through this array. This is implemented
+        in the idea of a sparse array because we can have channels
+        that remain in the same state for a long time.
 """
-GetLiveReadsResponse.ReadData.__doc__ = """Attributes:
-    id:
-        The id of this read, this id is unique for every read ever
-        produced.
-    number:
-        The minknow assigned number of this read  Read numbers always
-        increment throughout the experiment, and are unique per
-        channel - however they are not necessarily contiguous.
-    start_sample:
-        Absolute start point of this read
-    chunk_start_sample:
-        Absolute start point through the experiment of this chunk
-    chunk_length:
-        Length of the chunk in samples
-    chunk_classifications:
-        All Classifications given to intermediate chunks by analysis
-        See analysis_configuration.get_read_classifications for how to
-        map these integers to names.
-    raw_data:
-        Any raw data selected by the request  The type of the elements
-        will depend on whether calibrated data was chosen. The
-        get_data_types() RPC call should be used to determine the
-        precise format of the data, but in general terms, uncalibrated
-        data will be signed integers and calibrated data will be
-        floating-point numbers.
-    median_before:
-        The median of the read previous to this read. intended to
-        allow querying of the approximate level of this read, comapred
-        to the last.  For example, a user could try to verify this is
-        a strand be ensuring the median of the current read is lower
-        than the median_before level.
-    median:
-        The media pA level of this read from all aggregated read
-        chunks so far.
-    previous_read_classification:
-        The classification of the chunk prior to this read starting.
-    previous_read_end_reason:
-        The classification of the chunk prior to this read starting.
+GetReadStatisticsResponse.PerClassificationData.__doc__ = """Attributes:
+    duration_statistics:
+        Statistics of read (chunk) durations. These will be in the
+        same units as the requested duration (if you ask for X seconds
+        of data, you will get durations back in seconds, but if you
+        ask for X samples of data, you will get durations back in
+        samples).  NB: statistics may be estimates.
+    current_statistics:
+        Statistics for all current (signal) values for all reads under
+        this channel/configuration/classification combination.  NB:
+        Statistics are calculated from raw data.
+    chunk_statistics:
+        Statistics generated from the analysed read chunks (or
+        complete reads), rather than the raw signal.
+    samples_duration:
+        The number of samples seen with this classification on this
+        channel in this channel configuration.
+    seconds_duration:
+        The number of seconds spent in this classification on this
+        channel in this channel configuration.  This is the same as
+        ``samples_duration``, but expressed in seconds.
 """
-GetSignalMinMaxResponse.__doc__ = """Attributes:
+GetSignalBytesResponse.ChannelConfigChange.__doc__ = """Attributes:
+    config:
+        The new channel configuration.
+    offset:
+        The offset in the returned data where the change was applied.
+"""
+LockChannelStatesRequest.__doc__ = """Attributes:
+    channels:
+        The channels that we want to 'deactivate' = set them to the
+        given state until we re-activate them with
+        unlock_channel_states If the channels are already deactivated,
+        it will update the state to the new forced state given (if
+        different). Channels are indexed from 1.
+    state_name:
+        Channel state name as specified in the channel state
+        configuration. It HAS to be different to 'unclassified', which
+        denotes that the channel is active, but had not met any
+        successful criteria yet.
+"""
+GetSignalBytesResponse.__doc__ = """Attributes:
     samples_since_start:
         The number of samples collected before the first sample
         included in this response.  This gives the position of the
         first data point on each channel in the overall stream of data
         being acquired from the device (since this period of data
         acquisition was started).
     seconds_since_start:
         The number of seconds elapsed since data acquisition started.
         This is the same as ``samples_since_start``, but expressed in
         seconds.
     skipped_channels:
         The number of channels omitted at the start of the
         ``channels`` array.
     channels:
-        The window bounds for each requested channel.  Note that
+        The signal for each requested channel.  Note that
         ``skipped_channels`` must be used to determine which channels
         are given here, as not all channels will be included in every
         message. The channels that are provided are contiguous and in
         order, with the first channel being ``first_channel +
         skipped_channels`` (where ``first_channel`` is from the
         request message).
+    bias_voltages:
+        The bias voltages set for each sample.  If bias voltages were
+        requested, this will provide voltage data, one voltage per
+        sample. Note that not every message may include bias_voltages
+        (they will generally be included when ``skipped_channels`` is
+        0, but that is not guaranteed).  The get_data_types() RPC call
+        should be used to determine the format of the data.
 """
 GetLiveReadsRequest.Action.__doc__ = """Attributes:
     channel:
         Channel name to unblock
     read:
         Identifier for the read to act on.  If the read requested is
         no longer in progress, the action fails.
     unblock:
         Unblock a read and skip further data from this read.
     stop_further_data:
         Skip further data from this read, doesn't affect the read
         data.
 """
-GetDataTypesResponse.__doc__ = """Attributes:
-    uncalibrated_signal:
-        The format of the uncalibrated (ADC) signal data returned by
-        get_raw_signal_bytes().  In the current release, this will
-        describe 16-bit little-endian integers.
-    calibrated_signal:
-        The format of the calibrated (picoamp) signal data returned by
-        get_raw_signal_bytes().  In the current release, this will
-        describe 32-bit IEEE 754 floating point values.
-    bias_voltages:
-        The format of the bias voltage data returned by
-        get_raw_signal_bytes().  In the current release, this will
-        describe 16-bit little-endian integers.
-"""
-UnlockChannelStatesRequest.__doc__ = """Attributes:
+GetLiveReadsResponse.__doc__ = """Attributes:
+    samples_since_start:
+        The number of samples collected before the first sample
+        included in this response.  This gives the position of the
+        first data point on each channel in the overall stream of data
+        being acquired from the device (since this period of data
+        acquisition was started).
+    seconds_since_start:
+        The number of seconds elapsed since data acquisition started.
+        This is the same as ``samples_since_start``, but expressed in
+        seconds.
     channels:
-        The channels to activate (active = they will be considered for
-        channel state evaluation in the future). Channels are indexed
-        from 1.
+        In progress reads for the requested channels.  Sparsely
+        populated as not all channels have new/incomplete reads.
+    action_responses:
+        List of responses to requested actions, informing the caller
+        of results to requested unblocks or discards of data.
 """
 GetLiveReadsRequest.StreamSetup.__doc__ = """Attributes:
     first_channel:
         The first channel (inclusive) to return data for.  Note that
         channel numbering starts at 1.
     last_channel:
         The last channel (inclusive) to return data for.  Note that
@@ -374,191 +480,147 @@
         seconds).  A value of 0.0 will cause minknow to unblock reads
         of any length.
     accepted_first_chunk_classifications:
         A set of classification identifiers which the client is
         interested in. If a read starts with a classification not
         listed here the read is never sent to the client.
 """
-GetDataTypesResponse.DataType.__doc__ = """Attributes:
-    type:
-        The basic type of the data item.
-    big_endian:
-        Whether the type is big-endian (high-byte first).  For numeric
-        data types, if this is not set, they are little-endian (low-
-        byte first).
-    size:
-        The size of the data type in bytes.
+GetLiveReadsResponse.ReadData.__doc__ = """Attributes:
+    id:
+        The id of this read, this id is unique for every read ever
+        produced.
+    number:
+        The minknow assigned number of this read  Read numbers always
+        increment throughout the experiment, and are unique per
+        channel - however they are not necessarily contiguous.
+    start_sample:
+        Absolute start point of this read
+    chunk_start_sample:
+        Absolute start point through the experiment of this chunk
+    chunk_length:
+        Length of the chunk in samples
+    chunk_classifications:
+        All Classifications given to intermediate chunks by analysis
+        See analysis_configuration.get_read_classifications for how to
+        map these integers to names.
+    raw_data:
+        Any raw data selected by the request  The type of the elements
+        will depend on whether calibrated data was chosen. The
+        get_data_types() RPC call should be used to determine the
+        precise format of the data, but in general terms, uncalibrated
+        data will be signed integers and calibrated data will be
+        floating-point numbers.
+    median_before:
+        The median of the read previous to this read. intended to
+        allow querying of the approximate level of this read, comapred
+        to the last.  For example, a user could try to verify this is
+        a strand be ensuring the median of the current read is lower
+        than the median_before level.
+    median:
+        The media pA level of this read from all aggregated read
+        chunks so far.
+    previous_read_classification:
+        The classification of the chunk prior to this read starting.
+    previous_read_end_reason:
+        The classification of the chunk prior to this read starting.
 """
-GetSignalBytesResponse.__doc__ = """Attributes:
+GetDataTypesResponse.__doc__ = """Attributes:
+    uncalibrated_signal:
+        The format of the uncalibrated (ADC) signal data returned by
+        get_raw_signal_bytes().  In the current release, this will
+        describe 16-bit little-endian integers.
+    calibrated_signal:
+        The format of the calibrated (picoamp) signal data returned by
+        get_raw_signal_bytes().  In the current release, this will
+        describe 32-bit IEEE 754 floating point values.
+    bias_voltages:
+        The format of the bias voltage data returned by
+        get_raw_signal_bytes().  In the current release, this will
+        describe 16-bit little-endian integers.
+"""
+GetReadStatisticsResponse.ChunkStatistics.__doc__ = """Attributes:
+    median_sd:
+        Aggregated median_sd value from all classified reads. Computed
+        as median(median_sd[...])
+    median:
+        Aggregated median_sd value from all classified reads.
+        Computed as median(median[...])
+    range:
+        Aggregated range value from all classified reads.  Computed as
+        median(q90[...] - q10[...])
+"""
+GetLiveReadsRequest.__doc__ = """Attributes:
+    setup:
+        Read setup request, initialises channel numbers and type of
+        data returned.  note: Must be specified in the first message
+        sent to MinKNOW. Once MinKNOW has the first setup message
+        reads are sent to the caller as requested. The user can then
+        resend a setup message as frequently as they need to in order
+        to reconfigure live reads - for example by changing if raw
+        data is sent with reads or not.
+    actions:
+        Actions to take given data returned to the user - can only be
+        sent once the setup message above has been sent.
+"""
+GetReadStatisticsResponse.PerConfigurationData.__doc__ = """Attributes:
+    channel_configuration:
+        The channel configuration active during the reads these
+        statistics were gathered for.
+    classifications:
+        Map from classification names to statistics about read
+        (chunks) with that classification.
+    incomplete:
+        If statistics about complete reads were requested, this field
+        may contain data for a final, incomplete read (whose
+        classification is therefore unknown).  This field will not be
+        set if read chunks were requested, or if the data capture
+        happened to end at a complete read boundary.
+"""
+GetReadStatisticsResponse.PerChannelData.__doc__ = """Attributes:
+    configurations:
+        Data for each channel configuration seen on this channel.
+        Note that each channel configuration will only appear once in
+        this list, and this list is *not* in any way ordered by time.
+        The only reason it is not a map is because of restrictions on
+        map key types.
+    samples_since_start:
+        The number of samples collected before this channel's first
+        sample.
+    seconds_since_start:
+        The number of seconds elapsed since data acquisition started.
+        This is the same as ``samples_since_start``, but expressed in
+        seconds.
+    samples_duration:
+        The number of samples collected for this channel.
+    seconds_duration:
+        The number of seconds of data captured for this session.  This
+        is the same as ``samples_duration``, but expressed in seconds.
+"""
+GetSignalMinMaxResponse.__doc__ = """Attributes:
     samples_since_start:
         The number of samples collected before the first sample
         included in this response.  This gives the position of the
         first data point on each channel in the overall stream of data
         being acquired from the device (since this period of data
         acquisition was started).
     seconds_since_start:
         The number of seconds elapsed since data acquisition started.
         This is the same as ``samples_since_start``, but expressed in
         seconds.
     skipped_channels:
         The number of channels omitted at the start of the
         ``channels`` array.
     channels:
-        The signal for each requested channel.  Note that
+        The window bounds for each requested channel.  Note that
         ``skipped_channels`` must be used to determine which channels
         are given here, as not all channels will be included in every
         message. The channels that are provided are contiguous and in
         order, with the first channel being ``first_channel +
         skipped_channels`` (where ``first_channel`` is from the
         request message).
-    bias_voltages:
-        The bias voltages set for each sample.  If bias voltages were
-        requested, this will provide voltage data, one voltage per
-        sample. Note that not every message may include bias_voltages
-        (they will generally be included when ``skipped_channels`` is
-        0, but that is not guaranteed).  The get_data_types() RPC call
-        should be used to determine the format of the data.
-"""
-GetChannelStatesResponse.__doc__ = """Attributes:
-    channel_states:
-        The streamed data for all channels will be appended to this
-        vector. After the request is made, all the channel state
-        changes are streamed through this array. This is implemented
-        in the idea of a sparse array because we can have channels
-        that remain in the same state for a long time.
-"""
-GetSignalBytesResponse.ChannelData.__doc__ = """Attributes:
-    data:
-        The signal data.  This is the byte representation of a C-style
-        array of values. Values are stored in order and adjacent to
-        each other.  The type of the elements will depend on whether
-        calibrated data was chosen. The get_data_types() RPC call
-        should be used to determine the precise format of the data,
-        but in general terms, uncalibrated data will be signed
-        integers and calibrated data will be floating-point numbers.
-        Returning the data in this format allows it to be efficiently
-        processed in dynamic languages that can pass the data straight
-        down to a native runtime. For example, in Python, this data
-        can be intepreted directly into a numpy array using
-        numpy.fromstring().  Calibrated data is in picoamps.
-        Uncalibrated data is the raw values output by the device's ADC
-        (analogue-digital converter).
-    config_changes:
-        The configuration changes on the channel during data
-        collection.  If channel configuration changes were requested,
-        this will contain all the channel configuration changes that
-        affect the returned data. This will include at least one
-        element, with offset 0, that describes the configuration at
-        the time the first sample was taken.  Note that the offset is
-        the zero-based index into the adc or picoamps list.  The
-        changes will be ordered by offset.
-"""
-GetSignalBytesRequest.__doc__ = """Attributes:
-    length:
-        The amount of data to return.  If this is omitted, data will
-        be streamed until the call is cancelled.
-    seconds:
-        The amount of data to return in seconds.  The number of
-        samples returned will be just enough to cover this period of
-        time. Cannot be specified at the same time as ``samples``.
-    samples:
-        The amount of data to return in samples.  The result will
-        contain exactly this many samples. If this is not possible,
-        the call will fail. Cannot be specified at the same time as
-        ``seconds``.
-    first_channel:
-        The first channel (inclusive) to return data for.  Note that
-        channel numbering starts at 1.
-    last_channel:
-        The last channel (inclusive) to return data for.  Note that
-        channel numbering starts at 1.
-    include_channel_configs:
-        Whether to include channel configuration settings.
-    include_bias_voltages:
-        Whether to include bias voltage information.
-    calibrated_data:
-        Whether the data should be calibrated.
-    return_when_listening:
-        When this value is set to true, then an empty message will be
-        sent back to the client to indicate that the backend has
-        acknowleged the request, and that any calls made that will
-        affect the signal after that initial  response will be
-        reflected in the next messages
-"""
-GetSignalBytesResponse.ChannelConfigChange.__doc__ = """Attributes:
-    config:
-        The new channel configuration.
-    offset:
-        The offset in the returned data where the change was applied.
-"""
-GetReadStatisticsResponse.PerClassificationData.__doc__ = """Attributes:
-    duration_statistics:
-        Statistics of read (chunk) durations. These will be in the
-        same units as the requested duration (if you ask for X seconds
-        of data, you will get durations back in seconds, but if you
-        ask for X samples of data, you will get durations back in
-        samples).  NB: statistics may be estimates.
-    current_statistics:
-        Statistics for all current (signal) values for all reads under
-        this channel/configuration/classification combination.  NB:
-        Statistics are calculated from raw data.
-    chunk_statistics:
-        Statistics generated from the analysed read chunks (or
-        complete reads), rather than the raw signal.
-    samples_duration:
-        The number of samples seen with this classification on this
-        channel in this channel configuration.
-    seconds_duration:
-        The number of seconds spent in this classification on this
-        channel in this channel configuration.  This is the same as
-        ``samples_duration``, but expressed in seconds.
-"""
-GetReadStatisticsResponse.Statistics.__doc__ = """Attributes:
-    q_5:
-         Quantiles (percentiles)
-"""
-GetLiveReadsResponse.__doc__ = """Attributes:
-    samples_since_start:
-        The number of samples collected before the first sample
-        included in this response.  This gives the position of the
-        first data point on each channel in the overall stream of data
-        being acquired from the device (since this period of data
-        acquisition was started).
-    seconds_since_start:
-        The number of seconds elapsed since data acquisition started.
-        This is the same as ``samples_since_start``, but expressed in
-        seconds.
-    channels:
-        In progress reads for the requested channels.  Sparsely
-        populated as not all channels have new/incomplete reads.
-    action_responses:
-        List of responses to requested actions, informing the caller
-        of results to requested unblocks or discards of data.
-"""
-GetSignalMinMaxResponse.ChannelData.__doc__ = """Attributes:
-    calibrated_minima:
-        The minimum value for each window.  The type of the elements
-        will depend on whether calibrated data was chosen.
-        Uncalibrated data will be signed integers and calibrated data
-        will be floating-point numbers.  It would be nice to use the
-        "oneof" enum-like type to capture this, but you can't have
-        repeated members in a oneof, and nor can you have a repeated
-        oneof field.  We can simply include message fields for both
-        types of data, as all fields are optional in proto3.  We will
-        rely on the code that constructs this message to guarantee
-        that we don't try and put both types of data into the same
-        message.  Calibrated data is in picoamps. Uncalibrated data is
-        the raw values output by the device's ADC (analogue-digital
-        converter).  This is guaranteed to be the same size as the
-        respective foo_maxima field.
-    calibrated_maxima:
-        The maximum value for each window.  See comments for the
-        "minima" fields above for details of calibrated and
-        uncalibrated data.  This is guaranteed to be the same size as
-        the respective foo_minima field.
 """
 GetChannelStatesRequest.__doc__ = """Attributes:
     first_channel:
         The first channel (inclusive) to return data for.  Note that
         channel numbering starts at 1.
     last_channel:
         The last channel (inclusive) to return data for.  Note that
@@ -577,76 +639,14 @@
         circumstances (eg: a flow cell with no sample loaded) there
         can be long periods of time without updates.  Setting this
         value will ensure that if this period of time passes without
         there being any channel state changes to report, an empty
         message will be sent. This can be useful to force a minimum
         wakeup interval in the client code.
 """
-GetChannelStatesResponse.ChannelStateData.__doc__ = """Attributes:
-    channel:
-        Represents the channel number, indexed from one. (i.e. what
-        channel did the channel state change happened on)
-    state:
-        depending on the channel state request, MinKNOW can fill in
-        either the name or the criteria id of the channel state. The
-        criteria id (or state_id) is the number passed in the channel
-        states configuration. Note that MinKNOW also has some default
-        channel states (like unclassified, pending mux change) which
-        receive unique ids - these are numbers bigger than 200.
-    acquisition_raw_index:
-        Indices of when the channel state was first seen. For example,
-        if a request is done half way through the experiment, the
-        first message will contain the current state on the requested
-        channels. The acquisition/analysis index of these would be
-        from when the channel states were set. These are exactly the
-        same numbers we see in the bulk file, in the 'states' table
-    config:
-        Channel config (mux state) the channel state was determined
-        on.
-"""
-GetLiveReadsRequest.UnblockAction.__doc__ = """Attributes:
-    duration:
-        Duration of unblock in seconds.
-"""
-GetLiveReadsRequest.__doc__ = """Attributes:
-    setup:
-        Read setup request, initialises channel numbers and type of
-        data returned.  note: Must be specified in the first message
-        sent to MinKNOW. Once MinKNOW has the first setup message
-        reads are sent to the caller as requested. The user can then
-        resend a setup message as frequently as they need to in order
-        to reconfigure live reads - for example by changing if raw
-        data is sent with reads or not.
-    actions:
-        Actions to take given data returned to the user - can only be
-        sent once the setup message above has been sent.
-"""
-GetReadStatisticsResponse.__doc__ = """Attributes:
-    channels:
-        Data for each requested channel, in the same order as
-        requested.
-    samples_since_start:
-        The number of samples collected before the first sample
-        included in this response.  This gives the position of the
-        first data point which all channels share in the calculated
-        statistics. Each individual channel may have samples from read
-        chunks previous to this sample due to read boundaries not
-        being consistent across channels.
-    seconds_since_start:
-        The number of seconds elapsed before the first sample included
-        in this response.  This is the same as
-        ``samples_since_start``, but expressed in seconds.
-"""
-LockChannelStatesRequest.__doc__ = """Attributes:
+UnlockChannelStatesRequest.__doc__ = """Attributes:
     channels:
-        The channels that we want to 'deactivate' = set them to the
-        given state until we re-activate them with
-        unlock_channel_states If the channels are already deactivated,
-        it will update the state to the new forced state given (if
-        different). Channels are indexed from 1.
-    state_name:
-        Channel state name as specified in the channel state
-        configuration. It HAS to be different to 'unclassified', which
-        denotes that the channel is active, but had not met any
-        successful criteria yet.
+        The channels to activate (active = they will be considered for
+        channel state evaluation in the future). Channels are indexed
+        from 1.
 """
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/data_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/data_service.py` & `minknow_api-5.9.5/minknow_api/data_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/device.py` & `minknow_api-5.9.5/minknow_api/device.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/device_pb2.py` & `minknow_api-5.9.5/minknow_api/device_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -252,195 +252,14 @@
   _globals['_SETFLOWCELLBARCODEKITRESPONSE']._serialized_end=6382
   _globals['_REGISTERFLOWCELLBARCODESREQUEST']._serialized_start=6384
   _globals['_REGISTERFLOWCELLBARCODESREQUEST']._serialized_end=6435
   _globals['_REGISTERFLOWCELLBARCODESRESPONSE']._serialized_start=6437
   _globals['_REGISTERFLOWCELLBARCODESRESPONSE']._serialized_end=6471
   _globals['_DEVICESERVICE']._serialized_start=6741
   _globals['_DEVICESERVICE']._serialized_end=10400
-SaturationConfig.Thresholds.__doc__ = """The thresholds define how many over limit samples are required to
-trigger saturation on the device.  Each packet of frames minknow
-receive is delivered to the saturation check (in approx 64 frame
-chunks), only the first frame of each packet is inspected. The
-thresholds control how many _packets_ must be outside the valid range.
-ie. if general_threshold is set to 10, at least 640 frames are
-required to trigger saturation.  It is also possible to not define the
-value to never trigger saturation in this config.  Note: Setting a
-saturation threshold to 0 will prevent the threshold from triggering.
-
-Attributes:
-    general_threshold:
-        Threshold for software saturation on all non-unblock muxes
-    unblock_threshold:
-        Threshold for software saturation on unblock muxes
-    user_general_threshold:
-        Threshold for user threshold  saturation on all non-unblock
-        muxes
-    user_unblock_threshold:
-        Threshold for user threshold saturation on unblock muxes
-"""
-GetDeviceStateResponse.__doc__ = """Attributes:
-    device_state:
-        Whether the physical hardware is present.  This is really only
-        relevant to MinIONs, which could be unplugged by the user at
-        any time.
-    flow_cell_connector:
-        Indicates what sort of flow cell can be inserted.  For
-        example, if the user needs to set or override the flow cell
-        product code, this can be used to limit the list of possible
-        flow cell product codes to choose from.  Since 4.1
-"""
-RegisterFlowCellBarcodesRequest.__doc__ = """Attributes:
-    barcodes:
-        List of unique barcodes that have been used with the flow-cell
-        Where a barcode is represented by an index in the range of 1
-        to 384 only.
-"""
-UnblockRequest.__doc__ = """Attributes:
-    channels:
-        List of channels indexed from 1.
-    duration:
-        How long should an unblock last.
-"""
-SaturationConfig.UserThresholdSaturation.__doc__ = """User threshold is specified in pico amps
-
-Attributes:
-    enabled:
-        Set to enable or disable software saturation.
-    user_threshold_min_pa:
-        The minimum pA value that is not a saturation.  If this value
-        is not specified, the previous value is kept.
-    user_threshold_max_pa:
-        The maximum pA value that is not a saturation.  If this value
-        is not specified, the previous value is kept.
-"""
-SetChannelConfigurationRequest.__doc__ = """Attributes:
-    channel_configurations:
-        A map between <channel name, config to set>  Will return an
-        error if any of the key values (representing channel names)
-        are below 1, or above the channel count value returned from
-        :meth:`get_flow_cell_info`  The selected well cannot be set to
-        WELL_OTHER, and will error if it tries to do so  DEPRECATED:
-        Note that the type to set may change from 4.0 to enforce the
-        fact that unblock cannot be set through this call
-"""
-SaturationConfig.__doc__ = """Attributes:
-    thresholds:
-        Settings for saturation count thresholds, this controls how
-        long a saturated value must be over limit before the channel
-        is turned off.  If not specified, the previous thresholds are
-        kept.
-    software_saturation:
-        Settings for software saturation, specified in adc units of
-        the device.  If not specified, the previous thresholds are
-        kept.
-    user_threshold_saturation:
-        Settings for user threshold saturation, specified in pA.  If
-        not specified, the previous thresholds are kept.
-"""
-SetTemperatureResponse.__doc__ = """Attributes:
-    timed_out_waiting_for_temperature:
-        Find if we hit a timeout waiting for the temperature to be
-        hit.  Deprecated since 5.5; in favour of the
-        `TIMED_OUT_WAITING_FOR_TEMPERATURE` result code.
-    result:
-        The result of setting the temperature  Since 5.5  NB - before
-        5.5, checking this field will always return a value of
-        `TARGET_TEMPERATURE_SET` The "real" value may be inferred as
-        follows:  - If `wait_for_temperature` was NOT specified, the
-        "real" result is    `TARGET_TEMPERATURE_SET`  - If
-        `wait_for_temperature` was specified, and
-        `timed_out_waiting_for_temperature` is    false, the "real"
-        result is `REACHED_TEMPERATURE`  - If `wait_for_temperature`
-        was specified, and `timed_out_waiting_for_temperature` is
-        true, the "real" result is `TIMED_OUT_WAITING_FOR_TEMPERATURE`
-        - Versions prior to 5.5 do not support setting the secondary
-        temperature limit, and so (for    these versions) the "real"
-        value can never be `SECONDARY_TEMPERATURE_LIMITS_EXCEEDED`
-"""
-SetTemperatureRequest.WaitForTemperatureSettings.__doc__ = """Attributes:
-    timeout:
-        Maximum duration (in seconds) to wait for the device to reach
-        temperature.  Not specifying a value will wait for a maximum
-        of 5 minutes.
-    min_stable_duration:
-        Minimum duration (in seconds) that the reported temperature
-        must be continually within the target temperature range,
-        before the device is considered to have reached temperature.
-        A value of zero means that the device will be considered to
-        have reached temperature as soon as the reported temperature
-        is equal to the target temperature.  Not specifying a value is
-        equivalent to specifying a value of zero.  The
-        min_stable_duration must be less than or equal to the timeout
-        duration (if it were greater, then the temperature would never
-        be read as 'stable' before the time-out occurred).  Since 3.4
-    tolerance:
-        Specify an optional tolerance to apply to the wait.  For
-        example, if the target temperature is 35, and the tolerance is
-        1 any temperature in the range 34 - 36 will cause the request
-        to return.  Default is 0.5 degree tolerance.
-"""
-GetCalibrationRequest.__doc__ = """Attributes:
-    first_channel:
-        The first channel to get calibration data for.  This should
-        normally be 1.
-    last_channel:
-        The last channel included in calibration data.  This should
-        normally be the channel count returned by
-        :meth:`get_flow_cell_info`.
-"""
-SetCalibrationRequest.__doc__ = """Attributes:
-    first_channel:
-        The first channel included in calibration data.  This must
-        always be 1. This is required in order to make sure the client
-        and MinKNOW agree on what data is being provided.
-    last_channel:
-        The last channel included in calibration data.  This must
-        always be the same as the channel count returned by
-        :meth:`get_flow_cell_info`. This is required in order to make
-        sure the client and MinKNOW agree on what data is being
-        provided.
-    offsets:
-        The ADC value adjustment to reach 0pA on each channel.  This
-        is ``-x``, where ``x`` is the (mean) ADC value at 0pA.
-    pa_ranges:
-        The range of possible pA values that can be produced by the
-        device.
-"""
-SaturationConfig.SoftwareSaturation.__doc__ = """The ranges specify the actual pA or ADC ranges which will trigger
-saturation. This range is checked against the first sample in each
-delivered packet.  software saturation is specified in adc units
-
-Attributes:
-    enabled:
-        Set to enable or disable software saturation.
-    software_min_adc:
-        The minimum adc value that is not a saturation.  If this value
-        is not specified, the previous value is kept.
-    software_max_adc:
-        The maximum adc value that is not a saturation.  If this value
-        is not specified, the previous value is kept.
-"""
-SetTemperatureRequest.SecondaryTemperatureLimits.__doc__ = """Attributes:
-    min:
-        The minimum permissible "secondary" temperature
-    max:
-        The maximum permissible "secondary" temperature
-"""
-GetTemperatureResponse.__doc__ = """Attributes:
-    target_temperature:
-        Return the temperature target the device is aiming to reach.
-    flowcell_temperature:
-        Temperature as measured by thermistor TH2 on the P-Chip.
-    chamber_temperature:
-        Flow-cell chamber-temperature, calculated from the pixel-block
-        temperatures
-    pixel_block_temperature:
-        Temperature measured at each sensor in the ASIC, there are 12
-        sensors, one sensor per pixel-block
-"""
 GetFlowCellInfoResponse.__doc__ = """Attributes:
     has_flow_cell:
         Whether there is a flow cell present.  If both this and
         has_adapter are false, none of the other fields will contain
         useful information.
     channel_count:
         The number of channels currently supported by the device.
@@ -527,25 +346,73 @@
     barcode_kit:
         The flow cell barcode kit identity  Since 5.6
     barcodes:
         The unique barcodes (as represented by indices between 1 to
         384) that have been set by calls to
         register_flow_cell_barcodes() on this flow cell. Since 5.6
 """
-SetUserSpecifiedProductCodeRequest.__doc__ = """Attributes:
-    code:
-        A product code for the flow cell, which the user can specify.
-        In the event a flow cell does not have an eeprom, the user can
-        specify product code here.  Since 1.12
+SaturationConfig.__doc__ = """Attributes:
+    thresholds:
+        Settings for saturation count thresholds, this controls how
+        long a saturated value must be over limit before the channel
+        is turned off.  If not specified, the previous thresholds are
+        kept.
+    software_saturation:
+        Settings for software saturation, specified in adc units of
+        the device.  If not specified, the previous thresholds are
+        kept.
+    user_threshold_saturation:
+        Settings for user threshold saturation, specified in pA.  If
+        not specified, the previous thresholds are kept.
 """
-CancelUnblocksResponse.__doc__ = """Attributes:
-    cancelled_unblocks:
-        The number of unblocks which have been cancelled as part of
-        this request.  Should return the total number of unblock
-        operations which have been cancelled.
+SetSampleRateResponse.__doc__ = """Attributes:
+    real_sample_rate:
+        The real sample rate is the actual sample rate that is set on
+        the device, which may be different from the actual value
+        passed into the rpc.  For example on promethion, when it is
+        given a sample rate, it will round to the nearest 1000. So
+        1499 becomes 1000 and 1500 becomes 2000 real sample rate  For
+        a minion, the actual sample rate is determined via 3 separate
+        values; clock speed, integration time and clock divider, and
+        so not all values are possible. e.g. setting 3000 will return
+        3012 real sample rate. See 'sampling_frequency' in
+        MinionDeviceService for a slightly more in depth explanation
+"""
+GetCalibrationRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel to get calibration data for.  This should
+        normally be 1.
+    last_channel:
+        The last channel included in calibration data.  This should
+        normally be the channel count returned by
+        :meth:`get_flow_cell_info`.
+"""
+SaturationConfig.UserThresholdSaturation.__doc__ = """User threshold is specified in pico amps
+
+Attributes:
+    enabled:
+        Set to enable or disable software saturation.
+    user_threshold_min_pa:
+        The minimum pA value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+    user_threshold_max_pa:
+        The maximum pA value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+"""
+RegisterFlowCellBarcodesRequest.__doc__ = """Attributes:
+    barcodes:
+        List of unique barcodes that have been used with the flow-cell
+        Where a barcode is represented by an index in the range of 1
+        to 384 only.
+"""
+GetChannelConfigurationResponse.__doc__ = """Attributes:
+    channel_configurations:
+        A list of channel configurations  The order of channel
+        configurations matches the channel order specified by
+        :attribute:`channels` in the request message
 """
 GetDeviceInfoResponse.ComponentVersion.__doc__ = """Firmware versions and serial-numbers of components associated with
 this device  Depending on the hardware, there may be several
 components associated with this device, each with their own firmware
 version and serial-number. Not all components have serial-numbers.
 
 Attributes:
@@ -556,38 +423,32 @@
         component where the firmware version would usually be
         available, this will contain "Unknown"
     serial_number:
         The serial-number of a component. If this in not applicable to
         the type of component or cannot be read at the current time,
         then this field will be blank.
 """
-SetSampleRateResponse.__doc__ = """Attributes:
-    real_sample_rate:
-        The real sample rate is the actual sample rate that is set on
-        the device, which may be different from the actual value
-        passed into the rpc.  For example on promethion, when it is
-        given a sample rate, it will round to the nearest 1000. So
-        1499 becomes 1000 and 1500 becomes 2000 real sample rate  For
-        a minion, the actual sample rate is determined via 3 separate
-        values; clock speed, integration time and clock divider, and
-        so not all values are possible. e.g. setting 3000 will return
-        3012 real sample rate. See 'sampling_frequency' in
-        MinionDeviceService for a slightly more in depth explanation
-"""
-StreamTemperatureRequest.__doc__ = """Attributes:
-    period_seconds:
-        How often temperature updates should be sent Defaults to a
-        period of 1 second, if not specified, or set to 0
-    acquisition_run_id:
-        The acquisition id of the experiment.
-    data_selection:
-        The desired data selection.  The units for all values are
-        `seconds since the start of the experiment`.
+GetCalibrationResponse.__doc__ = """Attributes:
+    digitisation:
+        The range of possible ADC values that can be produced by the
+        device.  This is the same as the digitisation value returned
+        by the :meth:`DeviceService.get_device_info` RPC. It is
+        included here for convenience.
+    offsets:
+        The ADC value adjustment to reach 0pA on each channel.  This
+        is ``-x``, where ``x`` is the (mean) ADC value at 0pA.
+    pa_ranges:
+        The range of possible pA values that can be produced on each
+        channel.  The change in pA represented by a change of 1 ADC
+        can be calculated by dividing the digitisation by this value.
+    has_calibration:
+        Find if there is a stored calibration, or if the returned
+        response is empty.  Since 1.12
 """
-ReturnedChannelConfiguration.__doc__ = """Describes the configuration of a channel on the device.  Note that
+ChannelConfiguration.__doc__ = """Describes the configuration of a channel on the device.  Note that
 this is a lossy representation. The device-specific APIs provide more
 precise information. This only describes common configurations, and
 omits anything that doesn't impact the received signal.
 
 Attributes:
     well:
         The currently-connected well.  Wells are counted from 1. 0
@@ -601,36 +462,14 @@
         can simultaneously connect all wells, and MinIONs can connect
         to ground).
     test_current:
         Whether the test current is connected to the integrator
         (measurement circuit).  The signal will be a steady test
         current produced on the device. This can be used for
         calibration or to test the device integration circuits.
-    unblock:
-        Whether the unblock voltage is connected to the integrator
-        (measurement circuit).  Provides a reverse potential across
-        the connected well. This can be used to drive molecules back
-        out of the well.
-"""
-GetTemperatureResponse.PromethIONTemperature.__doc__ = """Packet of temperatures appropriate for a PromethION.
-
-Attributes:
-    flowcell_temperature:
-        Temperature as measured by thermistor TH2 on the P-Chip. This
-        is the "primary" temperature
-    chamber_temperature:
-        Mean of 12 pixel-blocks temperatures measured with sensors in
-        the ASIC. This is the "secondary" temperature
-"""
-SetUserSpecifiedFlowCellIdRequest.__doc__ = """Attributes:
-    id:
-        A unique identifier for the flow cell, which the user can
-        specify.  In the event a flow cell does not have an eeprom,
-        this field can be used by the user to record their
-        flow_cell_id.  Since 1.12
 """
 GetDeviceInfoResponse.__doc__ = """Attributes:
     device_id:
         A unique identifier for the device.  This is the identifier of
         the device MinKNOW was started for. It will only communicate
         with this device.  Note that simulated device IDs are only
         unique for this host, not globally.  This value will be set
@@ -667,53 +506,140 @@
         the temperature will be maintained at a pre-determined
         temperature.
     digitisation:
         The range of uncalibrated data values.  This is the number of
         distinct signal values that can be produced by the device's
         analog to digital converter (ADC).
 """
-GetChannelConfigurationResponse.__doc__ = """Attributes:
+SetFlowCellBarcodeKitRequest.__doc__ = """Attributes:
+    id:
+        The Barcode Kit ID can be up to 8 characters long
+"""
+SetChannelConfigurationRequest.__doc__ = """Attributes:
     channel_configurations:
-        A list of channel configurations  The order of channel
-        configurations matches the channel order specified by
-        :attribute:`channels` in the request message
+        A map between <channel name, config to set>  Will return an
+        error if any of the key values (representing channel names)
+        are below 1, or above the channel count value returned from
+        :meth:`get_flow_cell_info`  The selected well cannot be set to
+        WELL_OTHER, and will error if it tries to do so  DEPRECATED:
+        Note that the type to set may change from 4.0 to enforce the
+        fact that unblock cannot be set through this call
 """
-GetTemperatureResponse.MinIONTemperature.__doc__ = """Packet of temperatures appropriate for a MinION.
+SetUserSpecifiedProductCodeRequest.__doc__ = """Attributes:
+    code:
+        A product code for the flow cell, which the user can specify.
+        In the event a flow cell does not have an eeprom, the user can
+        specify product code here.  Since 1.12
+"""
+SetTemperatureRequest.WaitForTemperatureSettings.__doc__ = """Attributes:
+    timeout:
+        Maximum duration (in seconds) to wait for the device to reach
+        temperature.  Not specifying a value will wait for a maximum
+        of 5 minutes.
+    min_stable_duration:
+        Minimum duration (in seconds) that the reported temperature
+        must be continually within the target temperature range,
+        before the device is considered to have reached temperature.
+        A value of zero means that the device will be considered to
+        have reached temperature as soon as the reported temperature
+        is equal to the target temperature.  Not specifying a value is
+        equivalent to specifying a value of zero.  The
+        min_stable_duration must be less than or equal to the timeout
+        duration (if it were greater, then the temperature would never
+        be read as 'stable' before the time-out occurred).  Since 3.4
+    tolerance:
+        Specify an optional tolerance to apply to the wait.  For
+        example, if the target temperature is 35, and the tolerance is
+        1 any temperature in the range 34 - 36 will cause the request
+        to return.  Default is 0.5 degree tolerance.
+"""
+GetTemperatureResponse.__doc__ = """Attributes:
+    target_temperature:
+        Return the temperature target the device is aiming to reach.
+    flowcell_temperature:
+        Temperature as measured by thermistor TH2 on the P-Chip.
+    chamber_temperature:
+        Flow-cell chamber-temperature, calculated from the pixel-block
+        temperatures
+    pixel_block_temperature:
+        Temperature measured at each sensor in the ASIC, there are 12
+        sensors, one sensor per pixel-block
+"""
+GetDeviceStateResponse.__doc__ = """Attributes:
+    device_state:
+        Whether the physical hardware is present.  This is really only
+        relevant to MinIONs, which could be unplugged by the user at
+        any time.
+    flow_cell_connector:
+        Indicates what sort of flow cell can be inserted.  For
+        example, if the user needs to set or override the flow cell
+        product code, this can be used to limit the list of possible
+        flow cell product codes to choose from.  Since 4.1
+"""
+SetUserSpecifiedFlowCellIdRequest.__doc__ = """Attributes:
+    id:
+        A unique identifier for the flow cell, which the user can
+        specify.  In the event a flow cell does not have an eeprom,
+        this field can be used by the user to record their
+        flow_cell_id.  Since 1.12
+"""
+SaturationConfig.Thresholds.__doc__ = """The thresholds define how many over limit samples are required to
+trigger saturation on the device.  Each packet of frames minknow
+receive is delivered to the saturation check (in approx 64 frame
+chunks), only the first frame of each packet is inspected. The
+thresholds control how many _packets_ must be outside the valid range.
+ie. if general_threshold is set to 10, at least 640 frames are
+required to trigger saturation.  It is also possible to not define the
+value to never trigger saturation in this config.  Note: Setting a
+saturation threshold to 0 will prevent the threshold from triggering.
 
 Attributes:
-    asic_temperature:
-        Temperature as measured by the probe inside the asic. This is
-        the "secondary" temperature
-    heatsink_temperature:
-        Temperature as measured by the probe in the minion heatsink.
-        This is the "primary" temperature
+    general_threshold:
+        Threshold for software saturation on all non-unblock muxes
+    unblock_threshold:
+        Threshold for software saturation on unblock muxes
+    user_general_threshold:
+        Threshold for user threshold  saturation on all non-unblock
+        muxes
+    user_unblock_threshold:
+        Threshold for user threshold saturation on unblock muxes
 """
-GetChannelConfigurationRequest.__doc__ = """Attributes:
-    channels:
-        A list of channel names (1-indexed) to specify what channels
-        to get channel configs for  Will return an error if any of the
-        channel names are below 1, or above the channel count value
-        returned from :meth:`get_flow_cell_info`
+CancelUnblocksResponse.__doc__ = """Attributes:
+    cancelled_unblocks:
+        The number of unblocks which have been cancelled as part of
+        this request.  Should return the total number of unblock
+        operations which have been cancelled.
 """
-GetCalibrationResponse.__doc__ = """Attributes:
-    digitisation:
-        The range of possible ADC values that can be produced by the
-        device.  This is the same as the digitisation value returned
-        by the :meth:`DeviceService.get_device_info` RPC. It is
-        included here for convenience.
-    offsets:
-        The ADC value adjustment to reach 0pA on each channel.  This
-        is ``-x``, where ``x`` is the (mean) ADC value at 0pA.
-    pa_ranges:
-        The range of possible pA values that can be produced on each
-        channel.  The change in pA represented by a change of 1 ADC
-        can be calculated by dividing the digitisation by this value.
-    has_calibration:
-        Find if there is a stored calibration, or if the returned
-        response is empty.  Since 1.12
+ReturnedChannelConfiguration.__doc__ = """Describes the configuration of a channel on the device.  Note that
+this is a lossy representation. The device-specific APIs provide more
+precise information. This only describes common configurations, and
+omits anything that doesn't impact the received signal.
+
+Attributes:
+    well:
+        The currently-connected well.  Wells are counted from 1. 0
+        indicates that no well is connected. 5 indicates some non-
+        generic configuration such as ground for a minion or
+        connecting all wells on promethion  Note that MinKNOW can
+        return channel configurations where the well number is larger
+        than the ``max_well_count`` value returned by
+        :meth:`DeviceService.get_device_info`. This indicates that
+        some other connection has been made (for example, PromethIONs
+        can simultaneously connect all wells, and MinIONs can connect
+        to ground).
+    test_current:
+        Whether the test current is connected to the integrator
+        (measurement circuit).  The signal will be a steady test
+        current produced on the device. This can be used for
+        calibration or to test the device integration circuits.
+    unblock:
+        Whether the unblock voltage is connected to the integrator
+        (measurement circuit).  Provides a reverse potential across
+        the connected well. This can be used to drive molecules back
+        out of the well.
 """
 SetTemperatureRequest.__doc__ = """Attributes:
     temperature:
         The desired temperature in degrees Celsius.  If temperature
         control is supported and enabled, the device will attempt to
         keep its primary temperature at this value. The reading used
         as the "primary" temperature depends on the device: - For
@@ -755,35 +681,109 @@
         to be reached, then all temperature control settings are reset
         to the values they had prior to the call to
         `set_temperature()` being made.  NB - These limits apply ONLY
         when waiting for the target temperature to be reached; once
         the call to `set_temperature()` returns, these limits are no
         longer checked.  Since 5.5
 """
-SetFlowCellBarcodeKitRequest.__doc__ = """Attributes:
-    id:
-        The Barcode Kit ID can be up to 8 characters long
+SetCalibrationRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel included in calibration data.  This must
+        always be 1. This is required in order to make sure the client
+        and MinKNOW agree on what data is being provided.
+    last_channel:
+        The last channel included in calibration data.  This must
+        always be the same as the channel count returned by
+        :meth:`get_flow_cell_info`. This is required in order to make
+        sure the client and MinKNOW agree on what data is being
+        provided.
+    offsets:
+        The ADC value adjustment to reach 0pA on each channel.  This
+        is ``-x``, where ``x`` is the (mean) ADC value at 0pA.
+    pa_ranges:
+        The range of possible pA values that can be produced by the
+        device.
 """
-ChannelConfiguration.__doc__ = """Describes the configuration of a channel on the device.  Note that
-this is a lossy representation. The device-specific APIs provide more
-precise information. This only describes common configurations, and
-omits anything that doesn't impact the received signal.
+GetTemperatureResponse.MinIONTemperature.__doc__ = """Packet of temperatures appropriate for a MinION.
 
 Attributes:
-    well:
-        The currently-connected well.  Wells are counted from 1. 0
-        indicates that no well is connected. 5 indicates some non-
-        generic configuration such as ground for a minion or
-        connecting all wells on promethion  Note that MinKNOW can
-        return channel configurations where the well number is larger
-        than the ``max_well_count`` value returned by
-        :meth:`DeviceService.get_device_info`. This indicates that
-        some other connection has been made (for example, PromethIONs
-        can simultaneously connect all wells, and MinIONs can connect
-        to ground).
-    test_current:
-        Whether the test current is connected to the integrator
-        (measurement circuit).  The signal will be a steady test
-        current produced on the device. This can be used for
-        calibration or to test the device integration circuits.
+    asic_temperature:
+        Temperature as measured by the probe inside the asic. This is
+        the "secondary" temperature
+    heatsink_temperature:
+        Temperature as measured by the probe in the minion heatsink.
+        This is the "primary" temperature
+"""
+GetTemperatureResponse.PromethIONTemperature.__doc__ = """Packet of temperatures appropriate for a PromethION.
+
+Attributes:
+    flowcell_temperature:
+        Temperature as measured by thermistor TH2 on the P-Chip. This
+        is the "primary" temperature
+    chamber_temperature:
+        Mean of 12 pixel-blocks temperatures measured with sensors in
+        the ASIC. This is the "secondary" temperature
+"""
+GetChannelConfigurationRequest.__doc__ = """Attributes:
+    channels:
+        A list of channel names (1-indexed) to specify what channels
+        to get channel configs for  Will return an error if any of the
+        channel names are below 1, or above the channel count value
+        returned from :meth:`get_flow_cell_info`
+"""
+SaturationConfig.SoftwareSaturation.__doc__ = """The ranges specify the actual pA or ADC ranges which will trigger
+saturation. This range is checked against the first sample in each
+delivered packet.  software saturation is specified in adc units
+
+Attributes:
+    enabled:
+        Set to enable or disable software saturation.
+    software_min_adc:
+        The minimum adc value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+    software_max_adc:
+        The maximum adc value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+"""
+StreamTemperatureRequest.__doc__ = """Attributes:
+    period_seconds:
+        How often temperature updates should be sent Defaults to a
+        period of 1 second, if not specified, or set to 0
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
+"""
+SetTemperatureRequest.SecondaryTemperatureLimits.__doc__ = """Attributes:
+    min:
+        The minimum permissible "secondary" temperature
+    max:
+        The maximum permissible "secondary" temperature
+"""
+SetTemperatureResponse.__doc__ = """Attributes:
+    timed_out_waiting_for_temperature:
+        Find if we hit a timeout waiting for the temperature to be
+        hit.  Deprecated since 5.5; in favour of the
+        `TIMED_OUT_WAITING_FOR_TEMPERATURE` result code.
+    result:
+        The result of setting the temperature  Since 5.5  NB - before
+        5.5, checking this field will always return a value of
+        `TARGET_TEMPERATURE_SET` The "real" value may be inferred as
+        follows:  - If `wait_for_temperature` was NOT specified, the
+        "real" result is    `TARGET_TEMPERATURE_SET`  - If
+        `wait_for_temperature` was specified, and
+        `timed_out_waiting_for_temperature` is    false, the "real"
+        result is `REACHED_TEMPERATURE`  - If `wait_for_temperature`
+        was specified, and `timed_out_waiting_for_temperature` is
+        true, the "real" result is `TIMED_OUT_WAITING_FOR_TEMPERATURE`
+        - Versions prior to 5.5 do not support setting the secondary
+        temperature limit, and so (for    these versions) the "real"
+        value can never be `SECONDARY_TEMPERATURE_LIMITS_EXCEEDED`
+"""
+UnblockRequest.__doc__ = """Attributes:
+    channels:
+        List of channels indexed from 1.
+    duration:
+        How long should an unblock last.
 """
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/device_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/device_service.py` & `minknow_api-5.9.5/minknow_api/device_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/create_client_certificates.py` & `minknow_api-5.9.5/minknow_api/examples/create_client_certificates.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/export_to_csv.py` & `minknow_api-5.9.5/minknow_api/examples/export_to_csv.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/extract_run_statistics.py` & `minknow_api-5.9.5/minknow_api/examples/extract_run_statistics.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/list_sequencing_positions.py` & `minknow_api-5.9.5/minknow_api/examples/list_sequencing_positions.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/load_sample_sheet.py` & `minknow_api-5.9.5/minknow_api/examples/load_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/manage_simulated_devices.py` & `minknow_api-5.9.5/minknow_api/examples/manage_simulated_devices.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/run_after_protocol.py` & `minknow_api-5.9.5/minknow_api/examples/run_after_protocol.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/examples/start_protocol.py` & `minknow_api-5.9.5/minknow_api/examples/start_protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,62 +188,81 @@
         help="Specify bed file to send to basecaller.",
     )
 
     # Output arguments
     parser.add_argument(
         "--fastq",
         action="store_true",
-        help="enables FastQ file output, defaulting to 4000 reads per file",
+        help="enables FastQ file output.",
     )
 
     parser.add_argument(
         "--fastq-reads-per-file",
         type=int,
-        default=4000,
         help="set the number of reads combined into one FastQ file.",
     )
 
     parser.add_argument(
+        "--fastq-batch-duration",
+        type=int,
+        help="Duration (in seconds) of a single fastq file batch; if set to 0, time-based batching is disabled",
+    )
+
+    parser.add_argument(
         "--fast5",
         action="store_true",
-        help="enables Fast5 file output, defaulting to 4000 reads per file, this will store raw, "
-        "fastq and trace-table data",
+        help="enables Fast5 file output, this will store raw, fastq and trace-table data.",
     )
 
     parser.add_argument(
         "--fast5-reads-per-file",
         type=int,
-        default=4000,
         help="set the number of reads combined into one Fast5 file.",
     )
 
     parser.add_argument(
+        "--fast5-batch-duration",
+        type=int,
+        help="Duration (in seconds) of a single fast5 file batch; if set to 0, time-based batching is disabled",
+    )
+
+    parser.add_argument(
         "--pod5",
         action="store_true",
-        help="enables Pod5 file output, defaulting to 4000 reads per file, this will store raw data.",
+        help="enables Pod5 file output, this will store raw data.",
     )
 
     parser.add_argument(
         "--pod5-reads-per-file",
         type=int,
-        default=4000,
         help="set the number of reads combined into one Pod5 file.",
     )
 
     parser.add_argument(
+        "--pod5-batch-duration",
+        type=int,
+        help="Duration (in seconds) of a single pod5 file batch; if set to 0, time-based batching is disabled",
+    )
+
+    parser.add_argument(
         "--bam",
         action="store_true",
-        help="enables BAM file output, defaulting to 4000 reads per file",
+        help="enables BAM file output.",
     )
 
     parser.add_argument(
         "--bam-reads-per-file",
         type=int,
-        default=4000,
-        help="set the number of reads combined into one BAM file.",
+        help="set the number of reads combined into one bam file.",
+    )
+
+    parser.add_argument(
+        "--bam-batch-duration",
+        type=int,
+        help="Duration (in seconds) of a single bam file batch; if set to 0, time-based batching is disabled",
     )
 
     # Read until
     parser.add_argument(
         "--read-until-reference",
         type=str,
         help="Reference file to use in read until",
@@ -654,15 +673,16 @@
             last_channel=None,
         )
 
     def build_output_arguments(args, name):
         if not getattr(args, name):
             return None
         return protocols.OutputArgs(
-            reads_per_file=getattr(args, "%s_reads_per_file" % name)
+            reads_per_file=getattr(args, "%s_reads_per_file" % name, None),
+            batch_duration=getattr(args, "%s_batch_duration" % name, None),
         )
 
     fastq_arguments = build_output_arguments(args, "fastq")
     fast5_arguments = build_output_arguments(args, "fast5")
     pod5_arguments = build_output_arguments(args, "pod5")
     bam_arguments = build_output_arguments(args, "bam")
```

### Comparing `minknow_api-5.9.1/minknow_api/instance_pb2.py` & `minknow_api-5.9.5/minknow_api/instance_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,23 @@
   _globals['_STREAMINSTANCEACTIVITYRESPONSE']._serialized_end=2698
   _globals['_STREAMINSTANCEACTIVITYRESPONSE_FLOWCELLHEALTH']._serialized_start=2468
   _globals['_STREAMINSTANCEACTIVITYRESPONSE_FLOWCELLHEALTH']._serialized_end=2682
   _globals['_STREAMINSTANCEACTIVITYRESPONSE_FLOWCELLHEALTH_CHANNELSTATEPERCENTAGESENTRY']._serialized_start=2620
   _globals['_STREAMINSTANCEACTIVITYRESPONSE_FLOWCELLHEALTH_CHANNELSTATEPERCENTAGESENTRY']._serialized_end=2682
   _globals['_INSTANCESERVICE']._serialized_start=2701
   _globals['_INSTANCESERVICE']._serialized_end=3857
+OutputDirectories.__doc__ = """Attributes:
+    output:
+        The base output directory. Anything that is output to files is
+        branched from this directory.
+    log:
+        Directory where logs will be stored.
+    reads:
+        Base directory where reads will be outputted.
+"""
 N50.__doc__ = """Attributes:
     n50:
         N50 data, in basecalled bases  This value is only streamed for
         acquisitions where basecalling is enabled.  The latest value
         is sent once per minute
     estimated_n50:
         N50 data, in estimated bases  The latest value is sent once
@@ -136,14 +145,28 @@
         only available if an acquisition with basecalling enabled is
         in progress
 """
 GetMachineIdResponse.__doc__ = """Attributes:
     machine_id:
         The machine_id MinKNOW uses for this host.
 """
+BasecallSpeed.__doc__ = """Attributes:
+    mean_basecall_speed:
+        Mean basecall speed, in bases per second.  This value is only
+        streamed for acquisitions where basecalling is enabled.  The
+        value reported here is the value stored in last completed
+        basecall boxplot bucket Each boxplot bucket covers a duration
+        of `boxplot_time_coverage_in_minutes`
+"""
+StreamDiskSpaceInfoRequest.__doc__ = """Attributes:
+    period:
+        Disk space information will be streamed with this value
+        determining the period in seconds between updates. A period of
+        0 is invalid
+"""
 DeviceInfo.__doc__ = """Attributes:
     device_state:
         The current state of the device
     device_info:
         Information about the connected device (or no content if
         disconnected see: device_state)
 """
@@ -189,31 +212,14 @@
         affect the available features, or the update process.  Since
         4.1
     guppy_build_version:
         Version of guppy MinKNOW was packaged against.  Since 5.0
     guppy_connected_version:
         Version of guppy MinKNOW running with.  Since 5.0
 """
-BasecallSpeed.__doc__ = """Attributes:
-    mean_basecall_speed:
-        Mean basecall speed, in bases per second.  This value is only
-        streamed for acquisitions where basecalling is enabled.  The
-        value reported here is the value stored in last completed
-        basecall boxplot bucket Each boxplot bucket covers a duration
-        of `boxplot_time_coverage_in_minutes`
-"""
-OutputDirectories.__doc__ = """Attributes:
-    output:
-        The base output directory. Anything that is output to files is
-        branched from this directory.
-    log:
-        Directory where logs will be stored.
-    reads:
-        Base directory where reads will be outputted.
-"""
 FilesystemDiskSpaceInfo.__doc__ = """disk-usage information for one file-system
 
 Attributes:
     filesystem_id:
         The name of the file-system
     bytes_available:
         How much space is left on the file-system
@@ -238,14 +244,8 @@
         indicate that bytes_available is decreasing and space is being
         used A value of 0 can indicate that this has not applicable or
         not available.
     file_types_stored:
         A list of what types of file MinKNOW stores on this file-
         system, eg: reads, logs, intermediate-files, etc.
 """
-StreamDiskSpaceInfoRequest.__doc__ = """Attributes:
-    period:
-        Disk space information will be streamed with this value
-        determining the period in seconds between updates. A period of
-        0 is invalid
-"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/instance_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/instance_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/instance_service.py` & `minknow_api-5.9.5/minknow_api/instance_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/keystore_pb2.py` & `minknow_api-5.9.5/minknow_api/keystore_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,33 @@
   _globals['_WATCHREQUEST']._serialized_end=762
   _globals['_WATCHRESPONSE']._serialized_start=765
   _globals['_WATCHRESPONSE']._serialized_end=938
   _globals['_WATCHRESPONSE_VALUESENTRY']._serialized_start=247
   _globals['_WATCHRESPONSE_VALUESENTRY']._serialized_end=314
   _globals['_KEYSTORESERVICE']._serialized_start=1061
   _globals['_KEYSTORESERVICE']._serialized_end=1510
+GetRequest.__doc__ = """Attributes:
+    names:
+        The names of the values you wish to fetch.
+    allow_missing:
+        Whether to allow missing values.  If set, names that are not
+        present in the store will simply be omitted from the response.
+        Otherwise, missing values will cause an error to be returned.
+        Defaults to 'false'
+"""
+RemoveRequest.__doc__ = """Attributes:
+    names:
+        The names of the values you wish to remove.
+    allow_missing:
+        Whether to allow missing values.  If set, names that are not
+        present in the store will be ignored, but any present values
+        will still be removed. Otherwise, missing values will cause an
+        error to be returned (in which case nothing will be removed).
+        Defaults to 'false'
+"""
 GetOneResponse.__doc__ = """Attributes:
     value:
         The requested value.
 """
 WatchRequest.__doc__ = """Attributes:
     send_finished_runs:
         By default, no information will be sent about runs that were
@@ -88,41 +107,18 @@
     allow_missing:
         Whether to allow missing values.  If set, names that are not
         present in the store will be omitted from the first response,
         but will still be watched. If and when they are added, a
         message will be sent with the set values. Otherwise, missing
         values will cause an immediate error.  Defaults to 'false'
 """
-RemoveRequest.__doc__ = """Attributes:
-    names:
-        The names of the values you wish to remove.
-    allow_missing:
-        Whether to allow missing values.  If set, names that are not
-        present in the store will be ignored, but any present values
-        will still be removed. Otherwise, missing values will cause an
-        error to be returned (in which case nothing will be removed).
-        Defaults to 'false'
-"""
 GetOneRequest.__doc__ = """Attributes:
     name:
         The name of the value to fetch.
 """
-GetRequest.__doc__ = """Attributes:
-    names:
-        The names of the values you wish to fetch.
-    allow_missing:
-        Whether to allow missing values.  If set, names that are not
-        present in the store will simply be omitted from the response.
-        Otherwise, missing values will cause an error to be returned.
-        Defaults to 'false'
-"""
-GetResponse.__doc__ = """Attributes:
-    values:
-        The requested values.
-"""
 StoreRequest.__doc__ = """Attributes:
     values:
         The values to store.  See the notes in the KeyStore service
         documentation about names - in short, for any values not
         documented elsewhere, you should be prefixing the name with
         "<product>:", where <product> is the name of your software
         product.
@@ -139,8 +135,12 @@
     values:
         The values that have changed.  The first received message will
         contain the current state of all the watched values.
         Subsequent messages will only contain the values that changed.
     removed_values:
         The values that have been removed.
 """
+GetResponse.__doc__ = """Attributes:
+    values:
+        The requested values.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/keystore_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/keystore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/keystore_service.py` & `minknow_api-5.9.5/minknow_api/keystore_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/log_pb2.py` & `minknow_api-5.9.5/minknow_api/log_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,33 +58,14 @@
   _globals['_SENDPINGRESPONSE']._serialized_end=790
   _globals['_COLLECTPINGSREQUEST']._serialized_start=792
   _globals['_COLLECTPINGSREQUEST']._serialized_end=891
   _globals['_COLLECTPINGSRESPONSE']._serialized_start=893
   _globals['_COLLECTPINGSRESPONSE']._serialized_end=966
   _globals['_LOGSERVICE']._serialized_start=1269
   _globals['_LOGSERVICE']._serialized_end=1665
-GetUserMessagesRequest.__doc__ = """Attributes:
-    include_old_messages:
-        If set, any messages which have already been sent to listeners
-        will be sent to the new stream again, before new messages are
-        sent.  If not specified - the default will not send messages
-        that were sent previously.  note: there is a limit on how many
-        messages are recorded for replay.
-"""
-CollectPingsRequest.__doc__ = """Attributes:
-    collected_ping_file:
-        Any pings that are queued to be sent will be collected into a
-        zip file and written to this location. This location must be
-        in a folder writable by minknow. If the file name does not end
-        with ".zip", minknow will append ".zip" to the provided file
-        name.
-    include_previously_colleced_pings:
-        Normally previously collected pings are ignored, but by
-        setting this they will be included. Defaults to False.
-"""
 SendPingRequest.__doc__ = """Since 5.0
 
 Attributes:
     ping_data:
         The json data to send as a ping.  note: if this string is not
         a valid json object, an error will be raised.
     days_until_expiry:
@@ -100,14 +81,33 @@
         identify the message for translation purposes
     user_message:
         The user message to send to any listeners.
     extra_data:
         Any extra data associated with the user message, as a map from
         key to data.
 """
+GetUserMessagesRequest.__doc__ = """Attributes:
+    include_old_messages:
+        If set, any messages which have already been sent to listeners
+        will be sent to the new stream again, before new messages are
+        sent.  If not specified - the default will not send messages
+        that were sent previously.  note: there is a limit on how many
+        messages are recorded for replay.
+"""
+CollectPingsRequest.__doc__ = """Attributes:
+    collected_ping_file:
+        Any pings that are queued to be sent will be collected into a
+        zip file and written to this location. This location must be
+        in a folder writable by minknow. If the file name does not end
+        with ".zip", minknow will append ".zip" to the provided file
+        name.
+    include_previously_colleced_pings:
+        Normally previously collected pings are ignored, but by
+        setting this they will be included. Defaults to False.
+"""
 UserMessage.__doc__ = """Attributes:
     time:
         Timestamp for when the log message was emitted
     severity:
         The severity of the message
     identifier:
         A short unique textual identifier for the message Used to
```

### Comparing `minknow_api-5.9.1/minknow_api/log_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/log_service.py` & `minknow_api-5.9.5/minknow_api/log_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/manager.py` & `minknow_api-5.9.5/minknow_api/manager.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/manager_pb2.py` & `minknow_api-5.9.5/minknow_api/manager_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -257,31 +257,126 @@
   _globals['_GETFEATURESRESPONSE_STATE']._serialized_end=11409
   _globals['_SETFEATURESREQUEST']._serialized_start=11411
   _globals['_SETFEATURESREQUEST']._serialized_end=11483
   _globals['_SETFEATURESRESPONSE']._serialized_start=11485
   _globals['_SETFEATURESRESPONSE']._serialized_end=11506
   _globals['_MANAGERSERVICE']._serialized_start=11889
   _globals['_MANAGERSERVICE']._serialized_end=15918
-CreateDirectoryResponse.__doc__ = """Attributes:
-    path:
-        The path to the created directory.
+GetFlowCellTypesResponse.__doc__ = """Response message for `ManagerService.get_flow_cell_types`.
+
+Attributes:
+    types:
+        The flow cell types.
+"""
+GetFlowCellTypesResponse.Info.__doc__ = """Information about a flow cell type.
+
+Attributes:
+    product_code:
+        The product code for the flow cell type.  This is the user-
+        visible name for the flow cell type. It is the name used to
+        order flow cells, and is also displayed on the packaging.
+        While most product codes are 10 characters, be aware that
+        longer product codes can exist and have been used in the past.
+        Example: "FLO-MIN106".
+    connector_type:
+        The connector type of this flow cell type.  This determines
+        which flow cell positions it is possible to insert this flow
+        cell into. The connector type for a given flow cell position
+        can be determined using
+        `minknow_api.device.DeviceService.get_device_state`.  This
+        will never be ``FCCON_NOT_SET``.
+    cannot_live_basecall:
+        Indicates that live basecalling is not possible on the flow
+        cell.  Note that almost all flow cell types can be basecalled
+        on: that is why this indicates a negative (saving some bytes
+        on the wire by allowing the common case of basecalling being
+        possible to be omitted entirely).
+"""
+CreateDeveloperApiTokenResponse.__doc__ = """Attributes:
+    id:
+        Unique ID assigned to the token for identification purposes.
+        Not valid as an authentication token.
+    token:
+        Created token, available to be used with minknow API's
+        immediately.
 """
 GetLampKitInfoResponse.__doc__ = """Attributes:
     lamp_kits:
         Lamp kit names
 """
-GetSequencingKitsResponse.__doc__ = """Response message for `ManagerService.get_sequencing_kits`.
+FlowCellPosition.RpcPorts.__doc__ = """Attributes:
+    secure:
+        A port providing the standard gRPC protocol over TLS
+    secure_grpc_web:
+        A port providing the gRPC-Web protocol over TLS
+"""
+GetAlignmentReferenceInformationResponse.__doc__ = """Attributes:
+    estimated_load_time_seconds:
+        Estimated load time of the reference in seconds.
+    estimated_reference_size_bases:
+        Estimated size of the reference file in bases.
+    recommended_live_usage:
+        Does the reference file fit within the recommended live usage
+        memory size?  This uses an estimate of how much memory a
+        reference may use when running in guppy and compares to the
+        amount of memory in the sequencer. It does not account for
+        whether the reference will run in real time.
+"""
+RemoveSimulatedDeviceRequest.__doc__ = """Attributes:
+    name:
+        The name of the simulated device to be removed
+"""
+FindProtocolsResponse.Protocol.__doc__ = """Attributes:
+    identifier:
+        An identifying string for protocol, of the form:
+        LOCATION:relative/path/to/protocol  The identifier uniquely
+        identifies the protocol.
+    requires_flow_cell_product_code:
+        Whether the protocol requires a flow cell product code in
+        order to start.
+    requires_sequencing_kit:
+        Whether the protocol requires a sequencing kit in order to
+        start.
+"""
+ResetPositionRequest.__doc__ = """Attributes:
+    positions:
+        The names of positions to restart.
+    force:
+        Force the software to be restarted even when it appears to be
+        in a healthy state (ie: STATE_RUNNING).
+"""
+AssociationDeviceCodeRequest.__doc__ = """Offline association is now the default workflow  The following are
+therefore reserved/deprecated
 
 Attributes:
-    kits:
-        The known sequencing kits.
-    barcoding_expansion_kits:
-        The possible barcoding expansion kits.  These are kits that
-        can be used in combination with certain sequencing kits to add
-        (or extend) barcoding functionality.
+    position_name:
+        The flow cell position to get the association code/key for.
+        If this is omitted, the code/key for the sequencing device as
+        a whole is returned.  Note that this cannot be omitted if
+        MinKNOW is installed on a PC (as opposed to a sequencing
+        device). It should be omitted if (and only if) the data
+        returned from `describe_host` has its ``needs_association``
+        field set to true.  Passing a integrated flow cell position
+        will return the code/key for the whole sequencing device.
+"""
+CreateDirectoryResponse.__doc__ = """Attributes:
+    path:
+        The path to the created directory.
+"""
+FlowCellPositionsResponse.__doc__ = """Attributes:
+    total_count:
+        How many positions are available in total.  This is the same
+        in every message returned from a single call, and allows the
+        caller to easily see how many further positions might be in
+        subsequent messages.
+    positions:
+        Known flow cell positions.  Note that not all positions listed
+        here are necessarily available. In particular, integrated flow
+        cell positions (eg: on GridIONs or PromethIONs) will always be
+        listed.
 """
 DescribeHostResponse.__doc__ = """Attributes:
     product_code:
         The product code for the host, if applicable.  If this is an
         integrated Oxford Nanopore device, this will be the product
         code of the device, or the part of the device that runs
         MinKNOW (eg: several PromethION models have separate product
@@ -328,209 +423,14 @@
         sequencing devices can sequence without an internet
         connection. This indicates whether it is possible for the
         integrated sequencing positions. Note that this will only be
         set if `needs_association` is true.  Since 4.4
     can_basecall:
         Whether the device can currently provide basecalling
 """
-CreateDeveloperApiTokenResponse.__doc__ = """Attributes:
-    id:
-        Unique ID assigned to the token for identification purposes.
-        Not valid as an authentication token.
-    token:
-        Created token, available to be used with minknow API's
-        immediately.
-"""
-FeatureList.__doc__ = """Attributes:
-    feature_flags:
-        feature_flags is a special value  If false, turns off all
-        other feature flags If true, allows individual flags to be
-        enabled and disabled
-"""
-GetBarcodeKeysResponse.__doc__ = """Attributes:
-    barcode_keys:
-        Returned barcode keys.
-    lamp_keys:
-        Returned lamp barcode ids.
-    combined_keys:
-        Combined barcode and lamp keys.  Returned keys are joined
-        strings of all requested barcode kits, giving the caller a
-        unique string to identify each barcode pair.  eg. if both a
-        lamp kit + barcode kit are specified, NxM barcode keys are
-        returned:  - barcode01_lamp01  - barcode01_lamp02  -
-        barcode01_lamp03  - barcode02_lamp01  - barcode02_lamp02  -
-        barcode02_lamp03
-"""
-GetAlignmentReferenceInformationRequest.__doc__ = """Attributes:
-    path:
-        The full path of the alignment reference.  Should be a .fasta,
-        or .mmi file.
-"""
-FlowCellPosition.RpcPorts.__doc__ = """Attributes:
-    secure:
-        A port providing the standard gRPC protocol over TLS
-    secure_grpc_web:
-        A port providing the gRPC-Web protocol over TLS
-"""
-AssociationDeviceCodeRequest.__doc__ = """Offline association is now the default workflow  The following are
-therefore reserved/deprecated
-
-Attributes:
-    position_name:
-        The flow cell position to get the association code/key for.
-        If this is omitted, the code/key for the sequencing device as
-        a whole is returned.  Note that this cannot be omitted if
-        MinKNOW is installed on a PC (as opposed to a sequencing
-        device). It should be omitted if (and only if) the data
-        returned from `describe_host` has its ``needs_association``
-        field set to true.  Passing a integrated flow cell position
-        will return the code/key for the whole sequencing device.
-"""
-ListSettingsForProtocolResponse.__doc__ = """Attributes:
-    protocol_settings:
-        Any protocol settings not covered by the above structures, for
-        example those required for custom-scripts.
-"""
-ListSettingsForProtocolRequest.__doc__ = """Attributes:
-    identifier:
-        specify the protocol with a string containing all the
-        protocol's identifying components, eg:
-        "sequencing/sequencing_MIN106_DNA:FLO-MIN106:SQK-RPB004"
-    components:
-        specify the protocol providing the identifying components
-        individually. All components are optional, if more than one
-        protocol matches given strings, information about the first
-        will be returned.
-    flow_cell_connector:
-        The flow-cell connector type identifies the type of hardware
-        and is used to identify the correct protocol. The flow-cell
-        connector types applicable to the device are listed by the
-        get_flow_cell_types rpc in this service and the
-        get_device_state rpc in the device service.
-"""
-FindProtocolsResponse.Protocol.__doc__ = """Attributes:
-    identifier:
-        An identifying string for protocol, of the form:
-        LOCATION:relative/path/to/protocol  The identifier uniquely
-        identifies the protocol.
-    requires_flow_cell_product_code:
-        Whether the protocol requires a flow cell product code in
-        order to start.
-    requires_sequencing_kit:
-        Whether the protocol requires a sequencing kit in order to
-        start.
-"""
-CreateDeveloperApiTokenRequest.__doc__ = """Attributes:
-    name:
-        User facing name describing the token.
-    expiry:
-        Optional expiry time for the token.
-"""
-RevokeDeveloperApiTokenRequest.__doc__ = """Attributes:
-    id:
-        The id passed back from [CreateDeveloperApiTokenRequest] or
-        [DeveloperApiToken].
-"""
-ListSettingsForProtocolResponse.RunOptions.__doc__ = """Run options
-
-Attributes:
-    active_channel_selection:
-         bool
-    mux_scan_period:
-         in hours
-"""
-GetAlignmentReferenceInformationResponse.__doc__ = """Attributes:
-    estimated_load_time_seconds:
-        Estimated load time of the reference in seconds.
-    estimated_reference_size_bases:
-        Estimated size of the reference file in bases.
-    recommended_live_usage:
-        Does the reference file fit within the recommended live usage
-        memory size?  This uses an estimate of how much memory a
-        reference may use when running in guppy and compares to the
-        amount of memory in the sequencer. It does not account for
-        whether the reference will run in real time.
-"""
-AddSimulatedDeviceRequest.__doc__ = """Attributes:
-    name:
-        The name of the position, this must be unique and the correct
-        format:  For MinION Mk1B and Mk1C: "MS" followed by five
-        digits, eg: "MS12345". For GridION: "GS" followed by five
-        digits, eg: "GS12345". For P2 Solo: "P2S_" followed by five
-        digits, and then "-A" or "-B" eg: "P2S_12345-A".  PromethION
-        and P2 Solo position-names have no format restriction, but
-        must be unique. It is strongly recommended to follow standard
-        naming conventions:  For PromethION: start with "1A" and then
-        increase the number and/or the letter as you add more
-        positions. For P2 Solo: use "P2S_00000-A" and "P2S_00000-B"
-        (these fit the format of real P2 Solo devices, but do not
-        correspond to any real device).  Future versions might
-        constrain PromethION and P2 Solo device names. Using the above
-        suggestions should ensure that your code will continue to
-        work.  Note that MinKNOW Core 5.5 and earlier required the P2
-        Solo device name to be "P2S" followed by four digits. This is
-        no longer recommended.
-    type:
-        The type of the simulated device to create.  If left at
-        default (AUTO), then a sensible default device type is
-        selected.
-"""
-GetFlowCellTypesResponse.__doc__ = """Response message for `ManagerService.get_flow_cell_types`.
-
-Attributes:
-    types:
-        The flow cell types.
-"""
-FlowCellPosition.Location.__doc__ = """Attributes:
-    x:
-        The column (counting from 0, left-to-right) of the flow cell
-        position on the sequencing unit when viewed from above/in
-        front.
-    y:
-        The row (counting from 0, top-to-bottom) of the flow cell
-        position on the sequencing unit when viewed from above/in
-        front.
-"""
-BasecallerApiResponse.__doc__ = """Attributes:
-    secure:
-        The port to use to access the minknow_api.basecaller API using
-        the standard gRPC protocol over TLS
-    secure_grpc_web:
-        The port to use to access the minknow_api.basecaller API using
-        the gRPC-Web protocol over TLS
-"""
-CreateDirectoryRequest.__doc__ = """Attributes:
-    parent_path:
-        The path at which to create the directory.  This must exist,
-        be a directory, and be within the protocol output directory.
-        This can be determined via calls to
-        list_protocol_output_dir_files().
-    name:
-        The name of the directory to create.  This must be a single
-        path component (ie: it cannot contain '/' or '\'). There may
-        be other restrictions on valid characters, depending on the
-        operating system.
-"""
-LocalAuthenticationTokenPathResponse.__doc__ = """Attributes:
-    path:
-        The full path of the local authentication token
-"""
-ListSettingsForProtocolResponse.Output.__doc__ = """Output
-
-Attributes:
-    read_filtering_min_duplex_qscore:
-        Since 5.8
-"""
-AssociationDeviceCodeResponse.__doc__ = """Attributes:
-    code:
-        The code required to associate the device with an account.  If
-        the request had `offline` set, this code is suitable for use
-        in the customer portal offline association page. Otherwise, it
-        is suitable for the online association APIs.
-"""
 WatchFlowCellPositionsResponse.__doc__ = """Each flow cell position will first be listed in `additions`. After
 that, it may appear in `changes` in zero or more messages. Then, it
 may appear in `removals` once, after which it will either never appear
 again, or appear in `additions` again (restarting the cycle).  No
 position will ever appear in more than one field in the same response
 message.
 
@@ -549,68 +449,35 @@
         provided in `additions`.
     removals:
         A flow cell position has been removed.  Note that this can
         only happen with MinIONs - integrated flow cell positions are
         never removed (if they become unavailable, this will be noted
         in the `changes` field).
 """
-StreamDiskSpaceInfoRequest.__doc__ = """Attributes:
-    period:
-        Disk space information will be streamed with this value
-        determining the period in seconds between updates. A period of
-        0 is invalid
-"""
-GetGuppyInfoResponse.__doc__ = """Attributes:
-    port:
-        The port Guppy is listening on.
-    ipc_path:
-        The path to an ipc file Guppy is using. Use "ipc://<ipc_path>"
-        for a guppy connection string.
-    version:
-        The Guppy server version.
-"""
-GetFlowCellTypesResponse.Info.__doc__ = """Information about a flow cell type.
-
-Attributes:
-    product_code:
-        The product code for the flow cell type.  This is the user-
-        visible name for the flow cell type. It is the name used to
-        order flow cells, and is also displayed on the packaging.
-        While most product codes are 10 characters, be aware that
-        longer product codes can exist and have been used in the past.
-        Example: "FLO-MIN106".
-    connector_type:
-        The connector type of this flow cell type.  This determines
-        which flow cell positions it is possible to insert this flow
-        cell into. The connector type for a given flow cell position
-        can be determined using
-        `minknow_api.device.DeviceService.get_device_state`.  This
-        will never be ``FCCON_NOT_SET``.
-    cannot_live_basecall:
-        Indicates that live basecalling is not possible on the flow
-        cell.  Note that almost all flow cell types can be basecalled
-        on: that is why this indicates a negative (saving some bytes
-        on the wire by allowing the common case of basecalling being
-        possible to be omitted entirely).
+GetBasecallerFeaturesResponse.__doc__ = """Attributes:
+    is_live_basecalling_with_adaptive_sampling_recommended:
+        Is live basecalling with adaptive sampling recommended on this
+        hardware Currently not recommended for Apple or Mk1C  Since
+        5.9
 """
-FindProtocolsResponse.__doc__ = """Attributes:
-    protocols:
-        Protocols available for starting.
+ApplyOfflineAssociationUnlockCodeRequest.__doc__ = """Attributes:
+    position_name:
+        The flow cell position to unlock.  This should be set (or not
+        set) to match the corresponding call to
+        `offline_association_device_code`.
+    unlock_code:
+        The unlock code provided by the user.  This the code given by
+        the customer support portal when the corresponding device code
+        is entered into the device association page.
 """
-FlowCellPositionsResponse.__doc__ = """Attributes:
-    total_count:
-        How many positions are available in total.  This is the same
-        in every message returned from a single call, and allows the
-        caller to easily see how many further positions might be in
-        subsequent messages.
-    positions:
-        Known flow cell positions.  Note that not all positions listed
-        here are necessarily available. In particular, integrated flow
-        cell positions (eg: on GridIONs or PromethIONs) will always be
-        listed.
+FeatureList.__doc__ = """Attributes:
+    feature_flags:
+        feature_flags is a special value  If false, turns off all
+        other feature flags If true, allows individual flags to be
+        enabled and disabled
 """
 GetSequencingKitsResponse.Kit.__doc__ = """Information about a sequencing kit.
 
 Attributes:
     product_code:
         The product code for the sequencing kit.  This is the user-
         visible name for the kit. It is the name used to order kits,
@@ -648,30 +515,183 @@
         The kit can be used with RNA samples.
     pcr:
         The kit can be used with samples that have had PCR applied to
         them.
     pcr_free:
         The kit can be used without a PCR step.
 """
-GetFlowCellTypesRequest.__doc__ = """Request message for `ManagerService.get_flow_cell_types`."""
-ApplyOfflineAssociationUnlockCodeRequest.__doc__ = """Attributes:
-    position_name:
-        The flow cell position to unlock.  This should be set (or not
-        set) to match the corresponding call to
-        `offline_association_device_code`.
-    unlock_code:
-        The unlock code provided by the user.  This the code given by
-        the customer support portal when the corresponding device code
-        is entered into the device association page.
-"""
 ApplyOfflineAssociationUnlockCodeResponse.__doc__ = """Attributes:
     associated:
         True if the association was successful (the unlock_code was
         accepted), false otherwise.
 """
+FindProtocolsRequest.__doc__ = """Attributes:
+    flow_cell_product_code:
+        Find protocols that are compatible with this flow cell product
+        code.  Set to empty string to find protocols matching all flow
+        cell product codes.
+    sequencing_kit:
+        Limit to protocols that are compatible with this sequencing
+        kit.  Set to empty string to find protocols matching all kits.
+    experiment_type:
+        Limit response to certain protocol types.
+"""
+GetBarcodeKeysResponse.__doc__ = """Attributes:
+    barcode_keys:
+        Returned barcode keys.
+    lamp_keys:
+        Returned lamp barcode ids.
+    combined_keys:
+        Combined barcode and lamp keys.  Returned keys are joined
+        strings of all requested barcode kits, giving the caller a
+        unique string to identify each barcode pair.  eg. if both a
+        lamp kit + barcode kit are specified, NxM barcode keys are
+        returned:  - barcode01_lamp01  - barcode01_lamp02  -
+        barcode01_lamp03  - barcode02_lamp01  - barcode02_lamp02  -
+        barcode02_lamp03
+"""
+ListProtocolOutputDirFilesRequest.__doc__ = """Attributes:
+    path:
+        Specify the root path to list files from. If the path is left
+        empty, then the base protocol output directory will be used.
+        Note that the path specified HAS to be a descendant of the
+        protocol output directory, otherwise a INVALID_ARGUMENT error
+        will be returned  If the path is left empty, and the path
+        specified in the user config doesn't exist, then the NOT_FOUND
+        error code will be returned
+"""
+FilesystemDiskSpaceInfo.__doc__ = """disk-usage information for one file-system
+
+Attributes:
+    filesystem_id:
+        The name of the file-system
+    bytes_available:
+        How much space is left on the file-system
+    bytes_capacity:
+        The total capacity of the file-system when empty.
+    what:
+        A list of what MinKNOW stores on this file-system, eg: reads,
+        logs, intermediate-files
+    bytes_to_stop_cleanly:
+        MinKNOW needs this much space to stop experiments. If
+        bytes_available goes below this number, data could be lost!
+    bytes_when_alert_issued:
+        The amount of space left on the file-system when
+        recommend_alert was set true.
+    recommend_alert:
+        MinKNOW recommends that you alert someone about the disk-usage
+    recommend_stop:
+        MinKNOW recommends that you stop experiments due to disk-usage
+        concerns
+    bytes_per_second:
+        Rate of change in bytes_available (per second) +'ve numbers
+        indicate that bytes_available is decreasing and space is being
+        used A value of 0 can indicate that this has not applicable or
+        not available.
+    file_types_stored:
+        A list of what types of file MinKNOW stores on this file-
+        system, eg: reads, logs, intermediate-files, etc.
+"""
+ListProtocolOutputDirFilesResponse.__doc__ = """Attributes:
+    directories:
+        List of sub-directories in the directory specified
+    files:
+        List of files in the directory specified
+    current_listed_path:
+        The absolute directory that is being listed within this
+        response
+"""
+AddSimulatedDeviceRequest.__doc__ = """Attributes:
+    name:
+        The name of the position, this must be unique and the correct
+        format:  For MinION Mk1B and Mk1C: "MS" followed by five
+        digits, eg: "MS12345". For GridION: "GS" followed by five
+        digits, eg: "GS12345". For P2 Solo: "P2S_" followed by five
+        digits, and then "-A" or "-B" eg: "P2S_12345-A".  PromethION
+        and P2 Solo position-names have no format restriction, but
+        must be unique. It is strongly recommended to follow standard
+        naming conventions:  For PromethION: start with "1A" and then
+        increase the number and/or the letter as you add more
+        positions. For P2 Solo: use "P2S_00000-A" and "P2S_00000-B"
+        (these fit the format of real P2 Solo devices, but do not
+        correspond to any real device).  Future versions might
+        constrain PromethION and P2 Solo device names. Using the above
+        suggestions should ensure that your code will continue to
+        work.  Note that MinKNOW Core 5.5 and earlier required the P2
+        Solo device name to be "P2S" followed by four digits. This is
+        no longer recommended.
+    type:
+        The type of the simulated device to create.  If left at
+        default (AUTO), then a sensible default device type is
+        selected.
+"""
+ListSettingsForProtocolResponse.RunOptions.__doc__ = """Run options
+
+Attributes:
+    active_channel_selection:
+         bool
+    mux_scan_period:
+         in hours
+"""
+GetBarcodeKitInfoResponse.__doc__ = """Attributes:
+    barcode_kit_info:
+        Map of barcode kit name to barcode kit info
+"""
+GetAlignmentReferenceInformationRequest.__doc__ = """Attributes:
+    path:
+        The full path of the alignment reference.  Should be a .fasta,
+        or .mmi file.
+"""
+GetBarcodeKeysRequest.__doc__ = """Attributes:
+    barcode_kit_names:
+        Names of barcode kits to obtain barcode names for  Fails with
+        INVALID_ARGUMENT if any of the requested `barcode_kit_names`
+        are unavailable
+    lamp_kit_name:
+        Name of lamp kit to obtain barcode names for.  Fails with
+        INVALID_ARGUMENT if the requested `lamp_kit_name` is
+        unavailable.
+"""
+ListSettingsForProtocolResponse.__doc__ = """Attributes:
+    protocol_settings:
+        Any protocol settings not covered by the above structures, for
+        example those required for custom-scripts.
+"""
+AssociationDeviceCodeResponse.__doc__ = """Attributes:
+    code:
+        The code required to associate the device with an account.  If
+        the request had `offline` set, this code is suitable for use
+        in the customer portal offline association page. Otherwise, it
+        is suitable for the online association APIs.
+"""
+GetFlowCellTypesRequest.__doc__ = """Request message for `ManagerService.get_flow_cell_types`."""
+LocalAuthenticationTokenPathResponse.__doc__ = """Attributes:
+    path:
+        The full path of the local authentication token
+"""
+CreateDirectoryRequest.__doc__ = """Attributes:
+    parent_path:
+        The path at which to create the directory.  This must exist,
+        be a directory, and be within the protocol output directory.
+        This can be determined via calls to
+        list_protocol_output_dir_files().
+    name:
+        The name of the directory to create.  This must be a single
+        path component (ie: it cannot contain '/' or '\'). There may
+        be other restrictions on valid characters, depending on the
+        operating system.
+"""
+BasecallerApiResponse.__doc__ = """Attributes:
+    secure:
+        The port to use to access the minknow_api.basecaller API using
+        the standard gRPC protocol over TLS
+    secure_grpc_web:
+        The port to use to access the minknow_api.basecaller API using
+        the gRPC-Web protocol over TLS
+"""
 FlowCellPosition.__doc__ = """Attributes:
     name:
         The name of the position.  For MinIONs, this is the name of
         the MinION (eg: MN12345). For integrated positions, this is
         the label for the position on the sequencer (eg: X1 for
         GridION, 1-A1-D1 for PromethION).
     location:
@@ -730,139 +750,119 @@
     parent_name:
         The name of the device this flow cell position is part of.
         For an integrated position, this will be the host serial, as
         returned by describe_host().  For a MinION Mk1B, this will be
         the same as the `name` field.  For a P2 Solo, this will be the
         name of the P2 Solo unit.  Since 5.3
 """
-GetBarcodeKitInfoResponse.__doc__ = """Attributes:
-    barcode_kit_info:
-        Map of barcode kit name to barcode kit info
-"""
-ListProtocolOutputDirFilesRequest.__doc__ = """Attributes:
-    path:
-        Specify the root path to list files from. If the path is left
-        empty, then the base protocol output directory will be used.
-        Note that the path specified HAS to be a descendant of the
-        protocol output directory, otherwise a INVALID_ARGUMENT error
-        will be returned  If the path is left empty, and the path
-        specified in the user config doesn't exist, then the NOT_FOUND
-        error code will be returned
-"""
-Feature.__doc__ = """Attributes:
-    enabled:
-        Enable or disable the feature
-"""
 ListDeveloperApiTokensResponse.DeveloperApiToken.__doc__ = """Attributes:
     id:
         Unique ID assigned to the token.
     name:
         User facing name describing the token (guaranteed unique
         across tokens).
     expiry:
         Optional expiry of the token.
 """
-RemoveSimulatedDeviceRequest.__doc__ = """Attributes:
-    name:
-        The name of the simulated device to be removed
-"""
-ListProtocolOutputDirFilesResponse.__doc__ = """Attributes:
-    directories:
-        List of sub-directories in the directory specified
-    files:
-        List of files in the directory specified
-    current_listed_path:
-        The absolute directory that is being listed within this
-        response
-"""
-ResetPositionRequest.__doc__ = """Attributes:
-    positions:
-        The names of positions to restart.
-    force:
-        Force the software to be restarted even when it appears to be
-        in a healthy state (ie: STATE_RUNNING).
-"""
 GetSequencingKitsRequest.__doc__ = """Request message for `ManagerService.get_sequencing_kits`.
 
 Attributes:
     flow_cell_product_code:
         The product code of the flow cell that will be used for
         sequencing.  Only kits compatible with this flow cell type
         will be returned (currently, this means that there is at least
         one (sequencing or control) protocol that is compatible with
         both the kit and this flow cell product code).  This may also
         affect the returned information about the kit. For example, if
         it isn't possible to basecall on the flow cell, none of the
         kits will claim to be barcoding capable (or compatible with
         any barcoding expansion kits).
 """
-FindProtocolsRequest.__doc__ = """Attributes:
-    flow_cell_product_code:
-        Find protocols that are compatible with this flow cell product
-        code.  Set to empty string to find protocols matching all flow
-        cell product codes.
-    sequencing_kit:
-        Limit to protocols that are compatible with this sequencing
-        kit.  Set to empty string to find protocols matching all kits.
-    experiment_type:
-        Limit response to certain protocol types.
+Feature.__doc__ = """Attributes:
+    enabled:
+        Enable or disable the feature
+"""
+GetGuppyInfoResponse.__doc__ = """Attributes:
+    port:
+        The port Guppy is listening on.
+    ipc_path:
+        The path to an ipc file Guppy is using. Use "ipc://<ipc_path>"
+        for a guppy connection string.
+    version:
+        The Guppy server version.
 """
 GetSequencingKitsResponse.BarcodingExpansionKit.__doc__ = """Information about a barcoding expansion kit.  In the future, this may
 include compatibility information for dual barcoding, for example.
 
 Attributes:
     product_code:
         The product code for the barcoding expansion kit.  This is the
         user-visible name for the kit. It is the name used to order
         kits, and is also displayed on the packaging.  While most
         product codes are 10 characters, be aware that longer product
         codes can exist.  Example: "EXP-NBD104".
 """
-FilesystemDiskSpaceInfo.__doc__ = """disk-usage information for one file-system
+RevokeDeveloperApiTokenRequest.__doc__ = """Attributes:
+    id:
+        The id passed back from [CreateDeveloperApiTokenRequest] or
+        [DeveloperApiToken].
+"""
+ListSettingsForProtocolResponse.Output.__doc__ = """Output
 
 Attributes:
-    filesystem_id:
-        The name of the file-system
-    bytes_available:
-        How much space is left on the file-system
-    bytes_capacity:
-        The total capacity of the file-system when empty.
-    what:
-        A list of what MinKNOW stores on this file-system, eg: reads,
-        logs, intermediate-files
-    bytes_to_stop_cleanly:
-        MinKNOW needs this much space to stop experiments. If
-        bytes_available goes below this number, data could be lost!
-    bytes_when_alert_issued:
-        The amount of space left on the file-system when
-        recommend_alert was set true.
-    recommend_alert:
-        MinKNOW recommends that you alert someone about the disk-usage
-    recommend_stop:
-        MinKNOW recommends that you stop experiments due to disk-usage
-        concerns
-    bytes_per_second:
-        Rate of change in bytes_available (per second) +'ve numbers
-        indicate that bytes_available is decreasing and space is being
-        used A value of 0 can indicate that this has not applicable or
-        not available.
-    file_types_stored:
-        A list of what types of file MinKNOW stores on this file-
-        system, eg: reads, logs, intermediate-files, etc.
+    read_filtering_min_duplex_qscore:
+        Since 5.8
 """
-GetBasecallerFeaturesResponse.__doc__ = """Attributes:
-    is_live_basecalling_with_adaptive_sampling_recommended:
-        Is live basecalling with adaptive sampling recommended on this
-        hardware Currently not recommended for Apple or Mk1C  Since
-        5.9
+StreamDiskSpaceInfoRequest.__doc__ = """Attributes:
+    period:
+        Disk space information will be streamed with this value
+        determining the period in seconds between updates. A period of
+        0 is invalid
 """
-GetBarcodeKeysRequest.__doc__ = """Attributes:
-    barcode_kit_names:
-        Names of barcode kits to obtain barcode names for  Fails with
-        INVALID_ARGUMENT if any of the requested `barcode_kit_names`
-        are unavailable
-    lamp_kit_name:
-        Name of lamp kit to obtain barcode names for.  Fails with
-        INVALID_ARGUMENT if the requested `lamp_kit_name` is
-        unavailable.
+CreateDeveloperApiTokenRequest.__doc__ = """Attributes:
+    name:
+        User facing name describing the token.
+    expiry:
+        Optional expiry time for the token.
+"""
+ListSettingsForProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        specify the protocol with a string containing all the
+        protocol's identifying components, eg:
+        "sequencing/sequencing_MIN106_DNA:FLO-MIN106:SQK-RPB004"
+    components:
+        specify the protocol providing the identifying components
+        individually. All components are optional, if more than one
+        protocol matches given strings, information about the first
+        will be returned.
+    flow_cell_connector:
+        The flow-cell connector type identifies the type of hardware
+        and is used to identify the correct protocol. The flow-cell
+        connector types applicable to the device are listed by the
+        get_flow_cell_types rpc in this service and the
+        get_device_state rpc in the device service.
+"""
+FindProtocolsResponse.__doc__ = """Attributes:
+    protocols:
+        Protocols available for starting.
+"""
+FlowCellPosition.Location.__doc__ = """Attributes:
+    x:
+        The column (counting from 0, left-to-right) of the flow cell
+        position on the sequencing unit when viewed from above/in
+        front.
+    y:
+        The row (counting from 0, top-to-bottom) of the flow cell
+        position on the sequencing unit when viewed from above/in
+        front.
+"""
+GetSequencingKitsResponse.__doc__ = """Response message for `ManagerService.get_sequencing_kits`.
+
+Attributes:
+    kits:
+        The known sequencing kits.
+    barcoding_expansion_kits:
+        The possible barcoding expansion kits.  These are kits that
+        can be used in combination with certain sequencing kits to add
+        (or extend) barcoding functionality.
 """
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/manager_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/manager_service.py` & `minknow_api-5.9.5/minknow_api/manager_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/minion_device_pb2.py` & `minknow_api-5.9.5/minknow_api/minion_device_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,21 +70,57 @@
   _globals['_GETSETTINGSRESPONSE']._serialized_end=3602
   _globals['_GETFANSPEEDREQUEST']._serialized_start=3604
   _globals['_GETFANSPEEDREQUEST']._serialized_end=3624
   _globals['_GETFANSPEEDRESPONSE']._serialized_start=3626
   _globals['_GETFANSPEEDRESPONSE']._serialized_end=3660
   _globals['_MINIONDEVICESERVICE']._serialized_start=3663
   _globals['_MINIONDEVICESERVICE']._serialized_end=4042
+SamplingFrequencyParameters.__doc__ = """These values control the sampling frequency.
+
+Attributes:
+    clock_divider:
+        Clock divider.  Values over 31 cannot be set.
+    integration_time:
+        The time spent sampling a data point, in microseconds.  Must
+        be between 30 and 1023 (inclusive).  Note that setting the
+        integration_time to less than 50 will force the
+        sinc_decimation value to 32.
+    clock_speed:
+        The speed of the high-speed clock.
+"""
+ChangeSettingsRequest.__doc__ = """Attributes:
+    settings:
+        MinION device settings
+    channel_config_default:
+        The default channel configuration.  This provides the default
+        configuration to apply to any channels not listed in
+        settings.channel_config.
+"""
 GetSettingsResponse.__doc__ = """Response for MinionDeviceService.get_settings
 
 Attributes:
     settings:
         MinION device settings
 """
-GetSettingsRequest.__doc__ = """Request for MinionDeviceService.get_settings"""
+TemperatureRange.__doc__ = """Temperature range.
+
+Attributes:
+    min:
+        The minimum temperature in degrees Celsius.  If temperature
+        control is enabled, the device will attempt to keep its
+        temperature at or above this value.  Must be less than or
+        equal to max.  When soft temperature control is enabled, this
+        value is not used.
+    max:
+        The maximum temperature in degrees Celsius.  If temperature
+        control is enabled, the device will attempt to keep its
+        temperature at or below this value.  Must be less than or
+        equal to min.  When soft temperature control is enabled, this
+        is used as the target temperature, and ``min`` is not used.
+"""
 MinionDeviceSettings.__doc__ = """Describes the MinION device settings.  Both unset structures and
 *_KEEP values in enums indicate "no change". When changing settings,
 these are the default values.
 
 Attributes:
     bias_voltage:
         The voltage potential to be applied across the wells (in
@@ -240,45 +276,9 @@
     bias_voltage_lookup_table:
         The bias voltage lookup table.  If no entries are provided,
         the existing lookup table (if any) is preserved.  See
         ``enable_bias_voltage_lookup``.  Up to 75 values can be
         provided. The values have the same constraints as
         ``bias_voltage``.
 """
-ChangeSettingsRequest.__doc__ = """Attributes:
-    settings:
-        MinION device settings
-    channel_config_default:
-        The default channel configuration.  This provides the default
-        configuration to apply to any channels not listed in
-        settings.channel_config.
-"""
-TemperatureRange.__doc__ = """Temperature range.
-
-Attributes:
-    min:
-        The minimum temperature in degrees Celsius.  If temperature
-        control is enabled, the device will attempt to keep its
-        temperature at or above this value.  Must be less than or
-        equal to max.  When soft temperature control is enabled, this
-        value is not used.
-    max:
-        The maximum temperature in degrees Celsius.  If temperature
-        control is enabled, the device will attempt to keep its
-        temperature at or below this value.  Must be less than or
-        equal to min.  When soft temperature control is enabled, this
-        is used as the target temperature, and ``min`` is not used.
-"""
-SamplingFrequencyParameters.__doc__ = """These values control the sampling frequency.
-
-Attributes:
-    clock_divider:
-        Clock divider.  Values over 31 cannot be set.
-    integration_time:
-        The time spent sampling a data point, in microseconds.  Must
-        be between 30 and 1023 (inclusive).  Note that setting the
-        integration_time to less than 50 will force the
-        sinc_decimation value to 32.
-    clock_speed:
-        The speed of the high-speed clock.
-"""
+GetSettingsRequest.__doc__ = """Request for MinionDeviceService.get_settings"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/minion_device_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/minion_device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/minion_device_service.py` & `minknow_api-5.9.5/minknow_api/minion_device_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/post_processing_protocol_connection.py` & `minknow_api-5.9.5/minknow_api/post_processing_protocol_connection.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/promethion_device_pb2.py` & `minknow_api-5.9.5/minknow_api/promethion_device_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -112,116 +112,57 @@
   _globals['_GETPIXELSETTINGSRESPONSE']._serialized_end=5103
   _globals['_STREAMTEMPERATUREREQUEST']._serialized_start=5105
   _globals['_STREAMTEMPERATUREREQUEST']._serialized_end=5155
   _globals['_GETTEMPERATURERESPONSE']._serialized_start=5158
   _globals['_GETTEMPERATURERESPONSE']._serialized_end=5418
   _globals['_PROMETHIONDEVICESERVICE']._serialized_start=5421
   _globals['_PROMETHIONDEVICESERVICE']._serialized_end=6499
-ChangePixelBlockSettingsRequest.__doc__ = """Attributes:
-    pixel_blocks:
-        1 based map of different pixel blocks settings, a sparse map
-        is accepted, keys should be integers between 1 and 12.
-    pixel_block_default:
-        If supplied, contains settings applied to every block before
-        then applying any specific settings in the per block settings.
+PixelSettings.InputWell.__doc__ = """Attributes:
+    input_well:
+        Control which well is driving the adc minknow reads from.  ALL
+        is not a valid value here (other values are acceptable).
+    regeneration_well:
+        Control which wells are being regenerated (has the specified
+        regeneration current driven to it).  All possible Input values
+        are acceptable, as long as the input is not the active adc
+        input. For example, { input: 1, regeneration: all } is
+        invalid, as an well cannot be both input and regenerated.
+"""
+ChangeDeviceSettingsResponse.__doc__ = """Attributes:
+    real_sampling_frequency:
+        The sampling frequency actually applied to the hardware, as
+        close as possible to the requested rate.  Note: only returned
+        if sampling rate was set as part of this call.
+"""
+StreamTemperatureRequest.__doc__ = """Attributes:
+    period_seconds:
+        How often temperature updates should be sent Defaults to a
+        period of 1 second, if not specified, or set to 0
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
 """
 GetPixelSettingsRequest.__doc__ = """Attributes:
     pixels:
         The channels (one based) to return data for. A sparse map is
         accepted
 """
-GetTemperatureResponse.__doc__ = """Attributes:
-    target_temperature:
-        Return the temperature target the device is aiming to reach.
-    flowcell_temperature:
-        Temperature as measured by thermistor TH2 on the P-Chip.
-    chamber_temperature:
-        Flow-cell chamber-temperature, calculated from the pixel-block
-        temperatures
-    pixel_block_temperature:
-        Temperature measured at each sensor in the ASIC, there are 12
-        sensors, one sensor per pixel-block
-"""
-ChangePixelSettingsRequest.__doc__ = """Attributes:
-    pixels:
-        1 based map of up to 3000 different pixel settings
-    pixel_default:
-        If supplied, contains settings applied to every pixel before
-        then applying any specific settings in the per pixel settings.
-"""
 PixelBlockSettings.__doc__ = """Attributes:
     regen_current_voltage_clamp:
         Voltage clamp for regeneration circuit (in millivolts)  The
         voltage in the regeneration circuit is clamped under this
         value, whilst applying the current specified in each pixel's
         settings.  The acceptable input range is -1000..1000
         (inclusive)
     unblock_voltage:
         The unblock voltage to apply when a pixel is unblocking.  The
         acceptable input range is -1000..1000 (inclusive)
 """
-WaveformSettings.__doc__ = """Attributes:
-    voltages:
-        The waveform data applied to the device (in millivolts)  Must
-        contain 32 values, in order to be a valid waveform.
-    frequency:
-        The frequency of the applied waveform, in Hz.  Valid values
-        are between 7.8125Hz and 500Hz.
-"""
-GetPixelBlockSettingsResponse.__doc__ = """Attributes:
-    pixel_blocks:
-        1 based map of different pixel blocks settings, containing 12
-        entries.
-"""
-PixelSettings.InputWell.__doc__ = """Attributes:
-    input_well:
-        Control which well is driving the adc minknow reads from.  ALL
-        is not a valid value here (other values are acceptable).
-    regeneration_well:
-        Control which wells are being regenerated (has the specified
-        regeneration current driven to it).  All possible Input values
-        are acceptable, as long as the input is not the active adc
-        input. For example, { input: 1, regeneration: all } is
-        invalid, as an well cannot be both input and regenerated.
-"""
-PixelSettings.__doc__ = """Attributes:
-    input:
-        The input driving the adv
-    overload_mode:
-        The mode the asic uses to handle currents that go above its
-        adc range.
-    cutoff_frequency:
-        Signal filter for input adc signal.
-    gain_multiplier:
-        Signal gain multiplier, applied to the integrator circuit.
-    gain_capacitor:
-        Gain capacitor, used in the integrator circuit.
-    calibration_mode:
-        The calibration mode to use.
-    unblock_voltage:
-        Controls the application of the unblock voltage to the pixel.
-    current_inverted:
-        Inverts the current's polarity.
-    membrane_simulation_enabled:
-        Control the state of the membrane simulation.
-    regeneration_current:
-        Control the regeneration current used when regenerating
-        well's.
-    regeneration_current_test_enabled:
-        Control if the regeneration current test is enabled.  This
-        connects the regeneration current to the integration adc
-        circuit and the input well. and allows users to read regen
-        current via the channel adc value.
-    bias_current:
-        The bias current for the amplifier - this controls the level
-        of noise of the signal.  The higher the bias current, the
-        lower the noise, but the bigger the heat and power drawn by
-        the amplifier. If it is set to off, no signal readings can be
-        made.
-"""
 DeviceSettings.__doc__ = """Attributes:
     sampling_frequency:
         The number of measurements to take each second.  Possible
         values are between 1000, and 10000. If the value is outside of
         this range, it will be clamped within it  This value cannot be
         changed during acquisition.
     ramp_voltage:
@@ -249,34 +190,58 @@
         and max_user_setpoint_temperature_celsius
     timings:
         If specified, the device will adopt these timings to set how
         long is spent at various stages of the current digitisation
         processes. The message includes a way of returning to default
         timings.  This value cannot be changed during acquisition
 """
-StreamTemperatureRequest.__doc__ = """Attributes:
-    period_seconds:
-        How often temperature updates should be sent Defaults to a
-        period of 1 second, if not specified, or set to 0
-    acquisition_run_id:
-        The acquisition id of the experiment.
-    data_selection:
-        The desired data selection.  The units for all values are
-        `seconds since the start of the experiment`.
+WaveformSettings.__doc__ = """Attributes:
+    voltages:
+        The waveform data applied to the device (in millivolts)  Must
+        contain 32 values, in order to be a valid waveform.
+    frequency:
+        The frequency of the applied waveform, in Hz.  Valid values
+        are between 7.8125Hz and 500Hz.
 """
-ChangeDeviceSettingsResponse.__doc__ = """Attributes:
-    real_sampling_frequency:
-        The sampling frequency actually applied to the hardware, as
-        close as possible to the requested rate.  Note: only returned
-        if sampling rate was set as part of this call.
+ChangePixelBlockSettingsRequest.__doc__ = """Attributes:
+    pixel_blocks:
+        1 based map of different pixel blocks settings, a sparse map
+        is accepted, keys should be integers between 1 and 12.
+    pixel_block_default:
+        If supplied, contains settings applied to every block before
+        then applying any specific settings in the per block settings.
+"""
+GetPixelBlockSettingsResponse.__doc__ = """Attributes:
+    pixel_blocks:
+        1 based map of different pixel blocks settings, containing 12
+        entries.
+"""
+ChangePixelSettingsRequest.__doc__ = """Attributes:
+    pixels:
+        1 based map of up to 3000 different pixel settings
+    pixel_default:
+        If supplied, contains settings applied to every pixel before
+        then applying any specific settings in the per pixel settings.
 """
 GetPixelSettingsResponse.__doc__ = """Attributes:
     pixels:
         List of all requested pixel settings, in the order requested.
 """
+GetTemperatureResponse.__doc__ = """Attributes:
+    target_temperature:
+        Return the temperature target the device is aiming to reach.
+    flowcell_temperature:
+        Temperature as measured by thermistor TH2 on the P-Chip.
+    chamber_temperature:
+        Flow-cell chamber-temperature, calculated from the pixel-block
+        temperatures
+    pixel_block_temperature:
+        Temperature measured at each sensor in the ASIC, there are 12
+        sensors, one sensor per pixel-block
+"""
 TimingEnginePeriods.__doc__ = """ Timing-engine periods are specified in 5ns units. Some of the timing
 mechanism can only achieve 10ns accuracy, so even numbers are
 preferred.  Note: There is a timing feature in the ASIC that requires
 the sum of the RST1 and DATA periods to be a multiple of 16
 
 Attributes:
     RST1:
@@ -314,8 +279,43 @@
     use_default_values:
         If written true, other fields will be ignored and the hardware
         will use default timings. When read will return true if
         previously set true, it will not tell you if the timing
         periods you previously entered are the same as the default
         values.
 """
+PixelSettings.__doc__ = """Attributes:
+    input:
+        The input driving the adv
+    overload_mode:
+        The mode the asic uses to handle currents that go above its
+        adc range.
+    cutoff_frequency:
+        Signal filter for input adc signal.
+    gain_multiplier:
+        Signal gain multiplier, applied to the integrator circuit.
+    gain_capacitor:
+        Gain capacitor, used in the integrator circuit.
+    calibration_mode:
+        The calibration mode to use.
+    unblock_voltage:
+        Controls the application of the unblock voltage to the pixel.
+    current_inverted:
+        Inverts the current's polarity.
+    membrane_simulation_enabled:
+        Control the state of the membrane simulation.
+    regeneration_current:
+        Control the regeneration current used when regenerating
+        well's.
+    regeneration_current_test_enabled:
+        Control if the regeneration current test is enabled.  This
+        connects the regeneration current to the integration adc
+        circuit and the input well. and allows users to read regen
+        current via the channel adc value.
+    bias_current:
+        The bias current for the amplifier - this controls the level
+        of noise of the signal.  The higher the bias current, the
+        lower the noise, but the bigger the heat and power drawn by
+        the amplifier. If it is set to off, no signal readings can be
+        made.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/promethion_device_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/promethion_device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/promethion_device_service.py` & `minknow_api-5.9.5/minknow_api/promethion_device_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/protocol_pb2.py` & `minknow_api-5.9.5/minknow_api/protocol_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -249,22 +249,148 @@
   _globals['_PROTOCOLPHASEMANAGEMENTRESPONSE']._serialized_end=8567
   _globals['_GENERATERUNREPORTREQUEST']._serialized_start=8569
   _globals['_GENERATERUNREPORTREQUEST']._serialized_end=8648
   _globals['_GENERATERUNREPORTRESPONSE']._serialized_start=8651
   _globals['_GENERATERUNREPORTRESPONSE']._serialized_end=8802
   _globals['_PROTOCOLSERVICE']._serialized_start=9834
   _globals['_PROTOCOLSERVICE']._serialized_end=12947
+PlatformQcResult.__doc__ = """Attributes:
+    flow_cell_id:
+        The flow cell id that the pqc was performed for
+    passed:
+        Whether the flow cell passed the platform qc check
+    total_pore_count:
+        Total number of pores that were found on the flow cell, across
+        all muxes.
+"""
+ProtocolRunUserInfo.__doc__ = """Attributes:
+    protocol_group_id:
+        The group which the experiment should be held in.  note: This
+        value could be unset if a user did not specify a group_id when
+        starting the protocol.
+    sample_id:
+        sample_id created by the user
+    barcode_user_info:
+        User supplied info for barcodes
+    user_specified_flow_cell_id:
+        user_specified_flow_cell_id created by the user
+    user_specified_product_code:
+        user_specified_product_code created by the user
+    kit_info:
+        Kit information the user requested
+"""
+BeginProtocolResponse.__doc__ = """Attributes:
+    run_id:
+        UUID generated when the protocol is started, to uniquely
+        represent this protocol instance
+"""
+BeginProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        Specify the protocol with a string containing all the
+        protocol's identifying components, eg:
+        "sequencing/sequencing_MIN106_DNA:FLO-MIN106:SQK-RPB004"
+    components:
+        Specify the protocol providing the identifying components
+        individually, all components are optional. Exactly one
+        protocol should match the given components otherwise and error
+        will be returned
+    user_info:
+        User info options for the protocol
+    offload_location_info:
+        Information about data offload locations to use to store data
+        Since 5.0.
+    target_run_until_criteria:
+        Initial Target Run-Until Criteria to use when starting an
+        acquisition for this protocol. These can be updated during the
+        acquisition using the Run-Until API.  Since 5.3
+    settings:
+        Any settings changed from the defaults specified in the
+        protocol's .toml file.
+"""
+AssociatePostProcessingAnalysisResponse.__doc__ = """Attributes:
+    id:
+        Id of the basecaller.proto post processing task that was
+        triggered, if the post processing analysis was executed
+        immediately (protocol was finished).
+"""
+ProtocolPhaseManagementRequest.__doc__ = """Attributes:
+    set_capabilities:
+        Update the set of capabilities (messages that will be
+        responded to by the protocol).
+    phase:
+        Update the protocol phase.  Leave empty (ie: PHASE_UNKNOWN) to
+        keep the previous phase.
+"""
+RequestOrigin.MinKNOW.__doc__ = """A request from minknow will usually come in the form of something
+ending naturally, or an error occurring where minknow has to take
+action
+
+Attributes:
+    cause:
+        Optional further details on the cause of the request
+"""
+SetPlatformQcResultRequest.__doc__ = """Attributes:
+    protocol_run_id:
+        The protocol_run_id that was given when the pqc run was
+        started
+"""
+BeginPlatformQcResponse.__doc__ = """Attributes:
+    run_id:
+        UUID generated when the protocol is started, to uniquely
+        represent this protocol instance
+"""
 KitInfo.__doc__ = """Attributes:
     sequencing_kit:
         The sequencing kit used to select the protocol e.g. "SQK-
         LSK108"
     barcode_expansion_kits:
         The expansion barcoding kits that the protocol supports e.g.
         "EXP-NBD104"
 """
+RequestOrigin.User.__doc__ = """'User' based changes will typically come from calls made by the UI
+such as 'stop_protocol'
+
+Attributes:
+    identity:
+        If available then provide any identity information MinKNOW
+        has about the client that made the RPC request
+"""
+ProtocolPhaseManagementRequest.Capabilities.__doc__ = """Attributes:
+    can_pause:
+        Indicate that the protocol will respond to pause and resume
+        requests.
+    can_trigger_mux_scan:
+        Indicate that the protocol will respond to mux scan requests.
+"""
+OffloadLocationInfo.__doc__ = """Attributes:
+    offload_location_ids:
+        Data offload locations to use to store protocol data,
+        specified using their `location_id`.  Valid `location_id`s can
+        be retrieved using
+        mooneye.offload_manager.list_offload_locations()  If any
+        `offload_location_ids` are specified, then:   - Data is not
+        stored locally   - `offload_location_path` must NOT be set (or
+        must be set to an empty value)      - The
+        `offload_location_ids` indicate that data should be offloaded,
+        rather than        stored locally; the `offload_location_path`
+        is used to set a local storage location.      - If both are
+        set, an error is returned  This requires a running instance of
+        Mooneye  Since 5.0.
+    offload_location_path:
+        Local, e.g., internal / external drive, paths to where the
+        protocol output will be stored.  This setting overrides the
+        default output locations (as set through configuration files
+        and/or the instance service).  If `offload_location_path` is
+        set to a non-empty value, then:  -  `offload_location_ids`
+        MUST be empty      - The `offload_location_ids` indicate that
+        data should be offloaded, rather than        stored locally;
+        the `offload_location_path` is used to set a local storage
+        location.      - If both are set, an error is returned  This
+        does not require a running instance of Mooneye  Since 5.0
+"""
 GenerateRunReportResponse.__doc__ = """Attributes:
     protocol_run_id:
         Protocol ID the run report is for.
     report_data:
         A section of the run report data (note the api to return this
         data may stream back several sections).
     remaining_length:
@@ -275,90 +401,89 @@
         data (note the api to return this data may stream back several
         sections).
     remaining_input_length:
         If include_input_data was set, how many further characters of
         input data remain  after this message (excluding of this
         message).
 """
-ListProtocolsRequest.__doc__ = """Attributes:
-    force_reload:
-        If this is false, then will try to use the cached value of the
-        protocol list where possible (still subject to changes in flow
-        cell). If this is true, then will force a reload of the
-        protocol list  Defaults to false
+BarcodeUserData.__doc__ = """Attributes:
+    barcode_name:
+        Barcode name the user data applies to, eg: "barcode02".   Acts
+        as the external barcode name `barcode_name_internal` is  also
+        set for dual barcoding   Acts as the rapid barcode name in
+        lampore barcoding if `lamp_barcode_id` is set
+    barcode_name_internal:
+        The internal barcode name if using dual barcode
+    lamp_barcode_id:
+        Lamp barcode id the user data applies to, eg: "FIP04"
+    alias:
+        User defined string alias for the barcode.
+    type:
+        Sample type grouping for the barcode.
+    passenger_info:
+        Extra context per barcode
 """
-ExternalOffload.__doc__ = """Attributes:
-    offload_ids:
-        The `id`s associated with active external data offloads
-        associated with the protocol The offload status can be queried
-        using `mooneye.offload_manager.watch_offloads()``
+RequestOrigin.ProtocolPhaseManagement.__doc__ = """The protocol script/bream is mainly responsible for making changes via
+protocol_phase_management"""
+StopProtocolRequest.__doc__ = """Attributes:
+    data_action_on_stop:
+        Specify how any running acquisition should be handled when
+        stopping the protocol.  Protocol state will enter
+        PROTOCOL_WAITING_FOR_ACQUISITION whilst any running
+        acquisition is finished.  If a script ends on its own any
+        analysis that was started is stopped, and it is allowed to
+        catchup. If the caller wants to end catchup they can call
+        stop_protocol to end catchup.  Since 1.15
 """
-GetVersionInfoResponse.__doc__ = """From instance.proto  Since 5.6
-
-Attributes:
-    minknow:
-        What minknow version is installed. Split into major, minor and
-        patch versions Also includes the full version as a string,
-        which contain the major, minor and patch numbers as well as if
-        the version is pre-release version (-pre), whether it is a
-        release candidate (-rc#) or whether it is a variant version
-        (i.e. for conferences) (-variant). For non-release builds it
-        also  includes the hash of the commit it is based on, and
-        whether the working copy is different from that has (-dirty)
-    bream:
-        The version of Bream that is installed.  An invalid
-        installation will cause this to return "0.0.0".  Prior to 5.0,
-        this field was called "protocols".  Since 5.0
-    distribution_version:
-        Describes the distribution that this MinKNOW installation is
-        part of, usually this will be the Metapackage version
-        number/identity, this will be "unknown" if the distribution-
-        version hasn't been set. This information is also communicated
-        in the Manager's DaemonMessage in daemon.proto
-    distribution_status:
-        Indicates if the MinKNOW distribution including components
-        such as Bream are stable, unstable or have been modified.
-    protocol_configuration:
-        The version of the protocol configuration files that is
-        installed.  An invalid installation will cause this to return
-        "0.0.0".  Prior to 5.0, this field was called "configuration".
-        Since 5.0
-    installation_type:
-        The installation type of MinKNOW.  The installation type may
-        affect the available features, or the update process.  Since
-        4.1
-    guppy_build_version:
-        Version of guppy MinKNOW was packaged against.  Since 5.0
-    guppy_connected_version:
-        Version of guppy MinKNOW running with.  Since 5.0
+FilteringInfo.__doc__ = """Attributes:
+    pqc_filter:
+        Filter by runs that have platform QC results  Just
+        initialising this message is enough to filter out runs with
+        platform QC results from ones that don't  Further filtering on
+        the platform QC results can be applied by using the fields
+        within PlatformQcFilter
+    protocol_group_id:
+        Filter runs by a specific protocol_group_id
 """
 GenerateRunReportRequest.__doc__ = """Attributes:
     protocol_run_id:
         The protocol_run_id to generate a report for.
     include_input_data:
         Optionally return the input data used to generate the report.
         This input data is represented as the data seen in
         report_data.proto
 """
-ListProtocolGroupIdsResponse.__doc__ = """Attributes:
-    protocol_group_ids:
-        A list of protocol group ids used in any protocol started on
-        this instance of minknow.  deprecated and replaced by string
-        protocol_group_id in message ProtocolGroupIdInfo  string data
-        is guaranteed to be ordered by most recent start time, since
-        5.6
-    protocol_group_ids_info:
-        A list of the most recent start time for each protocol group
-        id on this instance of minknow.  guaranteed to be ordered by
-        most recent start time since 5.6
-"""
-BeginPlatformQcResponse.__doc__ = """Attributes:
+GetRunInfoRequest.__doc__ = """Attributes:
     run_id:
-        UUID generated when the protocol is started, to uniquely
-        represent this protocol instance
+        The protocol run to get information about.
+"""
+StartProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        The identifier of the protocol, as provided by
+        list_protocols().
+    args:
+        The arguments to pass to the protocol.
+    user_info:
+        User input describing the protocol.
+    offload_location_info:
+        Information about data offload locations to use to store data
+        Since 5.0.
+    target_run_until_criteria:
+        Initial Target Run-Until Criteria to use when starting an
+        acquisition for this protocol. These can be updated during the
+        acquisition using the Run-Until API.  Since 5.3
+"""
+ProtocolPhaseManagementResponse.__doc__ = """Attributes:
+    action:
+        Requests that the protocol changes phase.  The client should
+        never receive an action type (other than possibly ACTION_NONE)
+        that it has not explicitly opted into via the
+        `ProtocolPhaseManagementRequest.set_capabilities` field.  If
+        this is set to ACTION_NONE, the message should be ignored
+        (this is for future compatibility).
 """
 ProtocolRunInfo.__doc__ = """Attributes:
     run_id:
         The unique identifier assigned to this run.  This is
         guaranteed to be made of ASCII characters, and at most 40
         characters. It is globally unique across all protocols runs on
         all MinKNOW instances.
@@ -441,252 +566,127 @@
         a pqc run)
     external_offload:
         Contains information about external data offloads associated
         with this protocol  Since 5.0
     software_versions:
         For storing version numbers to output to run report  Since 5.6
 """
-RequestOrigin.User.__doc__ = """'User' based changes will typically come from calls made by the UI
-such as 'stop_protocol'
-
-Attributes:
-    identity:
-        If available then provide any identity information MinKNOW
-        has about the client that made the RPC request
-"""
-ProtocolPhaseManagementResponse.__doc__ = """Attributes:
-    action:
-        Requests that the protocol changes phase.  The client should
-        never receive an action type (other than possibly ACTION_NONE)
-        that it has not explicitly opted into via the
-        `ProtocolPhaseManagementRequest.set_capabilities` field.  If
-        this is set to ACTION_NONE, the message should be ignored
-        (this is for future compatibility).
+AssociatePostProcessingAnalysisRequest.__doc__ = """Attributes:
+    run_id:
+        Protocol id to associate analysis with:
 """
 Epi2meWorkflowReference.__doc__ = """Attributes:
     id:
         The unique identifier for a workflow ( unique to a specific
         instance of epi2me )
     url:
         URL that links to the workflow report. Syntax for a local
         workflow: file:// otherwise: http(s)://
 """
-BeginProtocolResponse.__doc__ = """Attributes:
-    run_id:
-        UUID generated when the protocol is started, to uniquely
-        represent this protocol instance
-"""
-ProtocolGroupIdInfo.__doc__ = """timestamp for the last activity for experiment ordering since 5.6
-
-Attributes:
-    start_time:
-        Most recent start time for the protocol group id
-"""
-StartProtocolRequest.__doc__ = """Attributes:
-    identifier:
-        The identifier of the protocol, as provided by
-        list_protocols().
-    args:
-        The arguments to pass to the protocol.
-    user_info:
-        User input describing the protocol.
-    offload_location_info:
-        Information about data offload locations to use to store data
-        Since 5.0.
-    target_run_until_criteria:
-        Initial Target Run-Until Criteria to use when starting an
-        acquisition for this protocol. These can be updated during the
-        acquisition using the Run-Until API.  Since 5.3
-"""
-PlatformQcResult.__doc__ = """Attributes:
-    flow_cell_id:
-        The flow cell id that the pqc was performed for
-    passed:
-        Whether the flow cell passed the platform qc check
-    total_pore_count:
-        Total number of pores that were found on the flow cell, across
-        all muxes.
-"""
-AssociatePostProcessingAnalysisRequest.__doc__ = """Attributes:
-    run_id:
-        Protocol id to associate analysis with:
-"""
-AssociatedPostProcessingAnalysis.__doc__ = """Attributes:
-    started_id:
-        Id of analysis if this has been triggered (otherwise empty).
-    start_request:
-        Start request for analysis
-"""
-ProtocolRunUserInfo.__doc__ = """Attributes:
-    protocol_group_id:
-        The group which the experiment should be held in.  note: This
-        value could be unset if a user did not specify a group_id when
-        starting the protocol.
-    sample_id:
-        sample_id created by the user
-    barcode_user_info:
-        User supplied info for barcodes
-    user_specified_flow_cell_id:
-        user_specified_flow_cell_id created by the user
-    user_specified_product_code:
-        user_specified_product_code created by the user
-    kit_info:
-        Kit information the user requested
-"""
-BarcodeUserData.__doc__ = """Attributes:
-    barcode_name:
-        Barcode name the user data applies to, eg: "barcode02".   Acts
-        as the external barcode name `barcode_name_internal` is  also
-        set for dual barcoding   Acts as the rapid barcode name in
-        lampore barcoding if `lamp_barcode_id` is set
-    barcode_name_internal:
-        The internal barcode name if using dual barcode
-    lamp_barcode_id:
-        Lamp barcode id the user data applies to, eg: "FIP04"
-    alias:
-        User defined string alias for the barcode.
-    type:
-        Sample type grouping for the barcode.
-    passenger_info:
-        Extra context per barcode
-"""
-StopProtocolRequest.__doc__ = """Attributes:
-    data_action_on_stop:
-        Specify how any running acquisition should be handled when
-        stopping the protocol.  Protocol state will enter
-        PROTOCOL_WAITING_FOR_ACQUISITION whilst any running
-        acquisition is finished.  If a script ends on its own any
-        analysis that was started is stopped, and it is allowed to
-        catchup. If the caller wants to end catchup they can call
-        stop_protocol to end catchup.  Since 1.15
-"""
-RequestOrigin.RunUntil.__doc__ = """A request made by the run until script due to certain criteria being
-met
-
-Attributes:
-    criteria:
-        What criteria caused the state change
-"""
-RequestOrigin.ProtocolPhaseManagement.__doc__ = """The protocol script/bream is mainly responsible for making changes via
-protocol_phase_management"""
-AssociatePostProcessingAnalysisResponse.__doc__ = """Attributes:
-    id:
-        Id of the basecaller.proto post processing task that was
-        triggered, if the post processing analysis was executed
-        immediately (protocol was finished).
-"""
-StartProtocolResponse.__doc__ = """Attributes:
-    run_id:
-        UUID generated when the protocol is started, to uniquely
-        represent this protocol instance
-"""
-OffloadLocationInfo.__doc__ = """Attributes:
-    offload_location_ids:
-        Data offload locations to use to store protocol data,
-        specified using their `location_id`.  Valid `location_id`s can
-        be retrieved using
-        mooneye.offload_manager.list_offload_locations()  If any
-        `offload_location_ids` are specified, then:   - Data is not
-        stored locally   - `offload_location_path` must NOT be set (or
-        must be set to an empty value)      - The
-        `offload_location_ids` indicate that data should be offloaded,
-        rather than        stored locally; the `offload_location_path`
-        is used to set a local storage location.      - If both are
-        set, an error is returned  This requires a running instance of
-        Mooneye  Since 5.0.
-    offload_location_path:
-        Local, e.g., internal / external drive, paths to where the
-        protocol output will be stored.  This setting overrides the
-        default output locations (as set through configuration files
-        and/or the instance service).  If `offload_location_path` is
-        set to a non-empty value, then:  -  `offload_location_ids`
-        MUST be empty      - The `offload_location_ids` indicate that
-        data should be offloaded, rather than        stored locally;
-        the `offload_location_path` is used to set a local storage
-        location.      - If both are set, an error is returned  This
-        does not require a running instance of Mooneye  Since 5.0
-"""
-ProtocolPhaseManagementRequest.Capabilities.__doc__ = """Attributes:
-    can_pause:
-        Indicate that the protocol will respond to pause and resume
-        requests.
-    can_trigger_mux_scan:
-        Indicate that the protocol will respond to mux scan requests.
-"""
 WaitForFinishedRequest.__doc__ = """Attributes:
     run_id:
         Only consider a specific protocol run.
     state:
         Control what to wait for.  Specifying
         NOTIFY_BEFORE_TERMINATION allows a caller to be notified the
         script will be ended _soon_, and do final work to end cleanly.
         Since 1.11
     timeout:
         Timeout to wait for finished, if the timeout expires before
         the protocol is complete (in the state requested) then the
         response returns.  By default the timeout will wait forever.
         Since 1.15
 """
-ProtocolPhaseManagementRequest.__doc__ = """Attributes:
-    set_capabilities:
-        Update the set of capabilities (messages that will be
-        responded to by the protocol).
-    phase:
-        Update the protocol phase.  Leave empty (ie: PHASE_UNKNOWN) to
-        keep the previous phase.
+RequestOrigin.RunUntil.__doc__ = """A request made by the run until script due to certain criteria being
+met
+
+Attributes:
+    criteria:
+        What criteria caused the state change
 """
-GetRunInfoRequest.__doc__ = """Attributes:
+ExternalOffload.__doc__ = """Attributes:
+    offload_ids:
+        The `id`s associated with active external data offloads
+        associated with the protocol The offload status can be queried
+        using `mooneye.offload_manager.watch_offloads()``
+"""
+AssociatedPostProcessingAnalysis.__doc__ = """Attributes:
+    started_id:
+        Id of analysis if this has been triggered (otherwise empty).
+    start_request:
+        Start request for analysis
+"""
+ListProtocolGroupIdsResponse.__doc__ = """Attributes:
+    protocol_group_ids:
+        A list of protocol group ids used in any protocol started on
+        this instance of minknow.  deprecated and replaced by string
+        protocol_group_id in message ProtocolGroupIdInfo  string data
+        is guaranteed to be ordered by most recent start time, since
+        5.6
+    protocol_group_ids_info:
+        A list of the most recent start time for each protocol group
+        id on this instance of minknow.  guaranteed to be ordered by
+        most recent start time since 5.6
+"""
+BeginHardwareCheckResponse.__doc__ = """Attributes:
     run_id:
-        The protocol run to get information about.
+        UUID generated when the protocol is started, to uniquely
+        represent this protocol instance
 """
-SetPlatformQcResultRequest.__doc__ = """Attributes:
-    protocol_run_id:
-        The protocol_run_id that was given when the pqc run was
-        started
+ProtocolGroupIdInfo.__doc__ = """timestamp for the last activity for experiment ordering since 5.6
+
+Attributes:
+    start_time:
+        Most recent start time for the protocol group id
 """
-RequestOrigin.MinKNOW.__doc__ = """A request from minknow will usually come in the form of something
-ending naturally, or an error occurring where minknow has to take
-action
+GetVersionInfoResponse.__doc__ = """From instance.proto  Since 5.6
 
 Attributes:
-    cause:
-        Optional further details on the cause of the request
+    minknow:
+        What minknow version is installed. Split into major, minor and
+        patch versions Also includes the full version as a string,
+        which contain the major, minor and patch numbers as well as if
+        the version is pre-release version (-pre), whether it is a
+        release candidate (-rc#) or whether it is a variant version
+        (i.e. for conferences) (-variant). For non-release builds it
+        also  includes the hash of the commit it is based on, and
+        whether the working copy is different from that has (-dirty)
+    bream:
+        The version of Bream that is installed.  An invalid
+        installation will cause this to return "0.0.0".  Prior to 5.0,
+        this field was called "protocols".  Since 5.0
+    distribution_version:
+        Describes the distribution that this MinKNOW installation is
+        part of, usually this will be the Metapackage version
+        number/identity, this will be "unknown" if the distribution-
+        version hasn't been set. This information is also communicated
+        in the Manager's DaemonMessage in daemon.proto
+    distribution_status:
+        Indicates if the MinKNOW distribution including components
+        such as Bream are stable, unstable or have been modified.
+    protocol_configuration:
+        The version of the protocol configuration files that is
+        installed.  An invalid installation will cause this to return
+        "0.0.0".  Prior to 5.0, this field was called "configuration".
+        Since 5.0
+    installation_type:
+        The installation type of MinKNOW.  The installation type may
+        affect the available features, or the update process.  Since
+        4.1
+    guppy_build_version:
+        Version of guppy MinKNOW was packaged against.  Since 5.0
+    guppy_connected_version:
+        Version of guppy MinKNOW running with.  Since 5.0
 """
-BeginHardwareCheckResponse.__doc__ = """Attributes:
+StartProtocolResponse.__doc__ = """Attributes:
     run_id:
         UUID generated when the protocol is started, to uniquely
         represent this protocol instance
 """
-FilteringInfo.__doc__ = """Attributes:
-    pqc_filter:
-        Filter by runs that have platform QC results  Just
-        initialising this message is enough to filter out runs with
-        platform QC results from ones that don't  Further filtering on
-        the platform QC results can be applied by using the fields
-        within PlatformQcFilter
-    protocol_group_id:
-        Filter runs by a specific protocol_group_id
-"""
-BeginProtocolRequest.__doc__ = """Attributes:
-    identifier:
-        Specify the protocol with a string containing all the
-        protocol's identifying components, eg:
-        "sequencing/sequencing_MIN106_DNA:FLO-MIN106:SQK-RPB004"
-    components:
-        Specify the protocol providing the identifying components
-        individually, all components are optional. Exactly one
-        protocol should match the given components otherwise and error
-        will be returned
-    user_info:
-        User info options for the protocol
-    offload_location_info:
-        Information about data offload locations to use to store data
-        Since 5.0.
-    target_run_until_criteria:
-        Initial Target Run-Until Criteria to use when starting an
-        acquisition for this protocol. These can be updated during the
-        acquisition using the Run-Until API.  Since 5.3
-    settings:
-        Any settings changed from the defaults specified in the
-        protocol's .toml file.
+ListProtocolsRequest.__doc__ = """Attributes:
+    force_reload:
+        If this is false, then will try to use the cached value of the
+        protocol list where possible (still subject to changes in flow
+        cell). If this is true, then will force a reload of the
+        protocol list  Defaults to false
 """
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/protocol_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/protocol_service.py` & `minknow_api-5.9.5/minknow_api/protocol_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/protocol_settings_pb2.py` & `minknow_api-5.9.5/minknow_api/protocol_settings_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,29 @@
   _globals['_PROTOCOLSETTING_DEPENDENCY']._serialized_end=1805
   _globals['_PROTOCOLSETTING_CATEGORY']._serialized_start=1807
   _globals['_PROTOCOLSETTING_CATEGORY']._serialized_end=1874
   _globals['_PROTOCOLSETTING_UNIT']._serialized_start=1877
   _globals['_PROTOCOLSETTING_UNIT']._serialized_end=2081
   _globals['_PROTOCOLSETTING_VISIBILITY']._serialized_start=2083
   _globals['_PROTOCOLSETTING_VISIBILITY']._serialized_end=2146
+ProtocolIdentifierComponents.__doc__ = """Attributes:
+    location:
+        If not specified, will default to "ANY"
+    experiment_type:
+        one of "custom", "sequencing", "control", "ctc", "platform qc"
+        or "flowcell_plugin"
+    name:
+        Name (or path) of the protocol, without the .toml extension
+        eg: "sequencing/sequencing_MIN106_DNA" this is relative to the
+        system or user protocol directory
+    flow_cell_product_code:
+        eg: "FLO-MIN106"
+    kit:
+        eg: "SQK-RPB004"
+"""
 ProtocolSetting.__doc__ = """Attributes:
     identifier:
         Identifier is the unique primary-key for referring to
         protocol-settings, dependencies refer to other settings via
         their identifier.
     help:
         Optional additional help text for a setting that may be shown
@@ -90,23 +105,8 @@
     visibility:
         If any of the dependencies match their constraints, this level
         of visibility should be adopted. It should also be adopted if
         no dependencies are specified.
     choices:
         when unit is CHOICE, this defines the acceptable choices.
 """
-ProtocolIdentifierComponents.__doc__ = """Attributes:
-    location:
-        If not specified, will default to "ANY"
-    experiment_type:
-        one of "custom", "sequencing", "control", "ctc", "platform qc"
-        or "flowcell_plugin"
-    name:
-        Name (or path) of the protocol, without the .toml extension
-        eg: "sequencing/sequencing_MIN106_DNA" this is relative to the
-        system or user protocol directory
-    flow_cell_product_code:
-        eg: "FLO-MIN106"
-    kit:
-        eg: "SQK-RPB004"
-"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/protocol_settings_service.py` & `minknow_api-5.9.5/minknow_api/protocol_settings_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/report_data_pb2.py` & `minknow_api-5.9.5/minknow_api/report_data_pb2.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,14 @@
   _globals['_BASECALLBOXPLOT']._serialized_end=883
   _globals['_ACQUISTIONREPORTDATA']._serialized_start=886
   _globals['_ACQUISTIONREPORTDATA']._serialized_end=1816
   _globals['_HOST']._serialized_start=1818
   _globals['_HOST']._serialized_end=1862
   _globals['_REPORTDATA']._serialized_start=1865
   _globals['_REPORTDATA']._serialized_end=2181
-Host.__doc__ = """This is a subset of the information available from the describe_host()
-call"""
 AcquistionReportData.__doc__ = """This is spelt incorrectly (should be AcquisitionReportData)
 
 Attributes:
     acquisition_run_info:
         Information about the executed acquisition
     bucket_size:
         Size of buckets for all statistics data, in minutes.
@@ -69,8 +67,10 @@
         Information about the acquisitions that are a part of the
         protocol.
     user_messages:
         All the user messages from protocol start to protocol end.
     report_data_generation_time:
         The time at which the report data was generated (UTC)
 """
+Host.__doc__ = """This is a subset of the information available from the describe_host()
+call"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/report_data_service.py` & `minknow_api-5.9.5/minknow_api/report_data_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/rpc_options_pb2.py` & `minknow_api-5.9.5/minknow_api/rpc_options_pb2.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/run_until_pb2.py` & `minknow_api-5.9.5/minknow_api/run_until_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -85,44 +85,68 @@
   _globals['_WRITEUPDATESRESPONSE']._serialized_end=2647
   _globals['_STREAMUPDATESREQUEST']._serialized_start=2649
   _globals['_STREAMUPDATESREQUEST']._serialized_end=2724
   _globals['_STREAMUPDATESRESPONSE']._serialized_start=2726
   _globals['_STREAMUPDATESRESPONSE']._serialized_end=2851
   _globals['_RUNUNTILSERVICE']._serialized_start=2854
   _globals['_RUNUNTILSERVICE']._serialized_end=3359
-ScriptUpdate.CriteriaUpdated.__doc__ = """Indicates the the Run-Until Script has update its criteria in response
-to receiving a `StreamTargetCriteriaResponse` message"""
+WriteUpdatesRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition this Run-Until update applies to
+"""
+ErrorUpdate.InvalidCriteria.__doc__ = """Indicates that one or more of the supplied target criteria is not
+recognised by the  Run-Until Script.  Unrecognised target criteria
+will not be used to pause or stop the run."""
+ErrorUpdate.__doc__ = """Indicates that a problem has been encountered by the Run-Until Script"""
 ActionUpdate.__doc__ = """Indicates that an action has been performed  When a request is sent
 using `write_updates()`, MinKNOW performs the specified action.
 
 Attributes:
     criteria:
         The criteria associated with this action
 """
-EstimatedTimeRemainingUpdate.NotEstimated.__doc__ = """Indicates that a time is not estimated"""
-EstimatedTimeRemainingUpdate.EstimatedTimes.__doc__ = """Map of Run-Until Criterion to `EstimatedTime` when the criterion will
-be fulfilled  Only criteria for which an update is being provided are
-contained in the map."""
-ErrorUpdate.OtherError.__doc__ = """An error that is not covered by one of the other error types, above."""
-WriteUpdatesRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition this Run-Until update applies to
-"""
-StreamTargetCriteriaRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition to obtain the Run-Until Criteria for
+CriteriaValues.__doc__ = """A map of criterion name -> value  This message is deliberately
+flexible, to allow custom Run-Until Scripts to expand the range and
+types of available criteria."""
+EstimatedTimeRemainingUpdate.Estimated.__doc__ = """ These times are estimates of the (UTC) time at which the condition
+will be fulfilled  Some idea of the expected accuracy of this estimate
+can be obtained by comparing `min_time` with `max_time`.  If the
+estimated time is believed to be accurate (e.g. for a "runtime"
+criterion), then `min_time` may be equal to `max_time`.  Otherwise, if
+the estimate is believed to be inaccurate (e.g. for a "pore_scan"
+criterion which is not close to being fulfilled), then `min_time` and
+`max_time` may differ significantly.
+
+Attributes:
+    min_time:
+        Estimated lower bound on the time at which the condition will
+        occur (UTC)
+    max_time:
+        Estimated upper bound on the time at which the condition will
+        occur (UTC)
 """
 Update.__doc__ = """Attributes:
     current_progress_update:
         Gives the current values of the criteria (Compare to
         stream_target_criteria call to see %)
     other:
         Space for custom updates from custom Run-Until scripts
 """
-ErrorUpdate.__doc__ = """Indicates that a problem has been encountered by the Run-Until Script"""
+StreamUpdatesResponse.__doc__ = """Attributes:
+    idx:
+        The index of this update  The index is incremented after each
+        "interesting" update (i.e. an update that contains information
+        besides an `estimated_time_remaining_update` or a
+        `current_progress_update`). See `Update History`, above, for
+        further information.
+    time:
+        The timestamp of this update (UTC)
+    update:
+        The update data itself
+"""
 StreamUpdatesRequest.__doc__ = """Attributes:
     acquisition_run_id:
         The acquisition to stream Run-Until updates for
     start_idx:
         The index of the first update to send.  If an index is set
         that is greater than the current greatest update index, no
         past updates will be sent, but any future updates will be
@@ -135,51 +159,27 @@
         will cause the last update to be sent, and any future updates
         to be streamed.  The negative value is clamped such that a
         "large" negative number will be equivalent to setting a
         `start_idx` of `0`.  By default, `start_idx` is `0`, which
         means that all updates from the first update onwards will be
         sent.
 """
-CriteriaValues.__doc__ = """A map of criterion name -> value  This message is deliberately
-flexible, to allow custom Run-Until Scripts to expand the range and
-types of available criteria."""
-StreamUpdatesResponse.__doc__ = """Attributes:
-    idx:
-        The index of this update  The index is incremented after each
-        "interesting" update (i.e. an update that contains information
-        besides an `estimated_time_remaining_update` or a
-        `current_progress_update`). See `Update History`, above, for
-        further information.
-    time:
-        The timestamp of this update (UTC)
-    update:
-        The update data itself
+EstimatedTimeRemainingUpdate.__doc__ = """Indicates the estimated time remaining  An estimated time may be
+provided for each Run-Until Criterion that is specified as an end-
+point."""
+ErrorUpdate.OtherError.__doc__ = """An error that is not covered by one of the other error types, above."""
+StreamTargetCriteriaRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition to obtain the Run-Until Criteria for
 """
 WriteTargetCriteriaRequest.__doc__ = """Attributes:
     acquisition_run_id:
         The acquisition to set the Run-Until Criteria for
 """
-EstimatedTimeRemainingUpdate.Estimated.__doc__ = """ These times are estimates of the (UTC) time at which the condition
-will be fulfilled  Some idea of the expected accuracy of this estimate
-can be obtained by comparing `min_time` with `max_time`.  If the
-estimated time is believed to be accurate (e.g. for a "runtime"
-criterion), then `min_time` may be equal to `max_time`.  Otherwise, if
-the estimate is believed to be inaccurate (e.g. for a "pore_scan"
-criterion which is not close to being fulfilled), then `min_time` and
-`max_time` may differ significantly.
-
-Attributes:
-    min_time:
-        Estimated lower bound on the time at which the condition will
-        occur (UTC)
-    max_time:
-        Estimated upper bound on the time at which the condition will
-        occur (UTC)
-"""
-ErrorUpdate.InvalidCriteria.__doc__ = """Indicates that one or more of the supplied target criteria is not
-recognised by the  Run-Until Script.  Unrecognised target criteria
-will not be used to pause or stop the run."""
-EstimatedTimeRemainingUpdate.__doc__ = """Indicates the estimated time remaining  An estimated time may be
-provided for each Run-Until Criterion that is specified as an end-
-point."""
+EstimatedTimeRemainingUpdate.EstimatedTimes.__doc__ = """Map of Run-Until Criterion to `EstimatedTime` when the criterion will
+be fulfilled  Only criteria for which an update is being provided are
+contained in the map."""
+EstimatedTimeRemainingUpdate.NotEstimated.__doc__ = """Indicates that a time is not estimated"""
+ScriptUpdate.CriteriaUpdated.__doc__ = """Indicates the the Run-Until Script has update its criteria in response
+to receiving a `StreamTargetCriteriaResponse` message"""
 ScriptUpdate.Started.__doc__ = """Indicates that the run-until script has started and is running"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/run_until_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/run_until_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/run_until_service.py` & `minknow_api-5.9.5/minknow_api/run_until_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/statistics_pb2.py` & `minknow_api-5.9.5/minknow_api/statistics_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,292 +194,39 @@
   _globals['_STREAMBOXPLOTREQUEST_BOXPLOTTYPE']._serialized_end=7500
   _globals['_BOXPLOTRESPONSE']._serialized_start=7503
   _globals['_BOXPLOTRESPONSE']._serialized_end=7785
   _globals['_BOXPLOTRESPONSE_BOXPLOTDATASET']._serialized_start=7597
   _globals['_BOXPLOTRESPONSE_BOXPLOTDATASET']._serialized_end=7785
   _globals['_STATISTICSSERVICE']._serialized_start=8260
   _globals['_STATISTICSSERVICE']._serialized_end=9978
-StreamWriterOutputRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition id of the experiment.
-    data_selection:
-        The desired data selection.  The units for all values are
-        `seconds since the start of the experiment`.
-"""
-StreamBiasVoltagesRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition id of the experiment.
-"""
-StreamAcquisitionOutputResponse.FilteredSnapshots.__doc__ = """Attributes:
-    filtering:
-        The filtering parameters which contributed to this bucket.
-"""
-ReadLengthN50Response.__doc__ = """Attributes:
-    n50_data:
-        The N50 return data
-"""
-StreamReadLengthHistogramResponse.__doc__ = """Attributes:
-    read_length_type:
-        The data source for the histograms  Also specifies the units
-        for `data_selection` and `n50`  See `ReadLengthType` for
-        further information about the possible options.
-    bucket_ranges:
-        The range covered by each bucket in the histogram data
-    source_data_end:
-        The right hand edge of the last source bucket which contains
-        data  Measured across all source data, after excluding the
-        reads specified by `discard_outlier_percent` in the stream
-        request.
-    bucket_value_type:
-        The data accumulated in the read length histogram buckets  See
-        `BucketValueType` for further information about the possible
-        options.
-    histogram_data:
-        The histogram data
-"""
-ReadLengthHistogramSplit.__doc__ = """Attributes:
-    read_end_reason:
-        Split returned data by read_end_reason
-"""
-StreamQAccuracyHistogramRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The `acquisition_run_id` of the acquisition to obtain data for
-        If this is set to the `acquisition_run_id` of an acquisition
-        which is in-progress, then updates containing the latest
-        histogram data for that acquisition will be streamed regularly
-        until that acquisition finishes (see `poll_time_seconds`
-        below)  Otherwise, if this is set to the `acquisition_run_id`
-        of an acquisition which is finished, and for which final
-        histogram data is available, then the final histogram data for
-        that acquisition will be returned.  Final histogram data is
-        available until it is cleared.  Otherwise, if this parameter
-        is not set, or is set to a value which is neither the
-        `acquisition_run_id` of an acquisition which is in-progress,
-        nor the `acquisition_run_id` of an acquisition for which final
-        histogram data is available, then this call will fail with the
-        status `INVALID_ARGUMENT`.
-    poll_time_seconds:
-        How often to return new histogram data, in seconds  If not
-        specified, or set to `0`, then the poll time will be set to 60
-        seconds  If data is being returned for an acquisition which is
-        in progress, then one update will be sent when the call is
-        first performed, then subsequently every `poll_time` after
-        that, and then finally once again when the acquisition
-        finishes.  Otherwise, if final histogram data is being
-        returned for an acquisition that has already finished, this
-        parameter has no effect.  The final histogram data will be
-        returned, and the call will complete.
-    data_selection:
-        The desired q accuracy range which histograms should cover.
-    bucket_value_type:
-        What data to accumulate in the histogram buckets  See
-        `QAccuracyHistogramBucketValueType` for further information
-        about the available options.
-"""
-StreamQAccuracyHistogramResponse.__doc__ = """Attributes:
-    bucket_value_type:
-        The data accumulated in the histogram buckets  See
-        `QAccuracyHistogramBucketValueType` for further information
-        about the possible options.
-    bucket_ranges:
-        The range covered by each bucket in the histogram data
-    source_data_range:
-        The range covered by non-empty buckets in the source data
-    histogram_data:
-        The histogram data  If duplex basecalling is not enabled, then
-        Simplex histogram data will be returned If duplex basecalling
-        is enabled, then Simplex, Duplex and "All" (i.e. overall)
-        histogram data will be returned
-"""
-StreamDutyTimeResponse.__doc__ = """Attributes:
-    bucket_ranges:
-        The range covered by each entry in state_times
-    channel_states:
-        Map between channel state names, and a list of bucketed duty
-        time data
-"""
-WriterOutputSnapshot.__doc__ = """A snapshot of writer data.
-
-Attributes:
-    seconds:
-        The time the snapshot was collected, in seconds.  Represents
-        the number of seconds since the start of the experiment Will
-        usually stream in minute chunks, so will first see 60, then
-        120 etc
-    writer_output:
-        The writer data for this bucket.
-"""
-StreamDutyTimeRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition id of the experiment.
-    data_selection:
-        The desired data selection.  The units for all values are
-        `seconds since the start of the experiment`.
-"""
-AcquisitionOutputSnapshot.__doc__ = """A snapshot of acquisition output data, for a given set of filtering
-criteria.
-
-Attributes:
-    seconds:
-        The time the snapshot was collected, in seconds.  Represents
-        the number of seconds since the start of the experiment Will
-        usually stream in minute chunks, so will first see 60, then
-        120 etc
-    yield_summary:
-        The yield summary data.
-"""
-StreamEncounteredAcquisitionOutputKeysRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition id of the experiment.
-"""
-TemperaturePacket.Range.__doc__ = """Represents a range of values."""
-AcquisitionOutputSplit.__doc__ = """Attributes:
-    barcode_name:
-        Split data for every individual barcode.
-    alignment_reference:
-        Split data for each individual alignment reference.
-        References are defined in alignment references.
-    alignment_bed_file_region:
-        Split data for each target region.  Target regions are defined
-        in bed files.
-    lamp_barcode_id:
-        Split data for each lamp barcode id.  Lamp barcodes are
-        defined by the active lamp kit.
-    lamp_target_id:
-        Split data for each lamp targets id.  Lamp targets are defined
-        by the active lamp kit.
-    read_end_reason:
-        Split returned data by read_end_reason
+StreamQScoreHistogramResponse.BucketRange.__doc__ = """Attributes:
+    start:
+        The range covered by a bucket  The range [start, end) is half
+        open (i.e. the start value is included, the end value is not).
 """
 ReadLengthN50Response.ReadN50Data.__doc__ = """Attributes:
     estimated_n50:
         The estimated N50 value in bases  This is always set
     basecalled_n50:
         The basecalled N50 value  If the acquisition did/does not have
         live basecalling enabled, this will be 0.0
 """
-StreamQAccuracyHistogramResponse.QAccuracyHistogramData.__doc__ = """Attributes:
-    filtering:
-        The filtering parameters which contributed to this bucket.
-    bucket_values:
-        Counts for each histogram bucket  Units and type of
-        accumulated values are as specified in `bucket_value_type` The
-        range covered by each bucket is as in `bucket_ranges`
-    modal_q_accuracy:
-        The modal q accuracy, calculated using the `bucket_value_type`
-"""
-StreamTemperatureRequest.__doc__ = """Attributes:
-    period_seconds:
-        How often temperature updates should be sent Defaults to a
-        period of 1 second, if not specified, or set to 0
-    acquisition_run_id:
-        The acquisition id of the experiment.
-    data_selection:
-        The desired data selection.  The units for all values are
-        `seconds since the start of the experiment`.
-"""
-TemperaturePacket.__doc__ = """Attributes:
-    target_temperature:
-        The range is based on the requested target temperature and
-        tolerance.  For example, if the target temperature is 35, and
-        the tolerance is 1 then target temperatures will return as
-        34(min) and 36(max).
-"""
-StreamQScoreHistogramRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The `acquisition_run_id` of the acquisition to obtain data for
-        If this is set to the `acquisition_run_id` of an acquisition
-        which is in-progress, then updates containing the latest
-        histogram data for that acquisition will be streamed regularly
-        until that acquisition finishes (see `poll_time_seconds`
-        below)  Otherwise, if this is set to the `acquisition_run_id`
-        of an acquisition which is finished, and for which final
-        histogram data is available, then the final histogram data for
-        that acquisition will be returned.  Final histogram data is
-        available until it is cleared.  Otherwise, if this parameter
-        is not set, or is set to a value which is neither the
-        `acquisition_run_id` of an acquisition which is in-progress,
-        nor the `acquisition_run_id` of an acquisition for which final
-        histogram data is available, then this call will fail with the
-        status `INVALID_ARGUMENT`.
-    poll_time_seconds:
-        How often to return new histogram data, in seconds  If not
-        specified, or set to `0`, then the poll time will be set to 60
-        seconds  If data is being returned for an acquisition which is
-        in progress, then one update will be sent when the call is
-        first performed, then subsequently every `poll_time` after
-        that, and then finally once again when the acquisition
-        finishes.  Otherwise, if final histogram data is being
-        returned for an acquisition that has already finished, this
-        parameter has no effect.  The final histogram data will be
-        returned, and the call will complete.
-    data_selection:
-        The desired q score range which histograms should cover.
-    bucket_value_type:
-        What data to accumulate in the histogram buckets  See
-        `QScoreHistogramBucketValueType` for further information about
-        the available options.
-"""
 TemperaturePacket.PromethIONTemperature.__doc__ = """Packet of temperatures appropriate for a PromethION.
 
 Attributes:
     flowcell_temperature:
         Temperature as measured by thermistor TH2 on the P-Chip.
     chamber_temperature:
         Mean of 12 pixel-blocks temperatures measured with sensors in
         the ASIC.
 """
-StreamAcquisitionOutputResponse.__doc__ = """Attributes:
-    snapshots:
-        Snapshots split by requested filtering parameters.
-"""
-BoxplotResponse.BoxplotDataset.__doc__ = """Attributes:
-    min:
-        Minimum value for any point in the dataset.
-    q25:
-        25th quartile value for all points in the dataset.
-    q50:
-        50th quartile or median value for all points in the dataset.
-    q75:
-        75th quartile value for all points in the dataset.
-    max:
-        Maximum value for any point in the dataset.
-    count:
-        Number of items in this box plot's stats.
-    lower_full_width_half_maximum:
-        Estimated lower value where there is half the data compared to
-        the mode. provides some estimate on the sharpness of the mode
-        peak.
-    mode:
-        Estimated mode for the dataset.
-    upper_full_width_half_maximum:
-        Estimated upper value where there is half the data compared to
-        the mode. provides some estimate on the sharpness of the mode
-        peak.
-"""
-StreamQScoreHistogramResponse.QScoreHistogramData.__doc__ = """Attributes:
-    filtering:
-        The filtering parameters which contributed to this bucket.
-    bucket_values:
-        Counts for each histogram bucket  Units and type of
-        accumulated values are as specified in `bucket_value_type` The
-        range covered by each bucket is as in `bucket_ranges`
-    modal_q_score:
-        The modal q score, calculated using the `bucket_value_type`
-"""
-StreamAcquisitionOutputRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition id of the experiment.
-    data_selection:
-        The desired data selection.  The units for all values are
-        `seconds since the start of the experiment`.
-    filtering:
-        Define filtering parameters for streamed data.
-    split:
-        Define how results are split for returned data.
+GetReadLengthTypesResponse.__doc__ = """Attributes:
+    available_types:
+        Array of the types of bucket for which a histogram is
+        currently available
 """
 StreamReadLengthHistogramRequest.__doc__ = """Attributes:
     acquisition_run_id:
         The `acquisition_run_id` of the acquisition to obtain data for
         If this is set to the `acquisition_run_id` of an acquisition
         which is in-progress, then updates containing the latest
         histogram data for that acquisition will be streamed regularly
@@ -536,66 +283,72 @@
         total read lengths to be discarded (since it is always
         calculated from read length data)
     filtering:
         Define filtering parameters for streamed data.
     split:
         Define how results are split for returned data.
 """
-GetReadLengthTypesRequest.__doc__ = """Attributes:
-    acquisition_run_id:
-        The acquisition id of the experiment.
-"""
-ReadLengthN50Request.__doc__ = """Attributes:
-    acquisition_run_id:
-        The `acquisition_run_id` of the acquisition to obtain data for
-"""
-DataSelection.__doc__ = """Specify a desired data selection.  Units for values are as specified
-in the corresponding Request  The actual data selection used may
-differ from the desired one.  They are adjusted in the following
-sequence:   1. All values are set equal to the corresponding desired
-value.  2. Negative `start` or `end` values are fixed up by adding the
-current maximum value to the     specified value      - Negative start
-and end values are only supported for certain requests; typically they
-are        supported for time-series data      - If, after adding the
-current bucket count, the `start` value is still negative, then the
-start value is adjusted to `0`      - If, after adding the current
-bucket count, the `end` value is still negative, or is zero,
-then the data selection is empty      - If data collection is still
-ongoing, then the current bucket count may change between rpc
-calls as more data is collected.  3. Values which are not set, or
-which are set at `0`, are then adjusted to a default value:      -
-`start` and `step` will be set to the minimum valid value      - `end`
-will be set to the maximum valid value  4. Values which are outside of
-the valid range are clamped to the nearest valid value:      - Values
-less than minimum valid value will be set equal to the minimum valid
-value      - Values greater than the maximum valid value will be set
-equal to the maximum valid value  5. Finally, all values are 'rounded'
-to a nearby valid value      - `start` and `step` will be rounded down
-to the first valid value less than or equal to        their current
-values      - `end` will be rounded up to the first valid value that
-is greater than or equal to its        current value      - This means
-that the range that is specified after rounding includes the range
-that was        specified prior to rounding  If (`end` - `start`) is
-not an exact integer multiple of `step`, then the final bucket will
-cover a smaller range than that specified by `step`.  Note also that
-the maximum valid start and end value may not be known if data
-collection is still ongoing -- for example, the maximum valid time for
-time series data.  If this is the case, then the maximum valid value
-will be determined when the experiment ends, and values in use will be
-adjusted accordingly."""
-ReadLengthHistogramKey.__doc__ = """Attributes:
+AcquisitionOutputKey.__doc__ = """Attributes:
+    barcode_name:
+        Only return data for the given barcode.  Special values:   -
+        Specify "unclassified" for data which does not have a barcode.
+        - Specify "classified" for all data which has a barcode.  If
+        unspecified all barcodes are returned.
+    alignment_reference:
+        Only return data for the given alignment reference.  Special
+        values:   - Specify "unaligned" for data which does not align
+        to a reference   - Specify "aligned" for all data which aligns
+        to a reference  If unspecified all alignment targets are
+        returned.
+    alignment_bed_file_region:
+        Only return data for the given target region.  Target regions
+        are defined in bed files.  The region is a string which
+        identifies an entry in the bed file.  Special values:   -
+        Specify "offtarget" for data which does not have a bed region.
+        - Specify "ontarget" for all data which has a bed region.  If
+        unspecified all alignment regions are returned.
+    alignment_bed_file_region_name:
+        An alias to `alignment_bed_file_region`  An optional name can
+        be used to identify a target region in the bed file
+    lamp_barcode_id:
+        Only return data for the given lamp barcode.  Special values:
+        - Specify "unclassified" for data which does not have a lamp
+        barcode.   - Specify "classified" for all data which has a
+        lamp barcode.  If unspecified all lamp barcodes are returned.
+    lamp_target_id:
+        Only return data for the given lamp target.  Special values:
+        - Specify "unclassified" for data which does not have a lamp
+        target.   - Specify "classified" for all data which has a lamp
+        target. Using barcode terms here as lamp is part of barcoding
+        pipeline  If unspecified all lamp target are returned.
+    barcode_alias:
+        The barcode alias corresponding to the `barcode_name` and
+        `lamp_barcode_id`
     read_end_reason:
         Only return data for the given ReadEndReason.  Special values:
         - Specify `ReadEndReason::All` to return data for all read end
         reasons  If unspecified all read end reasons are returned.
 """
-StreamDutyTimeResponse.ChannelStateData.__doc__ = """Attributes:
-    state_times:
-        How much time (in samples) spent in this channel state, for
-        each bucket
+AcquisitionOutputSplit.__doc__ = """Attributes:
+    barcode_name:
+        Split data for every individual barcode.
+    alignment_reference:
+        Split data for each individual alignment reference.
+        References are defined in alignment references.
+    alignment_bed_file_region:
+        Split data for each target region.  Target regions are defined
+        in bed files.
+    lamp_barcode_id:
+        Split data for each lamp barcode id.  Lamp barcodes are
+        defined by the active lamp kit.
+    lamp_target_id:
+        Split data for each lamp targets id.  Lamp targets are defined
+        by the active lamp kit.
+    read_end_reason:
+        Split returned data by read_end_reason
 """
 StreamQScoreHistogramResponse.__doc__ = """Attributes:
     bucket_value_type:
         The data accumulated in the histogram buckets  See
         `QScoreHistogramBucketValueType` for further information about
         the possible options.
     bucket_ranges:
@@ -604,14 +357,49 @@
         The range covered by non-empty buckets in the source data
     histogram_data:
         The histogram data  If duplex basecalling is not enabled, then
         Simplex histogram data will be returned If duplex basecalling
         is enabled, then Simplex, Duplex and "All" (i.e. overall)
         histogram data will be returned
 """
+TemperaturePacket.__doc__ = """Attributes:
+    target_temperature:
+        The range is based on the requested target temperature and
+        tolerance.  For example, if the target temperature is 35, and
+        the tolerance is 1 then target temperatures will return as
+        34(min) and 36(max).
+"""
+BoxplotResponse.__doc__ = """Attributes:
+    datasets:
+        Result boxplots are stored in this array. This is an overview
+        of the stored data from the START of the acquisition period.
+        This includes ALL the basecalled stats from MinKNOW, not just
+        updates since previous calls!
+"""
+StreamDutyTimeResponse.__doc__ = """Attributes:
+    bucket_ranges:
+        The range covered by each entry in state_times
+    channel_states:
+        Map between channel state names, and a list of bucketed duty
+        time data
+"""
+StreamQAccuracyHistogramResponse.QAccuracyHistogramData.__doc__ = """Attributes:
+    filtering:
+        The filtering parameters which contributed to this bucket.
+    bucket_values:
+        Counts for each histogram bucket  Units and type of
+        accumulated values are as specified in `bucket_value_type` The
+        range covered by each bucket is as in `bucket_ranges`
+    modal_q_accuracy:
+        The modal q accuracy, calculated using the `bucket_value_type`
+"""
+GetReadLengthTypesRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition id of the experiment.
+"""
 StreamReadLengthHistogramResponse.ReadLengthHistogramData.__doc__ = """Attributes:
     filtering:
         The filtering parameters which contributed to this bucket.
     bucket_values:
         Counts for each histogram bucket  Units are as specified in
         `read_length_type` The range covered by each bucket is as in
         `bucket_ranges` The type of data accumulated in each bucket is
@@ -619,19 +407,17 @@
     n50:
         The N50 value for the read length data for the selected
         `read_length_type` and `read_end_reasons`.  Units are as
         specified by `read_length_type`.  Measured across all source
         data, after excluding the reads specified by
         `discard_outlier_percent` in the stream request.
 """
-StreamReadLengthHistogramResponse.BucketRange.__doc__ = """Attributes:
-    start:
-        The range covered by a bucket Units are as set in
-        `read_length_type`, above  The range [start, end) is half open
-        (i.e. the start value is included, the end value is not).
+ReadLengthN50Response.__doc__ = """Attributes:
+    n50_data:
+        The N50 return data
 """
 FloatDataSelection.__doc__ = """Specify a desired data selection, using floating point values  The
 actual data selection used may differ from the desired one.  They are
 adjusted in the following sequence:   1. The selection is set equal to
 the desired selection  2. Any selection value that is not set is
 adjusted to its default value:      - `start` and `step` will be set
 to the minimum valid value      - `end` will be set to the maximum
@@ -642,90 +428,136 @@
 valid value  4. Finally, all values are 'rounded' to a nearby valid
 value      - `start` and `step` will be rounded down to the first
 valid value less than or equal to        their current values      -
 `end` will be rounded up to the first valid value that is greater than
 or equal to its        current value      - This means that the range
 that is specified after rounding includes the range that was
 specified prior to rounding"""
-GetReadLengthTypesResponse.__doc__ = """Attributes:
-    available_types:
-        Array of the types of bucket for which a histogram is
-        currently available
+DataSelection.__doc__ = """Specify a desired data selection.  Units for values are as specified
+in the corresponding Request  The actual data selection used may
+differ from the desired one.  They are adjusted in the following
+sequence:   1. All values are set equal to the corresponding desired
+value.  2. Negative `start` or `end` values are fixed up by adding the
+current maximum value to the     specified value      - Negative start
+and end values are only supported for certain requests; typically they
+are        supported for time-series data      - If, after adding the
+current bucket count, the `start` value is still negative, then the
+start value is adjusted to `0`      - If, after adding the current
+bucket count, the `end` value is still negative, or is zero,
+then the data selection is empty      - If data collection is still
+ongoing, then the current bucket count may change between rpc
+calls as more data is collected.  3. Values which are not set, or
+which are set at `0`, are then adjusted to a default value:      -
+`start` and `step` will be set to the minimum valid value      - `end`
+will be set to the maximum valid value  4. Values which are outside of
+the valid range are clamped to the nearest valid value:      - Values
+less than minimum valid value will be set equal to the minimum valid
+value      - Values greater than the maximum valid value will be set
+equal to the maximum valid value  5. Finally, all values are 'rounded'
+to a nearby valid value      - `start` and `step` will be rounded down
+to the first valid value less than or equal to        their current
+values      - `end` will be rounded up to the first valid value that
+is greater than or equal to its        current value      - This means
+that the range that is specified after rounding includes the range
+that was        specified prior to rounding  If (`end` - `start`) is
+not an exact integer multiple of `step`, then the final bucket will
+cover a smaller range than that specified by `step`.  Note also that
+the maximum valid start and end value may not be known if data
+collection is still ongoing -- for example, the maximum valid time for
+time series data.  If this is the case, then the maximum valid value
+will be determined when the experiment ends, and values in use will be
+adjusted accordingly."""
+StreamWriterOutputRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
 """
-StreamQScoreHistogramResponse.BucketRange.__doc__ = """Attributes:
-    start:
-        The range covered by a bucket  The range [start, end) is half
-        open (i.e. the start value is included, the end value is not).
+TemperaturePacket.MinIONTemperature.__doc__ = """Packet of temperatures appropriate for a MinION.
+
+Attributes:
+    asic_temperature:
+        Temperature as measured by the probe inside the asic.
+    heatsink_temperature:
+        Temperature as measured by the probe in the minion heatsink.
 """
-AcquisitionOutputKey.__doc__ = """Attributes:
-    barcode_name:
-        Only return data for the given barcode.  Special values:   -
-        Specify "unclassified" for data which does not have a barcode.
-        - Specify "classified" for all data which has a barcode.  If
-        unspecified all barcodes are returned.
-    alignment_reference:
-        Only return data for the given alignment reference.  Special
-        values:   - Specify "unaligned" for data which does not align
-        to a reference   - Specify "aligned" for all data which aligns
-        to a reference  If unspecified all alignment targets are
-        returned.
-    alignment_bed_file_region:
-        Only return data for the given target region.  Target regions
-        are defined in bed files.  The region is a string which
-        identifies an entry in the bed file.  Special values:   -
-        Specify "offtarget" for data which does not have a bed region.
-        - Specify "ontarget" for all data which has a bed region.  If
-        unspecified all alignment regions are returned.
-    alignment_bed_file_region_name:
-        An alias to `alignment_bed_file_region`  An optional name can
-        be used to identify a target region in the bed file
-    lamp_barcode_id:
-        Only return data for the given lamp barcode.  Special values:
-        - Specify "unclassified" for data which does not have a lamp
-        barcode.   - Specify "classified" for all data which has a
-        lamp barcode.  If unspecified all lamp barcodes are returned.
-    lamp_target_id:
-        Only return data for the given lamp target.  Special values:
-        - Specify "unclassified" for data which does not have a lamp
-        target.   - Specify "classified" for all data which has a lamp
-        target. Using barcode terms here as lamp is part of barcoding
-        pipeline  If unspecified all lamp target are returned.
-    barcode_alias:
-        The barcode alias corresponding to the `barcode_name` and
-        `lamp_barcode_id`
-    read_end_reason:
-        Only return data for the given ReadEndReason.  Special values:
-        - Specify `ReadEndReason::All` to return data for all read end
-        reasons  If unspecified all read end reasons are returned.
+ReadLengthN50Request.__doc__ = """Attributes:
+    acquisition_run_id:
+        The `acquisition_run_id` of the acquisition to obtain data for
 """
-BoxplotResponse.__doc__ = """Attributes:
-    datasets:
-        Result boxplots are stored in this array. This is an overview
-        of the stored data from the START of the acquisition period.
-        This includes ALL the basecalled stats from MinKNOW, not just
-        updates since previous calls!
+StreamDutyTimeRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
+"""
+StreamQAccuracyHistogramResponse.__doc__ = """Attributes:
+    bucket_value_type:
+        The data accumulated in the histogram buckets  See
+        `QAccuracyHistogramBucketValueType` for further information
+        about the possible options.
+    bucket_ranges:
+        The range covered by each bucket in the histogram data
+    source_data_range:
+        The range covered by non-empty buckets in the source data
+    histogram_data:
+        The histogram data  If duplex basecalling is not enabled, then
+        Simplex histogram data will be returned If duplex basecalling
+        is enabled, then Simplex, Duplex and "All" (i.e. overall)
+        histogram data will be returned
 """
 StreamQAccuracyHistogramResponse.BucketRange.__doc__ = """Attributes:
     start:
         The range covered by a bucket  The range [start, end) is half
         open (i.e. the start value is included, the end value is not).
 """
-TemperaturePacket.MinIONTemperature.__doc__ = """Packet of temperatures appropriate for a MinION.
+StreamDutyTimeResponse.ChannelStateData.__doc__ = """Attributes:
+    state_times:
+        How much time (in samples) spent in this channel state, for
+        each bucket
+"""
+ReadLengthHistogramSplit.__doc__ = """Attributes:
+    read_end_reason:
+        Split returned data by read_end_reason
+"""
+StreamAcquisitionOutputResponse.__doc__ = """Attributes:
+    snapshots:
+        Snapshots split by requested filtering parameters.
+"""
+StreamAcquisitionOutputRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
+    filtering:
+        Define filtering parameters for streamed data.
+    split:
+        Define how results are split for returned data.
+"""
+StreamEncounteredAcquisitionOutputKeysRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition id of the experiment.
+"""
+WriterOutputSnapshot.__doc__ = """A snapshot of writer data.
 
 Attributes:
-    asic_temperature:
-        Temperature as measured by the probe inside the asic.
-    heatsink_temperature:
-        Temperature as measured by the probe in the minion heatsink.
+    seconds:
+        The time the snapshot was collected, in seconds.  Represents
+        the number of seconds since the start of the experiment Will
+        usually stream in minute chunks, so will first see 60, then
+        120 etc
+    writer_output:
+        The writer data for this bucket.
 """
-StreamDutyTimeResponse.BucketRange.__doc__ = """Attributes:
-    start:
-        The range covered by a bucket Values are in seconds  The range
-        [start, end) is half open (i.e. the start value is included,
-        the end value is not).
+StreamBiasVoltagesRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The acquisition id of the experiment.
 """
 StreamBoxplotRequest.__doc__ = """Attributes:
     acquisition_run_id:
         The acquisition id of the experiment.
     data_type:
         Type of boxplot data to return.
     dataset_width:
@@ -748,8 +580,176 @@
         seconds. Note that this stream will return results regardless
         of the stats updates (because it always returns all the
         datasets). poll_time should be larger than the basecalled
         stats update rate in MinKNOW - please see
         basecalled_stats_refresh_rate_seconds in the configs (set to 1
         second in MinKNOW 3.2).  If unspecified, defaults to 1 minute.
 """
+StreamTemperatureRequest.__doc__ = """Attributes:
+    period_seconds:
+        How often temperature updates should be sent Defaults to a
+        period of 1 second, if not specified, or set to 0
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
+"""
+StreamDutyTimeResponse.BucketRange.__doc__ = """Attributes:
+    start:
+        The range covered by a bucket Values are in seconds  The range
+        [start, end) is half open (i.e. the start value is included,
+        the end value is not).
+"""
+BoxplotResponse.BoxplotDataset.__doc__ = """Attributes:
+    min:
+        Minimum value for any point in the dataset.
+    q25:
+        25th quartile value for all points in the dataset.
+    q50:
+        50th quartile or median value for all points in the dataset.
+    q75:
+        75th quartile value for all points in the dataset.
+    max:
+        Maximum value for any point in the dataset.
+    count:
+        Number of items in this box plot's stats.
+    lower_full_width_half_maximum:
+        Estimated lower value where there is half the data compared to
+        the mode. provides some estimate on the sharpness of the mode
+        peak.
+    mode:
+        Estimated mode for the dataset.
+    upper_full_width_half_maximum:
+        Estimated upper value where there is half the data compared to
+        the mode. provides some estimate on the sharpness of the mode
+        peak.
+"""
+ReadLengthHistogramKey.__doc__ = """Attributes:
+    read_end_reason:
+        Only return data for the given ReadEndReason.  Special values:
+        - Specify `ReadEndReason::All` to return data for all read end
+        reasons  If unspecified all read end reasons are returned.
+"""
+StreamReadLengthHistogramResponse.BucketRange.__doc__ = """Attributes:
+    start:
+        The range covered by a bucket Units are as set in
+        `read_length_type`, above  The range [start, end) is half open
+        (i.e. the start value is included, the end value is not).
+"""
+StreamReadLengthHistogramResponse.__doc__ = """Attributes:
+    read_length_type:
+        The data source for the histograms  Also specifies the units
+        for `data_selection` and `n50`  See `ReadLengthType` for
+        further information about the possible options.
+    bucket_ranges:
+        The range covered by each bucket in the histogram data
+    source_data_end:
+        The right hand edge of the last source bucket which contains
+        data  Measured across all source data, after excluding the
+        reads specified by `discard_outlier_percent` in the stream
+        request.
+    bucket_value_type:
+        The data accumulated in the read length histogram buckets  See
+        `BucketValueType` for further information about the possible
+        options.
+    histogram_data:
+        The histogram data
+"""
+StreamQScoreHistogramResponse.QScoreHistogramData.__doc__ = """Attributes:
+    filtering:
+        The filtering parameters which contributed to this bucket.
+    bucket_values:
+        Counts for each histogram bucket  Units and type of
+        accumulated values are as specified in `bucket_value_type` The
+        range covered by each bucket is as in `bucket_ranges`
+    modal_q_score:
+        The modal q score, calculated using the `bucket_value_type`
+"""
+StreamAcquisitionOutputResponse.FilteredSnapshots.__doc__ = """Attributes:
+    filtering:
+        The filtering parameters which contributed to this bucket.
+"""
+StreamQAccuracyHistogramRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The `acquisition_run_id` of the acquisition to obtain data for
+        If this is set to the `acquisition_run_id` of an acquisition
+        which is in-progress, then updates containing the latest
+        histogram data for that acquisition will be streamed regularly
+        until that acquisition finishes (see `poll_time_seconds`
+        below)  Otherwise, if this is set to the `acquisition_run_id`
+        of an acquisition which is finished, and for which final
+        histogram data is available, then the final histogram data for
+        that acquisition will be returned.  Final histogram data is
+        available until it is cleared.  Otherwise, if this parameter
+        is not set, or is set to a value which is neither the
+        `acquisition_run_id` of an acquisition which is in-progress,
+        nor the `acquisition_run_id` of an acquisition for which final
+        histogram data is available, then this call will fail with the
+        status `INVALID_ARGUMENT`.
+    poll_time_seconds:
+        How often to return new histogram data, in seconds  If not
+        specified, or set to `0`, then the poll time will be set to 60
+        seconds  If data is being returned for an acquisition which is
+        in progress, then one update will be sent when the call is
+        first performed, then subsequently every `poll_time` after
+        that, and then finally once again when the acquisition
+        finishes.  Otherwise, if final histogram data is being
+        returned for an acquisition that has already finished, this
+        parameter has no effect.  The final histogram data will be
+        returned, and the call will complete.
+    data_selection:
+        The desired q accuracy range which histograms should cover.
+    bucket_value_type:
+        What data to accumulate in the histogram buckets  See
+        `QAccuracyHistogramBucketValueType` for further information
+        about the available options.
+"""
+TemperaturePacket.Range.__doc__ = """Represents a range of values."""
+AcquisitionOutputSnapshot.__doc__ = """A snapshot of acquisition output data, for a given set of filtering
+criteria.
+
+Attributes:
+    seconds:
+        The time the snapshot was collected, in seconds.  Represents
+        the number of seconds since the start of the experiment Will
+        usually stream in minute chunks, so will first see 60, then
+        120 etc
+    yield_summary:
+        The yield summary data.
+"""
+StreamQScoreHistogramRequest.__doc__ = """Attributes:
+    acquisition_run_id:
+        The `acquisition_run_id` of the acquisition to obtain data for
+        If this is set to the `acquisition_run_id` of an acquisition
+        which is in-progress, then updates containing the latest
+        histogram data for that acquisition will be streamed regularly
+        until that acquisition finishes (see `poll_time_seconds`
+        below)  Otherwise, if this is set to the `acquisition_run_id`
+        of an acquisition which is finished, and for which final
+        histogram data is available, then the final histogram data for
+        that acquisition will be returned.  Final histogram data is
+        available until it is cleared.  Otherwise, if this parameter
+        is not set, or is set to a value which is neither the
+        `acquisition_run_id` of an acquisition which is in-progress,
+        nor the `acquisition_run_id` of an acquisition for which final
+        histogram data is available, then this call will fail with the
+        status `INVALID_ARGUMENT`.
+    poll_time_seconds:
+        How often to return new histogram data, in seconds  If not
+        specified, or set to `0`, then the poll time will be set to 60
+        seconds  If data is being returned for an acquisition which is
+        in progress, then one update will be sent when the call is
+        first performed, then subsequently every `poll_time` after
+        that, and then finally once again when the acquisition
+        finishes.  Otherwise, if final histogram data is being
+        returned for an acquisition that has already finished, this
+        parameter has no effect.  The final histogram data will be
+        returned, and the call will complete.
+    data_selection:
+        The desired q score range which histograms should cover.
+    bucket_value_type:
+        What data to accumulate in the histogram buckets  See
+        `QScoreHistogramBucketValueType` for further information about
+        the available options.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.9.1/minknow_api/statistics_pb2_grpc.py` & `minknow_api-5.9.5/minknow_api/statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/statistics_service.py` & `minknow_api-5.9.5/minknow_api/statistics_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/testutils.py` & `minknow_api-5.9.5/minknow_api/testutils.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/tools/any_helpers.py` & `minknow_api-5.9.5/minknow_api/tools/any_helpers.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/minknow_api/tools/protocols.py` & `minknow_api-5.9.5/minknow_api/tools/protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         "min_score_mid",
     ],
 )
 AlignmentArgs = collections.namedtuple("AlignmentArgs", ["reference_files", "bed_file"])
 BasecallingArgs = collections.namedtuple(
     "BasecallingArgs", ["config", "barcoding", "alignment"]
 )
-OutputArgs = collections.namedtuple("OutputArgs", ["reads_per_file"])
+OutputArgs = collections.namedtuple("OutputArgs", ["reads_per_file", "batch_duration"])
 
 
 @dataclasses.dataclass
 class CriteriaValues:
     """
     Python representation of a `minknow_api.run_until.CriteriaValues` message
 
@@ -337,47 +337,63 @@
 
         if read_until.first_channel:
             read_until_args.append("first_channel={}".format(read_until.first_channel))
 
         if read_until.last_channel:
             read_until_args.append("last_channel={}".format(read_until.last_channel))
 
-        # --read_until filter_type='enrich' reference_files=['/data/my-alignment-file'] bed_file='/data/bed_file.bed' first_channel=1 last_channel=512
-        print(read_until_args)
         protocol_args.extend(["--read_until"] + read_until_args)
 
     protocol_args.append("--fast5=" + on_off(fast5_arguments))
     if fast5_arguments:
         protocol_args.extend(
             ["--fast5_data", "trace_table", "fastq", "raw", "vbz_compress"]
         )
-        protocol_args.append(
-            "--fast5_reads_per_file={}".format(fast5_arguments.reads_per_file)
-        )
+        if fast5_arguments.reads_per_file is not None:
+            protocol_args.append(
+                "--fast5_reads_per_file={}".format(fast5_arguments.reads_per_file)
+            )
+        if fast5_arguments.batch_duration is not None:
+            protocol_args.append(
+                "--fast5_batch_duration={}".format(fast5_arguments.batch_duration)
+            )
 
     protocol_args.append("--pod5=" + on_off(pod5_arguments))
     if pod5_arguments:
-        protocol_args.append(
-            "--pod5_reads_per_file={}".format(pod5_arguments.reads_per_file)
-        )
+        if pod5_arguments.reads_per_file is not None:
+            protocol_args.append(
+                "--pod5_reads_per_file={}".format(pod5_arguments.reads_per_file)
+            )
+        if pod5_arguments.batch_duration is not None:
+            protocol_args.append(
+                "--pod5_batch_duration={}".format(pod5_arguments.batch_duration)
+            )
 
     protocol_args.append("--fastq=" + on_off(fastq_arguments))
     if fastq_arguments:
         protocol_args.extend(["--fastq_data", "compress"])
-        protocol_args.append(
-            "--fastq_reads_per_file={}".format(fastq_arguments.reads_per_file)
-        )
+        if fastq_arguments.reads_per_file is not None:
+            protocol_args.append(
+                "--fastq_reads_per_file={}".format(fastq_arguments.reads_per_file)
+            )
+        if fastq_arguments.batch_duration is not None:
+            protocol_args.append(
+                "--fastq_batch_duration={}".format(fastq_arguments.batch_duration)
+            )
 
     protocol_args.append("--bam=" + on_off(bam_arguments))
     if bam_arguments:
-        if bam_arguments.reads_per_file != 4000:
-            raise Exception("Unable to change reads per file for BAM.")
-        """protocol_args.append(
-            "--bam_reads_per_file={}".format(bam_arguments.reads_per_file)
-        )"""
+        if bam_arguments.reads_per_file is not None:
+            protocol_args.append(
+                "--bam_reads_per_file={}".format(bam_arguments.reads_per_file)
+            )
+        if bam_arguments.batch_duration is not None:
+            protocol_args.append(
+                "--bam_batch_duration={}".format(bam_arguments.batch_duration)
+            )
 
     if not is_flongle:
         protocol_args.append(
             "--active_channel_selection=" + on_off(not disable_active_channel_selection)
         )
         if not disable_active_channel_selection:
             protocol_args.append("--mux_scan_period={}".format(mux_scan_period))
```

### Comparing `minknow_api-5.9.1/minknow_api.egg-info/PKG-INFO` & `minknow_api-5.9.5/minknow_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minknow_api
-Version: 5.9.1
+Version: 5.9.5
 Summary: MinKNOW RPC API bindings
 Home-page: https://github.com/nanoporetech/minknow_api
 Author: Oxford Nanopore Technologies PLC
 Author-email: info@nanoporetech.com
 Description-Content-Type: text/markdown
 Requires-Dist: importlib-resources<3.3; python_version < "3.7.0"
 Requires-Dist: grpcio~=1.51
```

### Comparing `minknow_api-5.9.1/minknow_api.egg-info/SOURCES.txt` & `minknow_api-5.9.5/minknow_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minknow_api-5.9.1/setup.py` & `minknow_api-5.9.5/setup.py`

 * *Files identical despite different names*

