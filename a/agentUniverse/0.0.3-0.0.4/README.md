# Comparing `tmp/agentUniverse-0.0.3.tar.gz` & `tmp/agentUniverse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentUniverse-0.0.3.tar", last modified: Fri Apr 19 04:59:49 2024, max compression
+gzip compressed data, was "agentUniverse-0.0.4.tar", last modified: Fri Apr 26 09:36:05 2024, max compression
```

## Comparing `agentUniverse-0.0.3.tar` & `agentUniverse-0.0.4.tar`

### file list

```diff
@@ -1,261 +1,334 @@
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.171234 agentUniverse-0.0.3/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/LICENSE
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-19 04:59:49.170901 agentUniverse-0.0.3/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2560 2024-04-19 04:56:45.000000 agentUniverse-0.0.3/README.md
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.170492 agentUniverse-0.0.3/agentUniverse.egg-info/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9829 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/SOURCES.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/dependency_links.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/requires.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       68 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/top_level.txt
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.134226 agentUniverse-0.0.3/agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.3/agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.135182 agentUniverse-0.0.3/agentuniverse/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.135327 agentUniverse-0.0.3/agentuniverse/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.135960 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.136408 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      957 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4458 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.136699 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.137573 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1636 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1463 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/reader.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.138293 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4644 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1967 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/store.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.138853 agentUniverse-0.0.3/agentuniverse/agent/action/tool/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3853 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/agent_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/agent_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.140398 agentUniverse-0.0.3/agentuniverse/agent/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/executing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/executing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/expressing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/expressing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/planning_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      352 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/planning_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      266 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/rag_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/reviewing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      357 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/reviewing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/input_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.142170 agentUniverse-0.0.3/agentuniverse/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3675 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/chat_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7755 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3042 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/message.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1759 2024-04-09 06:57:56.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/output_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.142319 agentUniverse-0.0.3/agentuniverse/agent/plan/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.142782 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.143400 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3103 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1287 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.143999 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3040 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1493 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.144444 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7621 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6441 2024-04-19 04:58:00.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.145155 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2987 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1178 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.146445 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      675 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2784 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.147159 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1212 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3041 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.148112 agentUniverse-0.0.3/agentuniverse/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.149090 agentUniverse-0.0.3/agentuniverse/agent_serve/web/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.149466 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.149833 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5231 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9326 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/request_task.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2573 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5064 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2434 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.150132 agentUniverse-0.0.3/agentuniverse/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9442 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/base/agentuniverse.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.150426 agentUniverse-0.0.3/agentuniverse/base/annotation/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/annotation/singleton.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.151489 agentUniverse-0.0.3/agentuniverse/base/component/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/component/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_base.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4129 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      604 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_manager_base.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.152327 agentUniverse-0.0.3/agentuniverse/base/config/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.152859 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3885 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/application_config_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.153219 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2557 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/component_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.154305 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4828 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.154607 agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/custom_key_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.155433 agentUniverse-0.0.3/agentuniverse/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/context/framework_context.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/context/framework_context_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.156355 agentUniverse-0.0.3/agentuniverse/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/env_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.156988 agentUniverse-0.0.3/agentuniverse/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/base/util/memory_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6379 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/system_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.158045 agentUniverse-0.0.3/agentuniverse/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/llm/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.158645 agentUniverse-0.0.3/agentuniverse/llm/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/llm/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1422 2024-04-19 04:40:08.000000 agentUniverse-0.0.3/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2907 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4946 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/llm/llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/llm/llm_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      328 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/llm/llm_output.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4512 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/llm/openai_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.159214 agentUniverse-0.0.3/agentuniverse/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1931 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/prompt/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/prompt/prompt_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.159435 agentUniverse-0.0.3/agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.3/agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.159625 agentUniverse-0.0.3/agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.3/agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160141 agentUniverse-0.0.3/agentuniverse_extension/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2074 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/pyproject.toml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-19 04:59:49.171290 agentUniverse-0.0.3/setup.cfg
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1176 2024-04-19 04:56:45.000000 agentUniverse-0.0.3/setup.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160542 agentUniverse-0.0.3/tests/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.3/tests/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160724 agentUniverse-0.0.3/tests/test_agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160885 agentUniverse-0.0.3/tests/test_agentuniverse/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.162360 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.162595 agentUniverse-0.0.3/tests/test_agentuniverse/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.163017 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.163229 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.163877 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.164274 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.164720 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/test_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      786 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/test_agent.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.166178 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.166373 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.166890 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/test_framework_context.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.167095 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.167609 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168168 agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/test_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168361 agentUniverse-0.0.3/tests/test_agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168522 agentUniverse-0.0.3/tests/test_agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168868 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.169577 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.169812 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.170222 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.006355 agentUniverse-0.0.4/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/LICENSE
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-26 09:36:05.006088 agentUniverse-0.0.4/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2713 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/README.md
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.005705 agentUniverse-0.0.4/agentUniverse.egg-info/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    12853 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/requires.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       88 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/top_level.txt
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.946788 agentUniverse-0.0.4/agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.4/agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.949625 agentUniverse-0.0.4/agentuniverse/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.949900 agentUniverse-0.0.4/agentuniverse/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.950793 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.951580 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      972 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4473 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.952004 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.953455 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1651 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1478 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/reader.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.954383 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4674 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1997 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/store.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.955193 agentUniverse-0.0.4/agentuniverse/agent/action/tool/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3868 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-26 03:44:06.000000 agentUniverse-0.0.4/agentuniverse/agent/agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-26 03:44:12.000000 agentUniverse-0.0.4/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/agent_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.957938 agentUniverse-0.0.4/agentuniverse/agent/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/executing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      369 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/executing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/expressing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      366 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/expressing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/planning_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      356 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/planning_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/rag_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      284 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/rag_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/reviewing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      361 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/reviewing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/input_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.960279 agentUniverse-0.0.4/agentuniverse/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3907 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/chat_memory.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.960873 agentUniverse-0.0.4/agentuniverse/agent/memory/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      845 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/default/default_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      321 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/default/default_memory.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7689 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3054 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/message.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      754 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/summarizer_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/output_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.961045 agentUniverse-0.0.4/agentuniverse/agent/plan/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.961798 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.962818 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1227 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1421 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3393 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.963840 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1471 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1841 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3330 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.964713 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     8675 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6396 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.965905 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1315 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1586 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3276 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.966898 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      741 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      859 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3074 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.967825 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1194 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1387 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3331 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.968896 agentUniverse-0.0.4/agentuniverse/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.970768 agentUniverse-0.0.4/agentuniverse/agent_serve/web/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.971202 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.971690 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5473 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5327 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/flask_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2351 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/gunicorn_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9311 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/request_task.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.972159 agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1224 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/rpc_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      822 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2679 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.972573 agentUniverse-0.0.4/agentuniverse/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    10614 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/base/agentuniverse.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.973044 agentUniverse-0.0.4/agentuniverse/base/annotation/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/annotation/singleton.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.974530 agentUniverse-0.0.4/agentuniverse/base/component/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/component/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_base.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4380 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_manager_base.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.975498 agentUniverse-0.0.4/agentuniverse/base/config/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.976476 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4173 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/application_config_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.977774 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2811 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/component_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.980164 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1889 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/prompt_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4846 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/base/config/configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.980684 agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-26 03:55:12.000000 agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/custom_key_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.981491 agentUniverse-0.0.4/agentuniverse/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/context/framework_context_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.982816 agentUniverse-0.0.4/agentuniverse/base/prompt/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      286 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/combine_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      318 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/combine_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      253 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/summary_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      272 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/summary_en_prompt.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.984168 agentUniverse-0.0.4/agentuniverse/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/env_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.985307 agentUniverse-0.0.4/agentuniverse/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-26 03:42:29.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-26 03:42:21.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-26 03:42:41.000000 agentUniverse-0.0.4/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6644 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/system_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.986802 agentUniverse-0.0.4/agentuniverse/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/llm/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.987443 agentUniverse-0.0.4/agentuniverse/llm/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1352 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2892 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5508 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      408 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/llm_output.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6482 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/openai_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.988521 agentUniverse-0.0.4/agentuniverse/prompt/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/prompt/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      548 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/prompt/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3105 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/prompt/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      741 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/prompt/prompt_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/prompt/prompt_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.988691 agentUniverse-0.0.4/agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.4/agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.988967 agentUniverse-0.0.4/agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.4/agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.989401 agentUniverse-0.0.4/agentuniverse_extension/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2162 2024-04-26 09:31:08.000000 agentUniverse-0.0.4/pyproject.toml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.989590 agentUniverse-0.0.4/sample_standard_app/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.989863 agentUniverse-0.0.4/sample_standard_app/app/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990118 agentUniverse-0.0.4/sample_standard_app/app/biz/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/biz/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990521 agentUniverse-0.0.4/sample_standard_app/app/bootstrap/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/bootstrap/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/bootstrap/server_application.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990718 agentUniverse-0.0.4/sample_standard_app/app/core/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990900 agentUniverse-0.0.4/sample_standard_app/app/core/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.992327 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1360 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_executing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1562 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_expressing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      793 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_peer_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      430 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_peer_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      485 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_planning_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      325 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_reviewing_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.992956 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      725 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/demo_rag_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      341 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/demo_rag_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.993501 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2474 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/demo_knowledge.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/demo_knowledge.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.993856 agentUniverse-0.0.4/sample_standard_app/app/core/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/llm/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      212 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/llm/demo_llm.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.994032 agentUniverse-0.0.4/sample_standard_app/app/core/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/memory/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.994221 agentUniverse-0.0.4/sample_standard_app/app/core/planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/planner/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.994573 agentUniverse-0.0.4/sample_standard_app/app/core/service/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/service/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      114 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/service/demo_service.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.995177 agentUniverse-0.0.4/sample_standard_app/app/core/tool/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/tool/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      857 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/tool/demo_tool.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      182 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/tool/demo_tool.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.995909 agentUniverse-0.0.4/sample_standard_app/app/test/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    15065 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/test_peer_agents.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      943 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/test_rag_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      325 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/test_server_application.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996092 agentUniverse-0.0.4/sample_standard_app/app/web/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/web/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-26 09:36:05.006405 agentUniverse-0.0.4/setup.cfg
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1176 2024-04-26 09:31:08.000000 agentUniverse-0.0.4/setup.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996261 agentUniverse-0.0.4/tests/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.4/tests/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996608 agentUniverse-0.0.4/tests/test_agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996913 agentUniverse-0.0.4/tests/test_agentuniverse/mock/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.998167 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.998375 agentUniverse-0.0.4/tests/test_agentuniverse/unit/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.998849 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.999108 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.999502 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.999991 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.000460 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/test_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      820 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/test_rag_agent.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.002005 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      390 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.002240 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.002761 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/test_framework_context.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.003039 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.003387 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.003833 agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/test_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004091 agentUniverse-0.0.4/tests/test_agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004257 agentUniverse-0.0.4/tests/test_agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004419 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004819 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004992 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.005379 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-19 04:49:33.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
```

### Comparing `agentUniverse-0.0.3/LICENSE` & `agentUniverse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/PKG-INFO` & `agentUniverse-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.3
+Version: 0.0.4
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
 Home-page: https://gitee.com/agentUniverse/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `agentUniverse-0.0.3/README.md` & `agentUniverse-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 ****************************************
 Language version: [English](./README.md) | [中文](./README_zh.md)
 
 ![](https://img.shields.io/badge/framework-agentUniverse-pink)
 ![](https://img.shields.io/badge/python-3.10%2B-blue?logo=Python)
 [![](https://img.shields.io/badge/%20license-Apache--2.0-yellow)](LICENSE)
 [![Static Badge](https://img.shields.io/badge/pypi-v0.0.3-blue?logo=pypi)](https://pypi.org/project/agentUniverse/)
+
+![](docs/guidebook/_picture/logo_bar.jpg)
 ****************************************
 
 ## Overview
 agentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
 The framework will come with serveral pre-install multi-agent collaboration patterns which have been proven effective in real business scenarios, and will continue to be enriched in the future. Patterns that are currently about to be released include:
 
@@ -18,27 +20,29 @@
 
 
 - DOE pattern：
 This pattern consists of three agents: Data-fining agent, which is designed to solve data-intensive and high-computational-precision task; Opinion-inject agent, which combines the data results from first agent and the expert opinions which are pre-collected and structured; the third agent, Express agent generates the final result base on given document type and language style.
 
 More patterns are coming soon...
 
+![](docs/guidebook/_picture/agent_universe_framework_resize.jpg)
+
 ## agentUniverseSample Project
-[agentUniverse Sample Project pending...](pending...)
+[agentUniverse Sample Project](sample_standard_app/README.md)
 
 ## Quick Installation
 Using pip:
 ```shell
-pending...
+pip install agentUniverse
 ```
 
 ## Quick Start
 We will show you how to:
 * Prepare the environment and application project
 * Build a simple agent
 * Use pattern components to complete multi-agent collaboration
 * Test and optimize the performance of the agent
 * Quickly serve the agent
-For details, please read [Quick Start pending...](pending...).
+For details, please read [Quick Start](docs/guidebook/en/1_3_Quick_Start.md).
 
 ## Guidebook
-For more detailed information, please refer to the [Guidebook  pending...]( pending...).
+For more detailed information, please refer to the [Guidebook](docs/guidebook/en/0_index.md).
```

### Comparing `agentUniverse-0.0.3/agentUniverse.egg-info/PKG-INFO` & `agentUniverse-0.0.4/agentUniverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.3
+Version: 0.0.4
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
 Home-page: https://gitee.com/agentUniverse/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         """Get embeddings."""
 
     @abstractmethod
     async def async_get_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Asynchronously get embeddings."""
 
     def as_langchain(self) -> LCEmbeddings:
-        """Convert the aU embedding class to the langchain embedding class."""
+        """Convert the AgentUniverse(AU) embedding class to the langchain embedding class."""
         pass
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,10 +95,10 @@
 
             # Return the embeddings as a list of lists of floats
             return [embedding.embedding for embedding in data]
         except BadRequestError as e:
             raise ValueError(e.message)
 
     def as_langchain(self) -> OpenAIEmbeddings:
-        """Convert the aU openai embedding class to the langchain openai embedding class."""
+        """Convert the AgentUniverse(AU) openai embedding class to the langchain openai embedding class."""
         return OpenAIEmbeddings(openai_api_key=self.openai_api_key,
                                 client=self.client.embeddings, async_client=self.async_client.embeddings)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ".pdf": PdfReader,
     ".docx": DocxReader,
     ".pptx": PptxReader,
 }
 
 
 class FileReader(Reader):
-    """The aU file reader class.
+    """The AgentUniverse(AU) file reader class.
 
     FileReader is used to load data from files based on the provided file paths.
 
     Attributes:
         file_readers (Dict[str, Type[Reader]], optional): The file reader dictionary,
         the key is the suffix of the file, and the value is the specific file reader class.
     """
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import requests
 
 from agentuniverse.agent.action.knowledge.reader.reader import Reader
 from agentuniverse.agent.action.knowledge.store.document import Document
 
 
 class WebPdfReader(Reader):
-    """The aU web pdf reader.
+    """The AgentUniverse(AU) web pdf reader.
 
     The pdf file will be downloaded and then parsed by `pdfminer.six`.
     """
 
     def load_data(self, web_pdf_url: str) -> List[Document]:
         if web_pdf_url is None:
             return []
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 query_embeddings=[embedding]
             )
         else:
             query_result = self.collection.query(
                 n_results=query.similarity_top_k,
                 query_texts=[query.query_str]
             )
-        # convert to the aU document format
+        # convert to the AgentUniverse(AU) document format
         return self.to_documents(query_result)
 
     def insert_documents(self, documents: List[Document], **kwargs: Any):
         """Insert documents to the chroma collection.
 
         Args:
             documents (List[Document]): The documents to be inserted.
@@ -97,15 +97,15 @@
                 metadatas=[document.metadata],
                 embeddings=[embedding] if embedding is not None else None,
                 ids=[document.id]
             )
 
     @staticmethod
     def to_documents(query_result: QueryResult) -> List[Document]:
-        """Convert the query results of ChromaDB to the aU document format."""
+        """Convert the query results of ChromaDB to the AgentUniverse(AU) document format."""
 
         if query_result is None:
             return []
         documents = []
         for i in range(len(query_result['ids'][0])):
             documents.append(Document(id=query_result['ids'][0][i],
                                       text=query_result['documents'][0][i],
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/document.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     def as_langchain(self) -> LCDocument:
         """Convert to LangChain document format."""
         metadata = self.metadata or {}
         return LCDocument(page_content=self.text, metadata=metadata)
 
     @staticmethod
     def as_langchain_list(document_list) -> List[LCDocument]:
-        """Convert aU document list to langchain document list """
+        """Convert AgentUniverse(AU) document list to langchain document list """
         langchain_document_list = []
         if document_list is None:
             return langchain_document_list
         for document in document_list:
             langchain_document_list.append(LCDocument(page_content=document.text, metadata=document.metadata))
         return langchain_document_list
 
     @staticmethod
     def from_langchain_list(lc_document_list: List[LCDocument]):
-        """Convert langchain document list to aU document list """
+        """Convert langchain document list to AgentUniverse(AU) document list """
         document_list = []
         if lc_document_list is None:
             return document_list
         for lc_document in lc_document_list:
             document_list.append(Document(text=lc_document.page_content, metadata=lc_document.metadata))
         return document_list
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/query.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/store.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 raise Exception(f'{self.get_instance_code()} - The input must include key: {key}.')
 
     @abstractmethod
     def execute(self, tool_input: ToolInput):
         raise NotImplementedError
 
     def as_langchain(self) -> LangchainTool:
-        """Convert the aU tool class to the langchain tool class."""
+        """Convert the AgentUniverse(AU) tool class to the langchain tool class."""
         return LangchainTool(name=self.name,
                              func=self.run,
                              description=self.description)
 
     def get_instance_code(self) -> str:
         """Return the full name of the tool."""
         appname = ApplicationConfigManager().app_configer.base_info_appname
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool_manager.py` & `agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/agent.py` & `agentUniverse-0.0.4/agentuniverse/agent/agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/agent_manager.py` & `agentUniverse-0.0.4/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/agent_model.py` & `agentUniverse-0.0.4/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/default/executing_agent.py` & `agentUniverse-0.0.4/agentuniverse/agent/default/executing_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/default/expressing_agent.py` & `agentUniverse-0.0.4/agentuniverse/agent/default/expressing_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/default/planning_agent.py` & `agentUniverse-0.0.4/agentuniverse/agent/default/planning_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/default/rag_agent.py` & `agentUniverse-0.0.4/agentuniverse/agent/default/rag_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/default/reviewing_agent.py` & `agentUniverse-0.0.4/agentuniverse/agent/default/reviewing_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/input_object.py` & `agentUniverse-0.0.4/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/memory/chat_memory.py` & `agentUniverse-0.0.4/agentuniverse/agent/memory/chat_memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Optional, List
 
 from langchain.memory.chat_memory import BaseChatMemory
 
 from agentuniverse.agent.memory.enum import MemoryTypeEnum
 from agentuniverse.agent.memory.memory import Memory
 from agentuniverse.agent.memory.message import Message
-from agentuniverse.agent.memory.langchain_instance import FinCoConversationSummaryBufferMemory, \
-    FinCoConversationTokenBufferMemory
+from agentuniverse.agent.memory.langchain_instance import AuConversationSummaryBufferMemory, \
+    AuConversationTokenBufferMemory
 from agentuniverse.base.config.component_configer.configers.memory_configer import MemoryConfiger
 from agentuniverse.llm.llm import LLM
 
 
 class ChatMemory(Memory):
     """The basic class for chat memory model.
 
@@ -30,27 +30,29 @@
         messages (Optional[List[Message]]): The list of conversation messages to send to the LLM memory.
     """
 
     llm: Optional[LLM] = None
     input_key: Optional[str] = None
     output_key: Optional[str] = None
     messages: Optional[List[Message]] = None
+    prompt_version: Optional[str] = None
 
     def as_langchain(self) -> BaseChatMemory:
-        """Convert the finCo chat memory class to the langchain chat memory class."""
+        """Convert the AgentUniverse(AU) chat memory class to the langchain chat memory class."""
         if self.llm is None:
             raise ValueError("Must set `llm` when using langchain memory.")
         if self.type is None or self.type == MemoryTypeEnum.SHORT_TERM:
-            return FinCoConversationTokenBufferMemory(llm=self.llm.as_langchain(), memory_key=self.memory_key,
-                                                      input_key=self.input_key, output_key=self.output_key,
-                                                      max_token_limit=self.max_tokens, messages=self.messages)
+            return AuConversationTokenBufferMemory(llm=self.llm.as_langchain(), memory_key=self.memory_key,
+                                                   input_key=self.input_key, output_key=self.output_key,
+                                                   max_token_limit=self.max_tokens, messages=self.messages)
         elif self.type == MemoryTypeEnum.LONG_TERM:
-            return FinCoConversationSummaryBufferMemory(llm=self.llm.as_langchain(), memory_key=self.memory_key,
-                                                        input_key=self.input_key, output_key=self.output_key,
-                                                        max_token_limit=self.max_tokens, messages=self.messages)
+            return AuConversationSummaryBufferMemory(llm=self.llm.as_langchain(), memory_key=self.memory_key,
+                                                     input_key=self.input_key, output_key=self.output_key,
+                                                     max_token_limit=self.max_tokens, messages=self.messages,
+                                                     prompt_version=self.prompt_version)
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the ChatMemory model in the agent configuration."""
         super().set_by_agent_model(**kwargs)
         if 'messages' in kwargs and kwargs['messages']:
             self.messages = kwargs['messages']
         if 'llm' in kwargs and kwargs['llm']:
@@ -68,8 +70,10 @@
             ChatMemory: the ChatMemory object
         """
         super().initialize_by_component_configer(component_configer)
         if component_configer.input_key:
             self.input_key = component_configer.input_key
         if component_configer.output_key:
             self.output_key = component_configer.output_key
+        if component_configer.prompt_version:
+            self.prompt_version = component_configer.prompt_version
         return self
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/memory/langchain_instance.py` & `agentUniverse-0.0.4/agentuniverse/agent/memory/langchain_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,57 +5,35 @@
 # @Author  : wangchongshi
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: langchain_instance.py
 from typing import List, Optional, Dict, Any
 
 from langchain.chains import LLMChain
 from langchain_core.messages import BaseMessage, get_buffer_string
-from langchain_core.prompts import BasePromptTemplate
 from langchain.memory import ConversationSummaryBufferMemory, ConversationTokenBufferMemory
 from langchain.memory.summary import SummarizerMixin
 
 from agentuniverse.agent.memory.enum import ChatMessageEnum
 from agentuniverse.agent.memory.message import Message
-from agentuniverse.agent.memory.prompt import SUMMARY_PROMPT
+from agentuniverse.prompt.prompt import Prompt
+from agentuniverse.prompt.prompt_manager import PromptManager
 
 
-class FinCoSummarizerMixin(SummarizerMixin):
-    """Mixin for the finCo memory summarizer.
-
-    Long term memory: summarize memories in multiple rounds of conversations.
-
-    Attributes:
-        prompt (BasePromptTemplate): The prompt to use when generating the summary.
-    """
-
-    prompt: BasePromptTemplate = SUMMARY_PROMPT
-
-    def predict_new_summary(
-            self, messages: List[BaseMessage], existing_summary: str
-    ) -> str:
-        """Predict new summary, summarize memories in multiple rounds of conversations."""
-        new_lines = get_buffer_string(
-            messages,
-            human_prefix=self.human_prefix,
-            ai_prefix=self.ai_prefix,
-        )
-        chain = LLMChain(llm=self.llm, prompt=self.prompt)
-        return chain.predict(summary=existing_summary, new_lines=new_lines)
-
-
-class FinCoConversationSummaryBufferMemory(ConversationSummaryBufferMemory, FinCoSummarizerMixin):
+class AuConversationSummaryBufferMemory(ConversationSummaryBufferMemory, SummarizerMixin):
     """Long term memory to store conversation memory.
 
-    If memories exceeds the max tokens limit, memories are compressed by the FinCoSummarizer.
+    If memories exceeds the max tokens limit,
+    memories will be compressed by the AuConversationSummaryBufferMemory.predict_new_summary method.
 
     Attributes:
         messages (List[BaseMessage]): List of BaseMessage to save.
     """
 
     messages: Optional[List[Message]] = None
+    prompt_version: Optional[str] = None
 
     def __init__(self, **kwargs):
         """The __init__ method.
 
         The initialization method saves the memory context from messages in `messages` attribute to the memory buffer.
 
         Args:
@@ -112,27 +90,42 @@
             elif pair.type.lower() == ChatMessageEnum.AI.value:
                 ai_dict = {self.output_key: pair.content}
 
         return human_dict, ai_dict
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         """Save context from the conversation to buffer and prune memories"""
+
         def message_to_dict(message):
             return {
                 "content": message.content,
                 "type": message.type
             }
 
         super().save_context(inputs, outputs)
         message_list = self.load_memory
         messages_dicts = [message_to_dict(message) for message in message_list]
         inputs[self.memory_key] = messages_dicts
 
+    def predict_new_summary(
+            self, messages: List[BaseMessage], existing_summary: str
+    ) -> str:
+        """Predict new summary, summarize memories in multiple rounds of conversations."""
+        new_lines = get_buffer_string(
+            messages,
+            human_prefix=self.human_prefix,
+            ai_prefix=self.ai_prefix,
+        )
+        prompt_version = self.prompt_version if self.prompt_version else 'chat_memory.summarizer_cn'
+        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+        chain = LLMChain(llm=self.llm, prompt=prompt.as_langchain())
+        return chain.predict(summary=existing_summary, new_lines=new_lines)
+
 
-class FinCoConversationTokenBufferMemory(ConversationTokenBufferMemory):
+class AuConversationTokenBufferMemory(ConversationTokenBufferMemory):
     """Short term memory to store conversation memory.
 
     If memories exceeds the max tokens limit, the requirement is met by truncating part of memories
 
     Attributes:
         messages (List[BaseMessage]): List of BaseMessage to save.
     """
@@ -187,14 +180,15 @@
             elif pair.type == ChatMessageEnum.AI.value:
                 ai_dict = {self.output_key: pair.content}
 
         return human_dict, ai_dict
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         """Save context from the conversation to buffer and truncate part of memories."""
+
         def message_to_dict(message):
             return {
                 "content": message.content,
                 "type": message.type
             }
 
         super().save_context(inputs, outputs)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/memory/memory.py` & `agentUniverse-0.0.4/agentuniverse/agent/memory/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     memory_key: Optional[str] = 'chat_history'
     max_tokens: int = 2000
 
     def __init__(self, **kwargs):
         super().__init__(component_type=ComponentEnum.MEMORY, **kwargs)
 
     def as_langchain(self) -> BaseMemory:
-        """Convert the finCo memory class to the langchain memory class."""
+        """Convert the AgentUniverse(AU) memory class to the langchain memory class."""
         pass
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the Memory model in the agent configuration."""
         if 'memory_key' in kwargs and kwargs['memory_key']:
             self.memory_key = kwargs['memory_key']
         if 'max_tokens' in kwargs and kwargs['max_tokens']:
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/memory/memory_manager.py` & `agentUniverse-0.0.4/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/output_object.py` & `agentUniverse-0.0.4/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 """Execution planner module."""
 import asyncio
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
 from langchain_core.prompts import PromptTemplate
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
-from agentuniverse.agent.plan.planner.executing_planner.prompt import target, introduction, instruction
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
+from agentuniverse.prompt.prompt import Prompt
+from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
 class ExecutingPlanner(Planner):
     """Executing planner class."""
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
@@ -61,12 +62,18 @@
         origin_instruction = profile.get('instruction')
         user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
 
         user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
                                                                target=profile.get('target'),
                                                                instruction=user_instruction)
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=introduction, target=target,
-                                                                 instruction=expert_framework + instruction)
-        self.prompt.build_prompt_template(user_prompt_model, system_prompt_model,
-                                          self.prompt_assemble_order)
+        # get the prompt by the prompt version
+        prompt_version: str = profile.get('prompt_version') or 'executing_planner.default_cn'
+        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
+                                                                 target=prompt.target,
+                                                                 instruction=expert_framework + prompt.instruction)
+
+        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
+                                 self.prompt_assemble_order)
         process_llm_token(self.prompt.as_langchain(), profile, planner_input)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/prompt.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_cn_prompt.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-# !/usr/bin/env python3
-# -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:46
-# @Author  : heji
-# @Email   : lc299034@antgroup.com
-# @FileName: prompt.py
-introduction = """
-你是一位精通信息分析的ai助手。
-"""
-
-target = """
-你的目标是根据用户提供的问题，对查找到的知识进行整合、修正，用来回答用户问题。
-"""
-
-instruction = """
-你需要仅仅根据我提供的背景知识来回答我的问题。
-你的回答需要尽可能的详细、全面，包含足够多的数据信息。
---------------------------------------------------------------
-需要遵守下面的规则：
-1.去除重复的信息。
-2.去除对回答问题没有帮助的信息。
-3.去除错误的信息。
-4.只可以使用这些信息来回答问题。
-5.简明扼要，重点突出，不过多花哨词藻。
-6.不在多处讲到同一个细节点，一个点只出现一次。
-7.尽量多的使用数值类信息。
-8.不可以出现XXX、ABC等不明确的词语。
-
-之前的对话:
-{chat_history}
-
-背景信息是:
-{background}
-
-开始!
-我的问题是: {input}
-
---------------------------------------------------------------
-必须使用中文进行详细的回答。你需要聚焦在我的问题上，不要延伸这个问题。
-让我们一步一步来。
-"""
+introduction: 你是一位精通信息分析的ai助手。
+target: 你的目标是根据用户提供的问题，对查找到的知识进行整合、修正，用来回答用户问题。
+instruction: |
+  你需要仅仅根据我提供的背景知识来回答我的问题。
+  你的回答需要尽可能的详细、全面，包含足够多的数据信息。
+  --------------------------------------------------------------
+  需要遵守下面的规则：
+  1.去除重复的信息。
+  2.去除对回答问题没有帮助的信息。
+  3.去除错误的信息。
+  4.只可以使用这些信息来回答问题。
+  5.简明扼要，重点突出，不过多花哨词藻。
+  6.不在多处讲到同一个细节点，一个点只出现一次。
+  7.尽量多的使用数值类信息。
+  8.不可以出现XXX、ABC等不明确的词语。
+  
+  之前的对话:
+  {chat_history}
+  
+  背景信息是:
+  {background}
+  
+  开始!
+  我的问题是: {input}
+  
+  --------------------------------------------------------------
+  必须使用中文进行详细的回答。你需要聚焦在我的问题上，不要延伸这个问题。
+  让我们一步一步来。
+metadata:
+  type: 'PROMPT'
+  version: 'executing_planner.default_cn'
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
 from langchain_core.prompts import PromptTemplate
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
-from agentuniverse.agent.plan.planner.expressing_planner.prompt import target, instruction, introduction
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
+from agentuniverse.prompt.prompt import Prompt
+from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
 class ExpressingPlanner(Planner):
     """Expressing planner class."""
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
@@ -61,12 +62,18 @@
         origin_instruction = profile.get('instruction')
         user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
 
         user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
                                                                target=profile.get('target'),
                                                                instruction=user_instruction)
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=introduction, target=target,
-                                                                 instruction=expert_framework + instruction)
-        self.prompt.build_prompt_template(user_prompt_model, system_prompt_model,
-                                          self.prompt_assemble_order)
+        # get the prompt by the prompt version
+        prompt_version: str = profile.get('prompt_version') or 'expressing_planner.default_cn'
+        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
+                                                                 target=prompt.target,
+                                                                 instruction=expert_framework + prompt.instruction)
+
+        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
+                                 self.prompt_assemble_order)
         process_llm_token(self.prompt.as_langchain(), profile, planner_input)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/prompt.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_cn_prompt.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-# !/usr/bin/env python3
-# -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:51
-# @Author  : heji
-# @Email   : lc299034@antgroup.com
-# @FileName: prompt.py
-introduction = """
-你是一个文本编辑专家，你非常擅长从繁杂的信息中提取关键信息。
-"""
-
-target = """
-你的目标是根据提供的信息生成一个新的答案，用来回答一个新的问题。
-"""
-
-instruction = """
-需要从不同角度、有条理的回答用户的问题。
-仅仅使用提供的知识，专业、详细的回答用户的问题。
-需要遵守下面的规则：
-- 回答必须是总-分结构，第一段总论点，用一句话简要总结回答问题。第二段分论点，进行专业、有结构性、通顺流畅的阐述论点。
-- 仅仅可以使用提供的知识来回答问题，如果字数允许，可以使用知识中的数值和数据，作为分论点的论据支撑。如果提供的知识并不足够回答问题，则可以回复"缺乏具体信息"等解释的话术。
-- 不描述重复的信息、不做对问题没有帮助的回答、不说模糊的推测、不可以出现XXX、ABC等不明确的词语。
-- 整体文风要简明扼要，重点突出，没有重复信息，必要时可以通过空行提升阅读体验，生成的字数小于500字。
-
-之前的对话:
-{chat_history}
-
-背景信息是:
-{background}
-
-开始!
-需要回答的问题是: {input}
---------------------------------------------------------------
-请根据规则要求做出回答。
-"""
+introduction: 你是一个文本编辑专家，你非常擅长从繁杂的信息中提取关键信息。
+target: 你的目标是根据提供的信息生成一个新的答案，用来回答一个新的问题。
+instruction: |
+  需要从不同角度、有条理的回答用户的问题。
+  仅仅使用提供的知识，专业、详细的回答用户的问题。
+  需要遵守下面的规则：
+  - 回答必须是总-分结构，第一段总论点，用一句话简要总结回答问题。第二段分论点，进行专业、有结构性、通顺流畅的阐述论点。
+  - 仅仅可以使用提供的知识来回答问题，如果字数允许，可以使用知识中的数值和数据，作为分论点的论据支撑。如果提供的知识并不足够回答问题，则可以回复"缺乏具体信息"等解释的话术。
+  - 不描述重复的信息、不做对问题没有帮助的回答、不说模糊的推测、不可以出现XXX、ABC等不明确的词语。
+  - 整体文风要简明扼要，重点突出，没有重复信息，必要时可以通过空行提升阅读体验，生成的字数小于500字。
+  
+  之前的对话:
+  {chat_history}
+  
+  背景信息是:
+  {background}
+  
+  开始!
+  必须使用中文回答用户提出的问题。
+  需要回答的问题是: {input}
+  --------------------------------------------------------------
+  请根据规则要求做出回答。
+metadata:
+  type: 'PROMPT'
+  version: 'expressing_planner.default_cn'
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,53 +112,71 @@
             if not planning_result or jump_step == "planning":
                 if not planningAgent:
                     LOGGER.warn("no planning agent, use default.")
                     planning_result = OutputObject({"framework": [agent_input.get('input')]})
                 else:
                     planning_result = planningAgent.run(**input_object.to_dict())
 
-                LOGGER.info(f"Planning agent execution result is {planning_result.to_json_str()}.")
                 input_object.add_data('planning_result', planning_result)
+                # add planning agent log info
+                logger_info = f"\nPlanning agent execution result is :\n"
+                for index, one_framework in enumerate(planning_result.get_data('framework')):
+                    logger_info += f"[{index + 1}] {one_framework} \n"
+                LOGGER.info(logger_info)
 
             if not executing_result or jump_step in ["planning", "executing"]:
                 if not executingAgent:
                     LOGGER.warn("no executing agent, use default.")
                     executing_result = OutputObject({})
                 else:
                     executing_result = executingAgent.run(**input_object.to_dict())
 
-                LOGGER.info(f"Executing agent execution result is {executing_result.to_json_str()}.")
                 input_object.add_data('executing_result', executing_result)
+                # add executing agent log info
+                logger_info = f"\nExecuting agent execution result is :\n"
+                for index, one_exec_res in enumerate(executing_result.get_data('executing_result')):
+                    one_exec_log_info = f"[{index + 1}] input: {one_exec_res['input']}\n"
+                    one_exec_log_info += f"[{index + 1}] output: {one_exec_res['output']}\n"
+                    logger_info += one_exec_log_info
+                LOGGER.info(logger_info)
 
             if not expressing_result or jump_step in ["planning", "executing", "expressing"]:
                 if not expressingAgent:
                     LOGGER.warn("no expression agent, use default.")
                     expressing_result = OutputObject({})
                 else:
                     expressing_result = expressingAgent.run(**input_object.to_dict())
 
-                LOGGER.info(f"Expressing agent execution result is {expressing_result.to_json_str()}.")
                 input_object.add_data('expressing_result', expressing_result)
+                # add expressing agent log info
+                logger_info = f"\nExpressing agent execution result is :\n"
+                logger_info += f"{expressing_result.get_data('output')}"
+                LOGGER.info(logger_info)
 
             if not reviewing_result or jump_step in ["planning", "executing", "expressing", "reviewing"]:
                 if not reviewingAgent:
                     LOGGER.warn("no expression agent, use default.")
                     loopResults.append({
                         "planning_result": planning_result,
                         "executing_result": executing_result,
                         "expressing_result": expressing_result,
                         "reviewing_result": reviewing_result
                     })
                     result['result'] = loopResults
                     return result
                 else:
                     reviewing_result = reviewingAgent.run(**input_object.to_dict())
-
-                    LOGGER.info(f"Reviewing agent execution result is {reviewing_result.to_json_str()}.")
                     input_object.add_data('evaluator_result', reviewing_result)
+
+                    # add reviewing agent log info
+                    logger_info = f"\nReviewing agent execution result is :\n"
+                    reviewing_info_str = f"review suggestion: {reviewing_result.get_data('suggestion')} \n"
+                    reviewing_info_str += f"useful: {reviewing_result.get_data('is_useful')} \n"
+                    LOGGER.info(logger_info + reviewing_info_str)
+
                     if reviewing_result.get_data('score') and reviewing_result.get_data('score') >= eval_threshold:
                         loopResults.append({
                             "planning_result": planning_result,
                             "executing_result": executing_result,
                             "expressing_result": expressing_result,
                             "reviewing_result": reviewing_result
                         })
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.memory.memory import Memory
 from agentuniverse.agent.memory.message import Message
 from agentuniverse.agent.memory.memory_manager import MemoryManager
 from agentuniverse.base.component.component_base import ComponentBase
 from agentuniverse.base.component.component_enum import ComponentEnum
 from agentuniverse.base.config.component_configer.configers.planner_configer import PlannerConfiger
-from agentuniverse.base.util.logging.logging_util import LOGGER
 from agentuniverse.llm.llm import LLM
 from agentuniverse.llm.llm_manager import LLMManager
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.base.util.memory_util import generate_messages
 
 
 class Planner(ComponentBase):
@@ -83,16 +82,14 @@
         params['messages'] = messages
         params['llm'] = llm
         params['input_key'] = self.input_key
         params['output_key'] = self.output_key
 
         memory: Memory = MemoryManager().get_instance_obj(memory_name)
         if memory is None:
-            # todo process memory warning
-            # LOGGER.warn('memory does not exist.')
             return None
         memory.set_by_agent_model(**params)
         langchain_memory: BaseMemory = memory.as_langchain()
 
         planner_input['chat_history'] = langchain_memory.load_memory_str
         return langchain_memory
 
@@ -108,19 +105,23 @@
         tools: list = action.get('tool') or list()
         knowledge: list = action.get('knowledge') or list()
 
         action_result: list = list()
 
         for tool_name in tools:
             tool = ToolManager().get_instance_obj(tool_name)
+            if tool is None:
+                continue
             tool_input = {key: input_object.get_data(key) for key in tool.input_keys}
             action_result.append(tool.run(**tool_input))
 
         for knowledge_name in knowledge:
             knowledge: Knowledge = KnowledgeManager().get_instance_obj(knowledge_name)
+            if knowledge is None:
+                continue
             knowledge_res: List[Document] = knowledge.store.query(
                 Query(query_str=input_object.get_data(self.input_key), similarity_top_k=2), **input_object.to_dict())
             for document in knowledge_res:
                 action_result.append(document.text)
 
         planner_input['background'] = planner_input['background'] or '' + "\n".join(action_result)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner_manager.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/14 16:02
+# @Time    : 2024/3/18 10:55
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: planning_planner.py
-"""Planning planner module."""
+# @FileName: reviewing_planner.py
+"""Reviewing planner module."""
 import asyncio
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
-
+from langchain_core.prompts import PromptTemplate
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
-from agentuniverse.agent.plan.planner.planning_planner.prompt import instruction, target, introduction
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
+from agentuniverse.prompt.prompt import Prompt
+from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class PlanningPlanner(Planner):
-    """Planning planner class."""
+class ReviewingPlanner(Planner):
+    """Reviewing planner class."""
 
-    def invoke(self, agent_model: AgentModel, planner_input: dict,
-               input_object: InputObject) -> dict:
+    def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         Returns:
@@ -38,34 +38,40 @@
 
         self.handle_prompt(agent_model, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
                              prompt=self.prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
 
-        return asyncio.run(llm_chain.acall(planner_input))
+        return asyncio.run(llm_chain.acall(inputs=planner_input))
 
     def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
-        """Prompt module processing.
+        """Generate prompt template for the planner.
 
         Args:
-            agent_model (AgentModel): Agent model object.
-            planner_input (dict): Planner input object.
+            agent_model (AgentModel): The agent model.
+            planner_input (dict): The agent input.
         Returns:
             PromptTemplate: The prompt template.
         """
         expert_framework = planner_input.pop('expert_framework', '') or ''
 
         profile: dict = agent_model.profile
 
         origin_instruction = profile.get('instruction')
         user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
 
         user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
                                                                target=profile.get('target'),
                                                                instruction=user_instruction)
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=introduction, target=target,
-                                                                 instruction=expert_framework + instruction)
-        self.prompt.build_prompt_template(user_prompt_model, system_prompt_model,
-                                          self.prompt_assemble_order)
+        # get the prompt by the prompt version
+        prompt_version: str = profile.get('prompt_version') or 'reviewing_planner.default_cn'
+        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
+                                                                 target=prompt.target,
+                                                                 instruction=expert_framework + prompt.instruction)
+
+        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
+                                 self.prompt_assemble_order)
         process_llm_token(self.prompt.as_langchain(), profile, planner_input)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 """Rag planner module."""
 import asyncio
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
-from agentuniverse.agent.plan.planner.rag_planner.prompt import introduction, target, instruction
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
+from agentuniverse.prompt.prompt import Prompt
+from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
 class RagPlanner(Planner):
     """Rag planner class."""
 
     def invoke(self, agent_model: AgentModel, planner_input: dict,
@@ -55,12 +56,18 @@
         """
         profile: dict = agent_model.profile
 
         user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
                                                                target=profile.get('target'),
                                                                instruction=profile.get('instruction'))
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=introduction, target=target,
-                                                                 instruction=instruction)
-        self.prompt.build_prompt_template(user_prompt_model, system_prompt_model,
-                                          self.prompt_assemble_order)
+        # get the prompt by the prompt version
+        prompt_version: str = profile.get('prompt_version') or 'rag_planner.default_cn'
+        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
+                                                                 target=prompt.target,
+                                                                 instruction=prompt.instruction)
+
+        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
+                                 self.prompt_assemble_order)
         process_llm_token(self.prompt.as_langchain(), profile, planner_input)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:55
+# @Time    : 2024/3/14 16:02
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: reviewing_planner.py
-"""Reviewing planner module."""
+# @FileName: planning_planner.py
+"""Planning planner module."""
 import asyncio
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
-from langchain_core.prompts import PromptTemplate
+
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
-from agentuniverse.agent.plan.planner.reviewing_planner.prompt import target, instruction, introduction
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
+from agentuniverse.prompt.prompt import Prompt
+from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class ReviewingPlanner(Planner):
-    """Reviewing planner class."""
+class PlanningPlanner(Planner):
+    """Planning planner class."""
 
-    def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
+    def invoke(self, agent_model: AgentModel, planner_input: dict,
+               input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         Returns:
@@ -37,34 +39,39 @@
 
         self.handle_prompt(agent_model, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
                              prompt=self.prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
 
-        return asyncio.run(llm_chain.acall(inputs=planner_input))
+        return asyncio.run(llm_chain.acall(planner_input))
 
     def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
-        """Generate prompt template for the planner.
+        """Prompt module processing.
 
         Args:
-            agent_model (AgentModel): The agent model.
-            planner_input (dict): The agent input.
+            agent_model (AgentModel): Agent model object.
+            planner_input (dict): Planner input object.
         Returns:
             PromptTemplate: The prompt template.
         """
         expert_framework = planner_input.pop('expert_framework', '') or ''
 
         profile: dict = agent_model.profile
 
         origin_instruction = profile.get('instruction')
         user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
 
         user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
                                                                target=profile.get('target'),
                                                                instruction=user_instruction)
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=introduction, target=target,
-                                                                 instruction=expert_framework + instruction)
-        self.prompt.build_prompt_template(user_prompt_model, system_prompt_model,
-                                          self.prompt_assemble_order)
+        # get the prompt by the prompt version
+        prompt_version: str = profile.get('prompt_version') or 'planning_planner.default_cn'
+        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
+                                                                 target=prompt.target,
+                                                                 instruction=expert_framework + prompt.instruction)
+        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
+                                 self.prompt_assemble_order)
         process_llm_token(self.prompt.as_langchain(), profile, planner_input)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/service.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/service_configer.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/service_instance.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/request_library.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # @Author  : fanen.lhy
 # @Email   : fanen.lhy@antgroup.com
 # @FileName: request_library.py
 
 import datetime
 import json
 
-from sqlalchemy import JSON, Integer, String, DateTime, Column, create_engine
+from sqlalchemy import JSON, Integer, String, DateTime, Text, Column
+from sqlalchemy import create_engine
 from sqlalchemy import select
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
 from .entity.request_do import RequestDO
 from agentuniverse.base.util.system_util import get_project_root_path
 from agentuniverse.base.config.configer import Configer
@@ -23,18 +24,18 @@
 Base = declarative_base()
 
 
 class RequestORM(Base):
     """SQLAlchemy ORM Model for RequestDO."""
     __tablename__ = REQUEST_TABLE_NAME
     id = Column(Integer, primary_key=True, autoincrement=True)
-    request_id = Column(String, nullable=False)
-    query = Column(String)
-    session_id = Column(String)
-    state = Column(String)
+    request_id = Column(String(20), nullable=False)
+    query = Column(Text)
+    session_id = Column(String(50))
+    state = Column(String(20))
     result = Column(JSON)
     steps = Column(JSON)
     additional_args = Column(JSON)
     gmt_create = Column(DateTime, default=datetime.datetime.now)
     gmt_modified = Column(DateTime, default=datetime.datetime.now,
                           onupdate=datetime.datetime.now)
 
@@ -50,35 +51,27 @@
         if mysql_uri and mysql_uri.strip():
             db_uri = mysql_uri
         else:
             db_path = get_project_root_path() / 'DB' / 'agent_framework.db'
             db_path.parent.mkdir(parents=True, exist_ok=True)
             db_uri = f'sqlite:////{db_path}'
 
-        # Create database engine
-        self.engine = create_engine(
-            db_uri,
-            _json_serializer=lambda x: json.dumps(x, ensure_ascii=False)
-        )
-        self.Session = sessionmaker(bind=self.engine)
-
-        with self.engine.connect() as conn:
-            if not conn.dialect.has_table(conn, REQUEST_TABLE_NAME):
-                Base.metadata.create_all(self.engine)
+        self.db_uri = db_uri
+        self.Session = None
 
     def query_request_by_request_id(self, request_id: str) -> RequestDO | None:
         """Get a RequestDO with given request_id.
 
         Args:
             request_id(`str`): The unique request id of request task.
 
         Return:
             The target RequestDO or none when no such data.
         """
-        session = self.Session()
+        session = self.__get_session()
         try:
             result = session.execute(
                 select(RequestORM).where(RequestORM.request_id == request_id)
             ).scalars().first()
             if not result:
                 return None
             return self.__request_orm_to_do(result)
@@ -90,52 +83,67 @@
 
         Args:
             request_do(`RequestDO`): A new RequestDO to be added.
 
         Return:
             A int stands unique data id in table.
         """
-        session = self.Session()
+        session = self.__get_session()
         try:
             request_orm = RequestORM(**request_do.model_dump())
             session.add(request_orm)
             session.commit()
             return request_orm.id
         finally:
             session.close()
 
     def update_request(self, request_do: RequestDO):
         """Update the request data with same request id as the given
         RequestDO."""
-        session = self.Session()
+        session = self.__get_session()
         try:
             db_request_do = session.query(RequestORM).filter(
                 RequestORM.request_id == request_do.request_id).first()
             if db_request_do:
                 update_data = request_do.model_dump(exclude_unset=True)
                 for key, value in update_data.items():
                     setattr(db_request_do, key, value)
                 session.commit()
                 session.refresh(db_request_do)
         finally:
             session.close()
 
     def update_gmt_modified(self, request_id: str):
         """Update the request task latest active time."""
-        session = self.Session()
+        session = self.__get_session()
         try:
             db_request_do = session.query(RequestORM).filter(
                 RequestORM.request_id == request_id).first()
             if db_request_do:
                 setattr(db_request_do, "gmt_modified", datetime.datetime.now())
                 session.commit()
                 session.refresh(db_request_do)
         finally:
             session.close()
 
+    def __get_session(self):
+        if self.Session:
+            return self.Session()
+        # Create database engine
+        self.engine = create_engine(
+            self.db_uri,
+            json_serializer=lambda x: json.dumps(x, ensure_ascii=False)
+        )
+        self.Session = sessionmaker(bind=self.engine)
+
+        with self.engine.connect() as conn:
+            if not conn.dialect.has_table(conn, REQUEST_TABLE_NAME):
+                Base.metadata.create_all(self.engine)
+        return self.Session()
+
     def __request_orm_to_do(self, request_orm: RequestORM) -> RequestDO:
         """Transfer a RequestORM to RequestDO."""
         request_obj = RequestDO(
             request_id='',
             session_id="",
             query='',
             state='',
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/web/request_task.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/web/request_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
         """Update request task state if the transition is valid."""
         if ((TaskStateEnum[self.__request_do__.state.upper()], next_state)
                 in VALID_TRANSITIONS):
             self.__request_do__.state = next_state.value
         else:
             raise Exception("Invalid state transition")
 
-
     def check_state(self):
         """Keep check request task thread state every minute, if the thread
         is alive, update the request modified time in database."""
         while True:
             if self.thread is not None and self.thread.is_alive():
                 LOGGER.debug(
                     "request:" + str(self.request_id) + "task thread alive")
@@ -230,17 +229,17 @@
         """Query the request data in database by given request_id.
 
         Args:
             request_id(str): Unique request id.
         """
         request_do = RequestLibrary().query_request_by_request_id(
             request_id)
-        RequestTask.is_validate(request_do)
         if request_do is None:
             return {"state": TaskStateEnum.INIT.value,
                     "result": None,
                     "steps": None}
+        RequestTask.is_validate(request_do)
         return {
             "state": request_do.state,
-            "result": request_do.result.get('result'),
+            "result": request_do.result,
             "steps": request_do.steps
         }
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/web/thread_with_result.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_server.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/web/flask_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from flask import Flask, Response
 from werkzeug.exceptions import HTTPException
 
 from ..service_instance import ServiceInstance, ServiceNotFoundError
 from .request_task import RequestTask
 from .web_util import request_param, service_run_queue, make_standard_response
-from agentuniverse.base.util.logging.logging_util import LOGGER
+from ...base.util.logging.logging_util import LOGGER
 
 
 app = Flask(__name__)
 app.config['JSON_AS_ASCII'] = False
 
 
 @app.route("/echo")
@@ -22,67 +22,70 @@
 def liveness():
     return make_standard_response(success=True,
                                   result="liveness health check pass!")
 
 
 @app.route("/service_run", methods=['POST'])
 @request_param
-def service_run(service_id: str, params: dict):
+def service_run(service_id: str, params: dict, saved: bool = False):
     """Synchronous invocation of an agent service.
 
     Request Args:
         service_id(`str`): The id of the agent service. Format like
             {appname}.service.{service_name}.
         params(`dict`): Json style params passed to service.
+        saved(`bool`): Save the request and result into database.
 
     Return:
         Returns a dict containing two keys: success and result.
         success: This key holds a boolean value indicating the task was
         successfully or not.
         result: This key points to a nested dictionary that includes the
         result of the task.
     """
     params = {} if params is None else params
-    request_task = RequestTask(ServiceInstance(service_id).run, **params)
+    request_task = RequestTask(ServiceInstance(service_id).run, saved, **params)
     result = request_task.run()
     return make_standard_response(success=True, result=result,
                                   request_id=request_task.request_id)
 
 
 @app.route("/service_run_stream", methods=['POST'])
 @request_param
-def service_run_stream(service_id: str, params: dict):
+def service_run_stream(service_id: str, params: dict, saved: bool = False):
     """Synchronous invocation of an agent service, return in stream form.
 
     Request Args:
         service_id(`str`): The id of the agent service. Format like
             {appname}.service.{service_name}.
         params(`dict`): Json style params passed to service.
+        saved(`bool`): Save the request and result into database.
 
     Return:
         A SSE(Server-Sent Event) stream.
     """
     params = {} if params is None else params
     params['service_id'] = service_id
-    task = RequestTask(service_run_queue, False, **params)
+    task = RequestTask(service_run_queue, saved, **params)
     response = Response(task.stream_run(), mimetype="text/event-stream")
     response.headers['X-Request-ID'] = task.request_id
     return response
 
 
 @app.route("/service_run_async", methods=['POST'])
 @request_param
-def service_run_async(service_id: str, params: dict):
+def service_run_async(service_id: str, params: dict, saved: bool = True):
     """Async invocation of an agent service, return the request id used to
     get result later.
 
     Request Args:
         service_id(`str`): The id of the agent service. Format like
             {appname}.service.{service_name}.
         params(`dict`): Json style params passed to service.
+        saved(`bool`): Save the request and result into database.
 
     Return:
         Returns a dict containing two keys: success and result.
         success: This key holds a boolean value indicating the task was
         successfully or not.
         result: This key points to a dictionary contains a key: request_id,
         its value can be used in service_run_result api to get the result
@@ -90,15 +93,15 @@
 
     Example Response:
         {"success": True, "data": {
         "request_id":"05d0a28785cc455894ebb88bba14a67e"}}.
     """
     params = {} if params is None else params
     params['service_id'] = service_id
-    task = RequestTask(service_run_queue, **params)
+    task = RequestTask(service_run_queue, saved, **params)
     task.async_run()
     return make_standard_response(success=True,
                                   request_id=task.request_id)
 
 
 @app.route("/service_run_result", methods=['GET'])
 @request_param
```

### Comparing `agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_util.py` & `agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,20 @@
         sig = inspect.signature(func)
         for name, param in sig.parameters.items():
             if name == "kwargs":
                 for key in req_data:
                     if key not in kwargs:
                         kwargs[key] = req_data[key]
                 continue
+            if name == "saved":
+                if "saved" in req_data:
+                    kwargs['saved'] = req_data['saved']
+                else:
+                    kwargs['saved'] = sig.parameters['saved'].default
+                continue
             if name == "session_id":
                 kwargs[name] = request.headers.get("X-Session-Id")
             elif param.annotation in (str, int, dict, list):
                 kwargs[name] = req_data.get(name)
             else:
                 kwargs[name] = param.annotation(**req_data)
         return func(*args, **kwargs)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/agentuniverse.py` & `agentUniverse-0.0.4/agentuniverse/base/agentuniverse.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,65 +19,75 @@
 from agentuniverse.base.config.config_type_enum import ConfigTypeEnum
 from agentuniverse.base.config.configer import Configer
 from agentuniverse.base.config.custom_configer.custom_key_configer import CustomKeyConfiger
 from agentuniverse.base.component.component_enum import ComponentEnum
 from agentuniverse.base.util.system_util import get_project_root_path
 from agentuniverse.base.util.logging.logging_util import init_loggers
 from agentuniverse.agent_serve.web.request_task import RequestLibrary
-from agentuniverse.agent_serve.web.web_booster import GunicornApplication
 
 
 @singleton
 class AgentUniverse(object):
-    """agentUniverse object, responsible for the framework initialization,
+    """AgentUniverse framework object, responsible for the framework initialization,
        system variables management, etc."""
 
     def __init__(self):
         self.__application_container = ApplicationComponentManager()
         self.__config_container: ApplicationConfigManager = ApplicationConfigManager()
         self.__system_default_package = ['agentuniverse']
 
     def start(self, config_path: str = None):
         """Start the agentUniverse framework."""
-        # step0: get default config path
+        # get default config path
         project_root_path = get_project_root_path()
+        sys.path.append(str(project_root_path.parent))
         app_path = project_root_path / 'app'
         if app_path.exists():
             sys.path.append(str(app_path))
         if not config_path:
             config_path = project_root_path / 'config' / 'config.toml'
             config_path = str(config_path)
 
-        # step1: load the configuration file
+        # load the configuration file
         configer = Configer(path=config_path).load()
         app_configer = AppConfiger().load_by_configer(configer)
         self.__config_container.app_configer = app_configer
 
-        # Load User custom key.
+        # load user custom key
         custom_key_configer_path = self.__parse_sub_config_path(
             configer.value.get('SUB_CONFIG_PATH', {}).get('custom_key_path'),
             config_path)
         CustomKeyConfiger(custom_key_configer_path)
 
-        # Init loguru loggers.
+        # init loguru loggers
         log_config_path = self.__parse_sub_config_path(
             configer.value.get('SUB_CONFIG_PATH', {}).get('log_config_path'),
             config_path)
         init_loggers(log_config_path)
 
-        # Init web request task database.
+        # init web request task database
         RequestLibrary(configer=configer)
 
-        # Init gunicorn web server.
-        gunicorn_config_path = self.__parse_sub_config_path(
-            configer.value.get('SUB_CONFIG_PATH', {})
-            .get('gunicorn_config_path'), config_path)
-        GunicornApplication(config_path=gunicorn_config_path)
+        # init gunicorn web server on mac or unix platform
+        if not sys.platform.lower().startswith("win"):
+            gunicorn_config_path = self.__parse_sub_config_path(
+                configer.value.get('SUB_CONFIG_PATH', {})
+                .get('gunicorn_config_path'), config_path
+            )
+            from ..agent_serve.web.gunicorn_server import \
+                GunicornApplication
+            GunicornApplication(config_path=gunicorn_config_path)
+
+        # init all extension module
+        ext_classes = configer.value.get('EXTENSION_MODULES', {}).get('class_list')
+        if isinstance(ext_classes, list):
+            for ext_class in ext_classes:
+                self.__dynamic_import_and_init(ext_class, configer)
 
-        # step2: scan and register the components
+        # scan and register the components
         self.__scan_and_register(self.__config_container.app_configer)
 
     def __scan_and_register(self, app_configer: AppConfiger):
         """Scan the component directory and register the components.
 
         Args:
             app_configer(AppConfiger): the AppConfiger object
@@ -85,23 +95,25 @@
         core_agent_package_list = app_configer.core_agent_package_list or app_configer.core_default_package_list + self.__system_default_package
         core_knowledge_package_list = app_configer.core_knowledge_package_list or app_configer.core_default_package_list + self.__system_default_package
         core_llm_package_list = app_configer.core_llm_package_list or app_configer.core_default_package_list + self.__system_default_package
         core_planner_package_list = app_configer.core_planner_package_list or app_configer.core_default_package_list + self.__system_default_package
         core_tool_package_list = app_configer.core_tool_package_list or app_configer.core_default_package_list + self.__system_default_package
         core_service_package_list = app_configer.core_service_package_list or app_configer.core_default_package_list + self.__system_default_package
         core_memory_package_list = app_configer.core_memory_package_list or app_configer.core_default_package_list + self.__system_default_package
+        core_prompt_package_list = app_configer.core_prompt_package_list or app_configer.core_default_package_list + self.__system_default_package
 
         component_package_map = {
             ComponentEnum.AGENT: core_agent_package_list,
             ComponentEnum.KNOWLEDGE: core_knowledge_package_list,
             ComponentEnum.LLM: core_llm_package_list,
             ComponentEnum.PLANNER: core_planner_package_list,
             ComponentEnum.TOOL: core_tool_package_list,
             ComponentEnum.SERVICE: core_service_package_list,
-            ComponentEnum.MEMORY: core_memory_package_list
+            ComponentEnum.MEMORY: core_memory_package_list,
+            ComponentEnum.PROMPT: core_prompt_package_list
         }
 
         component_configer_list_map = {}
         for component_enum, package_list in component_package_map.items():
             if not package_list:
                 continue
             component_configer_list = self.__scan(package_list, ConfigTypeEnum.YAML, component_enum)
@@ -176,20 +188,33 @@
                                 reference_file_path: str) -> str | None:
         """Resolve a sub config file path according to main config file.
 
             Args:
                 input_path(str): Absolute or relative path of sub config file.
                 reference_file_path(str): Main config file path.
             Returns:
-                str or None: Final
+                str or None: A file path or none when no such file.
         """
         if not input_path:
             return None
 
         input_path_obj = Path(input_path)
         if input_path_obj.is_absolute():
             combined_path = input_path_obj
         else:
             reference_file_path_obj = Path(reference_file_path)
             combined_path = reference_file_path_obj.parent / input_path_obj
 
         return str(combined_path)
+
+    def __dynamic_import_and_init(self, class_path: str, configer: Configer):
+        """Resolve a sub config file path according to main config file.
+
+            Args:
+                class_path(str): Full class path like package_name.class_name.
+                Auto read from config file.
+        """
+
+        module_path, _, class_name = class_path.rpartition('.')
+        module = importlib.import_module(module_path)
+        cls = getattr(module, class_name)
+        cls(configer)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/annotation/singleton.py` & `agentUniverse-0.0.4/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/component/application_component_manager.py` & `agentUniverse-0.0.4/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/component/component_base.py` & `agentUniverse-0.0.4/agentuniverse/base/component/component_base.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/component/component_configer_util.py` & `agentUniverse-0.0.4/agentuniverse/base/component/component_configer_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,43 +16,47 @@
 from agentuniverse.agent_serve.service_manager import ServiceManager
 from agentuniverse.agent_serve.service_configer import ServiceConfiger
 from agentuniverse.base.config.component_configer.component_configer import ComponentConfiger
 from agentuniverse.base.config.component_configer.configers.agent_configer import AgentConfiger
 from agentuniverse.base.config.component_configer.configers.knowledge_configer import KnowledgeConfiger
 from agentuniverse.base.config.component_configer.configers.memory_configer import MemoryConfiger
 from agentuniverse.base.config.component_configer.configers.planner_configer import PlannerConfiger
+from agentuniverse.base.config.component_configer.configers.prompt_configer import PromptConfiger
 from agentuniverse.base.config.component_configer.configers.tool_configer import ToolConfiger
 from agentuniverse.base.config.config_type_enum import ConfigTypeEnum
 from agentuniverse.base.config.component_configer.configers.llm_configer import LLMConfiger
 from agentuniverse.base.component.component_enum import ComponentEnum
 from agentuniverse.llm.llm_manager import LLMManager
+from agentuniverse.prompt.prompt_manager import PromptManager
 
 
 class ComponentConfigerUtil(object):
     """The ComponentConfigerUtil class, which is used to load and manage the component configuration."""
 
     __COMPONENT_CONFIGER_CLZ_MAP = {
         ComponentEnum.AGENT: AgentConfiger,
         ComponentEnum.KNOWLEDGE: KnowledgeConfiger,
         ComponentEnum.LLM: LLMConfiger,
         ComponentEnum.PLANNER: PlannerConfiger,
         ComponentEnum.TOOL: ToolConfiger,
         ComponentEnum.MEMORY: MemoryConfiger,
         ComponentEnum.SERVICE: ServiceConfiger,
+        ComponentEnum.PROMPT: PromptConfiger,
         ComponentEnum.DEFAULT: ComponentConfiger
     }
 
     __COMPONENT_MANAGER_CLZ_MAP = {
         ComponentEnum.AGENT: AgentManager,
         ComponentEnum.KNOWLEDGE: KnowledgeManager,
         ComponentEnum.LLM: LLMManager,
         ComponentEnum.PLANNER: PlannerManager,
         ComponentEnum.TOOL: ToolManager,
         ComponentEnum.MEMORY: MemoryManager,
-        ComponentEnum.SERVICE: ServiceManager
+        ComponentEnum.SERVICE: ServiceManager,
+        ComponentEnum.PROMPT: PromptManager
     }
 
     @classmethod
     def get_component_config_clz_by_type(cls, component_type_enum: ComponentEnum) -> \
             Type[ComponentConfiger | LLMConfiger]:
         """Get the ComponentConfiger object by the component type.
         Args:
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/component/component_enum.py` & `agentUniverse-0.0.4/agentuniverse/base/component/component_enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,12 +14,13 @@
     KNOWLEDGE = "KNOWLEDGE"
     LLM = "LLM"
     PLANNER = "PLANNER"
     TOOL = "TOOL"
     DEFAULT = "DEFAULT"
     SERVICE = "SERVICE"
     MEMORY = "MEMORY"
+    PROMPT = "PROMPT"
 
     @staticmethod
     def to_value_list():
         """Return the value list of the enumeration."""
         return [item.value for item in ComponentEnum]
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/component/component_manager_base.py` & `agentUniverse-0.0.4/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/application_configer/app_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.__core_agent_package_list: Optional[list[str]] = None
         self.__core_knowledge_package_list: Optional[list[str]] = None
         self.__core_llm_package_list: Optional[list[str]] = None
         self.__core_planner_package_list: Optional[list[str]] = None
         self.__core_tool_package_list: Optional[list[str]] = None
         self.__core_memory_package_list: Optional[list[str]] = None
         self.__core_service_package_list: Optional[list[str]] = None
+        self.__core_prompt_package_list: Optional[list[str]] = None
 
     @property
     def base_info_appname(self) -> Optional[str]:
         """Return the appname of the application."""
         return self.__base_info_appname
 
     @property
@@ -66,14 +67,18 @@
         return self.__core_memory_package_list
 
     @property
     def core_service_package_list(self) -> Optional[list[str]]:
         """Return the service package list of the core."""
         return self.__core_service_package_list
 
+    @property
+    def core_prompt_package_list(self) -> Optional[list[str]]:
+        return self.__core_prompt_package_list
+
     def load_by_configer(self, configer: Configer) -> 'AppConfiger':
         """Load the AppConfiger by the given Configer.
 
         Args:
             configer(Configer): the Configer object
         Returns:
             AppConfiger: the AppConfiger object
@@ -84,8 +89,9 @@
         self.__core_agent_package_list = configer.value.get('CORE_PACKAGE', {}).get('agent')
         self.__core_knowledge_package_list = configer.value.get('CORE_PACKAGE', {}).get('knowledge')
         self.__core_llm_package_list = configer.value.get('CORE_PACKAGE', {}).get('llm')
         self.__core_planner_package_list = configer.value.get('CORE_PACKAGE', {}).get('planner')
         self.__core_tool_package_list = configer.value.get('CORE_PACKAGE', {}).get('tool')
         self.__core_memory_package_list = configer.value.get('CORE_PACKAGE', {}).get('memory')
         self.__core_service_package_list = configer.value.get('CORE_PACKAGE', {}).get('service')
+        self.__core_prompt_package_list = configer.value.get('CORE_PACKAGE', {}).get('prompt')
         return self
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentUniverse-0.0.4/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/component_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
-# @Time    : 2024/3/12 23:16
+# @Time    : 2024/3/13 12:01
 # @Author  : jerry.zzw 
 # @Email   : jerry.zzw@antgroup.com
-# @FileName: component_configer.py
-
+# @FileName: agent_configer.py
 from typing import Optional
+from agentuniverse.base.config.component_configer.component_configer import ComponentConfiger
 from agentuniverse.base.config.configer import Configer
 
 
-class ComponentConfiger(object):
-    """The ComponentConfiger class, which is used to load and manage the component configuration."""
+class AgentConfiger(ComponentConfiger):
+    """The AgentConfiger class, which is used to load and manage the Agent configuration."""
 
     def __init__(self, configer: Optional[Configer] = None):
-        """Initialize the ComponentConfiger."""
-        self.__configer: Optional[Configer] = configer
-        self.__metadata_type: Optional[str] = None
-        self.__metadata_module: Optional[str] = None
-        self.__metadata_class: Optional[str] = None
+        """Initialize the AgentConfiger."""
+        super().__init__(configer)
+        self.__info: Optional[dict] = dict()
+        self.__profile: Optional[dict] = dict()
+        self.__plan: Optional[dict] = dict()
+        self.__memory: Optional[dict] = dict()
+        self.__action: Optional[dict] = dict()
+
+    @property
+    def memory(self) -> Optional[dict]:
+        """Return the name of the Agent."""
+        return self.__memory
 
     @property
-    def configer(self) -> Optional[Configer]:
-        """Return the Configer object."""
-        return self.__configer
+    def action(self) -> Optional[dict]:
+        """Return the name of the Agent."""
+        return self.__action
 
     @property
-    def metadata_type(self) -> Optional[str]:
-        """Return the type of the component."""
-        return self.__metadata_type
+    def profile(self) -> Optional[dict]:
+        """Return the name of the Agent."""
+        return self.__profile
 
     @property
-    def metadata_module(self) -> Optional[str]:
-        """Return the module of the component."""
-        return self.__metadata_module
+    def plan(self) -> Optional[dict]:
+        """Return the description of the Agent."""
+        return self.__plan
 
     @property
-    def metadata_class(self) -> Optional[str]:
-        """Return the class of the component."""
-        return self.__metadata_class
+    def info(self) -> Optional[dict]:
+        """Return the name of the Agent."""
+        return self.__info
 
-    def load(self) -> 'ComponentConfiger':
+    def load(self) -> 'AgentConfiger':
         """Load the configuration by the Configer object.
         Returns:
-            ComponentConfiger: the ComponentConfiger object
+            AgentConfiger: the AgentConfiger object
         """
         return self.load_by_configer(self.configer)
 
-    def load_by_configer(self, configer: Configer) -> 'ComponentConfiger':
+    def load_by_configer(self, configer: Configer) -> 'AgentConfiger':
         """Load the configuration by the Configer object.
         Args:
             configer(Configer): the Configer object
         Returns:
-            ComponentConfiger: the ComponentConfiger object
+            AgentConfiger: the AgentConfiger object
         """
-        self.__configer = configer
+        super().load_by_configer(configer)
 
         try:
-            for k, v in configer.value.items():
-                self.__dict__[k] = v
-            self.__metadata_type = configer.value.get('metadata').get('type')
-            self.__metadata_module = configer.value.get('metadata').get('module')
-            self.__metadata_class = configer.value.get('metadata').get('class')
+            configer_value: dict = configer.value
+            self.__info = configer_value.get('info') or self.__info
+            self.__profile = configer_value.get('profile') or self.__profile
+            self.__plan = configer_value.get('plan') or self.__plan
+            self.__memory = configer_value.get('memory') or self.__memory
+            self.__action = configer_value.get('action') or self.__action
         except Exception as e:
-            raise Exception(f"Failed to parse the component configuration: {e}")
-
+            raise Exception(f"Failed to parse the Agent configuration: {e}")
         return self
-
-    def get_component_config_type(self) -> Optional[str]:
-        """Return the type of the component.
-
-        Returns:
-            Optional[str]: the type of the component
-        """
-        return self.__metadata_type
-
-
-
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,59 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 # @Time    : 2024/3/13 12:01
 # @Author  : jerry.zzw 
 # @Email   : jerry.zzw@antgroup.com
-# @FileName: agent_configer.py
-from typing import Optional
+# @FileName: knowledge_configer.py
+from typing import Optional, Dict
 from agentuniverse.base.config.component_configer.component_configer import ComponentConfiger
 from agentuniverse.base.config.configer import Configer
 
 
-class AgentConfiger(ComponentConfiger):
-    """The AgentConfiger class, which is used to load and manage the Agent configuration."""
+class KnowledgeConfiger(ComponentConfiger):
+    """The KnowledgeConfiger class, which is used to load and manage the Knowledge configuration."""
 
     def __init__(self, configer: Optional[Configer] = None):
-        """Initialize the AgentConfiger."""
+        """Initialize the KnowledgeConfiger."""
         super().__init__(configer)
-        self.__info: Optional[dict] = dict()
-        self.__profile: Optional[dict] = dict()
-        self.__plan: Optional[dict] = dict()
-        self.__memory: Optional[dict] = dict()
-        self.__action: Optional[dict] = dict()
+        self.__name: Optional[str] = None
+        self.__description: Optional[str] = None
+        self.__ext_info: Optional[Dict] = None
 
     @property
-    def memory(self) -> Optional[dict]:
-        """Return the name of the Agent."""
-        return self.__memory
+    def name(self) -> Optional[str]:
+        """Return the name of the Knowledge."""
+        return self.__name
 
     @property
-    def action(self) -> Optional[dict]:
-        """Return the name of the Agent."""
-        return self.__action
+    def description(self) -> Optional[str]:
+        """Return the description of the Knowledge."""
+        return self.__description
 
     @property
-    def profile(self) -> Optional[dict]:
-        """Return the name of the Agent."""
-        return self.__profile
+    def ext_info(self) -> Optional[Dict]:
+        return self.__ext_info
 
-    @property
-    def plan(self) -> Optional[dict]:
-        """Return the description of the Agent."""
-        return self.__plan
-
-    @property
-    def info(self) -> Optional[dict]:
-        """Return the name of the Agent."""
-        return self.__info
-
-    def load(self) -> 'AgentConfiger':
+    def load(self) -> 'KnowledgeConfiger':
         """Load the configuration by the Configer object.
         Returns:
-            AgentConfiger: the AgentConfiger object
+            KnowledgeConfiger: the KnowledgeConfiger object
         """
-        return self.load_by_configer(self.configer)
+        return self.load_by_configer(self.__configer)
 
-    def load_by_configer(self, configer: Configer) -> 'AgentConfiger':
+    def load_by_configer(self, configer: Configer) -> 'KnowledgeConfiger':
         """Load the configuration by the Configer object.
         Args:
             configer(Configer): the Configer object
         Returns:
-            AgentConfiger: the AgentConfiger object
+            KnowledgeConfiger: the KnowledgeConfiger object
         """
         super().load_by_configer(configer)
 
         try:
-            configer_value: dict = configer.value
-            self.__info = configer_value.get('info') or self.__info
-            self.__profile = configer_value.get('profile') or self.__profile
-            self.__plan = configer_value.get('plan') or self.__plan
-            self.__memory = configer_value.get('memory') or self.__memory
-            self.__action = configer_value.get('action') or self.__action
+            self.__name = configer.value.get('name')
+            self.__description = configer.value.get('description')
+            self.__ext_info = configer.value.get('ext_info')
         except Exception as e:
-            raise Exception(f"Failed to parse the Agent configuration: {e}")
+            raise Exception(f"Failed to parse the Knowledge configuration: {e}")
         return self
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 # @Time    : 2024/3/13 12:01
 # @Author  : jerry.zzw 
 # @Email   : jerry.zzw@antgroup.com
-# @FileName: knowledge_configer.py
-from typing import Optional, Dict
+# @FileName: tool_configer.py
+from typing import Optional, List
 from agentuniverse.base.config.component_configer.component_configer import ComponentConfiger
 from agentuniverse.base.config.configer import Configer
 
 
-class KnowledgeConfiger(ComponentConfiger):
-    """The KnowledgeConfiger class, which is used to load and manage the Knowledge configuration."""
+class ToolConfiger(ComponentConfiger):
+    """The ToolConfiger class, which is used to load and manage the Tool configuration."""
 
     def __init__(self, configer: Optional[Configer] = None):
-        """Initialize the KnowledgeConfiger."""
+        """Initialize the ToolConfiger."""
         super().__init__(configer)
         self.__name: Optional[str] = None
         self.__description: Optional[str] = None
-        self.__ext_info: Optional[Dict] = None
+        self.__tool_type: Optional[str] = None
+        self.__input_keys: Optional[List] = None
 
     @property
     def name(self) -> Optional[str]:
-        """Return the name of the Knowledge."""
+        """Return the name of the Tool."""
         return self.__name
 
     @property
     def description(self) -> Optional[str]:
-        """Return the description of the Knowledge."""
+        """Return the description of the Tool."""
         return self.__description
 
     @property
-    def ext_info(self) -> Optional[Dict]:
-        return self.__ext_info
+    def tool_type(self) -> Optional[str]:
+        return self.__tool_type
 
-    def load(self) -> 'KnowledgeConfiger':
+    @property
+    def input_keys(self) -> Optional[List]:
+        return self.__input_keys
+
+    def load(self) -> 'ToolConfiger':
         """Load the configuration by the Configer object.
         Returns:
-            KnowledgeConfiger: the KnowledgeConfiger object
+            ToolConfiger: the ToolConfiger object
         """
         return self.load_by_configer(self.__configer)
 
-    def load_by_configer(self, configer: Configer) -> 'KnowledgeConfiger':
+    def load_by_configer(self, configer: Configer) -> 'ToolConfiger':
         """Load the configuration by the Configer object.
         Args:
             configer(Configer): the Configer object
         Returns:
-            KnowledgeConfiger: the KnowledgeConfiger object
+            ToolConfiger: the ToolConfiger object
         """
         super().load_by_configer(configer)
 
         try:
             self.__name = configer.value.get('name')
             self.__description = configer.value.get('description')
-            self.__ext_info = configer.value.get('ext_info')
+            self.__tool_type = configer.value.get('tool_type')
+            self.__input_keys = configer.value.get('input_keys')
         except Exception as e:
-            raise Exception(f"Failed to parse the Knowledge configuration: {e}")
+            raise Exception(f"Failed to parse the Tool configuration: {e}")
         return self
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/configer.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,10 +154,10 @@
         """Load the yaml file.
 
         Args:
             path(str): the path of the yaml file
         Returns:
             dict: the value of the yaml file
         """
-        with open(path, 'r') as stream:
+        with open(path, 'r', encoding='utf-8') as stream:
             config_data = yaml.safe_load(stream)
         return config_data
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/context/framework_context.py` & `agentUniverse-0.0.4/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/context/framework_context_manager.py` & `agentUniverse-0.0.4/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/util/logging/general_logger.py` & `agentUniverse-0.0.4/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_config.py` & `agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_util.py` & `agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/base/util/prompt_util.py` & `agentUniverse-0.0.4/agentuniverse/base/util/prompt_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,55 @@
-from enum import Enum
+# !/usr/bin/env python3
+# -*- coding:utf-8 -*-
+
+# @Time    : 2024/4/16 14:42
+# @Author  : wangchongshi
+# @Email   : wangchongshi.wcs@antgroup.com
+# @FileName: prompt_util.py
+import asyncio
 from typing import List
+
 from langchain.chains.summarize import load_summarize_chain
-import asyncio
 from langchain_core.documents import Document
 from langchain_core.prompts import PromptTemplate
+
 from agentuniverse.llm.llm import LLM
 from agentuniverse.llm.llm_manager import LLMManager
+from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
+from agentuniverse.prompt.enum import PromptProcessEnum
 
 
-class PromptProcessEnum(Enum):
-    TRUNCATE = 'truncate'
-    STUFF = 'stuff'
-    MAP_REDUCE = 'map_reduce'
-
-    @classmethod
-    def from_value(cls, value):
-        for member in cls:
-            if member.value.lower() == value.lower():
-                return member
-        raise ValueError(f"No enum member with value: {value}")
-
-
-summarize_prompt_template = """
-写下这段文字的详细摘要，输出结果中需要涵盖文本的要点、数据以及任何重要的细节。
-注意：结果输出时必须用中文。
-{text}
-"""
-
-combine_prompt_template = """
-写出以下由三重反引号分隔的文本的详细摘要，输出结果中需要涵盖文本的要点、数据以及任何重要的细节。
-注意：结果输出时必须用中文。
-```{text}```
-"""
-
-summarize_prompt = PromptTemplate(template=summarize_prompt_template, input_variables=["text"])
-combine_prompt = PromptTemplate(template=combine_prompt_template, input_variables=["text"])
-
-
-def summarize_by_stuff(texts: List[str], llm: LLM):
+def summarize_by_stuff(texts: List[str], llm: LLM, summary_prompt_version: str):
     """
     stuff summarization -- general method
     """
-    stuff_chain = load_summarize_chain(llm.as_langchain(), chain_type='stuff', verbose=True, prompt=summarize_prompt)
+    summary_prompt = PromptManager().get_instance_obj(summary_prompt_version)
+    stuff_chain = load_summarize_chain(llm.as_langchain(), chain_type='stuff', verbose=True,
+                                       prompt=summary_prompt.as_langchain())
     return asyncio.run(stuff_chain.arun([Document(page_content=text) for text in texts]))
 
 
-def summarize_by_map_reduce(texts: List[str], llm: LLM, agent_llm: LLM):
+def summarize_by_map_reduce(texts: List[str], llm: LLM, agent_llm: LLM, summary_prompt_version: str,
+                            combine_prompt_version: str):
     """
     map reduce summarization -- general method
     """
     texts = split_texts(texts, agent_llm)
+    summary_prompt = PromptManager().get_instance_obj(summary_prompt_version)
+    combine_prompt = PromptManager().get_instance_obj(combine_prompt_version)
     map_reduce_chain = load_summarize_chain(llm.as_langchain(), chain_type='map_reduce', verbose=True,
-                                            map_prompt=summarize_prompt,
-                                            combine_prompt=combine_prompt)
+                                            map_prompt=summary_prompt.as_langchain(),
+                                            combine_prompt=combine_prompt.as_langchain())
     return asyncio.run(map_reduce_chain.arun([Document(page_content=text) for text in texts]))
 
 
 def split_text_on_tokens(text: str, text_token, chunk_size=800, chunk_overlap=100) -> List[str]:
     """Split incoming text and return chunks using tokenizer."""
-    # Calculate the number of characters represented by each token.
+    # calculate the number of characters represented by each token.
     char_per_token = len(text) / text_token
     chunk_char_size = int(chunk_size * char_per_token)
     chunk_char_overlap = int(chunk_overlap * char_per_token)
 
     result = []
     current_position = 0
 
@@ -81,17 +67,16 @@
 
 def split_texts(texts: list[str], agent_llm: LLM, chunk_size=800, chunk_overlap=100, retry=True) -> list[str]:
     """
     split texts into chunks with the fixed token length -- general method
     """
     try:
         split_texts_res = []
-        llm = agent_llm.as_langchain()
         for text in texts:
-            text_token = llm.get_num_tokens(text)
+            text_token = agent_llm.get_num_tokens(text)
             split_texts_res.extend(
                 split_text_on_tokens(text=text, text_token=text_token, chunk_size=chunk_size,
                                      chunk_overlap=chunk_overlap))
         return split_texts_res
     except Exception as e:
         if retry:
             return split_texts(texts=texts, agent_llm=agent_llm, retry=False)
@@ -130,33 +115,42 @@
         prompt_template (PromptTemplate): The prompt template.
         profile (dict): The profile.
         planner_input (dict): The planner input.
     """
     llm_model: dict = profile.get('llm_model')
     llm_name: str = llm_model.get('name')
 
+    # get the prompt processor configuration
     prompt_processor: dict = llm_model.get('prompt_processor') or dict()
     prompt_processor_type: str = prompt_processor.get('type') or PromptProcessEnum.TRUNCATE.value
     prompt_processor_llm: str = prompt_processor.get('llm') or llm_name
+
+    # get the summary and combine prompt versions
+    summary_prompt_version: str = prompt_processor.get('summary_prompt_version') or 'prompt_processor.summary_cn'
+    combine_prompt_version: str = prompt_processor.get('combine_prompt_version') or 'prompt_processor.combine_cn'
+
     prompt_input_dict = {key: planner_input[key] for key in prompt_template.input_variables if key in planner_input}
 
     agent_llm: LLM = LLMManager().get_instance_obj(llm_name)
-    llm_max_tokens: int = agent_llm.max_tokens
+    # get the llm instance for prompt compression
     prompt_llm: LLM = LLMManager().get_instance_obj(prompt_processor_llm)
 
     prompt = prompt_template.format(**prompt_input_dict)
-    prompt_token_length: int = len(prompt)
+    # get the number of tokens in the prompt
+    prompt_tokens: int = agent_llm.get_num_tokens(prompt)
 
-    if prompt_token_length <= llm_max_tokens:
-        return
+    remaining_tokens = agent_llm.max_context_length() - agent_llm.max_tokens
 
-    remaining_token_length: int = prompt_token_length - llm_max_tokens
+    if prompt_tokens <= remaining_tokens:
+        return
 
     process_prompt_type_enum = PromptProcessEnum.from_value(prompt_processor_type)
 
+    # compress the background in the prompt
     content = planner_input.get('background')
     if process_prompt_type_enum == PromptProcessEnum.TRUNCATE:
-        planner_input['background'] = truncate_content(content, remaining_token_length, agent_llm)
+        planner_input['background'] = truncate_content(content, remaining_tokens, agent_llm)
     elif process_prompt_type_enum == PromptProcessEnum.STUFF:
-        planner_input['background'] = summarize_by_stuff([content], prompt_llm)
+        planner_input['background'] = summarize_by_stuff([content], prompt_llm, summary_prompt_version)
     elif process_prompt_type_enum == PromptProcessEnum.MAP_REDUCE:
-        planner_input['background'] = summarize_by_map_reduce([content], prompt_llm, agent_llm)
+        planner_input['background'] = summarize_by_map_reduce([content], prompt_llm,
+                                                              agent_llm, summary_prompt_version, combine_prompt_version)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `agentUniverse-0.0.3/agentuniverse/base/util/system_util.py` & `agentUniverse-0.0.4/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/llm/default/default_openai_llm.py` & `agentUniverse-0.0.4/agentuniverse/llm/default/default_openai_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 class DefaultOpenAILLM(OpenAILLM):
     """The agentUniverse default openai llm module.
 
     LLM parameters, such as name/description/model_name/max_tokens,
     are injected into this class by the default_openai_llm.yaml configuration.
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
     def call(self, messages: list, **kwargs: Any) -> LLMOutput:
         """ The call method of the LLM.
 
         Users can customize how the model interacts by overriding call method of the LLM class.
 
         Args:
             messages (list): The messages to send to the LLM.
```

### Comparing `agentUniverse-0.0.3/agentuniverse/llm/langchain_instance.py` & `agentUniverse-0.0.4/agentuniverse/llm/langchain_instance.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,68 +5,67 @@
 # @Author  : wangchongshi
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: langchain_instance.py
 from typing import Any, List, Optional
 
 from langchain.callbacks.manager import AsyncCallbackManagerForLLMRun, CallbackManagerForLLMRun
 from langchain.chat_models import ChatOpenAI
-from langchain_community.chat_models.openai import acompletion_with_retry
 from langchain.schema import BaseMessage, ChatResult
 
 from agentuniverse.llm.llm import LLM
 
 
 class LangchainOpenAI(ChatOpenAI):
     """Langchain OpenAI LLM wrapper."""
 
+    llm: Optional[LLM] = None
+
     def __init__(self, llm: LLM):
         """The __init__ method.
 
         The agentUniverse LLM instance is passed to this class as an argument.
-        Convert the attributes of aU LLM instance to the LangchainOpenAI object for initialization
+        Convert the attributes of AgentUniverse(AU) LLM instance to the LangchainOpenAI object for initialization
 
         Args:
-            llm (LLM): the aU LLM instance.
+            llm (LLM): the AgentUniverse(AU) LLM instance.
         """
         init_params = dict()
         init_params['model_name'] = llm.model_name if llm.model_name is not None else 'gpt-3.5-turbo'
         init_params['temperature'] = llm.temperature if llm.temperature is not None else 0.7
         init_params['request_timeout'] = llm.request_timeout
         init_params['max_tokens'] = llm.max_tokens
         init_params['max_retries'] = llm.max_retries if llm.max_retries is not None else 2
         init_params['streaming'] = llm.streaming if llm.streaming is not None else False
         init_params['openai_api_key'] = llm.openai_api_key
         init_params['openai_organization'] = llm.openai_organization
         init_params['openai_api_base'] = llm.openai_api_base
+        init_params['openai_proxy'] = llm.openai_proxy
         super().__init__(**init_params)
+        self.llm = llm
 
     def _generate(
             self,
             messages: List[BaseMessage],
             stop: Optional[List[str]] = None,
             run_manager: Optional[CallbackManagerForLLMRun] = None,
             stream: Optional[bool] = None,
             **kwargs,
     ) -> ChatResult:
         """Run the Langchain OpenAI LLM."""
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs}
-        response = self.completion_with_retry(
-            messages=message_dicts, run_manager=run_manager, **params
-        )
-        return self._create_chat_result(response)
+        llm_output = self.llm.call(messages=message_dicts, **params)
+        return self._create_chat_result(llm_output.raw)
 
     async def _agenerate(
             self,
             messages: List[BaseMessage],
             stop: Optional[List[str]] = None,
             run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
             stream: Optional[bool] = None,
             **kwargs: Any,
     ) -> ChatResult:
         """Asynchronously run the Langchain OpenAI LLM."""
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs}
-        response = await acompletion_with_retry(
-            self, messages=message_dicts, **params
-        )
-        return self._create_chat_result(response)
+        llm_output = await self.llm.acall(messages=message_dicts, **params)
+        return self._create_chat_result(llm_output.raw)
```

### Comparing `agentUniverse-0.0.3/agentuniverse/llm/llm.py` & `agentUniverse-0.0.4/agentuniverse/llm/llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,7 +112,27 @@
             self.request_timeout = kwargs['request_timeout']
         if 'max_tokens' in kwargs and kwargs['max_tokens']:
             self.max_tokens = kwargs['max_tokens']
         if 'max_retries' in kwargs and kwargs['max_retries']:
             self.max_retries = kwargs['max_retries']
         if 'streaming' in kwargs and kwargs['streaming']:
             self.streaming = kwargs['streaming']
+
+    @abstractmethod
+    def max_context_length(self) -> int:
+        """Max context length.
+
+        The total length of input tokens and generated tokens is limited by the model's context length.
+        """
+
+    @abstractmethod
+    def get_num_tokens(self, text: str) -> int:
+        """Get the number of tokens present in the text.
+
+        Useful for checking if an input will fit in a model's context window.
+
+        Args:
+            text: The string input to tokenize.
+
+        Returns:
+            The integer number of tokens in the text.
+        """
```

### Comparing `agentUniverse-0.0.3/agentuniverse/llm/llm_manager.py` & `agentUniverse-0.0.4/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse/prompt/prompt.py` & `agentUniverse-0.0.4/agentuniverse/prompt/prompt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,82 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Time    : 2024/3/13 15:22
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: prompt_base.py
+# @FileName: prompt.py
 """Prompt base module."""
 import re
 from typing import Optional
 
 from langchain_core.prompts import PromptTemplate
 
 from agentuniverse.base.component.component_base import ComponentBase
 from agentuniverse.base.component.component_enum import ComponentEnum
+from agentuniverse.base.config.component_configer.configers.prompt_configer import PromptConfiger
 from agentuniverse.base.util.prompt_util import generate_template
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
 class Prompt(ComponentBase):
     """Prompt class."""
 
+    prompt_version: Optional[str] = None
     prompt_template: Optional[str] = None
     input_variables: Optional[list[str]] = None
-    component_type: ComponentEnum = ComponentEnum.DEFAULT
+
+    def __init__(self, **kwargs):
+        super().__init__(component_type=ComponentEnum.PROMPT, **kwargs)
 
     def as_langchain(self) -> PromptTemplate:
         """Convert the prompt template into a LangChain prompt template.
 
         Returns:
             PromptTemplate: The prompt template.
         """
         return PromptTemplate(template=self.prompt_template,
                               input_variables=self.input_variables)
 
-    def build_prompt_template(self, user_agent_prompt_model: AgentPromptModel,
-                              system_agent_prompt_model: AgentPromptModel,
-                              prompt_assemble_order: list[str]):
-        """Build the prompt template.
+    def build_prompt(self, user_agent_prompt_model: AgentPromptModel, system_agent_prompt_model: AgentPromptModel,
+                     prompt_assemble_order: list[str]):
+        """Build the prompt class.
 
         Args:
             user_agent_prompt_model (AgentPromptModel): The user agent prompt model.
             system_agent_prompt_model (AgentPromptModel): The system agent prompt model.
             prompt_assemble_order (list[str]): The prompt assemble ordered list.
 
         Returns:
             PromptTemplate: The prompt template.
         """
         agent_prompt_model = user_agent_prompt_model + system_agent_prompt_model
         self.prompt_template = generate_template(agent_prompt_model, prompt_assemble_order)
         self.input_variables = re.findall(r'\{(.*?)}', self.prompt_template)
+
+    def get_instance_code(self) -> str:
+        """Return the prompt version of the current prompt."""
+        return self.prompt_version
+
+    def initialize_by_component_configer(self, component_configer: PromptConfiger) -> 'Prompt':
+        """Initialize the prompt by the PromptConfiger object.
+
+        Args:
+            component_configer(PromptConfiger): the PromptConfiger object
+        Returns:
+            Prompt: the prompt object
+        """
+        prompt_values = []
+        for k, v in component_configer.configer.value.items():
+            # ignore metadata values
+            if k == 'metadata':
+                continue
+            self.__dict__[k] = v
+            # splice the values in the prompt configer
+            prompt_values.append(str(v))
+
+        if component_configer.metadata_version:
+            self.prompt_version = component_configer.metadata_version
+
+        self.prompt_template = '\n'.join(prompt_values)
+
+        self.input_variables = re.findall(r'\{(.*?)}', self.prompt_template)
+        return self
```

### Comparing `agentUniverse-0.0.3/agentuniverse/prompt/prompt_model.py` & `agentUniverse-0.0.4/agentuniverse/prompt/prompt_model.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/agentuniverse_extension/logger/sls_sink.py` & `agentUniverse-0.0.4/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/pyproject.toml` & `agentUniverse-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentUniverse"
-version = "0.0.2"
+version = "0.0.4"
 description = "agentUniverse is a framework for developing applications powered by multi-agent base on large language model."
 authors = ["AntGroup <AntGroup>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
@@ -19,18 +19,21 @@
 flask_cors = '4.0.0'
 SQLAlchemy = '2.0.25'
 pydantic = "^2.6.4"
 gunicorn = "21.2.0"
 chromadb = "0.4.24"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
-aliyun-log-python-sdk = "0.8.8"
+aliyun-log-python-sdk = { version = "0.8.8", optional = true}
 googleapis-common-protos = "^1.63.0"
 myst-parser = "^2.0.0"
 
+[tool.poetry.extras]
+log_ext = ["aliyun-log-python-sdk"]
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.6.4"
 pre-commit = "^2.20.0"
```

### Comparing `agentUniverse-0.0.3/setup.py` & `agentUniverse-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setuptools.setup(
     name="agentUniverse",
-    version="0.0.3",
+    version="0.0.4",
     author="AntGroup",
     author_email="jerry.zzw@antgroup.com",
     description="agentUniverse is a framework for developing applications powered "
                 "by multi-agent base on large language model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/agentUniverse/agentUniverse",
```

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_agent.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/test_memory.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/test_memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/test_agent.py` & `agentUniverse-0.0.4/sample_standard_app/app/test/test_rag_agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 15:27
-# @Author  : heji
-# @Email   : lc299034@antgroup.com
-# @FileName: test_agent.py
+
+# @Time    : 2024/4/1 14:32
+# @Author  : wangchongshi
+# @Email   : wangchongshi.wcs@antgroup.com
+# @FileName: test_rag_agent.py
 import unittest
 
 from agentuniverse.agent.agent import Agent
 from agentuniverse.agent.agent_manager import AgentManager
 from agentuniverse.agent.output_object import OutputObject
 from agentuniverse.base.agentuniverse import AgentUniverse
 
-AgentUniverse().start(config_path='./config.toml')
 
+class RagAgentTest(unittest.TestCase):
+    """
+    Test cases for the rag agent
+    """
 
-class TestAgent(unittest.TestCase):
+    def setUp(self) -> None:
+        AgentUniverse().start(config_path='../../config/config.toml')
 
     def test_rag_agent(self):
-        instance: Agent = AgentManager().get_instance_obj('rag_agent')
-        output_object: OutputObject = instance.run(input='分析下先锋领航退出中国的原因')
+        """Test demo rag agent."""
+        instance: Agent = AgentManager().get_instance_obj('demo_rag_agent')
+        output_object: OutputObject = instance.run(input='英伟达股票大涨原因是什么？')
         print(output_object.get_data('output'))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/test_framework_context.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/test_framework_context.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/test_llm.py` & `agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/test_llm.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py` & `agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py` & `agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py`

 * *Files identical despite different names*

