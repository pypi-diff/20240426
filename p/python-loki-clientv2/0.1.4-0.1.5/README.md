# Comparing `tmp/python_loki_clientv2-0.1.4.tar.gz` & `tmp/python_loki_clientv2-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_loki_clientv2-0.1.4.tar", max compression
+gzip compressed data, was "python_loki_clientv2-0.1.5.tar", max compression
```

## Comparing `python_loki_clientv2-0.1.4.tar` & `python_loki_clientv2-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,49 @@
--rw-r--r--   0        0        0     1072 2024-04-09 16:38:02.232240 python_loki_clientv2-0.1.4/LICENSE
--rw-r--r--   0        0        0     3495 2024-04-09 16:38:02.232240 python_loki_clientv2-0.1.4/README.md
--rw-r--r--   0        0        0      155 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/__init__.py
--rw-r--r--   0        0        0       45 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/build_info/__init__.py
--rw-r--r--   0        0        0     3311 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/build_info/get_loki_api_v1_status_buildinfo.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/format_query/__init__.py
--rw-r--r--   0        0        0     3826 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/format_query/get_loki_api_v1_format_query.py
--rw-r--r--   0        0        0     4132 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/format_query/post_loki_api_v1_format_query.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/labels/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/labels/get_loki_api_v1_labels.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/query/__init__.py
--rw-r--r--   0        0        0     6036 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/query/get_loki_api_v1_query.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/query_range/__init__.py
--rw-r--r--   0        0        0     9005 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/query_range/get_loki_api_v1_query_range.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/ready/__init__.py
--rw-r--r--   0        0        0     2086 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/ready/get_ready.py
--rw-r--r--   0        0        0        0 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/services/__init__.py
--rw-r--r--   0        0        0     4386 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/api/services/get_services.py
--rw-r--r--   0        0        0    12509 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/client.py
--rw-r--r--   0        0        0      546 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/errors.py
--rw-r--r--   0        0        0     2228 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/__init__.py
--rw-r--r--   0        0        0      164 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/direction.py
--rw-r--r--   0        0        0     1953 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_body.py
--rw-r--r--   0        0        0     2708 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_data.py
--rw-r--r--   0        0        0      178 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_data_result_type.py
--rw-r--r--   0        0        0     1957 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_metric.py
--rw-r--r--   0        0        0      205 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_metric_level.py
--rw-r--r--   0        0        0     3054 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_result.py
--rw-r--r--   0        0        0     1228 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_streams.py
--rw-r--r--   0        0        0     2568 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics.py
--rw-r--r--   0        0        0     3147 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_ingester.py
--rw-r--r--   0        0        0     1741 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_querier.py
--rw-r--r--   0        0        0     3041 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_store.py
--rw-r--r--   0        0        0     3086 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_store_chunk.py
--rw-r--r--   0        0        0     4345 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_summary.py
--rw-r--r--   0        0        0      985 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/grafana_loki_client/types.py
--rw-r--r--   0        0        0     1609 2024-04-09 16:38:02.236240 python_loki_clientv2-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 python_loki_clientv2-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3495 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/README.md
+-rw-r--r--   0        0        0      155 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/build_info/__init__.py
+-rw-r--r--   0        0        0     3311 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/build_info/get_loki_api_v1_status_buildinfo.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/format_query/__init__.py
+-rw-r--r--   0        0        0     3826 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/format_query/get_loki_api_v1_format_query.py
+-rw-r--r--   0        0        0     4132 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/format_query/post_loki_api_v1_format_query.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/labels/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/labels/get_loki_api_v1_labels.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/query/__init__.py
+-rw-r--r--   0        0        0     6036 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/query/get_loki_api_v1_query.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/query_range/__init__.py
+-rw-r--r--   0        0        0     9005 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/query_range/get_loki_api_v1_query_range.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/ready/__init__.py
+-rw-r--r--   0        0        0     2086 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/ready/get_ready.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/services/__init__.py
+-rw-r--r--   0        0        0     4386 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/api/services/get_services.py
+-rw-r--r--   0        0        0    12509 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/client.py
+-rw-r--r--   0        0        0      546 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/errors.py
+-rw-r--r--   0        0        0     2228 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/models/__init__.py
+-rw-r--r--   0        0        0     3353 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/models/build_info_response_body.py
+-rw-r--r--   0        0        0      164 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/models/direction.py
+-rw-r--r--   0        0        0     1896 2024-04-26 09:05:58.922217 python_loki_clientv2-0.1.5/grafana_loki_client/models/format_query_response_body.py
+-rw-r--r--   0        0        0     2010 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/labels_response_body.py
+-rw-r--r--   0        0        0     1615 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/post_loki_api_v1_format_query_body.py
+-rw-r--r--   0        0        0     2018 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_range_response_body.py
+-rw-r--r--   0        0        0     2868 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_range_response_data.py
+-rw-r--r--   0        0        0      205 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_range_response_data_result_type.py
+-rw-r--r--   0        0        0     3092 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_range_response_result.py
+-rw-r--r--   0        0        0     1953 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_body.py
+-rw-r--r--   0        0        0     2708 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_data.py
+-rw-r--r--   0        0        0      178 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_data_result_type.py
+-rw-r--r--   0        0        0     1957 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_metric.py
+-rw-r--r--   0        0        0      205 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_metric_level.py
+-rw-r--r--   0        0        0     3054 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_result.py
+-rw-r--r--   0        0        0     1228 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_streams.py
+-rw-r--r--   0        0        0     2568 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics.py
+-rw-r--r--   0        0        0     3147 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_ingester.py
+-rw-r--r--   0        0        0     1741 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_querier.py
+-rw-r--r--   0        0        0     3041 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_store.py
+-rw-r--r--   0        0        0     3086 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_store_chunk.py
+-rw-r--r--   0        0        0     4345 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_summary.py
+-rw-r--r--   0        0        0      265 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/service_state_enum.py
+-rw-r--r--   0        0        0     2296 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/models/services_list_response_body_item.py
+-rw-r--r--   0        0        0      985 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/grafana_loki_client/types.py
+-rw-r--r--   0        0        0     1609 2024-04-26 09:05:58.926217 python_loki_clientv2-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 python_loki_clientv2-0.1.5/PKG-INFO
```

### Comparing `python_loki_clientv2-0.1.4/LICENSE` & `python_loki_clientv2-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/README.md` & `python_loki_clientv2-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/build_info/get_loki_api_v1_status_buildinfo.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/build_info/get_loki_api_v1_status_buildinfo.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/format_query/get_loki_api_v1_format_query.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/format_query/get_loki_api_v1_format_query.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/format_query/post_loki_api_v1_format_query.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/format_query/post_loki_api_v1_format_query.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/labels/get_loki_api_v1_labels.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/labels/get_loki_api_v1_labels.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/query/get_loki_api_v1_query.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/query/get_loki_api_v1_query.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/query_range/get_loki_api_v1_query_range.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/query_range/get_loki_api_v1_query_range.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/ready/get_ready.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/ready/get_ready.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/api/services/get_services.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/api/services/get_services.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/client.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/client.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/errors.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/errors.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/__init__.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_body.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_body.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_data.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_data.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_metric.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_metric.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_result.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_result.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_response_streams.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_response_streams.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_ingester.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_ingester.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_querier.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_querier.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_store.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_store.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_store_chunk.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_store_chunk.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/models/query_statistics_summary.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/models/query_statistics_summary.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/grafana_loki_client/types.py` & `python_loki_clientv2-0.1.5/grafana_loki_client/types.py`

 * *Files identical despite different names*

### Comparing `python_loki_clientv2-0.1.4/pyproject.toml` & `python_loki_clientv2-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.isort]
 profile = "black"
 float_to_top = true
 skip_glob = ".venv"
 
 [tool.poetry]
 name = "python-loki-clientv2"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python client for Grafana Loki"
 repository = "https://github.com/FearZee/python-loki-client"
 authors = ["FearZee <Sascha.zierke+plaesh@outlook.com>","Daniele Esposti <daniele.esposti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "grafana_loki_client" }]
```

### Comparing `python_loki_clientv2-0.1.4/PKG-INFO` & `python_loki_clientv2-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-loki-clientv2
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for Grafana Loki
 Home-page: https://github.com/FearZee/python-loki-client
 License: MIT
 Author: FearZee
 Author-email: Sascha.zierke+plaesh@outlook.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
```

