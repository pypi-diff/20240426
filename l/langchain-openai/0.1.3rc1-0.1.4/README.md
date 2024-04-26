# Comparing `tmp/langchain_openai-0.1.3rc1.tar.gz` & `tmp/langchain_openai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.3rc1.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.4.tar", max compression
```

## Comparing `langchain_openai-0.1.3rc1.tar` & `langchain_openai-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/LICENSE
--rw-r--r--   0        0        0     1627 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/README.md
--rw-r--r--   0        0        0      371 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10508 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    44617 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    23294 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24477 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/py.typed
--rw-r--r--   0        0        0     2865 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/pyproject.toml
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 langchain_openai-0.1.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1627 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/README.md
+-rw-r--r--   0        0        0      371 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10508 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    46560 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    24428 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8008 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24578 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2819 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.4/PKG-INFO
```

### Comparing `langchain_openai-0.1.3rc1/LICENSE` & `langchain_openai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3rc1/README.md` & `langchain_openai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.4/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3rc1/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.4/langchain_openai/chat_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """OpenAI chat wrapper."""
 
 from __future__ import annotations
 
+import json
 import logging
 import os
 import sys
 from operator import itemgetter
 from typing import (
     Any,
     AsyncIterator,
@@ -24,15 +25,14 @@
     Union,
     cast,
     overload,
 )
 
 import openai
 import tiktoken
-from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
@@ -46,16 +46,18 @@
     BaseMessageChunk,
     ChatMessage,
     ChatMessageChunk,
     FunctionMessage,
     FunctionMessageChunk,
     HumanMessage,
     HumanMessageChunk,
+    InvalidToolCall,
     SystemMessage,
     SystemMessageChunk,
+    ToolCall,
     ToolMessage,
     ToolMessageChunk,
 )
 from langchain_core.output_parsers import (
     JsonOutputParser,
     PydanticOutputParser,
 )
@@ -141,46 +143,77 @@
             name=name,
             id=id_,
         )
     else:
         return ChatMessage(content=_dict.get("content", ""), role=role, id=id_)
 
 
+def _format_message_content(content: Any) -> Any:
+    """Format message content."""
+    if content and isinstance(content, list):
+        # Remove unexpected block types
+        formatted_content = []
+        for block in content:
+            if (
+                isinstance(block, dict)
+                and "type" in block
+                and block["type"] == "tool_use"
+            ):
+                continue
+            else:
+                formatted_content.append(block)
+    else:
+        formatted_content = content
+
+    return formatted_content
+
+
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     """Convert a LangChain message to a dictionary.
 
     Args:
         message: The LangChain message.
 
     Returns:
         The dictionary.
     """
     message_dict: Dict[str, Any] = {
-        "content": message.content,
+        "content": _format_message_content(message.content),
     }
     if (name := message.name or message.additional_kwargs.get("name")) is not None:
         message_dict["name"] = name
 
     # populate role and additional message data
     if isinstance(message, ChatMessage):
         message_dict["role"] = message.role
     elif isinstance(message, HumanMessage):
         message_dict["role"] = "user"
     elif isinstance(message, AIMessage):
         message_dict["role"] = "assistant"
         if "function_call" in message.additional_kwargs:
             message_dict["function_call"] = message.additional_kwargs["function_call"]
-            # If function call only, content is None not empty string
-            if message_dict["content"] == "":
-                message_dict["content"] = None
-        if "tool_calls" in message.additional_kwargs:
+        if message.tool_calls or message.invalid_tool_calls:
+            message_dict["tool_calls"] = [
+                _lc_tool_call_to_openai_tool_call(tc) for tc in message.tool_calls
+            ] + [
+                _lc_invalid_tool_call_to_openai_tool_call(tc)
+                for tc in message.invalid_tool_calls
+            ]
+        elif "tool_calls" in message.additional_kwargs:
             message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
-            # If tool calls only, content is None not empty string
-            if message_dict["content"] == "":
-                message_dict["content"] = None
+            tool_call_supported_props = {"id", "type", "function"}
+            message_dict["tool_calls"] = [
+                {k: v for k, v in tool_call.items() if k in tool_call_supported_props}
+                for tool_call in message_dict["tool_calls"]
+            ]
+        else:
+            pass
+        # If tool calls present, content null value should be None not empty string.
+        if "function_call" in message_dict or "tool_calls" in message_dict:
+            message_dict["content"] = message_dict["content"] or None
     elif isinstance(message, SystemMessage):
         message_dict["role"] = "system"
     elif isinstance(message, FunctionMessage):
         message_dict["role"] = "function"
     elif isinstance(message, ToolMessage):
         message_dict["role"] = "tool"
         message_dict["tool_call_id"] = message.tool_call_id
@@ -666,14 +699,16 @@
         except KeyError:
             model = "cl100k_base"
             encoding = tiktoken.get_encoding(model)
         return model, encoding
 
     def get_token_ids(self, text: str) -> List[int]:
         """Get the tokens present in the text with tiktoken package."""
+        if self.custom_get_token_ids is not None:
+            return self.custom_get_token_ids(text)
         # tiktoken NOT supported for Python 3.7 or below
         if sys.version_info[1] <= 7:
             return super().get_token_ids(text)
         _, encoding_model = self._get_encoding_model()
         return encoding_model.encode(text)
 
     def get_num_tokens_from_messages(self, messages: List[BaseMessage]) -> int:
@@ -804,15 +839,18 @@
             if isinstance(tool_choice, str):
                 if tool_choice not in ("auto", "none"):
                     tool_choice = {
                         "type": "function",
                         "function": {"name": tool_choice},
                     }
             elif isinstance(tool_choice, bool):
-                tool_choice = formatted_tools[0]
+                tool_choice = {
+                    "type": "function",
+                    "function": {"name": formatted_tools[0]["function"]["name"]},
+                }
             elif isinstance(tool_choice, dict):
                 if (
                     formatted_tools[0]["function"]["name"]
                     != tool_choice["function"]["name"]
                 ):
                     raise ValueError(
                         f"Tool choice {tool_choice} was specified, but the only "
@@ -844,15 +882,14 @@
         *,
         method: Literal["function_calling", "json_mode"] = "function_calling",
         include_raw: Literal[False] = False,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, _DictOrPydantic]:
         ...
 
-    @beta()
     def with_structured_output(
         self,
         schema: Optional[_DictOrPydanticClass] = None,
         *,
         method: Literal["function_calling", "json_mode"] = "function_calling",
         include_raw: bool = False,
         **kwargs: Any,
@@ -1054,7 +1091,31 @@
             return RunnableMap(raw=llm) | parser_with_fallback
         else:
             return llm | output_parser
 
 
 def _is_pydantic_class(obj: Any) -> bool:
     return isinstance(obj, type) and issubclass(obj, BaseModel)
+
+
+def _lc_tool_call_to_openai_tool_call(tool_call: ToolCall) -> dict:
+    return {
+        "type": "function",
+        "id": tool_call["id"],
+        "function": {
+            "name": tool_call["name"],
+            "arguments": json.dumps(tool_call["args"]),
+        },
+    }
+
+
+def _lc_invalid_tool_call_to_openai_tool_call(
+    invalid_tool_call: InvalidToolCall,
+) -> dict:
+    return {
+        "type": "function",
+        "id": invalid_tool_call["id"],
+        "function": {
+            "name": invalid_tool_call["name"],
+            "arguments": invalid_tool_call["args"],
+        },
+    }
```

### Comparing `langchain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.4/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3rc1/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.4/langchain_openai/embeddings/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,17 @@
     http_client: Union[Any, None] = None
     """Optional httpx.Client. Only used for sync invocations. Must specify 
         http_async_client as well if you'd like a custom client for async invocations.
     """
     http_async_client: Union[Any, None] = None
     """Optional httpx.AsyncClient. Only used for async invocations. Must specify 
         http_client as well if you'd like a custom client for sync invocations."""
+    check_embedding_ctx_length: bool = True
+    """Whether to check the token length of inputs and automatically split inputs 
+        longer than embedding_ctx_length."""
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -507,14 +510,26 @@
             texts: The list of texts to embed.
             chunk_size: The chunk size of embeddings. If None, will use the chunk size
                 specified by the class.
 
         Returns:
             List of embeddings, one for each text.
         """
+        if not self.check_embedding_ctx_length:
+            embeddings: List[List[float]] = []
+            for text in texts:
+                response = self.client.create(
+                    input=text,
+                    **self._invocation_params,
+                )
+                if not isinstance(response, dict):
+                    response = response.dict()
+                embeddings.extend(r["embedding"] for r in response["data"])
+            return embeddings
+
         # NOTE: to keep things simple, we assume the list may contain texts longer
         #       than the maximum context and use length-safe embedding function.
         engine = cast(str, self.deployment)
         return self._get_len_safe_embeddings(texts, engine=engine)
 
     async def aembed_documents(
         self, texts: List[str], chunk_size: Optional[int] = 0
@@ -525,14 +540,26 @@
             texts: The list of texts to embed.
             chunk_size: The chunk size of embeddings. If None, will use the chunk size
                 specified by the class.
 
         Returns:
             List of embeddings, one for each text.
         """
+        if not self.check_embedding_ctx_length:
+            embeddings: List[List[float]] = []
+            for text in texts:
+                response = await self.async_client.create(
+                    input=text,
+                    **self._invocation_params,
+                )
+                if not isinstance(response, dict):
+                    response = response.dict()
+                embeddings.extend(r["embedding"] for r in response["data"])
+            return embeddings
+
         # NOTE: to keep things simple, we assume the list may contain texts longer
         #       than the maximum context and use length-safe embedding function.
         engine = cast(str, self.deployment)
         return await self._aget_len_safe_embeddings(texts, engine=engine)
 
     def embed_query(self, text: str) -> List[float]:
         """Call out to OpenAI's embedding endpoint for embedding query text.
```

### Comparing `langchain_openai-0.1.3rc1/langchain_openai/llms/azure.py` & `langchain_openai-0.1.4/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3rc1/langchain_openai/llms/base.py` & `langchain_openai-0.1.4/langchain_openai/llms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,14 +517,16 @@
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "openai"
 
     def get_token_ids(self, text: str) -> List[int]:
         """Get the token IDs using the tiktoken package."""
+        if self.custom_get_token_ids is not None:
+            return self.custom_get_token_ids(text)
         # tiktoken NOT supported for Python < 3.8
         if sys.version_info[1] < 8:
             return super().get_num_tokens(text)
 
         model_name = self.tiktoken_model_name or self.model_name
         try:
             enc = tiktoken.encoding_for_model(model_name)
```

### Comparing `langchain_openai-0.1.3rc1/pyproject.toml` & `langchain_openai-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.3rc1"
+version = "0.1.4"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
+langchain-core = "^0.1.46"
 openai = "^1.10.0"
 tiktoken = ">=0.5.2,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_openai-0.1.3rc1/PKG-INFO` & `langchain_openai-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.3rc1
+Version: 0.1.4
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.46,<0.2.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

