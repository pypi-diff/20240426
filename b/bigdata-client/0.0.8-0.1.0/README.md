# Comparing `tmp/bigdata_client-0.0.8.tar.gz` & `tmp/bigdata_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdata_client-0.0.8.tar", max compression
+gzip compressed data, was "bigdata_client-0.1.0.tar", max compression
```

## Comparing `bigdata_client-0.0.8.tar` & `bigdata_client-0.1.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0      358 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/README.md
--rw-r--r--   0        0        0      155 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/__init__.py
--rw-r--r--   0        0        0     6526 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/advanced_search_query.py
--rw-r--r--   0        0        0        0 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/api/__init__.py
--rw-r--r--   0        0        0      888 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/api/knowledge_graph.py
--rw-r--r--   0        0        0     8148 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/api/search.py
--rw-r--r--   0        0        0      975 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/api/watchlist.py
--rw-r--r--   0        0        0     6324 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/auth.py
--rw-r--r--   0        0        0        0 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/authenticators/__init__.py
--rw-r--r--   0        0        0     2256 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/authenticators/base_instance.py
--rw-r--r--   0        0        0     4166 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/authenticators/dev_instance.py
--rw-r--r--   0        0        0     3650 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/authenticators/production_instance.py
--rw-r--r--   0        0        0      853 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/exceptions.py
--rw-r--r--   0        0        0      245 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/models.py
--rw-r--r--   0        0        0        0 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/sign_in_strategies/__init__.py
--rw-r--r--   0        0        0      243 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/sign_in_strategies/base.py
--rw-r--r--   0        0        0     1008 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/sign_in_strategies/password.py
--rw-r--r--   0        0        0     2510 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/token_manager.py
--rw-r--r--   0        0        0     2040 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/clerk/token_manager_factory.py
--rw-r--r--   0        0        0     9361 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/connection.py
--rw-r--r--   0        0        0      475 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/connection_protocol.py
--rw-r--r--   0        0        0      154 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/constants.py
--rw-r--r--   0        0        0     3626 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/daterange.py
--rw-r--r--   0        0        0     1234 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/entity_types.py
--rw-r--r--   0        0        0      664 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/enum_utils.py
--rw-r--r--   0        0        0       82 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/errors.py
--rw-r--r--   0        0        0      513 2024-04-22 14:41:18.000398 bigdata_client-0.0.8/bigdata/jwt.py
--rw-r--r--   0        0        0        0 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/__init__.py
--rw-r--r--   0        0        0    21160 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/advanced_search_query.py
--rw-r--r--   0        0        0     1181 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/comentions.py
--rw-r--r--   0        0        0     5961 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/entities.py
--rw-r--r--   0        0        0     1094 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/languages.py
--rw-r--r--   0        0        0     3841 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/parse.py
--rw-r--r--   0        0        0     1710 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/search.py
--rw-r--r--   0        0        0     2280 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/sources.py
--rw-r--r--   0        0        0      855 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/story.py
--rw-r--r--   0        0        0     2180 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/topics.py
--rw-r--r--   0        0        0     1384 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/uploads.py
--rw-r--r--   0        0        0     2820 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/models/watchlists.py
--rw-r--r--   0        0        0     4633 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/old_auth.py
--rw-r--r--   0        0        0      970 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/query.py
--rw-r--r--   0        0        0      251 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/query_type.py
--rw-r--r--   0        0        0     7862 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/search.py
--rw-r--r--   0        0        0    11601 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/services.py
--rw-r--r--   0        0        0     1020 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/settings.py
--rw-r--r--   0        0        0    12157 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/simple_search_query.py
--rw-r--r--   0        0        0     2022 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/story.py
--rw-r--r--   0        0        0      465 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/bigdata/user_agent.py
--rw-r--r--   0        0        0     1359 2024-04-22 14:41:18.004398 bigdata_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/README.md
+-rw-r--r--   0        0        0      155 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/__init__.py
+-rw-r--r--   0        0        0     6526 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/advanced_search_query.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/knowledge_graph.py
+-rw-r--r--   0        0        0     8304 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/search.py
+-rw-r--r--   0        0        0     2985 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/uploads.py
+-rw-r--r--   0        0        0      975 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/api/watchlist.py
+-rw-r--r--   0        0        0     6464 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/auth.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/__init__.py
+-rw-r--r--   0        0        0     2256 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/base_instance.py
+-rw-r--r--   0        0        0     4166 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/dev_instance.py
+-rw-r--r--   0        0        0     3650 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/authenticators/production_instance.py
+-rw-r--r--   0        0        0      853 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/exceptions.py
+-rw-r--r--   0        0        0      245 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/models.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/base.py
+-rw-r--r--   0        0        0     1008 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/password.py
+-rw-r--r--   0        0        0     2510 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/token_manager.py
+-rw-r--r--   0        0        0     2040 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/clerk/token_manager_factory.py
+-rw-r--r--   0        0        0    13702 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/connection.py
+-rw-r--r--   0        0        0      475 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/connection_protocol.py
+-rw-r--r--   0        0        0      154 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/constants.py
+-rw-r--r--   0        0        0     4501 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/daterange.py
+-rw-r--r--   0        0        0     1234 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/entity_types.py
+-rw-r--r--   0        0        0      664 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/enum_utils.py
+-rw-r--r--   0        0        0       82 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/errors.py
+-rw-r--r--   0        0        0      196 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/file_status.py
+-rw-r--r--   0        0        0      513 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/jwt.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/__init__.py
+-rw-r--r--   0        0        0    21160 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/advanced_search_query.py
+-rw-r--r--   0        0        0     1181 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/comentions.py
+-rw-r--r--   0        0        0     5961 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/entities.py
+-rw-r--r--   0        0        0     1094 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/languages.py
+-rw-r--r--   0        0        0     3841 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/parse.py
+-rw-r--r--   0        0        0     1710 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/search.py
+-rw-r--r--   0        0        0     2280 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/sources.py
+-rw-r--r--   0        0        0      855 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/story.py
+-rw-r--r--   0        0        0     2180 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/topics.py
+-rw-r--r--   0        0        0     6580 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/uploads.py
+-rw-r--r--   0        0        0     2820 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/models/watchlists.py
+-rw-r--r--   0        0        0     4773 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/old_auth.py
+-rw-r--r--   0        0        0      177 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/pdf_utils.py
+-rw-r--r--   0        0        0      970 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/query.py
+-rw-r--r--   0        0        0      251 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/query_type.py
+-rw-r--r--   0        0        0     7859 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/search.py
+-rw-r--r--   0        0        0    15123 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/services.py
+-rw-r--r--   0        0        0     1086 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/settings.py
+-rw-r--r--   0        0        0    12157 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/simple_search_query.py
+-rw-r--r--   0        0        0     2022 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/story.py
+-rw-r--r--   0        0        0      465 2024-04-26 08:25:50.391026 bigdata_client-0.1.0/bigdata/user_agent.py
+-rw-r--r--   0        0        0     1359 2024-04-26 08:25:50.395026 bigdata_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.1.0/PKG-INFO
```

### Comparing `bigdata_client-0.0.8/bigdata/advanced_search_query.py` & `bigdata_client-0.1.0/bigdata/advanced_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/api/knowledge_graph.py` & `bigdata_client-0.1.0/bigdata/api/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/api/search.py` & `bigdata_client-0.1.0/bigdata/api/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,23 @@
     id: str
     name: str
     query: SavedSearchQueryResponse
     save_status: Literal["saved"] = Field(default="saved", alias="saveStatus")
     # TODO: Add dateCreated, lastExecuted, lastUpdated, owner, ownerName, permissions
 
 
+# Delete a saved search
+
+
+class DeleteSavedSearchResponse(BaseModel):
+    """Model to represent the response from deleting a saved search"""
+
+    id: str
+
+
 # List saved searches
 
 
 class ListSavedSearchResponse(BaseModel):
     """
     Part of the response from listing saved searches. It represents a single
     saved search, without all the details.
```

### Comparing `bigdata_client-0.0.8/bigdata/api/watchlist.py` & `bigdata_client-0.1.0/bigdata/api/watchlist.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/auth.py` & `bigdata_client-0.1.0/bigdata/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,29 +73,36 @@
         self,
         method,
         url,
         params=None,
         data=None,
         headers=None,
         json=None,
+        stream=None,
     ):
         """Makes an HTTP request, handling the token refresh if needed"""
         headers = headers or {}
         headers["origin"] = f"{settings.BIGDATA_API_URL}"
         headers["referer"] = f"{settings.BIGDATA_API_URL}"
         # if "content-type" not in headers:
         # We may have to conditionally set the content type when uploading files
         headers["content-type"] = "application/json"
         headers["accept"] = "application/json"
         headers["user-agent"] = get_user_agent(settings.PACKAGE_NAME)
         headers["Authorization"] = f"Bearer {self._token_manager.get_session_token()}"
 
         # The request method has other arguments but we are not using them currently
         response = self._session.request(
-            method=method, url=url, params=params, data=data, headers=headers, json=json
+            method=method,
+            url=url,
+            params=params,
+            data=data,
+            headers=headers,
+            json=json,
+            stream=stream,
         )
         if response.status_code == HTTPStatus.UNAUTHORIZED:
             # This headers.copy() is needed for testing. Mock lib does not make a copy, instead it points to
             # the original headers, so asserting that the headers changed fails.
             headers = headers.copy()
             headers["Authorization"] = (
                 f"Bearer {self._token_manager.refresh_session_token()}"
@@ -104,14 +111,15 @@
             response = self._session.request(
                 method=method,
                 url=url,
                 params=params,
                 data=data,
                 headers=headers,
                 json=json,
+                stream=stream,
             )
         return response
 
     def async_requests(
         self, method: str, request_contexts: list[AsyncRequestContext]
     ) -> list[AsyncResponseContext]:
         """Makes an async HTTP request, handling the token refresh if needed"""
```

### Comparing `bigdata_client-0.0.8/bigdata/clerk/authenticators/base_instance.py` & `bigdata_client-0.1.0/bigdata/clerk/authenticators/base_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/clerk/authenticators/dev_instance.py` & `bigdata_client-0.1.0/bigdata/clerk/authenticators/dev_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/clerk/authenticators/production_instance.py` & `bigdata_client-0.1.0/bigdata/clerk/authenticators/production_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/clerk/exceptions.py` & `bigdata_client-0.1.0/bigdata/clerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/clerk/sign_in_strategies/password.py` & `bigdata_client-0.1.0/bigdata/clerk/sign_in_strategies/password.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/clerk/token_manager.py` & `bigdata_client-0.1.0/bigdata/clerk/token_manager.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/clerk/token_manager_factory.py` & `bigdata_client-0.1.0/bigdata/clerk/token_manager_factory.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/connection.py` & `bigdata_client-0.1.0/bigdata/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,59 @@
-from typing import Generator, TypeVar, Union
+from typing import IO, Generator, Iterable, Optional, TypeVar, Union
 from urllib.parse import urljoin
 
+import requests
 from pydantic import BaseModel, ValidationError
 
 from bigdata.api.knowledge_graph import (
     AutosuggestRequests,
     AutosuggestResponse,
     ByIdsRequest,
     ByIdsResponse,
 )
 from bigdata.api.search import (
+    DeleteSavedSearchResponse,
     DiscoveryPanelRequest,
     DiscoveryPanelResponse,
     ListSavedSearchesResponse,
     QueryChunksRequest,
     QueryChunksResponse,
     SavedSearchResponse,
     SaveSearchRequest,
     UpdateSearchRequest,
 )
+from bigdata.api.uploads import (
+    DeleteFileResponse,
+    GetDownloadPresignedUrlResponse,
+    GetFileResponse,
+    GetFileStatusResponse,
+    ListFilesResponse,
+    PostFileRequest,
+    PostFileResponse,
+)
 from bigdata.api.watchlist import (
     CreateWatchlistRequest,
     CreateWatchlistResponse,
     DeleteSingleWatchlistResponse,
     GetSingleWatchlistResponse,
     GetWatchlistsResponse,
     UpdateSingleWatchlistResponse,
     UpdateWatchlistRequest,
 )
 from bigdata.auth import AsyncRequestContext, AsyncResponseContext, Auth
+from bigdata.daterange import AbsoluteDateRange
+from bigdata.file_status import FileStatus
 from bigdata.models.parse import (
     get_discriminator_knowledge_graph_value,
     parse_knowledge_graph_object,
 )
 from bigdata.models.watchlists import Watchlist
 
 CONCURRENT_AUTOSUGGEST_REQUESTS_LIMIT = 10
+CHUNK_SIZE = 32 * 1024
 
 
 class AsyncRequestPartialContext(BaseModel):
     """
     Context used to pass information to connection module for making async requests.
     Async requests are made in parallel, so each request is associated with an id to
     retrieve it from a list of responses.
@@ -145,27 +159,32 @@
         if saved:
             params["save_status"] = "saved"
         if owned:
             params["owned"] = "true"
         json_response = self.http.get("user-data/queries", params=params)
         return ListSavedSearchesResponse(**json_response)
 
-    def save_search(self, request: SaveSearchRequest) -> dict:
+    def save_search(self, request: SaveSearchRequest) -> SavedSearchResponse:
         """Calls POST /user-data/queries"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        return self.http.post("user-data/queries", json=json_request)
+        response = self.http.post("user-data/queries", json=json_request)
+        return SavedSearchResponse(**response)
 
-    def update_search(self, request: UpdateSearchRequest, search_id: str) -> dict:
+    def update_search(
+        self, request: UpdateSearchRequest, search_id: str
+    ) -> SavedSearchResponse:
         """Calls PATCH /user-data/queries/{id}"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        return self.http.patch(f"user-data/queries/{search_id}", json=json_request)
+        response = self.http.patch(f"user-data/queries/{search_id}", json=json_request)
+        return SavedSearchResponse(**response)
 
-    def delete_search(self, id: str) -> dict:
+    def delete_search(self, id: str) -> DeleteSavedSearchResponse:
         """Calls DELETE /user-data/queries/{id}"""
-        return self.http.delete(f"user-data/queries/{id}")
+        response = self.http.delete(f"user-data/queries/{id}")
+        return DeleteSavedSearchResponse(**response)
 
     def query_discovery_panel(
         self, request: DiscoveryPanelRequest
     ) -> DiscoveryPanelResponse:
         """Calls POST /cqs/discovery-panel"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
         json_response = self.http.post("cqs/discovery-panel", json=json_request)
@@ -206,14 +225,107 @@
         """Calls PATCH /user-data/watchlists/{id_}"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
         json_response = self.http.patch(f"user-data/watchlists/{id_}", json_request)
 
         return UpdateSingleWatchlistResponse.model_validate(json_response)
 
 
+class UploadsConnection:
+    """
+    The connection to the Uploads API.
+
+    Contains the Auth object with the JWT and abstracts all the calls to the API,
+    receiving and returning objects to/from the caller.
+    For internal use only.
+    """
+
+    def __init__(self, auth: Auth, api_url: str):
+        self.http = HTTPWrapper(auth, api_url)
+
+    def list_files(
+        self,
+        date_range: Optional[AbsoluteDateRange] = None,
+        tags: Optional[list[str]] = None,
+        status: Optional[FileStatus] = None,
+        file_name: Optional[str] = None,
+        folder_id: Optional[str] = None,
+        page_size: Optional[int] = None,
+    ) -> ListFilesResponse:
+        start, end = None, None
+        if date_range is not None:
+            start, end = date_range.to_string_tuple()
+        params = {
+            "start_date": start,
+            "end_date": end,
+            "tags": tags,
+            "status": status,
+            "file_name": file_name,
+            "folder_id": folder_id,
+            "page_size": page_size,
+        }
+        params = {k: v for k, v in params.items() if v is not None}
+        json_response = self.http.get("files", params=params)
+        return ListFilesResponse(**json_response)
+
+    def get_file(self, id: str) -> GetFileResponse:
+        json_response = self.http.get(f"files/{id}/metadata")
+        return GetFileResponse(**json_response)
+
+    def post_file(self, request: PostFileRequest) -> PostFileResponse:
+        json_request = request.model_dump(exclude_none=True, by_alias=True)
+        json_response = self.http.post("files", json=json_request)
+        return PostFileResponse(**json_response)
+
+    def get_file_status(self, id: str) -> GetFileStatusResponse:
+        json_response = self.http.get(f"files/{id}/status")
+        return GetFileStatusResponse(**json_response)
+
+    def delete_file(self, id: str) -> DeleteFileResponse:
+        response = self.http.delete(f"files/{id}")
+        return DeleteFileResponse(**response)
+
+    def get_download_presigned_url(self, id: str) -> GetDownloadPresignedUrlResponse:
+        json_response = self.http.get(f"files/{id}")
+        return GetDownloadPresignedUrlResponse(**json_response)
+
+    def download_analytics(self, id: str) -> Iterable[bytes]:
+        return self.http.get_chunks(f"files/{id}/analytics", chunk_size=CHUNK_SIZE)
+
+    def download_annotated(self, id: str) -> Iterable[bytes]:
+        return self.http.get_chunks(f"files/{id}/annotated", chunk_size=CHUNK_SIZE)
+
+    def download_text(self, id: str) -> Iterable[bytes]:
+        return self.http.get_chunks(
+            f"files/{id}/text-extraction", chunk_size=CHUNK_SIZE
+        )
+
+
+def upload_file(url: str, file_descriptor: IO):
+    """Used to upload files to third-parties like S3"""
+    response = requests.put(
+        url,
+        data=file_descriptor,
+        headers={
+            "x-amz-server-side-encryption": "AES256",
+            "Content-Type": "application/octet-stream",
+        },
+    )
+    response.raise_for_status()
+
+
+def get_chunks_from_presigned_url(
+    url: str, chunk_size: int = CHUNK_SIZE
+) -> Iterable[bytes]:
+    """Used to download files from third-parties like S3"""
+    response = requests.get(url, stream=True)
+    response.raise_for_status()
+    for chunk in response.iter_content(chunk_size=chunk_size):
+        yield chunk
+
+
 class HTTPWrapper:
     """
     A basic connection to perform HTTP GET, POST, PATCH, DELETE requests.
     """
 
     # Wrappers for HTTP methods
 
@@ -242,14 +354,22 @@
 
     def delete(self, endpoint: str) -> json_types:
         url = self._get_url(endpoint)
         response = self.auth.request("DELETE", url)
         response.raise_for_status()
         return response.json()
 
+    def get_chunks(self, endpoint: str, chunk_size: int) -> Iterable[bytes]:
+        """Does an HTTP GET but returns the response in chunks of bytes."""
+        url = self._get_url(endpoint)
+        response = self.auth.request("GET", url, stream=True)
+        response.raise_for_status()
+        for chunk in response.iter_content(chunk_size=chunk_size):
+            yield chunk
+
     # Async wrappers for HTTP methods
     def async_get(
         self, async_partial_contexts: list[AsyncRequestPartialContext]
     ) -> list[AsyncResponseContext]:
         all_requests_context = [
             AsyncRequestContext(
                 id=partial_context.id,
```

### Comparing `bigdata_client-0.0.8/bigdata/daterange.py` & `bigdata_client-0.1.0/bigdata/daterange.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from enum import Enum
-from typing import Union
+from typing import Optional, Union
 
 from bigdata.models.advanced_search_query import (
     AbsoluteDateRangeQuery,
     RollingDateRangeQuery,
 )
 from bigdata.models.search import Expression
 
@@ -71,38 +71,63 @@
     >>> start, end = ran1.to_string_tuple()
     >>> start
     '2021-01-01T00:00:00'
     >>> end
     '2021-01-02T00:00:00'
     """
 
-    def __init__(self, start: Union[datetime, str], end: Union[datetime, str]):
+    def __init__(
+        self, start: Union[datetime, str, None], end: Union[datetime, str, None]
+    ):
         """Creates a new AbsoluteDateRange from two datetimes or strings."""
         if isinstance(start, str):
             start = datetime.fromisoformat(start)
         if isinstance(end, str):
             end = datetime.fromisoformat(end)
         self.start_dt = start
         self.end_dt = end
 
-    def to_string_tuple(self):
-        """Converts datetimes to strings and returns the tuple"""
-        return self.start_dt.isoformat(), self.end_dt.isoformat()
+    def to_string_tuple(self) -> tuple[Optional[str], Optional[str]]:
+        """
+        Converts datetimes to strings and returns the tuple
+
+        >>> ran = AbsoluteDateRange(datetime(2021, 1, 1), datetime(2021, 1, 2))
+        >>> ran.to_string_tuple()
+        ('2021-01-01T00:00:00', '2021-01-02T00:00:00')
+
+        >>> ran2 = AbsoluteDateRange(None, datetime(2021, 1, 2))
+        >>> ran2.to_string_tuple()
+        (None, '2021-01-02T00:00:00')
+
+        >>> ran3 = AbsoluteDateRange(datetime(2021, 1, 1), None)
+        >>> ran3.to_string_tuple()
+        ('2021-01-01T00:00:00', None)
+
+        >>> ran4 = AbsoluteDateRange(*ran.to_string_tuple())
+        >>> ran == ran4
+        True
+        """
+        start = self.start_dt.isoformat() if self.start_dt else None
+        end = self.end_dt.isoformat() if self.end_dt else None
+        return start, end
 
     def __eq__(self, other):
         if not isinstance(other, AbsoluteDateRange):
             return False
         return self.start_dt == other.start_dt and self.end_dt == other.end_dt
 
     def __repr__(self):
         return f"AbsoluteDateRange{self.to_string_tuple()}"
 
     @property
     def _proxy_query(self):
-        return AbsoluteDateRangeQuery(*self.to_string_tuple())
+        start, end = self.to_string_tuple()
+        if start is None or end is None:
+            raise ValueError("Cannot create a query with None values")
+        return AbsoluteDateRangeQuery(start, end)
 
     def to_expression(self):
         return self._proxy_query.to_expression()
 
     def to_dict(self):
         return self._proxy_query.to_dict()
```

### Comparing `bigdata_client-0.0.8/bigdata/entity_types.py` & `bigdata_client-0.1.0/bigdata/entity_types.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/enum_utils.py` & `bigdata_client-0.1.0/bigdata/enum_utils.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/jwt.py` & `bigdata_client-0.1.0/bigdata/jwt.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/advanced_search_query.py` & `bigdata_client-0.1.0/bigdata/models/advanced_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/comentions.py` & `bigdata_client-0.1.0/bigdata/models/comentions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/entities.py` & `bigdata_client-0.1.0/bigdata/models/entities.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/languages.py` & `bigdata_client-0.1.0/bigdata/models/languages.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/parse.py` & `bigdata_client-0.1.0/bigdata/models/parse.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/search.py` & `bigdata_client-0.1.0/bigdata/models/search.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/sources.py` & `bigdata_client-0.1.0/bigdata/models/sources.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/story.py` & `bigdata_client-0.1.0/bigdata/models/story.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/topics.py` & `bigdata_client-0.1.0/bigdata/models/topics.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/models/watchlists.py` & `bigdata_client-0.1.0/bigdata/models/watchlists.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/old_auth.py` & `bigdata_client-0.1.0/bigdata/old_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,39 +79,47 @@
         self,
         method,
         url,
         params=None,
         data=None,
         headers=None,
         json=None,
+        stream=None,
     ):
         """Makes an HTTP request, handling the token refresh if needed"""
         headers = headers or {}
         headers["origin"] = "https://bigdata.com"
         headers["referer"] = "https://bigdata.com/"
         # if "content-type" not in headers:
         # We may have to conditionally set the content type when uploading files
         headers["content-type"] = "application/json"
         headers["accept"] = "application/json"
         headers["x-csrf-token"] = self.x_csrf_token
         headers["user-agent"] = get_user_agent(settings.PACKAGE_NAME)
         # The requet method has other arguments but we are not using them currently
         response = self._session.request(
-            method=method, url=url, params=params, data=data, headers=headers, json=json
+            method=method,
+            url=url,
+            params=params,
+            data=data,
+            headers=headers,
+            json=json,
+            stream=stream,
         )
         if response.status_code == 401:
             self.refresh_jwt()
             # Retry the request
             response = self._session.request(
                 method=method,
                 url=url,
                 params=params,
                 data=data,
                 headers=headers,
                 json=json,
+                stream=stream,
             )
         return response
 
     def _handle_auth_response(self, response):
         response.raise_for_status()
         self.jwt_refresh_token = response.json()["refresh"]
         self.is_datetime_in_sync = self._is_jwt_recent(self.jwt_refresh_token)
```

### Comparing `bigdata_client-0.0.8/bigdata/query.py` & `bigdata_client-0.1.0/bigdata/query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/search.py` & `bigdata_client-0.1.0/bigdata/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             raise ValueError("The search object must have an API to save.")
         if self.id is None:
             # Create a new search
             request = SaveSearchRequest(
                 name=name, query=self.query.to_save_search_request()
             )
             response = self.api.save_search(request)
-            self.id = response["id"]
+            self.id = response.id
         else:
             # Update an existing search
             request = UpdateSearchRequest(
                 name=name, query=self.query.to_save_search_request()
             )
             self.api.update_search(request, self.id)
```

### Comparing `bigdata_client-0.0.8/bigdata/services.py` & `bigdata_client-0.1.0/bigdata/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import os
+import time
+from datetime import datetime
 from typing import List, Optional, Union
 
+import requests
+
 from bigdata import old_auth
 from bigdata.api.knowledge_graph import (
     AutosuggestRequests,
     AutosuggestResponse,
     ByIdsRequest,
 )
+from bigdata.api.uploads import ExtractorTypes, PostFileRequest
 from bigdata.api.watchlist import CreateWatchlistRequest, UpdateWatchlistRequest
 from bigdata.auth import Auth
-from bigdata.connection import BigdataConnection
+from bigdata.connection import BigdataConnection, UploadsConnection, upload_file
 from bigdata.connection_protocol import BigdataConnectionProtocol
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
+from bigdata.file_status import FileStatus
 from bigdata.models.advanced_search_query import QueryComponent
 from bigdata.models.entities import MacroEntity
 from bigdata.models.languages import Language
 from bigdata.models.parse import (
     AutosuggestedSavedSearch,
     EntityTypes,
     KnowledgeGraphTypes,
 )
 from bigdata.models.search import FileType, SortBy
 from bigdata.models.sources import Source
 from bigdata.models.topics import Topic
-from bigdata.models.uploads import Document, UploadQuota
+from bigdata.models.uploads import File, UploadQuota
 from bigdata.models.watchlists import Watchlist
+from bigdata.pdf_utils import is_pdf_file
 from bigdata.query_type import QueryType
 from bigdata.search import Search
 from bigdata.settings import BigdataAuthType, settings
 
 CONCURRENT_AUTOSUGGEST_REQUESTS_LIMIT = 10
 
 
@@ -43,36 +50,41 @@
     """
 
     def __init__(
         self,
         username: Optional[str] = None,
         password: Optional[str] = None,
         auth_type: Optional[BigdataAuthType] = None,
-        api_url: Optional[str] = None,
+        bigdata_api_url: Optional[str] = None,
+        upload_api_url: Optional[str] = None,
     ):
         if password is None:
             password = os.environ.get("BIGDATA_PASSWORD")
         if username is None:
             username = os.environ.get("BIGDATA_USER")
         if username is None or password is None:
             raise ValueError("Username and password must be provided")
         if auth_type is None:
             auth_type = settings.BIGDATA_AUTH_TYPE
         if auth_type == BigdataAuthType.CLERK:
             auth = Auth.from_username_and_password(username, password)
         else:
             auth = old_auth.Auth.from_username_and_password(username, password)
 
-        if api_url is None:
-            api_url = str(settings.BIGDATA_API_URL)
-        self.api = BigdataConnection(auth, api_url)
+        if bigdata_api_url is None:
+            bigdata_api_url = str(settings.BIGDATA_API_URL)
+        if upload_api_url is None:
+            upload_api_url = str(settings.UPLOAD_API_URL)
+
+        self.api = BigdataConnection(auth, bigdata_api_url)
+        self.upload_api = UploadsConnection(auth, upload_api_url)
         self.knowledge_graph = KnowledgeGraph(self.api)
         self.content_search = ContentSearch(self.api)
         self.watchlists = Watchlists(self.api)
-        self.uploads = Uploads(self.api)
+        self.uploads = Uploads(self.upload_api)
 
 
 class KnowledgeGraph:
     """For finding entities, sources and topics"""
 
     def __init__(self, api_connection: BigdataConnectionProtocol):
         self.api = api_connection
@@ -299,26 +311,115 @@
         """Delete a saved search by its id."""
         self.api.delete_search(id_)
 
 
 class Uploads:
     """For managing internal uploads. Searching will be done through content"""
 
-    def __init__(self, api_connection: BigdataConnection):
+    def __init__(self, api_connection: UploadsConnection):
         self.api = api_connection
 
-    def get(self, id_, /) -> Document:
-        """Retrieve a document by its id."""
+    def get(self, id_, /) -> File:
+        """Retrieve a file by its id."""
+        response = None
+        while response is None:
+            try:
+                response = self.api.get_file(id_)
+            except requests.exceptions.HTTPError as e:
+                # While unavailable, keep trying
+                if e.response.status_code == 425:
+                    time.sleep(1)
+                    continue
+                raise e
+        return File(
+            _api=self.api,
+            id=response.id,
+            name=response.name,
+            status=response.status,
+            uploaded_at=response.uploaded_at,
+            raw_size=response.raw_size,
+            folder_id=response.folder_id,
+            trashed=response.trashed,
+            starred=response.starred,
+            tags=response.tags,
+        )
 
-    def list(self) -> list[Document]:
+    def list(
+        self,
+        start_date: Optional[Union[datetime, str]] = None,
+        end_date: Optional[Union[datetime, str]] = None,
+        tags: Optional[list[str]] = None,
+        status: Optional[FileStatus] = None,
+        file_name: Optional[str] = None,
+        folder_id: Optional[str] = None,
+        page_size: Optional[int] = None,
+    ) -> list[File]:
         """Retrieve all documents for the current user."""
+        date_range = (
+            AbsoluteDateRange(start_date, end_date) if start_date or end_date else None
+        )
+        response = self.api.list_files(
+            date_range=date_range,
+            tags=tags,
+            status=status,
+            file_name=file_name,
+            folder_id=folder_id,
+            page_size=page_size,
+        )
+        docs = []
+        for upload in response.results:
+            doc = File(
+                _api=self.api,
+                id=upload.id,
+                name=upload.name,
+                status=upload.status,
+                uploaded_at=upload.uploaded_at,
+                raw_size=upload.raw_size,
+                folder_id=upload.folder_id,
+                trashed=upload.trashed,
+                starred=upload.starred,
+                tags=upload.tags,
+            )
+            docs.append(doc)
 
-    def upload_document(self, document: Document, /):
-        """Uploads a document to the bigdata platform."""
+        return docs
 
-    def delete(self, id_, /):
-        """Delete a document by its id."""
+    def upload_from_disk(
+        self,
+        path: str,
+        /,
+        provider_document_id: Optional[str] = None,
+        provider_date_utc: Optional[Union[str, datetime]] = None,
+    ) -> File:
+        """Uploads a file to the bigdata platform."""
+        filename = os.path.basename(path)
+
+        properties = {}
+        if provider_document_id is not None:
+            properties["provider_document_id"] = provider_document_id
+        if provider_date_utc is not None:
+            if isinstance(provider_date_utc, datetime):
+                provider_date_utc = provider_date_utc.strftime("%Y-%m-%d %H:%M:%S")
+            properties["provider_date_utc"] = provider_date_utc
+        if is_pdf_file(path):
+            properties["extractor"] = ExtractorTypes.PDF_EXTRACTOR_1_0
+        properties = properties or None
+
+        # Pre-upload
+        post_file_request = PostFileRequest(
+            filename=filename,
+            folder_id=None,
+            source_url=None,
+            upload_mode=None,
+            properties=properties,
+        )
+        post_file_request = self.api.post_file(post_file_request)
 
-    def get_quota(self) -> UploadQuota:
-        """Retrieve the remaining upload quota for the current user."""
+        with open(path, "rb") as file:
+            upload_file(post_file_request.location, file)
+        return self.get(post_file_request.file_id)
+
+    def delete(self, id_, /):
+        """Delete a file by its id."""
+        self.api.delete_file(id_)
 
     # TODO: add methods to manage folders etc
```

### Comparing `bigdata_client-0.0.8/bigdata/settings.py` & `bigdata_client-0.1.0/bigdata/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 class Settings(
     BaseSettings
 ):  # FIXME OLD AUTH remove Clerk config when old auth is removed
     PACKAGE_NAME: str = "bigdata-client"  # The name of the python package
     BIGDATA_API_URL: HttpUrl = "https://api.bigdata.com"
+    UPLOAD_API_URL: HttpUrl = "https://upload.ravenpack.com/1.0/"
     BIGDATA_AUTH_TYPE: BigdataAuthType = BigdataAuthType.CLERK
     CLERK_INSTANCE_TYPE: ClerkInstanceType = ClerkInstanceType.PROD
     # TODO: Change to another endpoint as we need the refresh token
     AUTH_LOGIN_FORM_ENDPOINT: HttpUrl = "https://auth.ravenpack.com/2.0/login"
     CLERK_FRONTEND_URL: HttpUrl = "https://clerk.bigdata.com/v1"
     LLM: LLMSettings = LLMSettings()
```

### Comparing `bigdata_client-0.0.8/bigdata/simple_search_query.py` & `bigdata_client-0.1.0/bigdata/simple_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/bigdata/story.py` & `bigdata_client-0.1.0/bigdata/story.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.8/pyproject.toml` & `bigdata_client-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bigdata-client"
 packages = [
     { include = "bigdata" },
 ]
-version = "0.0.8"
+version = "0.1.0"
 description = ""
 authors = [
     "Bigdata Team <support@bigdata.com>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `bigdata_client-0.0.8/PKG-INFO` & `bigdata_client-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdata-client
-Version: 0.0.8
+Version: 0.1.0
 Summary: 
 Author: Bigdata Team
 Author-email: support@bigdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

