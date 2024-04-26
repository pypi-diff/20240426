# Comparing `tmp/streamlit_chat_handler-0.0.3.tar.gz` & `tmp/streamlit_chat_handler-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.0.3.tar", last modified: Thu Apr 25 02:28:49 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.0.4.tar", last modified: Thu Apr 25 04:47:06 2024, max compression
```

## Comparing `streamlit_chat_handler-0.0.3.tar` & `streamlit_chat_handler-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.0.3/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3710 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.0.3/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-23 03:41:26.000000 streamlit_chat_handler-0.0.3/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-25 02:27:43.000000 streamlit_chat_handler-0.0.3/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      356 2024-04-23 01:52:45.000000 streamlit_chat_handler-0.0.3/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7434 2024-04-25 02:27:16.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-23 03:47:04.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3710 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      272 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 04:47:06.074305 streamlit_chat_handler-0.0.4/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.0.4/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-25 04:47:06.074305 streamlit_chat_handler-0.0.4/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.0.4/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 04:47:06.070305 streamlit_chat_handler-0.0.4/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-23 03:41:26.000000 streamlit_chat_handler-0.0.4/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-25 04:46:15.000000 streamlit_chat_handler-0.0.4/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.0.4/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-25 04:47:06.074305 streamlit_chat_handler-0.0.4/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 04:47:06.070305 streamlit_chat_handler-0.0.4/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7661 2024-04-25 04:45:55.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-23 03:47:04.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 04:47:06.074305 streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-25 04:47:06.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-25 04:47:06.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-25 04:47:06.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-25 04:47:06.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-25 04:47:06.000000 streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.0.3/LICENSE` & `streamlit_chat_handler-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.3/PKG-INFO` & `streamlit_chat_handler-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.0.3
+Version: 0.0.4
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
 Requires-Dist: streamlit-chat==0.1.1
 Requires-Dist: streamlit-extras==0.4.2
 Requires-Dist: streamlit-feedback==0.1.3
 Requires-Dist: pydantic==2.7.0
+Requires-Dist: loguru
 Provides-Extra: lint
 Requires-Dist: black==23.7.0; extra == "lint"
 Requires-Dist: flake8==6.1.0; extra == "lint"
 Requires-Dist: Flake8-pyproject==1.2.3; extra == "lint"
 Requires-Dist: mypy==1.4.1; extra == "lint"
 Requires-Dist: bandit==1.7.5; extra == "lint"
 Provides-Extra: test
```

### Comparing `streamlit_chat_handler-0.0.3/README.md` & `streamlit_chat_handler-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.3/examples/template.py` & `streamlit_chat_handler-0.0.4/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.3/pyproject.toml` & `streamlit_chat_handler-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.0.3"
+version = "0.0.4"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.0.3/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.0.4/streamlit_chat_handler/_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import uuid
 from typing import Any, Literal, Tuple
 from collections import OrderedDict
 
 import streamlit as st
+from loguru import logger
 from streamlit.runtime.state.session_state_proxy import SessionStateProxy
 
 from streamlit_chat_handler.types import StreamlitChatElement
 
 
 class StreamlitChatHandler:
     """Handles the state and rendering of chat elements within a Streamlit session.
@@ -138,17 +139,20 @@
 
         response = OrderedDict({})
         count = 0
         for element_list in element_groups:
             role = element_list[0].role
             with st.chat_message(role):
                 for element in element_list:
-                    response[list(chat_element)[count]] = getattr(st, element.type)(
-                        element.content, *element.args, **element.kwargs
-                    )
+                    try:
+                        response[list(chat_element)[count]] = getattr(st, element.type)(
+                            element.content, *element.args, **element.kwargs
+                        )
+                    except Exception as err:
+                        logger.warning(f"Error rendering element {element} in key {list(chat_element)[count]}: {err}")
                     count += 1
         return response
 
 
 def _get_last_item(ordered_dict: OrderedDict) -> Tuple[str, Any]:
     """Retrieve the last key-value pair from an OrderedDict.
```

### Comparing `streamlit_chat_handler-0.0.3/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.0.4/streamlit_chat_handler/types.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.0.4/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.0.3
+Version: 0.0.4
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
 Requires-Dist: streamlit-chat==0.1.1
 Requires-Dist: streamlit-extras==0.4.2
 Requires-Dist: streamlit-feedback==0.1.3
 Requires-Dist: pydantic==2.7.0
+Requires-Dist: loguru
 Provides-Extra: lint
 Requires-Dist: black==23.7.0; extra == "lint"
 Requires-Dist: flake8==6.1.0; extra == "lint"
 Requires-Dist: Flake8-pyproject==1.2.3; extra == "lint"
 Requires-Dist: mypy==1.4.1; extra == "lint"
 Requires-Dist: bandit==1.7.5; extra == "lint"
 Provides-Extra: test
```

