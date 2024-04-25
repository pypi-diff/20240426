# Comparing `tmp/athena_intelligence-0.1.52.tar.gz` & `tmp/athena_intelligence-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.52.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.53.tar", max compression
```

## Comparing `athena_intelligence-0.1.52.tar` & `athena_intelligence-0.1.53.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4235 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/README.md
--rw-r--r--   0        0        0      603 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/pyproject.toml
--rw-r--r--   0        0        0     1595 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/__init__.py
--rw-r--r--   0        0        0     6860 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/base_client.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/chain/__init__.py
--rw-r--r--   0        0        0    16236 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/chain/client.py
--rw-r--r--   0        0        0     3576 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/client.py
--rw-r--r--   0        0        0      853 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1495 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12498 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6338 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6623 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/tasks/__init__.py
--rw-r--r--   0        0        0     8234 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/tasks/client.py
--rw-r--r--   0        0        0       65 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    20114 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/tools/client.py
--rw-r--r--   0        0        0     1799 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/__init__.py
--rw-r--r--   0        0        0      994 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1061 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/document.py
--rw-r--r--   0        0        0      875 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1001 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1143 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      969 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      969 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      953 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      892 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0     4101 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/llm_model.py
--rw-r--r--   0        0        0      950 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/map_reduce_chain_out.py
--rw-r--r--   0        0        0      845 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1031 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2991 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/model.py
--rw-r--r--   0        0        0     1034 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/plan_execute_out.py
--rw-r--r--   0        0        0      926 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/report.py
--rw-r--r--   0        0        0     1106 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/snippet.py
--rw-r--r--   0        0        0      880 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      885 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1829 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/tool_models.py
--rw-r--r--   0        0        0     1422 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/tools.py
--rw-r--r--   0        0        0      873 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/url_result.py
--rw-r--r--   0        0        0      972 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       87 2024-04-25 00:12:44.935835 athena_intelligence-0.1.52/src/athena/version.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.52/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-25 02:06:41.864585 athena_intelligence-0.1.53/README.md
+-rw-r--r--   0        0        0      603 2024-04-25 02:06:41.864585 athena_intelligence-0.1.53/pyproject.toml
+-rw-r--r--   0        0        0     1595 2024-04-25 02:06:41.864585 athena_intelligence-0.1.53/src/athena/__init__.py
+-rw-r--r--   0        0        0     6860 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0    16177 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/chain/client.py
+-rw-r--r--   0        0        0     3576 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/client.py
+-rw-r--r--   0        0        0      853 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1495 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12498 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6338 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6623 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/tasks/__init__.py
+-rw-r--r--   0        0        0     8234 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/tasks/client.py
+-rw-r--r--   0        0        0       65 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    20114 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1799 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1061 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/document.py
+-rw-r--r--   0        0        0      875 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1001 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1143 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      969 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      969 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      953 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      892 2024-04-25 02:06:41.868585 athena_intelligence-0.1.53/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0     4101 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/llm_model.py
+-rw-r--r--   0        0        0      950 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/map_reduce_chain_out.py
+-rw-r--r--   0        0        0      845 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1031 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2991 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/model.py
+-rw-r--r--   0        0        0     1034 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/plan_execute_out.py
+-rw-r--r--   0        0        0      926 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/report.py
+-rw-r--r--   0        0        0     1106 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      880 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      885 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1829 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/tool_models.py
+-rw-r--r--   0        0        0     1422 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/tools.py
+-rw-r--r--   0        0        0      873 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      972 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       87 2024-04-25 02:06:41.872585 athena_intelligence-0.1.53/src/athena/version.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.53/PKG-INFO
```

### Comparing `athena_intelligence-0.1.52/README.md` & `athena_intelligence-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/pyproject.toml` & `athena_intelligence-0.1.53/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-intelligence"
-version = "0.1.52"
+version = "0.1.53"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "athena", from = "src"}
 ]
```

### Comparing `athena_intelligence-0.1.52/src/athena/__init__.py` & `athena_intelligence-0.1.53/src/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/base_client.py` & `athena_intelligence-0.1.53/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/chain/client.py` & `athena_intelligence-0.1.53/src/athena/chain/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.document import Document
 from ..types.http_validation_error import HttpValidationError
 from ..types.llm_model import LlmModel
 from ..types.map_reduce_chain_out import MapReduceChainOut
 from ..types.structured_parse_result import StructuredParseResult
-from ..types.tool_models import ToolModels
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ChainClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
@@ -94,47 +93,47 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def map_reduce_chain(
         self,
         *,
         documents: typing.Sequence[Document],
-        model: ToolModels,
+        model: LlmModel,
         operator_prompt: str,
         reducer_prompt: str,
         input: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MapReduceChainOut:
         """
         Parameters:
             - documents: typing.Sequence[Document].
 
-            - model: ToolModels.
+            - model: LlmModel.
 
             - operator_prompt: str.
 
             - reducer_prompt: str.
 
             - input: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import Document, ToolModels
+        from athena import Document, LlmModel
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.chain.map_reduce_chain(
             documents=[
                 Document(
                     page_content="Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, allowing you to hand over controls to her for autonomous execution with confidence.",
                 )
             ],
-            model=ToolModels.MISTRAL_LARGE_0224,
+            model=LlmModel.MISTRAL_LARGE_0224,
             operator_prompt="summarize the content",
             reducer_prompt="Combine these summaries",
             input="return a summary in a single sentence",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
@@ -263,47 +262,47 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def map_reduce_chain(
         self,
         *,
         documents: typing.Sequence[Document],
-        model: ToolModels,
+        model: LlmModel,
         operator_prompt: str,
         reducer_prompt: str,
         input: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> MapReduceChainOut:
         """
         Parameters:
             - documents: typing.Sequence[Document].
 
-            - model: ToolModels.
+            - model: LlmModel.
 
             - operator_prompt: str.
 
             - reducer_prompt: str.
 
             - input: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import Document, ToolModels
+        from athena import Document, LlmModel
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.chain.map_reduce_chain(
             documents=[
                 Document(
                     page_content="Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, allowing you to hand over controls to her for autonomous execution with confidence.",
                 )
             ],
-            model=ToolModels.MISTRAL_LARGE_0224,
+            model=LlmModel.MISTRAL_LARGE_0224,
             operator_prompt="summarize the content",
             reducer_prompt="Combine these summaries",
             input="return a summary in a single sentence",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
```

### Comparing `athena_intelligence-0.1.52/src/athena/client.py` & `athena_intelligence-0.1.53/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/core/__init__.py` & `athena_intelligence-0.1.53/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.53/src/athena/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.52",
+            "X-Fern-SDK-Version": "0.1.53",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.52/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.53/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/core/file.py` & `athena_intelligence-0.1.53/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/core/http_client.py` & `athena_intelligence-0.1.53/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.53/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/core/request_options.py` & `athena_intelligence-0.1.53/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/dataset/client.py` & `athena_intelligence-0.1.53/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/message/client.py` & `athena_intelligence-0.1.53/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/polling_message_client.py` & `athena_intelligence-0.1.53/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/query/client.py` & `athena_intelligence-0.1.53/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/report/client.py` & `athena_intelligence-0.1.53/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/search/client.py` & `athena_intelligence-0.1.53/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/snippet/client.py` & `athena_intelligence-0.1.53/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/tasks/client.py` & `athena_intelligence-0.1.53/src/athena/tasks/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/tools/client.py` & `athena_intelligence-0.1.53/src/athena/tools/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/__init__.py` & `athena_intelligence-0.1.53/src/athena/types/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/dataset.py` & `athena_intelligence-0.1.53/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/document.py` & `athena_intelligence-0.1.53/src/athena/types/document.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.53/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.53/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.53/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.53/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.53/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.53/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.53/src/athena/types/langchain_documents_request_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/llm_model.py` & `athena_intelligence-0.1.53/src/athena/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/map_reduce_chain_out.py` & `athena_intelligence-0.1.53/src/athena/types/map_reduce_chain_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/message_out.py` & `athena_intelligence-0.1.53/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.53/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/model.py` & `athena_intelligence-0.1.53/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/plan_execute_out.py` & `athena_intelligence-0.1.53/src/athena/types/plan_execute_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/report.py` & `athena_intelligence-0.1.53/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/snippet.py` & `athena_intelligence-0.1.53/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/sql_results.py` & `athena_intelligence-0.1.53/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/status_enum.py` & `athena_intelligence-0.1.53/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.53/src/athena/types/structured_parse_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/tool_models.py` & `athena_intelligence-0.1.53/src/athena/types/tool_models.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/tools.py` & `athena_intelligence-0.1.53/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/url_result.py` & `athena_intelligence-0.1.53/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/src/athena/types/validation_error.py` & `athena_intelligence-0.1.53/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.52/PKG-INFO` & `athena_intelligence-0.1.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.52
+Version: 0.1.53
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

