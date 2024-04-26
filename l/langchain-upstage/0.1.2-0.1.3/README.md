# Comparing `tmp/langchain_upstage-0.1.2.tar.gz` & `tmp/langchain_upstage-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.2.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.3.tar", max compression
```

## Comparing `langchain_upstage-0.1.2.tar` & `langchain_upstage-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/LICENSE
--rw-r--r--   0        0        0      979 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/README.md
--rw-r--r--   0        0        0      496 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9097 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0     6430 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/layout_analysis.py
--rw-r--r--   0        0        0    12390 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/layout_analysis_parsers.py
--rw-r--r--   0        0        0        0 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/py.typed
--rw-r--r--   0        0        0     3574 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/tools/groundedness_check.py
--rw-r--r--   0        0        0     2727 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/LICENSE
+-rw-r--r--   0        0        0      979 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/README.md
+-rw-r--r--   0        0        0      567 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9097 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0     6430 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/layout_analysis.py
+-rw-r--r--   0        0        0    12390 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/layout_analysis_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     4323 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/langchain_upstage/tools/groundedness_check.py
+-rw-r--r--   0        0        0     2727 2024-04-26 17:36:42.225502 langchain_upstage-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.3/PKG-INFO
```

### Comparing `langchain_upstage-0.1.2/LICENSE` & `langchain_upstage-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.2/README.md` & `langchain_upstage-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.2/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.3/langchain_upstage/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.2/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.3/langchain_upstage/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.2/langchain_upstage/layout_analysis.py` & `langchain_upstage-0.1.3/langchain_upstage/layout_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.2/langchain_upstage/layout_analysis_parsers.py` & `langchain_upstage-0.1.3/langchain_upstage/layout_analysis_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.2/langchain_upstage/tools/groundedness_check.py` & `langchain_upstage-0.1.3/langchain_upstage/tools/groundedness_check.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import os
-from typing import Any, Literal, Optional, Type, Union
+from typing import Any, List, Literal, Optional, Type, Union
 
+from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManagerForToolRun,
     CallbackManagerForToolRun,
 )
+from langchain_core.documents import Document
 from langchain_core.messages import AIMessage, HumanMessage
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr
 from langchain_core.tools import BaseTool
 from langchain_core.utils import convert_to_secret_str
 
 from langchain_upstage import ChatUpstage
 
 
-class GroundednessCheckInput(BaseModel):
+class UpstageGroundednessCheckInput(BaseModel):
     """Input for the Groundedness Check tool."""
 
-    context: str = Field(description="context in which the answer should be verified")
-    query: str = Field(
+    context: Union[str, List[Document]] = Field(
+        description="context in which the answer should be verified"
+    )
+    answer: str = Field(
         description="assistant's reply or a text that is subject to groundedness check"
     )
 
 
-class GroundednessCheck(BaseTool):
+class UpstageGroundednessCheck(BaseTool):
     """Tool that checks the groundedness of a context and an assistant message.
 
     To use, you should have the environment variable `UPSTAGE_API_KEY`
     set with your API key or pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
 
-                from langchain_upstage import GroundednessCheck
+                from langchain_upstage import UpstageGroundednessCheck
 
-                tool = GroundednessCheck()
+                tool = UpstageGroundednessCheck()
     """
 
     name: str = "groundedness_check"
     description: str = (
         "A tool that checks the groundedness of an assistant response "
-        "to user-provided context. GroundednessCheck ensures that "
+        "to user-provided context. UpstageGroundednessCheck ensures that "
         "the assistant’s response is not only relevant but also "
         "precisely aligned with the user's initial context, "
         "promoting a more reliable and context-aware interaction. "
         "When using retrieval-augmented generation (RAG), "
         "the Groundedness Check can be used to determine whether "
         "the assistant's message is grounded in the provided context."
     )
     upstage_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     api_wrapper: ChatUpstage
 
-    args_schema: Type[BaseModel] = GroundednessCheckInput
+    args_schema: Type[BaseModel] = UpstageGroundednessCheckInput
 
     def __init__(self, **kwargs: Any) -> None:
         upstage_api_key = kwargs.get("upstage_api_key", None)
         if not upstage_api_key:
             upstage_api_key = kwargs.get("api_key", None)
         if not upstage_api_key:
             upstage_api_key = SecretStr(os.getenv("UPSTAGE_API_KEY", ""))
@@ -69,29 +73,45 @@
 
         api_wrapper = ChatUpstage(
             model_name="solar-1-mini-answer-verification",
             upstage_api_key=upstage_api_key.get_secret_value(),
         )
         super().__init__(upstage_api_key=upstage_api_key, api_wrapper=api_wrapper)
 
+    def formatDocumentsAsString(self, docs: List[Document]) -> str:
+        return "\n".join([doc.page_content for doc in docs])
+
     def _run(
         self,
-        context: str,
-        query: str,
+        context: Union[str, List[Document]],
+        answer: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> Union[str, Literal["grounded", "notGrounded", "notSure"]]:
         """Use the tool."""
+        if isinstance(context, List):
+            context = self.formatDocumentsAsString(context)
         response = self.api_wrapper.invoke(
-            [HumanMessage(context), AIMessage(query)], stream=False
+            [HumanMessage(context), AIMessage(answer)], stream=False
         )
         return str(response.content)
 
     async def _arun(
         self,
-        context: str,
-        query: str,
+        context: Union[str, List[Document]],
+        answer: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> Union[str, Literal["grounded", "notGrounded", "notSure"]]:
+        if isinstance(context, List):
+            context = self.formatDocumentsAsString(context)
         response = await self.api_wrapper.ainvoke(
-            [HumanMessage(context), AIMessage(query)], stream=False
+            [HumanMessage(context), AIMessage(answer)], stream=False
         )
         return str(response.content)
+
+
+@deprecated(
+    since="0.1.3",
+    removal="0.2.0",
+    alternative_import="langchain_upstage.UpstageGroundednessCheck",
+)
+class GroundednessCheck(UpstageGroundednessCheck):
+    pass
```

### Comparing `langchain_upstage-0.1.2/pyproject.toml` & `langchain_upstage-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-upstage"
-version = "0.1.2"
+version = "0.1.3"
 description = "An integration package connecting Upstage and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_upstage-0.1.2/PKG-INFO` & `langchain_upstage-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integration package connecting Upstage and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

