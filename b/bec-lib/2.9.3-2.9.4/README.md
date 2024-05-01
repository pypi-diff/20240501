# Comparing `tmp/bec_lib-2.9.3.tar.gz` & `tmp/bec_lib-2.9.4.tar.gz`

## Comparing `bec_lib-2.9.3.tar` & `bec_lib-2.9.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.9.3/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/bec_service.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/bec_yaml_loader.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/client.py
--rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/connector.py
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    30828 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/device.py
--rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    37580 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/logger.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/queue_items.py
--rw-r--r--   0        0        0    39012 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/request_items.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/scan_data.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/scan_report.py
--rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.9.3/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_bec_logger.py
--rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_callback_handler.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_config_helper.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_core_utils.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_device_manager.py
--rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_file_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_redis_connector.py
--rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scan_data.py
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scan_items.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 bec_lib-2.9.3/tests/test_yaml_loader.py
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/init_config.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/README_template_tests.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/gitignore
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/pyproject.toml
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/setup_device_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/git_hooks/post-commit
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 bec_lib-2.9.3/util_scripts/plugin_setup_files/git_hooks/pre-commit
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.9.3/.gitignore
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 bec_lib-2.9.3/pyproject.toml
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 bec_lib-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.9.4/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/bec_yaml_loader.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/client.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/connector.py
+-rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    30862 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/device.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    37580 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/logger.py
+-rw-r--r--   0        0        0    22362 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    39012 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    17050 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.9.4/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_file_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 bec_lib-2.9.4/tests/test_yaml_loader.py
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/setup_device_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 bec_lib-2.9.4/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.9.4/.gitignore
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 bec_lib-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 bec_lib-2.9.4/PKG-INFO
```

### Comparing `bec_lib-2.9.3/README.md` & `bec_lib-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/__init__.py` & `bec_lib-2.9.4/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/alarm_handler.py` & `bec_lib-2.9.4/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/async_data.py` & `bec_lib-2.9.4/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/bec_service.py` & `bec_lib-2.9.4/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/bec_yaml_loader.py` & `bec_lib-2.9.4/bec_lib/bec_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/bl_checks.py` & `bec_lib-2.9.4/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/bl_conditions.py` & `bec_lib-2.9.4/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/callback_handler.py` & `bec_lib-2.9.4/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/channel_monitor.py` & `bec_lib-2.9.4/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/client.py` & `bec_lib-2.9.4/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/config_helper.py` & `bec_lib-2.9.4/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/connector.py` & `bec_lib-2.9.4/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/dap_plugin_objects.py` & `bec_lib-2.9.4/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/dap_plugins.py` & `bec_lib-2.9.4/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/device.py` & `bec_lib-2.9.4/bec_lib/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,16 +787,16 @@
         """
         Returns the device limits.
         """
         limit_msg = self.root.parent.connector.get(MessageEndpoints.device_limits(self.root.name))
         if not limit_msg:
             return [0, 0]
         limits = [
-            limit_msg.content["signals"].get("low", 0),
-            limit_msg.content["signals"].get("high", 0),
+            limit_msg.content["signals"].get("low", {}).get("value", 0),
+            limit_msg.content["signals"].get("high", {}).get("value", 0),
         ]
         return limits
 
     @limits.setter
     def limits(self, val: list):
         self.update_config({"deviceConfig": {"limits": val}})
```

### Comparing `bec_lib-2.9.3/bec_lib/devicemanager.py` & `bec_lib-2.9.4/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/endpoints.py` & `bec_lib-2.9.4/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/file_utils.py` & `bec_lib-2.9.4/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/lmfit_serializer.py` & `bec_lib-2.9.4/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/logbook_connector.py` & `bec_lib-2.9.4/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/logger.py` & `bec_lib-2.9.4/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/messages.py` & `bec_lib-2.9.4/bec_lib/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,23 +297,23 @@
     parameter: dict
 
 
 class DeviceMessage(BECMessage):
     """Message type for sending device readings from the device server
 
     Args:
-        signals (dict): Dictionary of device signals
+        signals (dict): Dictionary containing the device signals and their values
         metadata (dict, optional): Metadata to describe the conditions of the device reading
 
     Examples:
         >>> BECMessage.DeviceMessage(signals={'samx': {'value': 14.999033949016491, 'timestamp': 1686385306.0265112}, 'samx_setpoint': {'value': 15.0, 'timestamp': 1686385306.016806}, 'samx_motor_is_moving': {'value': 0, 'timestamp': 1686385306.026888}}}, metadata={'stream': 'primary', 'DIID': 353, 'RID': 'd3471acc-309d-43b7-8ff8-f986c3fdecf1', 'point_id': 49, 'scan_id': '8e234698-358e-402d-a272-73e168a72f66', 'queue_id': '7a232746-6c90-44f5-81f5-74ab0ea22d4a'})
     """
 
     msg_type: ClassVar[str] = "device_message"
-    signals: dict = Field(default_factory=dict)
+    signals: dict[str, dict[Literal["value", "timestamp"], Any]]
 
 
 class DeviceRPCMessage(BECMessage):
     """Message type for sending device RPC return values from the device server
 
     Args:
         device (str): Device name.
```

### Comparing `bec_lib-2.9.3/bec_lib/numpy_encoder.py` & `bec_lib-2.9.4/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/observer.py` & `bec_lib-2.9.4/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/pdf_writer.py` & `bec_lib-2.9.4/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/plugin_helper.py` & `bec_lib-2.9.4/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/queue_items.py` & `bec_lib-2.9.4/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/redis_connector.py` & `bec_lib-2.9.4/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/request_items.py` & `bec_lib-2.9.4/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/scan_data.py` & `bec_lib-2.9.4/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/scan_items.py` & `bec_lib-2.9.4/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/scan_manager.py` & `bec_lib-2.9.4/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/scan_report.py` & `bec_lib-2.9.4/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/scans.py` & `bec_lib-2.9.4/bec_lib/scans.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,17 @@
             metadata["scan_def_id"] = scans._scan_def_id
         if scans._dataset_id_on_hold:
             metadata["dataset_id_on_hold"] = scans._dataset_id_on_hold
 
         kwargs["md"] = metadata
 
         request = Scans.prepare_scan_request(self.scan_name, self.scan_info, *args, **kwargs)
-        requestID = str(uuid.uuid4())  # TODO: move this to the API server
+        requestID = str(uuid.uuid4())
+
+        # pylint: disable=unsupported-assignment-operation
         request.metadata["RID"] = requestID
 
         self._send_scan_request(request)
 
         report = ScanReport.from_request(request, client=self.client)
         report.request.callbacks.register_many("scan_segment", callback, sync=True)
         report.request.callbacks.register_many("scan_segment", async_callback, sync=False)
```

### Comparing `bec_lib-2.9.3/bec_lib/scibec_validator.py` & `bec_lib-2.9.4/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/serialization.py` & `bec_lib-2.9.4/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/service_config.py` & `bec_lib-2.9.4/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/signature_serializer.py` & `bec_lib-2.9.4/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/user_scripts_mixin.py` & `bec_lib-2.9.4/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/utils.py` & `bec_lib-2.9.4/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/configs/demo_config.yaml` & `bec_lib-2.9.4/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/configs/openapi_schema.json` & `bec_lib-2.9.4/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/tests/fixtures.py` & `bec_lib-2.9.4/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/tests/test_config.yaml` & `bec_lib-2.9.4/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/bec_lib/tests/utils.py` & `bec_lib-2.9.4/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_async_data.py` & `bec_lib-2.9.4/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_beamline_checks.py` & `bec_lib-2.9.4/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_bec_logger.py` & `bec_lib-2.9.4/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_bec_messages.py` & `bec_lib-2.9.4/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_bec_service.py` & `bec_lib-2.9.4/tests/test_bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_bl_conditions.py` & `bec_lib-2.9.4/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_callback_handler.py` & `bec_lib-2.9.4/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_channel_monitor.py` & `bec_lib-2.9.4/tests/test_channel_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from bec_lib import messages
 from bec_lib.channel_monitor import channel_callback, channel_monitor_launch, log_callback
 from bec_lib.redis_connector import MessageObject
 
 
 def test_channel_monitor_callback():
     with mock.patch("builtins.print") as mock_print:
-        msg = messages.DeviceMessage(signals={"x": 1, "y": 2, "z": 3}, metadata={"name": "test"})
+        msg = messages.DeviceMessage(
+            signals={"x": {"value": 1}, "y": {"value": 2}}, metadata={"name": "test"}
+        )
         msg_obj = MessageObject("test", msg)
         channel_callback(msg_obj)
         mock_print.assert_called_once()
 
 
 def test_channel_monitor_start_register():
     with mock.patch("bec_lib.channel_monitor.argparse") as mock_argparse:
```

### Comparing `bec_lib-2.9.3/tests/test_config_helper.py` & `bec_lib-2.9.4/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_core_utils.py` & `bec_lib-2.9.4/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_dap_plugins.py` & `bec_lib-2.9.4/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_device_manager.py` & `bec_lib-2.9.4/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_devices.py` & `bec_lib-2.9.4/tests/test_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,15 +596,15 @@
     console.print.assert_called_once()
 
 
 def test_adjustable_mixin_limits():
     adj = AdjustableMixin()
     adj.root = mock.MagicMock()
     adj.root.parent.connector.get.return_value = messages.DeviceMessage(
-        signals={"low": -12, "high": 12}, metadata={}
+        signals={"low": {"value": -12}, "high": {"value": 12}}, metadata={}
     )
     assert adj.limits == [-12, 12]
 
 
 def test_adjustable_mixin_limits_missing():
     adj = AdjustableMixin()
     adj.root = mock.MagicMock()
@@ -620,26 +620,26 @@
 
 
 def test_adjustable_mixin_set_low_limit():
     adj = AdjustableMixin()
     adj.update_config = mock.MagicMock()
     adj.root = mock.MagicMock()
     adj.root.parent.connector.get.return_value = messages.DeviceMessage(
-        signals={"low": -12, "high": 12}, metadata={}
+        signals={"low": {"value": -12}, "high": {"value": 12}}, metadata={}
     )
     adj.low_limit = -20
     adj.update_config.assert_called_once_with({"deviceConfig": {"limits": [-20, 12]}})
 
 
 def test_adjustable_mixin_set_high_limit():
     adj = AdjustableMixin()
     adj.update_config = mock.MagicMock()
     adj.root = mock.MagicMock()
     adj.root.parent.connector.get.return_value = messages.DeviceMessage(
-        signals={"low": -12, "high": 12}, metadata={}
+        signals={"low": {"value": -12}, "high": {"value": 12}}, metadata={}
     )
     adj.high_limit = 20
     adj.update_config.assert_called_once_with({"deviceConfig": {"limits": [-12, 20]}})
 
 
 def test_computed_signal_set_compute_method():
     comp_signal = ComputedSignal(name="comp_signal", parent=mock.MagicMock())
```

### Comparing `bec_lib-2.9.3/tests/test_file_utils.py` & `bec_lib-2.9.4/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_lmfit_serializer.py` & `bec_lib-2.9.4/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_observer.py` & `bec_lib-2.9.4/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_plugin_helper.py` & `bec_lib-2.9.4/tests/test_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_redis_connector.py` & `bec_lib-2.9.4/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_redis_connector_fakeredis.py` & `bec_lib-2.9.4/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_scan_context.py` & `bec_lib-2.9.4/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_scan_data.py` & `bec_lib-2.9.4/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_scan_items.py` & `bec_lib-2.9.4/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_scan_manager.py` & `bec_lib-2.9.4/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_scan_object.py` & `bec_lib-2.9.4/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_scan_report.py` & `bec_lib-2.9.4/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_serializer.py` & `bec_lib-2.9.4/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_signature_serializer.py` & `bec_lib-2.9.4/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_user_scripts_mixin.py` & `bec_lib-2.9.4/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/tests/test_yaml_loader.py` & `bec_lib-2.9.4/tests/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/create_plugin_structure.py` & `bec_lib-2.9.4/util_scripts/create_plugin_structure.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/init_config.py` & `bec_lib-2.9.4/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/plugin_setup_files/README_template_tests.md` & `bec_lib-2.9.4/util_scripts/plugin_setup_files/README_template_tests.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/plugin_setup_files/gitignore` & `bec_lib-2.9.4/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/plugin_setup_files/post_startup.py` & `bec_lib-2.9.4/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/plugin_setup_files/pyproject.toml` & `bec_lib-2.9.4/util_scripts/plugin_setup_files/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/util_scripts/plugin_setup_files/scan_plugin_template.py` & `bec_lib-2.9.4/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/.gitignore` & `bec_lib-2.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_lib-2.9.3/pyproject.toml` & `bec_lib-2.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.9.3"
+version = "2.9.4"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
@@ -60,7 +60,14 @@
 
 [tool.hatch.build.targets.wheel]
 include = ["*"]
 
 [tool.black]
 line-length = 100
 skip-magic-trailing-comma = true
+
+[tool.isort]
+profile = "black"
+line_length = 100
+multi_line_output = 3
+include_trailing_comma = true
+known_first_party = ["bec_lib", "bec_server", "bec_ipython_client"]
```

### Comparing `bec_lib-2.9.3/PKG-INFO` & `bec_lib-2.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec_lib
-Version: 2.9.3
+Version: 2.9.4
 Summary: BEC library
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

