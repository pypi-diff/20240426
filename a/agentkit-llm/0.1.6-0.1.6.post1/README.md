# Comparing `tmp/agentkit-llm-0.1.6.tar.gz` & `tmp/agentkit-llm-0.1.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.6.tar", last modified: Wed Apr 24 17:53:06 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.6.post1.tar", last modified: Fri Apr 26 20:04:13 2024, max compression
```

## Comparing `agentkit-llm-0.1.6.tar` & `agentkit-llm-0.1.6.post1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.6/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8390 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     7906 2024-04-24 17:52:07.000000 agentkit-llm-0.1.6/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      995 2024-04-24 17:35:02.000000 agentkit-llm-0.1.6/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.156235 agentkit-llm-0.1.6/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.156235 agentkit-llm-0.1.6/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.6/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.6/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.6/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.6/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.6/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.6/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.156235 agentkit-llm-0.1.6/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5142 2024-04-24 17:42:15.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3992 2024-04-24 17:36:07.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.6/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.6/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.6/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/
--rw-r--r--   0 holmes    (1000) holmes    (1000)     8390 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.6.post1/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8525 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8035 2024-04-26 20:02:45.000000 agentkit-llm-0.1.6.post1/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1001 2024-04-26 20:03:26.000000 agentkit-llm-0.1.6.post1/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.390998 agentkit-llm-0.1.6.post1/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.6.post1/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.6.post1/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.6.post1/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.6.post1/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.6.post1/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.6.post1/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     5142 2024-04-24 17:42:15.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3992 2024-04-24 17:36:07.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.6.post1/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.6.post1/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.6.post1/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/
+-rw-r--r--   0 holmes    (1000) holmes    (1000)     8525 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.6/LICENSE` & `agentkit-llm-0.1.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/PKG-INFO` & `agentkit-llm-0.1.6.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.6
+Version: 0.1.6.post1
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -86,26 +86,28 @@
 import agentkit
 from agentkit import Graph, BaseNode
 
 import agentkit.llm_api
 
 LLM_API_FUNCTION = agentkit.llm_api.get_query("gpt-4-turbo")
 
+LLM_API_FUNCTION.debug = True # Disable this to enable API-level error handling-retry
+
 graph = Graph()
 
 subtask1 = "What are the pros and cons for using LLM Agents for Game AI?" 
-node1 = BaseNode(subtask1, subtask1, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node1 = BaseNode(subtask1, subtask1, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node1)
 
 subtask2 = "Give me an outline for an essay titled 'LLM Agents for Games'." 
-node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node2)
 
 subtask3 = "Now, write a full essay on the topic 'LLM Agents for Games'."
-node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node3)
 
 # add dependencies between nodes
 graph.add_edge(subtask1, subtask2)
 graph.add_edge(subtask1, subtask3)
 graph.add_edge(subtask2, subtask3)
```

### Comparing `agentkit-llm-0.1.6/README.md` & `agentkit-llm-0.1.6.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,26 +71,28 @@
 import agentkit
 from agentkit import Graph, BaseNode
 
 import agentkit.llm_api
 
 LLM_API_FUNCTION = agentkit.llm_api.get_query("gpt-4-turbo")
 
+LLM_API_FUNCTION.debug = True # Disable this to enable API-level error handling-retry
+
 graph = Graph()
 
 subtask1 = "What are the pros and cons for using LLM Agents for Game AI?" 
-node1 = BaseNode(subtask1, subtask1, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node1 = BaseNode(subtask1, subtask1, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node1)
 
 subtask2 = "Give me an outline for an essay titled 'LLM Agents for Games'." 
-node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node2)
 
 subtask3 = "Now, write a full essay on the topic 'LLM Agents for Games'."
-node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node3)
 
 # add dependencies between nodes
 graph.add_edge(subtask1, subtask2)
 graph.add_edge(subtask1, subtask3)
 graph.add_edge(subtask2, subtask3)
```

### Comparing `agentkit-llm-0.1.6/setup.py` & `agentkit-llm-0.1.6.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.6"
+VERSION = "0.1.6.post1"
 EXTRAS = {
     "logging": ["wandb"],
     "all": ["wandb", "openai", "anthropic", "tiktoken"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
```

### Comparing `agentkit-llm-0.1.6/src/agentkit/after_query.py` & `agentkit-llm-0.1.6.post1/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/base_node.py` & `agentkit-llm-0.1.6.post1/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.6.post1/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/exceptions.py` & `agentkit-llm-0.1.6.post1/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/graph.py` & `agentkit-llm-0.1.6.post1/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/GPT.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/node.py` & `agentkit-llm-0.1.6.post1/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit/utils.py` & `agentkit-llm-0.1.6.post1/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.6
+Version: 0.1.6.post1
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -86,26 +86,28 @@
 import agentkit
 from agentkit import Graph, BaseNode
 
 import agentkit.llm_api
 
 LLM_API_FUNCTION = agentkit.llm_api.get_query("gpt-4-turbo")
 
+LLM_API_FUNCTION.debug = True # Disable this to enable API-level error handling-retry
+
 graph = Graph()
 
 subtask1 = "What are the pros and cons for using LLM Agents for Game AI?" 
-node1 = BaseNode(subtask1, subtask1, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node1 = BaseNode(subtask1, subtask1, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node1)
 
 subtask2 = "Give me an outline for an essay titled 'LLM Agents for Games'." 
-node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node2 = BaseNode(subtask2, subtask2, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node2)
 
 subtask3 = "Now, write a full essay on the topic 'LLM Agents for Games'."
-node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt())
+node3 = BaseNode(subtask3, subtask3, graph, LLM_API_FUNCTION, agentkit.compose_prompt.BaseComposePrompt(), verbose=True)
 graph.add_node(node3)
 
 # add dependencies between nodes
 graph.add_edge(subtask1, subtask2)
 graph.add_edge(subtask1, subtask3)
 graph.add_edge(subtask2, subtask3)
```

### Comparing `agentkit-llm-0.1.6/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

