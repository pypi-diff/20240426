# Comparing `tmp/nista_library-4.4.1.tar.gz` & `tmp/nista_library-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.4.1.tar", max compression
+gzip compressed data, was "nista_library-4.5.0.tar", max compression
```

## Comparing `nista_library-4.4.1.tar` & `nista_library-4.5.0.tar`

### file list

```diff
@@ -1,122 +1,126 @@
--rw-r--r--   0        0        0     1117 2024-03-20 14:50:08.928277 nista_library-4.4.1/LICENSE.md
--rw-r--r--   0        0        0     6428 2024-03-20 14:50:08.928277 nista_library-4.4.1/README.md
--rw-r--r--   0        0        0      153 2024-03-20 14:50:08.929277 nista_library-4.4.1/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2024-03-20 14:50:08.929277 nista_library-4.4.1/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 14:50:08.962277 nista_library-4.4.1/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2024-03-20 14:50:08.929277 nista_library-4.4.1/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2024-03-20 14:50:08.968276 nista_library-4.4.1/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     6042 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5525 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5441 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4868 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4873 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     6049 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_finish_execution_result_data.py
--rw-r--r--   0        0        0     5768 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5301 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5622 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     9635 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     5888 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_quality.py
--rw-r--r--   0        0        0     5546 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5518 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     5530 2024-03-20 14:50:08.930277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5530 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0        0 2024-03-20 14:50:08.968276 nista_library-4.4.1/data_point_client/api/data_point_area/__init__.py
--rw-r--r--   0        0        0     5768 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_create_area.py
--rw-r--r--   0        0        0     6225 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_create_area_message.py
--rw-r--r--   0        0        0     5184 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_delete_area.py
--rw-r--r--   0        0        0     5563 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_delete_message.py
--rw-r--r--   0        0        0     5592 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_list_areas.py
--rw-r--r--   0        0        0     5769 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_update_area.py
--rw-r--r--   0        0        0     6226 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_update_message.py
--rw-r--r--   0        0        0        0 2024-03-20 14:50:08.968276 nista_library-4.4.1/data_point_client/api/data_point_manual_input/__init__.py
--rw-r--r--   0        0        0     5621 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py
--rw-r--r--   0        0        0     5413 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py
--rw-r--r--   0        0        0     5628 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py
--rw-r--r--   0        0        0        0 2024-03-20 14:50:08.968276 nista_library-4.4.1/data_point_client/api/data_point_tag/__init__.py
--rw-r--r--   0        0        0     7848 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_tag/data_point_tag_get_tags.py
--rw-r--r--   0        0        0     4954 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py
--rw-r--r--   0        0        0     2817 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/client.py
--rw-r--r--   0        0        0      470 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/errors.py
--rw-r--r--   0        0        0     5758 2024-03-20 14:50:08.931277 nista_library-4.4.1/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1379 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     2319 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/append_manual_input_request.py
--rw-r--r--   0        0        0     2976 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     9207 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     7534 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0     1905 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_point_info.py
--rw-r--r--   0        0        0      779 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     4487 2024-03-20 14:50:08.932277 nista_library-4.4.1/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0    10470 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     1845 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/date_range_dto.py
--rw-r--r--   0        0        0     7569 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     9224 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      240 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_import_options.py
--rw-r--r--   0        0        0      181 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2571 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/finish_execution_result_data_request.py
--rw-r--r--   0        0        0     2579 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     2839 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_data_quality_request.py
--rw-r--r--   0        0        0     4179 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     1922 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_quality_response.py
--rw-r--r--   0        0        0     3053 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2024-03-20 14:50:08.933277 nista_library-4.4.1/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2307 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/manual_input_request.py
--rw-r--r--   0        0        0     2311 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/manual_input_response.py
--rw-r--r--   0        0        0     2045 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/rule.py
--rw-r--r--   0        0        0    12102 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3346 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     1529 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/time_series_quality_response.py
--rw-r--r--   0        0        0     1257 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/time_series_quality_response_curve.py
--rw-r--r--   0        0        0     3686 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2024-03-20 14:50:08.934277 nista_library-4.4.1/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     4428 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     9236 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/py.typed
--rw-r--r--   0        0        0      993 2024-03-20 14:50:08.935277 nista_library-4.4.1/data_point_client/types.py
--rw-r--r--   0        0        0     1007 2024-03-20 14:50:08.936277 nista_library-4.4.1/nista_library/__init__.py
--rw-r--r--   0        0        0    11406 2024-03-20 14:50:08.936277 nista_library-4.4.1/nista_library/nista_connetion.py
--rw-r--r--   0        0        0     1049 2024-03-20 14:50:08.936277 nista_library-4.4.1/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    23757 2024-03-20 14:50:08.936277 nista_library-4.4.1/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1970 2024-03-20 14:50:08.936277 nista_library-4.4.1/nista_library/nista_data_points.py
--rw-r--r--   0        0        0      835 2024-03-20 14:50:08.936277 nista_library-4.4.1/nista_library/nista_date_range.py
--rw-r--r--   0        0        0     1383 2024-03-20 14:50:08.937277 nista_library-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     7522 1970-01-01 00:00:00.000000 nista_library-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1117 2024-04-26 18:00:31.351168 nista_library-4.5.0/LICENSE.md
+-rw-r--r--   0        0        0     6428 2024-04-26 18:00:31.351168 nista_library-4.5.0/README.md
+-rw-r--r--   0        0        0      153 2024-04-26 18:00:31.352168 nista_library-4.5.0/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:00:31.387169 nista_library-4.5.0/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     6042 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5525 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5441 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4868 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4873 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     6049 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_finish_execution_result_data.py
+-rw-r--r--   0        0        0     5768 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5301 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5622 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0    10245 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     5888 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_quality.py
+-rw-r--r--   0        0        0     6027 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_get_quality_statistic.py
+-rw-r--r--   0        0        0     5546 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2024-04-26 18:00:31.353168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5518 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     5530 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5530 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point_area/__init__.py
+-rw-r--r--   0        0        0     5768 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area.py
+-rw-r--r--   0        0        0     6225 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area_message.py
+-rw-r--r--   0        0        0     5184 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_area.py
+-rw-r--r--   0        0        0     5563 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_message.py
+-rw-r--r--   0        0        0     5592 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_list_areas.py
+-rw-r--r--   0        0        0     5769 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_area.py
+-rw-r--r--   0        0        0     6226 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_message.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point_manual_input/__init__.py
+-rw-r--r--   0        0        0     5621 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py
+-rw-r--r--   0        0        0     5413 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py
+-rw-r--r--   0        0        0     5628 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:00:31.388169 nista_library-4.5.0/data_point_client/api/data_point_tag/__init__.py
+-rw-r--r--   0        0        0     7848 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags.py
+-rw-r--r--   0        0        0     4954 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py
+-rw-r--r--   0        0        0     2817 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/errors.py
+-rw-r--r--   0        0        0     6078 2024-04-26 18:00:31.354168 nista_library-4.5.0/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1379 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     2319 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/append_manual_input_request.py
+-rw-r--r--   0        0        0     2976 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     9207 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     7534 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0     1905 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_info.py
+-rw-r--r--   0        0        0     2814 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_list_response.py
+-rw-r--r--   0        0        0     1809 2024-04-26 18:00:31.355168 nista_library-4.5.0/data_point_client/models/data_point_list_response_common_units.py
+-rw-r--r--   0        0        0      779 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     4487 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0    10485 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     1845 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/date_range_dto.py
+-rw-r--r--   0        0        0     7569 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     9224 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      240 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_import_options.py
+-rw-r--r--   0        0        0      181 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2571 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/finish_execution_result_data_request.py
+-rw-r--r--   0        0        0     2579 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     2839 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_data_quality_request.py
+-rw-r--r--   0        0        0     4179 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     1922 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_quality_response.py
+-rw-r--r--   0        0        0     1415 2024-04-26 18:00:31.356168 nista_library-4.5.0/data_point_client/models/get_quality_statistic_response.py
+-rw-r--r--   0        0        0     3053 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2307 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/manual_input_request.py
+-rw-r--r--   0        0        0     2311 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/manual_input_response.py
+-rw-r--r--   0        0        0     2045 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/rule.py
+-rw-r--r--   0        0        0    12102 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3346 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     1529 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_quality_response.py
+-rw-r--r--   0        0        0     1257 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_quality_response_curve.py
+-rw-r--r--   0        0        0     3686 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2024-04-26 18:00:31.357168 nista_library-4.5.0/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     4428 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     9236 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/py.typed
+-rw-r--r--   0        0        0      993 2024-04-26 18:00:31.358168 nista_library-4.5.0/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    25077 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1970 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0      835 2024-04-26 18:00:31.359168 nista_library-4.5.0/nista_library/nista_date_range.py
+-rw-r--r--   0        0        0     1383 2024-04-26 18:00:31.360168 nista_library-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7522 1970-01-01 00:00:00.000000 nista_library-4.5.0/PKG-INFO
```

### Comparing `nista_library-4.4.1/LICENSE.md` & `nista_library-4.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/README.md` & `nista_library-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-4.5.0/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_finish_execution_result_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_finish_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.data_point_response_base import DataPointResponseBase
+from ...models.data_point_list_response import DataPointListResponse
 from ...models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from ...models.en_data_point_type import EnDataPointType
 from ...models.problem_details import ProblemDetails
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
@@ -17,14 +17,15 @@
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
     existence: Union[Unset, None, List[EnDataPointExistenceDTO]] = UNSET,
     filter_smart_query: Union[Unset, None, str] = UNSET,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
     facility: Union[Unset, None, str] = UNSET,
+    filter_ids: Union[Unset, None, List[str]] = UNSET,
 ) -> Dict[str, Any]:
     url = "{}/DataPoint/workspace/{workspaceId}/dataPoint".format(client.base_url, workspaceId=workspace_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
@@ -63,14 +64,23 @@
         else:
             json_filter_tags = filter_tags
 
     params["filterTags"] = json_filter_tags
 
     params["facility"] = facility
 
+    json_filter_ids: Union[Unset, None, List[str]] = UNSET
+    if not isinstance(filter_ids, Unset):
+        if filter_ids is None:
+            json_filter_ids = None
+        else:
+            json_filter_ids = filter_ids
+
+    params["filterIds"] = json_filter_ids
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
@@ -78,22 +88,17 @@
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[Union[List["DataPointResponseBase"], ProblemDetails]]:
+) -> Optional[Union[DataPointListResponse, ProblemDetails]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = DataPointResponseBase.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = DataPointListResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = ProblemDetails.from_dict(response.json())
 
         return response_400
     if response.status_code == HTTPStatus.UNAUTHORIZED:
@@ -108,15 +113,15 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[Union[List["DataPointResponseBase"], ProblemDetails]]:
+) -> Response[Union[DataPointListResponse, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -126,40 +131,43 @@
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
     existence: Union[Unset, None, List[EnDataPointExistenceDTO]] = UNSET,
     filter_smart_query: Union[Unset, None, str] = UNSET,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
     facility: Union[Unset, None, str] = UNSET,
-) -> Response[Union[List["DataPointResponseBase"], ProblemDetails]]:
+    filter_ids: Union[Unset, None, List[str]] = UNSET,
+) -> Response[Union[DataPointListResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
         facility (Union[Unset, None, str]):
+        filter_ids (Union[Unset, None, List[str]]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[List['DataPointResponseBase'], ProblemDetails]]
+        Response[Union[DataPointListResponse, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         client=client,
         type=type,
         existence=existence,
         filter_smart_query=filter_smart_query,
         filter_tags=filter_tags,
         facility=facility,
+        filter_ids=filter_ids,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
@@ -171,78 +179,84 @@
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
     existence: Union[Unset, None, List[EnDataPointExistenceDTO]] = UNSET,
     filter_smart_query: Union[Unset, None, str] = UNSET,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
     facility: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[List["DataPointResponseBase"], ProblemDetails]]:
+    filter_ids: Union[Unset, None, List[str]] = UNSET,
+) -> Optional[Union[DataPointListResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
         facility (Union[Unset, None, str]):
+        filter_ids (Union[Unset, None, List[str]]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[List['DataPointResponseBase'], ProblemDetails]
+        Union[DataPointListResponse, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         client=client,
         type=type,
         existence=existence,
         filter_smart_query=filter_smart_query,
         filter_tags=filter_tags,
         facility=facility,
+        filter_ids=filter_ids,
     ).parsed
 
 
 async def asyncio_detailed(
     workspace_id: str,
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
     existence: Union[Unset, None, List[EnDataPointExistenceDTO]] = UNSET,
     filter_smart_query: Union[Unset, None, str] = UNSET,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
     facility: Union[Unset, None, str] = UNSET,
-) -> Response[Union[List["DataPointResponseBase"], ProblemDetails]]:
+    filter_ids: Union[Unset, None, List[str]] = UNSET,
+) -> Response[Union[DataPointListResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
         facility (Union[Unset, None, str]):
+        filter_ids (Union[Unset, None, List[str]]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[List['DataPointResponseBase'], ProblemDetails]]
+        Response[Union[DataPointListResponse, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         client=client,
         type=type,
         existence=existence,
         filter_smart_query=filter_smart_query,
         filter_tags=filter_tags,
         facility=facility,
+        filter_ids=filter_ids,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
@@ -252,36 +266,39 @@
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
     existence: Union[Unset, None, List[EnDataPointExistenceDTO]] = UNSET,
     filter_smart_query: Union[Unset, None, str] = UNSET,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
     facility: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[List["DataPointResponseBase"], ProblemDetails]]:
+    filter_ids: Union[Unset, None, List[str]] = UNSET,
+) -> Optional[Union[DataPointListResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
         facility (Union[Unset, None, str]):
+        filter_ids (Union[Unset, None, List[str]]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[List['DataPointResponseBase'], ProblemDetails]
+        Union[DataPointListResponse, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             client=client,
             type=type,
             existence=existence,
             filter_smart_query=filter_smart_query,
             filter_tags=filter_tags,
             facility=facility,
+            filter_ids=filter_ids,
         )
     ).parsed
```

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_get_data_quality.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_get_data_quality.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-4.5.0/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_create_area.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_create_area_message.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_delete_area.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_delete_message.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_list_areas.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_update_area.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_area/data_point_area_update_message.py` & `nista_library-4.5.0/data_point_client/api/data_point_area/data_point_area_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py` & `nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_append_manual_inputs.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py` & `nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_get_manual_inputs.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py` & `nista_library-4.5.0/data_point_client/api/data_point_manual_input/data_point_manual_input_update_manual_inputs.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_tag/data_point_tag_get_tags.py` & `nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py` & `nista_library-4.5.0/data_point_client/api/data_point_tag/data_point_tag_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/client.py` & `nista_library-4.5.0/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/__init__.py` & `nista_library-4.5.0/data_point_client/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from .create_area_request import CreateAreaRequest
 from .data_bucket_base import DataBucketBase
 from .data_export_request import DataExportRequest
 from .data_point_comment_message_response import DataPointCommentMessageResponse
 from .data_point_data_base import DataPointDataBase
 from .data_point_data_response import DataPointDataResponse
 from .data_point_info import DataPointInfo
+from .data_point_list_response import DataPointListResponse
+from .data_point_list_response_common_units import DataPointListResponseCommonUnits
 from .data_point_origin import DataPointOrigin
 from .data_point_request import DataPointRequest
 from .data_point_response_base import DataPointResponseBase
 from .date_range_dto import DateRangeDTO
 from .day_data_by_hour_transfer import DayDataByHourTransfer
 from .day_period_data_bucket import DayPeriodDataBucket
 from .day_period_data_point_data import DayPeriodDataPointData
@@ -35,14 +37,15 @@
 from .finish_execution_result_data_request import FinishExecutionResultDataRequest
 from .get_constant_response import GetConstantResponse
 from .get_data_quality_request import GetDataQualityRequest
 from .get_data_request import GetDataRequest
 from .get_data_response import GetDataResponse
 from .get_day_period_response import GetDayPeriodResponse
 from .get_quality_response import GetQualityResponse
+from .get_quality_statistic_response import GetQualityStatisticResponse
 from .get_series_response import GetSeriesResponse
 from .get_week_period_response import GetWeekPeriodResponse
 from .gnista_unit_response import GnistaUnitResponse
 from .live_data_origin import LiveDataOrigin
 from .location_rest import LocationRest
 from .manual_input_request import ManualInputRequest
 from .manual_input_response import ManualInputResponse
@@ -83,14 +86,16 @@
     "CreateAreaRequest",
     "DataBucketBase",
     "DataExportRequest",
     "DataPointCommentMessageResponse",
     "DataPointDataBase",
     "DataPointDataResponse",
     "DataPointInfo",
+    "DataPointListResponse",
+    "DataPointListResponseCommonUnits",
     "DataPointOrigin",
     "DataPointRequest",
     "DataPointResponseBase",
     "DateRangeDTO",
     "DayDataByHourTransfer",
     "DayPeriodDataBucket",
     "DayPeriodDataPointData",
@@ -106,14 +111,15 @@
     "FinishExecutionResultDataRequest",
     "GetConstantResponse",
     "GetDataQualityRequest",
     "GetDataRequest",
     "GetDataResponse",
     "GetDayPeriodResponse",
     "GetQualityResponse",
+    "GetQualityStatisticResponse",
     "GetSeriesResponse",
     "GetWeekPeriodResponse",
     "GnistaUnitResponse",
     "LiveDataOrigin",
     "LocationRest",
     "ManualInputRequest",
     "ManualInputResponse",
```

### Comparing `nista_library-4.4.1/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.5.0/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/append_manual_input_request.py` & `nista_library-4.5.0/data_point_client/models/append_manual_input_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/append_time_series_request.py` & `nista_library-4.5.0/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/area_of_interest_response.py` & `nista_library-4.5.0/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/calculation_origin.py` & `nista_library-4.5.0/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/constant_data_bucket.py` & `nista_library-4.5.0/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/constant_data_point_data.py` & `nista_library-4.5.0/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/continuous_location_rest.py` & `nista_library-4.5.0/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/create_area_message_request.py` & `nista_library-4.5.0/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/create_area_request.py` & `nista_library-4.5.0/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_bucket_base.py` & `nista_library-4.5.0/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_export_request.py` & `nista_library-4.5.0/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_comment_message_response.py` & `nista_library-4.5.0/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_data_base.py` & `nista_library-4.5.0/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_data_response.py` & `nista_library-4.5.0/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_info.py` & `nista_library-4.5.0/data_point_client/models/data_point_info.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_origin.py` & `nista_library-4.5.0/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_request.py` & `nista_library-4.5.0/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/data_point_response_base.py` & `nista_library-4.5.0/data_point_client/models/data_point_response_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         state (Union[Unset, EnDataPointStateDTO]):
         existence (Union[Unset, EnDataPointExistenceDTO]):
         error_details (Union[Unset, None, str]):
         origin (Union[Unset, None, DataPointOrigin]):
         used_in_calculations (Union[Unset, None, List[str]]):
         used_in_reports (Union[Unset, None, List[str]]):
         used_in_analysis (Union[Unset, None, List[str]]):
-        used_in_insights (Union[Unset, None, List[str]]):
+        used_in_violation (Union[Unset, None, List[str]]):
         used_in_tasks (Union[Unset, None, List[str]]):
         base_64_thumbnail (Union[Unset, None, str]):
     """
 
     data_point_id: str
     created_on: datetime.datetime
     facility_id: Union[Unset, None, str] = UNSET
@@ -54,15 +54,15 @@
     state: Union[Unset, EnDataPointStateDTO] = UNSET
     existence: Union[Unset, EnDataPointExistenceDTO] = UNSET
     error_details: Union[Unset, None, str] = UNSET
     origin: Union[Unset, None, "DataPointOrigin"] = UNSET
     used_in_calculations: Union[Unset, None, List[str]] = UNSET
     used_in_reports: Union[Unset, None, List[str]] = UNSET
     used_in_analysis: Union[Unset, None, List[str]] = UNSET
-    used_in_insights: Union[Unset, None, List[str]] = UNSET
+    used_in_violation: Union[Unset, None, List[str]] = UNSET
     used_in_tasks: Union[Unset, None, List[str]] = UNSET
     base_64_thumbnail: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         data_point_id = self.data_point_id
         created_on = self.created_on.isoformat()
 
@@ -115,20 +115,20 @@
         used_in_analysis: Union[Unset, None, List[str]] = UNSET
         if not isinstance(self.used_in_analysis, Unset):
             if self.used_in_analysis is None:
                 used_in_analysis = None
             else:
                 used_in_analysis = self.used_in_analysis
 
-        used_in_insights: Union[Unset, None, List[str]] = UNSET
-        if not isinstance(self.used_in_insights, Unset):
-            if self.used_in_insights is None:
-                used_in_insights = None
+        used_in_violation: Union[Unset, None, List[str]] = UNSET
+        if not isinstance(self.used_in_violation, Unset):
+            if self.used_in_violation is None:
+                used_in_violation = None
             else:
-                used_in_insights = self.used_in_insights
+                used_in_violation = self.used_in_violation
 
         used_in_tasks: Union[Unset, None, List[str]] = UNSET
         if not isinstance(self.used_in_tasks, Unset):
             if self.used_in_tasks is None:
                 used_in_tasks = None
             else:
                 used_in_tasks = self.used_in_tasks
@@ -166,16 +166,16 @@
             field_dict["origin"] = origin
         if used_in_calculations is not UNSET:
             field_dict["usedInCalculations"] = used_in_calculations
         if used_in_reports is not UNSET:
             field_dict["usedInReports"] = used_in_reports
         if used_in_analysis is not UNSET:
             field_dict["usedInAnalysis"] = used_in_analysis
-        if used_in_insights is not UNSET:
-            field_dict["usedInInsights"] = used_in_insights
+        if used_in_violation is not UNSET:
+            field_dict["usedInViolation"] = used_in_violation
         if used_in_tasks is not UNSET:
             field_dict["usedInTasks"] = used_in_tasks
         if base_64_thumbnail is not UNSET:
             field_dict["base64Thumbnail"] = base_64_thumbnail
 
         return field_dict
 
@@ -245,15 +245,15 @@
 
         used_in_calculations = cast(List[str], d.pop("usedInCalculations", UNSET))
 
         used_in_reports = cast(List[str], d.pop("usedInReports", UNSET))
 
         used_in_analysis = cast(List[str], d.pop("usedInAnalysis", UNSET))
 
-        used_in_insights = cast(List[str], d.pop("usedInInsights", UNSET))
+        used_in_violation = cast(List[str], d.pop("usedInViolation", UNSET))
 
         used_in_tasks = cast(List[str], d.pop("usedInTasks", UNSET))
 
         base_64_thumbnail = d.pop("base64Thumbnail", UNSET)
 
         data_point_response_base = cls(
             data_point_id=data_point_id,
@@ -268,13 +268,13 @@
             state=state,
             existence=existence,
             error_details=error_details,
             origin=origin,
             used_in_calculations=used_in_calculations,
             used_in_reports=used_in_reports,
             used_in_analysis=used_in_analysis,
-            used_in_insights=used_in_insights,
+            used_in_violation=used_in_violation,
             used_in_tasks=used_in_tasks,
             base_64_thumbnail=base_64_thumbnail,
         )
 
         return data_point_response_base
```

### Comparing `nista_library-4.4.1/data_point_client/models/date_range_dto.py` & `nista_library-4.5.0/data_point_client/models/date_range_dto.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.5.0/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.5.0/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.5.0/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/file_origin.py` & `nista_library-4.5.0/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/finish_execution_result_data_request.py` & `nista_library-4.5.0/data_point_client/models/finish_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_constant_response.py` & `nista_library-4.5.0/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_data_quality_request.py` & `nista_library-4.5.0/data_point_client/models/get_data_quality_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_data_request.py` & `nista_library-4.5.0/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_data_response.py` & `nista_library-4.5.0/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_day_period_response.py` & `nista_library-4.5.0/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_quality_response.py` & `nista_library-4.5.0/data_point_client/models/get_quality_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_series_response.py` & `nista_library-4.5.0/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/get_week_period_response.py` & `nista_library-4.5.0/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/gnista_unit_response.py` & `nista_library-4.5.0/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/live_data_origin.py` & `nista_library-4.5.0/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/location_rest.py` & `nista_library-4.5.0/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/manual_input_request.py` & `nista_library-4.5.0/data_point_client/models/manual_input_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/manual_input_response.py` & `nista_library-4.5.0/data_point_client/models/manual_input_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/point_location_rest.py` & `nista_library-4.5.0/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/problem_details.py` & `nista_library-4.5.0/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/problem_details_extensions.py` & `nista_library-4.5.0/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/remote_origin.py` & `nista_library-4.5.0/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/rule.py` & `nista_library-4.5.0/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/series_data_bucket.py` & `nista_library-4.5.0/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/series_data_point_data.py` & `nista_library-4.5.0/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/sub_series_request.py` & `nista_library-4.5.0/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/sub_series_request_values.py` & `nista_library-4.5.0/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/time_series_period.py` & `nista_library-4.5.0/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/time_series_quality_response.py` & `nista_library-4.5.0/data_point_client/models/time_series_quality_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/time_series_quality_response_curve.py` & `nista_library-4.5.0/data_point_client/models/time_series_quality_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/time_series_response.py` & `nista_library-4.5.0/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/time_series_response_curve.py` & `nista_library-4.5.0/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/update_area_message_request.py` & `nista_library-4.5.0/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/update_area_request.py` & `nista_library-4.5.0/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/update_constant_data_request.py` & `nista_library-4.5.0/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/update_day_period_request.py` & `nista_library-4.5.0/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/update_time_series_request.py` & `nista_library-4.5.0/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/update_week_period_request.py` & `nista_library-4.5.0/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/week_data_transfere.py` & `nista_library-4.5.0/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.5.0/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.5.0/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/data_point_client/types.py` & `nista_library-4.5.0/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/nista_library/__init__.py` & `nista_library-4.5.0/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/nista_library/nista_connetion.py` & `nista_library-4.5.0/nista_library/nista_connetion.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/nista_library/nista_credential_manager.py` & `nista_library-4.5.0/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/nista_library/nista_data_point.py` & `nista_library-4.5.0/nista_library/nista_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     data_point_get_data,
     data_point_get_data_point,
     data_point_update_constant_data,
     data_point_update_time_series_data,
     data_point_update_week_period_data,
     data_point_update_data_point,
     data_point_get_data_quality,
+    data_point_get_quality_statistic,
 )
 from data_point_client.models import GetConstantResponse, GetSeriesResponse
 from data_point_client.models.append_execution_result_data_request import (
     AppendExecutionResultDataRequest,
 )
 from data_point_client.models.append_time_series_request import AppendTimeSeriesRequest
 from data_point_client.models.constant_data_bucket import ConstantDataBucket
@@ -34,14 +35,15 @@
 from data_point_client.models.day_data_by_hour_transfer import DayDataByHourTransfer
 from data_point_client.models.day_period_data_bucket import DayPeriodDataBucket
 from data_point_client.models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from data_point_client.models.finish_execution_result_data_request import FinishExecutionResultDataRequest
 from data_point_client.models.get_data_quality_request import GetDataQualityRequest
 from data_point_client.models.get_data_request import GetDataRequest
 from data_point_client.models.get_day_period_response import GetDayPeriodResponse
+from data_point_client.models.get_quality_statistic_response import GetQualityStatisticResponse
 from data_point_client.models.get_week_period_response import GetWeekPeriodResponse
 from data_point_client.models.problem_details import ProblemDetails
 from data_point_client.models.series_data_bucket import SeriesDataBucket
 from data_point_client.models.sub_series_request import SubSeriesRequest
 from data_point_client.models.sub_series_request_values import SubSeriesRequestValues
 from data_point_client.models.time_series_quality_response_curve import TimeSeriesQualityResponseCurve
 from data_point_client.models.time_series_response_curve import TimeSeriesResponseCurve
@@ -268,14 +270,48 @@
                     )
                     data_frames.append(data_frame)
 
             return data_frames
 
         return None
 
+    def get_data_point_quality_statistic(
+        self,
+        request: GetDataQualityRequest,
+        timeout: float = 30,
+    ) -> Union[GetQualityStatisticResponse, None]:
+        """Retrieves the Quality Metric Statistic from a DataPoint
+        :param request: Request details for retrieving Data Quality
+        :param timeout: How long to wait for response
+        :return: The DataPoint Quality Metric
+        """
+        token = self.connection.get_access_token()
+        client = AuthenticatedClient(
+            base_url=self.connection.datapoint_base_url,
+            token=token,
+            verify_ssl=self.connection.verify_ssl,
+            timeout=timeout,
+        )
+
+        series_response = data_point_get_quality_statistic.sync(
+            client=client,
+            data_point_id=self.data_point_id,
+            workspace_id=self.connection.workspace_id,
+            json_body=request,
+        )
+
+        if series_response is None:
+            raise ValueError("Cannot load Datapoint")
+
+        if isinstance(series_response, ProblemDetails):
+            log.error(series_response.detail)
+            raise ValueError("Cannot load Datapoint")
+
+        return series_response
+
     # pylint: disable=too-many-arguments
     # pylint: disable=too-many-branches
     def get_data_point_data(
         self,
         request: GetDataRequest,
         post_fix: bool = False,
         timeout: float = 30,
@@ -417,16 +453,17 @@
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
 
         sub_series_as_data_range_dto = None
         if sub_series_ranges is not None:
-            sub_series_as_data_range_dto = [sub_series_range.to_data_range_dto(time_zone)
-                                            for sub_series_range in sub_series_ranges]
+            sub_series_as_data_range_dto = [
+                sub_series_range.to_data_range_dto(time_zone) for sub_series_range in sub_series_ranges
+            ]
 
         append_request = FinishExecutionResultDataRequest(
             unit=unit,
             time_zone=time_zone.key,
             is_major_change=is_major_change,
             sub_series=sub_series_as_data_range_dto,
         )
```

### Comparing `nista_library-4.4.1/nista_library/nista_data_points.py` & `nista_library-4.5.0/nista_library/nista_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/nista_library/nista_date_range.py` & `nista_library-4.5.0/nista_library/nista_date_range.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.4.1/pyproject.toml` & `nista_library-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.4.1"
+version = "4.5.0"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
```

### Comparing `nista_library-4.4.1/PKG-INFO` & `nista_library-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nista-library
-Version: 4.4.1
+Version: 4.5.0
 Summary: A client library for accessing nista.io
 Home-page: https://nista.io
 License: MIT
 Author: Markus Hoffmann
 Author-email: markus.hoffmann@nista.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

