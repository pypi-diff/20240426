# Comparing `tmp/bec_lib-2.7.1.tar.gz` & `tmp/bec_lib-2.7.2.tar.gz`

## Comparing `bec_lib-2.7.1.tar` & `bec_lib-2.7.2.tar`

### file list

```diff
@@ -1,90 +1,93 @@
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.7.1/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/bec_service.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/client.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/connector.py
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    30828 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/device.py
--rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/logger.py
--rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/queue_items.py
--rw-r--r--   0        0        0    38959 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/request_items.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/scan_data.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/scan_report.py
--rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.7.1/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_bec_logger.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_callback_handler.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_config_helper.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_core_utils.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_device_manager.py
--rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_file_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_redis_connector.py
--rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scan_data.py
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scan_items.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.7.1/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/init_config.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/plugin_setup_files/setup.cfg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bec_lib-2.7.1/util_scripts/plugin_setup_files/setup.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.7.1/.gitignore
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 bec_lib-2.7.1/pyproject.toml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 bec_lib-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.7.2/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/client.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/connector.py
+-rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    30828 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/device.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/logger.py
+-rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    39044 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.7.2/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_file_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.7.2/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 bec_lib-2.7.2/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.7.2/.gitignore
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 bec_lib-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 bec_lib-2.7.2/PKG-INFO
```

### Comparing `bec_lib-2.7.1/README.md` & `bec_lib-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/__init__.py` & `bec_lib-2.7.2/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/alarm_handler.py` & `bec_lib-2.7.2/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/async_data.py` & `bec_lib-2.7.2/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/bec_service.py` & `bec_lib-2.7.2/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/bl_checks.py` & `bec_lib-2.7.2/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/bl_conditions.py` & `bec_lib-2.7.2/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/callback_handler.py` & `bec_lib-2.7.2/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/channel_monitor.py` & `bec_lib-2.7.2/bec_lib/channel_monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     print(json.dumps(out, indent=4, default=lambda o: "<not serializable object>"))
 
 
 def _start_register(config_path, topic):
     config = ServiceConfig(config_path)
     connector = RedisConnector(config.redis)
     register = connector.register(topics=topic, cb=channel_callback)
-    register.start()
     event = threading.Event()
     event.wait()
 
 
 def channel_monitor_launch():
     """
     Launch a channel monitor for a given channel.
```

### Comparing `bec_lib-2.7.1/bec_lib/client.py` & `bec_lib-2.7.2/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/config_helper.py` & `bec_lib-2.7.2/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/connector.py` & `bec_lib-2.7.2/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/dap_plugin_objects.py` & `bec_lib-2.7.2/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/dap_plugins.py` & `bec_lib-2.7.2/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/device.py` & `bec_lib-2.7.2/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/devicemanager.py` & `bec_lib-2.7.2/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/endpoints.py` & `bec_lib-2.7.2/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/file_utils.py` & `bec_lib-2.7.2/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/lmfit_serializer.py` & `bec_lib-2.7.2/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/logbook_connector.py` & `bec_lib-2.7.2/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/logger.py` & `bec_lib-2.7.2/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/messages.py` & `bec_lib-2.7.2/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/numpy_encoder.py` & `bec_lib-2.7.2/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/observer.py` & `bec_lib-2.7.2/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/pdf_writer.py` & `bec_lib-2.7.2/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/plugin_helper.py` & `bec_lib-2.7.2/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/queue_items.py` & `bec_lib-2.7.2/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/redis_connector.py` & `bec_lib-2.7.2/bec_lib/redis_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,20 +566,22 @@
             patterns = self._normalize_patterns(patterns)
             # see if registered streams can be unregistered
             for pattern in patterns:
                 self._unregister_stream(
                     fnmatch.filter(self._stream_topics_subscription, pattern), cb
                 )
             pubsub_unsubscribe_list = self._filter_topics_cb(patterns, cb)
-            self._pubsub_conn.punsubscribe(pubsub_unsubscribe_list)
+            if pubsub_unsubscribe_list:
+                self._pubsub_conn.punsubscribe(pubsub_unsubscribe_list)
         else:
             topics, _ = self._convert_endpointinfo(topics, check_message_op=False)
             if not self._unregister_stream(topics, cb):
                 unsubscribe_list = self._filter_topics_cb(topics, cb)
-                self._pubsub_conn.unsubscribe(unsubscribe_list)
+                if unsubscribe_list:
+                    self._pubsub_conn.unsubscribe(unsubscribe_list)
 
     def _unregister_stream(self, topics: list[str], cb: callable = None) -> bool:
         """
         Unregister a stream listener.
 
         Args:
             topics (list[str]): list of stream topics
```

### Comparing `bec_lib-2.7.1/bec_lib/request_items.py` & `bec_lib-2.7.2/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/scan_data.py` & `bec_lib-2.7.2/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/scan_items.py` & `bec_lib-2.7.2/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/scan_manager.py` & `bec_lib-2.7.2/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/scan_report.py` & `bec_lib-2.7.2/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/scans.py` & `bec_lib-2.7.2/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/scibec_validator.py` & `bec_lib-2.7.2/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/serialization.py` & `bec_lib-2.7.2/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/service_config.py` & `bec_lib-2.7.2/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/signature_serializer.py` & `bec_lib-2.7.2/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/user_scripts_mixin.py` & `bec_lib-2.7.2/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/utils.py` & `bec_lib-2.7.2/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/configs/demo_config.yaml` & `bec_lib-2.7.2/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/configs/openapi_schema.json` & `bec_lib-2.7.2/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/tests/fixtures.py` & `bec_lib-2.7.2/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/tests/test_config.yaml` & `bec_lib-2.7.2/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/bec_lib/tests/utils.py` & `bec_lib-2.7.2/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_async_data.py` & `bec_lib-2.7.2/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_beamline_checks.py` & `bec_lib-2.7.2/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_bec_logger.py` & `bec_lib-2.7.2/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_bec_messages.py` & `bec_lib-2.7.2/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_bec_service.py` & `bec_lib-2.7.2/tests/test_bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_bl_conditions.py` & `bec_lib-2.7.2/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_callback_handler.py` & `bec_lib-2.7.2/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_channel_monitor.py` & `bec_lib-2.7.2/tests/test_channel_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,8 @@
                     clargs.config = "test_config"
                     clargs.channel = "test_channel"
                     mock_threading.Event().wait.return_value = True
                     mock_config.return_value = mock.MagicMock()
                     mock_connector.return_value = mock.MagicMock()
                     channel_monitor_launch()
                     mock_connector().register.assert_called_once()
-                    mock_connector().register.return_value.start.assert_called_once()
                     mock_threading.Event().wait.assert_called_once()
```

### Comparing `bec_lib-2.7.1/tests/test_config_helper.py` & `bec_lib-2.7.2/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_core_utils.py` & `bec_lib-2.7.2/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_dap_plugins.py` & `bec_lib-2.7.2/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_device_manager.py` & `bec_lib-2.7.2/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_devices.py` & `bec_lib-2.7.2/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_file_utils.py` & `bec_lib-2.7.2/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_lmfit_serializer.py` & `bec_lib-2.7.2/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_observer.py` & `bec_lib-2.7.2/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_plugin_helper.py` & `bec_lib-2.7.2/tests/test_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_redis_connector.py` & `bec_lib-2.7.2/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_redis_connector_fakeredis.py` & `bec_lib-2.7.2/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_scan_context.py` & `bec_lib-2.7.2/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_scan_data.py` & `bec_lib-2.7.2/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_scan_items.py` & `bec_lib-2.7.2/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_scan_manager.py` & `bec_lib-2.7.2/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_scan_object.py` & `bec_lib-2.7.2/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_scan_report.py` & `bec_lib-2.7.2/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_serializer.py` & `bec_lib-2.7.2/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_signature_serializer.py` & `bec_lib-2.7.2/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/tests/test_user_scripts_mixin.py` & `bec_lib-2.7.2/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/util_scripts/init_config.py` & `bec_lib-2.7.2/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/util_scripts/plugin_setup_files/post_startup.py` & `bec_lib-2.7.2/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/util_scripts/plugin_setup_files/pre_startup.py` & `bec_lib-2.7.2/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/util_scripts/plugin_setup_files/scan_plugin_template.py` & `bec_lib-2.7.2/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/.gitignore` & `bec_lib-2.7.2/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `bec_lib-2.7.1/pyproject.toml` & `bec_lib-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.7.1"
+version = "2.7.2"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `bec_lib-2.7.1/PKG-INFO` & `bec_lib-2.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec_lib
-Version: 2.7.1
+Version: 2.7.2
 Summary: BEC library
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```
