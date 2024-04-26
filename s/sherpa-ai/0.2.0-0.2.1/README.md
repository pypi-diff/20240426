# Comparing `tmp/sherpa_ai-0.2.0.tar.gz` & `tmp/sherpa_ai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa_ai-0.2.0.tar", max compression
+gzip compressed data, was "sherpa_ai-0.2.1.tar", max compression
```

## Comparing `sherpa_ai-0.2.0.tar` & `sherpa_ai-0.2.1.tar`

### file list

```diff
@@ -1,68 +1,71 @@
--rw-r--r--   0        0        0     1281 2024-04-04 20:47:37.185107 sherpa_ai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-09-07 18:58:13.889346 sherpa_ai-0.2.0/README.md
--rw-r--r--   0        0        0       23 2023-09-07 18:58:13.896351 sherpa_ai-0.2.0/sherpa_ai/__init__.py
--rw-r--r--   0        0        0      203 2023-10-22 21:42:20.082581 sherpa_ai-0.2.0/sherpa_ai/action_planner/__init__.py
--rw-r--r--   0        0        0     3888 2023-12-19 19:27:04.507940 sherpa_ai-0.2.0/sherpa_ai/action_planner/action_planner.py
--rw-r--r--   0        0        0      285 2023-12-19 19:27:04.507940 sherpa_ai-0.2.0/sherpa_ai/action_planner/base.py
--rw-r--r--   0        0        0     1427 2023-11-22 04:28:04.077007 sherpa_ai-0.2.0/sherpa_ai/action_planner/selective_planner.py
--rw-r--r--   0        0        0       66 2023-10-22 21:42:20.092581 sherpa_ai-0.2.0/sherpa_ai/action_planner/simple_planner.py
--rw-r--r--   0        0        0      409 2024-04-04 20:46:01.175058 sherpa_ai-0.2.0/sherpa_ai/actions/__init__.py
--rw-r--r--   0        0        0     1684 2024-02-28 14:01:30.482499 sherpa_ai-0.2.0/sherpa_ai/actions/arxiv_search.py
--rw-r--r--   0        0        0      482 2023-12-19 19:27:04.509940 sherpa_ai-0.2.0/sherpa_ai/actions/base.py
--rw-r--r--   0        0        0     1787 2023-12-19 19:27:04.510941 sherpa_ai-0.2.0/sherpa_ai/actions/context_search.py
--rw-r--r--   0        0        0     1331 2023-12-19 19:27:04.510941 sherpa_ai-0.2.0/sherpa_ai/actions/deliberation.py
--rw-r--r--   0        0        0     2918 2024-02-28 14:01:30.482499 sherpa_ai-0.2.0/sherpa_ai/actions/google_search.py
--rw-r--r--   0        0        0     5641 2023-12-19 19:27:04.512941 sherpa_ai-0.2.0/sherpa_ai/actions/planning.py
--rw-r--r--   0        0        0     1918 2024-03-01 16:22:17.952293 sherpa_ai-0.2.0/sherpa_ai/actions/synthesize.py
--rw-r--r--   0        0        0      493 2024-02-20 04:55:11.807341 sherpa_ai-0.2.0/sherpa_ai/agents/__init__.py
--rw-r--r--   0        0        0     1177 2023-11-22 02:47:37.184142 sherpa_ai-0.2.0/sherpa_ai/agents/agent_pool.py
--rw-r--r--   0        0        0     4886 2024-03-01 16:17:05.632211 sherpa_ai-0.2.0/sherpa_ai/agents/base.py
--rw-r--r--   0        0        0     5146 2023-12-19 19:27:04.514940 sherpa_ai-0.2.0/sherpa_ai/agents/critic.py
--rw-r--r--   0        0        0     2895 2024-02-28 14:01:30.483423 sherpa_ai-0.2.0/sherpa_ai/agents/ml_engineer.py
--rw-r--r--   0        0        0     2581 2024-02-28 14:01:30.483423 sherpa_ai-0.2.0/sherpa_ai/agents/physicist.py
--rw-r--r--   0        0        0     2849 2023-12-19 19:27:04.515940 sherpa_ai-0.2.0/sherpa_ai/agents/planner.py
--rw-r--r--   0        0        0     4838 2024-02-28 14:01:30.483423 sherpa_ai-0.2.0/sherpa_ai/agents/qa_agent.py
--rw-r--r--   0        0        0     1665 2023-10-22 21:42:20.116222 sherpa_ai-0.2.0/sherpa_ai/agents/user.py
--rw-r--r--   0        0        0     3905 2024-04-04 20:44:04.473809 sherpa_ai-0.2.0/sherpa_ai/config/__init__.py
--rw-r--r--   0        0        0     3025 2024-01-17 05:47:33.698412 sherpa_ai-0.2.0/sherpa_ai/config/task_config.py
--rw-r--r--   0        0        0     1424 2023-09-14 14:00:23.450118 sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/load_dump_to_chroma.py
--rw-r--r--   0        0        0     1249 2023-09-14 14:00:23.451116 sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/query_chroma.py
--rw-r--r--   0        0        0     6843 2024-02-07 04:00:13.352018 sherpa_ai-0.2.0/sherpa_ai/connectors/vectorstores.py
--rw-r--r--   0        0        0      102 2023-09-07 18:58:13.900426 sherpa_ai-0.2.0/sherpa_ai/database/__init__.py
--rw-r--r--   0        0        0    15220 2024-03-07 04:24:18.868368 sherpa_ai-0.2.0/sherpa_ai/database/user_usage_tracker.py
--rw-r--r--   0        0        0      111 2023-09-07 18:58:13.901553 sherpa_ai-0.2.0/sherpa_ai/error_handling/__init__.py
--rw-r--r--   0        0        0     1762 2023-09-07 18:58:13.901553 sherpa_ai-0.2.0/sherpa_ai/error_handling/agent_error_handler.py
--rw-r--r--   0        0        0      841 2024-04-04 20:44:04.474845 sherpa_ai-0.2.0/sherpa_ai/events.py
--rw-r--r--   0        0        0      141 2023-10-22 21:42:20.118096 sherpa_ai-0.2.0/sherpa_ai/memory/__init__.py
--rw-r--r--   0        0        0     5423 2024-04-04 20:44:04.475878 sherpa_ai-0.2.0/sherpa_ai/memory/belief.py
--rw-r--r--   0        0        0     2171 2024-02-28 14:01:30.484418 sherpa_ai-0.2.0/sherpa_ai/memory/shared_memory.py
--rw-r--r--   0        0        0      181 2023-09-07 18:58:13.902558 sherpa_ai-0.2.0/sherpa_ai/models/__init__.py
--rw-r--r--   0        0        0     2066 2024-02-15 02:06:06.152905 sherpa_ai-0.2.0/sherpa_ai/models/chat_model_with_logging.py
--rw-r--r--   0        0        0     3224 2024-02-20 04:55:11.812339 sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_chat_model.py
--rw-r--r--   0        0        0     1510 2024-04-03 04:17:33.589955 sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_model.py
--rw-r--r--   0        0        0     4402 2023-10-22 21:42:20.122097 sherpa_ai-0.2.0/sherpa_ai/orchestrator.py
--rw-r--r--   0        0        0     1616 2023-09-07 18:58:13.904341 sherpa_ai-0.2.0/sherpa_ai/output_parser.py
--rw-r--r--   0        0        0      474 2024-02-28 14:01:30.485416 sherpa_ai-0.2.0/sherpa_ai/output_parsers/__init__.py
--rw-r--r--   0        0        0     1953 2024-02-28 14:01:30.485416 sherpa_ai-0.2.0/sherpa_ai/output_parsers/base.py
--rw-r--r--   0        0        0    11349 2024-04-03 04:17:33.589955 sherpa_ai-0.2.0/sherpa_ai/output_parsers/citation_validation.py
--rw-r--r--   0        0        0     4165 2024-02-15 02:06:06.155286 sherpa_ai-0.2.0/sherpa_ai/output_parsers/link_parse.py
--rw-r--r--   0        0        0     1485 2024-02-15 02:06:06.155286 sherpa_ai-0.2.0/sherpa_ai/output_parsers/md_to_slack_parse.py
--rw-r--r--   0        0        0     2062 2024-04-04 20:47:25.540942 sherpa_ai-0.2.0/sherpa_ai/output_parsers/number_validation.py
--rw-r--r--   0        0        0      715 2024-04-03 04:17:33.590956 sherpa_ai-0.2.0/sherpa_ai/output_parsers/validation_result.py
--rw-r--r--   0        0        0      274 2023-09-07 18:58:13.905751 sherpa_ai-0.2.0/sherpa_ai/post_processors.py
--rw-r--r--   0        0        0     2834 2024-02-15 02:06:06.156687 sherpa_ai-0.2.0/sherpa_ai/prompt.py
--rw-r--r--   0        0        0     6810 2023-09-07 18:58:13.906764 sherpa_ai-0.2.0/sherpa_ai/prompt_generator.py
--rw-r--r--   0        0        0     2700 2023-09-07 18:58:13.906764 sherpa_ai-0.2.0/sherpa_ai/reflection.py
--rw-r--r--   0        0        0     3226 2024-03-07 04:24:18.869369 sherpa_ai-0.2.0/sherpa_ai/scrape/extract_github_readme.py
--rw-r--r--   0        0        0     5252 2024-04-03 04:17:33.591954 sherpa_ai-0.2.0/sherpa_ai/scrape/file_scraper.py
--rw-r--r--   0        0        0     3588 2024-04-03 04:17:33.591954 sherpa_ai-0.2.0/sherpa_ai/scrape/prompt_reconstructor.py
--rw-r--r--   0        0        0    10509 2024-02-15 02:06:06.156687 sherpa_ai-0.2.0/sherpa_ai/task_agent.py
--rw-r--r--   0        0        0      327 2024-02-28 14:01:30.486415 sherpa_ai-0.2.0/sherpa_ai/test_utils/data.py
--rw-r--r--   0        0        0     1752 2024-03-07 05:54:44.991058 sherpa_ai-0.2.0/sherpa_ai/test_utils/llms.py
--rw-r--r--   0        0        0      755 2023-12-19 20:27:38.204282 sherpa_ai-0.2.0/sherpa_ai/test_utils/loggers.py
--rw-r--r--   0        0        0    10071 2024-02-07 04:00:13.356017 sherpa_ai-0.2.0/sherpa_ai/tools.py
--rw-r--r--   0        0        0    13170 2024-04-04 20:47:25.541939 sherpa_ai-0.2.0/sherpa_ai/utils.py
--rw-r--r--   0        0        0      238 2024-02-15 02:06:06.158160 sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/__init__.py
--rw-r--r--   0        0        0      141 2023-09-07 18:58:13.910518 sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/base.py
--rw-r--r--   0        0        0     1012 2023-11-20 05:23:41.530778 sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/verbose_loggers.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 sherpa_ai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1279 2024-04-24 02:25:14.174706 sherpa_ai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-09-07 18:58:13.889346 sherpa_ai-0.2.1/README.md
+-rw-r--r--   0        0        0       23 2023-09-07 18:58:13.896351 sherpa_ai-0.2.1/sherpa_ai/__init__.py
+-rw-r--r--   0        0        0      203 2023-10-22 21:42:20.082581 sherpa_ai-0.2.1/sherpa_ai/action_planner/__init__.py
+-rw-r--r--   0        0        0     3888 2023-12-19 19:27:04.507940 sherpa_ai-0.2.1/sherpa_ai/action_planner/action_planner.py
+-rw-r--r--   0        0        0      285 2023-12-19 19:27:04.507940 sherpa_ai-0.2.1/sherpa_ai/action_planner/base.py
+-rw-r--r--   0        0        0     1427 2023-11-22 04:28:04.077007 sherpa_ai-0.2.1/sherpa_ai/action_planner/selective_planner.py
+-rw-r--r--   0        0        0       66 2023-10-22 21:42:20.092581 sherpa_ai-0.2.1/sherpa_ai/action_planner/simple_planner.py
+-rw-r--r--   0        0        0      409 2024-04-11 01:46:59.690575 sherpa_ai-0.2.1/sherpa_ai/actions/__init__.py
+-rw-r--r--   0        0        0     1684 2024-02-28 14:01:30.482499 sherpa_ai-0.2.1/sherpa_ai/actions/arxiv_search.py
+-rw-r--r--   0        0        0      482 2023-12-19 19:27:04.509940 sherpa_ai-0.2.1/sherpa_ai/actions/base.py
+-rw-r--r--   0        0        0     1787 2023-12-19 19:27:04.510941 sherpa_ai-0.2.1/sherpa_ai/actions/context_search.py
+-rw-r--r--   0        0        0     1331 2023-12-19 19:27:04.510941 sherpa_ai-0.2.1/sherpa_ai/actions/deliberation.py
+-rw-r--r--   0        0        0     2918 2024-02-28 14:01:30.482499 sherpa_ai-0.2.1/sherpa_ai/actions/google_search.py
+-rw-r--r--   0        0        0     5641 2023-12-19 19:27:04.512941 sherpa_ai-0.2.1/sherpa_ai/actions/planning.py
+-rw-r--r--   0        0        0     1918 2024-03-01 16:22:17.952293 sherpa_ai-0.2.1/sherpa_ai/actions/synthesize.py
+-rw-r--r--   0        0        0      493 2024-02-20 04:55:11.807341 sherpa_ai-0.2.1/sherpa_ai/agents/__init__.py
+-rw-r--r--   0        0        0     1177 2023-11-22 02:47:37.184142 sherpa_ai-0.2.1/sherpa_ai/agents/agent_pool.py
+-rw-r--r--   0        0        0     4886 2024-03-01 16:17:05.632211 sherpa_ai-0.2.1/sherpa_ai/agents/base.py
+-rw-r--r--   0        0        0     5146 2023-12-19 19:27:04.514940 sherpa_ai-0.2.1/sherpa_ai/agents/critic.py
+-rw-r--r--   0        0        0     2895 2024-02-28 14:01:30.483423 sherpa_ai-0.2.1/sherpa_ai/agents/ml_engineer.py
+-rw-r--r--   0        0        0     2581 2024-02-28 14:01:30.483423 sherpa_ai-0.2.1/sherpa_ai/agents/physicist.py
+-rw-r--r--   0        0        0     2849 2023-12-19 19:27:04.515940 sherpa_ai-0.2.1/sherpa_ai/agents/planner.py
+-rw-r--r--   0        0        0     4838 2024-04-08 03:33:58.816371 sherpa_ai-0.2.1/sherpa_ai/agents/qa_agent.py
+-rw-r--r--   0        0        0     1665 2023-10-22 21:42:20.116222 sherpa_ai-0.2.1/sherpa_ai/agents/user.py
+-rw-r--r--   0        0        0     3984 2024-04-24 02:25:02.470359 sherpa_ai-0.2.1/sherpa_ai/config/__init__.py
+-rw-r--r--   0        0        0     3025 2024-01-17 05:47:33.698412 sherpa_ai-0.2.1/sherpa_ai/config/task_config.py
+-rw-r--r--   0        0        0     4220 2024-04-24 02:25:02.472359 sherpa_ai-0.2.1/sherpa_ai/connectors/chroma_vector_store.py
+-rw-r--r--   0        0        0     2547 2024-04-24 02:25:02.470359 sherpa_ai-0.2.1/sherpa_ai/connectors/ChromaVectorStore.py
+-rw-r--r--   0        0        0     1424 2023-09-14 14:00:23.450118 sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/load_dump_to_chroma.py
+-rw-r--r--   0        0        0     1249 2023-09-14 14:00:23.451116 sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/query_chroma.py
+-rw-r--r--   0        0        0     6843 2024-02-07 04:00:13.352018 sherpa_ai-0.2.1/sherpa_ai/connectors/vectorstores.py
+-rw-r--r--   0        0        0      102 2023-09-07 18:58:13.900426 sherpa_ai-0.2.1/sherpa_ai/database/__init__.py
+-rw-r--r--   0        0        0    15320 2024-04-24 02:25:02.475359 sherpa_ai-0.2.1/sherpa_ai/database/user_usage_tracker.py
+-rw-r--r--   0        0        0      111 2023-09-07 18:58:13.901553 sherpa_ai-0.2.1/sherpa_ai/error_handling/__init__.py
+-rw-r--r--   0        0        0     1762 2023-09-07 18:58:13.901553 sherpa_ai-0.2.1/sherpa_ai/error_handling/agent_error_handler.py
+-rw-r--r--   0        0        0      861 2024-04-24 02:25:02.476359 sherpa_ai-0.2.1/sherpa_ai/events.py
+-rw-r--r--   0        0        0      141 2023-10-22 21:42:20.118096 sherpa_ai-0.2.1/sherpa_ai/memory/__init__.py
+-rw-r--r--   0        0        0     5441 2024-04-24 02:25:02.479359 sherpa_ai-0.2.1/sherpa_ai/memory/belief.py
+-rw-r--r--   0        0        0     2171 2024-02-28 14:01:30.484418 sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory.py
+-rw-r--r--   0        0        0     2170 2024-04-24 02:25:02.481359 sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory_with_vectordb.py
+-rw-r--r--   0        0        0      181 2023-09-07 18:58:13.902558 sherpa_ai-0.2.1/sherpa_ai/models/__init__.py
+-rw-r--r--   0        0        0     2066 2024-02-15 02:06:06.152905 sherpa_ai-0.2.1/sherpa_ai/models/chat_model_with_logging.py
+-rw-r--r--   0        0        0     3224 2024-02-20 04:55:11.812339 sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_chat_model.py
+-rw-r--r--   0        0        0     1510 2024-04-03 04:17:33.589955 sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_model.py
+-rw-r--r--   0        0        0     4402 2023-10-22 21:42:20.122097 sherpa_ai-0.2.1/sherpa_ai/orchestrator.py
+-rw-r--r--   0        0        0     1616 2023-09-07 18:58:13.904341 sherpa_ai-0.2.1/sherpa_ai/output_parser.py
+-rw-r--r--   0        0        0      474 2024-02-28 14:01:30.485416 sherpa_ai-0.2.1/sherpa_ai/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1953 2024-02-28 14:01:30.485416 sherpa_ai-0.2.1/sherpa_ai/output_parsers/base.py
+-rw-r--r--   0        0        0    11374 2024-04-24 02:25:02.483363 sherpa_ai-0.2.1/sherpa_ai/output_parsers/citation_validation.py
+-rw-r--r--   0        0        0     4165 2024-02-15 02:06:06.155286 sherpa_ai-0.2.1/sherpa_ai/output_parsers/link_parse.py
+-rw-r--r--   0        0        0     1485 2024-02-15 02:06:06.155286 sherpa_ai-0.2.1/sherpa_ai/output_parsers/md_to_slack_parse.py
+-rw-r--r--   0        0        0     2062 2024-04-04 20:47:25.540942 sherpa_ai-0.2.1/sherpa_ai/output_parsers/number_validation.py
+-rw-r--r--   0        0        0      715 2024-04-03 04:17:33.590956 sherpa_ai-0.2.1/sherpa_ai/output_parsers/validation_result.py
+-rw-r--r--   0        0        0      274 2023-09-07 18:58:13.905751 sherpa_ai-0.2.1/sherpa_ai/post_processors.py
+-rw-r--r--   0        0        0     2834 2024-02-15 02:06:06.156687 sherpa_ai-0.2.1/sherpa_ai/prompt.py
+-rw-r--r--   0        0        0     6810 2023-09-07 18:58:13.906764 sherpa_ai-0.2.1/sherpa_ai/prompt_generator.py
+-rw-r--r--   0        0        0     2700 2023-09-07 18:58:13.906764 sherpa_ai-0.2.1/sherpa_ai/reflection.py
+-rw-r--r--   0        0        0     3226 2024-03-07 04:24:18.869369 sherpa_ai-0.2.1/sherpa_ai/scrape/extract_github_readme.py
+-rw-r--r--   0        0        0     5252 2024-04-03 04:17:33.591954 sherpa_ai-0.2.1/sherpa_ai/scrape/file_scraper.py
+-rw-r--r--   0        0        0     3588 2024-04-03 04:17:33.591954 sherpa_ai-0.2.1/sherpa_ai/scrape/prompt_reconstructor.py
+-rw-r--r--   0        0        0    10509 2024-02-15 02:06:06.156687 sherpa_ai-0.2.1/sherpa_ai/task_agent.py
+-rw-r--r--   0        0        0      327 2024-02-28 14:01:30.486415 sherpa_ai-0.2.1/sherpa_ai/test_utils/data.py
+-rw-r--r--   0        0        0     1752 2024-03-07 05:54:44.991058 sherpa_ai-0.2.1/sherpa_ai/test_utils/llms.py
+-rw-r--r--   0        0        0      755 2023-12-19 20:27:38.204282 sherpa_ai-0.2.1/sherpa_ai/test_utils/loggers.py
+-rw-r--r--   0        0        0    10200 2024-04-16 16:58:00.924883 sherpa_ai-0.2.1/sherpa_ai/tools.py
+-rw-r--r--   0        0        0    13170 2024-04-04 20:47:25.541939 sherpa_ai-0.2.1/sherpa_ai/utils.py
+-rw-r--r--   0        0        0      238 2024-02-15 02:06:06.158160 sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/__init__.py
+-rw-r--r--   0        0        0      141 2023-09-07 18:58:13.910518 sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/base.py
+-rw-r--r--   0        0        0     1012 2023-11-20 05:23:41.530778 sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/verbose_loggers.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 sherpa_ai-0.2.1/PKG-INFO
```

### Comparing `sherpa_ai-0.2.0/pyproject.toml` & `sherpa_ai-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sherpa-ai"
-version = "0.2.0"
+version = "0.2.1"
 description = "Sherpa: AI-augmented thinking companion"
 authors = []
 readme = "README.md"
 repository = "https://github.com/Aggregate-Intellect/sherpa"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -22,15 +22,14 @@
 pypdf = "^3.17.0"
 transformers = "^4.35.2"
 pydantic = "^2.5.3"
 hydra-core = "^1.3.2"
 word2number = "^1.1"
 spacy = "^3.7.4"
 
-
 [tool.poetry.group.test.dependencies]
 pytest = "7.4.0"
 pytest-cov = "^4.1.0"
 
 
 [tool.poetry.group.lint.dependencies]
 black = "23.7.0"
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/action_planner/action_planner.py` & `sherpa_ai-0.2.1/sherpa_ai/action_planner/action_planner.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/action_planner/selective_planner.py` & `sherpa_ai-0.2.1/sherpa_ai/action_planner/selective_planner.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/actions/arxiv_search.py` & `sherpa_ai-0.2.1/sherpa_ai/actions/arxiv_search.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/actions/context_search.py` & `sherpa_ai-0.2.1/sherpa_ai/actions/context_search.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/actions/deliberation.py` & `sherpa_ai-0.2.1/sherpa_ai/actions/deliberation.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/actions/google_search.py` & `sherpa_ai-0.2.1/sherpa_ai/actions/google_search.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/actions/planning.py` & `sherpa_ai-0.2.1/sherpa_ai/actions/planning.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/actions/synthesize.py` & `sherpa_ai-0.2.1/sherpa_ai/actions/synthesize.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/agent_pool.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/agent_pool.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/base.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/base.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/critic.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/critic.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/ml_engineer.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/ml_engineer.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/physicist.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/physicist.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/planner.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/planner.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/qa_agent.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/qa_agent.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/agents/user.py` & `sherpa_ai-0.2.1/sherpa_ai/agents/user.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/config/__init__.py` & `sherpa_ai-0.2.1/sherpa_ai/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 TEMPERATURE = environ.get("TEMPERATURE") or 0
 
 # Pinecone settings
 PINECONE_API_KEY = environ.get("PINECONE_API_KEY")
 PINECONE_NAMESPACE = environ.get("PINECONE_NAMESPACE", "ReadTheDocs")
 PINECONE_ENV = environ.get("PINECONE_ENV")
 PINECONE_INDEX = environ.get("PINECONE_INDEX")
+INDEX_NAME_FILE_STORAGE = environ.get("INDEX_NAME_FILE_STORAGE", "sherpa_db")
 
 # Chroma settings
 CHROMA_HOST = environ.get("CHROMA_HOST")
 CHROMA_PORT = environ.get("CHROMA_PORT")
 CHROMA_INDEX = environ.get("CHROMA_INDEX")
 
 SERPER_API_KEY = environ.get("SERPER_API_KEY")
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/config/task_config.py` & `sherpa_ai-0.2.1/sherpa_ai/config/task_config.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/load_dump_to_chroma.py` & `sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/load_dump_to_chroma.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/query_chroma.py` & `sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/query_chroma.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/connectors/vectorstores.py` & `sherpa_ai-0.2.1/sherpa_ai/connectors/vectorstores.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/database/user_usage_tracker.py` & `sherpa_ai-0.2.1/sherpa_ai/database/user_usage_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 import time
 
 import boto3
 from anyio import Path
 from sqlalchemy import TIMESTAMP, Boolean, Column, Integer, String, create_engine
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
+from sqlalchemy import Boolean, Column, Integer, String, create_engine
+from sqlalchemy.orm import declarative_base, sessionmaker
 
 import sherpa_ai.config as cfg
 from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
-Base = declarative_base()
-
 import boto3
+import sqlalchemy.orm
+Base = sqlalchemy.orm.declarative_base()
 
 
 class UsageTracker(Base):
-
     """SQLAlchemy base model for tracking LLM token usage on per-user basis"""
 
     __tablename__ = "usage_tracker"
     id = Column(Integer, primary_key=True, autoincrement=True)
     user_id = Column(String)
     token = Column(Integer)
     timestamp = Column(Integer)
     reset_timestamp = Column(Boolean)
     reminded_timestamp = Column(Boolean)
 
 
 class Whitelist(Base):
-
     """Represents a trusted list of users whose usage is not tracked"""
 
     __tablename__ = "whitelist"
 
     id = Column(Integer, primary_key=True, autoincrement=True)
     user_id = Column(String)
 
 
 class UserUsageTracker:
-
     """Enables an app to track LLM token usage on per-user basis"""
 
     def __init__(
         self,
         db_name=cfg.DB_NAME,
         verbose_logger: BaseVerboseLogger = DummyVerboseLogger(),
     ):
@@ -110,15 +108,14 @@
         if not cfg.FLASK_DEBUG:
             self.upload_to_s3(
                 "./token_counter.db", "sherpa-sqlight", "token_counter.db"
             )
 
     def get_all_whitelisted_ids(self):
         """Get a list of all user IDs in the whitelist."""
-
         whitelisted_ids = [user.user_id for user in self.session.query(Whitelist).all()]
         return whitelisted_ids
 
     def get_whitelist_by_user_id(self, user_id):
         """
         Get whitelist information for a specific user.
 
@@ -371,15 +368,14 @@
         Returns:
             dict: Result containing information about tokens remaining,
                   whether more tokens can be consumed (can_excute),
                   any associated message, and the time left.
         """
 
         user_is_whitelisted = self.is_in_whitelist(user_id)
-
         if user_is_whitelisted:
             return {
                 "token-left": self.max_daily_token,
                 "can_excute": True,
                 "message": "",
                 "time_left": "",
             }
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/error_handling/agent_error_handler.py` & `sherpa_ai-0.2.1/sherpa_ai/error_handling/agent_error_handler.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/events.py` & `sherpa_ai-0.2.1/sherpa_ai/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class EventType(Enum):
     planning = 1
     task = 2
     result = 3
     feedback = 4
     action = 5
     action_output = 6
+    user_input = 7
 
 
 class Event:
     def __init__(self, event_type: EventType, agent: str, content: str) -> None:
         self.event_type = event_type
         self.agent = agent
         self.content = content
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/memory/belief.py` & `sherpa_ai-0.2.1/sherpa_ai/memory/belief.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,19 @@
             max_tokens: Maximum number of tokens
 
         Returns:
             str: Context of the agent
         """
         context = ""
         for event in reversed(self.events):
-            if (
-                event.event_type == EventType.task
-                or event.event_type == EventType.result
-            ):
+            if event.event_type in [
+                EventType.task,
+                EventType.result,
+                EventType.user_input,
+            ]:
                 context = event.content + "\n" + context
 
                 if token_counter(context) > max_tokens:
                     break
 
         if context == "":
             exit(1)
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/memory/shared_memory.py` & `sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/models/chat_model_with_logging.py` & `sherpa_ai-0.2.1/sherpa_ai/models/chat_model_with_logging.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_chat_model.py` & `sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_chat_model.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_model.py` & `sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_model.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/orchestrator.py` & `sherpa_ai-0.2.1/sherpa_ai/orchestrator.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parser.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parser.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parsers/base.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parsers/citation_validation.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parsers/citation_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     def resources_from_belief(self, belief: Belief) -> list[dict]:
         """
         Returns a list of all resources within belief.actions.
         """
         resources = []
         for action in belief.actions:
-            if hasattr(action, "meta") and action.meta is not None:
+            if hasattr(action, "meta") and action.meta is not None and len(action.meta) > 0:
                 resources.extend(action.meta[-1])
         return resources
 
     def process_output(self, text: str, belief: Belief) -> ValidationResult:
         """
          Add citations to sentences in the generated text using resources based on fact checking model.
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parsers/link_parse.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parsers/link_parse.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parsers/md_to_slack_parse.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parsers/md_to_slack_parse.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parsers/number_validation.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parsers/number_validation.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/output_parsers/validation_result.py` & `sherpa_ai-0.2.1/sherpa_ai/output_parsers/validation_result.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/prompt.py` & `sherpa_ai-0.2.1/sherpa_ai/prompt.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/prompt_generator.py` & `sherpa_ai-0.2.1/sherpa_ai/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/reflection.py` & `sherpa_ai-0.2.1/sherpa_ai/reflection.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/scrape/extract_github_readme.py` & `sherpa_ai-0.2.1/sherpa_ai/scrape/extract_github_readme.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/scrape/file_scraper.py` & `sherpa_ai-0.2.1/sherpa_ai/scrape/file_scraper.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/scrape/prompt_reconstructor.py` & `sherpa_ai-0.2.1/sherpa_ai/scrape/prompt_reconstructor.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/task_agent.py` & `sherpa_ai-0.2.1/sherpa_ai/task_agent.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/test_utils/llms.py` & `sherpa_ai-0.2.1/sherpa_ai/test_utils/llms.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/test_utils/loggers.py` & `sherpa_ai-0.2.1/sherpa_ai/test_utils/loggers.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/tools.py` & `sherpa_ai-0.2.1/sherpa_ai/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     def _run(
         self, query: str, require_meta=False
     ) -> Union[str, Tuple[str, List[dict]]]:
         result = ""
         if self.config.search_domains:
             query_list = [
-                query + " Site: " + str(i) for i in self.config.search_domains
+                self.formulate_site_search(query, str(i)) for i in self.config.search_domains
             ]
             if len(query_list) >= 5:
                 query_list = query_list[:5]
                 result = (
                     result
                     + "Warning: Only the first 5 URLs are taken into consideration.\n"
                 )  # noqa: E501
@@ -123,14 +123,17 @@
             else:
                 result += "\n" + cur_result
 
         if require_meta:
             result = (result, meta)
 
         return result
+    
+    def formulate_site_search(self, query: str, site: str) -> str:
+        return query + " site:" + site
 
     def _run_single_query(
         self, query: str, top_k: int, require_meta=False
     ) -> Union[str, Tuple[str, List[dict]]]:
         logger.debug(f"Search query: {query}")
         google_serper = GoogleSerperAPIWrapper()
         search_results = google_serper._google_serper_api_results(query)
```

### Comparing `sherpa_ai-0.2.0/sherpa_ai/utils.py` & `sherpa_ai-0.2.1/sherpa_ai/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/verbose_loggers.py` & `sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/verbose_loggers.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.0/PKG-INFO` & `sherpa_ai-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-ai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sherpa: AI-augmented thinking companion
 Home-page: https://github.com/Aggregate-Intellect/sherpa
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

