# Comparing `tmp/langchain_mistralai-0.1.2rc1.tar.gz` & `tmp/langchain_mistralai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.2rc1.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.4.tar", max compression
```

## Comparing `langchain_mistralai-0.1.2rc1.tar` & `langchain_mistralai-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/LICENSE
--rw-r--r--   0        0        0     1336 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/README.md
--rw-r--r--   0        0        0      173 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    26092 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     5961 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2437 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0     2247 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1336 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/README.md
+-rw-r--r--   0        0        0      173 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    29480 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     7158 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2391 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.4/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.2rc1/LICENSE` & `langchain_mistralai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.2rc1/README.md` & `langchain_mistralai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.2rc1/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.4/langchain_mistralai/chat_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import json
 import logging
+import uuid
 from operator import itemgetter
 from typing import (
     Any,
     AsyncContextManager,
     AsyncIterator,
     Callable,
     Dict,
@@ -16,15 +18,14 @@
     Type,
     Union,
     cast,
 )
 
 import httpx
 from httpx_sse import EventSource, aconnect_sse, connect_sse
-from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
@@ -37,16 +38,18 @@
     AIMessageChunk,
     BaseMessage,
     BaseMessageChunk,
     ChatMessage,
     ChatMessageChunk,
     HumanMessage,
     HumanMessageChunk,
+    InvalidToolCall,
     SystemMessage,
     SystemMessageChunk,
+    ToolCall,
     ToolMessage,
 )
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
     PydanticToolsParser,
     make_invalid_tool_call,
@@ -87,39 +90,68 @@
     tool_calls = []
     invalid_tool_calls = []
     if raw_tool_calls := _message.get("tool_calls"):
         additional_kwargs["tool_calls"] = raw_tool_calls
         for raw_tool_call in raw_tool_calls:
             try:
                 parsed: dict = cast(
-                    dict, parse_tool_call(raw_tool_call, return_id=False)
-                )
-                tool_calls.append(
-                    {
-                        **parsed,
-                        **{"id": None},
-                    },
+                    dict, parse_tool_call(raw_tool_call, return_id=True)
                 )
+                if not parsed["id"]:
+                    tool_call_id = uuid.uuid4().hex[:]
+                    tool_calls.append(
+                        {
+                            **parsed,
+                            **{"id": tool_call_id},
+                        },
+                    )
+                else:
+                    tool_calls.append(parsed)
             except Exception as e:
                 invalid_tool_calls.append(
                     dict(make_invalid_tool_call(raw_tool_call, str(e)))
                 )
     return AIMessage(
         content=content,
         additional_kwargs=additional_kwargs,
         tool_calls=tool_calls,
         invalid_tool_calls=invalid_tool_calls,
     )
 
 
+def _raise_on_error(response: httpx.Response) -> None:
+    """Raise an error if the response is an error."""
+    if httpx.codes.is_error(response.status_code):
+        error_message = response.read().decode("utf-8")
+        raise httpx.HTTPStatusError(
+            f"Error response {response.status_code} "
+            f"while fetching {response.url}: {error_message}",
+            request=response.request,
+            response=response,
+        )
+
+
+async def _araise_on_error(response: httpx.Response) -> None:
+    """Raise an error if the response is an error."""
+    if httpx.codes.is_error(response.status_code):
+        error_message = (await response.aread()).decode("utf-8")
+        raise httpx.HTTPStatusError(
+            f"Error response {response.status_code} "
+            f"while fetching {response.url}: {error_message}",
+            request=response.request,
+            response=response,
+        )
+
+
 async def _aiter_sse(
     event_source_mgr: AsyncContextManager[EventSource],
 ) -> AsyncIterator[Dict]:
     """Iterate over the server-sent events."""
     async with event_source_mgr as event_source:
+        await _araise_on_error(event_source.response)
         async for event in event_source.aiter_sse():
             if event.data == "[DONE]":
                 return
             yield event.json()
 
 
 async def acompletion_with_retry(
@@ -135,18 +167,18 @@
         if "stream" not in kwargs:
             kwargs["stream"] = False
         stream = kwargs["stream"]
         if stream:
             event_source = aconnect_sse(
                 llm.async_client, "POST", "/chat/completions", json=kwargs
             )
-
             return _aiter_sse(event_source)
         else:
             response = await llm.async_client.post(url="/chat/completions", json=kwargs)
+            await _araise_on_error(response)
             return response.json()
 
     return await _completion_with_retry(**kwargs)
 
 
 def _convert_delta_to_message_chunk(
     _delta: Dict, default_class: Type[BaseMessageChunk]
@@ -156,23 +188,28 @@
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         additional_kwargs: Dict = {}
         if raw_tool_calls := _delta.get("tool_calls"):
             additional_kwargs["tool_calls"] = raw_tool_calls
             try:
-                tool_call_chunks = [
-                    {
-                        "name": rtc["function"].get("name"),
-                        "args": rtc["function"].get("arguments"),
-                        "id": rtc.get("id"),
-                        "index": rtc.get("index"),
-                    }
-                    for rtc in raw_tool_calls
-                ]
+                tool_call_chunks = []
+                for raw_tool_call in raw_tool_calls:
+                    if not raw_tool_call.get("index") and not raw_tool_call.get("id"):
+                        tool_call_id = uuid.uuid4().hex[:]
+                    else:
+                        tool_call_id = raw_tool_call.get("id")
+                    tool_call_chunks.append(
+                        {
+                            "name": raw_tool_call["function"].get("name"),
+                            "args": raw_tool_call["function"].get("arguments"),
+                            "id": tool_call_id,
+                            "index": raw_tool_call.get("index"),
+                        }
+                    )
             except KeyError:
                 pass
         else:
             tool_call_chunks = []
         return AIMessageChunk(
             content=content,
             additional_kwargs=additional_kwargs,
@@ -182,37 +219,81 @@
         return SystemMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role)
     else:
         return default_class(content=content)
 
 
+def _format_tool_call_for_mistral(tool_call: ToolCall) -> dict:
+    """Format Langchain ToolCall to dict expected by Mistral."""
+    result: Dict[str, Any] = {
+        "function": {
+            "name": tool_call["name"],
+            "arguments": json.dumps(tool_call["args"]),
+        }
+    }
+    if _id := tool_call.get("id"):
+        result["id"] = _id
+
+    return result
+
+
+def _format_invalid_tool_call_for_mistral(invalid_tool_call: InvalidToolCall) -> dict:
+    """Format Langchain InvalidToolCall to dict expected by Mistral."""
+    result: Dict[str, Any] = {
+        "function": {
+            "name": invalid_tool_call["name"],
+            "arguments": invalid_tool_call["args"],
+        }
+    }
+    if _id := invalid_tool_call.get("id"):
+        result["id"] = _id
+
+    return result
+
+
 def _convert_message_to_mistral_chat_message(
     message: BaseMessage,
 ) -> Dict:
     if isinstance(message, ChatMessage):
         return dict(role=message.role, content=message.content)
     elif isinstance(message, HumanMessage):
         return dict(role="user", content=message.content)
     elif isinstance(message, AIMessage):
-        if "tool_calls" in message.additional_kwargs:
-            tool_calls = [
-                {
+        tool_calls = []
+        if message.tool_calls or message.invalid_tool_calls:
+            for tool_call in message.tool_calls:
+                tool_calls.append(_format_tool_call_for_mistral(tool_call))
+            for invalid_tool_call in message.invalid_tool_calls:
+                tool_calls.append(
+                    _format_invalid_tool_call_for_mistral(invalid_tool_call)
+                )
+        elif "tool_calls" in message.additional_kwargs:
+            for tc in message.additional_kwargs["tool_calls"]:
+                chunk = {
                     "function": {
                         "name": tc["function"]["name"],
                         "arguments": tc["function"]["arguments"],
                     }
                 }
-                for tc in message.additional_kwargs["tool_calls"]
-            ]
+                if _id := tc.get("id"):
+                    chunk["id"] = _id
+                tool_calls.append(chunk)
+        else:
+            pass
+        if tool_calls and message.content:
+            # Assistant message must have either content or tool_calls, but not both.
+            # Some providers may not support tool_calls in the same message as content.
+            # This is done to ensure compatibility with messages from other providers.
+            content: Any = ""
         else:
-            tool_calls = []
+            content = message.content
         return {
             "role": "assistant",
-            "content": message.content,
+            "content": content,
             "tool_calls": tool_calls,
         }
     elif isinstance(message, SystemMessage):
         return dict(role="system", content=message.content)
     elif isinstance(message, ToolMessage):
         return {
             "role": "tool",
@@ -229,16 +310,15 @@
     client: httpx.Client = Field(default=None)  #: :meta private:
     async_client: httpx.AsyncClient = Field(default=None)  #: :meta private:
     mistral_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     endpoint: str = "https://api.mistral.ai/v1"
     max_retries: int = 5
     timeout: int = 120
     max_concurrent_requests: int = 64
-
-    model: str = "mistral-small"
+    model: str = Field(default="mistral-small", alias="model_name")
     temperature: float = 0.7
     max_tokens: Optional[int] = None
     top_p: float = 1
     """Decode using nucleus sampling: consider the smallest set of tokens whose
        probability sum is at least top_p. Must be in the closed interval [0.0, 1.0]."""
     random_seed: Optional[int] = None
     safe_mode: bool = False
@@ -282,22 +362,25 @@
             stream = kwargs["stream"]
             if stream:
 
                 def iter_sse() -> Iterator[Dict]:
                     with connect_sse(
                         self.client, "POST", "/chat/completions", json=kwargs
                     ) as event_source:
+                        _raise_on_error(event_source.response)
                         for event in event_source.iter_sse():
                             if event.data == "[DONE]":
                                 return
                             yield event.json()
 
                 return iter_sse()
             else:
-                return self.client.post(url="/chat/completions", json=kwargs).json()
+                response = self.client.post(url="/chat/completions", json=kwargs)
+                _raise_on_error(response)
+                return response.json()
 
         rtn = _completion_with_retry(**kwargs)
         return rtn
 
     def _combine_llm_outputs(self, llm_outputs: List[Optional[dict]]) -> dict:
         overall_token_usage: dict = {}
         for output in llm_outputs:
@@ -500,15 +583,14 @@
             **kwargs: Any additional parameters to pass to the
                 :class:`~langchain.runnable.Runnable` constructor.
         """
 
         formatted_tools = [convert_to_openai_tool(tool) for tool in tools]
         return super().bind(tools=formatted_tools, **kwargs)
 
-    @beta()
     def with_structured_output(
         self,
         schema: Union[Dict, Type[BaseModel]],
         *,
         include_raw: bool = False,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, Union[Dict, BaseModel]]:
```

### Comparing `langchain_mistralai-0.1.2rc1/pyproject.toml` & `langchain_mistralai-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.2rc1"
+version = "0.1.4"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
+langchain-core = "^0.1.46"
 tokenizers = "^0.15.1"
 httpx = ">=0.25.2,<1"
 httpx-sse = ">=0.3.1,<1"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_mistralai-0.1.2rc1/PKG-INFO` & `langchain_mistralai-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.2rc1
+Version: 0.1.4
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: httpx-sse (>=0.3.1,<1)
-Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.46,<0.2.0)
 Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai
 Description-Content-Type: text/markdown
 
 # langchain-mistralai
```

