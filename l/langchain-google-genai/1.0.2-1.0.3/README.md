# Comparing `tmp/langchain_google_genai-1.0.2.tar.gz` & `tmp/langchain_google_genai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_genai-1.0.2.tar", max compression
+gzip compressed data, was "langchain_google_genai-1.0.3.tar", max compression
```

## Comparing `langchain_google_genai-1.0.2.tar` & `langchain_google_genai-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/LICENSE
--rw-r--r--   0        0        0     2875 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/README.md
--rw-r--r--   0        0        0     2762 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/__init__.py
--rw-r--r--   0        0        0      136 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_common.py
--rw-r--r--   0        0        0      163 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_enums.py
--rw-r--r--   0        0        0     3640 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_function_utils.py
--rw-r--r--   0        0        0    18736 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_genai_extension.py
--rw-r--r--   0        0        0    23557 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/chat_models.py
--rw-r--r--   0        0        0     4562 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/embeddings.py
--rw-r--r--   0        0        0     4303 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/genai_aqa.py
--rw-r--r--   0        0        0    16139 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/langchain_google_genai/google_vector_store.py
--rw-r--r--   0        0        0    13193 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/langchain_google_genai/llms.py
--rw-r--r--   0        0        0        0 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/langchain_google_genai/py.typed
--rw-r--r--   0        0        0     3012 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2875 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/README.md
+-rw-r--r--   0        0        0     2762 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/__init__.py
+-rw-r--r--   0        0        0      136 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/_common.py
+-rw-r--r--   0        0        0      163 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/_enums.py
+-rw-r--r--   0        0        0     8705 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/_function_utils.py
+-rw-r--r--   0        0        0    18736 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/_genai_extension.py
+-rw-r--r--   0        0        0    29969 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/chat_models.py
+-rw-r--r--   0        0        0     4807 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/embeddings.py
+-rw-r--r--   0        0        0     4303 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/genai_aqa.py
+-rw-r--r--   0        0        0    16139 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/google_vector_store.py
+-rw-r--r--   0        0        0    13518 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/llms.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/py.typed
+-rw-r--r--   0        0        0     3013 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.3/PKG-INFO
```

### Comparing `langchain_google_genai-1.0.2/LICENSE` & `langchain_google_genai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.2/README.md` & `langchain_google_genai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/__init__.py` & `langchain_google_genai-1.0.3/langchain_google_genai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/_genai_extension.py` & `langchain_google_genai-1.0.3/langchain_google_genai/_genai_extension.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/chat_models.py` & `langchain_google_genai-1.0.3/langchain_google_genai/chat_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import base64
 import json
 import logging
 import os
+import uuid
 import warnings
 from io import BytesIO
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
@@ -25,41 +26,58 @@
 import google.ai.generativelanguage as glm
 import google.api_core
 
 # TODO: remove ignore once the google package is published with types
 import google.generativeai as genai  # type: ignore[import]
 import proto  # type: ignore[import]
 import requests
+from google.generativeai.types import SafetySettingDict  # type: ignore[import]
+from google.generativeai.types import Tool as GoogleTool  # type: ignore[import]
+from google.generativeai.types.content_types import (  # type: ignore[import]
+    FunctionDeclarationType,
+    ToolDict,
+)
 from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
+from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     FunctionMessage,
     HumanMessage,
+    InvalidToolCall,
     SystemMessage,
+    ToolCall,
+    ToolCallChunk,
+    ToolMessage,
 )
+from langchain_core.output_parsers.openai_tools import parse_tool_calls
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import SecretStr, root_validator
+from langchain_core.runnables import Runnable
 from langchain_core.utils import get_from_dict_or_env
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
 from langchain_google_genai._common import GoogleGenerativeAIError
 from langchain_google_genai._function_utils import (
+    _tool_choice_to_tool_config,
+    _ToolChoiceType,
+    _ToolConfigDict,
     convert_to_genai_function_declarations,
+    tool_to_dict,
 )
 from langchain_google_genai.llms import GoogleModelFamily, _BaseGoogleGenerativeAI
 
 IMAGE_TYPES: Tuple = ()
 try:
     import PIL
     from PIL.Image import Image
@@ -346,42 +364,141 @@
                             {"output": response}
                             if not isinstance(response, dict)
                             else response
                         ),
                     )
                 )
             ]
+        elif isinstance(message, ToolMessage):
+            role = "user"
+            prev_message: Optional[BaseMessage] = (
+                input_messages[i - 1] if i > 0 else None
+            )
+            if (
+                prev_message
+                and isinstance(prev_message, AIMessage)
+                and prev_message.tool_calls
+            ):
+                # message.name can be null for ToolMessage
+                name: str = prev_message.tool_calls[0]["name"]
+            else:
+                name = message.name  # type: ignore
+            tool_response: Any
+            if not isinstance(message.content, str):
+                tool_response = message.content
+            else:
+                try:
+                    tool_response = json.loads(message.content)
+                except json.JSONDecodeError:
+                    tool_response = message.content  # leave as str representation
+            parts = [
+                glm.Part(
+                    function_response=glm.FunctionResponse(
+                        name=name,
+                        response=(
+                            {"output": tool_response}
+                            if not isinstance(tool_response, dict)
+                            else tool_response
+                        ),
+                    )
+                )
+            ]
         else:
             raise ValueError(
                 f"Unexpected message with type {type(message)} at the position {i}."
             )
 
         messages.append({"role": role, "parts": parts})
     return system_instruction, messages
 
 
 def _parse_response_candidate(
-    response_candidate: glm.Candidate, stream: bool
+    response_candidate: glm.Candidate, streaming: bool = False
 ) -> AIMessage:
-    first_part = response_candidate.content.parts[0]
-    if first_part.function_call:
-        function_call = proto.Message.to_dict(first_part.function_call)
-        function_call["arguments"] = json.dumps(function_call.pop("args", {}))
-        return (AIMessageChunk if stream else AIMessage)(
-            content="", additional_kwargs={"function_call": function_call}
-        )
-    else:
-        parts = response_candidate.content.parts
-
-    if len(parts) == 1 and parts[0].text:
-        content: Union[str, List[Union[str, Dict]]] = parts[0].text
-    else:
-        content = [proto.Message.to_dict(part) for part in parts]
-    return (AIMessageChunk if stream else AIMessage)(
-        content=content, additional_kwargs={}
+    content: Union[None, str, List[str]] = None
+    additional_kwargs = {}
+    tool_calls = []
+    invalid_tool_calls = []
+    tool_call_chunks = []
+
+    for part in response_candidate.content.parts:
+        try:
+            text: Optional[str] = part.text
+        except AttributeError:
+            text = None
+
+        if text is not None:
+            if not content:
+                content = text
+            elif isinstance(content, str) and text:
+                content = [content, text]
+            elif isinstance(content, list) and text:
+                content.append(text)
+            elif text:
+                raise Exception("Unexpected content type")
+
+        if part.function_call:
+            # TODO: support multiple function calls
+            if "function_call" in additional_kwargs:
+                raise Exception("Multiple function calls are not currently supported")
+            function_call = {"name": part.function_call.name}
+            # dump to match other function calling llm for now
+            function_call_args_dict = proto.Message.to_dict(part.function_call)["args"]
+            function_call["arguments"] = json.dumps(
+                {k: function_call_args_dict[k] for k in function_call_args_dict}
+            )
+            additional_kwargs["function_call"] = function_call
+
+            if streaming:
+                tool_call_chunks.append(
+                    ToolCallChunk(
+                        name=function_call.get("name"),
+                        args=function_call.get("arguments"),
+                        id=function_call.get("id", str(uuid.uuid4())),
+                        index=function_call.get("index"),  # type: ignore
+                    )
+                )
+            else:
+                try:
+                    tool_calls_dicts = parse_tool_calls(
+                        [{"function": function_call}],
+                        return_id=False,
+                    )
+                    tool_calls = [
+                        ToolCall(
+                            name=tool_call["name"],
+                            args=tool_call["args"],
+                            id=tool_call.get("id", str(uuid.uuid4())),
+                        )
+                        for tool_call in tool_calls_dicts
+                    ]
+                except Exception as e:
+                    invalid_tool_calls = [
+                        InvalidToolCall(
+                            name=function_call.get("name"),
+                            args=function_call.get("arguments"),
+                            id=function_call.get("id", str(uuid.uuid4())),
+                            error=str(e),
+                        )
+                    ]
+    if content is None:
+        content = ""
+
+    if streaming:
+        return AIMessageChunk(
+            content=cast(Union[str, List[Union[str, Dict[Any, Any]]]], content),
+            additional_kwargs=additional_kwargs,
+            tool_call_chunks=tool_call_chunks,
+        )
+
+    return AIMessage(
+        content=cast(Union[str, List[Union[str, Dict[Any, Any]]]], content),
+        additional_kwargs=additional_kwargs,
+        tool_calls=tool_calls,
+        invalid_tool_calls=invalid_tool_calls,
     )
 
 
 def _response_to_result(
     response: glm.GenerateContentResponse,
     stream: bool = False,
 ) -> ChatResult:
@@ -396,15 +513,15 @@
             generation_info["finish_reason"] = candidate.finish_reason.name
         generation_info["safety_ratings"] = [
             proto.Message.to_dict(safety_rating, use_integers_for_enums=False)
             for safety_rating in candidate.safety_ratings
         ]
         generations.append(
             (ChatGenerationChunk if stream else ChatGeneration)(
-                message=_parse_response_candidate(candidate, stream=stream),
+                message=_parse_response_candidate(candidate, streaming=stream),
                 generation_info=generation_info,
             )
         )
     if not response.candidates:
         # Likely a "prompt feedback" violation (e.g., toxic input)
         # Raising an error would be different than how OpenAI handles it,
         # so we'll just log a warning and continue with an empty message.
@@ -623,28 +740,37 @@
                 await run_manager.on_llm_new_token(gen.text)
             yield gen
 
     def _prepare_chat(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
+        tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
+        functions: Optional[Sequence[FunctionDeclarationType]] = None,
+        safety_settings: Optional[SafetySettingDict] = None,
+        tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
         **kwargs: Any,
     ) -> Tuple[Dict[str, Any], genai.ChatSession, genai.types.ContentDict]:
         client = self.client
-        functions = kwargs.pop("functions", None)
-        safety_settings = kwargs.pop("safety_settings", self.safety_settings)
-        if functions or safety_settings:
-            tools = (
-                convert_to_genai_function_declarations(functions) if functions else None
-            )
+        formatted_tools = None
+        if tools:
+            formatted_tools = [
+                convert_to_genai_function_declarations(tool) for tool in tools
+            ]
+        elif functions:
+            formatted_tools = [convert_to_genai_function_declarations(functions)]
+
+        if formatted_tools or safety_settings:
             client = genai.GenerativeModel(
-                model_name=self.model, tools=tools, safety_settings=safety_settings
+                model_name=self.model,
+                tools=formatted_tools,
+                safety_settings=safety_settings,
             )
 
-        params = self._prepare_params(stop, **kwargs)
+        params = self._prepare_params(stop, tool_config=tool_config, **kwargs)
         system_instruction, history = _parse_chat_history(
             messages,
             convert_system_message_to_human=self.convert_system_message_to_human,
         )
         message = history.pop()
         if self.client._system_instruction != system_instruction:
             self.client = genai.GenerativeModel(
@@ -668,7 +794,41 @@
             result = self.client.count_tokens(text)
             token_count = result.total_tokens
         else:
             result = self.client.count_text_tokens(model=self.model, prompt=text)
             token_count = result["token_count"]
 
         return token_count
+
+    def bind_tools(
+        self,
+        tools: Sequence[Union[ToolDict, GoogleTool]],
+        tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
+        *,
+        tool_choice: Optional[Union[_ToolChoiceType, bool]] = None,
+        **kwargs: Any,
+    ) -> Runnable[LanguageModelInput, BaseMessage]:
+        """Bind tool-like objects to this chat model.
+
+        Assumes model is compatible with google-generativeAI tool-calling API.
+
+        Args:
+            tools: A list of tool definitions to bind to this chat model.
+                Can be a pydantic model, callable, or BaseTool. Pydantic
+                models, callables, and BaseTools will be automatically converted to
+                their schema dictionary representation.
+            **kwargs: Any additional parameters to pass to the
+                :class:`~langchain.runnable.Runnable` constructor.
+        """
+        if tool_choice and tool_config:
+            raise ValueError(
+                "Must specify at most one of tool_choice and tool_config, received "
+                f"both:\n\n{tool_choice=}\n\n{tool_config=}"
+            )
+        # Bind dicts for easier serialization/deserialization.
+        genai_tools = [tool_to_dict(convert_to_genai_function_declarations(tools))]
+        if tool_choice:
+            all_names = [
+                f["name"] for t in genai_tools for f in t["function_declarations"]
+            ]
+            tool_config = _tool_choice_to_tool_config(tool_choice, all_names)
+        return self.bind(tools=genai_tools, tool_config=tool_config, **kwargs)
```

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/embeddings.py` & `langchain_google_genai-1.0.3/langchain_google_genai/embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,19 @@
             "such as `api_endpoint`."
         ),
     )
     transport: Optional[str] = Field(
         None,
         description="A string, one of: [`rest`, `grpc`, `grpc_asyncio`].",
     )
+    request_options: Optional[Dict] = Field(
+        None,
+        description="A dictionary of request options to pass to the Google API client."
+        "Example: `{'timeout': 10}`",
+    )
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validates params and passes them to google-generativeai package."""
         if values.get("credentials"):
             genai.configure(
                 credentials=values.get("credentials"),
@@ -91,14 +96,15 @@
         task_type = self.task_type or "retrieval_document"
         try:
             result = genai.embed_content(
                 model=self.model,
                 content=texts,
                 task_type=task_type,
                 title=title,
+                request_options=self.request_options,
             )
         except Exception as e:
             raise GoogleGenerativeAIError(f"Error embedding content: {e}") from e
         return result["embedding"]
 
     def embed_documents(
         self, texts: List[str], batch_size: int = 5
```

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/genai_aqa.py` & `langchain_google_genai-1.0.3/langchain_google_genai/genai_aqa.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/google_vector_store.py` & `langchain_google_genai-1.0.3/langchain_google_genai/google_vector_store.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.2/langchain_google_genai/llms.py` & `langchain_google_genai-1.0.3/langchain_google_genai/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         try:
             if is_gemini:
                 return llm.client.generate_content(
                     contents=prompt,
                     stream=stream,
                     generation_config=generation_config,
                     safety_settings=kwargs.pop("safety_settings", None),
+                    request_options={"timeout": llm.timeout} if llm.timeout else None,
                 )
             return llm.client.generate_text(prompt=prompt, **kwargs)
         except google.api_core.exceptions.FailedPrecondition as exc:
             if "location is not supported" in exc.message:
                 raise ValueError(error_msg)
 
     return _completion_with_retry(
@@ -139,14 +140,18 @@
     """Maximum number of tokens to include in a candidate. Must be greater than zero.
        If unset, will default to 64."""
     n: int = 1
     """Number of chat completions to generate for each prompt. Note that the API may
        not return the full n completions if duplicates are generated."""
     max_retries: int = 6
     """The maximum number of retries to make when generating."""
+
+    timeout: Optional[float] = None
+    """The maximum number of seconds to wait for a response."""
+
     client_options: Optional[Dict] = Field(
         None,
         description=(
             "A dictionary of client options to pass to the Google API client, "
             "such as `api_endpoint`."
         ),
     )
@@ -255,14 +260,17 @@
 
         if values["top_k"] is not None and values["top_k"] <= 0:
             raise ValueError("top_k must be positive")
 
         if values["max_output_tokens"] is not None and values["max_output_tokens"] <= 0:
             raise ValueError("max_output_tokens must be greater than zero")
 
+        if values["timeout"] is not None and values["timeout"] <= 0:
+            raise ValueError("timeout must be greater than zero")
+
         return values
 
     def _generate(
         self,
         prompts: List[str],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
```

### Comparing `langchain_google_genai-1.0.2/pyproject.toml` & `langchain_google_genai-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-google-genai"
-version = "1.0.2"
+version = "1.0.3"
 description = "An integration package connecting Google's genai package and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-google/tree/main/libs/genai"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = ">=0.1.27,<0.2"
-google-generativeai = "^0.5.0"
+langchain-core = ">=0.1.45,<0.2"
+google-generativeai = "^0.5.2"
 pillow = { version = "^10.1.0", optional = true }
 
 [tool.poetry.extras]
 images = ["pillow"]
 
 [tool.poetry.group.test]
 optional = true
@@ -92,15 +92,15 @@
 #
 # https://docs.pytest.org/en/7.1.x/reference/reference.html
 # --strict-config       any warnings encountered while parsing the `pytest`
 #                       section of the configuration file raise errors.
 #
 # https://github.com/tophat/syrupy
 # --snapshot-warn-unused    Prints a warning on unused snapshots rather than fail the test suite.
-addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
+#addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
 # Registering custom markers.
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
   "compile: mark placeholder test used to compile integration tests without running them",
 ]
```

### Comparing `langchain_google_genai-1.0.2/PKG-INFO` & `langchain_google_genai-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-google-genai
-Version: 1.0.2
+Version: 1.0.3
 Summary: An integration package connecting Google's genai package and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: images
-Requires-Dist: google-generativeai (>=0.5.0,<0.6.0)
-Requires-Dist: langchain-core (>=0.1.27,<0.2)
+Requires-Dist: google-generativeai (>=0.5.2,<0.6.0)
+Requires-Dist: langchain-core (>=0.1.45,<0.2)
 Requires-Dist: pillow (>=10.1.0,<11.0.0) ; extra == "images"
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/genai
 Description-Content-Type: text/markdown
 
 # langchain-google-genai
```

