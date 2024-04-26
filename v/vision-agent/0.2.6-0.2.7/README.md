# Comparing `tmp/vision_agent-0.2.6.tar.gz` & `tmp/vision_agent-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.6.tar", max compression
+gzip compressed data, was "vision_agent-0.2.7.tar", max compression
```

## Comparing `vision_agent-0.2.6.tar` & `vision_agent-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-25 06:01:28.383648 vision_agent-0.2.6/LICENSE
--rw-r--r--   0        0        0     6639 2024-04-25 06:01:28.383648 vision_agent-0.2.6/README.md
--rw-r--r--   0        0        0     2099 2024-04-25 06:01:28.939650 vision_agent-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    25971 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7552 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5383 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10539 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      413 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    43013 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/type_defs.py
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 17:35:32.460863 vision_agent-0.2.7/LICENSE
+-rw-r--r--   0        0        0     6639 2024-04-25 17:35:32.460863 vision_agent-0.2.7/README.md
+-rw-r--r--   0        0        0     2099 2024-04-25 17:35:33.044866 vision_agent-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    26024 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:35:32.472863 vision_agent-0.2.7/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7552 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5383 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10539 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      413 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    43013 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-25 17:35:32.484863 vision_agent-0.2.7/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.7/PKG-INFO
```

### Comparing `vision_agent-0.2.6/LICENSE` & `vision_agent-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/README.md` & `vision_agent-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/pyproject.toml` & `vision_agent-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.6"
+version = "0.2.7"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.6/vision_agent/agent/agent.py` & `vision_agent-0.2.7/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/agent/easytool.py` & `vision_agent-0.2.7/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.7/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/agent/reflexion.py` & `vision_agent-0.2.7/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.7/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.7/vision_agent/agent/vision_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,15 +517,17 @@
         self, images: Sequence[Union[str, Path]]
     ) -> None:
         """This is intended for streaming the visualization images via the callback to the client side."""
         if self.report_progress_callback:
             self.report_progress_callback("<VIZ>")
             if images:
                 for img in images:
-                    self.report_progress_callback(f"<IMG>{convert_to_b64(img)}</IMG>")
+                    self.report_progress_callback(
+                        f"<IMG>base:64{convert_to_b64(img)}</IMG>"
+                    )
             self.report_progress_callback("</VIZ>")
 
     def chat_with_workflow(
         self,
         chat: List[Dict[str, str]],
         image: Optional[Union[str, Path]] = None,
         reference_data: Optional[Dict[str, str]] = None,
```

### Comparing `vision_agent-0.2.6/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.7/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.7/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/image_utils.py` & `vision_agent-0.2.7/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/llm/llm.py` & `vision_agent-0.2.7/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/lmm/lmm.py` & `vision_agent-0.2.7/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/tools/prompts.py` & `vision_agent-0.2.7/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/tools/tools.py` & `vision_agent-0.2.7/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/tools/video.py` & `vision_agent-0.2.7/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/vision_agent/type_defs.py` & `vision_agent-0.2.7/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.6/PKG-INFO` & `vision_agent-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.6
+Version: 0.2.7
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

