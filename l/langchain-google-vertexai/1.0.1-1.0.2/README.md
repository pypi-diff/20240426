# Comparing `tmp/langchain_google_vertexai-1.0.1.tar.gz` & `tmp/langchain_google_vertexai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_vertexai-1.0.1.tar", max compression
+gzip compressed data, was "langchain_google_vertexai-1.0.2.tar", max compression
```

## Comparing `langchain_google_vertexai-1.0.1.tar` & `langchain_google_vertexai-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/LICENSE
--rw-r--r--   0        0        0     2594 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/README.md
--rw-r--r--   0        0        0     1853 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/__init__.py
--rw-r--r--   0        0        0     3255 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_anthropic_utils.py
--rw-r--r--   0        0        0    11390 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_base.py
--rw-r--r--   0        0        0      151 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_enums.py
--rw-r--r--   0        0        0     8169 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_image_utils.py
--rw-r--r--   0        0        0     6591 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_utils.py
--rw-r--r--   0        0        0     2511 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/callbacks.py
--rw-r--r--   0        0        0     6062 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/chains.py
--rw-r--r--   0        0        0    39128 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/chat_models.py
--rw-r--r--   0        0        0    16400 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/embeddings.py
--rw-r--r--   0        0        0     6491 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/functions_utils.py
--rw-r--r--   0        0        0    12748 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/gemma.py
--rw-r--r--   0        0        0    11722 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/llms.py
--rw-r--r--   0        0        0     8224 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/model_garden.py
--rw-r--r--   0        0        0        0 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/py.typed
--rw-r--r--   0        0        0      471 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/__init__.py
--rw-r--r--   0        0        0     4679 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_sdk_manager.py
--rw-r--r--   0        0        0     6103 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_searcher.py
--rw-r--r--   0        0        0     5436 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_utils.py
--rw-r--r--   0        0        0     8050 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/document_storage.py
--rw-r--r--   0        0        0    15958 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/vectorstores.py
--rw-r--r--   0        0        0    18548 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vision_models.py
--rw-r--r--   0        0        0     3366 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2594 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/README.md
+-rw-r--r--   0        0        0     1853 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/__init__.py
+-rw-r--r--   0        0        0     3255 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_anthropic_utils.py
+-rw-r--r--   0        0        0    11734 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_base.py
+-rw-r--r--   0        0        0      151 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_enums.py
+-rw-r--r--   0        0        0     8169 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_image_utils.py
+-rw-r--r--   0        0        0     6623 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_utils.py
+-rw-r--r--   0        0        0     2511 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/callbacks.py
+-rw-r--r--   0        0        0     6062 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/chains.py
+-rw-r--r--   0        0        0    41354 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/chat_models.py
+-rw-r--r--   0        0        0    16394 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/embeddings.py
+-rw-r--r--   0        0        0     9948 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/functions_utils.py
+-rw-r--r--   0        0        0    12748 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/gemma.py
+-rw-r--r--   0        0        0    11722 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/llms.py
+-rw-r--r--   0        0        0     8224 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/model_garden.py
+-rw-r--r--   0        0        0        0 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/py.typed
+-rw-r--r--   0        0        0      471 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     4679 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_sdk_manager.py
+-rw-r--r--   0        0        0     6103 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_searcher.py
+-rw-r--r--   0        0        0     5436 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_utils.py
+-rw-r--r--   0        0        0     8050 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/document_storage.py
+-rw-r--r--   0        0        0    15958 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/vectorstores.py
+-rw-r--r--   0        0        0    18548 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vision_models.py
+-rw-r--r--   0        0        0     3366 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.2/PKG-INFO
```

### Comparing `langchain_google_vertexai-1.0.1/LICENSE` & `langchain_google_vertexai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/README.md` & `langchain_google_vertexai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/__init__.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_anthropic_utils.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_base.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,20 @@
                 HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_MEDIUM_AND_ABOVE,
                 HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_ONLY_HIGH,
                 HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_LOW_AND_ABOVE,
                 HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
             }
             """  # noqa: E501
 
+    api_transport: Optional[str] = None
+    """The desired API transport method, can be either 'grpc' or 'rest'"""
+
+    api_endpoint: Optional[str] = None
+    """The desired API endpoint, e.g., us-central1-aiplatform.googleapis.com"""
+
     @property
     def _llm_type(self) -> str:
         return "vertexai"
 
     @property
     def is_codey_model(self) -> bool:
         return is_codey_model(self.model_name)
@@ -157,14 +163,16 @@
 
     @classmethod
     def _init_vertexai(cls, values: Dict) -> None:
         vertexai.init(
             project=values.get("project"),
             location=values.get("location"),
             credentials=values.get("credentials"),
+            api_transport=values.get("api_transport"),
+            api_endpoint=values.get("api_endpoint"),
         )
         return None
 
     def _prepare_params(
         self,
         stop: Optional[List[str]] = None,
         stream: bool = False,
```

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_image_utils.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_image_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_utils.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,21 @@
     Args:
         module (Optional[str]):
             Optional. The module for a custom user agent header.
     Returns:
         Tuple[str, str]
     """
     try:
-        langchain_version = metadata.version("langchain")
+        langchain_version = metadata.version("langchain-google-vertexai")
     except metadata.PackageNotFoundError:
         langchain_version = "0.0.0"
     client_library_version = (
         f"{langchain_version}-{module}" if module else langchain_version
     )
-    return client_library_version, f"langchain/{client_library_version}"
+    return client_library_version, f"langchain-google-vertexai/{client_library_version}"
 
 
 def get_client_info(module: Optional[str] = None) -> "ClientInfo":
     r"""Returns a client info object with a custom user agent header.
 
     Args:
         module (Optional[str]):
```

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/callbacks.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/chains.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/chains.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/chat_models.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/chat_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     Iterator,
     List,
     Optional,
     Sequence,
     Type,
     Union,
     cast,
+    Literal,
+    TypedDict,
+    overload,
 )
 
 import proto  # type: ignore[import-untyped]
 from google.cloud.aiplatform_v1beta1.types.content import Part as GapicPart
 from google.cloud.aiplatform_v1beta1.types.tool import FunctionCall
 from google.cloud.aiplatform import telemetry
 
@@ -43,32 +46,35 @@
     HumanMessage,
     InvalidToolCall,
     SystemMessage,
     ToolCall,
     ToolCallChunk,
     ToolMessage,
 )
-from langchain_core.tools import BaseTool, tool as tool_from_callable
 from langchain_core.output_parsers.base import OutputParserLike
-from langchain_core.output_parsers.openai_functions import (
-    JsonOutputFunctionsParser,
-    PydanticOutputFunctionsParser,
+from langchain_core.output_parsers.openai_tools import (
+    JsonOutputToolsParser,
+    PydanticToolsParser,
 )
 from langchain_core.output_parsers.openai_tools import parse_tool_calls
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, root_validator
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from vertexai.generative_models import (  # type: ignore
     Candidate,
     Content,
     GenerativeModel,
     Part,
+    Tool as VertexTool,
 )
 from vertexai.generative_models._generative_models import (  # type: ignore
     ToolConfig,
+    SafetySettingsType,
+    GenerationConfigType,
+    GenerationResponse,
 )
 from vertexai.language_models import (  # type: ignore
     ChatMessage,
     ChatModel,
     ChatSession,
     CodeChatModel,
     CodeChatSession,
@@ -82,35 +88,48 @@
 )
 
 from langchain_google_vertexai._base import (
     _VertexAICommon,
 )
 from langchain_google_vertexai._image_utils import ImageBytesLoader
 from langchain_google_vertexai._utils import (
+    create_retry_decorator,
     get_generation_info,
     is_codey_model,
     is_gemini_model,
 )
 from langchain_google_vertexai.functions_utils import (
     _format_tool_config,
-    _format_tool_to_vertex_function,
-    _format_tools_to_vertex_tool,
+    _ToolConfigDict,
+    _tool_choice_to_tool_config,
+    _ToolChoiceType,
+    _FunctionDeclarationLike,
+    _VertexToolDict,
+    _format_to_vertex_tool,
+    _format_functions_to_vertex_tool_dict,
 )
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _ChatHistory:
     """Represents a context and a history of messages."""
 
     history: List[ChatMessage] = field(default_factory=list)
     context: Optional[str] = None
 
 
+class _GeminiGenerateContentKwargs(TypedDict):
+    generation_config: Optional[GenerationConfigType]
+    safety_settings: Optional[SafetySettingsType]
+    tools: Optional[List[VertexTool]]
+    tool_config: Optional[ToolConfig]
+
+
 def _parse_chat_history(history: List[BaseMessage]) -> _ChatHistory:
     """Parse a sequence of messages into history.
 
     Args:
         history: The list of messages to re-create the history of the chat.
     Returns:
         A parsed chat history.
@@ -162,105 +181,131 @@
     def _convert_to_parts(message: BaseMessage) -> List[Part]:
         raw_content = message.content
         if isinstance(raw_content, str):
             raw_content = [raw_content]
         return [_convert_to_prompt(part) for part in raw_content]
 
     vertex_messages: List[Content] = []
-    convert_system_message_to_human_content = None
+    system_parts: List[Part] | None = None
     system_instruction = None
+
     for i, message in enumerate(history):
         if isinstance(message, SystemMessage):
+            if i != 0:
+                raise ValueError("SystemMessage should be the first in the history.")
             if system_instruction is not None:
                 raise ValueError(
                     "Detected more than one SystemMessage in the list of messages."
                     "Gemini APIs support the insertion of only one SystemMessage."
                 )
-            else:
-                if convert_system_message_to_human:
-                    logger.warning(
-                        "gemini models released from April 2024 support"
-                        "SystemMessages natively. For best performances,"
-                        "when working with these models,"
-                        "set convert_system_message_to_human to False"
-                    )
-                    convert_system_message_to_human_content = message
-                    continue
-                system_instruction = Content(
-                    role="user", parts=_convert_to_parts(message)
+            if convert_system_message_to_human:
+                logger.warning(
+                    "gemini models released from April 2024 support"
+                    "SystemMessages natively. For best performances,"
+                    "when working with these models,"
+                    "set convert_system_message_to_human to False"
                 )
+                system_parts = _convert_to_parts(message)
                 continue
-        elif (
-            i == 0
-            and isinstance(message, SystemMessage)
-            and convert_system_message_to_human
-        ):
-            convert_system_message_to_human_content = message
-            continue
+            system_instruction = Content(role="user", parts=_convert_to_parts(message))
+        elif isinstance(message, HumanMessage):
+            role = "user"
+            parts = _convert_to_parts(message)
+            if system_parts is not None:
+                if i != 1:
+                    raise ValueError(
+                        "System message should be immediately followed by HumanMessage"
+                    )
+                parts = system_parts + parts
+                system_parts = None
+            vertex_messages.append(Content(role=role, parts=parts))
         elif isinstance(message, AIMessage):
-            raw_function_call = message.additional_kwargs.get("function_call")
             role = "model"
-            if raw_function_call:
+
+            parts = []
+            if message.content:
+                parts = _convert_to_parts(message)
+
+            for tc in message.tool_calls:
                 function_call = FunctionCall(
                     {
-                        "name": raw_function_call["name"],
-                        "args": json.loads(raw_function_call["arguments"]),
+                        "name": tc["name"],
+                        "args": tc["args"],
                     }
                 )
                 gapic_part = GapicPart(function_call=function_call)
-                parts = [Part._from_gapic(gapic_part)]
-            else:
-                parts = _convert_to_parts(message)
-        elif isinstance(message, HumanMessage):
-            role = "user"
-            parts = _convert_to_parts(message)
+                parts.append(Part._from_gapic(gapic_part))
+
+            vertex_messages.append(Content(role=role, parts=parts))
         elif isinstance(message, FunctionMessage):
             role = "function"
-            parts = [
-                Part.from_function_response(
-                    name=message.name,
-                    response={
-                        "content": message.content,
-                    },
-                )
-            ]
+
+            part = Part.from_function_response(
+                name=message.name,
+                response={
+                    "content": message.content,
+                },
+            )
+
+            prev_content = vertex_messages[-1]
+            prev_content_is_function = prev_content and prev_content.role == "function"
+            if prev_content_is_function:
+                parts = prev_content.parts
+                parts.append(part)
+                # replacing last message
+                vertex_messages[-1] = Content(role=role, parts=parts)
+                continue
+
+            parts = [part]
+
+            vertex_messages.append(Content(role=role, parts=parts))
         elif isinstance(message, ToolMessage):
             role = "function"
-            if (i > 0) and isinstance(history[i - 1], AIMessage):
-                # message.name can be null for ToolMessage
-                if history[i - 1].tool_calls:  # type: ignore
-                    name = history[i - 1].tool_calls[0]["name"]  # type: ignore
-                else:
-                    name = message.name
-            else:
-                name = message.name
-            parts = [
-                Part.from_function_response(
-                    name=name,
-                    response={
-                        "content": message.content,
-                    },
-                )
-            ]
+
+            # message.name can be null for ToolMessage
+            name = message.name
+            if name is None:
+                prev_message = history[i - 1] if i > 0 else None
+                if isinstance(prev_message, AIMessage):
+                    tool_call_id = message.tool_call_id
+                    tool_call: ToolCall | None = next(
+                        (t for t in prev_message.tool_calls if t["id"] == tool_call_id),
+                        None,
+                    )
+                    if tool_call is None:
+                        raise ValueError(
+                            (
+                                "Message name is empty and can't find"
+                                + f"corresponding tool call for id: '${tool_call_id}'"
+                            )
+                        )
+                    name = tool_call["name"]
+            part = Part.from_function_response(
+                name=name,
+                response={
+                    "content": message.content,
+                },
+            )
+
+            prev_content = vertex_messages[-1]
+            prev_content_is_function = prev_content and prev_content.role == "function"
+            if prev_content_is_function:
+                parts = prev_content.parts
+                parts.append(part)
+                # replacing last message
+                vertex_messages[-1] = Content(role=role, parts=parts)
+                continue
+
+            parts = [part]
+
+            vertex_messages.append(Content(role=role, parts=parts))
         else:
             raise ValueError(
                 f"Unexpected message with type {type(message)} at the position {i}."
             )
-
-        if convert_system_message_to_human_content:
-            if role == "model":
-                raise ValueError(
-                    "SystemMessage should be followed by a HumanMessage and "
-                    "not by AIMessage."
-                )
-            parts = _convert_to_parts(convert_system_message_to_human_content) + parts
-            convert_system_message_to_human_content = None
-
-        vertex_message = Content(role=role, parts=parts)
-        vertex_messages.append(vertex_message)
     return system_instruction, vertex_messages
 
 
 def _parse_examples(examples: List[BaseMessage]) -> List[InputOutputTextPair]:
     if len(examples) % 2 != 0:
         raise ValueError(
             f"Expect examples to have an even amount of messages, got {len(examples)}."
@@ -296,94 +341,162 @@
     if not isinstance(question, HumanMessage):
         raise ValueError(
             f"Last message in the list should be from human, got {question.type}."
         )
     return question
 
 
-def _get_client_with_sys_instruction(
-    client: GenerativeModel,
-    system_instruction: Content,
-    model_name: str,
-):
-    if client._system_instruction != system_instruction:
-        client = GenerativeModel(
-            model_name=model_name,
-            system_instruction=system_instruction,
-        )
-    return client
+@overload
+def _parse_response_candidate(
+    response_candidate: "Candidate", streaming: Literal[False] = False
+) -> AIMessage:
+    ...
+
+
+@overload
+def _parse_response_candidate(
+    response_candidate: "Candidate", streaming: Literal[True]
+) -> AIMessageChunk:
+    ...
 
 
 def _parse_response_candidate(
     response_candidate: "Candidate", streaming: bool = False
 ) -> AIMessage:
-    try:
-        content = response_candidate.text
-    except AttributeError:
-        content = ""
-
+    content: Union[None, str, List[str]] = None
     additional_kwargs = {}
-    first_part = response_candidate.content.parts[0]
-    if first_part.function_call:
-        function_call = {"name": first_part.function_call.name}
-        # dump to match other function calling llm for now
-        function_call_args_dict = proto.Message.to_dict(first_part.function_call)[
-            "args"
-        ]
-        function_call["arguments"] = json.dumps(
-            {k: function_call_args_dict[k] for k in function_call_args_dict}
-        )
-        additional_kwargs["function_call"] = function_call
-        if streaming:
-            tool_call_chunks = [
-                ToolCallChunk(
-                    name=function_call.get("name"),
-                    args=function_call.get("arguments"),
-                    id=function_call.get("id", str(uuid.uuid4())),
-                    index=function_call.get("index"),
-                )
-            ]
-            return AIMessageChunk(
-                content=content,
-                additional_kwargs=additional_kwargs,
-                tool_call_chunks=tool_call_chunks,
-            )
-        else:
-            tool_calls = []
-            invalid_tool_calls = []
-            try:
-                tool_calls_dicts = parse_tool_calls(
-                    [{"function": function_call}],
-                    return_id=False,
-                )
-                tool_calls = [
-                    ToolCall(
-                        name=tool_call["name"],
-                        args=tool_call["args"],
-                        id=tool_call.get("id", str(uuid.uuid4())),
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
+            if content is None:
+                content = text
+            elif isinstance(content, str):
+                content = [content, text]
+            elif isinstance(content, list):
+                content.append(text)
+            else:
+                raise Exception("Unexpected content type")
+
+        if part.function_call:
+            if "function_call" in additional_kwargs:
+                logger.warning(
+                    (
+                        "This model can reply with multiple "
+                        "function calls in one response. "
+                        "Please don't rely on `additional_kwargs.function_call` "
+                        "as only the last one will be saved."
+                        "Use `tool_calls` instead."
                     )
-                    for tool_call in tool_calls_dicts
-                ]
-            except Exception as e:
-                invalid_tool_calls = [
-                    InvalidToolCall(
+                )
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
                         name=function_call.get("name"),
                         args=function_call.get("arguments"),
                         id=function_call.get("id", str(uuid.uuid4())),
-                        error=str(e),
+                        index=function_call.get("index"),
+                    )
+                )
+            else:
+                try:
+                    tool_calls_dicts = parse_tool_calls(
+                        [{"function": function_call}],
+                        return_id=False,
+                    )
+                    tool_calls.extend(
+                        [
+                            ToolCall(
+                                name=tool_call["name"],
+                                args=tool_call["args"],
+                                id=tool_call.get("id", str(uuid.uuid4())),
+                            )
+                            for tool_call in tool_calls_dicts
+                        ]
                     )
-                ]
+                except Exception as e:
+                    invalid_tool_calls.append(
+                        InvalidToolCall(
+                            name=function_call.get("name"),
+                            args=function_call.get("arguments"),
+                            id=function_call.get("id", str(uuid.uuid4())),
+                            error=str(e),
+                        )
+                    )
+    if content is None:
+        content = ""
 
-            return AIMessage(
-                content=content,
-                additional_kwargs=additional_kwargs,
-                tool_calls=tool_calls,
-                invalid_tool_calls=invalid_tool_calls,
-            )
-    return AIMessage(content=content, additional_kwargs=additional_kwargs)
+    if streaming:
+        return AIMessageChunk(
+            content=cast(Union[str, List[Union[str, Dict[Any, Any]]]], content),
+            additional_kwargs=additional_kwargs,
+            tool_call_chunks=tool_call_chunks,
+        )
+
+    return AIMessage(
+        content=cast(Union[str, List[Union[str, Dict[Any, Any]]]], content),
+        tool_calls=tool_calls,
+        additional_kwargs=additional_kwargs,
+        invalid_tool_calls=invalid_tool_calls,
+    )
+
+
+def _completion_with_retry(
+    generation_method: Callable,
+    *,
+    max_retries: int,
+    run_manager: Optional[CallbackManagerForLLMRun] = None,
+    **kwargs: Any,
+) -> Any:
+    """Use tenacity to retry the completion call."""
+    retry_decorator = create_retry_decorator(
+        max_retries=max_retries, run_manager=run_manager
+    )
+
+    @retry_decorator
+    def _completion_with_retry_inner(generation_method: Callable, **kwargs: Any) -> Any:
+        return generation_method(**kwargs)
+
+    return _completion_with_retry_inner(generation_method, **kwargs)
+
+
+async def _acompletion_with_retry(
+    generation_method: Callable,
+    *,
+    max_retries: int,
+    run_manager: Optional[CallbackManagerForLLMRun] = None,
+    **kwargs: Any,
+) -> Any:
+    """Use tenacity to retry the completion call."""
+    retry_decorator = create_retry_decorator(
+        max_retries=max_retries, run_manager=run_manager
+    )
+
+    @retry_decorator
+    async def _completion_with_retry_inner(
+        generation_method: Callable, **kwargs: Any
+    ) -> Any:
+        return await generation_method(**kwargs)
+
+    return await _completion_with_retry_inner(generation_method, **kwargs)
 
 
 class ChatVertexAI(_VertexAICommon, BaseChatModel):
     """`Vertex AI` Chat large language models API."""
 
     model_name: str = "chat-bison"
     "Underlying model name."
@@ -444,21 +557,17 @@
                 generative_model_name
             )
         return values
 
     @property
     def _is_gemini_advanced(self) -> bool:
         try:
-            if float(self.model_name.split("-")[1]) > 1.0:
-                return True
-        except ValueError:
-            pass
-        except IndexError:
-            pass
-        return False
+            return float(self.model_name.split("-")[1]) > 1.0
+        except (ValueError, IndexError):
+            return False
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         stream: Optional[bool] = None,
@@ -475,88 +584,68 @@
 
         Returns:
             The ChatResult that contains outputs generated by the model.
 
         Raises:
             ValueError: if the last message in the list is not from human.
         """
-        should_stream = stream if stream is not None else self.streaming
-        safety_settings = kwargs.pop("safety_settings", None)
-        if should_stream:
-            with telemetry.tool_context_manager(self._user_agent):
-                stream_iter = self._stream(
-                    messages, stop=stop, run_manager=run_manager, **kwargs
-                )
-                return generate_from_stream(stream_iter)
+        if stream is True or (stream is None and self.streaming):
+            stream_iter = self._stream(
+                messages, stop=stop, run_manager=run_manager, **kwargs
+            )
+            return generate_from_stream(stream_iter)
+        if not self._is_gemini_model:
+            return self._generate_non_gemini(messages, stop=stop, **kwargs)
 
+        client, contents = self._gemini_client_and_contents(messages)
+        params = self._gemini_params(stop=stop, **kwargs)
+        with telemetry.tool_context_manager(self._user_agent):
+            response = _completion_with_retry(
+                client.generate_content,
+                max_retries=self.max_retries,
+                contents=contents,
+                **params,
+            )
+        return self._gemini_response_to_chat_result(response)
+
+    def _generate_non_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        **kwargs: Any,
+    ) -> ChatResult:
+        kwargs.pop("safety_settings", None)
         params = self._prepare_params(stop=stop, stream=False, **kwargs)
+        question = _get_question(messages)
+        history = _parse_chat_history(messages[:-1])
+        examples = kwargs.get("examples") or self.examples
         msg_params = {}
         if "candidate_count" in params:
             msg_params["candidate_count"] = params.pop("candidate_count")
-
-        if self._is_gemini_model:
-            system_instruction, history_gemini = _parse_chat_history_gemini(
-                messages,
-                project=self.project,
-                convert_system_message_to_human=self.convert_system_message_to_human,
-            )
-            self.client = _get_client_with_sys_instruction(
-                client=self.client,
-                system_instruction=system_instruction,
-                model_name=self.model_name,
-            )
-
-            # set param to `functions` until core tool/function calling implemented
-            raw_tools = params.pop("functions") if "functions" in params else None
-            tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
-            raw_tool_config = (
-                params.pop("tool_config") if "tool_config" in params else None
-            )
-            tool_config = (
-                _format_tool_config(raw_tool_config) if raw_tool_config else None
-            )
-            with telemetry.tool_context_manager(self._user_agent):
-                response = self.client.generate_content(
-                    history_gemini,
-                    generation_config=params,
-                    tools=tools,
-                    tool_config=tool_config,
-                    safety_settings=safety_settings,
-                )
-            generations = [
-                ChatGeneration(
-                    message=_parse_response_candidate(candidate),
-                    generation_info=get_generation_info(
-                        candidate,
-                        self._is_gemini_model,
-                        usage_metadata=response.to_dict().get("usage_metadata"),
-                    ),
-                )
-                for candidate in response.candidates
-            ]
-        else:
-            question = _get_question(messages)
-            history = _parse_chat_history(messages[:-1])
-            examples = kwargs.get("examples") or self.examples
-            if examples:
-                params["examples"] = _parse_examples(examples)
-            with telemetry.tool_context_manager(self._user_agent):
-                chat = self._start_chat(history, **params)
-                response = chat.send_message(question.content, **msg_params)
-            generations = [
-                ChatGeneration(
-                    message=AIMessage(content=candidate.text),
-                    generation_info=get_generation_info(
-                        candidate,
-                        self._is_gemini_model,
-                        usage_metadata=response.raw_prediction_response.metadata,
-                    ),
-                )
-                for candidate in response.candidates
-            ]
+        if examples:
+            params["examples"] = _parse_examples(examples)
+        with telemetry.tool_context_manager(self._user_agent):
+            chat = self._start_chat(history, **params)
+            response = _completion_with_retry(
+                chat.send_message,
+                max_retries=self.max_retries,
+                message=question.content,
+                **msg_params,
+            )
+        generations = [
+            ChatGeneration(
+                message=AIMessage(content=candidate.text),
+                generation_info=get_generation_info(
+                    candidate,
+                    self._is_gemini_model,
+                    usage_metadata=response.raw_prediction_response.metadata,
+                ),
+            )
+            for candidate in response.candidates
+        ]
         return ChatResult(generations=generations)
 
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
@@ -576,220 +665,145 @@
         Raises:
             ValueError: if the last message in the list is not from human.
         """
         if "stream" in kwargs:
             kwargs.pop("stream")
             logger.warning("ChatVertexAI does not currently support async streaming.")
 
-        params = self._prepare_params(stop=stop, **kwargs)
-        safety_settings = kwargs.pop("safety_settings", None)
+        if not self._is_gemini_model:
+            return await self._agenerate_non_gemini(messages, stop=stop, **kwargs)
+
+        client, contents = self._gemini_client_and_contents(messages)
+        params = self._gemini_params(stop=stop, **kwargs)
+        with telemetry.tool_context_manager(self._user_agent):
+            response = await _acompletion_with_retry(
+                client.generate_content_async,
+                max_retries=self.max_retries,
+                contents=contents,
+                **params,
+            )
+        return self._gemini_response_to_chat_result(response)
+
+    async def _agenerate_non_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        **kwargs: Any,
+    ) -> ChatResult:
+        kwargs.pop("safety_settings", None)
+        params = self._prepare_params(stop=stop, stream=False, **kwargs)
+        question = _get_question(messages)
+        history = _parse_chat_history(messages[:-1])
+        examples = kwargs.get("examples") or self.examples
         msg_params = {}
         if "candidate_count" in params:
             msg_params["candidate_count"] = params.pop("candidate_count")
-
-        if self._is_gemini_model:
-            system_instruction, history_gemini = _parse_chat_history_gemini(
-                messages,
-                project=self.project,
-                convert_system_message_to_human=self.convert_system_message_to_human,
-            )
-
-            self.client = _get_client_with_sys_instruction(
-                client=self.client,
-                system_instruction=system_instruction,
-                model_name=self.model_name,
-            )
-            # set param to `functions` until core tool/function calling implemented
-            raw_tools = params.pop("functions") if "functions" in params else None
-            tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
-            raw_tool_config = (
-                params.pop("tool_config") if "tool_config" in params else None
-            )
-            tool_config = (
-                _format_tool_config(raw_tool_config) if raw_tool_config else None
-            )
-            with telemetry.tool_context_manager(self._user_agent):
-                response = await self.client.generate_content_async(
-                    history_gemini,
-                    generation_config=params,
-                    tools=tools,
-                    tool_config=tool_config,
-                    safety_settings=safety_settings,
-                )
-            generations = [
-                ChatGeneration(
-                    message=_parse_response_candidate(c),
-                    generation_info=get_generation_info(
-                        c,
-                        self._is_gemini_model,
-                        usage_metadata=response.to_dict().get("usage_metadata"),
-                    ),
-                )
-                for c in response.candidates
-            ]
-        else:
-            question = _get_question(messages)
-            history = _parse_chat_history(messages[:-1])
-            examples = kwargs.get("examples", None) or self.examples
-            if examples:
-                params["examples"] = _parse_examples(examples)
-            with telemetry.tool_context_manager(self._user_agent):
-                chat = self._start_chat(history, **params)
-                response = await chat.send_message_async(question.content, **msg_params)
-            generations = [
-                ChatGeneration(
-                    message=AIMessage(content=r.text),
-                    generation_info=get_generation_info(
-                        r,
-                        self._is_gemini_model,
-                        usage_metadata=response.raw_prediction_response.metadata,
-                    ),
-                )
-                for r in response.candidates
-            ]
+        if examples:
+            params["examples"] = _parse_examples(examples)
+        with telemetry.tool_context_manager(self._user_agent):
+            chat = self._start_chat(history, **params)
+            response = await _acompletion_with_retry(
+                chat.send_message_async,
+                message=question.content,
+                max_retries=self.max_retries,
+                **msg_params,
+            )
+        generations = [
+            ChatGeneration(
+                message=AIMessage(content=candidate.text),
+                generation_info=get_generation_info(
+                    candidate,
+                    self._is_gemini_model,
+                    usage_metadata=response.raw_prediction_response.metadata,
+                ),
+            )
+            for candidate in response.candidates
+        ]
         return ChatResult(generations=generations)
 
     def _stream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
+        if not self._is_gemini_model:
+            yield from self._stream_non_gemini(
+                messages, stop=stop, run_manager=run_manager, **kwargs
+            )
+            return
+
+        client, contents = self._gemini_client_and_contents(messages)
+        params = self._gemini_params(stop=stop, stream=True, **kwargs)
+        with telemetry.tool_context_manager(self._user_agent):
+            response_iter = _completion_with_retry(
+                client.generate_content,
+                max_retries=self.max_retries,
+                contents=contents,
+                stream=True,
+                **params,
+            )
+        for response_chunk in response_iter:
+            chunk = self._gemini_chunk_to_generation_chunk(response_chunk)
+            if run_manager and isinstance(chunk.message.content, str):
+                run_manager.on_llm_new_token(chunk.message.content)
+            yield chunk
+
+    def _stream_non_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        run_manager: Optional[CallbackManagerForLLMRun] = None,
+        **kwargs: Any,
+    ) -> Iterator[ChatGenerationChunk]:
         params = self._prepare_params(stop=stop, stream=True, **kwargs)
-        if self._is_gemini_model:
-            safety_settings = params.pop("safety_settings", None)
-            system_instruction, history_gemini = _parse_chat_history_gemini(
-                messages,
-                project=self.project,
-                convert_system_message_to_human=self.convert_system_message_to_human,
-            )
-            self.client = _get_client_with_sys_instruction(
-                client=self.client,
-                system_instruction=system_instruction,
-                model_name=self.model_name,
-            )
-            # set param to `functions` until core tool/function calling implemented
-            raw_tools = params.pop("functions") if "functions" in params else None
-            tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
-            raw_tool_config = (
-                params.pop("tool_config") if "tool_config" in params else None
-            )
-            tool_config = (
-                _format_tool_config(raw_tool_config) if raw_tool_config else None
-            )
-            with telemetry.tool_context_manager(self._user_agent):
-                responses = self.client.generate_content(
-                    history_gemini,
-                    stream=True,
-                    generation_config=params,
-                    tools=tools,
-                    tool_config=tool_config,
-                    safety_settings=safety_settings,
-                )
-                for response in responses:
-                    message = _parse_response_candidate(
-                        response.candidates[0], streaming=True
-                    )
-                    generation_info = get_generation_info(
-                        response.candidates[0],
+        question = _get_question(messages)
+        history = _parse_chat_history(messages[:-1])
+        examples = kwargs.get("examples", None)
+        if examples:
+            params["examples"] = _parse_examples(examples)
+        with telemetry.tool_context_manager(self._user_agent):
+            chat = self._start_chat(history, **params)
+            responses = chat.send_message_streaming(question.content, **params)
+            for response in responses:
+                if run_manager:
+                    run_manager.on_llm_new_token(response.text)
+                yield ChatGenerationChunk(
+                    message=AIMessageChunk(content=response.text),
+                    generation_info=get_generation_info(
+                        response,
                         self._is_gemini_model,
-                        usage_metadata=response.to_dict().get("usage_metadata"),
-                    )
-                    if run_manager and isinstance(message.content, str):
-                        run_manager.on_llm_new_token(message.content)
-                    if isinstance(message, AIMessageChunk):
-                        yield ChatGenerationChunk(
-                            message=message,
-                            generation_info=generation_info,
-                        )
-                    else:
-                        yield ChatGenerationChunk(
-                            message=AIMessageChunk(
-                                content=message.content,
-                                additional_kwargs=message.additional_kwargs,
-                            ),
-                            generation_info=generation_info,
-                        )
-        else:
-            question = _get_question(messages)
-            history = _parse_chat_history(messages[:-1])
-            examples = kwargs.get("examples", None)
-            if examples:
-                params["examples"] = _parse_examples(examples)
-            with telemetry.tool_context_manager(self._user_agent):
-                chat = self._start_chat(history, **params)
-                responses = chat.send_message_streaming(question.content, **params)
-                for response in responses:
-                    if run_manager:
-                        run_manager.on_llm_new_token(response.text)
-                    yield ChatGenerationChunk(
-                        message=AIMessageChunk(content=response.text),
-                        generation_info=get_generation_info(
-                            response,
-                            self._is_gemini_model,
-                            usage_metadata=response.raw_prediction_response.metadata,
-                        ),
-                    )
+                        usage_metadata=response.raw_prediction_response.metadata,
+                    ),
+                )
 
     async def _astream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         if not self._is_gemini_model:
             raise NotImplementedError()
-        params = self._prepare_params(stop=stop, stream=True, **kwargs)
-        safety_settings = params.pop("safety_settings", None)
-        system_instruction, history_gemini = _parse_chat_history_gemini(
-            messages,
-            project=self.project,
-            convert_system_message_to_human=self.convert_system_message_to_human,
-        )
-        self.client = _get_client_with_sys_instruction(
-            client=self.client,
-            system_instruction=system_instruction,
-            model_name=self.model_name,
-        )
-        raw_tools = params.pop("functions") if "functions" in params else None
-        tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
-        raw_tool_config = params.pop("tool_config") if "tool_config" in params else None
-        tool_config = _format_tool_config(raw_tool_config) if raw_tool_config else None
+        client, contents = self._gemini_client_and_contents(messages)
+        params = self._gemini_params(stop=stop, stream=True, **kwargs)
         with telemetry.tool_context_manager(self._user_agent):
-            async for chunk in await self.client.generate_content_async(
-                history_gemini,
+            async for response_chunk in await _acompletion_with_retry(
+                client.generate_content_async,
+                max_retries=self.max_retries,
+                contents=contents,
                 stream=True,
-                generation_config=params,
-                tools=tools,
-                tool_config=tool_config,
-                safety_settings=safety_settings,
+                **params,
             ):
-                message = _parse_response_candidate(chunk.candidates[0], streaming=True)
-                generation_info = get_generation_info(
-                    chunk.candidates[0],
-                    self._is_gemini_model,
-                    usage_metadata=chunk.to_dict().get("usage_metadata"),
-                )
-                if run_manager and isinstance(message.content, str):
-                    await run_manager.on_llm_new_token(message.content)
-                if isinstance(message, AIMessageChunk):
-                    yield ChatGenerationChunk(
-                        message=message,
-                        generation_info=generation_info,
-                    )
-                else:
-                    yield ChatGenerationChunk(
-                        message=AIMessageChunk(
-                            content=message.content,
-                            additional_kwargs=message.additional_kwargs,
-                        ),
-                        generation_info=generation_info,
-                    )
+                chunk = self._gemini_chunk_to_generation_chunk(response_chunk)
+                if run_manager and isinstance(chunk.message.content, str):
+                    await run_manager.on_llm_new_token(chunk.message.content)
+                yield chunk
 
     def with_structured_output(
         self,
         schema: Union[Dict, Type[BaseModel]],
         *,
         include_raw: bool = False,
         **kwargs: Any,
@@ -880,79 +894,168 @@
                 #     'justification': 'Both a pound of bricks and a pound of feathers weigh one pound. The weight is the same, but the volume and density of the two substances differ.'
                 # }
 
         """  # noqa: E501
         if kwargs:
             raise ValueError(f"Received unsupported arguments {kwargs}")
         if isinstance(schema, type) and issubclass(schema, BaseModel):
-            parser: OutputParserLike = PydanticOutputFunctionsParser(
-                pydantic_schema=schema
+            parser: OutputParserLike = PydanticToolsParser(
+                tools=[schema], first_tool_only=True
             )
         else:
-            parser = JsonOutputFunctionsParser()
-
-        name = _format_tool_to_vertex_function(schema)["name"]
-
-        if self._is_gemini_advanced:
-            llm = self.bind(
-                functions=[schema],
-                tool_config={
-                    "function_calling_config": {
-                        "mode": ToolConfig.FunctionCallingConfig.Mode.ANY,
-                        "allowed_function_names": [name],
-                    }
-                },
-            )
-        else:
-            llm = self.bind(functions=[schema])
+            parser = JsonOutputToolsParser()
+        llm = self.bind_tools([schema], tool_choice=self._is_gemini_advanced)
         if include_raw:
             parser_with_fallback = RunnablePassthrough.assign(
                 parsed=itemgetter("raw") | parser, parsing_error=lambda _: None
             ).with_fallbacks(
                 [RunnablePassthrough.assign(parsed=lambda _: None)],
                 exception_key="parsing_error",
             )
             return {"raw": llm} | parser_with_fallback
         else:
             return llm | parser
 
     def bind_tools(
         self,
-        tools: Sequence[Union[Type[BaseModel], Callable, BaseTool]],
-        tool_config: Optional[Dict[str, Any]] = None,
+        tools: Sequence[Union[_FunctionDeclarationLike, VertexTool]],
+        tool_config: Optional[_ToolConfigDict] = None,
+        *,
+        tool_choice: Optional[Union[_ToolChoiceType, bool]] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
         Assumes model is compatible with Vertex tool-calling API.
 
         Args:
             tools: A list of tool definitions to bind to this chat model.
                 Can be a pydantic model, callable, or BaseTool. Pydantic
                 models, callables, and BaseTools will be automatically converted to
                 their schema dictionary representation.
             **kwargs: Any additional parameters to pass to the
                 :class:`~langchain.runnable.Runnable` constructor.
         """
-        formatted_tools = []
+        if tool_choice and tool_config:
+            raise ValueError(
+                "Must specify at most one of tool_choice and tool_config, received "
+                f"both:\n\n{tool_choice=}\n\n{tool_config=}"
+            )
+        vertexai_tools: List[_VertexToolDict] = []
+        vertexai_functions = []
         for schema in tools:
-            if isinstance(schema, BaseTool) or (
-                isinstance(schema, type) and issubclass(schema, BaseModel)
-            ):
-                formatted_tools.append(schema)
-            elif callable(schema):
-                formatted_tools.append(tool_from_callable(schema))  # type: ignore
-            else:
-                raise ValueError(
-                    "Tool must be a BaseTool, Pydantic model, or callable."
+            if isinstance(schema, VertexTool):
+                vertexai_tools.append(
+                    {"function_declarations": schema.to_dict()["function_declarations"]}
                 )
-        return self.bind(functions=formatted_tools, tool_config=tool_config, **kwargs)
+            elif isinstance(schema, dict) and "function_declarations" in schema:
+                vertexai_tools.append(cast(_VertexToolDict, schema))
+            else:
+                vertexai_functions.append(schema)
+        vertexai_tools.append(_format_functions_to_vertex_tool_dict(vertexai_functions))
+        if tool_choice:
+            all_names = [
+                f["name"] for vt in vertexai_tools for f in vt["function_declarations"]
+            ]
+            tool_config = _tool_choice_to_tool_config(tool_choice, all_names)
+        # Bind dicts for easier serialization/deserialization.
+        return self.bind(tools=vertexai_tools, tool_config=tool_config, **kwargs)
 
     def _start_chat(
         self, history: _ChatHistory, **kwargs: Any
     ) -> Union[ChatSession, CodeChatSession]:
         if not self.is_codey_model:
             return self.client.start_chat(
                 context=history.context, message_history=history.history, **kwargs
             )
         else:
             return self.client.start_chat(message_history=history.history, **kwargs)
+
+    def _gemini_params(
+        self,
+        *,
+        stop: Optional[List[str]] = None,
+        stream: bool = False,
+        tools: Optional[List[Union[_VertexToolDict, VertexTool]]] = None,
+        functions: Optional[List[_FunctionDeclarationLike]] = None,
+        tool_config: Optional[Union[_ToolConfigDict, ToolConfig]] = None,
+        safety_settings: Optional[SafetySettingsType] = None,
+        **kwargs: Any,
+    ) -> _GeminiGenerateContentKwargs:
+        generation_config = self._prepare_params(stop=stop, stream=stream, **kwargs)
+        if tools:
+            tools = [_format_to_vertex_tool(tool) for tool in tools]
+        elif functions:
+            tools = [_format_to_vertex_tool(functions)]
+        else:
+            pass
+
+        if tool_config and not isinstance(tool_config, ToolConfig):
+            tool_config = _format_tool_config(cast(_ToolConfigDict, tool_config))
+
+        return _GeminiGenerateContentKwargs(
+            generation_config=generation_config,
+            tools=tools,
+            tool_config=tool_config,
+            safety_settings=safety_settings,
+        )
+
+    def _gemini_client_and_contents(
+        self, messages: List[BaseMessage]
+    ) -> tuple[GenerativeModel, list[Content]]:
+        system, contents = _parse_chat_history_gemini(
+            messages,
+            project=self.project,
+            convert_system_message_to_human=self.convert_system_message_to_human,
+        )
+        # TODO: Store default client params explicitly so private params don't have to
+        # be accessed, like _safety_settings.
+        client = GenerativeModel(
+            model_name=self.model_name,
+            system_instruction=system,
+            safety_settings=self.client._safety_settings,
+        )
+        return client, contents
+
+    def _gemini_response_to_chat_result(
+        self, response: GenerationResponse
+    ) -> ChatResult:
+        generations = []
+        usage = response.to_dict().get("usage_metadata")
+        for candidate in response.candidates:
+            info = get_generation_info(candidate, is_gemini=True, usage_metadata=usage)
+            message = _parse_response_candidate(candidate)
+            generations.append(ChatGeneration(message=message, generation_info=info))
+        if not response.candidates:
+            message = AIMessage(content="")
+            if usage:
+                generation_info = {"usage_metadata": usage}
+            else:
+                generation_info = {}
+            generations.append(
+                ChatGeneration(message=message, generation_info=generation_info)
+            )
+        return ChatResult(generations=generations)
+
+    def _gemini_chunk_to_generation_chunk(
+        self, response_chunk: GenerationResponse
+    ) -> ChatGenerationChunk:
+        # return an empty completion message if there's no candidates
+        usage_metadata = response_chunk.to_dict().get("usage_metadata")
+        if not response_chunk.candidates:
+            message = AIMessageChunk(content="")
+            if usage_metadata:
+                generation_info = {"usage_metadata": usage_metadata}
+            else:
+                generation_info = {}
+        else:
+            top_candidate = response_chunk.candidates[0]
+            message = _parse_response_candidate(top_candidate, streaming=True)
+            generation_info = get_generation_info(
+                top_candidate,
+                is_gemini=True,
+                usage_metadata=usage_metadata,
+            )
+        return ChatGenerationChunk(
+            message=message,
+            generation_info=generation_info,
+        )
```

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/embeddings.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 class GoogleEmbeddingModelType(str, Enum):
     TEXT = auto()
     MULTIMODAL = auto()
 
     @classmethod
     def _missing_(cls, value: Any) -> Optional["GoogleEmbeddingModelType"]:
-        if "textembedding-gecko" in value.lower():
+        if value.lower().startswith("text"):
             return GoogleEmbeddingModelType.TEXT
         elif "multimodalembedding" in value.lower():
             return GoogleEmbeddingModelType.MULTIMODAL
         return None
 
 
 class VertexAIEmbeddings(_VertexAICommon, Embeddings):
```

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/gemma.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/gemma.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/llms.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/model_garden.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/model_garden.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_sdk_manager.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_sdk_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_searcher.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_searcher.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_utils.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/document_storage.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/document_storage.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/vectorstores.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vision_models.py` & `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vision_models.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.1/pyproject.toml` & `langchain_google_vertexai-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "langchain-google-vertexai"
 
-version = "1.0.1"
+version = "1.0.2"
 description = "An integration package connecting Google VertexAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_google_vertexai-1.0.1/PKG-INFO` & `langchain_google_vertexai-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-vertexai
-Version: 1.0.1
+Version: 1.0.2
 Summary: An integration package connecting Google VertexAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

